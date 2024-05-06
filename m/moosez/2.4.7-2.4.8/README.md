# Comparing `tmp/moosez-2.4.7.tar.gz` & `tmp/moosez-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.7.tar", last modified: Tue Apr 23 18:28:25 2024, max compression
+gzip compressed data, was "moosez-2.4.8.tar", last modified: Mon May  6 19:52:34 2024, max compression
```

## Comparing `moosez-2.4.7.tar` & `moosez-2.4.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 18:28:18.000000 moosez-2.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 18:28:25.191945 moosez-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-04-23 18:28:18.000000 moosez-2.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-04-23 18:28:18.000000 moosez-2.4.7/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:28:25.191945 moosez-2.4.7/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 18:28:25.000000 moosez-2.4.7/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:28:25.191945 moosez-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 18:28:18.000000 moosez-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 19:52:30.000000 moosez-2.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 19:52:34.550170 moosez-2.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-06 19:52:30.000000 moosez-2.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.546170 moosez-2.4.8/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:52:34.550170 moosez-2.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 19:52:30.000000 moosez-2.4.8/setup.py
```

### Comparing `moosez-2.4.7/LICENSE` & `moosez-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/PKG-INFO` & `moosez-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.7
+Version: 2.4.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.7/README.md` & `moosez-2.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -311,14 +311,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Keyn34"><img src="https://github.com/Keyn34.png?s=100" width="100px;" alt="Sebastian Gutschmayer"/><br /><sub><b>Sebastian Gutschmayer</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=Keyn34" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/n7k-dobri"><img src="https://avatars.githubusercontent.com/u/114534264?v=4?s=100" width="100px;" alt="n7k-dobri"/><br /><sub><b>n7k-dobri</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=n7k-dobri" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mprires"><img src="https://avatars.githubusercontent.com/u/48754309?v=4?s=100" width="100px;" alt="Manuel Pires"/><br /><sub><b>Manuel Pires</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=mprires" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.meduniwien.ac.at/web/forschung/researcher-profiles/researcher-profiles/index.php?id=688&res=zacharias_chalampalakis1"><img src="https://avatars.githubusercontent.com/u/62066397?v=4?s=100" width="100px;" alt="Zach Chalampalakis"/><br /><sub><b>Zach Chalampalakis</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=zax0s" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dhaberl"><img src="https://avatars.githubusercontent.com/u/54232863?v=4?s=100" width="100px;" alt="David Haberl"/><br /><sub><b>David Haberl</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=dhaberl" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/W7ebere"><img src="https://avatars.githubusercontent.com/u/166598214?v=4?s=100" width="100px;" alt="W7ebere"/><br /><sub><b>W7ebere</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=W7ebere" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Kazezaka"><img src="https://avatars.githubusercontent.com/u/29598301?v=4?s=100" width="100px;" alt="Kazezaka"/><br /><sub><b>Kazezaka</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=Kazezaka" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `moosez-2.4.7/moosez/constants.py` & `moosez-2.4.8/moosez/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,24 +293,20 @@
         6: "Pancreas",
         7: "Adrenal Glands",
         8: "Lungs",
         9: "Heart",
         10: "Vessels",
         11: "Esophagus",
         12: "Trachea",
-        13: "Small_bowel",
-        14: "Duodenum",
-        15: "Colon",
-        16: "Brain",
-        17: "Skeleton",
-        18: "Subcutaneous_fat",
-        19: "Visceral fat",
-        20: "Muscles",
-        21: "Bladder",
-        22: "Filler"
+        13: "Digestive",
+        14: "Brain",
+        15: "Skeleton",
+        16: "Muscles",
+        17: "Bladder",
+        18: "Filler"
     },
     "clin_pt_fdg_brain_v1": {
         0: "background",
         1: "R-Hippocampus",
         2: "L-Hippocampus",
         3: "R-Amygdala",
         4: "L-Amygdala",
@@ -412,24 +408,20 @@
         6: "Pancreas",
         7: "Adrenal Glands",
         8: "Lungs",
         9: "Heart",
         10: "Vessels",
         11: "Esophagus",
         12: "Trachea",
-        13: "Small_bowel",
-        14: "Duodenum",
-        15: "Colon",
-        16: "Brain",
-        17: "Skeleton",
-        18: "Subcutaneous_fat",
-        19: "Visceral fat",
-        20: "Muscles",
-        21: "Bladder",
-        22: "Filler"
+        13: "Digestive",
+        14: "Brain",
+        15: "Skeleton",
+        16: "Muscles",
+        17: "Bladder",
+        18: "Filler"
     },
     # More index-to-name dictionaries for other models...
 }
 """
 
 This module contains the constants that are used in the moosez.
```

### Comparing `moosez-2.4.7/moosez/display.py` & `moosez-2.4.8/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/download.py` & `moosez-2.4.8/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/file_utilities.py` & `moosez-2.4.8/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/image_conversion.py` & `moosez-2.4.8/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/image_processing.py` & `moosez-2.4.8/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/input_validation.py` & `moosez-2.4.8/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/moosez.py` & `moosez-2.4.8/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.4.8/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.4.8/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/predict.py` & `moosez-2.4.8/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez/resources.py` & `moosez-2.4.8/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/moosez.egg-info/PKG-INFO` & `moosez-2.4.8/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.7
+Version: 2.4.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.7/moosez.egg-info/SOURCES.txt` & `moosez-2.4.8/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.7/setup.py` & `moosez-2.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.7',
+    version='2.4.8',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.10',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

