# Comparing `tmp/pyhisto-0.1.1.tar.gz` & `tmp/pyhisto-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhisto-0.1.1.tar", last modified: Thu Sep 22 09:47:23 2022, max compression
+gzip compressed data, was "dist/pyhisto-0.1.2.tar", last modified: Mon May  6 12:57:48 2024, max compression
```

## Comparing `pyhisto-0.1.1.tar` & `pyhisto-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2022-09-22 09:47:23.000000 pyhisto-0.1.1/
--rw-r--r--   0 ghenning  (7990) grace      (619)     5819 2022-09-22 09:47:23.000000 pyhisto-0.1.1/PKG-INFO
--rw-rw-rw-   0 ghenning  (7990) grace      (619)     4451 2020-09-17 13:50:44.000000 pyhisto-0.1.1/README.md
-drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto/
--rw-r--r--   0 ghenning  (7990) grace      (619)      547 2020-05-13 09:55:15.000000 pyhisto-0.1.1/pyhisto/__init__.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     7402 2020-08-31 12:46:18.000000 pyhisto-0.1.1/pyhisto/bin.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     1691 2020-05-13 12:06:01.000000 pyhisto-0.1.1/pyhisto/ghosthistogram.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     1930 2020-05-13 12:23:37.000000 pyhisto-0.1.1/pyhisto/ghosthistogram2D.py
--rw-r--r--   0 ghenning  (7990) grace      (619)    13750 2020-05-19 14:08:32.000000 pyhisto-0.1.1/pyhisto/histogram.py
--rw-r--r--   0 ghenning  (7990) grace      (619)    15340 2020-09-02 08:16:58.000000 pyhisto-0.1.1/pyhisto/histogram2D.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     2784 2020-05-14 08:37:29.000000 pyhisto-0.1.1/pyhisto/lazyhistogram.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     3308 2020-05-13 11:58:39.000000 pyhisto-0.1.1/pyhisto/lazyhistogram2D.py
-drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto/tools/
--rw-r--r--   0 ghenning  (7990) grace      (619)      221 2020-05-13 09:46:28.000000 pyhisto-0.1.1/pyhisto/tools/__init__.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     1109 2020-05-26 08:39:27.000000 pyhisto-0.1.1/pyhisto/tools/findpeaks.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     3420 2022-09-22 09:39:23.000000 pyhisto-0.1.1/pyhisto/tools/gaussfit.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     4239 2022-09-22 09:42:19.000000 pyhisto-0.1.1/pyhisto/tools/gaussrealfit.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     2096 2020-06-26 13:19:36.000000 pyhisto-0.1.1/pyhisto/tools/parzen_estimator.py
--rw-r--r--   0 ghenning  (7990) grace      (619)     1051 2020-05-26 08:09:24.000000 pyhisto-0.1.1/pyhisto/tools/stats.py
-drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto.egg-info/
--rw-rw-rw-   0 ghenning  (7990) grace      (619)     5819 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto.egg-info/PKG-INFO
--rw-rw-rw-   0 ghenning  (7990) grace      (619)      493 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto.egg-info/SOURCES.txt
--rw-rw-rw-   0 ghenning  (7990) grace      (619)        1 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto.egg-info/dependency_links.txt
--rw-rw-rw-   0 ghenning  (7990) grace      (619)        8 2022-09-22 09:47:23.000000 pyhisto-0.1.1/pyhisto.egg-info/top_level.txt
--rw-r--r--   0 ghenning  (7990) grace      (619)       38 2022-09-22 09:47:23.000000 pyhisto-0.1.1/setup.cfg
--rw-r--r--   0 ghenning  (7990) grace      (619)     1000 2022-09-22 09:46:58.000000 pyhisto-0.1.1/setup.py
+drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2024-05-06 12:57:48.562320 pyhisto-0.1.2/
+-rw-r--r--   0 ghenning  (7990) grace      (619)     5819 2024-05-06 12:57:48.562320 pyhisto-0.1.2/PKG-INFO
+-rw-r--r--   0 ghenning  (7990) grace      (619)     4451 2024-03-28 10:00:44.000000 pyhisto-0.1.2/README.md
+drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2024-05-06 12:57:48.560320 pyhisto-0.1.2/pyhisto/
+-rw-r--r--   0 ghenning  (7990) grace      (619)      547 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/__init__.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     7402 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/bin.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     1691 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/ghosthistogram.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     1930 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/ghosthistogram2D.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)    13750 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/histogram.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)    15340 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/histogram2D.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     2784 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/lazyhistogram.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     3308 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/lazyhistogram2D.py
+drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2024-05-06 12:57:48.562320 pyhisto-0.1.2/pyhisto/tools/
+-rw-r--r--   0 ghenning  (7990) grace      (619)      221 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/tools/__init__.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     1109 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/tools/findpeaks.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     3420 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/tools/gaussfit.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     4487 2024-05-06 12:56:36.000000 pyhisto-0.1.2/pyhisto/tools/gaussrealfit.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     2096 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/tools/parzen_estimator.py
+-rw-r--r--   0 ghenning  (7990) grace      (619)     1051 2024-03-28 10:00:44.000000 pyhisto-0.1.2/pyhisto/tools/stats.py
+drwxr-xr-x   0 ghenning  (7990) grace      (619)        0 2024-05-06 12:57:48.561320 pyhisto-0.1.2/pyhisto.egg-info/
+-rw-r--r--   0 ghenning  (7990) grace      (619)     5819 2024-05-06 12:57:48.000000 pyhisto-0.1.2/pyhisto.egg-info/PKG-INFO
+-rw-r--r--   0 ghenning  (7990) grace      (619)      493 2024-05-06 12:57:48.000000 pyhisto-0.1.2/pyhisto.egg-info/SOURCES.txt
+-rw-r--r--   0 ghenning  (7990) grace      (619)        1 2024-05-06 12:57:48.000000 pyhisto-0.1.2/pyhisto.egg-info/dependency_links.txt
+-rw-r--r--   0 ghenning  (7990) grace      (619)        8 2024-05-06 12:57:48.000000 pyhisto-0.1.2/pyhisto.egg-info/top_level.txt
+-rw-r--r--   0 ghenning  (7990) grace      (619)       38 2024-05-06 12:57:48.562320 pyhisto-0.1.2/setup.cfg
+-rw-r--r--   0 ghenning  (7990) grace      (619)     1000 2024-05-03 14:08:00.000000 pyhisto-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhisto-0.1.1/PKG-INFO` & `pyhisto-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhisto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Histogram Library
 Home-page: https://gitlab.in2p3.fr/gregoire.henning/pyhisto
 Author: Greg Henning
 Author-email: ghenning@iphc.cnrs.fr
 License: UNKNOWN
 Description: # Python Histogram module
```

### Comparing `pyhisto-0.1.1/README.md` & `pyhisto-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/__init__.py` & `pyhisto-0.1.2/pyhisto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/bin.py` & `pyhisto-0.1.2/pyhisto/bin.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/ghosthistogram.py` & `pyhisto-0.1.2/pyhisto/ghosthistogram.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/ghosthistogram2D.py` & `pyhisto-0.1.2/pyhisto/ghosthistogram2D.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/histogram.py` & `pyhisto-0.1.2/pyhisto/histogram.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/histogram2D.py` & `pyhisto-0.1.2/pyhisto/histogram2D.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/lazyhistogram.py` & `pyhisto-0.1.2/pyhisto/lazyhistogram.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/lazyhistogram2D.py` & `pyhisto-0.1.2/pyhisto/lazyhistogram2D.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/tools/findpeaks.py` & `pyhisto-0.1.2/pyhisto/tools/findpeaks.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/tools/gaussfit.py` & `pyhisto-0.1.2/pyhisto/tools/gaussfit.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/tools/gaussrealfit.py` & `pyhisto-0.1.2/pyhisto/tools/gaussrealfit.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,32 +39,34 @@
 except ImportError:
     raise ImportError("Could not implement Real Fit because `numpy` and `scipy` are not availble")
 
 
 class GaussRealFit:
     '''From an histogram, extract Gaussian 'fitted' parameters '''
     def __init__(self,
-                 h: Histogram):
+                 h: Histogram,
+                 _xguess: float = None,
+                 _stdevguess: float = None):
         '''computes sum, average x, stddev, max, bin'''
         self.h1 = h
         _simplefit = GaussFit(self.h1)
 
         def GaussFunc(x,
                       S, M, R,
                       B, SL):
             return B + SL * (x - M) + S / np.sqrt(2. * pi * R * R) * np.exp(-(x - M) ** 2. / 2. / R / R)
 
         first_guess = [_simplefit.integral,
-                       _simplefit.mean,
-                       _simplefit.stdev,
-                       self.h1[0].count,
+                       _xguess or _simplefit.mean,
+                       _stdevguess or _simplefit.stdev,
+                       sum(self.h1)/(1. + len(self.h1)), # background guess
                        0.0]
-        limits = list(zip((0., np.inf),
-                          (self.h1[0].lowedge, self.h1[-1].upedge),
-                          (0., np.inf),
+        limits = list(zip((0., np.inf), # sum
+                          (self.h1[0].lowedge, self.h1[-1].upedge), # gaussian center
+                          (0., (self.h1[-1].upedge - self.h1[0].lowedge)), # stddev max is the width of the histogram
                           (-np.inf, np.inf),
                           (-np.inf, np.inf)
                           ))
         fitrslt, cov = curve_fit(GaussFunc,
                                  *self.h1.xy(),
                                  p0=first_guess,
                                  bounds=limits)
@@ -100,17 +102,17 @@
     def plot(self,
              target='screen'):
         '''Plot in a new figure (alone) and send to `target` (screen or file)'''
         plt.figure()
         plt.grid(True)
         plt.step(*self.h1.xy(), label='original')
         plt.step(*self.background.xy(), label='background')
-        plt.step(*self.bgsubstracted.xy(), label='bacground subracted')
+        plt.step(*self.bgsubstracted.xy(), label='background subracted')
         plt.step(*self.gaussian.xy(), label='Gaussian')
-        plt.step(*self.residuals.xy(), label='residual')
+        plt.step(*self.residuals.xy(), label='Residual')
         plt.legend()
         if target == 'screen':
             plt.show()
         else:
             plt.savefig(target)
 
     def __repr__(self) -> str:
```

### Comparing `pyhisto-0.1.1/pyhisto/tools/parzen_estimator.py` & `pyhisto-0.1.2/pyhisto/tools/parzen_estimator.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto/tools/stats.py` & `pyhisto-0.1.2/pyhisto/tools/stats.py`

 * *Files identical despite different names*

### Comparing `pyhisto-0.1.1/pyhisto.egg-info/PKG-INFO` & `pyhisto-0.1.2/pyhisto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhisto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Histogram Library
 Home-page: https://gitlab.in2p3.fr/gregoire.henning/pyhisto
 Author: Greg Henning
 Author-email: ghenning@iphc.cnrs.fr
 License: UNKNOWN
 Description: # Python Histogram module
```

### Comparing `pyhisto-0.1.1/setup.py` & `pyhisto-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 '''
 Module docstring
 '''
 
 from setuptools import setup
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(name='pyhisto',
```

