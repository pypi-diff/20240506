# Comparing `tmp/machineroom-0.47.4.tar.gz` & `tmp/machineroom-0.47.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.47.4.tar", last modified: Wed May  1 18:19:15 2024, max compression
+gzip compressed data, was "machineroom-0.47.5.tar", last modified: Mon May  6 08:49:12 2024, max compression
```

## Comparing `machineroom-0.47.4.tar` & `machineroom-0.47.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-01 18:19:15.364379 machineroom-0.47.4/
--rw-r--r--   0 root         (0) staff       (20)     2370 2024-04-26 06:25:54.000000 machineroom-0.47.4/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4983 2024-05-01 18:19:15.364215 machineroom-0.47.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3852 2024-04-30 04:00:57.000000 machineroom-0.47.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-01 18:19:15.356278 machineroom-0.47.4/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.4/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-01 18:19:15.359959 machineroom-0.47.4/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10297 2024-04-26 07:21:15.000000 machineroom-0.47.4/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.4/machineroom/errs.py
--rw-r--r--   0 root         (0) staff       (20)     3682 2024-04-30 03:59:14.000000 machineroom-0.47.4/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.4/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14128 2024-04-26 07:27:26.000000 machineroom-0.47.4/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    30284 2024-04-30 03:53:47.000000 machineroom-0.47.4/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-01 18:19:15.363152 machineroom-0.47.4/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.4/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.4/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.4/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    17504 2024-05-01 18:18:50.000000 machineroom-0.47.4/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     7702 2024-04-26 07:27:26.000000 machineroom-0.47.4/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-01 18:19:15.363666 machineroom-0.47.4/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4983 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      534 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-05-01 18:19:15.000000 machineroom-0.47.4/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-05-01 18:19:15.364918 machineroom-0.47.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.4/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1534 2024-04-26 07:28:38.000000 machineroom-0.47.4/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-05-01 18:19:07.000000 machineroom-0.47.4/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-06 08:49:12.418002 machineroom-0.47.5/
+-rw-r--r--   0 root         (0) staff       (20)     2370 2024-04-26 06:25:54.000000 machineroom-0.47.5/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4983 2024-05-06 08:49:12.417658 machineroom-0.47.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3852 2024-04-30 04:00:57.000000 machineroom-0.47.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-06 08:49:12.393813 machineroom-0.47.5/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.5/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-06 08:49:12.407811 machineroom-0.47.5/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10297 2024-04-26 07:21:15.000000 machineroom-0.47.5/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.5/machineroom/errs.py
+-rw-r--r--   0 root         (0) staff       (20)     3682 2024-04-30 03:59:14.000000 machineroom-0.47.5/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.5/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14128 2024-04-26 07:27:26.000000 machineroom-0.47.5/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    30339 2024-05-05 04:50:00.000000 machineroom-0.47.5/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-06 08:49:12.414962 machineroom-0.47.5/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.5/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.5/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.5/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    17504 2024-05-01 18:18:50.000000 machineroom-0.47.5/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     7702 2024-04-26 07:27:26.000000 machineroom-0.47.5/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-06 08:49:12.416614 machineroom-0.47.5/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4983 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      534 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-05-06 08:49:12.000000 machineroom-0.47.5/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-05-06 08:49:12.419327 machineroom-0.47.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.5/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1534 2024-04-26 07:28:38.000000 machineroom-0.47.5/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-05-06 08:48:59.000000 machineroom-0.47.5/version
```

### Comparing `machineroom-0.47.4/.gitignore` & `machineroom-0.47.5/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/LICENSE` & `machineroom-0.47.5/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/PKG-INFO` & `machineroom-0.47.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.4
+Version: 0.47.5
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.4/README.md` & `machineroom-0.47.5/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/cmdbin/connect` & `machineroom-0.47.5/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/__init__.py` & `machineroom-0.47.5/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.47.4'
+__version__ = '0.47.5'
```

### Comparing `machineroom-0.47.4/machineroom/const.py` & `machineroom-0.47.5/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/infra.py` & `machineroom-0.47.5/machineroom/infra.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/schema.json` & `machineroom-0.47.5/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/sql.py` & `machineroom-0.47.5/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/taskbase.py` & `machineroom-0.47.5/machineroom/taskbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,21 @@
     finally:
         c.run("rm -f /tmp/id.pub /tmp/uniq.authorized_keys")
 
 
 def exists(c: Connection, path: str) -> bool:
     r = c.run(f'stat {path}', warn=True, pty=True, hide=True)
     line = str(r.stdout.strip().replace("\n", ""))
+    if "没有那个文件或目录" in line:
+        return False
+
     if "No such file or directory" in line:
         return False
-    else:
-        return True
+
+    return True
 
 
 def docker_version_checker(r: Result):
     line = str(r.stdout.strip().replace("\n", ""))
     if "Docker version" not in line:
         raise DockerAccessProblem("docker is not installed or may have permission problem")
     # Extract the version number
```

### Comparing `machineroom-0.47.4/machineroom/tunnels/conn.py` & `machineroom-0.47.5/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/util.py` & `machineroom-0.47.5/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom/worker.py` & `machineroom-0.47.5/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/machineroom.egg-info/PKG-INFO` & `machineroom-0.47.5/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.4
+Version: 0.47.5
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.4/machineroom.egg-info/SOURCES.txt` & `machineroom-0.47.5/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/setup.py` & `machineroom-0.47.5/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.4/update` & `machineroom-0.47.5/update`

 * *Files identical despite different names*

