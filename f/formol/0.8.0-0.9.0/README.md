# Comparing `tmp/formol-0.8.0.tar.gz` & `tmp/formol-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formol-0.8.0.tar", max compression
+gzip compressed data, was "formol-0.9.0.tar", max compression
```

## Comparing `formol-0.8.0.tar` & `formol-0.9.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0    38310 2024-05-03 17:33:50.048934 formol-0.8.0/formol.py
--rw-r--r--   0        0        0     1786 2024-05-03 17:33:58.382276 formol-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    38310 2024-05-06 21:25:01.447433 formol-0.9.0/formol.py
+-rw-r--r--   0        0        0     1831 2024-05-06 21:25:01.447433 formol-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.9.0/PKG-INFO
```

### Comparing `formol-0.8.0/formol.py` & `formol-0.9.0/formol.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # pyright: strict
 
 __all__ = [
     'format',
     'format_c_block_comment',
     'format_prefixed_block_comment',
 ]
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Philippe Proulx <eepp.ca>'
 
 
 from typing import Dict, Any, Type, TypeVar, Callable, List, Sequence, Union, Pattern, Match, Optional
 from dataclasses import dataclass
 import re
 
@@ -591,15 +591,15 @@
     #        * Lo-fi skateboard pug messenger.
     #
     # Example 3:
     #
     #     c) Meow Mix.
     def _try_parse_ol_item(self):
         # item start?
-        num_m = self._match_cur_line(r'^((?: *\d+)?\. |[a-z]\) )(\S.*)')
+        num_m = self._match_cur_line(r'^((?: *\d+)?\. +|[a-z]\) +)(\S.*)')
 
         if not num_m:
             # no item
             return
 
         # skip first line
         self._goto_next_line()
@@ -678,15 +678,15 @@
     #     pickled. Tofu disrupt poke four loko cronut sus shaman hell of
     #     food truck praxis wolf paleo fam.
     def _try_parse_p(self):
         lines: List[str] = []
 
         while not self._is_done:
             if (self._cur_line_is_empty or self._match_cur_line(self._bullet_line_pat) or
-                                           self._match_cur_line(r'^\. \S.*')):
+                                           self._match_cur_line(r'^\. +\S')):
                 # empty line or list item beginning: end of paragraph
                 break
 
             lines.append(self._cur_line)
             self._goto_next_line()
 
         if len(lines) >= 1:
@@ -744,15 +744,15 @@
     #     >>>
     def _try_parse_blockquote_delim(self):
         lines = self._try_parse_delim_block('>>>')
 
         if lines is not None:
             return _Blockquote(_Parser(lines).elems)
 
-    _verbatim_line_pat = re.compile(r'^(?: *\[\d+\]: [hf]|[│┃┆┇┊┋┌┍┎┏└┕┖┗├┝┞┟┠┡┢┣╎╏║╒╓╔╘╙╚╞╟╠╽╿]).+')
+    _verbatim_line_pat = re.compile(r'^(?: *\[\d+\]: +[hf]|[│┃┆┇┊┋┌┍┎┏└┕┖┗├┝┞┟┠┡┢┣╎╏║╒╓╔╘╙╚╞╟╠╽╿])')
 
     # Tries to parse a verbatim block.
     def _try_parse_verbatim(self):
         lines: List[str] = []
 
         while not self._is_done and self._match_cur_line(self._verbatim_line_pat):
             lines.append(self._cur_line)
```

### Comparing `formol-0.8.0/pyproject.toml` & `formol-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'formol'
-version = '0.8.0'
+version = '0.9.0'
 description = 'Plain text beautifier'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 repository = 'https://github.com/eepp/formol/'
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'License :: OSI Approved :: MIT License',
@@ -38,9 +38,12 @@
     'Topic :: Software Development :: Documentation',
 ]
 packages = [{include = 'formol.py'}]
 
 [tool.poetry.dependencies]
 python = '^3.8'
 
+[tool.poetry.dev-dependencies]
+pytest = '*'
+
 [tool.poetry.urls]
 'Bug tracker' = 'https://github.com/eepp/formol/issues/'
```

### Comparing `formol-0.8.0/PKG-INFO` & `formol-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formol
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plain text beautifier
 Home-page: https://github.com/eepp/formol/
 License: MIT
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

