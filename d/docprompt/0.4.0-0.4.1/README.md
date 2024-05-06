# Comparing `tmp/docprompt-0.4.0.tar.gz` & `tmp/docprompt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.0.tar", max compression
+gzip compressed data, was "docprompt-0.4.1.tar", max compression
```

## Comparing `docprompt-0.4.0.tar` & `docprompt-0.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      585 2024-04-18 22:55:47.915108 docprompt-0.4.0/LICENSE
--rw-r--r--   0        0        0     4917 2024-04-18 22:55:47.915108 docprompt-0.4.0/README.md
--rw-r--r--   0        0        0      752 2024-04-30 02:41:36.793371 docprompt-0.4.0/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7095 2024-04-23 00:28:28.294162 docprompt-0.4.0/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8981 2024-04-23 00:27:13.953736 docprompt-0.4.0/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/schema/layout.py
--rw-r--r--   0        0        0     8157 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     4015 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4061 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-30 02:41:16.997263 docprompt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5225 2024-04-30 00:05:31.753210 docprompt-0.4.0/tests/test_document.py
--rw-r--r--   0        0        0      916 2024-04-23 01:59:30.430813 docprompt-0.4.0/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/util.py
--rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.1/README.md
+-rw-r--r--   0        0        0      752 2024-05-06 01:13:33.499643 docprompt-0.4.1/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.1/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.1/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.4.1/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.1/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.1/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.1/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7095 2024-04-23 00:30:13.055039 docprompt-0.4.1/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.1/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8916 2024-05-04 15:33:18.517588 docprompt-0.4.1/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.1/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     8585 2024-05-06 01:07:35.940590 docprompt-0.4.1/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.1/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.1/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.1/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.1/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.1/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.1/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.1/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.1/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.1/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.1/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.1/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.1/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.1/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.1/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.1/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.1/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.1/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.4.1/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4061 2024-05-04 01:28:27.264357 docprompt-0.4.1/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-05-06 01:13:20.571235 docprompt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.1/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.1/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.1/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.1/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.1/tests/test_document.py
+-rw-r--r--   0        0        0     1329 2024-05-06 01:10:26.569945 docprompt-0.4.1/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.1/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.1/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.1/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.1/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.4.1/PKG-INFO
```

### Comparing `docprompt-0.4.0/LICENSE` & `docprompt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/README.md` & `docprompt-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/__init__.py` & `docprompt-0.4.1/docprompt/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.0/docprompt/_exec/ghostscript.py` & `docprompt-0.4.1/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/provenance/search.py` & `docprompt-0.4.1/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/provenance/source.py` & `docprompt-0.4.1/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/provenance/util.py` & `docprompt-0.4.1/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/rasterize.py` & `docprompt-0.4.1/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/schema/document.py` & `docprompt-0.4.1/docprompt/schema/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,29 +206,27 @@
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
         resize_mode: ResizeModes = "thumbnail",
         max_file_size_bytes: Optional[int] = None,
         resize_aspect_ratios: Optional[Iterable[AspectRatioRule]] = None,
-        use_cache: bool = True,
         do_convert: bool = False,
         image_covert_mode: str = "L",
         do_quantize: bool = False,
         quantize_color_count: int = 8,
     ) -> str:
         """
         Rasterizes a page of the document using Pdfium and returns a data URI, which can
         be embedded into HTML or passed to large language models
         """
         image_bytes = self.rasterize_page(
             page_number,
             dpi=dpi,
             downscale_size=downscale_size,
-            use_cache=use_cache,
             do_convert=do_convert,
             image_covert_mode=image_covert_mode,
             do_quantize=do_quantize,
             quantize_color_count=quantize_color_count,
             resize_mode=resize_mode,
             max_file_size_bytes=max_file_size_bytes,
             resize_aspect_ratios=resize_aspect_ratios,
```

### Comparing `docprompt-0.4.0/docprompt/schema/layout.py` & `docprompt-0.4.1/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/schema/pipeline.py` & `docprompt-0.4.1/docprompt/schema/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,26 +159,38 @@
     )
 
     ocr_results: ResultContainer[OcrPageResult] = Field(
         default_factory=lambda: ResultContainer(),
         description="The OCR results for the page",
         repr=False,
     )
-    table_extraction_results: ResultContainer = Field(
-        default_factory=lambda: ResultContainer(),
-        description="The table extraction results for the page",
-        repr=False,
-    )
 
     _raster_cache: Dict[str, bytes] = PrivateAttr(default_factory=dict)
 
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state["__pydantic_private__"]["_raster_cache"] = {}
+
+        return state
+
     @property
     def rasterizer(self):
         return PageRasterizer(self._raster_cache, self)
 
+    def search(
+        self, query: str, refine_to_words: bool = True, require_exact_match: bool = True
+    ):
+        return self.document.locator.search(
+            query,
+            page_number=self.page_number,
+            refine_to_word=refine_to_words,
+            require_exact_match=require_exact_match,
+        )
+
 
 class DocumentNode(BaseModel, Generic[DocumentNodeMetadata, PageNodeMetadata]):
     """
     Represents a single document, with some metadata
     """
 
     document: Document
@@ -187,14 +199,21 @@
     )
     metadata: Optional[DocumentNodeMetadata] = Field(
         description="Application-specific metadata for the document", default=None
     )
 
     _locator: Optional["DocumentProvenanceLocator"] = PrivateAttr(default=None)
 
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state["__pydantic_private__"]["_locator"] = None
+
+        return state
+
     def __len__(self):
         return len(self.page_nodes)
 
     def __getitem__(self, index):
         return self.page_nodes[index]
 
     def __iter__(self):
```

### Comparing `docprompt-0.4.0/docprompt/tasks/base.py` & `docprompt-0.4.1/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/message.py` & `docprompt-0.4.1/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.1/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/ocr/result.py` & `docprompt-0.4.1/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.1/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.1/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.1/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/utils/date_extraction.py` & `docprompt-0.4.1/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/utils/masking/image.py` & `docprompt-0.4.1/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/utils/splitter.py` & `docprompt-0.4.1/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/docprompt/utils/util.py` & `docprompt-0.4.1/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/pyproject.toml` & `docprompt-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.4.0"
+version = "0.4.1"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.4.0/tests/fixtures/1.pdf` & `docprompt-0.4.1/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/fixtures/1_ocr.json` & `docprompt-0.4.1/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/test_date_extraction.py` & `docprompt-0.4.1/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/test_document.py` & `docprompt-0.4.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/test_documentnode.py` & `docprompt-0.4.1/tests/test_documentnode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pickle
 from docprompt import load_document, DocumentNode
 from .fixtures import PDF_FIXTURES
 
 from PIL import Image
 import base64
 
 
@@ -24,10 +25,30 @@
 
     assert not page_node.rasterizer.raster_cache
 
     image_uri = page_node.rasterizer.rasterize_to_data_uri("test")
 
     assert image_uri.startswith("data:image/png;base64,")
 
-    image_bytes = base64.b64decode(image_uri.split("data:image/png;base64,")[1].encode("utf-8"))
+    image_bytes = base64.b64decode(
+        image_uri.split("data:image/png;base64,")[1].encode("utf-8")
+    )
 
     assert image_bytes == page_node.rasterizer.rasterize("test", return_mode="bytes")
+
+
+def test__pickling_drops_cache():
+    document = load_document(PDF_FIXTURES[0].get_full_path())
+
+    document_node = DocumentNode.from_document(document)
+
+    page_node = document_node.page_nodes[0]
+
+    page_node.rasterizer.rasterize()
+
+    assert page_node._raster_cache
+
+    dumped = pickle.dumps(page_node)
+
+    loaded = pickle.loads(dumped)
+
+    assert not loaded._raster_cache
```

### Comparing `docprompt-0.4.0/tests/test_layout_models.py` & `docprompt-0.4.1/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/test_search.py` & `docprompt-0.4.1/tests/test_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .fixtures import PDF_FIXTURES
 
 from docprompt import DocumentNode, load_document
 from pytest import raises
+import pickle
 
 
 def test_search():
     document = load_document(PDF_FIXTURES[0].get_full_path())
     document_node = DocumentNode.from_document(document)
 
     ocr_results = PDF_FIXTURES[0].get_ocr_results()
@@ -41,7 +42,53 @@
     n_best = locator.search_n_best("and", n=3)
 
     assert len(n_best) == 3
 
     raw_search = locator.search_raw('content:"rooted"')
 
     assert len(raw_search) == 1
+
+
+def test_pickling__removes_locator_document_basis():
+    document = load_document(PDF_FIXTURES[0].get_full_path())
+    document_node = DocumentNode.from_document(document)
+
+    ocr_results = PDF_FIXTURES[0].get_ocr_results()
+
+    for page_num, ocr_results in ocr_results.items():
+        document_node.page_nodes[page_num - 1].ocr_results.results[
+            ocr_results.provider_name
+        ] = ocr_results
+
+    result_page_1 = document_node.locator.search("rooted", page_number=1)
+
+    assert len(result_page_1) == 1
+
+    dumped = pickle.dumps(document_node)
+
+    loaded = pickle.loads(dumped)
+
+    assert loaded._locator is None
+
+
+def test_pickling__removes_locator_page_basis():
+    document = load_document(PDF_FIXTURES[0].get_full_path())
+    document_node = DocumentNode.from_document(document)
+
+    ocr_results = PDF_FIXTURES[0].get_ocr_results()
+
+    for page_num, ocr_results in ocr_results.items():
+        document_node.page_nodes[page_num - 1].ocr_results.results[
+            ocr_results.provider_name
+        ] = ocr_results
+
+    page = document_node.page_nodes[0]
+
+    result_page_1 = page.search("rooted")
+
+    assert len(result_page_1) == 1
+
+    dumped = pickle.dumps(page)
+
+    loaded = pickle.loads(dumped)
+
+    assert loaded.document._locator is None
```

### Comparing `docprompt-0.4.0/tests/test_threadpool.py` & `docprompt-0.4.1/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/tests/util.py` & `docprompt-0.4.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.0/PKG-INFO` & `docprompt-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 Provides-Extra: search
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.4.0 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.4.1 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Provides-
-Extra: azure Provides-Extra: dev Provides-Extra: doc Provides-Extra: google
-Provides-Extra: search Provides-Extra: test Requires-Dist: azure-ai-
-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist: bump2version
-(>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8 (>=6.1.0,<7.0.0) ;
-extra == "test" Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra ==
-"test" Requires-Dist: fsspec (>=2022.11.0) Requires-Dist: google-cloud-
-documentai (>=2.20.0) ; extra == "google" Requires-Dist: isort
-(>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ;
-extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist:
-mkdocs-material-extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings
-(>=0.15.2,<0.16.0) ; extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ;
-extra == "test" Requires-Dist: networkx (>=2.8.8) ; extra == "search" Requires-
-Dist: numpy (>=1.20.3,<2.0.0) Requires-Dist: pillow (>=9.0.1) Requires-Dist:
-pip (>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-commit
-(>=2.12.0,<3.0.0) ; extra == "dev" Requires-Dist: pydantic (>=2.1.0) Requires-
-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-Dist: pytest (>=7.4.2,<8.0.0) ;
-extra == "test" Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "test"
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-magic
-(>=0.4.24) Requires-Dist: rapidfuzz (>=3.0.0) Requires-Dist: rtree
-(>=1.2.0,<2.0.0) ; extra == "search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ;
-extra == "test" Requires-Dist: tantivy (>=0.21.0,<0.22.0) ; extra == "search"
-Requires-Dist: tenacity (>=7.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ;
-extra == "dev" Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-
-Dist: tqdm (>=4.61.0) Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
-Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev" Description-
-Content-Type: text/markdown [![pypi](https://img.shields.io/pypi/v/
-docprompt.svg)](https://pypi.org/project/docprompt/) [![python](https://
-img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/
-docprompt/) [![Build Status](https://github.com/Page-Leaf/Docprompt/actions/
-workflows/dev.yml/badge.svg)](https://github.com/Page-Leaf/docprompt/actions/
-workflows/dev.yml) [![codecov](https://codecov.io/gh/Page-Leaf/Docprompt/
-branch/main/graphs/badge.svg)](https://codecov.io/github/Page-Leaf/Docprompt)
+Python :: 3.8 Provides-Extra: azure Provides-Extra: dev Provides-Extra: doc
+Provides-Extra: google Provides-Extra: search Provides-Extra: test Requires-
+Dist: azure-ai-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist:
+bump2version (>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8
+(>=6.1.0,<7.0.0) ; extra == "test" Requires-Dist: flake8-docstrings
+(>=1.7.0,<2.0.0) ; extra == "test" Requires-Dist: fsspec (>=2022.11.0)
+Requires-Dist: google-cloud-documentai (>=2.20.0) ; extra == "google" Requires-
+Dist: isort (>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs
+(>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-autorefs
+(>=0.2.1,<0.3.0) ; extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
+(>=1.0.0,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-material
+(>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-extensions
+(>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ; extra ==
+"doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ; extra == "test" Requires-Dist:
+networkx (>=2.8.8) ; extra == "search" Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pillow (>=9.0.1) Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra
+== "dev" Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev" Requires-
+Dist: pydantic (>=2.1.0) Requires-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-
+Dist: pytest (>=7.4.2,<8.0.0) ; extra == "test" Requires-Dist: pytest-cov
+(>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24) Requires-Dist:
+rapidfuzz (>=3.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0) ; extra == "search"
+Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test" Requires-Dist: tantivy
+(>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist: tenacity (>=7.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tox
+(>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm (>=4.61.0) Requires-
+Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
+(>=20.2.2,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown [!
+[pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/project/
+docprompt/) [![python](https://img.shields.io/pypi/pyversions/docprompt.svg)]
+(https://pypi.org/project/docprompt/) [![Build Status](https://github.com/Page-
+Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://github.com/Page-
+Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://codecov.io/gh/
+Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://codecov.io/github/
+Page-Leaf/Docprompt)
                                     _[_L_o_g_o_]
                               ******** DDooccpprroommpptt ********
                         Document AI, powered by LLM's
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                        Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # About Docprompt is a library for Document AI. It aims to make enterprise-
```

