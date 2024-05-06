# Comparing `tmp/kfsconfig-2.0.0.tar.gz` & `tmp/kfsconfig-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.0.0.tar", max compression
+gzip compressed data, was "kfsconfig-2.0.1.tar", max compression
```

## Comparing `kfsconfig-2.0.0.tar` & `kfsconfig-2.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13919 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    14520 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-06 12:26:27.526300 kfsconfig-2.0.1/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.0.1/PKG-INFO
```

### Comparing `kfsconfig-2.0.0/KFSconfig/KFSconfig.py` & `kfsconfig-2.0.1/KFSconfig/KFSconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     
     if config_filepaths!=None and len(config_filepaths)!=0:
         for config_filepath in config_filepaths:
             try:
                 config.update({k: v for k, v in _load_config_file(config_filepath).items() if k in config.keys() and config[k]==None})  # update config with config file, only overwrite if key already exists and value is None
             except (FileNotFoundError, IsADirectoryError):                                                                              # if fails: ignore source
                 pass
+    logger.debug(f"Loaded all config sources.")
+    logger.debug(config)
 
 
     if any(v==None for v in config.values())==True and setting_None_ok==False:                                                                                  # if any setting is still None and not allowed to be None: error
         logger.error(f"After going through all enabled sources, settings {[k for k, v in config.items() if v==None]} are still None and setting_None_ok is false.")
         
         if config_filepaths!=None and 1<=len(config_filepaths) and all([os.path.exists(config_filepath)==False for config_filepath in config_filepaths])==True: # if a file source is enabled and no files at set filepaths exist: offer creation of default config file at highest priority filepath using config_default's values
             logger.info(f"None of the following filepaths exist: {config_filepaths}")
@@ -126,15 +128,29 @@
     """
     Loads the passed environmental variables from os.environ and returns them as a dictionary.
 
     Returns:
     - passed environmental variables from os.environ
     """
 
-    return dict(os.environ)
+    config: dict[str, typing.Any]   # passed environmental variables
+
+
+    if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
+        logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
+    else:                                       # if no root logger defined:
+        logger=KFSlog.setup_logging("KFS")      # use KFS default format
+
+
+    logger.info(f"Loading environmental variables...")
+    config=dict(os.environ) # load environmental variables
+    logger.info(f"\rLoaded environmental variables.")
+    logger.debug(config)
+
+    return config
 
 
 def _load_config_file(config_filepath: str) -> dict[str, typing.Any]:
     """
     Loads a config file from the specified filepath and returns its content as a dictionary.
 
     Arguments:
@@ -144,15 +160,15 @@
     - config_filecontent: content of config file as a dictionary
 
     Raises:
     - FileNotFoundError: config_filepath does not exist
     - IsADirectoryError: config_filepath is a directory
     """
 
-    config_filecontent: dict[str, typing.Any]   # content of config file
+    config: dict[str, typing.Any]   # config file
 
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
@@ -162,30 +178,31 @@
     if os.path.isdir(config_filepath)==True:    # if config file is a directory: error
         logger.error(f"Loading \"{config_filepath}\" failed, because it is a directory.")
         raise IsADirectoryError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because it is a directory.")
 
 
     logger.info(f"Loading \"{config_filepath}\"...")
     try:
-        with open(config_filepath, "rt", encoding="utf8") as config_file:                                                                                                                           # read file
-            match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                                                                                                                             # parse file content
+        with open(config_filepath, "rt", encoding="utf8") as config_file:                                                                                                               # read file
+            match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                                                                                                                 # parse file content
                 case "env":
-                    config_filecontent={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
+                    config={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
                 case "json":
-                    config_filecontent=json.loads(config_file.read())                                                                                                                               # parse json
+                    config=json.loads(config_file.read())                                                                                                                               # parse json
                 case _:
                     logger.critical(f"\rLoading \"{config_filepath}\" failed, because file extension is not implemented.")
                     raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file extension is not implemented.")
-    except OSError as e:                                                                                                                                                                            # write to log, then forward exception
+    except OSError as e:                                                                                                                                                                # write to log, then forward exception
         logger.error(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
         logger.info(f"\rLoaded \"{config_filepath}\".")
+        logger.debug(config)
     
-    return config_filecontent
+    return config
 
 
 def _create_default_file(config_default: dict[str, typing.Any], config_filepath: str) -> None:
     """
     Creates a default config file at the specified filepath using config_default.
 
     Arguments:
@@ -221,10 +238,10 @@
                 case _:
                     logger.critical(f"\rCreating default \"{config_filepath}\" failed, because file extension is not implemented.")
                     raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Creating default \"{config_filepath}\" failed, because file extension is not implemented.")
     except OSError as e:
         logger.error(f"\rCreating default \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
-        logger.info(f"\rCreated default \"{config_filepath}\".")    
+        logger.info(f"\rCreated default \"{config_filepath}\".")
 
     return
```

### Comparing `kfsconfig-2.0.0/pyproject.toml` & `kfsconfig-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.0.0"
+version     = "2.0.1"
 
 [tool.poetry.dependencies]
 KFSlog = "^1.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
```

### Comparing `kfsconfig-2.0.0/readme.md` & `kfsconfig-2.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.0.0/PKG-INFO` & `kfsconfig-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

