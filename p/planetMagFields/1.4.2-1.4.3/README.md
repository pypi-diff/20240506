# Comparing `tmp/planetmagfields-1.4.2.tar.gz` & `tmp/planetmagfields-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmagfields-1.4.2.tar", last modified: Tue Apr 30 14:53:45 2024, max compression
+gzip compressed data, was "planetmagfields-1.4.3.tar", last modified: Mon May  6 04:26:38 2024, max compression
```

## Comparing `planetmagfields-1.4.2.tar` & `planetmagfields-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/LICENSE
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7048 2024-04-29 13:24:10.000000 planetmagfields-1.4.2/README.md
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/planetMagFields.egg-info/
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1035 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/SOURCES.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/dependency_links.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/requires.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/top_level.txt
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.846647 planetmagfields-1.4.2/planetmagfields/
--rw-r--r--   0 ankit     (1000) ankit     (1000)      159 2024-04-30 14:51:50.000000 planetmagfields-1.4.2/planetmagfields/__init__.py
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/planetmagfields/data/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/earth_igrf13.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/ganymede_kivelson2002.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm09.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm33.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_vip4.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_anderson2012.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_thebault2018.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_wardinski2019.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/neptune_connerny1991.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassini11+.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassini11.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassinisoi.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/uranus_connerny1987.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     4701 2024-02-26 00:30:26.000000 planetmagfields-1.4.2/planetmagfields/libbfield.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3863 2024-02-26 01:09:53.000000 planetmagfields-1.4.2/planetmagfields/libdata.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/libgauss.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    11746 2024-04-30 14:44:50.000000 planetmagfields-1.4.2/planetmagfields/planet.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     6725 2024-04-30 14:45:13.000000 planetmagfields-1.4.2/planetmagfields/plotlib.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7835 2024-02-26 01:04:13.000000 planetmagfields-1.4.2/planetmagfields/potextra.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/utils.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-04-30 14:52:06.000000 planetmagfields-1.4.2/pyproject.toml
--rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/setup.cfg
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/setup.py
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/tests/
--rw-r--r--   0 ankit     (1000) ankit     (1000)      856 2024-04-29 13:24:53.000000 planetmagfields-1.4.2/tests/test_planetBr.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-06 04:26:38.327648 planetmagfields-1.4.3/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/LICENSE
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-05-06 04:26:38.327648 planetmagfields-1.4.3/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7048 2024-04-29 13:24:10.000000 planetmagfields-1.4.3/README.md
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-06 04:26:38.327648 planetmagfields-1.4.3/planetMagFields.egg-info/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-05-06 04:26:38.000000 planetmagfields-1.4.3/planetMagFields.egg-info/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1094 2024-05-06 04:26:38.000000 planetmagfields-1.4.3/planetMagFields.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-05-06 04:26:38.000000 planetmagfields-1.4.3/planetMagFields.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-05-06 04:26:38.000000 planetmagfields-1.4.3/planetMagFields.egg-info/requires.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-05-06 04:26:38.000000 planetmagfields-1.4.3/planetMagFields.egg-info/top_level.txt
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-06 04:26:38.317649 planetmagfields-1.4.3/planetmagfields/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      159 2024-05-06 04:12:55.000000 planetmagfields-1.4.3/planetmagfields/__init__.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-06 04:26:38.317649 planetmagfields-1.4.3/planetmagfields/data/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/earth_igrf13.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/ganymede_kivelson2002.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/jupiter_jrm09.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/jupiter_jrm33.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/jupiter_vip4.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/mercury_anderson2012.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/mercury_thebault2018.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/mercury_wardinski2019.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/neptune_connerny1991.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/saturn_cassini11+.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/saturn_cassini11.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/saturn_cassinisoi.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/data/uranus_connerny1987.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     4701 2024-02-26 00:30:26.000000 planetmagfields-1.4.3/planetmagfields/libbfield.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3863 2024-02-26 01:09:53.000000 planetmagfields-1.4.3/planetmagfields/libdata.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/libgauss.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    11746 2024-04-30 14:44:50.000000 planetmagfields-1.4.3/planetmagfields/planet.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     6725 2024-04-30 14:45:13.000000 planetmagfields-1.4.3/planetmagfields/plotlib.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7835 2024-04-30 19:32:35.000000 planetmagfields-1.4.3/planetmagfields/potextra.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/planetmagfields/utils.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-05-06 04:13:08.000000 planetmagfields-1.4.3/pyproject.toml
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-05-06 04:26:38.327648 planetmagfields-1.4.3/setup.cfg
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-22 17:26:25.000000 planetmagfields-1.4.3/setup.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-06 04:26:38.327648 planetmagfields-1.4.3/tests/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      446 2024-04-30 18:47:40.000000 planetmagfields-1.4.3/tests/test_earthBr.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      702 2024-04-30 19:43:11.000000 planetmagfields-1.4.3/tests/test_potextra.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-04-30 20:14:46.000000 planetmagfields-1.4.3/tests/test_read.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      420 2024-04-30 20:52:34.000000 planetmagfields-1.4.3/tests/test_vtk.py
```

### Comparing `planetmagfields-1.4.2/LICENSE` & `planetmagfields-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/PKG-INFO` & `planetmagfields-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.2
+Version: 1.4.3
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
```

### Comparing `planetmagfields-1.4.2/README.md` & `planetmagfields-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetMagFields.egg-info/PKG-INFO` & `planetmagfields-1.4.3/planetMagFields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.2
+Version: 1.4.3
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
```

### Comparing `planetmagfields-1.4.2/planetMagFields.egg-info/SOURCES.txt` & `planetmagfields-1.4.3/planetMagFields.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -24,8 +24,11 @@
 planetmagfields/data/mercury_thebault2018.dat
 planetmagfields/data/mercury_wardinski2019.dat
 planetmagfields/data/neptune_connerny1991.dat
 planetmagfields/data/saturn_cassini11+.dat
 planetmagfields/data/saturn_cassini11.dat
 planetmagfields/data/saturn_cassinisoi.dat
 planetmagfields/data/uranus_connerny1987.dat
-tests/test_planetBr.py
+tests/test_earthBr.py
+tests/test_potextra.py
+tests/test_read.py
+tests/test_vtk.py
```

### Comparing `planetmagfields-1.4.2/planetmagfields/data/earth_igrf13.dat` & `planetmagfields-1.4.3/planetmagfields/data/earth_igrf13.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm09.dat` & `planetmagfields-1.4.3/planetmagfields/data/jupiter_jrm09.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm33.dat` & `planetmagfields-1.4.3/planetmagfields/data/jupiter_jrm33.dat`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/libbfield.py` & `planetmagfields-1.4.3/planetmagfields/libbfield.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/libdata.py` & `planetmagfields-1.4.3/planetmagfields/libdata.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/libgauss.py` & `planetmagfields-1.4.3/planetmagfields/libgauss.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/planet.py` & `planetmagfields-1.4.3/planetmagfields/planet.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/plotlib.py` & `planetmagfields-1.4.3/planetmagfields/plotlib.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/potextra.py` & `planetmagfields-1.4.3/planetmagfields/potextra.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/planetmagfields/utils.py` & `planetmagfields-1.4.3/planetmagfields/utils.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/pyproject.toml` & `planetmagfields-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "planetMagFields"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
 ]
 maintainers = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
   { name="Regupathi Angappan", email="rangapp1@jhu.edu" },
 ]
```

### Comparing `planetmagfields-1.4.2/setup.py` & `planetmagfields-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `planetmagfields-1.4.2/tests/test_planetBr.py` & `planetmagfields-1.4.3/tests/test_potextra.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-#!/usr/bin/env python3
-
 import numpy as np
 import os
 import sys
-
-def test_earthBr():
-    sys.path.append(os.path.abspath('../'))
-    from planetmagfields import Planet
-
-    p = Planet(name='earth',r=1,year=2016,nphi=256,info=False)
-
-    br_ref = np.loadtxt('earth/Br_reference.dat')
-    br = p.Br
-
-    br_ref /=1e3
-
-    err = np.abs( (br_ref - br)/br_ref )
-
-    np.testing.assert_allclose(err.mean(), 0, rtol=0.1,
-                                atol=0.1)
+sys.path.append(os.path.abspath('../'))
+from planetmagfields import Planet
 
 def test_jupiterBr():
-    sys.path.append(os.path.abspath('../'))
-    from planetmagfields import Planet
     p = Planet(name='jupiter',r=0.85,nphi=256,info=False,model='jrm33')
 
     br_ref = np.loadtxt('jupiter/Br_reference.dat')
     br = p.Br
 
     percent_err = np.abs( (br_ref - br)/br_ref ) * 100
 
     np.testing.assert_allclose(percent_err, 0, rtol=0.1,
-                                atol=0.1)
+                                atol=0.1)
+
+def test_potextra():
+    p = Planet(name='jupiter',r=10,nphi=256,info=False,model='jrm33')
+
+    br,btheta,bphi = p.extrapolate(np.array([10]))
+    br_ref = np.squeeze(br)
+    err = np.abs( (br_ref - p.Br) )
+
+    np.testing.assert_allclose(err, 0, rtol=1e-2, atol=1e-2)
```

