# Comparing `tmp/bettermoments-1.8.5.tar.gz` & `tmp/bettermoments-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettermoments-1.8.5.tar", last modified: Mon Apr  3 19:55:57 2023, max compression
+gzip compressed data, was "bettermoments-1.8.6.tar", last modified: Mon May  6 13:58:01 2024, max compression
```

## Comparing `bettermoments-1.8.5.tar` & `bettermoments-1.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-03 19:55:57.210764 bettermoments-1.8.5/
--rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:29:43.000000 bettermoments-1.8.5/LICENSE.md
--rw-r--r--   0 richardteague   (501) staff       (20)     2182 2023-04-03 19:55:57.210650 bettermoments-1.8.5/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     1581 2023-03-27 18:29:43.000000 bettermoments-1.8.5/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-03 19:55:57.209522 bettermoments-1.8.5/bettermoments/
--rw-r--r--   0 richardteague   (501) staff       (20)      215 2023-03-27 18:29:43.000000 bettermoments-1.8.5/bettermoments/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    19751 2023-04-03 18:23:48.000000 bettermoments-1.8.5/bettermoments/collapse_cube.py
--rw-r--r--   0 richardteague   (501) staff       (20)    12642 2023-04-03 19:52:25.000000 bettermoments-1.8.5/bettermoments/io.py
--rw-r--r--   0 richardteague   (501) staff       (20)    12014 2023-03-27 18:29:43.000000 bettermoments-1.8.5/bettermoments/mcmc_sampling.py
--rw-r--r--   0 richardteague   (501) staff       (20)    29263 2023-04-03 19:55:28.000000 bettermoments-1.8.5/bettermoments/methods.py
--rw-r--r--   0 richardteague   (501) staff       (20)     7827 2023-03-27 18:29:43.000000 bettermoments-1.8.5/bettermoments/profiles.py
--rw-r--r--   0 richardteague   (501) staff       (20)     5032 2023-03-27 18:29:43.000000 bettermoments-1.8.5/bettermoments/quadratic.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-03 19:55:57.210352 bettermoments-1.8.5/bettermoments.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)     2182 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      471 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       67 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/entry_points.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       47 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       14 2023-04-03 19:55:57.000000 bettermoments-1.8.5/bettermoments.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-03-30 21:36:03.000000 bettermoments-1.8.5/bettermoments.egg-info/zip-safe
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-04-03 19:55:57.210805 bettermoments-1.8.5/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)     1240 2023-04-03 18:25:23.000000 bettermoments-1.8.5/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-06 13:58:01.225461 bettermoments-1.8.6/
+-rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:29:43.000000 bettermoments-1.8.6/LICENSE.md
+-rw-r--r--   0 richardteague   (501) staff       (20)     2182 2024-05-06 13:58:01.225343 bettermoments-1.8.6/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     1581 2023-03-27 18:29:43.000000 bettermoments-1.8.6/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-06 13:58:01.224427 bettermoments-1.8.6/bettermoments/
+-rw-r--r--   0 richardteague   (501) staff       (20)      215 2023-03-27 18:29:43.000000 bettermoments-1.8.6/bettermoments/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    20272 2024-05-06 13:53:32.000000 bettermoments-1.8.6/bettermoments/collapse_cube.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    12642 2023-04-03 19:52:25.000000 bettermoments-1.8.6/bettermoments/io.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    12014 2023-03-27 18:29:43.000000 bettermoments-1.8.6/bettermoments/mcmc_sampling.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    29288 2023-04-03 20:09:22.000000 bettermoments-1.8.6/bettermoments/methods.py
+-rw-r--r--   0 richardteague   (501) staff       (20)     7827 2023-03-27 18:29:43.000000 bettermoments-1.8.6/bettermoments/profiles.py
+-rw-r--r--   0 richardteague   (501) staff       (20)     5032 2023-03-27 18:29:43.000000 bettermoments-1.8.6/bettermoments/quadratic.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-06 13:58:01.225203 bettermoments-1.8.6/bettermoments.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)     2182 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      471 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       67 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/entry_points.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       47 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       14 2024-05-06 13:58:01.000000 bettermoments-1.8.6/bettermoments.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-03-30 21:36:03.000000 bettermoments-1.8.6/bettermoments.egg-info/zip-safe
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-05-06 13:58:01.225496 bettermoments-1.8.6/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)     1240 2024-05-06 13:52:18.000000 bettermoments-1.8.6/setup.py
```

### Comparing `bettermoments-1.8.5/LICENSE.md` & `bettermoments-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/PKG-INFO` & `bettermoments-1.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettermoments
-Version: 1.8.5
+Version: 1.8.6
 Summary: Robust moment map making.
 Home-page: https://github.com/richteague/bettermoments
 Author: Richard Teague & Daniel Foreman-Mackey
 Author-email: rteague@mit.edu
 License: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bettermoments Version: 1.8.5 Summary: Robust moment
+Metadata-Version: 2.1 Name: bettermoments Version: 1.8.6 Summary: Robust moment
 map making. Home-page: https://github.com/richteague/bettermoments Author:
 Richard Teague & Daniel Foreman-Mackey Author-email: rteague@mit.edu License:
 LICENSE.md Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE.md #
```

### Comparing `bettermoments-1.8.5/README.md` & `bettermoments-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/bettermoments/collapse_cube.py` & `bettermoments-1.8.6/bettermoments/collapse_cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     else:
         from .io import _get_data
         user_mask = np.where(_get_data(user_mask_path) > 0, 1.0, 0.0)
     assert user_mask.shape == data.shape
     return user_mask.astype('float')
 
 
-def get_threshold_mask(data, clip=None, smooth_threshold_mask=0,
+def get_threshold_mask(data, clip=None, rms=None, smooth_threshold_mask=0,
                        noise_channels=5):
     """
     Returns a mask based on a sigma-clip to the input data. The most standard
     approach would be to use ``clip=3`` to mask out all pixels with intensities
     :math:`|I| \leq 3\sigma`. If you wanted to specify an asymmetric criteria
     then you can provide a tuple, ``clip=(-2, 3)`` which would mask out all
     pixels where :math:`-2\sigma \leq I \leq 3\sigma`.
@@ -133,14 +133,17 @@
     [Some discussion on the smooth_threshold_mask coming...]
 
     Args:
         data (array): The data array to mask.
         clip (optional[float/tuple]): The sigma clip to apply. If a single
             value is provided, this is taken to be a symmetric mask. If a tuple
             if provided, this is taking as a minimum and maximum clip value.
+        rms (optional[float]): The RMS level to use for defining the noise. If
+            not specified, will calculate it based on the standard deviation of
+            the data.
         smooth_threshold_mask (optional[float]): Convolution kernel FWHM in
             pixels.
         noise_channels (optional[int]): Number of channels at the start and end
             of the velocity axis to use for estimating the noise.
 
     Returns:
         threshold_mask (array): A mask array the same shape as ``data``.
@@ -164,15 +167,23 @@
     assert smooth_threshold_mask >= 0.0
     if smooth_threshold_mask > 0.0:
         from scipy.ndimage import gaussian_filter
         SNR = [gaussian_filter(c, sigma=smooth_threshold_mask) for c in data]
         SNR = np.array(SNR)
     else:
         SNR = data.copy()
-    SNR /= estimate_RMS(SNR, noise_channels)
+
+    # Select the right RMS to use for the SNR calculate. If the RMS is provided,
+    # which is the default, we use that, otherwise we calculate it based on the
+    # standard deviation of (hopefully) line-free channels.
+
+    if rms is None:
+        SNR /= estimate_RMS(SNR, noise_channels)
+    else:
+        SNR /= rms
 
     # Return the mask.
 
     return np.logical_or(SNR < clip[0], SNR > clip[-1]).astype('float')
 
 
 def get_combined_mask(user_mask, threshold_mask, channel_mask, combine='and'):
@@ -322,14 +333,15 @@
     # Define the threshold mask. This includes the spatial smoothing of the
     # data for create Frankenmasks.
 
     if not args.silent and args.clip is not None:
         print("Calculating threshold-based mask...")
     threshold_mask = get_threshold_mask(data=data,
                                         clip=args.clip,
+                                        rms=args.rms,
                                         smooth_threshold_mask=args.smooththreshold,
                                         noise_channels=args.noisechannels)
     if args.debug:
         from .io import _save_threshold_mask
         _save_threshold_mask(threshold_mask, args)
 
     # Combine the masks and apply to the data.
```

### Comparing `bettermoments-1.8.5/bettermoments/io.py` & `bettermoments-1.8.6/bettermoments/io.py`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/bettermoments/mcmc_sampling.py` & `bettermoments-1.8.6/bettermoments/mcmc_sampling.py`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/bettermoments/methods.py` & `bettermoments-1.8.6/bettermoments/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     # Dummy arrays.
 
     wp = np.ones((3, data.shape[1], data.shape[2]))
     dwp = np.ones(wp.shape)
 
     # Calculate the weighted percentiles.
 
-    weights = np.cumsum(data.copy(), axis=0)
+    weights = np.cumsum(np.clip(data, a_min=0.0, a_max=None), axis=0)
     weights /= weights[-1]
     pcnts = np.array([0.16, 0.5, 0.84])
 
     # Loop through the pixels fiding the right values.
 
     with tqdm(total=data.shape[1]*data.shape[2]) as pbar:
         for i in range(weights.shape[2]):
```

### Comparing `bettermoments-1.8.5/bettermoments/profiles.py` & `bettermoments-1.8.6/bettermoments/profiles.py`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/bettermoments/quadratic.py` & `bettermoments-1.8.6/bettermoments/quadratic.py`

 * *Files identical despite different names*

### Comparing `bettermoments-1.8.5/bettermoments.egg-info/PKG-INFO` & `bettermoments-1.8.6/bettermoments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettermoments
-Version: 1.8.5
+Version: 1.8.6
 Summary: Robust moment map making.
 Home-page: https://github.com/richteague/bettermoments
 Author: Richard Teague & Daniel Foreman-Mackey
 Author-email: rteague@mit.edu
 License: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bettermoments Version: 1.8.5 Summary: Robust moment
+Metadata-Version: 2.1 Name: bettermoments Version: 1.8.6 Summary: Robust moment
 map making. Home-page: https://github.com/richteague/bettermoments Author:
 Richard Teague & Daniel Foreman-Mackey Author-email: rteague@mit.edu License:
 LICENSE.md Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE.md #
```

### Comparing `bettermoments-1.8.5/setup.py` & `bettermoments-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setuptools.setup(
     name="bettermoments",
-    version="1.8.5",
+    version="1.8.6",
     author="Richard Teague & Daniel Foreman-Mackey",
     author_email='rteague@mit.edu',
     packages=["bettermoments"],
     url="https://github.com/richteague/bettermoments",
     license="LICENSE.md",
     description=("Robust moment map making."),
     long_description=long_description,
```

