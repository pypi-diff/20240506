# Comparing `tmp/msmanager-0.4.1.tar.gz` & `tmp/msmanager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.4.1.tar", max compression
+gzip compressed data, was "msmanager-0.4.2.tar", max compression
```

## Comparing `msmanager-0.4.1.tar` & `msmanager-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.1/msmanager/__main__.py
--rw-r--r--   0        0        0    14066 2024-05-06 08:43:39.542808 msmanager-0.4.1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.1/msmanager/config.py
--rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.1/msmanager/exceptions.py
--rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.1/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.1/msmanager/models.py
--rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.1/msmanager/types.py
--rw-r--r--   0        0        0      596 2024-05-06 08:43:49.094860 msmanager-0.4.1/msmanager/units.py
--rw-r--r--   0        0        0      662 2024-05-06 08:43:43.383850 msmanager-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.1/README.md
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.2/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.2/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.2/msmanager/__main__.py
+-rw-r--r--   0        0        0    14066 2024-05-06 08:47:53.779873 msmanager-0.4.2/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.2/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.2/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.2/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.2/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.2/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.2/msmanager/types.py
+-rw-r--r--   0        0        0      596 2024-05-06 08:48:08.480294 msmanager-0.4.2/msmanager/units.py
+-rw-r--r--   0        0        0      662 2024-05-06 08:48:04.492427 msmanager-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.2/README.md
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.2/PKG-INFO
```

### Comparing `msmanager-0.4.1/LICENSE` & `msmanager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/cli.py` & `msmanager-0.4.2/msmanager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
 # ? Watchdog
 @click.command("watchdog", help="The active process of monitoring servers, which, if the server fails, restarts it.")
 @click.argument("scn", type=str)
 @click.option(
     "--localhost", "-l", "localhost", 
     help="The ping will take place not by the host settings, but by the local IP.",
-    defalut=False, is_flag=True
+    default=False, is_flag=True
 )
 @click.option(
     "--start-delay", "-d", "start_delay",
     help="The delay before watchdog starts (in secounds).",
     type=click.INT, default=120, show_default=True
 )
 @hand_exception()
```

### Comparing `msmanager-0.4.1/msmanager/config.py` & `msmanager-0.4.2/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/exceptions.py` & `msmanager-0.4.2/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/functions.py` & `msmanager-0.4.2/msmanager/functions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/models.py` & `msmanager-0.4.2/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/msm.py` & `msmanager-0.4.2/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/msmanager/units.py` & `msmanager-0.4.2/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __prog_name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.4.1/pyproject.toml` & `msmanager-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.4.1"
+version = "0.4.2"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.4.1/README.md` & `msmanager-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.1/PKG-INFO` & `msmanager-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.4.1
+Version: 0.4.2
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

