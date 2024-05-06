# Comparing `tmp/cltrier_nlp-0.1.6.tar.gz` & `tmp/cltrier_nlp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltrier_nlp-0.1.6.tar", max compression
+gzip compressed data, was "cltrier_nlp-0.1.7.tar", max compression
```

## Comparing `cltrier_nlp-0.1.6.tar` & `cltrier_nlp-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0      612 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.6/README.md
--rw-r--r--   0        0        0      513 2024-05-02 13:39:38.069285 cltrier_nlp-0.1.6/cltrier_nlp/__init__.py
--rw-r--r--   0        0        0     4127 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.6/cltrier_nlp/corpus/__init__.py
--rw-r--r--   0        0        0     1976 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.6/cltrier_nlp/corpus/sentence.py
--rw-r--r--   0        0        0     4369 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.6/cltrier_nlp/encoder/__init__.py
--rw-r--r--   0        0        0      840 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.6/cltrier_nlp/encoder/batch.py
--rw-r--r--   0        0        0     2556 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/encoder/pooler.py
--rw-r--r--   0        0        0      988 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/functional/__init__.py
--rw-r--r--   0        0        0      932 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/functional/neural.py
--rw-r--r--   0        0        0     1715 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/functional/text.py
--rw-r--r--   0        0        0       78 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/utility/__init__.py
--rw-r--r--   0        0        0      683 2024-05-02 13:22:04.985564 cltrier_nlp-0.1.6/cltrier_nlp/utility/map.py
--rw-r--r--   0        0        0      211 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/cltrier_nlp/utility/types.py
--rw-r--r--   0        0        0     1353 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      612 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.7/README.md
+-rw-r--r--   0        0        0      513 2024-05-02 13:39:38.069285 cltrier_nlp-0.1.7/cltrier_nlp/__init__.py
+-rw-r--r--   0        0        0     4153 2024-05-06 11:40:37.778248 cltrier_nlp-0.1.7/cltrier_nlp/corpus/__init__.py
+-rw-r--r--   0        0        0     1976 2024-05-03 06:35:46.993484 cltrier_nlp-0.1.7/cltrier_nlp/corpus/sentence.py
+-rw-r--r--   0        0        0     4305 2024-05-06 11:31:18.380722 cltrier_nlp-0.1.7/cltrier_nlp/encoder/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-06 11:35:54.074704 cltrier_nlp-0.1.7/cltrier_nlp/encoder/batch.py
+-rw-r--r--   0        0        0     2562 2024-05-06 11:34:52.424214 cltrier_nlp-0.1.7/cltrier_nlp/encoder/pooler.py
+-rw-r--r--   0        0        0     1007 2024-05-03 06:40:37.513605 cltrier_nlp-0.1.7/cltrier_nlp/functional/__init__.py
+-rw-r--r--   0        0        0      932 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.7/cltrier_nlp/functional/neural.py
+-rw-r--r--   0        0        0     1715 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.7/cltrier_nlp/functional/text.py
+-rw-r--r--   0        0        0     5081 2024-05-06 11:29:42.268538 cltrier_nlp-0.1.7/cltrier_nlp/trainer/__init__.py
+-rw-r--r--   0        0        0     3098 2024-05-06 11:30:07.800679 cltrier_nlp-0.1.7/cltrier_nlp/trainer/metric.py
+-rw-r--r--   0        0        0     3011 2024-05-06 11:26:39.387081 cltrier_nlp-0.1.7/cltrier_nlp/trainer/progress.py
+-rw-r--r--   0        0        0       78 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.7/cltrier_nlp/utility/__init__.py
+-rw-r--r--   0        0        0      683 2024-05-02 13:22:04.985564 cltrier_nlp-0.1.7/cltrier_nlp/utility/map.py
+-rw-r--r--   0        0        0      211 2024-05-03 06:35:46.996817 cltrier_nlp-0.1.7/cltrier_nlp/utility/types.py
+-rw-r--r--   0        0        0     1398 2024-05-06 11:42:03.984251 cltrier_nlp-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.7/PKG-INFO
```

### Comparing `cltrier_nlp-0.1.6/README.md` & `cltrier_nlp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/__init__.py` & `cltrier_nlp-0.1.7/cltrier_nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/corpus/__init__.py` & `cltrier_nlp-0.1.7/cltrier_nlp/corpus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         Returns:
             Corpus
         """
         return Corpus(
             sentences=(
                 subset := [sent for sent in self.sentences if sent.language == language]
             ),
-            raw=" ".join([sent.raw for sent in subset]),
+            raw=" ".join([sent.raw for sent in subset]),  # type: ignore[has-type]
         )
 
     def generate_ngrams(self, n: int) -> utility.types.NGrams:
         """
 
         Args:
             n (int):
```

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/corpus/sentence.py` & `cltrier_nlp-0.1.7/cltrier_nlp/corpus/sentence.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/encoder/__init__.py` & `cltrier_nlp-0.1.7/cltrier_nlp/encoder/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,23 +63,20 @@
             unpad (bool, optional): Whether to remove padding from embeddings and tokens. Defaults to True.
 
         Returns:
             EncoderBatch: A EncodedBatch object. See documentation for more.
         """
         return EncoderBatch(
             **(encoding := self.tokenizer(batch, padding=True, **self.args.tokenizer)),
-            **{
-                "embeds": self.forward(
-                    torch.tensor(encoding["input_ids"], device=self.args.device).long(),
-                    torch.tensor(encoding["attention_mask"], device=self.args.device).short(),
-                ),
-                "token": [self.ids_to_tokens(ids) for ids in encoding["input_ids"]],
-                "unpad": unpad,
-            }
-
+            embeds=self.forward(
+                torch.tensor(encoding["input_ids"], device=self.args.device).long(),
+                torch.tensor(encoding["attention_mask"], device=self.args.device).short(),
+            ),
+            token=[self.ids_to_tokens(ids) for ids in encoding["input_ids"]],
+            unpad=unpad,
         )
 
     def forward(self, ids: torch.Tensor, masks: torch.Tensor) -> torch.Tensor:
         """
         Perform a forward pass through the model and return the aggregated hidden states.
 
         Args:
```

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/encoder/batch.py` & `cltrier_nlp-0.1.7/cltrier_nlp/encoder/batch.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .. import utility
 
 
 class EncoderBatch(pydantic.BaseModel):
     """
 
     """
-    embeds: utility.types.Batch[torch.Tensor]
+    embeds: typing.Union[torch.Tensor, utility.types.Batch[torch.Tensor]]
     token: utility.types.Batch[utility.types.Tokens]
 
     input_ids: utility.types.Batch[typing.List[int]]
     token_type_ids: utility.types.Batch[typing.List[int]]
 
     attention_mask: utility.types.Batch[typing.List[int]]
     offset_mapping: utility.types.Batch[typing.List[typing.Tuple[int, int]]]
```

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/encoder/pooler.py` & `cltrier_nlp-0.1.7/cltrier_nlp/encoder/pooler.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         if form not in ["sent_cls", "sent_mean"] and not extract_spans:
             raise ValueError("Please provide a list of span values to extract.")
 
         return [
             EncoderPoolerArgs().fns[form](embed)
             for embed in (
-                encodes.embeds
+                list(encodes.embeds)
                 if form in ["sent_cls", "sent_mean"]
                 else EncoderPooler._extract_embed_spans(encodes, extract_spans)
             )
         ]
 
     @staticmethod
     def _extract_embed_spans(encodes: EncoderBatch, extract_spans) -> typing.Generator:
```

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/functional/__init__.py` & `cltrier_nlp-0.1.7/cltrier_nlp/functional/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from . import text
 from . import neural
 
 __all__ = ["text", "neural"]
 
 
-def timeit(func: typing.Callable):
+def timeit(func: typing.Callable) -> typing.Callable:
     """
     Decorator function to measure the execution time of the function argument.
 
     Args:
         func (Callable): The function to be measured.
 
     Returns:
```

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/functional/neural.py` & `cltrier_nlp-0.1.7/cltrier_nlp/functional/neural.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/functional/text.py` & `cltrier_nlp-0.1.7/cltrier_nlp/functional/text.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/cltrier_nlp/utility/map.py` & `cltrier_nlp-0.1.7/cltrier_nlp/utility/map.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.6/pyproject.toml` & `cltrier_nlp-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cltrier_nlp"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Simon Münker <muenker@uni-trier.de>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/simon-muenker/cltrier_nlp"
 documentation = "https://simon-muenker.github.io/cltrier_nlp/"
 classifiers = [
@@ -16,20 +16,20 @@
     "Intended Audience :: Science/Research",
     "Topic :: Text Processing"
 ]
 packages = [{ include = "cltrier_nlp" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-nltk = "^3.8.1"
 pydantic = "^2.7.1"
-langdetect = "^1.0.9"
-langcodes = "^3.4.0"
+nltk = "^3.8.1"
 transformers = "^4.40.1"
 torch = "^2.2.2"
+langdetect = "^1.0.9"
+langcodes = "^3.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pre-commit = "^3.7.0"
 ruff = "^0.4.2"
 mypy = "^1.10.0"
 
@@ -38,15 +38,17 @@
 mkdocstrings = { version = "^0.25.0", extras = ["python"] }
 mkdocs-literate-nav = "^0.6.1"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-section-index = "^0.3.9"
 
 [tool.poetry.group.examples.dependencies]
 jupyter = "^1.0.0"
+datasets = "^2.19.1"
 pandas = "^2.2.2"
+scikit-learn = "^1.4.2"
 matplotlib = "^3.8.4"
 seaborn = "^0.13.2"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "DEBUG"
 testpaths = [
```

### Comparing `cltrier_nlp-0.1.6/PKG-INFO` & `cltrier_nlp-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltrier_nlp
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/simon-muenker/cltrier_nlp
 License: Apache-2.0
 Author: Simon Münker
 Author-email: muenker@uni-trier.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

