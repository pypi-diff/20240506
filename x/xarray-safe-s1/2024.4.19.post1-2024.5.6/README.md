# Comparing `tmp/xarray_safe_s1-2024.4.19.post1.tar.gz` & `tmp/xarray_safe_s1-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_safe_s1-2024.4.19.post1.tar", last modified: Fri Apr 19 09:39:28 2024, max compression
+gzip compressed data, was "xarray_safe_s1-2024.5.6.tar", last modified: Mon May  6 12:40:39 2024, max compression
```

## Comparing `xarray_safe_s1-2024.4.19.post1.tar` & `xarray_safe_s1-2024.5.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.413893 xarray_safe_s1-2024.4.19.post1/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.405893 xarray_safe_s1-2024.4.19.post1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.405893 xarray_safe_s1-2024.4.19.post1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-19 09:39:28.413893 xarray_safe_s1-2024.4.19.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.405893 xarray_safe_s1-2024.4.19.post1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.405893 xarray_safe_s1-2024.4.19.post1/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.405893 xarray_safe_s1-2024.4.19.post1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/highleveltests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/highleveltests/open_SLC_IW.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/highleveltests/open_SLC_IW_S3.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/getconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    28974 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    52508 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:39:28.413893 xarray_safe_s1-2024.4.19.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.409893 xarray_safe_s1-2024.4.19.post1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-19 09:39:16.000000 xarray_safe_s1-2024.4.19.post1/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:39:28.413893 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-19 09:39:28.000000 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 09:39:28.000000 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:39:28.000000 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 09:39:28.000000 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 09:39:28.000000 xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.198913 xarray_safe_s1-2024.5.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.198913 xarray_safe_s1-2024.5.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/highleveltests/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW_S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/getconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29089 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52508 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray_safe_s1-2024.4.19.post1/.github/workflows/publish.yml` & `xarray_safe_s1-2024.5.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/.pre-commit-config.yaml` & `xarray_safe_s1-2024.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/LICENSE` & `xarray_safe_s1-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/PKG-INFO` & `xarray_safe_s1-2024.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.4.19.post1
+Version: 2024.5.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `xarray_safe_s1-2024.4.19.post1/README.md` & `xarray_safe_s1-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/ci/requirements/environment.yaml` & `xarray_safe_s1-2024.5.6/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/Makefile` & `xarray_safe_s1-2024.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/conf.py` & `xarray_safe_s1-2024.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/examples/simple_tutorial.ipynb` & `xarray_safe_s1-2024.5.6/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/index.rst` & `xarray_safe_s1-2024.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/installing.rst` & `xarray_safe_s1-2024.5.6/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/docs/make.bat` & `xarray_safe_s1-2024.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/highleveltests/open_SLC_IW_S3.py` & `xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW_S3.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/pyproject.toml` & `xarray_safe_s1-2024.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/safe_s1/getconfig.py` & `xarray_safe_s1-2024.5.6/safe_s1/getconfig.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/safe_s1/reader.py` & `xarray_safe_s1-2024.5.6/safe_s1/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             # windows might have semicolon in path ('c:\...')
             name_parts[1] = ':'.join(name_parts[1:-1])
             del name_parts[2:-1]
         name_parts[1] = os.path.basename(name_parts[1])
         self.short_name = ':'.join(name_parts)
         """Like name, but without path"""
         self.path = ':'.join(self.name.split(':')[1:-1])
+        # remove trailing slash in the safe path
+        if self.path[-1]=='/':
+            self.path = self.path.rstrip('/')
         """Dataset path"""
         self.safe = os.path.basename(self.path)
 
         self.path = os.fspath(self.path)
 
         if backend_kwargs is None:
             backend_kwargs = {}
@@ -105,15 +108,15 @@
                 'antenna_pattern':self.antenna_pattern,
                 'swath_merging': self.swath_merging
             }
             self.dt = datatree.DataTree.from_dict(self._dict)
             assert self.dt==self.datatree
         else:
             print('multidataset')
-            raise Exception()
+            # raise Exception()
 
     def load_digital_number(self, resolution=None, chunks=None, resampling=rasterio.enums.Resampling.rms):
         """
         load digital_number from self.sar_meta.files['measurement'], as an `xarray.Dataset`.
 
         Parameters
         ----------
@@ -515,15 +518,14 @@
         if 'GRD' in self.product:
             
             ds =  self.xml_parser.get_compound_var(self.files['annotation'].iloc[0], 'swath_merging')
             ds.attrs['history'] = self.xml_parser.get_compound_var(self.files['annotation'].iloc[0], 'swath_merging',
                                                                describe=True)
         else :
             ds = xr.Dataset()
-            
         return ds
 
     @property
     def multidataset(self):
         """
         Alias to `Sentinel1Reader._multidataset`
```

### Comparing `xarray_safe_s1-2024.4.19.post1/safe_s1/sentinel1_xml_mappings.py` & `xarray_safe_s1-2024.5.6/safe_s1/sentinel1_xml_mappings.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/safe_s1/xml_parser.py` & `xarray_safe_s1-2024.5.6/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/test/test_s1reader.py` & `xarray_safe_s1-2024.5.6/test/test_s1reader.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/PKG-INFO` & `xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.4.19.post1
+Version: 2024.5.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `xarray_safe_s1-2024.4.19.post1/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

