# Comparing `tmp/peak_finder_app-0.1.0b2.tar.gz` & `tmp/peak_finder_app-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak_finder_app-0.1.0b2.tar", max compression
+gzip compressed data, was "peak_finder_app-0.1.0b3.tar", max compression
```

## Comparing `peak_finder_app-0.1.0b2.tar` & `peak_finder_app-0.1.0b3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 peak_finder_app-0.1.0b2/LICENSE
--rw-r--r--   0        0        0      970 2024-05-03 15:34:48.623106 peak_finder_app-0.1.0b2/peak_finder/__init__.py
--rw-r--r--   0        0        0      866 2024-04-23 22:39:24.314550 peak_finder_app-0.1.0b2/peak_finder/anomaly.py
--rw-r--r--   0        0        0     8372 2024-04-23 22:39:24.314612 peak_finder_app-0.1.0b2/peak_finder/anomaly_group.py
--rw-r--r--   0        0        0    78823 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b2/peak_finder/application.py
--rw-r--r--   0        0        0     1785 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b2/peak_finder/constants.py
--rw-r--r--   0        0        0    15078 2024-04-23 22:39:24.316280 peak_finder_app-0.1.0b2/peak_finder/driver.py
--rw-r--r--   0        0        0   356591 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b2/peak_finder/images/peak_finder_app.png
--rw-r--r--   0        0        0    15808 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b2/peak_finder/layout.py
--rw-r--r--   0        0        0    10882 2024-04-23 22:39:24.319593 peak_finder_app-0.1.0b2/peak_finder/line_anomaly.py
--rw-r--r--   0        0        0    11584 2024-04-23 22:39:24.320130 peak_finder_app-0.1.0b2/peak_finder/line_data.py
--rw-r--r--   0        0        0    11849 2024-04-23 22:39:24.320197 peak_finder_app-0.1.0b2/peak_finder/line_group.py
--rw-r--r--   0        0        0    11812 2024-04-23 22:39:24.320728 peak_finder_app-0.1.0b2/peak_finder/line_position.py
--rw-r--r--   0        0        0    13241 2024-04-23 22:39:24.321386 peak_finder_app-0.1.0b2/peak_finder/params.py
--rw-r--r--   0        0        0     1106 2024-04-23 22:39:24.321970 peak_finder_app-0.1.0b2/peak_finder/utils.py
--rw-r--r--   0        0        0      117 2024-04-23 22:39:24.312898 peak_finder_app-0.1.0b2/peak_finder-assets/__init__.py
--rw-r--r--   0        0        0  1983716 2024-04-23 22:39:24.854255 peak_finder_app-0.1.0b2/peak_finder-assets/FlinFlon_tem_aoi.geoh5
--rw-r--r--   0        0        0     6446 2024-05-02 04:28:11.322688 peak_finder_app-0.1.0b2/peak_finder-assets/uijson/peak_finder.ui.json
--rw-r--r--   0        0        0     5019 2024-05-03 21:14:37.908631 peak_finder_app-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     6280 2024-04-28 20:57:34.791039 peak_finder_app-0.1.0b2/README.rst
--rw-r--r--   0        0        0     6573 2024-04-23 22:39:23.613401 peak_finder_app-0.1.0b2/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     8168 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 peak_finder_app-0.1.0b3/LICENSE
+-rw-r--r--   0        0        0      970 2024-05-04 03:06:40.559191 peak_finder_app-0.1.0b3/peak_finder/__init__.py
+-rw-r--r--   0        0        0      866 2024-04-23 22:39:24.314550 peak_finder_app-0.1.0b3/peak_finder/anomaly.py
+-rw-r--r--   0        0        0     8372 2024-04-23 22:39:24.314612 peak_finder_app-0.1.0b3/peak_finder/anomaly_group.py
+-rw-r--r--   0        0        0    78823 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b3/peak_finder/application.py
+-rw-r--r--   0        0        0     1785 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b3/peak_finder/constants.py
+-rw-r--r--   0        0        0    15078 2024-04-23 22:39:24.316280 peak_finder_app-0.1.0b3/peak_finder/driver.py
+-rw-r--r--   0        0        0   356591 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b3/peak_finder/images/peak_finder_app.png
+-rw-r--r--   0        0        0    15808 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b3/peak_finder/layout.py
+-rw-r--r--   0        0        0    10882 2024-04-23 22:39:24.319593 peak_finder_app-0.1.0b3/peak_finder/line_anomaly.py
+-rw-r--r--   0        0        0    11584 2024-04-23 22:39:24.320130 peak_finder_app-0.1.0b3/peak_finder/line_data.py
+-rw-r--r--   0        0        0    11849 2024-04-23 22:39:24.320197 peak_finder_app-0.1.0b3/peak_finder/line_group.py
+-rw-r--r--   0        0        0    11812 2024-04-23 22:39:24.320728 peak_finder_app-0.1.0b3/peak_finder/line_position.py
+-rw-r--r--   0        0        0    13241 2024-04-23 22:39:24.321386 peak_finder_app-0.1.0b3/peak_finder/params.py
+-rw-r--r--   0        0        0     1106 2024-04-23 22:39:24.321970 peak_finder_app-0.1.0b3/peak_finder/utils.py
+-rw-r--r--   0        0        0      117 2024-04-23 22:39:24.312898 peak_finder_app-0.1.0b3/peak_finder-assets/__init__.py
+-rw-r--r--   0        0        0  1983716 2024-04-23 22:39:24.854255 peak_finder_app-0.1.0b3/peak_finder-assets/FlinFlon_tem_aoi.geoh5
+-rw-r--r--   0        0        0     6446 2024-05-02 04:28:11.322688 peak_finder_app-0.1.0b3/peak_finder-assets/uijson/peak_finder.ui.json
+-rw-r--r--   0        0        0     5684 2024-05-04 03:06:40.573660 peak_finder_app-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     6280 2024-04-28 20:57:34.791039 peak_finder_app-0.1.0b3/README.rst
+-rw-r--r--   0        0        0     6573 2024-04-23 22:39:23.613401 peak_finder_app-0.1.0b3/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     8284 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0b3/PKG-INFO
```

### Comparing `peak_finder_app-0.1.0b2/LICENSE` & `peak_finder_app-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/__init__.py` & `peak_finder_app-0.1.0b3/peak_finder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of peak-finder-app project.
 #
 #  All rights reserved.
 #
 
-__version__ = "0.1.0-beta.2"
+__version__ = "0.1.0-beta.3"
 import os
 import warnings
 from pathlib import Path
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
```

### Comparing `peak_finder_app-0.1.0b2/peak_finder/anomaly.py` & `peak_finder_app-0.1.0b3/peak_finder/anomaly.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/anomaly_group.py` & `peak_finder_app-0.1.0b3/peak_finder/anomaly_group.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/application.py` & `peak_finder_app-0.1.0b3/peak_finder/application.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/constants.py` & `peak_finder_app-0.1.0b3/peak_finder/constants.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/driver.py` & `peak_finder_app-0.1.0b3/peak_finder/driver.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/images/peak_finder_app.png` & `peak_finder_app-0.1.0b3/peak_finder/images/peak_finder_app.png`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/layout.py` & `peak_finder_app-0.1.0b3/peak_finder/layout.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/line_anomaly.py` & `peak_finder_app-0.1.0b3/peak_finder/line_anomaly.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/line_data.py` & `peak_finder_app-0.1.0b3/peak_finder/line_data.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/line_group.py` & `peak_finder_app-0.1.0b3/peak_finder/line_group.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/line_position.py` & `peak_finder_app-0.1.0b3/peak_finder/line_position.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/params.py` & `peak_finder_app-0.1.0b3/peak_finder/params.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder/utils.py` & `peak_finder_app-0.1.0b3/peak_finder/utils.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder-assets/FlinFlon_tem_aoi.geoh5` & `peak_finder_app-0.1.0b3/peak_finder-assets/FlinFlon_tem_aoi.geoh5`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/peak_finder-assets/uijson/peak_finder.ui.json` & `peak_finder_app-0.1.0b3/peak_finder-assets/uijson/peak_finder.ui.json`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/pyproject.toml` & `peak_finder_app-0.1.0b3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peak-finder-app"
-version = "0.1.0-beta.2"
+version = "0.1.0-beta.3"
 license = "MIT"
 description = "Peak Finder App"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/peak-finder-app"
 documentation = "https://mirageoscience-peak-finder-app.readthedocs-hosted.com/"
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
@@ -68,14 +68,21 @@
 h5py = "^3.2.1"  # from geoh5py
 Pillow = "~10.1.0"  # from geoh5py
 pydantic = "~2.5.2"  # from geoapps-utils, curve-apps, also used by petro-lingo
 pyqtwebengine = {version = "~5.15.2, <5.15.7", optional = true}  # from geoapps-utils[dash]
 pyside2 = {version = "~5.15.2.1", optional = true}  # from geoapps-utils[dash]
 scikit-image = "~0.20.0"  # from curve-apps, also used by geo-unsup-mapper
 
+## force some versions to resolve incompatible resolution between PyPI and Conda
+#-------------------------------------------------------------------------------
+# these two *-qt5 dependencies are not relevant for Conda and will be discarded,
+# but conda-lock still look for them in PyPI during its dependency resolution
+pyqt5-qt5 = {version="5.15.2", source = "pypi", optional=true}  # to avoid conda-lock resolving to a dependency version not available on PyPI
+pyqtwebengine-qt5 = {version="5.15.2", source = "pypi", optional=true}  # to avoid conda-lock resolving to a dependency version not available on PyPI
+
 ## about pip dependencies
 # to be specified to work with conda-lock
 # - from PyPI: my_package = { version = "1.2.3", source = "pypi" }
 # - from URL:
 #   - for a tags: my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/tags/VERSION_TAG.zip#sha256=" }
 #   - for a branch: my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/heads/BRANCH.zip#sha256=" }
 # Note - conda-lock does not support the syntax: my_package = { git = ... }
@@ -94,15 +101,17 @@
 tomli = "*" # for tests only
 
 [tool.poetry.extras]
 dash = [
     "dash",
     "dash-daq",
     "flask",
+    "pyqt5-qt5",
     "pyqtwebengine",
+    "pyqtwebengine-qt5",
     "pyside2",
 ]
 
 [tool.conda-lock]
 platforms = ['win-64', 'linux-64']
 channels = ['conda-forge']
```

### Comparing `peak_finder_app-0.1.0b2/README.rst` & `peak_finder_app-0.1.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/THIRD_PARTY_SOFTWARE.rst` & `peak_finder_app-0.1.0b3/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0b2/PKG-INFO` & `peak_finder_app-0.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-finder-app
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Peak Finder App
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Dominique Fournier
 Maintainer-email: dominiquef@mirageoscience.com
@@ -32,15 +32,17 @@
 Requires-Dist: flask (>=3.0.3,<3.1.0) ; extra == "dash"
 Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: plotly (>=5.19.0,<5.20.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
+Requires-Dist: pyqt5-qt5 (==5.15.2) ; extra == "dash"
 Requires-Dist: pyqtwebengine (>=5.15.2,<5.15.7) ; extra == "dash"
+Requires-Dist: pyqtwebengine-qt5 (==5.15.2) ; extra == "dash"
 Requires-Dist: pyside2 (>=5.15.2.1,<5.16.0.0) ; extra == "dash"
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Documentation, https://mirageoscience-peak-finder-app.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/MiraGeoscience/peak-finder-app
 Description-Content-Type: text/x-rst
```

