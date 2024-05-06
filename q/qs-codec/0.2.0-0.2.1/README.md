# Comparing `tmp/qs_codec-0.2.0.tar.gz` & `tmp/qs_codec-0.2.1.tar.gz`

## Comparing `qs_codec-0.2.0.tar` & `qs_codec-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 qs_codec-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.2.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.2.0/requirements_dev.txt
--rw-r--r--   0        0        0    28785 2020-02-02 00:00:00.000000 qs_codec-0.2.0/docs/README.rst
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 qs_codec-0.2.0/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/__init__.py
--rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/compare_outputs.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/package.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/qs.js
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/qs.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/comparison/test_cases.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/e2e/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/decode_test.py
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/encode_test.py
--rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/example_test.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/fixed_qs_issues_test.py
--rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.2.0/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.2.0/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.2.0/LICENSE
--rw-r--r--   0        0        0    36399 2020-02-02 00:00:00.000000 qs_codec-0.2.0/README.rst
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 qs_codec-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    38005 2020-02-02 00:00:00.000000 qs_codec-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qs_codec-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.2.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.2.1/requirements_dev.txt
+-rw-r--r--   0        0        0    28785 2020-02-02 00:00:00.000000 qs_codec-0.2.1/docs/README.rst
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/__init__.py
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/compare_outputs.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/package.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/qs.js
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/qs.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/test_cases.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/example_test.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/fixed_qs_issues_test.py
+-rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.2.1/LICENSE
+-rw-r--r--   0        0        0    36399 2020-02-02 00:00:00.000000 qs_codec-0.2.1/README.rst
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 qs_codec-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    38005 2020-02-02 00:00:00.000000 qs_codec-0.2.1/PKG-INFO
```

### Comparing `qs_codec-0.2.0/CHANGELOG.md` & `qs_codec-0.2.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.2.1
+
+* [CHORE] update dependencies
+
 ## 0.2.0
 
 * [CHORE] update dependencies
 * [CHORE] update README
 
 ## 0.1.6
```

### Comparing `qs_codec-0.2.0/CODE-OF-CONDUCT.md` & `qs_codec-0.2.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/docs/README.rst` & `qs_codec-0.2.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/decode.py` & `qs_codec-0.2.1/src/qs_codec/decode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/encode.py` & `qs_codec-0.2.1/src/qs_codec/encode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/enums/format.py` & `qs_codec-0.2.1/src/qs_codec/enums/format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/enums/list_format.py` & `qs_codec-0.2.1/src/qs_codec/enums/list_format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/enums/sentinel.py` & `qs_codec-0.2.1/src/qs_codec/enums/sentinel.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/models/decode_options.py` & `qs_codec-0.2.1/src/qs_codec/models/decode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/models/encode_options.py` & `qs_codec-0.2.1/src/qs_codec/models/encode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/models/weak_wrapper.py` & `qs_codec-0.2.1/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/utils/decode_utils.py` & `qs_codec-0.2.1/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/utils/encode_utils.py` & `qs_codec-0.2.1/src/qs_codec/utils/encode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/utils/str_utils.py` & `qs_codec-0.2.1/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/src/qs_codec/utils/utils.py` & `qs_codec-0.2.1/src/qs_codec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/comparison/qs.py` & `qs_codec-0.2.1/tests/comparison/qs.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/comparison/test_cases.json` & `qs_codec-0.2.1/tests/comparison/test_cases.json`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/e2e/e2e_test.py` & `qs_codec-0.2.1/tests/e2e/e2e_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/unit/decode_test.py` & `qs_codec-0.2.1/tests/unit/decode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/unit/encode_test.py` & `qs_codec-0.2.1/tests/unit/encode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/unit/example_test.py` & `qs_codec-0.2.1/tests/unit/example_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/unit/utils_test.py` & `qs_codec-0.2.1/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/tests/unit/weakref_test.py` & `qs_codec-0.2.1/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/.gitignore` & `qs_codec-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/LICENSE` & `qs_codec-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/README.rst` & `qs_codec-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.0/pyproject.toml` & `qs_codec-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "regex==2024.4.28",
-    "types-regex==2024.4.28.20240430",
+    "regex>=2024.4.28",
+    "types-regex>=2024.4.28.20240506",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://techouse.github.io/qs_codec/"
 Documentation = "https://techouse.github.io/qs_codec/"
 Source = "https://github.com/techouse/qs_codec"
```

### Comparing `qs_codec-0.2.0/PKG-INFO` & `qs_codec-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qs-codec
-Version: 0.2.0
+Version: 0.2.1
 Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
 Project-URL: Homepage, https://techouse.github.io/qs_codec/
 Project-URL: Documentation, https://techouse.github.io/qs_codec/
 Project-URL: Source, https://github.com/techouse/qs_codec
 Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
@@ -25,16 +25,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
-Requires-Dist: regex==2024.4.28
-Requires-Dist: types-regex==2024.4.28.20240430
+Requires-Dist: regex>=2024.4.28
+Requires-Dist: types-regex>=2024.4.28.20240506
 Description-Content-Type: text/x-rst
 
 qs-codec
 ========
 
 A query string encoding and decoding library for Python.
```

