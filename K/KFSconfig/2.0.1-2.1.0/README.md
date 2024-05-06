# Comparing `tmp/kfsconfig-2.0.1.tar.gz` & `tmp/kfsconfig-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.0.1.tar", max compression
+gzip compressed data, was "kfsconfig-2.1.0.tar", max compression
```

## Comparing `kfsconfig-2.0.1.tar` & `kfsconfig-2.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    14520 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15695 2024-05-06 13:12:53.821235 kfsconfig-2.1.0/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-06 13:12:53.821235 kfsconfig-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-06 13:12:53.821235 kfsconfig-2.1.0/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.0/PKG-INFO
```

### Comparing `kfsconfig-2.0.1/KFSconfig/KFSconfig.py` & `kfsconfig-2.1.0/KFSconfig/KFSconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,23 +64,24 @@
     Tries to load config with the name of the config_default's keys. Multiple sources can be used and will be prioritised accordingly:
     1. if env is True: passed environemental variables from os.environ
     2. if config_filepath is not None: config from file at filepath with decreasing priority
     If any setting is still None after all sources have been tried and setting_None_ok is false, it is considered undefined and a ValueError is raised.
     If any setting is undefined and none of the enabled filepaths exist, creation of a default config file at the highest priority filepath will be offered using config_default's values.
 
     Arguments:
-    - config_default: defaults to use for creation of a default config file
+    - config_default: defaults to use for creation of a default config file, unformatted file formats like .txt require key "content"
     - env: use passed environmental variables from os.environ?
-    - config_filepath: filepath to config files or None if unused
+    - config_filepath: filepath to config files or None if unused, formats depending on file extension, unformatted formats like .txt save raw string content from file in key "content"
     - setting_None_ok: allow settings to be None or require to be set?
 
     Returns:
     - config: loaded config, same keys as config_default
 
     Raises:
+    - KeyError: config_default is missing key "content" while trying to save raw string content
     - ValueError: After going through all enabled sources, a setting is still None and setting_None_ok is false.
     """
 
     config: dict[str, typing.Any]={key: None for key in config_default.keys()}  # loaded config, initialised empty with same keys as config_default
     
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
@@ -150,15 +151,15 @@
 
 
 def _load_config_file(config_filepath: str) -> dict[str, typing.Any]:
     """
     Loads a config file from the specified filepath and returns its content as a dictionary.
 
     Arguments:
-    - config_filepath: filepath to config file
+    - config_filepath: filepath to config file, interprets data depending on file extension, unformatted formats like .txt save raw string content from file in key "content"
 
     Returns:
     - config_filecontent: content of config file as a dictionary
 
     Raises:
     - FileNotFoundError: config_filepath does not exist
     - IsADirectoryError: config_filepath is a directory
@@ -184,14 +185,16 @@
     try:
         with open(config_filepath, "rt", encoding="utf8") as config_file:                                                                                                               # read file
             match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                                                                                                                 # parse file content
                 case "env":
                     config={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
                 case "json":
                     config=json.loads(config_file.read())                                                                                                                               # parse json
+                case "token" | "txt":
+                    config={"content": config_file.read()}                                                                                                                              # parse raw string
                 case _:
                     logger.critical(f"\rLoading \"{config_filepath}\" failed, because file extension is not implemented.")
                     raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file extension is not implemented.")
     except OSError as e:                                                                                                                                                                # write to log, then forward exception
         logger.error(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
@@ -202,19 +205,20 @@
 
 
 def _create_default_file(config_default: dict[str, typing.Any], config_filepath: str) -> None:
     """
     Creates a default config file at the specified filepath using config_default.
 
     Arguments:
-    - config_default: defaults to use for creation of a default config file
-    - config_filepath: filepath to config file
+    - config_default: defaults to use for creation of a default config file, unformatted file formats like .txt require key "content"
+    - config_filepath: filepath to config file, formats depending on file extension, unformatted formats like .txt save raw string value from key "content" in file
 
     Raises:
     - FileExistsError: config_filepath already exists
+    - KeyError: config_default is missing key "content" while trying to save raw string content
     - NotImplementedError: file extension is not implemented yet
     - OSError: creating config_filepath failed
     """
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
@@ -231,17 +235,22 @@
             os.makedirs(os.path.dirname(config_filepath), exist_ok=True)    # create directories
         with open(config_filepath, "wt", encoding="utf8") as config_file:   # create file
             match os.path.basename(config_filepath).rsplit(".", 1)[-1]:     # fill with default content
                 case "env":
                     config_file.write("\n".join([f"{k}={v}" for k, v in config_default.items()]))
                 case "json":
                     config_file.write(json.dumps(config_default, indent=4))
+                case "token" | "txt":
+                    config_file.write(config_default["content"])
                 case _:
                     logger.critical(f"\rCreating default \"{config_filepath}\" failed, because file extension is not implemented.")
                     raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Creating default \"{config_filepath}\" failed, because file extension is not implemented.")
+    except KeyError:
+        logger.error(f"\rCreating default \"{config_filepath}\" failed, because config_default is missing key \"content\".")
+        raise
     except OSError as e:
         logger.error(f"\rCreating default \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
         logger.info(f"\rCreated default \"{config_filepath}\".")
 
     return
```

### Comparing `kfsconfig-2.0.1/pyproject.toml` & `kfsconfig-2.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.0.1"
+version     = "2.1.0"
 
 [tool.poetry.dependencies]
-KFSlog = "^1.0.0"
+kfslog = "^1.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
 pytest     = "^7.0.0"
 
 [build-system]
```

### Comparing `kfsconfig-2.0.1/readme.md` & `kfsconfig-2.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.0.1/PKG-INFO` & `kfsconfig-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.0.1
+Version: 2.1.0
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: KFSlog (>=1.0.0,<2.0.0)
+Requires-Dist: kfslog (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSconfig
 Description-Content-Type: text/markdown
 
 ---
 Topic: "KFSconfig"
 Author: "구FS"
 ---
```

