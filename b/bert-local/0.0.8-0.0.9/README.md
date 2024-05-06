# Comparing `tmp/bert_local-0.0.8.tar.gz` & `tmp/bert-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_local-0.0.8.tar", last modified: Sun Nov 12 11:03:04 2023, max compression
+gzip compressed data, was "bert-local-0.0.9.tar", last modified: Sun Nov 12 16:09:01 2023, max compression
```

## Comparing `bert_local-0.0.8.tar` & `bert-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 11:03:04.943466 bert_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-12 11:03:04.943466 bert_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-12 11:00:25.000000 bert_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 11:03:04.939466 bert_local-0.0.8/bert_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 11:03:04.943466 bert_local-0.0.8/bert_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 11:00:25.000000 bert_local-0.0.8/bert_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-11-12 11:00:25.000000 bert_local-0.0.8/bert_local/src/bert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 11:03:04.943466 bert_local-0.0.8/bert_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-12 11:03:04.000000 bert_local-0.0.8/bert_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-12 11:03:04.000000 bert_local-0.0.8/bert_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 11:03:04.000000 bert_local-0.0.8/bert_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-12 11:03:04.000000 bert_local-0.0.8/bert_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-12 11:03:04.000000 bert_local-0.0.8/bert_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-11-12 11:00:25.000000 bert_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-12 11:03:04.943466 bert_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-12 11:00:25.000000 bert_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 16:09:01.815230 bert-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-12 16:09:01.815230 bert-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-12 16:06:14.000000 bert-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 16:09:01.811230 bert-local-0.0.9/bert_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 16:09:01.815230 bert-local-0.0.9/bert_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 16:06:14.000000 bert-local-0.0.9/bert_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-11-12 16:06:14.000000 bert-local-0.0.9/bert_local/src/bert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 16:09:01.811230 bert-local-0.0.9/bert_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-12 16:09:01.000000 bert-local-0.0.9/bert_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-12 16:09:01.000000 bert-local-0.0.9/bert_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 16:09:01.000000 bert-local-0.0.9/bert_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-12 16:09:01.000000 bert-local-0.0.9/bert_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-12 16:09:01.000000 bert-local-0.0.9/bert_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2023-11-12 16:06:14.000000 bert-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-12 16:09:01.815230 bert-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-12 16:06:14.000000 bert-local-0.0.9/setup.py
```

### Comparing `bert_local-0.0.8/PKG-INFO` & `bert-local-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: bert_local
-Version: 0.0.8
+Name: bert-local
+Version: 0.0.9
 Summary: PyPI Package for Circles Local Bert Python
-Home-page: https://github.com/circles-zone/bert_local-python-package
+Home-page: https://github.com/circles-zone/bert-local-python-package
 Author: Circlez
 Author-email: info@circles.zone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: pytest>=7.4.3
 Requires-Dist: logger-local>=0.0.71
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: torch>=2.1.0
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: pandas>=2.1.2
 
-This is a package for sharing common Logger function used in different repositories
+# python-backend-template
```

### Comparing `bert_local-0.0.8/bert_local/src/bert.py` & `bert-local-0.0.9/bert_local/src/bert.py`

 * *Files identical despite different names*

### Comparing `bert_local-0.0.8/bert_local.egg-info/PKG-INFO` & `bert-local-0.0.9/bert_local.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bert-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles Local Bert Python
-Home-page: https://github.com/circles-zone/bert_local-python-package
+Home-page: https://github.com/circles-zone/bert-local-python-package
 Author: Circlez
 Author-email: info@circles.zone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: pytest>=7.4.3
 Requires-Dist: logger-local>=0.0.71
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: torch>=2.1.0
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: pandas>=2.1.2
 
-This is a package for sharing common Logger function used in different repositories
+# python-backend-template
```

### Comparing `bert_local-0.0.8/pyproject.toml` & `bert-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bert_local-0.0.8/setup.py` & `bert-local-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
-PACKAGE_NAME = "bert_local"
+PACKAGE_NAME = "bert-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
      name=PACKAGE_NAME,  
-     version='0.0.8',
+     version='0.0.9',
      author="Circlez",
      author_email="info@circles.zone",
      description="PyPI Package for Circles Local Bert Python",
-     long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
      packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
+    long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[ 
         'python-dotenv>=1.0.0',
```

