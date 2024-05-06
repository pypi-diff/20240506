# Comparing `tmp/neuroharmonize-2.4.1.tar.gz` & `tmp/neuroharmonize-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroharmonize-2.4.1.tar", last modified: Tue Apr 23 17:22:40 2024, max compression
+gzip compressed data, was "neuroharmonize-2.4.2.tar", last modified: Mon May  6 20:12:17 2024, max compression
```

## Comparing `neuroharmonize-2.4.1.tar` & `neuroharmonize-2.4.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.947218 neuroharmonize-2.4.1/
--rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.1/LICENSE
--rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.1/MANIFEST.in
--rw-r--r--   0 pomponior   (501) staff       (20)    10843 2024-04-23 17:22:40.947105 neuroharmonize-2.4.1/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)    10285 2024-04-23 17:20:20.000000 neuroharmonize-2.4.1/README.md
--rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.1/pyproject.toml
--rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-04-23 17:22:40.947461 neuroharmonize-2.4.1/setup.cfg
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.945467 neuroharmonize-2.4.1/src/
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-04-23 17:22:40.946925 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/
--rw-r--r--   0 pomponior   (501) staff       (20)    10843 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)      222 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/SOURCES.txt
--rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/dependency_links.txt
--rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-04-23 17:22:40.000000 neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/top_level.txt
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.963958 neuroharmonize-2.4.2/
+-rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.2/LICENSE
+-rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.2/MANIFEST.in
+-rw-r--r--   0 pomponior   (501) staff       (20)    10859 2024-05-06 20:12:17.963859 neuroharmonize-2.4.2/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)    10301 2024-05-06 20:08:17.000000 neuroharmonize-2.4.2/README.md
+-rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.2/pyproject.toml
+-rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-05-06 20:12:17.964233 neuroharmonize-2.4.2/setup.cfg
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.961604 neuroharmonize-2.4.2/src/
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.962997 neuroharmonize-2.4.2/src/neuroHarmonize/
+-rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/__init__.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)     9135 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationApply.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)    18851 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationLearn.py
+-rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationNIFTI.py
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.963680 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/
+-rw-r--r--   0 pomponior   (501) staff       (20)    10859 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)      376 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/top_level.txt
```

### Comparing `neuroharmonize-2.4.1/LICENSE` & `neuroharmonize-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.1/PKG-INFO` & `neuroharmonize-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.1
+Version: 2.4.2
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,28 +39,32 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.1` (April 2024)
+Latest development version: `2.4.2` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
-    >>> pip install neuroHarmonize
+   ```
+   pip install neuroHarmonize
+   ```
 
 **Option 2: Install from GitHub (Development Version)**
 
-    >>> pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
+   pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
 
 Quick Start
 -----------
 
 *Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
 effects as well you can use the argument `return_s_data`.
```

### Comparing `neuroharmonize-2.4.1/README.md` & `neuroharmonize-2.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,32 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.1` (April 2024)
+Latest development version: `2.4.2` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
-    >>> pip install neuroHarmonize
+   ```
+   pip install neuroHarmonize
+   ```
 
 **Option 2: Install from GitHub (Development Version)**
 
-    >>> pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
+   pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
 
 Quick Start
 -----------
 
 *Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
 effects as well you can use the argument `return_s_data`.
```

### Comparing `neuroharmonize-2.4.1/setup.cfg` & `neuroharmonize-2.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuroHarmonize
-version = 2.4.1
+version = 2.4.2
 author = Raymond Pomponio
 author_email = raymond.pomponio@outlook.com
 description = Harmonization tools for multi-center neuroimaging studies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rpomponio/neuroHarmonize
 project_urls =
```

### Comparing `neuroharmonize-2.4.1/src/neuroHarmonize.egg-info/PKG-INFO` & `neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.1
+Version: 2.4.2
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,28 +39,32 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.1` (April 2024)
+Latest development version: `2.4.2` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
 
-    >>> pip install neuroHarmonize
+   ```
+   pip install neuroHarmonize
+   ```
 
 **Option 2: Install from GitHub (Development Version)**
 
-    >>> pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
+   pip install git+https://github.com/rpomponio/neuroHarmonize
+   ```
 
 Quick Start
 -----------
 
 *Please note:* the ComBat [^3] algorithm corrects for site effects but
 intentionally preserves covariate effects. If you wish to remove covariate
 effects as well you can use the argument `return_s_data`.
```

