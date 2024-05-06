# Comparing `tmp/aigents-0.7.0.tar.gz` & `tmp/aigents-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.0.tar", max compression
+gzip compressed data, was "aigents-0.7.1.tar", max compression
```

## Comparing `aigents-0.7.0.tar` & `aigents-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.0/LICENSE
--rw-r--r--   0        0        0     4545 2024-03-20 10:12:52.420736 aigents-0.7.0/README.md
--rw-r--r--   0        0        0     1028 2024-05-06 12:34:31.880450 aigents-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      793 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.0/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/base.py
--rw-r--r--   0        0        0    12872 2024-05-06 12:34:31.880450 aigents-0.7.0/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.0/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    14618 2024-05-06 12:34:31.880450 aigents-0.7.0/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.0/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.0/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.0/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.0/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.0/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/utils.py
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 aigents-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.1/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.1/README.md
+-rw-r--r--   0        0        0     1028 2024-05-06 13:17:40.463660 aigents-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.1/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.1/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/base.py
+-rw-r--r--   0        0        0    12988 2024-05-06 12:48:38.007967 aigents-0.7.1/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.1/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    15091 2024-05-06 12:57:38.654315 aigents-0.7.1/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.1/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.1/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.1/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.1/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.1/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.1/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.1/src/aigents/utils.py
+-rw-r--r--   0        0        0     8675 1970-01-01 00:00:00.000000 aigents-0.7.1/PKG-INFO
```

### Comparing `aigents-0.7.0/LICENSE` & `aigents-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/pyproject.toml` & `aigents-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.0"
+version = "0.7.1"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.7.0/src/aigents/__init__.py` & `aigents-0.7.1/src/aigents/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .core import OpenAIChatter
 from .core import AsyncOpenAIChatter
 from .core import GoogleChatter
 from .core import AsyncGoogleChatter
 from .core import AsyncGoogleVision
 from .core import BingChatter
 from .core import AsyncBingChatter
+from .context.core import Context
 from . import base
 from . import constants
 from . import prompts
 
 from .settings import CONFIG_LOG
 
 dictConfig(CONFIG_LOG)
@@ -24,11 +25,12 @@
     'OpenAIChatter',
     'AsyncOpenAIChatter',
     'GoogleChatter',
     'AsyncGoogleChatter',
     'AsyncGoogleVision',
     'BingChatter',
     'AsyncBingChatter',
+    'Context',
     'base',
     'constants',
-    'prompts'
+    'prompts',
 ]
```

### Comparing `aigents-0.7.0/src/aigents/base.py` & `aigents-0.7.1/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/constants.py` & `aigents-0.7.1/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/context/base.py` & `aigents-0.7.1/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/context/core.py` & `aigents-0.7.1/src/aigents/context/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from aigents.constants import (
     MODELS, EMBEDDINGS_COLUMNS, MODELS_EMBEDDING, MAX_TOKENS
 )
 from aigents.settings import DEBUG
 from aigents.utils import number_of_tokens
 
-from .nlp.processors import TextProcessor
+from .nlp.processors import naive_text_to_embeddings_async
 from .nlp.errors import ProcessingError
 from .base import BaseContext
 from .errors import ContextError
 from .errors import APIContextError
 from .utils import distances_from_embeddings, to_embeddings_async
 
 
@@ -82,15 +82,15 @@
         self.embedding_model: str = None
 
     async def generate_embeddings(
             self,
             source: str | pd.DataFrame | Path | dict = None,
             model: str = MODELS[0],
             max_tokens: int = None,  # tokens per chunk
-            embeddings_generator: str | Coroutine = None,
+            embeddings_generator: str | Coroutine = naive_text_to_embeddings_async,
             **kwargs
     ) -> pd.DataFrame:
         """Generate embeddings dataframe from source.
 
         Dataframe columns can be found at:
             context_files.constants.EMBEDDINGS_COLUMNS
         Which are
@@ -162,17 +162,17 @@
             If there is an issue with the OpenAI API, such as an error message
             or code returned during the generation process.
         """
         if source is None:
             source = self.text
         if max_tokens is None:
             max_tokens = self.max_tokens
+        
         if isinstance(source, pd.DataFrame):
             self.embeddings = source
-
         elif isinstance(source, Path):
             self.embeddings = pd.read_parquet(source, engine='pyarrow')
         elif isinstance(source, dict):
             if EMBEDDINGS_COLUMNS != tuple(source.keys()):
                 raise ContextError(
                     f"Keys of `source` must be: {','.join(EMBEDDINGS_COLUMNS)}"
                 )
@@ -202,14 +202,15 @@
                                 "`embeddings_generator` must be a spacy "
                                 "pipeline and a model (either `openai`or "
                                 "`gemini`) separated by a comma"
                             )
                             message = f"{message}: {err.message}"
                             raise ContextError(message) from err
                     try:
+                        logger.debug("HERE")
                         self.embeddings = await to_embeddings_async(
                             source,
                             self.pipeline.strip(),
                             max_tokens=max_tokens,
                             embedding_model=self.embedding_model.strip()
                         )
                     except ProcessingError as err:
@@ -273,15 +274,15 @@
             distance_metric='cosine'
         )
 
         for _, row in data.sort_values('distances', ascending=True).iterrows():
 
             results.append(row["chunks"].replace('\n', ' '))
 
-            current_length = row["chunks"] + 3
+            current_length = number_of_tokens("\n-".join(results))
 
             if current_length > max_length:
                 if len(results) > 1:
                     results.pop()
                 break
 
         context = f"* {results[0]}"
```

### Comparing `aigents-0.7.0/src/aigents/context/nlp/base.py` & `aigents-0.7.1/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/context/nlp/processors.py` & `aigents-0.7.1/src/aigents/context/nlp/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,22 +374,41 @@
     )
 
 def naive_text_to_embeddings(
         text: str,
         model: str = MODELS[0],
         max_tokens: int = 500,
         api_key=None,
-        organization=None
+        organization=None,
+        **kwargs
 ):
     processor = TextProcessor()
     processor.dataframe = naive_token_splitter(text, model, max_tokens)
     return processor.embeddings(
         model=model,
-        api_key=openai_key,
-        organization=openai_organization
+        api_key=api_key,
+        organization=organization,
+        **kwargs
+    )
+
+async def naive_text_to_embeddings_async(
+        text: str,
+        model: str = MODELS[0],
+        max_tokens: int = 500,
+        api_key=None,
+        organization=None,
+        **kwargs
+):
+    processor = TextProcessor()
+    processor.dataframe = naive_token_splitter(text, model, max_tokens)
+    return await processor.async_embeddings(
+        model=model,
+        api_key=api_key,
+        organization=organization,
+        **kwargs
     )
 
 
 def create_embeddings(text: str,
                       pipeline: str = "en_core_web_md") -> List[float]:
     """
     Create text embeddings for the given input text.
```

### Comparing `aigents-0.7.0/src/aigents/context/nlp/utils.py` & `aigents-0.7.1/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/context/utils.py` & `aigents-0.7.1/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/core.py` & `aigents-0.7.1/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/errors.py` & `aigents-0.7.1/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/prompts.py` & `aigents-0.7.1/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/settings.py` & `aigents-0.7.1/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.0/src/aigents/utils.py` & `aigents-0.7.1/src/aigents/utils.py`

 * *Files identical despite different names*

