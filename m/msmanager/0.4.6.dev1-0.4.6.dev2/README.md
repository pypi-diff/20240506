# Comparing `tmp/msmanager-0.4.6.dev1.tar.gz` & `tmp/msmanager-0.4.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.4.6.dev1.tar", max compression
+gzip compressed data, was "msmanager-0.4.6.dev2.tar", max compression
```

## Comparing `msmanager-0.4.6.dev1.tar` & `msmanager-0.4.6.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.6.dev1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.6.dev1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.6.dev1/msmanager/__main__.py
--rw-r--r--   0        0        0    15407 2024-05-06 13:26:25.644413 msmanager-0.4.6.dev1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.6.dev1/msmanager/config.py
--rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.6.dev1/msmanager/exceptions.py
--rw-r--r--   0        0        0     4190 2024-05-06 13:11:57.556601 msmanager-0.4.6.dev1/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-05-06 12:56:09.812783 msmanager-0.4.6.dev1/msmanager/models.py
--rw-r--r--   0        0        0     3232 2024-05-06 12:57:54.532626 msmanager-0.4.6.dev1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.6.dev1/msmanager/types.py
--rw-r--r--   0        0        0      601 2024-05-06 13:23:54.511899 msmanager-0.4.6.dev1/msmanager/units.py
--rw-r--r--   0        0        0      667 2024-05-06 13:24:03.427458 msmanager-0.4.6.dev1/pyproject.toml
--rw-r--r--   0        0        0      928 2024-05-06 09:35:49.035878 msmanager-0.4.6.dev1/README.md
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 msmanager-0.4.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.6.dev2/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.6.dev2/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.6.dev2/msmanager/__main__.py
+-rw-r--r--   0        0        0    15407 2024-05-06 13:31:06.653571 msmanager-0.4.6.dev2/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.6.dev2/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.6.dev2/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4190 2024-05-06 13:11:57.556601 msmanager-0.4.6.dev2/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-05-06 12:56:09.812783 msmanager-0.4.6.dev2/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-06 12:57:54.532626 msmanager-0.4.6.dev2/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.6.dev2/msmanager/types.py
+-rw-r--r--   0        0        0      601 2024-05-06 13:31:15.774560 msmanager-0.4.6.dev2/msmanager/units.py
+-rw-r--r--   0        0        0      667 2024-05-06 13:31:19.417718 msmanager-0.4.6.dev2/pyproject.toml
+-rw-r--r--   0        0        0      928 2024-05-06 09:35:49.035878 msmanager-0.4.6.dev2/README.md
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 msmanager-0.4.6.dev2/PKG-INFO
```

### Comparing `msmanager-0.4.6.dev1/LICENSE` & `msmanager-0.4.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/cli.py` & `msmanager-0.4.6.dev2/msmanager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,16 +386,16 @@
 )
 @hand_exception()
 def main(
     check_environment: bool,
     debug: bool,
     output_format: Literal['text', 'json']
 ):
-    global msmanager, debag_mode, oformat
-    debag_mode, oformat = debug, output_format
+    global msmanager, debug_mode, oformat
+    debug_mode, oformat = debug, output_format
     msmanager = MSManager(check_environment=check_environment)
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
 main.add_command(stoper)
```

### Comparing `msmanager-0.4.6.dev1/msmanager/config.py` & `msmanager-0.4.6.dev2/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/exceptions.py` & `msmanager-0.4.6.dev2/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/functions.py` & `msmanager-0.4.6.dev2/msmanager/functions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/models.py` & `msmanager-0.4.6.dev2/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/msm.py` & `msmanager-0.4.6.dev2/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/msmanager/units.py` & `msmanager-0.4.6.dev2/msmanager/units.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __prog_name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.4.6.dev1"
+__version__ = "0.4.6.dev2"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.4.6.dev1/pyproject.toml` & `msmanager-0.4.6.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.4.6.dev1"
+version = "0.4.6.dev2"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.4.6.dev1/README.md` & `msmanager-0.4.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev1/PKG-INFO` & `msmanager-0.4.6.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.4.6.dev1
+Version: 0.4.6.dev2
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

