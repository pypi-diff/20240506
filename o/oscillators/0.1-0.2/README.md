# Comparing `tmp/oscillators-0.1.tar.gz` & `tmp/oscillators-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscillators-0.1.tar", last modified: Mon May  6 06:12:31 2024, max compression
+gzip compressed data, was "oscillators-0.2.tar", last modified: Mon May  6 06:22:07 2024, max compression
```

## Comparing `oscillators-0.1.tar` & `oscillators-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:12:31.804582 oscillators-0.1/
--rw-rw-rw-   0        0        0     1307 2024-05-06 06:08:31.000000 oscillators-0.1/.gitignore
--rw-rw-rw-   0        0        0      525 2024-05-06 06:12:31.804582 oscillators-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5048 2024-05-06 06:08:31.000000 oscillators-0.1/README.md
--rw-rw-rw-   0        0        0       60 2024-05-06 06:08:58.000000 oscillators-0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:12:31.803584 oscillators-0.1/oscillators.egg-info/
--rw-rw-rw-   0        0        0      525 2024-05-06 06:12:31.000000 oscillators-0.1/oscillators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-06 06:12:31.000000 oscillators-0.1/oscillators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:12:31.000000 oscillators-0.1/oscillators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-06 06:12:31.000000 oscillators-0.1/oscillators.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:12:31.000000 oscillators-0.1/oscillators.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 06:12:31.804582 oscillators-0.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-06 06:11:14.000000 oscillators-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:22:07.381073 oscillators-0.2/
+-rw-rw-rw-   0        0        0     1307 2024-05-06 06:08:31.000000 oscillators-0.2/.gitignore
+-rw-rw-rw-   0        0        0      525 2024-05-06 06:22:07.380065 oscillators-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5048 2024-05-06 06:08:31.000000 oscillators-0.2/README.md
+-rw-rw-rw-   0        0        0       61 2024-05-06 06:19:39.000000 oscillators-0.2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:22:07.378798 oscillators-0.2/oscillators.egg-info/
+-rw-rw-rw-   0        0        0      525 2024-05-06 06:22:07.000000 oscillators-0.2/oscillators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-06 06:22:07.000000 oscillators-0.2/oscillators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:22:07.000000 oscillators-0.2/oscillators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-06 06:22:07.000000 oscillators-0.2/oscillators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:22:07.000000 oscillators-0.2/oscillators.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:22:07.381073 oscillators-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-06 06:21:57.000000 oscillators-0.2/setup.py
```

### Comparing `oscillators-0.1/.gitignore` & `oscillators-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oscillators-0.1/PKG-INFO` & `oscillators-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscillators
-Version: 0.1
+Version: 0.2
 Summary: A package for simulating oscillators
 Home-page: https://github.com/Pradeep-Kumar-Rebbavarapu/CS-208-PROJECT-ODE-GRAPHER/module/oscillators.py
 Author: Pradeep Kumar Rebbavarapu
 Author-email: rpkiit2022@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oscillators-0.1/README.md` & `oscillators-0.2/README.md`

 * *Files identical despite different names*

### Comparing `oscillators-0.1/oscillators.egg-info/PKG-INFO` & `oscillators-0.2/oscillators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscillators
-Version: 0.1
+Version: 0.2
 Summary: A package for simulating oscillators
 Home-page: https://github.com/Pradeep-Kumar-Rebbavarapu/CS-208-PROJECT-ODE-GRAPHER/module/oscillators.py
 Author: Pradeep Kumar Rebbavarapu
 Author-email: rpkiit2022@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oscillators-0.1/setup.py` & `oscillators-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="oscillators",
-    version="0.1",
+    version="0.2",
     author="Pradeep Kumar Rebbavarapu",
     author_email="rpkiit2022@gmail.com",
     description="A package for simulating oscillators",
     long_description='kuramoto oscillator package',
     long_description_content_type="text/markdown",
     url="https://github.com/Pradeep-Kumar-Rebbavarapu/CS-208-PROJECT-ODE-GRAPHER/module/oscillators.py",
     packages=find_packages(),
```

