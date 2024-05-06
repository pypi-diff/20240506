# Comparing `tmp/docugenr8-0.0.0.tar.gz` & `tmp/docugenr8-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8-0.0.0.tar", last modified: Mon May  6 19:15:02 2024, max compression
+gzip compressed data, was "docugenr8-0.0.1.tar", last modified: Mon May  6 19:58:05 2024, max compression
```

## Comparing `docugenr8-0.0.0.tar` & `docugenr8-0.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.465435 docugenr8-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-06 19:14:31.000000 docugenr8-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 19:15:02.465435 docugenr8-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 19:14:31.000000 docugenr8-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 19:14:31.000000 docugenr8-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:15:02.465435 docugenr8-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.457435 docugenr8-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.461435 docugenr8-0.0.0/src/docugenr8/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/build_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/font.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.461435 docugenr8-0.0.0/src/docugenr8/text_area/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/paragraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/textline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/word.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-06 19:14:31.000000 docugenr8-0.0.0/src/docugenr8/text_area/words_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.465435 docugenr8-0.0.0/src/docugenr8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 19:15:02.000000 docugenr8-0.0.0/src/docugenr8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 19:15:02.000000 docugenr8-0.0.0/src/docugenr8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:15:02.000000 docugenr8-0.0.0/src/docugenr8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-06 19:15:02.000000 docugenr8-0.0.0/src/docugenr8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 19:15:02.000000 docugenr8-0.0.0/src/docugenr8.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:15:02.465435 docugenr8-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-06 19:14:31.000000 docugenr8-0.0.0/tests/test_1.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 19:14:31.000000 docugenr8-0.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.536198 docugenr8-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-06 19:57:34.000000 docugenr8-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 19:58:05.536198 docugenr8-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 19:57:34.000000 docugenr8-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 19:57:34.000000 docugenr8-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:58:05.536198 docugenr8-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.528198 docugenr8-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.528198 docugenr8-0.0.1/src/docugenr8/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/build_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.532198 docugenr8-0.0.1/src/docugenr8/text_area/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/textline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-06 19:57:34.000000 docugenr8-0.0.1/src/docugenr8/text_area/words_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.532198 docugenr8-0.0.1/src/docugenr8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-06 19:58:05.000000 docugenr8-0.0.1/src/docugenr8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 19:58:05.000000 docugenr8-0.0.1/src/docugenr8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:58:05.000000 docugenr8-0.0.1/src/docugenr8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-06 19:58:05.000000 docugenr8-0.0.1/src/docugenr8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 19:58:05.000000 docugenr8-0.0.1/src/docugenr8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.532198 docugenr8-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-06 19:57:34.000000 docugenr8-0.0.1/tests/test_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 19:57:34.000000 docugenr8-0.0.1/version.txt
```

### Comparing `docugenr8-0.0.0/LICENSE` & `docugenr8-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/PKG-INFO` & `docugenr8-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.0/pyproject.toml` & `docugenr8-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/__init__.py` & `docugenr8-0.0.1/src/docugenr8/__init__.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/build_dto.py` & `docugenr8-0.0.1/src/docugenr8/build_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,54 @@
 """build_dto module.
 
 This module provides functionality to build Data Transfer Objects (DTOs) for
 transferring document information between modules.
 """
 
+from typing import TYPE_CHECKING
+
+
+if TYPE_CHECKING:
+    from ..docugenr8 import Document
+
+from docugenr8_shared.dto import Dto
+from docugenr8_shared.dto import DtoFont
 from docugenr8_shared.dto import DtoFragment
+from docugenr8_shared.dto import DtoPage
 from docugenr8_shared.dto import DtoParagraph
 from docugenr8_shared.dto import DtoTextArea
 from docugenr8_shared.dto import DtoTextLine
 from docugenr8_shared.dto import DtoWord
 
 from .text_area.fragment import Fragment
 from .text_area.paragraph import Paragraph
 from .text_area.textarea import TextArea
 from .text_area.textline import TextLine
 from .text_area.word import Word
 
 
+def build_dto(doc: Document) -> Dto:
+    dto = Dto()
+    for font_name, font in doc.fonts.items():
+        dto_font = DtoFont(font_name, font.raw_data)
+        dto.fonts.append(dto_font)
+    for page_number, page in enumerate(doc.pages):
+        dto_page = DtoPage(page._width, page._height)
+        dto.pages.append(dto_page)
+        for content in page._contents:
+            match content:
+                case TextArea():
+                    content._build_current_page_fragments(page_number + 1)
+                    content._build_total_pages_fragments(len(doc.pages))
+                    dto_page.contents.append(_generate_dto_text_area(content))
+                case _:
+                    raise TypeError("Invalid content type.")
+    return dto
+
+
 def _generate_dto_fragment(
     x: float,
     y: float,
     dto_word: DtoWord,
     fragment: Fragment,
 ) -> DtoFragment:
     """Generate Dto fragment object. Dto fragment object is the smallest posible object that holds one character.
```

### Comparing `docugenr8-0.0.0/src/docugenr8/font.py` & `docugenr8-0.0.1/src/docugenr8/font.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/settings.py` & `docugenr8-0.0.1/src/docugenr8/settings.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/fragment.py` & `docugenr8-0.0.1/src/docugenr8/text_area/fragment.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/paragraph.py` & `docugenr8-0.0.1/src/docugenr8/text_area/paragraph.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/textarea.py` & `docugenr8-0.0.1/src/docugenr8/text_area/textarea.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/textline.py` & `docugenr8-0.0.1/src/docugenr8/text_area/textline.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/word.py` & `docugenr8-0.0.1/src/docugenr8/text_area/word.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8/text_area/words_creation.py` & `docugenr8-0.0.1/src/docugenr8/text_area/words_creation.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/src/docugenr8.egg-info/PKG-INFO` & `docugenr8-0.0.1/src/docugenr8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.0/src/docugenr8.egg-info/SOURCES.txt` & `docugenr8-0.0.1/src/docugenr8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.0/tests/test_1.py` & `docugenr8-0.0.1/tests/test_1.py`

 * *Files identical despite different names*

