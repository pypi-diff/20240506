# Comparing `tmp/getodo-2.0.0.tar.gz` & `tmp/getodo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getodo-2.0.0.tar", max compression
+gzip compressed data, was "getodo-2.0.1.tar", max compression
```

## Comparing `getodo-2.0.0.tar` & `getodo-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2024-04-30 17:03:44.134689 getodo-2.0.0/LICENSE
--rw-r--r--   0        0        0     2636 2024-04-30 17:03:44.134689 getodo-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/__main__.py
--rw-r--r--   0        0        0     6087 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo.py
--rw-r--r--   0        0        0      738 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo_cfg.json
--rw-r--r--   0        0        0     1768 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo_cli.py
--rw-r--r--   0        0        0     2098 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/utils.py
--rw-r--r--   0        0        0      410 2024-04-30 17:03:44.134689 getodo-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 getodo-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-06 09:05:48.262666 getodo-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3733 2024-05-06 09:05:48.262666 getodo-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/__main__.py
+-rw-r--r--   0        0        0     6087 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/getodo.py
+-rw-r--r--   0        0        0      738 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/getodo_cfg.json
+-rw-r--r--   0        0        0     1768 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/getodo_cli.py
+-rw-r--r--   0        0        0     2089 2024-05-06 09:05:48.262666 getodo-2.0.1/getodo/utils.py
+-rw-r--r--   0        0        0      410 2024-05-06 09:05:48.262666 getodo-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4277 1970-01-01 00:00:00.000000 getodo-2.0.1/PKG-INFO
```

### Comparing `getodo-2.0.0/LICENSE` & `getodo-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getodo-2.0.0/getodo/getodo.py` & `getodo-2.0.1/getodo/getodo.py`

 * *Files identical despite different names*

### Comparing `getodo-2.0.0/getodo/getodo_cfg.json` & `getodo-2.0.1/getodo/getodo_cfg.json`

 * *Files identical despite different names*

### Comparing `getodo-2.0.0/getodo/getodo_cli.py` & `getodo-2.0.1/getodo/getodo_cli.py`

 * *Files identical despite different names*

### Comparing `getodo-2.0.0/getodo/utils.py` & `getodo-2.0.1/getodo/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 def print_error(e: Exception | str) -> None:
     print(Fore.RED + Style.BRIGHT + "Encountered Error" + Style.RESET_ALL)
     print(e)
     exit(-1)
 
 
 def add_to_gitignore(parse_path: str, out_file: str) -> None:
-    # Assume .gitignore is in the root of the input_path
-    gitignore_root = path.abspath(path.dirname(parse_path))
+    # Assume .gitignore is in the directory of the parse_path
+    gitignore_root = path.abspath(parse_path)
     gitignore_file = path.join(gitignore_root, ".gitignore")
    
     if path.exists(gitignore_file):
         try:
             with open(gitignore_file, "r") as f:
                 lines = f.readlines()
                 for line in lines:
```

### Comparing `getodo-2.0.0/PKG-INFO` & `getodo-2.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: getodo
-Version: 2.0.0
-Summary: A python program to collect all your TODO(s)
-License: MIT
-Author: Vyshnav Vinod
-Author-email: vyshnav.vinod003@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Description-Content-Type: text/markdown
-
 # GETODO
 > A python program to collect all your TODO(s)
 
 `getodo` is a python program that collects all your TODO(s) from a folder/file and list them for you as a file or in the terminal screen. `getodo` makes it easy to keep track of your TODO(s)
 
 ## Installation
 
@@ -76,13 +60,16 @@
 
 `-o, --output` : Write to the file provided here. If no file is specified, the program will write to `todo.txt`
 
 `-t, --term` : Display the TODO's in the terminal with colors
 
 `-i, --ignore` : Ignore parsing the directories/files provided as arguments to this option
 
+## Additional Configurations
+
+Right now, `getodo` only supports editing the `getodo_cfg.json` directly to add some additional configs. In the future, a `-c,--config` command will be added so that anyone can add more configs(especially those who downloaded from `pip`). To add more comment syntax, change the default output file name, to add more default ignored folders and files and to even change the word to be parsed(i.e, If you want to parse comments beginning with `NOTE:` or `IMPORTANT:` , etc), go to `getodo_cfg.json` and add or remove the configs as you wish. Please note that you must stick to the given syntax or else the program will break. `getodo_cfg.json` can be found in the `getodo/` directory for those who cloned the repo. For those who installed via `pip`, please refer to this [link](https://stackoverflow.com/questions/29980798/where-does-pip-install-its-packages) and find out where the `getodo` folder is present and make your changes in there. You can always ask for help by raising an [issue](https://github.com/vyshnav-vinod/getodo/issues) and i will be glad to help.
+
 ## Contributing
 
 All contributions are welcome. You can submit a issue/bug or request for a feature or ask for help in the [issues](https://github.com/vyshnav-vinod/getodo/issues) tab.
 
 If you like to add a new feature or fix a bug, please checkout [CONTRIBUTING](https://github.com/vyshnav-vinod/getodo/blob/main/CONTRIBUTING.md) guidelines.
-
```

