# Comparing `tmp/bpm_ai_inference-0.3.4.tar.gz` & `tmp/bpm_ai_inference-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.3.4.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.3.5.tar", max compression
```

## Comparing `bpm_ai_inference-0.3.4.tar` & `bpm_ai_inference-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35128 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/LICENSE
--rw-r--r--   0        0        0      743 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2852 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/classification/transformers_text_classifier.py
--rw-r--r--   0        0        0     1909 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/image_classification/__init__.py
--rw-r--r--   0        0        0     2547 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/image_classification/transformers_image_classifier.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/__init__.py
--rw-r--r--   0        0        0      221 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/_constants.py
--rw-r--r--   0        0        0     8197 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/llama_chat.py
--rw-r--r--   0        0        0      199 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
--rw-r--r--   0        0        0      981 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
--rw-r--r--   0        0        0     1725 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/util.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3256 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1833 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2154 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2056 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1940 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1402 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3178 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18731 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0       36 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      483 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/util/files.py
--rw-r--r--   0        0        0      122 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/util/hf.py
--rw-r--r--   0        0        0      828 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     7153 2024-05-03 21:32:22.158323 bpm_ai_inference-0.3.4/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0      973 2024-05-03 21:32:22.162323 bpm_ai_inference-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/LICENSE
+-rw-r--r--   0        0        0      743 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2852 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/classification/transformers_text_classifier.py
+-rw-r--r--   0        0        0     1910 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/image_classification/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/image_classification/transformers_image_classifier.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/_constants.py
+-rw-r--r--   0        0        0     8219 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/llama_chat.py
+-rw-r--r--   0        0        0      199 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
+-rw-r--r--   0        0        0      981 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
+-rw-r--r--   0        0        0     1725 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/util.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.332312 bpm_ai_inference-0.3.5/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3369 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1833 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2154 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2056 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1940 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1402 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3178 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18765 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0       36 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/util/files.py
+-rw-r--r--   0        0        0      122 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/util/hf.py
+-rw-r--r--   0        0        0      828 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     7255 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0      973 2024-05-06 10:27:02.336312 bpm_ai_inference-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.5/PKG-INFO
```

### Comparing `bpm_ai_inference-0.3.4/LICENSE` & `bpm_ai_inference-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/README.md` & `bpm_ai_inference-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/classification/transformers_text_classifier.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/classification/transformers_text_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 if __name__ == "__main__":
     logging.basicConfig(format='%(levelname)s: %(message)s', level=int(os.getenv('LOG_LEVEL', str(logging.INFO))))
 
     daemon = create_remote_object_daemon(
         host=os.getenv('DAEMON_HOST', '0.0.0.0'),
         port=int(os.getenv('DAEMON_PORT', 6666)),
         instance_strategy=os.getenv('INSTANCE_STRATEGY', 'memory_limit'),
-        max_memory=int(os.getenv('SOFT_MEMORY_LIMIT', 8_589_934_592))
+        max_memory=int(os.getenv('SOFT_MEMORY_LIMIT', 16_000_000_000))
     )
 
     for c in remote_classes:
         daemon.register_class(c)
 
     daemon.serve()
```

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/image_classification/transformers_image_classifier.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/image_classification/transformers_image_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/llama_chat.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/llama_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def __init__(
         self,
         model: str = DEFAULT_MODEL,
         filename: str = DEFAULT_QUANT_BALANCED,
         temperature: float = DEFAULT_TEMPERATURE,
         max_retries: int = DEFAULT_MAX_RETRIES,
-        force_offline: bool = os.getenv(FORCE_OFFLINE_FLAG, False)
+        force_offline: bool = (os.getenv(FORCE_OFFLINE_FLAG, "false").lower() == "true")
     ):
         if not has_llama_cpp_python:
             raise ImportError('llama-cpp-python is not installed')
         super().__init__(
             model=model,
             temperature=temperature,
             max_retries=max_retries,
```

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/tool_use.prompt` & `bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/tool_use.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/llm/llama_cpp/util.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/llm/llama_cpp/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/ocr/tesseract.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,28 @@
     import pytesseract
     has_pytesseract = True
 except ImportError:
     has_pytesseract = False
 
 logger = logging.getLogger(__name__)
 
-TESSDATA_DIR = "~/.bpm.ai/tessdata/"
-
 
 @cachable()
 class TesseractOCR(OCR):
     """
     Local OCR model based on tesseract.
 
     To use, you should have the ``tesseract`` or ``tesseract-ocr`` package installed.
     """
     def __init__(self):
         if not has_pytesseract:
             raise ImportError('pytesseract is not installed')
-        os.makedirs(TESSDATA_DIR, exist_ok=True)
-        os.environ["TESSDATA_PREFIX"] = TESSDATA_DIR
+        self.tessdata_dir = os.path.join(os.getenv("BPM_AI_CACHE_DIR", os.path.join(os.path.expanduser("~"), ".cache", "bpm-ai")), "tessdata")
+        os.makedirs(self.tessdata_dir, exist_ok=True)
+        os.environ["TESSDATA_PREFIX"] = self.tessdata_dir
 
     @override
     async def _do_process(
             self,
             blob: Blob,
             language: str = None
     ) -> OCRResult:
@@ -78,16 +77,15 @@
         return OCRResult(pages=pages)
 
     def identify_image_language(self, image: Image) -> str:
         self.download_if_missing('eng')
         text = pytesseract.image_to_string(image)
         return indentify_language_iso_639_3(text) or "eng"
 
-    @staticmethod
-    def download_if_missing(lang: str):
+    def download_if_missing(self, lang: str):
         lang_file = f'{lang}.traineddata'
-        tessdata_file_path = os.path.join(TESSDATA_DIR, lang_file)
+        tessdata_file_path = os.path.join(self.tessdata_dir, lang_file)
         if not os.path.exists(tessdata_file_path):
-            logger.info(f'tesseract: {lang_file} not found in {TESSDATA_DIR}, downloading...')
+            logger.info(f'tesseract: {lang_file} not found in {self.tessdata_dir}, downloading...')
             download_url = f'https://github.com/tesseract-ocr/tessdata_best/raw/main/{lang_file}'
             urllib.request.urlretrieve(download_url, tessdata_file_path)
             logger.info(f'tesseract: Downloaded {lang_file} to tessdata directory')
```

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         if device is None:
             device = 'cuda' if torch.cuda.is_available() else 'cpu'
         self.device = device
 
         self.config = None
 
         if cache_folder is None:
-            if 'EASYNMT_CACHE' in os.environ:
-                cache_folder = os.environ['EASYNMT_CACHE']
+            if 'BPM_AI_CACHE_DIR' in os.environ:
+                cache_folder = os.path.join(os.environ['BPM_AI_CACHE_DIR'], 'easynmt_v2')
             else:
                 cache_folder = os.path.join(torch.hub._get_torch_home(), 'easynmt_v2')
         self._cache_folder = cache_folder
 
         if translator is not None:
             self.translator = translator
         else:
```

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.4/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.3.5/bpm_ai_inference/util/optimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 
 def _holisticon_onnx_repository_id(model_name: str) -> str:
     return f"holisticon/{model_name.split('/')[1]}-onnx"
 
 
 def get_optimized_model(model: str, task: str, optimization_level: int = None, push_to_hub: bool = False):
+    logger.info(f"Loading model {model}...")
+
     model_name = model
     model_dir = hf_home() + "/onnx/" + model.replace("/", "--")
     tokenizer = AutoTokenizer.from_pretrained(model)
 
     optimization_level = optimization_level or int(os.getenv("OPTIMIZATION_LEVEL", "2"))
 
     onnx = optimization_level >= 1
@@ -119,14 +121,15 @@
 
     # export to onnx
     return model_class.from_pretrained(repository_id, export=True)
 
 
 @timer
 def _optimize(repository_id: str, model_dir, task, push_to_hub=False):
+    logger.info(f"Optimizing model {repository_id}...")
     model_class = _task_to_model(task)
 
     # try to load from hub or cache
     pre_optimized_model = _try_load_from_hub(repository_id, FILENAME_OPTIMIZED_ONNX, model_class)
     if pre_optimized_model:
         return pre_optimized_model
```

### Comparing `bpm_ai_inference-0.3.4/pyproject.toml` & `bpm_ai_inference-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.3.4"
+version = "0.3.5"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
```

### Comparing `bpm_ai_inference-0.3.4/PKG-INFO` & `bpm_ai_inference-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.3.4
+Version: 0.3.5
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

