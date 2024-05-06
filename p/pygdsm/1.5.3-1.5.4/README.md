# Comparing `tmp/pygdsm-1.5.3.tar.gz` & `tmp/pygdsm-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdsm-1.5.3.tar", last modified: Mon Apr 15 07:44:57 2024, max compression
+gzip compressed data, was "pygdsm-1.5.4.tar", last modified: Mon May  6 06:29:05 2024, max compression
```

## Comparing `pygdsm-1.5.3.tar` & `pygdsm-1.5.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 07:44:37.000000 pygdsm-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:44:37.000000 pygdsm-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 07:44:57.224067 pygdsm-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-15 07:44:37.000000 pygdsm-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.220067 pygdsm-1.5.3/pygdsm/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/base_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/base_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/component_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/gsm08.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/gsm16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/lfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/pygdsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 07:44:37.000000 pygdsm-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 07:44:37.000000 pygdsm-1.5.3/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 07:44:57.224067 pygdsm-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 07:44:37.000000 pygdsm-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm2016.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_lfsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:29:05.326249 pygdsm-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 06:28:27.000000 pygdsm-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 06:28:27.000000 pygdsm-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-06 06:29:05.326249 pygdsm-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-06 06:28:27.000000 pygdsm-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:29:05.322249 pygdsm-1.5.4/pygdsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/base_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/base_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/component_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/gsm08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/gsm16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/lfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-06 06:28:27.000000 pygdsm-1.5.4/pygdsm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:29:05.326249 pygdsm-1.5.4/pygdsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-06 06:29:05.000000 pygdsm-1.5.4/pygdsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-06 06:29:05.000000 pygdsm-1.5.4/pygdsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:29:05.000000 pygdsm-1.5.4/pygdsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 06:29:05.000000 pygdsm-1.5.4/pygdsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 06:29:05.000000 pygdsm-1.5.4/pygdsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 06:28:27.000000 pygdsm-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 06:28:27.000000 pygdsm-1.5.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 06:29:05.326249 pygdsm-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-06 06:28:27.000000 pygdsm-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:29:05.322249 pygdsm-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_base_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_gsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_gsm2016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_gsm_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_lfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 06:28:27.000000 pygdsm-1.5.4/tests/test_utils.py
```

### Comparing `pygdsm-1.5.3/LICENSE` & `pygdsm-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/PKG-INFO` & `pygdsm-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
 Author: Danny C. Price
 Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pygdsm-1.5.3/README.md` & `pygdsm-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/__init__.py` & `pygdsm-1.5.4/pygdsm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/base_observer.py` & `pygdsm-1.5.4/pygdsm/base_observer.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/base_skymodel.py` & `pygdsm-1.5.4/pygdsm/base_skymodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import numpy as np
 import h5py
 import healpy as hp
 from astropy.io import fits
 from .plot_utils import show_plt
 
 def is_fits(filepath):
@@ -13,20 +14,20 @@
     ----------
     filepath: str
         Path to file
     """
     FITS_SIGNATURE = (b"\x53\x49\x4d\x50\x4c\x45\x20\x20\x3d\x20\x20\x20\x20\x20"
                       b"\x20\x20\x20\x20\x20\x20\x20\x20\x20\x20\x20\x20\x20\x20"
                       b"\x20\x54")
-    with open(str(filepath),'rb') as f:
-        try:
+    try:
+        with open(str(filepath),'rb') as f:
             return f.read(30) == FITS_SIGNATURE
-        except FileNotFoundError as e:
-            print(e)
-            return False
+    except FileNotFoundError as e:
+        print(e)
+        return False
 
 
 class BaseSkyModel(object):
     """ Global sky model (GSM) class for generating sky models.
     """
     def __init__(self, name, filepath, freq_unit, data_unit, basemap):
         """ Initialise basic sky model class
@@ -40,20 +41,23 @@
         basemap (str):   Map used as a basis for spatial structure in PCA fit.
 
         Notes
         -----
         Any GSM needs to supply a generate() function
         """
         self.name = name
-        if h5py.is_hdf5(filepath):
-            self.h5 = h5py.File(filepath, "r")
-        elif is_fits(filepath):
-            self.fits = fits.open(filepath, "readonly")
+        if os.path.exists(filepath):
+            if h5py.is_hdf5(filepath):
+                self.h5 = h5py.File(filepath, "r")
+            elif is_fits(filepath):
+                self.fits = fits.open(filepath, "readonly")
+            else:
+                raise RuntimeError(f"Cannot read HDF5/FITS file {filepath}")
         else:
-            raise RuntimeError(f"Cannot read HDF5/FITS file {filepath}")
+            raise RuntimeError(f"Cannot find {filepath}")
         self.basemap = basemap
         self.freq_unit = freq_unit
         self.data_unit = data_unit
 
         self.generated_map_data = None
         self.generated_map_freqs = None
 
@@ -86,34 +90,34 @@
         if logged:
             gmap = np.log2(gmap)
 
         hp.mollview(gmap, coord='G', title='%s %s, %s' % (self.name, str(freq), self.basemap))
 
         if show:
             show_plt()
-    
+
     def get_sky_temperature(self, coords, freqs=None, include_cmb=True):
         """ Get sky temperature at given coordinates.
 
         Returns sky temperature at a given SkyCoord (e.g. Ra/Dec or galactic l/b).
         Useful for estimating sky contribution to system temperature.
 
         Parameters
         ----------
-        coords (astropy.coordinates.SkyCoord): 
+        coords (astropy.coordinates.SkyCoord):
             Sky Coordinates to compute temperature for.
         freqs (None, float, or np.array):
-            frequencies to evaluate. If not set, will default to those supplied 
+            frequencies to evaluate. If not set, will default to those supplied
             when generate() was called.
-        include_cmb (bool): 
+        include_cmb (bool):
             Include a 2.725 K contribution from the CMB (default True).
         """
-        
+
         T_cmb = 2.725 if include_cmb else 0
-        
+
         if freqs is not None:
             self.generate(freqs)
 
         pix = hp.ang2pix(self.nside, coords.galactic.l.deg, coords.galactic.b.deg, lonlat=True)
         if self.generated_map_data.ndim == 2:
             return self.generated_map_data[:, pix] + T_cmb
         else:
```

### Comparing `pygdsm-1.5.3/pygdsm/component_data.py` & `pygdsm-1.5.4/pygdsm/component_data.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/gsm08.py` & `pygdsm-1.5.4/pygdsm/gsm08.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/gsm16.py` & `pygdsm-1.5.4/pygdsm/gsm16.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm/haslam.py` & `pygdsm-1.5.4/pygdsm/haslam.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Dickinson et al (2019), C-BASS experiment, https://doi.org/10.1093/mnras/stz522
         """
         data_unit = 'K'
         basemap = 'Haslam'
 
         super(HaslamSkyModel, self).__init__('Haslam', HASLAM_FILEPATH, freq_unit, data_unit, basemap)
         self.spectral_index = spectral_index
-        self.data = hp.read_map(self.fits, verbose=False, dtype=np.float64) - T_CMB
+        self.data = hp.read_map(self.fits, dtype=np.float64) - T_CMB
         self.nside = 512
 
         self.include_cmb = include_cmb
 
     def generate(self, freqs):
         """ Generate a global sky model at a given frequency or frequencies
```

### Comparing `pygdsm-1.5.3/pygdsm/lfsm.py` & `pygdsm-1.5.4/pygdsm/lfsm.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/pygdsm.egg-info/PKG-INFO` & `pygdsm-1.5.4/pygdsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
 Author: Danny C. Price
 Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pygdsm-1.5.3/pygdsm.egg-info/SOURCES.txt` & `pygdsm-1.5.4/pygdsm.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 pygdsm/base_skymodel.py
 pygdsm/component_data.py
 pygdsm/gsm08.py
 pygdsm/gsm16.py
 pygdsm/haslam.py
 pygdsm/lfsm.py
 pygdsm/plot_utils.py
+pygdsm/utils.py
 pygdsm.egg-info/PKG-INFO
 pygdsm.egg-info/SOURCES.txt
 pygdsm.egg-info/dependency_links.txt
 pygdsm.egg-info/requires.txt
 pygdsm.egg-info/top_level.txt
+tests/test_base_skymodel.py
 tests/test_gsm.py
 tests/test_gsm2016.py
 tests/test_gsm_observer.py
 tests/test_haslam.py
-tests/test_lfsm.py
+tests/test_init.py
+tests/test_lfsm.py
+tests/test_utils.py
```

### Comparing `pygdsm-1.5.3/setup.py` & `pygdsm-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 setup(
     name='pygdsm',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.5.3',
+    version='1.5.4',
 
     description='Python Global Sky Model of diffuse Galactic radio emission',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/telegraphic/pygdsm',
```

### Comparing `pygdsm-1.5.3/tests/test_gsm.py` & `pygdsm-1.5.4/tests/test_gsm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 test_gsm.py
 ===========
 
 Tests for GSM module.
 """
 
-import os
 from pygdsm import GlobalSkyModel
-from pygdsm import init_gsm, init_observer
+from pygdsm.component_data import GSM2008_TEST_DATA
 
+import os
 import time
+import pytest
 import numpy as np
 import h5py
 import healpy as hp
+from astropy.coordinates import SkyCoord
+
 
 def test_gsm_generate():
     """ Test maps generate successfully, and that output shapes are correct. """
 
     freq = 40
     gsm = GlobalSkyModel()
     map = gsm.generate(freq)
@@ -31,15 +34,15 @@
     freq_unit = 'GHz'
     for map_id in ['5deg', 'haslam', 'wmap']:
         gsm = GlobalSkyModel(basemap=map_id, interpolation='pchip', freq_unit=freq_unit)
         map = gsm.generate(freqs)
         assert map.shape == (10, 3145728)
 
 
-def compare_to_gsm():
+def test_compare_to_gsm():
     """ Compare output of python version to fortran version.
 
     Compares against output of original GSM. Note that the interpolation
     functions used in this and in the original differ. So, the outputs
     differ too, by as much as 5%. This just goes to show that there's only
     so much accuracy that one can get via interpolation.
 
@@ -48,23 +51,26 @@
     is required. In between maps is where the differences will become more apparent.
 
     Note: The gsm.f that is supplied only ever uses the haslam map. It also
           has no option to change the interpolation method.
 
     Note: Because each output
     """
-    gsm = GlobalSkyModel(basemap='haslam', interpolation='cubic')
-    gsm_fortran = h5py.File('gsm_fortran_test_data.h5', 'r')
+    gsm = GlobalSkyModel(basemap='haslam', interpolation='pchip')
+    gsm_fortran = h5py.File(GSM2008_TEST_DATA, 'r')
     for freq in (10, 100, 408, 1000, 1420, 2326, 10000, 23000, 40000, 90000, 94000):
         print("\nComparing at %i MHz..." % freq)
         a = gsm_fortran['map_%imhz.out' % freq][:]
         b = gsm.generate(freq)
-        print("FORTRAN: ", a)
-        print("PYTHON:  ", b)
-        print("FRAC AVG: %2.6f" % np.average(np.abs(1 - a/b)))
+        frac_avg = np.average(np.abs(1 - a/b))
+        if frac_avg > 0.01:
+            print("FORTRAN: ", a)
+            print("PYTHON:  ", b)
+            print(f"FRAC AVG: {frac_avg:.6f}")
+        assert frac_avg < 0.035
 
 
 def test_set_methods():
 
     gsm = GlobalSkyModel()
     gsm.generate(40)
     #gsm.view()
@@ -111,15 +117,41 @@
     g = GlobalSkyModel(freq_unit='MHz',  include_cmb=True)
     sky_with_cmb = g.generate(400)
 
     T_cmb = (sky_with_cmb - sky_no_cmb).mean()
     print(T_cmb)
     assert np.isclose(T_cmb, 2.725)
 
+def test_get_sky_temperature():
+    gc = SkyCoord(0, 0, unit='deg', frame='galactic')
+    freqs = (50, 100, 150)
+    g = GlobalSkyModel()
+    T = g.get_sky_temperature(gc, freqs)
+
+    T_gold = np.array([258368.7463149 ,  50466.45058671,  18968.12555978])
+    assert np.allclose(T, T_gold)
+
+def test_stupid_values():
+    with pytest.raises(RuntimeError):
+        g = GlobalSkyModel(basemap='haslamalan')
+    with pytest.raises(RuntimeError):
+        g = GlobalSkyModel(interpolation='linear')
+    with pytest.raises(RuntimeError):
+        g = GlobalSkyModel()
+        g.generate(9999999999)
+
+def test_set_interpolation_method():
+    g = GlobalSkyModel(interpolation='pchip')
+    assert g.interpolation_method == 'pchip'
+    g.set_interpolation_method('cubic')
+    assert g.interpolation_method == 'cubic'
 
 if __name__ == "__main__":
+    test_stupid_values()
+    test_set_interpolation_method()
     test_gsm_generate()
-    compare_to_gsm()
+    test_compare_to_gsm()
     test_speed()
     test_write_fits()
     test_set_methods()
     test_cmb_removal()
+    test_get_sky_temperature()
```

### Comparing `pygdsm-1.5.3/tests/test_gsm2016.py` & `pygdsm-1.5.4/tests/test_gsm2016.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/tests/test_gsm_observer.py` & `pygdsm-1.5.4/tests/test_gsm_observer.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/tests/test_haslam.py` & `pygdsm-1.5.4/tests/test_haslam.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.3/tests/test_lfsm.py` & `pygdsm-1.5.4/tests/test_lfsm.py`

 * *Files identical despite different names*

