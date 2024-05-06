# Comparing `tmp/multiform_validator-0.0.7.tar.gz` & `tmp/multiform_validator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiform_validator-0.0.7.tar", last modified: Mon May  6 06:31:18 2024, max compression
+gzip compressed data, was "multiform_validator-0.0.8.tar", last modified: Mon May  6 21:17:38 2024, max compression
```

## Comparing `multiform_validator-0.0.7.tar` & `multiform_validator-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.915777 multiform_validator-0.0.7/
--rw-rw-rw-   0        0        0     1074 2024-03-15 22:10:05.000000 multiform_validator-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4027 2024-05-06 06:31:18.897799 multiform_validator-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3277 2024-05-06 06:21:19.000000 multiform_validator-0.0.7/README.md
--rw-rw-rw-   0        0        0      728 2024-05-06 06:19:31.000000 multiform_validator-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 06:31:18.916765 multiform_validator-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.600974 multiform_validator-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.866872 multiform_validator-0.0.7/src/multiform_validator/
--rw-rw-rw-   0        0        0      389 2023-10-18 00:54:32.000000 multiform_validator-0.0.7/src/multiform_validator/__init__.py
--rw-rw-rw-   0        0        0     2222 2024-03-27 06:37:56.000000 multiform_validator-0.0.7/src/multiform_validator/cnpjValidator.py
--rw-rw-rw-   0        0        0     2496 2024-04-19 06:28:03.000000 multiform_validator-0.0.7/src/multiform_validator/cpfValidator.py
--rw-rw-rw-   0        0        0     2700 2024-03-27 06:38:41.000000 multiform_validator-0.0.7/src/multiform_validator/getOnlyEmail.py
--rw-rw-rw-   0        0        0     1132 2024-03-27 06:38:57.000000 multiform_validator-0.0.7/src/multiform_validator/identifyFlagCard.py
--rw-rw-rw-   0        0        0      679 2024-03-27 06:39:14.000000 multiform_validator-0.0.7/src/multiform_validator/isCreditCardValid.py
--rw-rw-rw-   0        0        0     1258 2024-05-06 06:23:22.000000 multiform_validator-0.0.7/src/multiform_validator/isEmail.py
--rw-rw-rw-   0        0        0     1461 2024-03-27 06:39:26.000000 multiform_validator-0.0.7/src/multiform_validator/passwordStrengthTester.py
--rw-rw-rw-   0        0        0     1139 2024-03-27 06:39:38.000000 multiform_validator-0.0.7/src/multiform_validator/validateBRPhoneNumber.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.897799 multiform_validator-0.0.7/src/multiform_validator.egg-info/
--rw-rw-rw-   0        0        0     4027 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.260419 multiform_validator-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/src/multiform_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/cnpjValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/cpfValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/getOnlyEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/identifyFlagCard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/isCreditCardValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/isEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/passwordStrengthTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 21:17:27.000000 multiform_validator-0.0.8/src/multiform_validator/validateBRPhoneNumber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:38.264418 multiform_validator-0.0.8/src/multiform_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 21:17:38.000000 multiform_validator-0.0.8/src/multiform_validator.egg-info/top_level.txt
```

### Comparing `multiform_validator-0.0.7/LICENSE` & `multiform_validator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/pyproject.toml` & `multiform_validator-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiform-validator"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Gabriel Logan" },
 ]
 description = "Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `multiform_validator-0.0.7/src/multiform_validator/cnpjValidator.py` & `multiform_validator-0.0.8/src/multiform_validator/cnpjValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/cpfValidator.py` & `multiform_validator-0.0.8/src/multiform_validator/cpfValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/getOnlyEmail.py` & `multiform_validator-0.0.8/src/multiform_validator/getOnlyEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/identifyFlagCard.py` & `multiform_validator-0.0.8/src/multiform_validator/identifyFlagCard.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/isCreditCardValid.py` & `multiform_validator-0.0.8/src/multiform_validator/isCreditCardValid.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/isEmail.py` & `multiform_validator-0.0.8/src/multiform_validator/isEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/passwordStrengthTester.py` & `multiform_validator-0.0.8/src/multiform_validator/passwordStrengthTester.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator/validateBRPhoneNumber.py` & `multiform_validator-0.0.8/src/multiform_validator/validateBRPhoneNumber.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.0.7/src/multiform_validator.egg-info/SOURCES.txt` & `multiform_validator-0.0.8/src/multiform_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

