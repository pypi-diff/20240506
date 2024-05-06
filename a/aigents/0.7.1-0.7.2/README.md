# Comparing `tmp/aigents-0.7.1.tar.gz` & `tmp/aigents-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.1.tar", max compression
+gzip compressed data, was "aigents-0.7.2.tar", max compression
```

## Comparing `aigents-0.7.1.tar` & `aigents-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.1/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.1/README.md
--rw-r--r--   0        0        0     1028 2024-05-06 13:17:40.463660 aigents-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.1/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.1/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/base.py
--rw-r--r--   0        0        0    12988 2024-05-06 12:48:38.007967 aigents-0.7.1/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.1/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    15091 2024-05-06 12:57:38.654315 aigents-0.7.1/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.1/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.1/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.1/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.1/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.1/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/utils.py
--rw-r--r--   0        0        0     8675 1970-01-01 00:00:00.000000 aigents-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.2/README.md
+-rw-r--r--   0        0        0     1028 2024-05-06 17:26:15.624797 aigents-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.2/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.2/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.2/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.2/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13007 2024-05-06 17:26:15.624797 aigents-0.7.2/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.2/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    15091 2024-05-06 12:57:38.654315 aigents-0.7.2/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.2/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.2/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.2/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.2/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.2/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.2/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.2/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.2/src/aigents/utils.py
+-rw-r--r--   0        0        0     8675 1970-01-01 00:00:00.000000 aigents-0.7.2/PKG-INFO
```

### Comparing `aigents-0.7.1/LICENSE` & `aigents-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/README.md` & `aigents-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/pyproject.toml` & `aigents-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.1"
+version = "0.7.2"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.7.1/src/aigents/__init__.py` & `aigents-0.7.2/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/base.py` & `aigents-0.7.2/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/constants.py` & `aigents-0.7.2/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/context/base.py` & `aigents-0.7.2/src/aigents/context/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             data = json.loads(
                 self.embeddings.to_json(
                     orient='table',
                     index=False,
                     force_ascii=False
                 )
             )['data']
-            self.json = {column: [] for column in EMBEDDINGS_COLUMNS}
+            self.json = {column: [] for column in self.embeddings.columns}
             for row in data:
                 for key, value in row.items():
                     self.json[key].append(value)
             return self.json
         if DEBUG:
             logger.warning(
                 'Embeddings weren\'t generated yet. Returning {}.'
```

### Comparing `aigents-0.7.1/src/aigents/context/core.py` & `aigents-0.7.2/src/aigents/context/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,17 +168,17 @@
             max_tokens = self.max_tokens
         
         if isinstance(source, pd.DataFrame):
             self.embeddings = source
         elif isinstance(source, Path):
             self.embeddings = pd.read_parquet(source, engine='pyarrow')
         elif isinstance(source, dict):
-            if EMBEDDINGS_COLUMNS != tuple(source.keys()):
+            if not set(EMBEDDINGS_COLUMNS).issubset(set(source.keys())):
                 raise ContextError(
-                    f"Keys of `source` must be: {','.join(EMBEDDINGS_COLUMNS)}"
+                    f"Keys of `source` must contain: {','.join(EMBEDDINGS_COLUMNS)}"
                 )
             lengths = list(map(len, source.values()))
             if not all(x == lengths[0] for x in lengths[1:]):
                 raise ContextError(
                     "Items of `source`must have the same length"
                 )
             self.json = source
```

### Comparing `aigents-0.7.1/src/aigents/context/nlp/base.py` & `aigents-0.7.2/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/context/nlp/processors.py` & `aigents-0.7.2/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/context/nlp/utils.py` & `aigents-0.7.2/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/context/utils.py` & `aigents-0.7.2/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/core.py` & `aigents-0.7.2/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/errors.py` & `aigents-0.7.2/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/prompts.py` & `aigents-0.7.2/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/settings.py` & `aigents-0.7.2/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/src/aigents/utils.py` & `aigents-0.7.2/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.1/PKG-INFO` & `aigents-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.7.1
+Version: 0.7.2
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

