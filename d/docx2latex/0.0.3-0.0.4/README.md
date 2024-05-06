# Comparing `tmp/docx2latex-0.0.3-py3-none-any.whl.zip` & `tmp/docx2latex-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5539 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     9586 b- defN 24-May-05 06:48 docx2latex/__init__.py
+Zip file size: 5540 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     9613 b- defN 24-May-06 14:44 docx2latex/__init__.py
 -rw-rw-rw-  2.0 fat     3132 b- defN 24-May-05 05:29 docx2latex/myutility.py
--rw-rw-rw-  2.0 fat     1071 b- defN 24-May-05 08:55 docx2latex-0.0.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      961 b- defN 24-May-05 08:55 docx2latex-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 08:55 docx2latex-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-05 08:55 docx2latex-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      563 b- defN 24-May-05 08:55 docx2latex-0.0.3.dist-info/RECORD
-7 files, 15416 bytes uncompressed, 4539 bytes compressed:  70.6%
+-rw-rw-rw-  2.0 fat     1071 b- defN 24-May-06 15:29 docx2latex-0.0.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      961 b- defN 24-May-06 15:29 docx2latex-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 15:29 docx2latex-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-06 15:29 docx2latex-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      563 b- defN 24-May-06 15:29 docx2latex-0.0.4.dist-info/RECORD
+7 files, 15443 bytes uncompressed, 4540 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: docx2latex/__init__.py
 Comment: 
 
 Filename: docx2latex/myutility.py
 Comment: 
 
-Filename: docx2latex-0.0.3.dist-info/LICENSE.txt
+Filename: docx2latex-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: docx2latex-0.0.3.dist-info/METADATA
+Filename: docx2latex-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: docx2latex-0.0.3.dist-info/WHEEL
+Filename: docx2latex-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: docx2latex-0.0.3.dist-info/top_level.txt
+Filename: docx2latex-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: docx2latex-0.0.3.dist-info/RECORD
+Filename: docx2latex-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docx2latex/__init__.py

```diff
@@ -2,18 +2,17 @@
 from defusedxml import ElementTree
 from xml.etree.ElementTree import fromstring
 import os, re
 from .myutility import xml_tags, tag_to_latex_exp
 
 
 class Document:
-    n_images = 0
-
     def __init__(self, document, inline_delimiter="$", block_delimiter="$$"):
         self.document = document
+        self.n_images = 0
         self.inline_delimiter = inline_delimiter
         self.block_delimiter = block_delimiter
 
     def check_file(self):
         return os.path.exists(self.document)
 
     def get_text(
@@ -27,15 +26,15 @@
             return "file not exist"
 
         if extensions is None:
             extensions = [".jpg", ".jpeg", ".png", ".svg", ".bmp", ".gif"]
         zip_f = zipfile.ZipFile(self.document)
         text = ""
         for f in zip_f.namelist():
-            text += self.xml_reader(zip_f.read(f),True)
+            # text += self.xml_reader(zip_f.read(f))
             if get_header_text and f.startswith("word/header"):
                 text += self.xml_to_text(zip_f.read(f))
             if f.startswith("word/document"):
                 text += self.xml_to_text(zip_f.read(f))
             if get_footer_text and f.startswith("word/footer"):
                 text += self.xml_to_text(zip_f.read(f))
 
@@ -76,15 +75,15 @@
             return "file not exist"
 
         if extensions is None:
             extensions = [".jpg", ".jpeg", ".png", ".svg", ".bmp", ".gif"]
         zip_f = zipfile.ZipFile(self.document)
         text = ""
         for f in zip_f.namelist():
-            text += self.xml_reader(zip_f.read(f),True) # for w:hrd ,foot
+            # text += self.xml_reader_text(zip_f.read(f)) # for w:hrd ,foot
             if get_header_text and f.startswith("word/head"):
                 text += self.xml_to_text(zip_f.read(f))
             if f.startswith("word/document"):
                 text += self.xml_to_html(zip_f.read(f))
 
             if get_footer_text and f.startswith("word/footer"):
                 text += self.xml_to_text(zip_f.read(f))
@@ -127,15 +126,15 @@
         return text
 
 
 
 
     def xml_to_text(self, xml):
         text = ""
-        n_images = 0
+        # global n_images
         root = ElementTree.fromstring(xml)
         for child in root.iter():
             if child.get("docxlatex_skip_iteration", False):
                 continue
 
             if child.tag == xml_tags("w:t"):
                 text += child.text if child.text is not None else ""
@@ -143,36 +142,36 @@
                 text += self.inline_delimiter + " "
                 text += tag_to_latex_exp(child)
                 text += " " + self.inline_delimiter
             elif child.tag == xml_tags("m:r"):
                 text += "".join(child.itertext())
             elif child.tag == xml_tags("w:drawing"):
                 print("img")
-                n_images += 1
-                text += f"\nIMAGE#{n_images}-image{n_images}\n"
+                self.n_images += 1
+                text += f"\nIMAGE#{self.n_images}-image{self.n_images}\n"
 
             elif child.tag == xml_tags("w:tab"):
                 text += "\t"
             elif child.tag == xml_tags("w:br") or child.tag == xml_tags("w:cr"):
                 text += "\n"
             elif child.tag == xml_tags("w:p"):
                 text += "\n\n"
 
         text = re.sub(r"\n(\n+)\$(\s*.+\s*)\$\n", r"\n\1$ \2 $", text)
         return text
 
     def get_t(self, xml):
-        global n_images  # Assuming n_images is initialized elsewhere
+        # global n_images  # Assuming n_images is initialized elsewhere
         text = ""
         for e in xml:
             if e.tag == xml_tags("w:t"):
                 text += e.text
             elif e.tag == xml_tags("w:drawing"):
-                n_images += 1
-                text += f'<img src="word/media/image{n_images}.png" alt="Image{n_images}"/>\n'
+                self.n_images += 1
+                text += f'<img src="word/media/image{self.n_images}.png" alt="Image{self.n_images}"/>\n'
         if len(text) > 0:
             return text
         return ""
 
     def get_paragraphs(self, xml):
         text = ""
         for e in xml:  # r,omath
@@ -212,15 +211,14 @@
                         html += self.get_table(doc_element)
 
         html += "</body>"
         html = html.replace("$ $", "$ ")  # Example replacement, modify as necessary
         return html
 
     def get_table(self, element, depth=0):
-        global n_images
         html = ""
         if element.tag == xml_tags("w:tbl"):
             # Start a new table
             html += f"{'  ' * depth}<table border='1'>\n"
 
             for child in element:
                 if child.tag == xml_tags("w:tr"):
@@ -235,15 +233,15 @@
                             elif item.tag == xml_tags("w:p"):
                                 # Handle paragraph
                                 cell_html += self.get_paragraphs(item)
 
                         html += (
                             f"{'  ' * depth}  <td>{cell_html}</td>\n"
                             if len(cell_html) > 0
-                            else ""
+                            else "<td></td>"
                         )
                     html += f"{'  ' * depth} </tr>\n"
 
             html += f"{'  ' * depth}</table>\n"
             return html
         else:
             # Process non-table elements or skip
```

## Comparing `docx2latex-0.0.3.dist-info/LICENSE.txt` & `docx2latex-0.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `docx2latex-0.0.3.dist-info/METADATA` & `docx2latex-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx2latex
-Version: 0.0.3
+Version: 0.0.4
 Summary: convert docx file to html code including latex linear equation
 Author: shadan
 Author-email: shadanparvez64@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

