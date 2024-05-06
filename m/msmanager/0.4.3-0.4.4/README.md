# Comparing `tmp/msmanager-0.4.3.tar.gz` & `tmp/msmanager-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.4.3.tar", max compression
+gzip compressed data, was "msmanager-0.4.4.tar", max compression
```

## Comparing `msmanager-0.4.3.tar` & `msmanager-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.3/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.3/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.3/msmanager/__main__.py
--rw-r--r--   0        0        0    14094 2024-05-06 08:59:39.356673 msmanager-0.4.3/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.3/msmanager/config.py
--rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.3/msmanager/exceptions.py
--rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.3/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.3/msmanager/models.py
--rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.3/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.3/msmanager/types.py
--rw-r--r--   0        0        0      596 2024-05-06 08:59:44.356054 msmanager-0.4.3/msmanager/units.py
--rw-r--r--   0        0        0      662 2024-05-06 08:59:47.678660 msmanager-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.3/README.md
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.4/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.4/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.4/msmanager/__main__.py
+-rw-r--r--   0        0        0    14335 2024-05-06 09:05:55.101396 msmanager-0.4.4/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.4/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.4/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.4/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.4/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.4/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.4/msmanager/types.py
+-rw-r--r--   0        0        0      596 2024-05-06 09:05:06.485027 msmanager-0.4.4/msmanager/units.py
+-rw-r--r--   0        0        0      662 2024-05-06 09:05:01.710207 msmanager-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.4/README.md
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.4/PKG-INFO
```

### Comparing `msmanager-0.4.3/LICENSE` & `msmanager-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/cli.py` & `msmanager-0.4.4/msmanager/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,17 @@
     time.sleep(start_delay)
     console.print("[green]>[/green] Watchdog is started!")
     try:
         while True:
             for server_config in servers_config:
                 if not pingok("localhost" if localhost else server_config.host, server_config.port):
                     msmanager.restart_server(server_config.screen_name)
+                    wait_start_server(server_config.host, server_config.port, server_config.input_port)
+                    console.print(f"[red]>[/red] Server is restarted: {repr(server_config.screen_name)}")
+            time.sleep(0.1)
     except KeyboardInterrupt:
         pass
     console.print("[green]>[/green] Watchdog is shutdown!")
 
 # ! Main Group
 @click.group()
 @click.option(
```

### Comparing `msmanager-0.4.3/msmanager/config.py` & `msmanager-0.4.4/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/exceptions.py` & `msmanager-0.4.4/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/functions.py` & `msmanager-0.4.4/msmanager/functions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/models.py` & `msmanager-0.4.4/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/msm.py` & `msmanager-0.4.4/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/msmanager/units.py` & `msmanager-0.4.4/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __prog_name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.4.3/pyproject.toml` & `msmanager-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.4.3"
+version = "0.4.4"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.4.3/README.md` & `msmanager-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.3/PKG-INFO` & `msmanager-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.4.3
+Version: 0.4.4
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

