# Comparing `tmp/dynabench-0.3.0.tar.gz` & `tmp/dynabench-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynabench-0.3.0.tar", max compression
+gzip compressed data, was "dynabench-0.3.1.tar", max compression
```

## Comparing `dynabench-0.3.0.tar` & `dynabench-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,29 @@
--rw-r--r--   0        0        0     1074 2024-04-19 07:42:53.501591 dynabench-0.3.0/LICENCE
--rw-r--r--   0        0        0    18657 2024-04-19 07:42:53.501591 dynabench-0.3.0/LICENCE_data
--rw-r--r--   0        0        0    11415 2024-04-19 15:34:38.150726 dynabench-0.3.0/README.md
--rw-r--r--   0        0        0      822 2024-04-19 15:31:13.754053 dynabench-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/_init_.py
--rw-r--r--   0        0        0      266 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/__init__.py
--rw-r--r--   0        0        0      504 2024-04-19 07:45:03.504922 dynabench-0.3.0/src/dynabench/dataset/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8924 2024-04-19 07:45:03.504922 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc
--rw-r--r--   0        0        0     5826 2024-04-19 07:45:03.518256 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc
--rw-r--r--   0        0        0     4744 2024-04-19 07:45:03.541589 dynabench-0.3.0/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc
--rw-r--r--   0        0        0     6087 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_download.py
--rw-r--r--   0        0        0     3119 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_iterator.py
--rw-r--r--   0        0        0     2466 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/dataset/_simulation_iterator.py
--rw-r--r--   0        0        0      201 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/__init__.py
--rw-r--r--   0        0        0      457 2024-04-19 14:58:43.960657 dynabench-0.3.0/src/dynabench/equation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2024-04-19 07:45:03.501589 dynabench-0.3.0/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc
--rw-r--r--   0        0        0     2662 2024-04-19 07:45:03.344923 dynabench-0.3.0/src/dynabench/equation/__pycache__/_base.cpython-311.pyc
--rw-r--r--   0        0        0     1224 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/_advection.py
--rw-r--r--   0        0        0     1456 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/equation/_base.py
--rw-r--r--   0        0        0       69 2024-04-19 15:31:13.754053 dynabench-0.3.0/src/dynabench/model/__init__.py
--rw-r--r--   0        0        0      267 2024-04-19 14:58:43.960657 dynabench-0.3.0/src/dynabench/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12038 1970-01-01 00:00:00.000000 dynabench-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-03 10:30:50.861280 dynabench-0.3.1/LICENCE
+-rw-r--r--   0        0        0    18657 2024-05-03 10:30:50.861280 dynabench-0.3.1/LICENCE_data
+-rw-r--r--   0        0        0    11415 2024-05-03 10:30:50.861280 dynabench-0.3.1/README.md
+-rw-r--r--   0        0        0     1054 2024-05-06 19:10:28.406476 dynabench-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/_init_.py
+-rw-r--r--   0        0        0      266 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-03 10:42:03.414598 dynabench-0.3.1/src/dynabench/dataset/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8924 2024-05-03 10:42:03.417931 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc
+-rw-r--r--   0        0        0     5826 2024-05-03 10:42:03.431264 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc
+-rw-r--r--   0        0        0     4744 2024-05-03 10:42:03.601265 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc
+-rw-r--r--   0        0        0     6087 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_download.py
+-rw-r--r--   0        0        0     3119 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_iterator.py
+-rw-r--r--   0        0        0     2466 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_simulation_iterator.py
+-rw-r--r--   0        0        0      201 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/__init__.py
+-rw-r--r--   0        0        0      457 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc
+-rw-r--r--   0        0        0     2662 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/_base.cpython-311.pyc
+-rw-r--r--   0        0        0     1224 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/_advection.py
+-rw-r--r--   0        0        0     1456 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/_base.py
+-rw-r--r--   0        0        0      212 2024-05-03 14:26:34.974287 dynabench-0.3.1/src/dynabench/model/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-03 14:28:35.757618 dynabench-0.3.1/src/dynabench/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      357 2024-05-03 10:42:03.621265 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4029 2024-05-06 17:33:04.099867 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/cnn.cpython-311.pyc
+-rw-r--r--   0        0        0     4149 2024-05-06 19:11:02.933142 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/neuralpde.cpython-311.pyc
+-rw-r--r--   0        0        0     9525 2024-05-06 17:33:04.099867 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/resnet.cpython-311.pyc
+-rw-r--r--   0        0        0     2600 2024-05-06 17:33:00.063201 dynabench-0.3.1/src/dynabench/model/_grid/cnn.py
+-rw-r--r--   0        0        0     2851 2024-05-06 19:04:54.813145 dynabench-0.3.1/src/dynabench/model/_grid/neuralpde.py
+-rwxr-xr-x   0        0        0     7407 2024-05-06 17:32:52.209867 dynabench-0.3.1/src/dynabench/model/_grid/resnet.py
+-rw-r--r--   0        0        0    12209 1970-01-01 00:00:00.000000 dynabench-0.3.1/PKG-INFO
```

### Comparing `dynabench-0.3.0/LICENCE` & `dynabench-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/LICENCE_data` & `dynabench-0.3.1/LICENCE_data`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/README.md` & `dynabench-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/pyproject.toml` & `dynabench-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "dynabench"
-version = "0.3.0"
+version = "0.3.1"
 description = "Benchmark dataset for learning dynamical systems from data"
 authors = ["Andrzej Dulny <andzej.dulny@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://dynabench.github.io/about.html"
+documentation = "https://dynabench.github.io/"
+repository = "https://github.com/badulion/dynabench/"
+
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 numpy = "^1.26.4"
 requests = "^2.31.0"
 tqdm = "^4.66.2"
 h5py = "^3.11.0"
@@ -29,10 +33,15 @@
 
 [tool.poetry.group.findiff]
 optional = true
 
 [tool.poetry.group.findiff.dependencies]
 py-pde = "^0.38.0"
 
+
+[tool.poetry.group.nn.dependencies]
+torch = "^2.3.0"
+torchdiffeq = "^0.2.3"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dynabench-0.3.0/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc` & `dynabench-0.3.1/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94202266 (Fri Apr 19 07:43:16 2024 UTC)
+moddate:  0xdabc3466 (Fri May  3 10:30:50 2024 UTC)
 files sz: 6087
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `dynabench-0.3.0/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc` & `dynabench-0.3.1/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94202266 (Fri Apr 19 07:43:16 2024 UTC)
+moddate:  0xdabc3466 (Fri May  3 10:30:50 2024 UTC)
 files sz: 3119
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `dynabench-0.3.0/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc` & `dynabench-0.3.1/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94202266 (Fri Apr 19 07:43:16 2024 UTC)
+moddate:  0xdabc3466 (Fri May  3 10:30:50 2024 UTC)
 files sz: 2466
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `dynabench-0.3.0/src/dynabench/dataset/_download.py` & `dynabench-0.3.1/src/dynabench/dataset/_download.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/src/dynabench/dataset/_iterator.py` & `dynabench-0.3.1/src/dynabench/dataset/_iterator.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/src/dynabench/dataset/_simulation_iterator.py` & `dynabench-0.3.1/src/dynabench/dataset/_simulation_iterator.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc` & `dynabench-0.3.1/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94202266 (Fri Apr 19 07:43:16 2024 UTC)
+moddate:  0xdabc3466 (Fri May  3 10:30:50 2024 UTC)
 files sz: 1224
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dynabench-0.3.0/src/dynabench/equation/__pycache__/_base.cpython-311.pyc` & `dynabench-0.3.1/src/dynabench/equation/__pycache__/_base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x94202266 (Fri Apr 19 07:43:16 2024 UTC)
+moddate:  0xdabc3466 (Fri May  3 10:30:50 2024 UTC)
 files sz: 1456
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dynabench-0.3.0/src/dynabench/equation/_advection.py` & `dynabench-0.3.1/src/dynabench/equation/_advection.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/src/dynabench/equation/_base.py` & `dynabench-0.3.1/src/dynabench/equation/_base.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.0/PKG-INFO` & `dynabench-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: dynabench
-Version: 0.3.0
+Version: 0.3.1
 Summary: Benchmark dataset for learning dynamical systems from data
+Home-page: https://dynabench.github.io/about.html
 License: MIT
 Author: Andrzej Dulny
 Author-email: andzej.dulny@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5py (>=3.11.0,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Project-URL: Documentation, https://dynabench.github.io/
+Project-URL: Repository, https://github.com/badulion/dynabench/
 Description-Content-Type: text/markdown
 
 # Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data
 
 This is the repository containing the data generation algorithms as well as all baseline models for the __Dynabench: A benchmark dataset for learning dynamical systems from low-resolution data__ paper (accepted at ECML-PKDD 2023)
 
 **!!!You can find the documentation on how to use this package here: [dynabench.github.io](https://dynabench.github.io)**
```

