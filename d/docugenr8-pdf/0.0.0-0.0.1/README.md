# Comparing `tmp/docugenr8_pdf-0.0.0.tar.gz` & `tmp/docugenr8_pdf-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8_pdf-0.0.0.tar", last modified: Thu May  2 19:54:38 2024, max compression
+gzip compressed data, was "docugenr8_pdf-0.0.1.tar", last modified: Mon May  6 20:45:30 2024, max compression
```

## Comparing `docugenr8_pdf-0.0.0.tar` & `docugenr8_pdf-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:54:38.909139 docugenr8_pdf-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 19:54:38.909139 docugenr8_pdf-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:54:38.909139 docugenr8_pdf-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:54:38.905140 docugenr8_pdf-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:54:38.909139 docugenr8_pdf-0.0.0/src/docugenr8_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_font.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:54:38.909139 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 19:54:38.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-02 19:54:38.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:54:38.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 19:54:38.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 19:54:38.000000 docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 19:54:07.000000 docugenr8_pdf-0.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.199011 docugenr8_pdf-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/src/docugenr8_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/version.txt
```

### Comparing `docugenr8_pdf-0.0.0/LICENSE` & `docugenr8_pdf-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/PKG-INFO` & `docugenr8_pdf-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-pdf
-Version: 0.0.0
+Version: 0.0.1
 Summary: Docugenr8 add-on library for pdf operations
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,12 +18,12 @@
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
 Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
-Requires-Dist: docugenr8-cicd[build,check,test]; extra == "dev"
+Requires-Dist: docugenr8-pdf[build,check,test]; extra == "dev"
 
 # docugenr8-pdf Library
 
 docugenr8-pdf is a Python library add-on for pdf operations.
```

### Comparing `docugenr8_pdf-0.0.0/pyproject.toml` & `docugenr8_pdf-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [tool.setuptools.dynamic]
 version = { file = "version.txt" }
 
 [project.optional-dependencies]
 check = ["ruff", "mypy"]
 test = ["pytest", "pytest-cov"]
 build = ["build", "setuptools", "twine", "tox"]
-dev = ["docugenr8-cicd[check, test, build]"]
+dev = ["docugenr8-pdf[check, test, build]"]
 
 [tool.ruff]
 extend-exclude = ["docs", "tests"]
 
 [tool.ruff.lint]
 select = ["D", "E", "F"]
 extend-select = ["W", "C90", "I", "N", "B", "A", "C4", "PERF", "RUF"]
```

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/core.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/core.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_content.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_content.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_font.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_font.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_info.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_info.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf/pdf_page.py` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,88 +27,72 @@
             return self._fontname_to_pagefontname[font_name]
         pagefontname = f"F{self._pagefont_num}"
         self._fontname_to_pagefontname[font_name] = pagefontname
         self._pagefontname_fontresource[pagefontname] = pdf_fonts[font_name]
         self._pagefont_num += 1
         return pagefontname
 
-
-    def calc_y(
-        self,
-        y: float,
-        height: float | None = None):
+    def calc_y(self, y: float, height: float | None = None):
         """Change y coordinate from top-to-bottom to bottom-to-top
         and moves content origin to bottom-left."""
         if height is None:
             return self._page_height - y
         return self._page_height - y - height
 
     def generate_pdf_obj(self, collector: Collector):
         self.page_obj = collector.new_obj()
         self.resources_obj = collector.new_obj()
         self.contents_obj = collector.new_obj()
 
     def add_dto_page_contents(
-        self,
-        contents: list[object],
-        pdf_fonts: dict[str, PdfFont]) -> None:
+        self, contents: list[object], pdf_fonts: dict[str, PdfFont]
+    ) -> None:
         for content in contents:
             match content:
                 case DtoTextArea():
                     self.generate_text_area(content, pdf_fonts)
                 case _:
                     raise ValueError("Type not defined.")
 
-    def draw_text_area(
-        self,
-        dto_text_area: DtoTextArea
-        ) -> None:
+    def draw_text_area(self, dto_text_area: DtoTextArea) -> None:
         self._page_contents.add_rectangle(
             x=dto_text_area.x,
-            y=self.calc_y(
-                dto_text_area.y,
-                dto_text_area.height),
+            y=self.calc_y(dto_text_area.y, dto_text_area.height),
             width=dto_text_area.width,
             height=dto_text_area.height,
             fill_color=MaterialColors.Gray100,
             line_color=MaterialColors.Gray600,
-            )
+        )
         for paragraph in dto_text_area.paragraphs:
             self._page_contents.add_rectangle(
                 x=paragraph.x,
-                y=self.calc_y(
-                    paragraph.y,
-                    paragraph.height),
+                y=self.calc_y(paragraph.y, paragraph.height),
                 width=paragraph.width,
                 height=paragraph.height,
                 fill_color=MaterialColors.Teal100,
                 line_color=MaterialColors.Teal600,
-                )
-            for text_line in paragraph.text_lines:
+            )
+            for text_line in paragraph.textlines:
                 self._page_contents.add_rectangle(
                     x=text_line.x,
-                    y=self.calc_y(
-                        text_line.y,
-                        text_line.height),
+                    y=self.calc_y(text_line.y, text_line.height),
                     width=text_line.width,
                     height=text_line.height,
                     fill_color=MaterialColors.Yellow100,
                     line_color=MaterialColors.Yellow600,
-                    )
+                )
                 for word in text_line.words:
                     self._page_contents.add_rectangle(
                         x=word.x,
-                        y=self.calc_y(
-                            word.y,
-                            word.height),
+                        y=self.calc_y(word.y, word.height),
                         width=word.width,
                         height=word.height,
                         fill_color=MaterialColors.DeepOrange100,
                         line_color=MaterialColors.DeepOrange600,
-                        )
+                    )
                     # for fragment in word.fragments:
                     #     self._page_contents.add_rectangle(
                     #         x=fragment.x,
                     #         y=self.calc_y(
                     #             fragment.y,
                     #             fragment.height),
                     #         width=fragment.width,
@@ -116,96 +100,81 @@
                     #         fill_color=MaterialColors.Purple100,
                     #         line_color=MaterialColors.Purple600,
                     #         )
 
     def check_and_update_text_state(
         self,
         current_state: tuple[float, tuple[float, float, float], str]
-            | tuple[None, None, None],
+        | tuple[None, None, None],
         fragment: DtoFragment,
-        pdf_fonts: dict[str, PdfFont]
+        pdf_fonts: dict[str, PdfFont],
     ) -> tuple[float, tuple[float, float, float], str]:
         new_state = (
-                fragment.font_size,
-                fragment.font_color,
-                fragment.font_name,
-            )
+            fragment.font_size,
+            fragment.font_color,
+            fragment.font_name,
+        )
         if (
-            (current_state[0] is None
-                or current_state[1] is None
-                or current_state[2] is None)
-            or new_state != current_state
-            ):
-            page_font_name = self.get_pagefontname(
-                    fragment.font_name,
-                    pdf_fonts)
+            current_state[0] is None
+            or current_state[1] is None
+            or current_state[2] is None
+        ) or new_state != current_state:
+            page_font_name = self.get_pagefontname(fragment.font_name, pdf_fonts)
             self._page_contents.add_page_font_with_size(
-                page_font_name,
-                fragment.font_size)
-            self._page_contents.add_fill_color(
-                fragment.font_color)
+                page_font_name, fragment.font_size
+            )
+            self._page_contents.add_fill_color(fragment.font_color)
             return new_state
         return current_state
 
-    def draw_text_fragment(
-        self,
-        fragment: DtoFragment,
-        pdf_font: PdfFont) -> None:
+    def draw_text_fragment(self, fragment: DtoFragment, pdf_font: PdfFont) -> None:
         cid_in_bytes = bytearray()
         for char in fragment.chars:
             cid = pdf_font.get_cid_in_bytes(char)
             if cid is not None:
                 cid_in_bytes.extend(cid)
         if len(cid_in_bytes) > 0:
             self._page_contents.add_text(
-                fragment.x,
-                self.calc_y(fragment.baseline),
-                cid_in_bytes)
-
-    def generate_text_area(self,
-                           dto_text_area: DtoTextArea,
-                           pdf_fonts: dict[str, PdfFont]):
+                fragment.x, self.calc_y(fragment.baseline), cid_in_bytes
+            )
+
+    def generate_text_area(
+        self, dto_text_area: DtoTextArea, pdf_fonts: dict[str, PdfFont]
+    ):
         self._page_contents.add_savestate()
         self.draw_text_area(dto_text_area)
         current_state = (None, None, None)
         for fragment in dto_text_area.fragments:
             current_state = self.check_and_update_text_state(
-                current_state,
-                fragment,
-                pdf_fonts)
-            self.draw_text_fragment(
-                fragment,
-                pdf_fonts[fragment.font_name])
+                current_state, fragment, pdf_fonts
+            )
+            self.draw_text_fragment(fragment, pdf_fonts[fragment.font_name])
         self._page_contents.add_restore_state()
 
-
     def build(
         self,
         should_compress: bool,
     ):
         if self.page_obj is None:
             raise ValueError("Page object not initialized.")
         if self.resources_obj is None:
             raise ValueError("Resources object not initialized.")
         if self.contents_obj is None:
             raise ValueError("Contents object not initialized.")
         self.page_obj.set_attribute_value(
-            "/MediaBox",
-            f"[0 0 {self._page_width} {self._page_height}]"
+            "/MediaBox", f"[0 0 {self._page_width} {self._page_height}]"
         )
         self.page_obj.set_attribute_value("/Resources", self.resources_obj)
         self.resources_obj.set_attribute_value(
             "/ProcSet", "[/PDF /Text /ImageB /ImageC /ImageI]"
         )
         self.resources_obj.set_attribute_value("/XObject", "<<\t>>")
         self.page_obj.add_attribute_value("/Contents", self.contents_obj)
         if should_compress:
-            self.contents_obj.extend_stream(
-                zlib.compress(
-                    self._page_contents.stream))
+            self.contents_obj.extend_stream(zlib.compress(self._page_contents.stream))
             self.contents_obj.set_attribute_value("/Filter", "/FlateDecode")
         else:
             self.contents_obj.extend_stream(self._page_contents.stream)
         fonts_dict = {}
         for page_fontname, font in self._pagefontname_fontresource.items():
             page_fontname_formatted = f"/{page_fontname}"
             fonts_dict[page_fontname_formatted] = font.obj_num
```

### Comparing `docugenr8_pdf-0.0.0/src/docugenr8_pdf.egg-info/PKG-INFO` & `docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-pdf
-Version: 0.0.0
+Version: 0.0.1
 Summary: Docugenr8 add-on library for pdf operations
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,12 +18,12 @@
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
 Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
-Requires-Dist: docugenr8-cicd[build,check,test]; extra == "dev"
+Requires-Dist: docugenr8-pdf[build,check,test]; extra == "dev"
 
 # docugenr8-pdf Library
 
 docugenr8-pdf is a Python library add-on for pdf operations.
```

