# Comparing `tmp/ssb_jordbruk_fagfunksjoner-0.1.1.tar.gz` & `tmp/ssb_jordbruk_fagfunksjoner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_jordbruk_fagfunksjoner-0.1.1.tar", max compression
+gzip compressed data, was "ssb_jordbruk_fagfunksjoner-0.2.0.tar", max compression
```

## Comparing `ssb_jordbruk_fagfunksjoner-0.1.1.tar` & `ssb_jordbruk_fagfunksjoner-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/LICENSE
--rw-r--r--   0        0        0     3215 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/README.md
--rw-r--r--   0        0        0     4167 2024-03-18 14:56:48.709983 ssb_jordbruk_fagfunksjoner-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/src/ssb_jordbruk_fagfunksjoner/__init__.py
--rw-r--r--   0        0        0      243 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/src/ssb_jordbruk_fagfunksjoner/__main__.py
--rw-r--r--   0        0        0    14362 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py
--rw-r--r--   0        0        0        0 2024-03-18 14:56:39.558067 ssb_jordbruk_fagfunksjoner-0.1.1/src/ssb_jordbruk_fagfunksjoner/py.typed
--rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ssb_jordbruk_fagfunksjoner-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3215 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/README.md
+-rw-r--r--   0        0        0     4169 2024-05-06 13:41:04.765917 ssb_jordbruk_fagfunksjoner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/src/ssb_jordbruk_fagfunksjoner/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/src/ssb_jordbruk_fagfunksjoner/__main__.py
+-rw-r--r--   0        0        0    14668 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:40:53.765826 ssb_jordbruk_fagfunksjoner-0.2.0/src/ssb_jordbruk_fagfunksjoner/py.typed
+-rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 ssb_jordbruk_fagfunksjoner-0.2.0/PKG-INFO
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.1.1/LICENSE` & `ssb_jordbruk_fagfunksjoner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_jordbruk_fagfunksjoner-0.1.1/README.md` & `ssb_jordbruk_fagfunksjoner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_jordbruk_fagfunksjoner-0.1.1/pyproject.toml` & `ssb_jordbruk_fagfunksjoner-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ssb-jordbruk-fagfunksjoner"
-version = "0.1.1"
+version = "0.2.0"
 description = "SSB Jordbruk Fagfunksjoner"
 authors = ["Magnus Theodor Engh <dor@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner"
 repository = "https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner"
 documentation = "https://statisticsnorway.github.io/ssb-jordbruk-fagfunksjoner"
 classifiers = ["Development Status :: 3 - Alpha"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner/releases"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 click = ">=8.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
@@ -62,15 +62,15 @@
 show_column_numbers = true
 show_error_context = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
-target-version = "py39"  # Minimum Python version supported
+target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 extend-exclude = [
     "__pycache__",
     "old",
     ".ipynb_checkpoints",
     "noxfile.py",
     "docs/conf.py",
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.1.1/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py` & `ssb_jordbruk_fagfunksjoner-0.2.0/src/ssb_jordbruk_fagfunksjoner/produksjonstilskudd.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,17 +121,17 @@
         "450": "Hester på utmarksbeite",
         "455": "Hester på beite",
         "480": "Lama på beite",
         "481": "Alpakka på beite",
         "486": "Hjort på beite",
         "487": "Sauer, født i fjor eller tidligere, beitetilskudd",
         "488": "Lam, født i år, beitetilskudd",
-        "521": "Høy",
-        "522": "Surfor",
-        "523": "Høyensilasje",
+        "521": "Salg av høy",
+        "522": "Salg av surfor",
+        "523": "Salg av høyensilasje",
         "720": "Storfe på utmarksbeite - Kyr av bevaringsverdig rase",
         "721": "Storfe på utmarksbeite - Okser av bevaringsverdig rase",
         "722": "Søyer av bevaringsverdig rase",
         "723": "Værer av bevaringsverdig rase",
         "724": "Ammegeiter av bevaringsverdig rase",
         "725": "Unghester under 3 år av bevaringsverdig rase",
         "801": "Økologiske melkekyr",
@@ -248,14 +248,22 @@
             "fjørfe_og_rugeegg",
             "pelsdyr",
             "andre_husdyr",
         ],
         "frukt_baer_groennsaker": ["frukt", "baer", "groennsaker"],
     }
 
+    statbank_groups: ClassVar[dict[str, list[str]]] = {
+        "storfe": ["119", "120", "121"],
+        "ku": ["120", "121"],
+        "sau": ["145", "146", "139"],
+        "avlssvin": ["155", "156", "158", "159"],
+        "svin": ["154", "155", "156", "157", "158", "159"],
+    }
+
     def __init__(self) -> None:
         """Initializes an instance of the Produksjonstilskudd class.
 
         This constructor method dynamically sets up class attributes based on predefined code groups and combinations. It organizes various agricultural product codes, including fruits, vegetables, and livestock, into easily accessible class attributes for further processing or querying.
         Upon instantiation, it calls the _setup_dynamic_attributes method to dynamically assign attributes to the instance based on the `code_groups` and `combinations` class variables. This setup allows for flexible manipulation and access to specific subsets of product codes.
         Attributes are set up to facilitate extraction of codes with the option to prefix them with 'PK_', indicating a primary key or unique identifier, which can be used for database operations or internal logic.
```

### Comparing `ssb_jordbruk_fagfunksjoner-0.1.1/PKG-INFO` & `ssb_jordbruk_fagfunksjoner-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ssb-jordbruk-fagfunksjoner
-Version: 0.1.1
+Version: 0.2.0
 Summary: SSB Jordbruk Fagfunksjoner
 Home-page: https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner
 License: MIT
 Author: Magnus Theodor Engh
 Author-email: dor@ssb.no
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/ssb-jordbruk-fagfunksjoner
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-jordbruk-fagfunksjoner
```

