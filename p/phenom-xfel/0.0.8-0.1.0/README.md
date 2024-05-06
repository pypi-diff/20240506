# Comparing `tmp/phenom_xfel-0.0.8.tar.gz` & `tmp/phenom_xfel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phenom_xfel-0.0.8.tar", last modified: Thu Sep 21 08:17:03 2023, max compression
+gzip compressed data, was "phenom_xfel-0.1.0.tar", last modified: Mon May  6 15:27:57 2024, max compression
```

## Comparing `phenom_xfel-0.0.8.tar` & `phenom_xfel-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.182937 phenom_xfel-0.0.8/
--rw-r--r--   0 guestt   (36329) gpex      (7987)      164 2023-06-28 08:34:54.000000 phenom_xfel-0.0.8/AUTHORS.rst
--rw-r--r--   0 guestt   (36329) gpex      (7987)     3011 2023-06-28 08:34:54.000000 phenom_xfel-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1518 2023-06-28 08:34:54.000000 phenom_xfel-0.0.8/LICENSE
--rw-r--r--   0 guestt   (36329) gpex      (7987)      359 2023-06-28 08:34:54.000000 phenom_xfel-0.0.8/MANIFEST.in
--rw-r--r--   0 guestt   (36329) gpex      (7987)     2171 2023-09-21 08:17:03.183070 phenom_xfel-0.0.8/PKG-INFO
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1442 2023-09-21 07:36:13.000000 phenom_xfel-0.0.8/README.md
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.170043 phenom_xfel-0.0.8/docs/
--rw-r--r--   0 guestt   (36329) gpex      (7987)      673 2023-06-28 08:34:54.000000 phenom_xfel-0.0.8/docs/Makefile
--rw-r--r--   0 guestt   (36329) gpex      (7987)      833 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/docs/make.bat
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.171999 phenom_xfel-0.0.8/docs/source/
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1679 2023-09-21 07:36:14.000000 phenom_xfel-0.0.8/docs/source/api.rst
--rw-r--r--   0 guestt   (36329) gpex      (7987)     6489 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/docs/source/conf.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      338 2023-09-21 07:36:14.000000 phenom_xfel-0.0.8/docs/source/examples.rst
--rw-r--r--   0 guestt   (36329) gpex      (7987)      342 2023-09-21 07:36:14.000000 phenom_xfel-0.0.8/docs/source/index.rst
--rw-r--r--   0 guestt   (36329) gpex      (7987)       93 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/docs/source/installation.rst
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.184911 phenom_xfel-0.0.8/phenom/
--rw-r--r--   0 guestt   (36329) gpex      (7987)      109 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/__info__.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)       93 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/__init__.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      194 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/__warnings__.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      497 2023-09-21 08:17:03.185021 phenom_xfel-0.0.8/phenom/_version.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1697 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/gaussian.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      818 2023-07-09 11:59:34.000000 phenom_xfel-0.0.8/phenom/io.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     3194 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/mesh.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)    10757 2023-07-09 10:21:19.000000 phenom_xfel-0.0.8/phenom/source.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      275 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/spectra.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     2126 2023-09-21 07:36:14.000000 phenom_xfel-0.0.8/phenom/spectrum.py
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.180458 phenom_xfel-0.0.8/phenom/tests/
--rw-r--r--   0 guestt   (36329) gpex      (7987)        0 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/tests/__init__.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)        0 2023-06-28 08:34:55.000000 phenom_xfel-0.0.8/phenom/tests/conftest.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)      223 2023-06-28 08:34:56.000000 phenom_xfel-0.0.8/phenom/tests/test_examples.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1072 2023-07-09 11:54:15.000000 phenom_xfel-0.0.8/phenom/utils.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     1050 2023-09-21 07:36:14.000000 phenom_xfel-0.0.8/phenom/wavefront_tools.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)     2061 2023-07-09 12:11:18.000000 phenom_xfel-0.0.8/phenom/wpg.py
-drwxr-xr-x   0 guestt   (36329) gpex      (7987)        0 2023-09-21 08:17:03.182647 phenom_xfel-0.0.8/phenom_xfel.egg-info/
--rw-r--r--   0 guestt   (36329) gpex      (7987)     2171 2023-09-21 08:17:03.180905 phenom_xfel-0.0.8/phenom_xfel.egg-info/PKG-INFO
--rw-r--r--   0 guestt   (36329) gpex      (7987)      796 2023-09-21 08:17:03.181234 phenom_xfel-0.0.8/phenom_xfel.egg-info/SOURCES.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)        1 2023-09-21 08:17:03.181562 phenom_xfel-0.0.8/phenom_xfel.egg-info/dependency_links.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)       20 2023-09-21 08:17:03.182067 phenom_xfel-0.0.8/phenom_xfel.egg-info/entry_points.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)       56 2023-09-21 08:17:03.182393 phenom_xfel-0.0.8/phenom_xfel.egg-info/requires.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)        7 2023-09-21 08:17:03.182730 phenom_xfel-0.0.8/phenom_xfel.egg-info/top_level.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)      276 2023-06-28 08:34:56.000000 phenom_xfel-0.0.8/pyproject.toml
--rw-r--r--   0 guestt   (36329) gpex      (7987)       57 2023-09-21 07:36:29.000000 phenom_xfel-0.0.8/requirements.txt
--rw-r--r--   0 guestt   (36329) gpex      (7987)      171 2023-09-21 08:17:03.183573 phenom_xfel-0.0.8/setup.cfg
--rw-r--r--   0 guestt   (36329) gpex      (7987)     2252 2023-09-21 08:16:30.000000 phenom_xfel-0.0.8/setup.py
--rw-r--r--   0 guestt   (36329) gpex      (7987)    68503 2023-06-28 08:34:56.000000 phenom_xfel-0.0.8/versioneer.py
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.649623 phenom_xfel-0.1.0/
+-rw-r--r--   0 twguest    (501) staff       (20)      164 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/AUTHORS.rst
+-rw-r--r--   0 twguest    (501) staff       (20)     3011 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 twguest    (501) staff       (20)     1518 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/LICENSE
+-rw-r--r--   0 twguest    (501) staff       (20)      359 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/MANIFEST.in
+-rw-r--r--   0 twguest    (501) staff       (20)     2994 2024-05-06 15:27:57.649558 phenom_xfel-0.1.0/PKG-INFO
+-rw-r--r--   0 twguest    (501) staff       (20)     2333 2024-05-06 15:26:46.000000 phenom_xfel-0.1.0/README.md
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.642801 phenom_xfel-0.1.0/docs/
+-rw-r--r--   0 twguest    (501) staff       (20)      673 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/docs/Makefile
+-rw-r--r--   0 twguest    (501) staff       (20)      833 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/docs/make.bat
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.644565 phenom_xfel-0.1.0/docs/source/
+-rw-r--r--   0 twguest    (501) staff       (20)     1679 2023-07-09 18:19:16.000000 phenom_xfel-0.1.0/docs/source/api.rst
+-rw-r--r--   0 twguest    (501) staff       (20)     6489 2023-06-14 20:05:26.000000 phenom_xfel-0.1.0/docs/source/conf.py
+-rw-r--r--   0 twguest    (501) staff       (20)      406 2024-05-06 10:04:57.000000 phenom_xfel-0.1.0/docs/source/examples.rst
+-rw-r--r--   0 twguest    (501) staff       (20)      342 2023-07-09 17:54:59.000000 phenom_xfel-0.1.0/docs/source/index.rst
+-rw-r--r--   0 twguest    (501) staff       (20)       93 2023-06-14 16:04:33.000000 phenom_xfel-0.1.0/docs/source/installation.rst
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.650105 phenom_xfel-0.1.0/phenom/
+-rw-r--r--   0 twguest    (501) staff       (20)      109 2023-06-14 15:03:47.000000 phenom_xfel-0.1.0/phenom/__info__.py
+-rw-r--r--   0 twguest    (501) staff       (20)       93 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/phenom/__init__.py
+-rw-r--r--   0 twguest    (501) staff       (20)      194 2023-06-14 15:03:47.000000 phenom_xfel-0.1.0/phenom/__warnings__.py
+-rw-r--r--   0 twguest    (501) staff       (20)      497 2024-05-06 15:27:57.650143 phenom_xfel-0.1.0/phenom/_version.py
+-rw-r--r--   0 twguest    (501) staff       (20)     1697 2023-06-14 16:04:33.000000 phenom_xfel-0.1.0/phenom/gaussian.py
+-rw-r--r--   0 twguest    (501) staff       (20)      818 2023-07-09 17:45:59.000000 phenom_xfel-0.1.0/phenom/io.py
+-rw-r--r--   0 twguest    (501) staff       (20)     3194 2023-06-14 16:04:33.000000 phenom_xfel-0.1.0/phenom/mesh.py
+-rw-r--r--   0 twguest    (501) staff       (20)    11068 2024-05-06 11:09:17.000000 phenom_xfel-0.1.0/phenom/source.py
+-rw-r--r--   0 twguest    (501) staff       (20)     2957 2024-05-06 11:09:17.000000 phenom_xfel-0.1.0/phenom/spectrum.py
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.648103 phenom_xfel-0.1.0/phenom/tests/
+-rw-r--r--   0 twguest    (501) staff       (20)        0 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/phenom/tests/__init__.py
+-rw-r--r--   0 twguest    (501) staff       (20)        0 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/phenom/tests/conftest.py
+-rw-r--r--   0 twguest    (501) staff       (20)       97 2024-05-06 10:11:12.000000 phenom_xfel-0.1.0/phenom/tests/test_examples.py
+-rw-r--r--   0 twguest    (501) staff       (20)     1072 2023-07-09 17:45:59.000000 phenom_xfel-0.1.0/phenom/utils.py
+-rw-r--r--   0 twguest    (501) staff       (20)     1050 2023-07-09 18:19:37.000000 phenom_xfel-0.1.0/phenom/wavefront_tools.py
+-rw-r--r--   0 twguest    (501) staff       (20)     2094 2024-05-06 11:09:17.000000 phenom_xfel-0.1.0/phenom/wpg.py
+drwxr-xr-x   0 twguest    (501) staff       (20)        0 2024-05-06 15:27:57.649236 phenom_xfel-0.1.0/phenom_xfel.egg-info/
+-rw-r--r--   0 twguest    (501) staff       (20)     2994 2024-05-06 15:27:57.000000 phenom_xfel-0.1.0/phenom_xfel.egg-info/PKG-INFO
+-rw-r--r--   0 twguest    (501) staff       (20)      740 2024-05-06 15:27:57.000000 phenom_xfel-0.1.0/phenom_xfel.egg-info/SOURCES.txt
+-rw-r--r--   0 twguest    (501) staff       (20)        1 2024-05-06 15:27:57.000000 phenom_xfel-0.1.0/phenom_xfel.egg-info/dependency_links.txt
+-rw-r--r--   0 twguest    (501) staff       (20)       56 2024-05-06 15:27:57.000000 phenom_xfel-0.1.0/phenom_xfel.egg-info/requires.txt
+-rw-r--r--   0 twguest    (501) staff       (20)        7 2024-05-06 15:27:57.000000 phenom_xfel-0.1.0/phenom_xfel.egg-info/top_level.txt
+-rw-r--r--   0 twguest    (501) staff       (20)      276 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/pyproject.toml
+-rw-r--r--   0 twguest    (501) staff       (20)       57 2023-10-18 07:01:34.000000 phenom_xfel-0.1.0/requirements.txt
+-rw-r--r--   0 twguest    (501) staff       (20)      171 2024-05-06 15:27:57.649946 phenom_xfel-0.1.0/setup.cfg
+-rw-r--r--   0 twguest    (501) staff       (20)     2252 2023-10-18 07:01:34.000000 phenom_xfel-0.1.0/setup.py
+-rw-r--r--   0 twguest    (501) staff       (20)    68503 2023-06-09 19:34:21.000000 phenom_xfel-0.1.0/versioneer.py
```

### Comparing `phenom_xfel-0.0.8/CONTRIBUTING.rst` & `phenom_xfel-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/LICENSE` & `phenom_xfel-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/PKG-INFO` & `phenom_xfel-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,36 @@
-Metadata-Version: 2.1
-Name: phenom_xfel
-Version: 0.0.8
-Summary: A phenomenological model of X-ray Free Electron Laser (XFEL) radiation and radiation statistics.
-Home-page: https://github.com/twguest/phenom
-Author: Trey Guest
-Author-email: trey.guest@xfel.eu
-License: BSD (3-clause)
-Description: # phenom
-        
-        [![](https://github.com/twguest/phenom/actions/workflows/testing.yml/badge.svg)]( https://github.com/twguest/phenom/actions/workflows/testing.yml)[![](https://img.shields.io/pypi/v/phenom.svg)](https://pypi.python.org/pypi/phenom_xfel)
-        
-        
-        A **phenom**enological model of X-ray Free Electron Laser (XFEL) radiation.
-        
-        The PHENOM python package is designed to provide a simple, robust and computationally efficient method for generating representations of the complex wavefield of X-ray Free Electron Laser pulses. By making use of approximate representations of pulse wavefront and [spectra](https://www.osapublishing.org/abstract.cfm?URI=ol-35-20-3441), phenom allows large ensembles of photon pulses with arbitrary statistics to be generated in a truly python-ised manner.
-        
-        ## Getting Started
-        At the command line::
-        
-            $ pip install phenom-xfel
-        
-        To check that your instillation has worked, open iPython and try::
-        
-            $ import phenom
-            
-        ## Examples
-        Phenom has been designed to require minimal knowledge of the XFEL process prior to generating your first pulse.
-        
-        1. [Getting Started](https://twguest.github.io/phenom/notebooks/sase_model_pt1.html)
-        2. [Tutorials](https://twguest.github.io/phenom/notebooks/sase_model_pt2.html).
-        3. [Integrating with WPG](https://twguest.github.io/phenom/notebooks/phenom_to_wpg.html).
-        
-        More details on generating these pulses can be found in the [documentation](https://twguest.github.io/phenom).
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# phenom
+
+[![](https://github.com/twguest/phenom/actions/workflows/testing.yml/badge.svg)]( https://github.com/twguest/phenom/actions/workflows/testing.yml)[![](https://img.shields.io/pypi/v/phenom.svg)](https://pypi.python.org/pypi/phenom_xfel)
+
+
+A **phenom**enological model of X-ray Free Electron Laser (XFEL) radiation.
+
+The PHENOM python package is designed to provide a simple, robust and computationally efficient method for generating representations of the complex wavefield of X-ray Free Electron Laser pulses. By making use of approximate representations of pulse wavefront and [spectra](https://www.osapublishing.org/abstract.cfm?URI=ol-35-20-3441), phenom allows large ensembles of photon pulses with arbitrary statistics to be generated in a truly python-ised manner.
+
+## Getting Started
+At the command line::
+
+    $ pip install phenom-xfel
+
+To check that your instillation has worked, open iPython and try::
+
+    $ import phenom
+    
+## Examples
+Phenom has been designed to require minimal knowledge of the XFEL process prior to generating your first pulse.
+
+1. [Getting Started](https://twguest.github.io/phenom/notebooks/sase_model_pt1.html)
+2. [Tutorials](https://twguest.github.io/phenom/notebooks/sase_model_pt2.html).
+3. [Integrating with WPG](https://twguest.github.io/phenom/notebooks/phenom_to_wpg.html).
+
+More details on generating these pulses can be found in the [documentation](https://twguest.github.io/phenom).
+
+## Citation:
+The use of this package and the methods applied therein should be acknowledged using the following citation:
+- Guest, T. W., R. Bean, R. Kammering, G. van Riessen, A. P. Mancuso, and B. Abbey. “A Phenomenological Model of the X-Ray Pulse Statistics of a High-Repetition-Rate X-Ray Free-Electron Laser.” IUCrJ 10, no. 6 (November 1, 2023). https://doi.org/10.1107/S2052252523008242.
+
+## Cited By:
+Below is a list of research which have acknowledged the application of this model
+- E, Juncheng, Carsten Fortmann-Grote, Trey Guest, Egor Sobolev, Luca Gelisio, Richard Bean, and Adrian P. Mancuso. “SimEx-Lite: Easy Access to Start-to-End Simulation for Experiments at Advanced Light Sources.” In Advances in Computational Methods for X-Ray Optics VI, edited by Oleg Chubar and Takashi Tanaka, 22. San Diego, United States: SPIE, 2023. https://doi.org/10.1117/12.2677299.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `phenom_xfel-0.0.8/docs/Makefile` & `phenom_xfel-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/docs/make.bat` & `phenom_xfel-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/docs/source/api.rst` & `phenom_xfel-0.1.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/docs/source/conf.py` & `phenom_xfel-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/gaussian.py` & `phenom_xfel-0.1.0/phenom/gaussian.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/io.py` & `phenom_xfel-0.1.0/phenom/io.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/mesh.py` & `phenom_xfel-0.1.0/phenom/mesh.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/source.py` & `phenom_xfel-0.1.0/phenom/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     sigma,
     div,
     x0,
     y0,
     t0,
     theta_x,
     theta_y,
+    domain = 'freq'
 ):
     """
     SASE pulse model
 
     :param x: horizontal coordinates (np.ndarray)
     :param y: vertical coordinates (np.ndarray)
     :param photon_energy: photon energy in eV (float)
@@ -46,30 +47,30 @@
     :param sigma: gaussian beam width (float)
     :param div: beam divergence (float)
     :param x0: horizontal position jitter (float)
     :param y0: vertical position jitter (float)
     :param t0: temporal jitter (float)
     :param theta_x: horizontal pointing angle (float)
     :param theta_y: vertical pointing angle (float)
-
+    :param domain: 'time' or 'freq', determines the output of sase spectrum
     """
 
     tfield = linear_SASE_spectrum(
         t,
         pulse_duration=pulse_duration,
         photon_energy=photon_energy,
         bandwidth=bandwidth,
         t0=t0,
-    )
+        output = domain)
 
     sfield = complex_gaussian_beam(
         x=x,
         y=y,
         photon_energy=photon_energy,
-        pulse_energy=photon_energy,
+        pulse_energy=pulse_energy,
         sigma=sigma,
         div=div,
         x0=x0,
         y0=x0,
         theta_x=theta_x,
         theta_y=theta_y,
     )
@@ -80,15 +81,15 @@
     efield /= np.sqrt(np.sum(abs(efield) ** 2) * np.ptp(x) * np.ptp(y) * np.ptp(t))
     efield *= pulse_energy
 
     return efield
 
 
 def check_arg_types(args):
-    parse_types = [float, list, np.ndarray, FunctionType]
+    parse_types = [float, list, str, np.ndarray, FunctionType]
 
     keys = list(args.keys())
 
     for key in keys:
         key_types = {}
         key_types[key] = type(args[key])
 
@@ -113,34 +114,37 @@
     :returns __set__: dict of argument keys sorted by value type
     """
 
     __keys__ = list(args.keys())
 
     __arrays__ = []
     __lams__ = []
-
+    __strs__ = []
     N = 1  ### number of pulses
 
     for key in __keys__:
         # print(key,type(args[key])) # dev @author: twguest - 13/06/23
-
+        
         if type(args[key]) == np.ndarray:
             __arrays__.append(key)
 
         elif type(args[key]) == FunctionType:
             __lams__.append(key)
-
+        
+        elif type(args[key]) == str:
+            __strs__.append(key)
+            
     __len__ = [args[key].shape[0] for key in __arrays__]
 
     if len(__arrays__) > 0:
         assert np.all(__len__ == np.mean(__len__)), "all length of all lists and 1d numpy arrays must be equal"
 
         N = int(np.mean(__len__))
 
-    __floats__ = list(set(__keys__) - set(__arrays__) - set(__lams__))
+    __floats__ = list(set(__keys__) - set(__arrays__) - set(__lams__) - set(__strs__))
 
     __set__ = {}
 
     __set__["float"] = __floats__
     __set__["np.ndarray"] = __arrays__
     __set__["FunctionType"] = __lams__
 
@@ -341,14 +345,15 @@
         sigma,
         div,
         x0,
         y0,
         t0,
         theta_x,
         theta_y,
+        domain = 'freq'
     ):
         """
         initialisation function.
 
         :param x: horizontal coordinates (np.ndarray)
         :param y: vertical coordinates (np.ndarray)
         :param photon_energy: photon energy in eV (float)
@@ -378,14 +383,15 @@
             sigma=sigma,
             div=div,
             x0=x0,
             y0=y0,
             t0=t0,
             theta_x=theta_x,
             theta_y=theta_y,
+            domain = domain
         )
 
     def generate_sase_field(self, params):
         sase_field = sase_pulse(
             x=self.x,
             y=self.y,
             t=self.t,
@@ -402,7 +408,8 @@
             theta_y=params["theta_y"],
         )
 
         return sase_field
 
     def generate_pulses(self, sdir):
         self.execute(self.generate_sase_field, sdir)
+
```

### Comparing `phenom_xfel-0.0.8/phenom/utils.py` & `phenom_xfel-0.1.0/phenom/utils.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/wavefront_tools.py` & `phenom_xfel-0.1.0/phenom/wavefront_tools.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/phenom/wpg.py` & `phenom_xfel-0.1.0/phenom/wpg.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,27 +54,30 @@
 
     # Setup E-field.
     wfr.data.arrEhor = np.zeros(shape=(nx, ny, nt, 2))
     wfr.data.arrEver = np.zeros(shape=(nx, ny, nt, 2))
 
     wfr.params.wEFieldUnit = 'sqrt(W/mm^2)'
     wfr.params.photonEnergy = photon_energy
-    wfr.params.wDomain = 'time'
+    
     wfr.params.Mesh.nSlices = nt
     wfr.params.Mesh.nx = nx
-    wfr.params.Mesh.ny = ny
-
+    wfr.params.Mesh.ny = ny      
+    
     wfr.params.Mesh.sliceMin = np.min(t)
     wfr.params.Mesh.sliceMax = np.max(t)
-
-
+    
+    wfr.params.wDomain = 'time'
+    
+    srwlpy.SetRepresElecField(wfr._srwl_wf, 'frequency')
+    
     wfr.params.Mesh.xMin = np.min(x)
     wfr.params.Mesh.xMax = np.max(x)
     wfr.params.Mesh.yMin = np.min(y)
     wfr.params.Mesh.yMax = np.max(y)
 
     wfr.params.Rx = 1
     wfr.params.Ry = 1
 
     wfr.data.arrEhor = complex_to_wpg(efield)
-    srwlpy.SetRepresElecField(wfr._srwl_wf, 'frequency')
+    
     return wfr
```

### Comparing `phenom_xfel-0.0.8/phenom_xfel.egg-info/SOURCES.txt` & `phenom_xfel-0.1.0/phenom_xfel.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,21 +19,19 @@
 phenom/__init__.py
 phenom/__warnings__.py
 phenom/_version.py
 phenom/gaussian.py
 phenom/io.py
 phenom/mesh.py
 phenom/source.py
-phenom/spectra.py
 phenom/spectrum.py
 phenom/utils.py
 phenom/wavefront_tools.py
 phenom/wpg.py
 phenom/tests/__init__.py
 phenom/tests/conftest.py
 phenom/tests/test_examples.py
 phenom_xfel.egg-info/PKG-INFO
 phenom_xfel.egg-info/SOURCES.txt
 phenom_xfel.egg-info/dependency_links.txt
-phenom_xfel.egg-info/entry_points.txt
 phenom_xfel.egg-info/requires.txt
 phenom_xfel.egg-info/top_level.txt
```

### Comparing `phenom_xfel-0.0.8/setup.py` & `phenom_xfel-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `phenom_xfel-0.0.8/versioneer.py` & `phenom_xfel-0.1.0/versioneer.py`

 * *Files identical despite different names*

