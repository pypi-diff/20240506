# Comparing `tmp/oslactionspotting-0.1.0.tar.gz` & `tmp/oslactionspotting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslactionspotting-0.1.0.tar", last modified: Wed May  1 12:44:32 2024, max compression
+gzip compressed data, was "oslactionspotting-0.1.2.tar", last modified: Mon May  6 17:53:30 2024, max compression
```

## Comparing `oslactionspotting-0.1.0.tar` & `oslactionspotting-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:44:32.280169 oslactionspotting-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:44:24.000000 oslactionspotting-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-01 12:44:32.280169 oslactionspotting-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-01 12:44:24.000000 oslactionspotting-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:44:32.280169 oslactionspotting-0.1.0/oslactionspotting/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-01 12:44:24.000000 oslactionspotting-0.1.0/oslactionspotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:44:32.280169 oslactionspotting-0.1.0/oslactionspotting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-01 12:44:32.000000 oslactionspotting-0.1.0/oslactionspotting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 12:44:32.000000 oslactionspotting-0.1.0/oslactionspotting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:44:32.000000 oslactionspotting-0.1.0/oslactionspotting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 12:44:32.000000 oslactionspotting-0.1.0/oslactionspotting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 12:44:32.000000 oslactionspotting-0.1.0/oslactionspotting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-01 12:44:32.280169 oslactionspotting-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-01 12:44:24.000000 oslactionspotting-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:29.997608 oslactionspotting-0.1.2/oslactionspotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/oslactionspotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/oslactionspotting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 17:53:29.000000 oslactionspotting-0.1.2/oslactionspotting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:53:30.001608 oslactionspotting-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 17:53:21.000000 oslactionspotting-0.1.2/tests/test_simple.py
```

### Comparing `oslactionspotting-0.1.0/LICENSE` & `oslactionspotting-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oslactionspotting-0.1.0/PKG-INFO` & `oslactionspotting-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oslactionspotting
-Version: 0.1.0
+Version: 0.1.2
 Summary: Action Spotting SDK
-Home-page: https://github.com/SoccerNet/sn-spotting-pip
+Home-page: https://github.com/OpenSportsLab/OSL-ActionSpotting
 Author: ['Silvio Giancola', 'Yassine Benzakour']
 Author-email: ['silvio.giancola@kaust.edu.sa', 'yassine.benzakour@student.uliege.be']
 License: MIT
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `oslactionspotting-0.1.0/README.md` & `oslactionspotting-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oslactionspotting-0.1.0/oslactionspotting.egg-info/PKG-INFO` & `oslactionspotting-0.1.2/oslactionspotting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oslactionspotting
-Version: 0.1.0
+Version: 0.1.2
 Summary: Action Spotting SDK
-Home-page: https://github.com/SoccerNet/sn-spotting-pip
+Home-page: https://github.com/OpenSportsLab/OSL-ActionSpotting
 Author: ['Silvio Giancola', 'Yassine Benzakour']
 Author-email: ['silvio.giancola@kaust.edu.sa', 'yassine.benzakour@student.uliege.be']
 License: MIT
 Keywords: SoccerNet,SDK,Spotting,Football,Soccer,Video
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `oslactionspotting-0.1.0/setup.py` & `oslactionspotting-0.1.2/setup.py`

 * *Files identical despite different names*

