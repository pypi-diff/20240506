# Comparing `tmp/scdistrank-0.0.0.2.tar.gz` & `tmp/scdistrank-0.0.0.3.tar.gz`

## Comparing `scdistrank-0.0.0.2.tar` & `scdistrank-0.0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/license.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/src/scDistRank/__init__.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/src/scDistRank/searchOptimal.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/src/scDistRank/visualization.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/.gitignore
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/README.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 scdistrank-0.0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/license.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/src/scDistRank/__init__.py
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/src/scDistRank/searchOptimal.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/src/scDistRank/visualization.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/.gitignore
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scdistrank-0.0.0.3/PKG-INFO
```

### Comparing `scdistrank-0.0.0.2/license.txt` & `scdistrank-0.0.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `scdistrank-0.0.0.2/src/scDistRank/searchOptimal.py` & `scdistrank-0.0.0.3/src/scDistRank/searchOptimal.py`

 * *Files identical despite different names*

### Comparing `scdistrank-0.0.0.2/src/scDistRank/visualization.py` & `scdistrank-0.0.0.3/src/scDistRank/visualization.py`

 * *Files identical despite different names*

### Comparing `scdistrank-0.0.0.2/pyproject.toml` & `scdistrank-0.0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scDistRank"
-version = "0.0.0.2"
+version = "0.0.0.3"
 authors = [
   { name="Tyler Jost", email="tyler_jost@utexas.edu" },
 ]
 dependencies = [
     "scanpy>=1.9.8",
     "scipy>=1.12.0",
-    "matplotlib-base>=3.8.2",
+    "matplotlib>=3.8",
     "numpy>=1.26.3",
     "seaborn>=0.13.2",
     "tqdm>=4.66.1",
     "pandas>=2.2.0"
 ]
 description = "Separate your clusters with gene distance"
 readme = "README.md"
@@ -24,8 +24,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/brocklab/scDistRank"
-Issues =   "https://github.com/brocklab/scDistRank/issues"
+Issues =   "https://github.com/brocklab/scDistRank/issues"
```

### Comparing `scdistrank-0.0.0.2/PKG-INFO` & `scdistrank-0.0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.3
 Name: scDistRank
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Separate your clusters with gene distance
 Project-URL: Homepage, https://github.com/brocklab/scDistRank
 Project-URL: Issues, https://github.com/brocklab/scDistRank/issues
 Author-email: Tyler Jost <tyler_jost@utexas.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: matplotlib-base>=3.8.2
+Requires-Dist: matplotlib>=3.8
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: scanpy>=1.9.8
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: tqdm>=4.66.1
 Description-Content-Type: text/markdown
 
 # scDistRank
-matplotlib
```

