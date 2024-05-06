# Comparing `tmp/fastembed_haystack-0.1.0.tar.gz` & `tmp/fastembed_haystack-1.0.0.tar.gz`

## Comparing `fastembed_haystack-0.1.0.tar` & `fastembed_haystack-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/examples/example.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/examples/sparse_example.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/pydoc/config.yml
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/__init__.py
--rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_backend.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_document_embedder.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_sparse_document_embedder.py
--rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_sparse_text_embedder.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/tests/test_fastembed_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/README.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 fastembed_haystack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/examples/example.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/examples/sparse_example.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/pydoc/config.yml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/__init__.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_backend.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_document_embedder.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/README.md
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/PKG-INFO
```

### Comparing `fastembed_haystack-0.1.0/examples/example.py` & `fastembed_haystack-1.0.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/examples/sparse_example.py` & `fastembed_haystack-1.0.0/examples/sparse_example.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/pydoc/config.yml` & `fastembed_haystack-1.0.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/__init__.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/__init__.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,39 @@
     )
 
     doc_embedder.warm_up()
 
     # Text taken from PubMed QA Dataset (https://huggingface.co/datasets/pubmed_qa)
     document_list = [
         Document(
-            content="Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint destruction. Radical species with oxidative activity, including reactive nitrogen species, represent mediators of inflammation and cartilage damage.",
+            content=("Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint "
+                     "destruction. Radical species with oxidative activity, including reactive nitrogen species, "
+                     "represent mediators of inflammation and cartilage damage."),
             meta={
                 "pubid": "25,445,628",
                 "long_answer": "yes",
             },
         ),
         Document(
-            content="Plasma levels of pancreatic polypeptide (PP) rise upon food intake. Although other pancreatic islet hormones, such as insulin and glucagon, have been extensively investigated, PP secretion and actions are still poorly understood.",
+            content=("Plasma levels of pancreatic polypeptide (PP) rise upon food intake. Although other pancreatic "
+                     "islet hormones, such as insulin and glucagon, have been extensively investigated, PP secretion "
+                     "and actions are still poorly understood."),
             meta={
                 "pubid": "25,445,712",
                 "long_answer": "yes",
             },
         ),
     ]
 
     result = doc_embedder.run(document_list)
     print(f"Document Text: {result['documents'][0].content}")
     print(f"Document Embedding: {result['documents'][0].embedding}")
     print(f"Embedding Dimension: {len(result['documents'][0].embedding)}")
     ```
-    """  # noqa: E501
+    """
 
     def __init__(
         self,
         model: str = "BAAI/bge-small-en-v1.5",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         prefix: str = "",
```

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,51 +8,52 @@
 @component
 class FastembedSparseDocumentEmbedder:
     """
     FastembedSparseDocumentEmbedder computes Document embeddings using Fastembed sparse models.
 
     Usage example:
     ```python
-    # To use this component, install the "fastembed-haystack" package.
-    # pip install fastembed-haystack
-
     from haystack_integrations.components.embedders.fastembed import FastembedSparseDocumentEmbedder
     from haystack.dataclasses import Document
 
-    doc_embedder = FastembedSparseDocumentEmbedder(
+    sparse_doc_embedder = FastembedSparseDocumentEmbedder(
         model="prithvida/Splade_PP_en_v1",
         batch_size=32,
     )
 
-    doc_embedder.warm_up()
+    sparse_doc_embedder.warm_up()
 
     # Text taken from PubMed QA Dataset (https://huggingface.co/datasets/pubmed_qa)
     document_list = [
         Document(
-            content="Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint destruction. Radical species with oxidative activity, including reactive nitrogen species, represent mediators of inflammation and cartilage damage.",
+            content=("Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint "
+                     "destruction. Radical species with oxidative activity, including reactive nitrogen species, "
+                     "represent mediators of inflammation and cartilage damage."),
             meta={
                 "pubid": "25,445,628",
                 "long_answer": "yes",
             },
         ),
         Document(
-            content="Plasma levels of pancreatic polypeptide (PP) rise upon food intake. Although other pancreatic islet hormones, such as insulin and glucagon, have been extensively investigated, PP secretion and actions are still poorly understood.",
+            content=("Plasma levels of pancreatic polypeptide (PP) rise upon food intake. Although other pancreatic "
+                     "islet hormones, such as insulin and glucagon, have been extensively investigated, PP secretion "
+                     "and actions are still poorly understood."),
             meta={
                 "pubid": "25,445,712",
                 "long_answer": "yes",
             },
         ),
     ]
 
-    result = doc_embedder.run(document_list)
+    result = sparse_doc_embedder.run(document_list)
     print(f"Document Text: {result['documents'][0].content}")
-    print(f"Document Embedding: {result['documents'][0].sparse_embedding}")
-    print(f"Embedding Dimension: {len(result['documents'][0].sparse_embedding)}")
+    print(f"Document Sparse Embedding: {result['documents'][0].sparse_embedding}")
+    print(f"Sparse Embedding Dimension: {len(result['documents'][0].sparse_embedding)}")
     ```
-    """  # noqa: E501
+    """
 
     def __init__(
         self,
         model: str = "prithvida/Splade_PP_en_v1",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         batch_size: int = 32,
```

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,59 +9,54 @@
 @component
 class FastembedSparseTextEmbedder:
     """
     FastembedSparseTextEmbedder computes string embedding using fastembed sparse models.
 
     Usage example:
     ```python
-    # To use this component, install the "fastembed-haystack" package.
-    # pip install fastembed-haystack
-
     from haystack_integrations.components.embedders.fastembed import FastembedSparseTextEmbedder
 
-    text = "It clearly says online this will work on a Mac OS system. The disk comes and it does not, only Windows. Do Not order this if you have a Mac!!"
+    text = ("It clearly says online this will work on a Mac OS system. "
+            "The disk comes and it does not, only Windows. Do Not order this if you have a Mac!!")
 
-    text_embedder = FastembedSparseTextEmbedder(
+    sparse_text_embedder = FastembedSparseTextEmbedder(
         model="prithvida/Splade_PP_en_v1"
     )
-    text_embedder.warm_up()
+    sparse_text_embedder.warm_up()
 
-    embedding = text_embedder.run(text)["embedding"]
+    sparse_embedding = sparse_text_embedder.run(text)["sparse_embedding"]
     ```
-    """  # noqa: E501
+    """
 
     def __init__(
         self,
         model: str = "prithvida/Splade_PP_en_v1",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
-        batch_size: int = 32,
         progress_bar: bool = True,
         parallel: Optional[int] = None,
     ):
         """
         Create a FastembedSparseTextEmbedder component.
 
         :param model: Local path or name of the model in Fastembed's model hub, such as `prithvida/Splade_PP_en_v1`
         :param cache_dir: The path to the cache directory.
                 Can be set using the `FASTEMBED_CACHE_PATH` env variable.
                 Defaults to `fastembed_cache` in the system's temp directory.
         :param threads: The number of threads single onnxruntime session can use. Defaults to None.
-        :param batch_size: Number of strings to encode at once.
         :param progress_bar: If true, displays progress bar during embedding.
         :param parallel:
                 If > 1, data-parallel encoding will be used, recommended for offline encoding of large datasets.
                 If 0, use all available cores.
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
         """
 
         self.model_name = model
         self.cache_dir = cache_dir
         self.threads = threads
-        self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.parallel = parallel
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
@@ -69,15 +64,14 @@
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             model=self.model_name,
             cache_dir=self.cache_dir,
             threads=self.threads,
-            batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             parallel=self.parallel,
         )
 
     def warm_up(self):
         """
         Initializes the component.
@@ -106,12 +100,11 @@
             raise TypeError(msg)
         if not hasattr(self, "embedding_backend"):
             msg = "The embedding model has not been loaded. Please call warm_up() before running."
             raise RuntimeError(msg)
 
         embedding = self.embedding_backend.embed(
             [text],
-            batch_size=self.batch_size,
             show_progress_bar=self.progress_bar,
             parallel=self.parallel,
         )[0]
         return {"sparse_embedding": embedding}
```

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 @component
 class FastembedTextEmbedder:
     """
     FastembedTextEmbedder computes string embedding using fastembed embedding models.
 
     Usage example:
     ```python
-    # To use this component, install the "fastembed-haystack" package.
-    # pip install fastembed-haystack
-
     from haystack_integrations.components.embedders.fastembed import FastembedTextEmbedder
 
-    text = "It clearly says online this will work on a Mac OS system. The disk comes and it does not, only Windows. Do Not order this if you have a Mac!!"
+    text = ("It clearly says online this will work on a Mac OS system. "
+            "The disk comes and it does not, only Windows. Do Not order this if you have a Mac!!")
 
     text_embedder = FastembedTextEmbedder(
         model="BAAI/bge-small-en-v1.5"
     )
     text_embedder.warm_up()
 
     embedding = text_embedder.run(text)["embedding"]
     ```
-    """  # noqa: E501
+    """
 
     def __init__(
         self,
         model: str = "BAAI/bge-small-en-v1.5",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         prefix: str = "",
```

### Comparing `fastembed_haystack-0.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py` & `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/tests/test_fastembed_backend.py` & `fastembed_haystack-1.0.0/tests/test_fastembed_backend.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/tests/test_fastembed_document_embedder.py` & `fastembed_haystack-1.0.0/tests/test_fastembed_document_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/tests/test_fastembed_sparse_document_embedder.py` & `fastembed_haystack-1.0.0/tests/test_fastembed_sparse_document_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/tests/test_fastembed_sparse_text_embedder.py` & `fastembed_haystack-1.0.0/tests/test_fastembed_sparse_text_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,34 +14,31 @@
         """
         Test default initialization parameters for FastembedSparseTextEmbedder.
         """
         embedder = FastembedSparseTextEmbedder(model="prithvida/Splade_PP_en_v1")
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir is None
         assert embedder.threads is None
-        assert embedder.batch_size == 32
         assert embedder.progress_bar is True
         assert embedder.parallel is None
 
     def test_init_with_parameters(self):
         """
         Test custom initialization parameters for FastembedSparseTextEmbedder.
         """
         embedder = FastembedSparseTextEmbedder(
             model="prithvida/Splade_PP_en_v1",
             cache_dir="fake_dir",
             threads=2,
-            batch_size=64,
             progress_bar=False,
             parallel=1,
         )
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
-        assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
 
     def test_to_dict(self):
         """
         Test serialization of FastembedSparseTextEmbedder to a dictionary, using default initialization parameters.
         """
@@ -49,40 +46,37 @@
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": None,
                 "threads": None,
-                "batch_size": 32,
                 "progress_bar": True,
                 "parallel": None,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
         Test serialization of FastembedSparseTextEmbedder to a dictionary, using custom initialization parameters.
         """
         embedder = FastembedSparseTextEmbedder(
             model="prithvida/Splade_PP_en_v1",
             cache_dir="fake_dir",
             threads=2,
-            batch_size=64,
             progress_bar=False,
             parallel=1,
         )
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": "fake_dir",
                 "threads": 2,
-                "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
             },
         }
 
     def test_from_dict(self):
         """
@@ -90,47 +84,43 @@
         """
         embedder_dict = {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": None,
                 "threads": None,
-                "batch_size": 32,
                 "progress_bar": True,
                 "parallel": None,
             },
         }
         embedder = default_from_dict(FastembedSparseTextEmbedder, embedder_dict)
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir is None
         assert embedder.threads is None
-        assert embedder.batch_size == 32
         assert embedder.progress_bar is True
         assert embedder.parallel is None
 
     def test_from_dict_with_custom_init_parameters(self):
         """
         Test deserialization of FastembedSparseTextEmbedder from a dictionary, using custom initialization parameters.
         """
         embedder_dict = {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": "fake_dir",
                 "threads": 2,
-                "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
             },
         }
         embedder = default_from_dict(FastembedSparseTextEmbedder, embedder_dict)
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
-        assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder._FastembedSparseEmbeddingBackendFactory"
     )
     def test_warmup(self, mocked_factory):
```

### Comparing `fastembed_haystack-0.1.0/tests/test_fastembed_text_embedder.py` & `fastembed_haystack-1.0.0/tests/test_fastembed_text_embedder.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/.gitignore` & `fastembed_haystack-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/LICENSE.txt` & `fastembed_haystack-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/README.md` & `fastembed_haystack-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-0.1.0/pyproject.toml` & `fastembed_haystack-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset GmbH", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

### Comparing `fastembed_haystack-0.1.0/PKG-INFO` & `fastembed_haystack-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: fastembed-haystack
-Version: 0.1.0
+Version: 1.0.0
 Summary: Haystack 2.x component to embed strings and Documents using fastembed embedding model
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/fastembed/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

