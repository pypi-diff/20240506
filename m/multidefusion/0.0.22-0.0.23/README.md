# Comparing `tmp/multidefusion-0.0.22.tar.gz` & `tmp/multidefusion-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.22.tar", last modified: Sun May  5 08:31:36 2024, max compression
+gzip compressed data, was "multidefusion-0.0.23.tar", last modified: Mon May  6 07:45:20 2024, max compression
```

## Comparing `multidefusion-0.0.22.tar` & `multidefusion-0.0.23.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 08:31:36.509057 multidefusion-0.0.22/
--rw-rw-rw-   0        0        0      154 2024-04-21 08:50:10.000000 multidefusion-0.0.22/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.22/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.22/MANIFEST.in
--rw-rw-rw-   0        0        0     2862 2024-05-05 08:31:36.509057 multidefusion-0.0.22/PKG-INFO
--rw-rw-rw-   0        0        0     1823 2024-04-24 19:38:47.000000 multidefusion-0.0.22/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 08:31:36.501517 multidefusion-0.0.22/multidefusion/
--rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.22/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    19080 2024-05-04 15:41:34.000000 multidefusion-0.0.22/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     3001 2024-05-05 08:16:55.000000 multidefusion-0.0.22/multidefusion/fusion.py
--rw-rw-rw-   0        0        0    26158 2024-05-05 08:17:29.000000 multidefusion-0.0.22/multidefusion/integration.py
--rw-rw-rw-   0        0        0    51964 2024-05-04 21:25:47.000000 multidefusion-0.0.22/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-05-05 08:31:36.509057 multidefusion-0.0.22/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     2862 2024-05-05 08:31:36.000000 multidefusion-0.0.22/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-05 08:31:36.000000 multidefusion-0.0.22/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       70 2024-05-05 08:31:36.000000 multidefusion-0.0.22/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.22/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-05-05 08:31:36.000000 multidefusion-0.0.22/multidefusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 08:31:36.000000 multidefusion-0.0.22/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       73 2024-04-26 08:15:06.000000 multidefusion-0.0.22/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-05-05 08:31:36.509057 multidefusion-0.0.22/setup.cfg
--rw-rw-rw-   0        0        0     1882 2024-05-05 08:26:57.000000 multidefusion-0.0.22/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 08:31:36.509057 multidefusion-0.0.22/tests/
--rw-rw-rw-   0        0        0      431 2024-04-25 16:58:41.000000 multidefusion-0.0.22/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:45:20.816307 multidefusion-0.0.23/
+-rw-rw-rw-   0        0        0      154 2024-04-21 08:50:10.000000 multidefusion-0.0.23/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.23/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.23/MANIFEST.in
+-rw-rw-rw-   0        0        0     2862 2024-05-06 07:45:20.816307 multidefusion-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     1823 2024-04-24 19:38:47.000000 multidefusion-0.0.23/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 07:45:20.800680 multidefusion-0.0.23/multidefusion/
+-rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.23/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0    19080 2024-05-04 15:41:34.000000 multidefusion-0.0.23/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     3001 2024-05-05 08:16:55.000000 multidefusion-0.0.23/multidefusion/fusion.py
+-rw-rw-rw-   0        0        0    26158 2024-05-05 08:17:29.000000 multidefusion-0.0.23/multidefusion/integration.py
+-rw-rw-rw-   0        0        0    51964 2024-05-04 21:25:47.000000 multidefusion-0.0.23/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:45:20.816307 multidefusion-0.0.23/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     2862 2024-05-06 07:45:20.000000 multidefusion-0.0.23/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-06 07:45:20.000000 multidefusion-0.0.23/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-05-06 07:45:20.000000 multidefusion-0.0.23/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.23/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-05-06 07:45:20.000000 multidefusion-0.0.23/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-06 07:45:20.000000 multidefusion-0.0.23/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-26 08:15:06.000000 multidefusion-0.0.23/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-05-06 07:45:20.816307 multidefusion-0.0.23/setup.cfg
+-rw-rw-rw-   0        0        0     1882 2024-05-06 07:44:08.000000 multidefusion-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:45:20.800680 multidefusion-0.0.23/tests/
+-rw-rw-rw-   0        0        0      431 2024-04-25 16:58:41.000000 multidefusion-0.0.23/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.22/LICENSE` & `multidefusion-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/PKG-INFO` & `multidefusion-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.22
+Version: 0.0.23
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.22/README.md` & `multidefusion-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/multidefusion/datainterface.py` & `multidefusion-0.0.23/multidefusion/datainterface.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/multidefusion/fusion.py` & `multidefusion-0.0.23/multidefusion/fusion.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/multidefusion/integration.py` & `multidefusion-0.0.23/multidefusion/integration.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/multidefusion/results.py` & `multidefusion-0.0.23/multidefusion/results.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.22/multidefusion.egg-info/PKG-INFO` & `multidefusion-0.0.23/multidefusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.22
+Version: 0.0.23
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.22/setup.py` & `multidefusion-0.0.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='multidefusion',
     name='multidefusion',
     packages=find_packages(include=['multidefusion', 'multidefusion.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/damiantondas/multidefusion',
-    version='0.0.22',
+    version='0.0.23',
     zip_safe=False,
 )
```

