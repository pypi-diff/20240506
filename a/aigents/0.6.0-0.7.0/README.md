# Comparing `tmp/aigents-0.6.0.tar.gz` & `tmp/aigents-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.6.0.tar", max compression
+gzip compressed data, was "aigents-0.7.0.tar", max compression
```

## Comparing `aigents-0.6.0.tar` & `aigents-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.6.0/LICENSE
--rw-r--r--   0        0        0     4545 2024-03-20 10:12:52.420736 aigents-0.6.0/README.md
--rw-r--r--   0        0        0     1028 2024-05-03 19:31:33.640604 aigents-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      525 2024-03-13 18:32:05.073594 aigents-0.6.0/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.6.0/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/constants.py
--rw-r--r--   0        0        0      309 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/base.py
--rw-r--r--   0        0        0    11688 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-03 19:35:36.280050 aigents-0.6.0/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    14367 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     2502 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.6.0/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.6.0/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.6.0/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.6.0/src/aigents/prompts.py
--rw-r--r--   0        0        0     2350 2024-02-25 18:23:33.244701 aigents-0.6.0/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.6.0/src/aigents/utils.py
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 aigents-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4545 2024-03-20 10:12:52.420736 aigents-0.7.0/README.md
+-rw-r--r--   0        0        0     1028 2024-05-06 12:34:31.880450 aigents-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      793 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.0/src/aigents/base.py
+-rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2018 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/base.py
+-rw-r--r--   0        0        0    12872 2024-05-06 12:34:31.880450 aigents-0.7.0/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.0/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    14618 2024-05-06 12:34:31.880450 aigents-0.7.0/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     1378 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     2502 2024-05-04 14:41:42.569117 aigents-0.7.0/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.0/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.0/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.0/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.0/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.0/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.0/src/aigents/utils.py
+-rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 aigents-0.7.0/PKG-INFO
```

### Comparing `aigents-0.6.0/LICENSE` & `aigents-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/README.md` & `aigents-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/pyproject.toml` & `aigents-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.6.0"
+version = "0.7.0"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.6.0/src/aigents/base.py` & `aigents-0.7.0/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/constants.py` & `aigents-0.7.0/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/context/base.py` & `aigents-0.7.0/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/context/core.py` & `aigents-0.7.0/src/aigents/context/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import logging
+import asyncio
 from pathlib import Path
 from typing import Coroutine
 
 import pandas as pd
 
 from openai import APIError
 from openai import AsyncOpenAI
@@ -74,14 +75,15 @@
             api_key=api_key,
             organization=organization,
             **kwargs
         )
         self.question_embedding = None
         self.pipeline: str = None
         self.embeddings_generator: str = None
+        self.embedding_model: str = None
 
     async def generate_embeddings(
             self,
             source: str | pd.DataFrame | Path | dict = None,
             model: str = MODELS[0],
             max_tokens: int = None,  # tokens per chunk
             embeddings_generator: str | Coroutine = None,
@@ -187,15 +189,17 @@
                 raise TypeError(
                     '`source` must either be a DataFrame, '
                     'Path object, a string or a dict'
                 )
             try:
                 if isinstance(embeddings_generator, str):
                     try:
-                        self.pipeline, self.embedding_model = embeddings_generator.rsplit(maxsplit=2, sep=',')
+                        (
+                            self.pipeline, self.embedding_model
+                        ) = embeddings_generator.rsplit(maxsplit=2, sep=',')
                     except ValueError as err:
                         if 'unpack' in str(err):
                             message = (
                                 "`embeddings_generator` must be a spacy "
                                 "pipeline and a model (either `openai`or "
                                 "`gemini`) separated by a comma"
                             )
@@ -216,34 +220,37 @@
                         model=model,
                         max_tokens=max_tokens,
                         **kwargs
                     )
                 else:
                     raise ContextError(
                         '`embeddings_generator` must be a coroutine or a str '
-                        'corresponding to a spacy pipeline model.'
+                        'corresponding to a spacy pipeline model (either `openai`or '
+                        '`gemini`) separated by a comma'
                     )
             except APIError as err:
                 message = (
                     f"OpenAI's error: {err.message} "
                     f"(code {err.code}) "
                     "Try again in a few minutes."
                 )
                 raise APIContextError(message) from err
         self.json = self.to_json()
         return self.embeddings
 
     async def generate_context(self,
                                question: str,
+                               data: pd.DataFrame = None,
                                max_length: int = 1800,
                                pipeline: str = None,
                                embedding_model: str = None) -> str:
         results = []
         current_length = 0
-        data = self.embeddings
+        if data is None:
+            data = self.embeddings
         if pipeline is None:
             pipeline = self.pipeline
             if pipeline is None:
                 pipeline = 'en_core_web_md'
         if embedding_model is None:
             embedding_model = self.embedding_model
             if embedding_model is None:
@@ -266,15 +273,15 @@
             distance_metric='cosine'
         )
 
         for _, row in data.sort_values('distances', ascending=True).iterrows():
 
             results.append(row["chunks"].replace('\n', ' '))
 
-            current_length = number_of_tokens("\n-".join(results))
+            current_length = row["chunks"] + 3
 
             if current_length > max_length:
                 if len(results) > 1:
                     results.pop()
                 break
 
         context = f"* {results[0]}"
@@ -284,7 +291,34 @@
         length = number_of_tokens(context)
         if DEBUG:
             logger.debug(
                 'Context created. Length: %s', length
             )
         # Return the context
         return context
+
+
+async def embeddings_from_dict(source: dict,
+                               max_tokens: int = None,  # tokens per chunk
+                               embeddings_generator: str | Coroutine = None,) -> pd.DataFrame:
+    contexter = Context()
+    dataframe = None
+    tasks = []
+    for text in source.values():
+        tasks.append(
+            contexter.generate_embeddings(
+                source=text,
+                max_tokens=max_tokens,
+                embeddings_generator=embeddings_generator
+            )
+        )
+
+    results = await asyncio.gather(*tasks)
+    for reference, result in zip(source, results):
+        if dataframe is None:
+            dataframe = result
+            dataframe['reference'] = dataframe.shape[0]*[reference]
+            continue
+        result['reference'] = result.shape[0]*[reference]
+        dataframe = pd.concat([dataframe, result], ignore_index=True)
+    return dataframe
+
```

### Comparing `aigents-0.6.0/src/aigents/context/nlp/base.py` & `aigents-0.7.0/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/context/nlp/processors.py` & `aigents-0.7.0/src/aigents/context/nlp/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     MODELS,
     MODELS_EMBEDDING,
     EMBEDDINGS_COLUMNS,
 )
 from aigents.utils import get_encoding, run_async
 
 from .base import BaseTextProcessor
+from .utils import clean_text
 from .errors import ProcessingError
 
 
 logger = logging.getLogger('standard')
 
 
 class TextProcessor(BaseTextProcessor):
@@ -77,26 +78,27 @@
                             openai_organization=None,
                             **kwargs) -> pd.DataFrame:
             Asynchronously obtain embeddings for chunks using OpenAI API.
 
         """
         super().__init__(*args, pipeline=pipeline, **kwargs)
 
-    def split(self, text) -> List[str]:
+    def split(self, text, clean=True) -> List[str]:
         self.text = text
+        if clean:
+            self.text = clean_text(self.text)
         self.doc = self.nlp(self.text)
         self.sequences = [sent.text for sent in self.doc.sents]
         return self.sequences
 
     def to_chunks(self,
                   text: str = None,
                   model: str = MODELS[0],
                   max_tokens: int = 100) -> List[str]:
         if text is not None:
-            self.text = text
             self.split(text)
         # group sentences semantically with a maximum number of tokens
         # using tiktoken to compute tokens
         # example maximum number of tokens
         chunks = []
         tokens = []
         current_chunk = []
@@ -216,15 +218,15 @@
                 embedding = genai.embed_content(
                     model=MODELS_EMBEDDING[-2],
                     content=row[EMBEDDINGS_COLUMNS[0]],
                     task_type='SEMANTIC_SIMILARITY'
                 )
                 return embedding['embedding']
             raise ValueError(
-                "`async_embeddings` only supports `openai` or `gemini` models"
+                "`embeddings` only supports `openai` or `gemini` models"
             )
 
 
         for _, row in self.dataframe.iterrows():
             embeddings.append(create_embedding(row))
 
         self.dataframe[EMBEDDINGS_COLUMNS[2]] = embeddings
@@ -244,49 +246,53 @@
             self.to_dataframe(
                 data=data,
                 model=model,
                 max_tokens=max_tokens,
                 threshold=threshold
             )
 
+        if 'gemini' in embedding_model.lower():
+            GoogleChatter(api_key=api_key)
         tasks = []
-        
         async def create_embedding_openai(row):
             
             client = AsyncOpenAIChatter(
                 api_key=api_key,
                 organization=organization,
             ).client
             embedding = await client.embeddings.create(
                 input=row[EMBEDDINGS_COLUMNS[0]],
                 model=MODELS_EMBEDDING[0]
             )
             return embedding.data[0].embedding
         
         def create_embedding_gemini(row):
             # NOTE: GoogleChatter is called only for setting credentials 
-            GoogleChatter(api_key=api_key)
-            embedding = genai.embed_content(
-                model=MODELS_EMBEDDING[-2],
-                content=row[EMBEDDINGS_COLUMNS[0]],
-                task_type='SEMANTIC_SIMILARITY'
-            )
+            try:
+                embedding = genai.embed_content(
+                    model=MODELS_EMBEDDING[-2],
+                    content=row[EMBEDDINGS_COLUMNS[0]],
+                    task_type='SEMANTIC_SIMILARITY'
+                )
+            except ValueError as err:
+                logger.debug(row[EMBEDDINGS_COLUMNS[0]])
+                raise err
             return embedding['embedding']
 
-        async def create_embedding(row):
+        for _, row in self.dataframe.iterrows():
             if 'openai' in embedding_model.lower():
-                return await create_embedding_openai(row)
+                tasks.append(create_embedding_openai(row))
             if 'gemini' in embedding_model.lower():
-                return await asyncio.to_thread(create_embedding_gemini, row)
-            raise ValueError(
-                "`async_embeddings` only supports `openai` or `gemini` models"
-            )
-
-        for _, row in self.dataframe.iterrows():
-            tasks.append(create_embedding(row))
+                tasks.append(
+                    asyncio.create_task(
+                        asyncio.to_thread(create_embedding_gemini, row)
+                    )
+                )
+            # allow some of the tasks time to start
+            await asyncio.sleep(0.1)
         
         self.dataframe[EMBEDDINGS_COLUMNS[2]] = await asyncio.gather(*tasks)
 
         return self.dataframe
 
 
 def naive_split(
```

### Comparing `aigents-0.6.0/src/aigents/context/utils.py` & `aigents-0.7.0/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/core.py` & `aigents-0.7.0/src/aigents/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/errors.py` & `aigents-0.7.0/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/prompts.py` & `aigents-0.7.0/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/src/aigents/settings.py` & `aigents-0.7.0/src/aigents/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,52 +46,58 @@
 Authors: {author}
 {DELIMITER}
 """
 
 CONFIG_LOG = {
     "version": 1,
     "formatters": {
-        "client": {
-            "format": "%(levelname)s: %(message)s"
-        },
+        "client": {"format": "%(levelname)s: %(message)s"},
         "standard": {
             "format": (
-                "%(levelname)s - function: (%(name)s at "
-                "%(funcName)s line %(lineno)d): %(message)s"
+                "%(levelname)s (at %(pathname)s - %(funcName)s "
+                "in line %(lineno)d): %(message)s"
             )
+        },
+        "debug": {
+            "format": (
+                "%(asctime)s %(levelname)s (at %(funcName)s "
+                "in line %(lineno)d):"
+                "\n\t|──file: %(pathname)s"
+                "\n\t|──task name: %(taskName)s"
+                "\n\t└──message: %(message)s\n"
+            ),
+            "datefmt": "%y-%m-%d %H:%M:%S"
         }
     },
     "handlers": {
         "client": {
             "class": "logging.StreamHandler",
             "formatter": "client",
             "level": "INFO"
         },
         "standard": {
             "class": "logging.StreamHandler",
             "formatter": "standard",
             "level": "DEBUG"
+        },
+        "debug": {
+            "class": "logging.StreamHandler",
+            "formatter": "debug",
+            "level": "DEBUG"
         }
     },
-    "root": {
-        "handlers": [
-            "standard"
-        ],
-        "level": "DEBUG"
-    },
+    "root": {"handlers": ["standard"], "level": "DEBUG"},
     "loggers": {
         "client": {
-            "handlers": [
-                "client"
-            ],
+            "handlers": ["client"],
             "level": "DEBUG",
-            "propagate": False
+            "propagate": False,
+            "disable_existing_loggers": False
         },
         "standard": {
-            "handlers": [
-                "standard"
-            ],
+            "handlers": ["standard"],
             "level": "DEBUG",
-            "propagate": False
+            "propagate": False,
+            "disable_existing_loggers": False
         }
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aigents-0.6.0/src/aigents/utils.py` & `aigents-0.7.0/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.6.0/PKG-INFO` & `aigents-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.6.0
+Version: 0.7.0
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

