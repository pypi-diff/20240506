# Comparing `tmp/picai_eval-1.4.5.tar.gz` & `tmp/picai_eval-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picai_eval-1.4.5.tar", last modified: Wed Aug 23 08:24:48 2023, max compression
+gzip compressed data, was "picai_eval-1.4.6.tar", last modified: Mon May  6 10:49:40 2024, max compression
```

## Comparing `picai_eval-1.4.5.tar` & `picai_eval-1.4.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.149087 picai_eval-1.4.5/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-07-02 18:08:14.000000 picai_eval-1.4.5/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)    26399 2023-08-23 08:24:48.149161 picai_eval-1.4.5/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)    25579 2023-03-26 14:28:54.000000 picai_eval-1.4.5/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      540 2022-07-02 18:08:14.000000 picai_eval-1.4.5/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      890 2023-08-23 08:24:48.149479 picai_eval-1.4.5/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)     2236 2023-05-16 09:55:16.000000 picai_eval-1.4.5/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.145397 picai_eval-1.4.5/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.147465 picai_eval-1.4.5/src/picai_eval/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1001 2022-07-02 18:08:14.000000 picai_eval-1.4.5/src/picai_eval/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     4160 2022-09-30 09:39:08.000000 picai_eval-1.4.5/src/picai_eval/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    13474 2022-10-10 15:59:36.000000 picai_eval-1.4.5/src/picai_eval/analysis_utils.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     3779 2022-07-02 18:08:14.000000 picai_eval-1.4.5/src/picai_eval/data_utils.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)    23214 2023-05-16 09:55:16.000000 picai_eval-1.4.5/src/picai_eval/eval.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3287 2022-07-02 18:08:14.000000 picai_eval-1.4.5/src/picai_eval/image_utils.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    16409 2023-06-10 09:16:01.000000 picai_eval-1.4.5/src/picai_eval/metrics.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)        0 2022-07-02 18:08:14.000000 picai_eval-1.4.5/src/picai_eval/py.typed
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.148509 picai_eval-1.4.5/src/picai_eval/stat_util/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     9072 2022-07-02 18:08:16.000000 picai_eval-1.4.5/src/picai_eval/stat_util/stat_util.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    23775 2023-05-16 09:55:16.000000 picai_eval-1.4.5/src/picai_eval/statistical_helper.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.148392 picai_eval-1.4.5/src/picai_eval.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    26399 2023-08-23 08:24:48.000000 picai_eval-1.4.5/src/picai_eval.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      688 2023-08-23 08:24:48.000000 picai_eval-1.4.5/src/picai_eval.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-08-23 08:24:48.000000 picai_eval-1.4.5/src/picai_eval.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2022-07-02 18:08:38.000000 picai_eval-1.4.5/src/picai_eval.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      161 2023-08-23 08:24:48.000000 picai_eval-1.4.5/src/picai_eval.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       11 2023-08-23 08:24:48.000000 picai_eval-1.4.5/src/picai_eval.egg-info/top_level.txt
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-08-23 08:24:48.148985 picai_eval-1.4.5/tests/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3843 2022-07-02 18:08:14.000000 picai_eval-1.4.5/tests/test_analysis_utils.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     2472 2022-11-10 13:10:31.000000 picai_eval-1.4.5/tests/test_case_evaluation.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     9909 2022-11-10 13:10:31.000000 picai_eval-1.4.5/tests/test_evaluation.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     6612 2023-01-23 13:54:49.000000 picai_eval-1.4.5/tests/test_statistical_helper.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.278511 picai_eval-1.4.6/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-07-02 18:08:14.000000 picai_eval-1.4.6/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    26831 2024-05-06 10:49:40.278388 picai_eval-1.4.6/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    25579 2023-03-26 14:28:54.000000 picai_eval-1.4.6/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      540 2022-07-02 18:08:14.000000 picai_eval-1.4.6/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      892 2024-05-06 10:49:40.278861 picai_eval-1.4.6/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     2236 2024-05-06 10:33:32.000000 picai_eval-1.4.6/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.272444 picai_eval-1.4.6/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.274922 picai_eval-1.4.6/src/picai_eval/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1001 2022-07-02 18:08:14.000000 picai_eval-1.4.6/src/picai_eval/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     4160 2022-09-30 09:39:08.000000 picai_eval-1.4.6/src/picai_eval/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    13474 2022-10-10 15:59:36.000000 picai_eval-1.4.6/src/picai_eval/analysis_utils.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     3779 2022-07-02 18:08:14.000000 picai_eval-1.4.6/src/picai_eval/data_utils.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)    23214 2023-05-16 09:55:16.000000 picai_eval-1.4.6/src/picai_eval/eval.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3392 2024-05-06 10:32:29.000000 picai_eval-1.4.6/src/picai_eval/image_utils.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    16409 2024-01-12 09:30:27.000000 picai_eval-1.4.6/src/picai_eval/metrics.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        0 2022-07-02 18:08:14.000000 picai_eval-1.4.6/src/picai_eval/py.typed
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.276334 picai_eval-1.4.6/src/picai_eval/stat_util/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     9072 2022-07-02 18:08:16.000000 picai_eval-1.4.6/src/picai_eval/stat_util/stat_util.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    23775 2023-05-16 09:55:16.000000 picai_eval-1.4.6/src/picai_eval/statistical_helper.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.277747 picai_eval-1.4.6/src/picai_eval.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    26831 2024-05-06 10:49:40.000000 picai_eval-1.4.6/src/picai_eval.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      688 2024-05-06 10:49:40.000000 picai_eval-1.4.6/src/picai_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-06 10:49:40.000000 picai_eval-1.4.6/src/picai_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2022-07-02 18:08:38.000000 picai_eval-1.4.6/src/picai_eval.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      161 2024-05-06 10:49:40.000000 picai_eval-1.4.6/src/picai_eval.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       11 2024-05-06 10:49:40.000000 picai_eval-1.4.6/src/picai_eval.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-06 10:49:40.277420 picai_eval-1.4.6/tests/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3843 2022-07-02 18:08:14.000000 picai_eval-1.4.6/tests/test_analysis_utils.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     2472 2022-11-10 13:10:31.000000 picai_eval-1.4.6/tests/test_case_evaluation.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     9909 2022-11-10 13:10:31.000000 picai_eval-1.4.6/tests/test_evaluation.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     6612 2023-01-23 13:54:49.000000 picai_eval-1.4.6/tests/test_statistical_helper.py
```

### Comparing `picai_eval-1.4.5/LICENSE` & `picai_eval-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/PKG-INFO` & `picai_eval-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
 Name: picai_eval
-Version: 1.4.5
+Version: 1.4.6
 Summary: PICAI Evaluation
 Home-page: https://github.com/DIAGNijmegen/picai_eval
 Author: Joeran Bosma, Anindo Saha and Matin Hosseinzadeh
 Author-email: Joeran.Bosma@radboudumc.nl
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_eval/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: SimpleITK
+Requires-Dist: scipy
+Requires-Dist: scikit-learn>=0.20.3
+Requires-Dist: mlxtend
+Requires-Dist: report_guided_annotation>=0.2.4
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
+Requires-Dist: tox>=3.24; extra == "testing"
 
 # Evaluation Utilities for 3D Detection and Diagnosis in Medical Imaging
 ![Tests](https://github.com/DIAGNijmegen/picai_eval/actions/workflows/tests.yml/badge.svg)
 
 This repository contains standardized functions to evaluate 3D detection and diagnosis performance in medical imaging —with its evaluation strategy being geared towards clinically significant prostate cancer (csPCa) detection in MRI. It is used for the official evaluation pipeline of the [PI-CAI challenge](https://pi-cai.grand-challenge.org/).
 
 ## Supported Evaluation Metrics
```

### Comparing `picai_eval-1.4.5/README.md` & `picai_eval-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/pyproject.toml` & `picai_eval-1.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/setup.cfg` & `picai_eval-1.4.6/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 author = Joeran Bosma, Anindo Saha and Matin Hosseinzadeh
 license = Apache 2.0
 license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
 	picai_eval
 install_requires = 
 	numpy
 	tqdm
```

### Comparing `picai_eval-1.4.5/setup.py` & `picai_eval-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version='1.4.5',  # also update version in metrics.py -> version
+        version='1.4.6',  # also update version in metrics.py -> version
         author_email='Joeran.Bosma@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/picai_eval',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/picai_eval/issues"
         },
```

### Comparing `picai_eval-1.4.5/src/picai_eval/__init__.py` & `picai_eval-1.4.6/src/picai_eval/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/__main__.py` & `picai_eval-1.4.6/src/picai_eval/__main__.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/analysis_utils.py` & `picai_eval-1.4.6/src/picai_eval/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/data_utils.py` & `picai_eval-1.4.6/src/picai_eval/data_utils.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/eval.py` & `picai_eval-1.4.6/src/picai_eval/eval.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/image_utils.py` & `picai_eval-1.4.6/src/picai_eval/image_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,18 @@
         assert isinstance(path, str), f"Unexpected path type: {type(path)}. Please provide a Path or str."
 
     if '.npy' in path:
         return np.load(path)
     elif '.nii' in path or '.mha' in path or 'mhd' in path:
         return sitk.GetArrayFromImage(sitk.ReadImage(path))
     elif '.npz' in path:
-        return np.load(path)['softmax'].astype('float32')[1]  # nnUnet format
+        # read the nnU-Net format
+        data = np.load(path)
+        data = data["softmax"] if "softmax" in data else data["probabilities"]
+        return data.astype("float32")[1]
     else:
         raise ValueError(f"Unexpected file path. Supported file formats: .nii(.gz), .mha, .npy and .npz. Got: {path}.")
 
 
 def read_prediction(path: PathLike) -> "npt.NDArray[np.float32]":
     """Read prediction, given a filepath"""
     # read prediction and ensure correct dtype
```

### Comparing `picai_eval-1.4.5/src/picai_eval/metrics.py` & `picai_eval-1.4.6/src/picai_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/stat_util/stat_util.py` & `picai_eval-1.4.6/src/picai_eval/stat_util/stat_util.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval/statistical_helper.py` & `picai_eval-1.4.6/src/picai_eval/statistical_helper.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/src/picai_eval.egg-info/PKG-INFO` & `picai_eval-1.4.6/src/picai_eval.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
-Name: picai-eval
-Version: 1.4.5
+Name: picai_eval
+Version: 1.4.6
 Summary: PICAI Evaluation
 Home-page: https://github.com/DIAGNijmegen/picai_eval
 Author: Joeran Bosma, Anindo Saha and Matin Hosseinzadeh
 Author-email: Joeran.Bosma@radboudumc.nl
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_eval/issues
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: SimpleITK
+Requires-Dist: scipy
+Requires-Dist: scikit-learn>=0.20.3
+Requires-Dist: mlxtend
+Requires-Dist: report_guided_annotation>=0.2.4
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
+Requires-Dist: tox>=3.24; extra == "testing"
 
 # Evaluation Utilities for 3D Detection and Diagnosis in Medical Imaging
 ![Tests](https://github.com/DIAGNijmegen/picai_eval/actions/workflows/tests.yml/badge.svg)
 
 This repository contains standardized functions to evaluate 3D detection and diagnosis performance in medical imaging —with its evaluation strategy being geared towards clinically significant prostate cancer (csPCa) detection in MRI. It is used for the official evaluation pipeline of the [PI-CAI challenge](https://pi-cai.grand-challenge.org/).
 
 ## Supported Evaluation Metrics
```

### Comparing `picai_eval-1.4.5/src/picai_eval.egg-info/SOURCES.txt` & `picai_eval-1.4.6/src/picai_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/tests/test_analysis_utils.py` & `picai_eval-1.4.6/tests/test_analysis_utils.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/tests/test_case_evaluation.py` & `picai_eval-1.4.6/tests/test_case_evaluation.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/tests/test_evaluation.py` & `picai_eval-1.4.6/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `picai_eval-1.4.5/tests/test_statistical_helper.py` & `picai_eval-1.4.6/tests/test_statistical_helper.py`

 * *Files identical despite different names*

