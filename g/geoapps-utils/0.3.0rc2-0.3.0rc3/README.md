# Comparing `tmp/geoapps_utils-0.3.0rc2.tar.gz` & `tmp/geoapps_utils-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoapps_utils-0.3.0rc2.tar", max compression
+gzip compressed data, was "geoapps_utils-0.3.0rc3.tar", max compression
```

## Comparing `geoapps_utils-0.3.0rc2.tar` & `geoapps_utils-0.3.0rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      318 2024-05-03 14:25:29.750449 geoapps_utils-0.3.0rc2/geoapps_utils/__init__.py
--rw-r--r--   0        0        0      242 2024-04-23 21:07:36.651950 geoapps_utils-0.3.0rc2/geoapps_utils/application/__init__.py
--rw-r--r--   0        0        0    24574 2024-04-23 21:07:36.653221 geoapps_utils-0.3.0rc2/geoapps_utils/application/dash_application.py
--rw-r--r--   0        0        0     3039 2024-04-23 21:07:36.653761 geoapps_utils-0.3.0rc2/geoapps_utils/application/layout.py
--rw-r--r--   0        0        0     1104 2024-04-23 21:07:36.654305 geoapps_utils-0.3.0rc2/geoapps_utils/conversions.py
--rw-r--r--   0        0        0      242 2024-04-23 21:07:36.654989 geoapps_utils-0.3.0rc2/geoapps_utils/driver/__init__.py
--rw-r--r--   0        0        0     3938 2024-04-23 21:07:36.654989 geoapps_utils-0.3.0rc2/geoapps_utils/driver/data.py
--rw-r--r--   0        0        0     4254 2024-04-23 21:07:36.655614 geoapps_utils-0.3.0rc2/geoapps_utils/driver/driver.py
--rw-r--r--   0        0        0    15475 2024-04-23 21:07:36.656157 geoapps_utils-0.3.0rc2/geoapps_utils/driver/params.py
--rw-r--r--   0        0        0      654 2024-04-23 21:07:36.656745 geoapps_utils-0.3.0rc2/geoapps_utils/formatters.py
--rw-r--r--   0        0        0     1539 2024-04-23 21:07:36.657364 geoapps_utils-0.3.0rc2/geoapps_utils/importing.py
--rw-r--r--   0        0        0     3550 2024-04-23 21:07:36.657948 geoapps_utils-0.3.0rc2/geoapps_utils/iterables.py
--rw-r--r--   0        0        0     3040 2024-04-23 21:07:36.658478 geoapps_utils-0.3.0rc2/geoapps_utils/locations.py
--rw-r--r--   0        0        0    10712 2024-04-23 21:07:36.658478 geoapps_utils-0.3.0rc2/geoapps_utils/numerical.py
--rw-r--r--   0        0        0     1702 2024-04-23 21:07:36.659540 geoapps_utils-0.3.0rc2/geoapps_utils/plotting.py
--rw-r--r--   0        0        0     1714 2024-04-23 21:07:36.659540 geoapps_utils-0.3.0rc2/geoapps_utils/transformations.py
--rw-r--r--   0        0        0     1697 2024-04-23 21:07:36.660574 geoapps_utils-0.3.0rc2/geoapps_utils/workspace.py
--rw-r--r--   0        0        0     1098 2024-04-23 21:07:36.644208 geoapps_utils-0.3.0rc2/LICENSE
--rw-r--r--   0        0        0     4043 2024-05-03 15:29:13.009750 geoapps_utils-0.3.0rc2/pyproject.toml
--rw-r--r--   0        0        0     6591 2024-04-23 21:07:36.645310 geoapps_utils-0.3.0rc2/README.rst
--rw-r--r--   0        0        0     5426 2024-04-23 21:02:26.252531 geoapps_utils-0.3.0rc2/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     8040 1970-01-01 00:00:00.000000 geoapps_utils-0.3.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      318 2024-05-06 01:40:40.815556 geoapps_utils-0.3.0rc3/geoapps_utils/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-23 21:07:36.651950 geoapps_utils-0.3.0rc3/geoapps_utils/application/__init__.py
+-rw-r--r--   0        0        0    24574 2024-04-23 21:07:36.653221 geoapps_utils-0.3.0rc3/geoapps_utils/application/dash_application.py
+-rw-r--r--   0        0        0     3039 2024-04-23 21:07:36.653761 geoapps_utils-0.3.0rc3/geoapps_utils/application/layout.py
+-rw-r--r--   0        0        0     1104 2024-04-23 21:07:36.654305 geoapps_utils-0.3.0rc3/geoapps_utils/conversions.py
+-rw-r--r--   0        0        0      242 2024-04-23 21:07:36.654989 geoapps_utils-0.3.0rc3/geoapps_utils/driver/__init__.py
+-rw-r--r--   0        0        0     3938 2024-04-23 21:07:36.654989 geoapps_utils-0.3.0rc3/geoapps_utils/driver/data.py
+-rw-r--r--   0        0        0     4254 2024-04-23 21:07:36.655614 geoapps_utils-0.3.0rc3/geoapps_utils/driver/driver.py
+-rw-r--r--   0        0        0    15475 2024-04-23 21:07:36.656157 geoapps_utils-0.3.0rc3/geoapps_utils/driver/params.py
+-rw-r--r--   0        0        0      654 2024-04-23 21:07:36.656745 geoapps_utils-0.3.0rc3/geoapps_utils/formatters.py
+-rw-r--r--   0        0        0     1539 2024-04-23 21:07:36.657364 geoapps_utils-0.3.0rc3/geoapps_utils/importing.py
+-rw-r--r--   0        0        0     3550 2024-04-23 21:07:36.657948 geoapps_utils-0.3.0rc3/geoapps_utils/iterables.py
+-rw-r--r--   0        0        0     3040 2024-04-23 21:07:36.658478 geoapps_utils-0.3.0rc3/geoapps_utils/locations.py
+-rw-r--r--   0        0        0    10712 2024-04-23 21:07:36.658478 geoapps_utils-0.3.0rc3/geoapps_utils/numerical.py
+-rw-r--r--   0        0        0     1702 2024-04-23 21:07:36.659540 geoapps_utils-0.3.0rc3/geoapps_utils/plotting.py
+-rw-r--r--   0        0        0     1714 2024-04-23 21:07:36.659540 geoapps_utils-0.3.0rc3/geoapps_utils/transformations.py
+-rw-r--r--   0        0        0     1697 2024-04-23 21:07:36.660574 geoapps_utils-0.3.0rc3/geoapps_utils/workspace.py
+-rw-r--r--   0        0        0     1098 2024-04-23 21:07:36.644208 geoapps_utils-0.3.0rc3/LICENSE
+-rw-r--r--   0        0        0     4043 2024-05-06 01:41:41.501999 geoapps_utils-0.3.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     6591 2024-04-23 21:07:36.645310 geoapps_utils-0.3.0rc3/README.rst
+-rw-r--r--   0        0        0     5426 2024-04-23 21:02:26.252531 geoapps_utils-0.3.0rc3/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 geoapps_utils-0.3.0rc3/PKG-INFO
```

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/application/dash_application.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/application/dash_application.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/application/layout.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/application/layout.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/conversions.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/conversions.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/driver/data.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/driver/data.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/driver/driver.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/driver/driver.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/driver/params.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/driver/params.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/formatters.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/importing.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/importing.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/iterables.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/iterables.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/locations.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/locations.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/numerical.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/numerical.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/plotting.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/transformations.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/transformations.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/geoapps_utils/workspace.py` & `geoapps_utils-0.3.0rc3/geoapps_utils/workspace.py`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/LICENSE` & `geoapps_utils-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/pyproject.toml` & `geoapps_utils-0.3.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoapps-utils"
-version = "0.3.0-rc.2"
+version = "0.3.0-rc.3"
 license = "MIT"
 description = "Geoapps Utils"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoapps-utils"
 #documentation  = "https://mirageoscience-geoapps-utils.readthedocs-hosted.com/"
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
@@ -45,16 +45,16 @@
 #----------------------------------------
 geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}
 #geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 #geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
 ## dependencies for plots with Dash
 #-------------------------------
-dash = {version = "~2.12", optional = true}
-flask = {version = "~3.0.3", optional = true}
+dash = {version = "^2.12", optional = true}
+flask = {version = "^3.0.3", optional = true}
 pyqtwebengine = {version = "~5.15.2, <5.15.7", optional = true}  # 5.15.7 and newer on conda-forge, but not in PyPI
 pyside2 = {version = "~5.15.2.1", optional = true}  # 5.15.3 and newer on conda-forge, but not in PyPI
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
 #---------------------------------------------------------------------------------
 h5py = "^3.2.1"  # from geoh5py
 Pillow = "~10.1.0"  # from geoh5py
```

### Comparing `geoapps_utils-0.3.0rc2/README.rst` & `geoapps_utils-0.3.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/THIRD_PARTY_SOFTWARE.rst` & `geoapps_utils-0.3.0rc3/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `geoapps_utils-0.3.0rc2/PKG-INFO` & `geoapps_utils-0.3.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoapps-utils
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: Geoapps Utils
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Dominique Fournier
 Maintainer-email: dominiquef@mirageoscience.com
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: dash
 Requires-Dist: Pillow (>=10.1.0,<10.2.0)
-Requires-Dist: dash (>=2.12,<2.13) ; extra == "dash"
-Requires-Dist: flask (>=3.0.3,<3.1.0) ; extra == "dash"
+Requires-Dist: dash (>=2.12,<3.0) ; extra == "dash"
+Requires-Dist: flask (>=3.0.3,<4.0.0) ; extra == "dash"
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: pyqtwebengine (>=5.15.2,<5.15.7) ; extra == "dash"
 Requires-Dist: pyside2 (>=5.15.2.1,<5.16.0.0) ; extra == "dash"
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
```

