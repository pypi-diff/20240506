# Comparing `tmp/double_indent_shiku-0.1.5.tar.gz` & `tmp/double_indent_shiku-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "double_indent_shiku-0.1.5.tar", last modified: Fri May  3 15:36:07 2024, max compression
+gzip compressed data, was "double_indent_shiku-0.1.6.tar", last modified: Mon May  6 07:07:01 2024, max compression
```

## Comparing `double_indent_shiku-0.1.5.tar` & `double_indent_shiku-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 konovalyuk.d   (501) staff       (20)        0 2024-05-03 15:36:07.099773 double_indent_shiku-0.1.5/
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1714 2024-05-03 15:36:07.099707 double_indent_shiku-0.1.5/PKG-INFO
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1094 2024-05-03 15:19:30.000000 double_indent_shiku-0.1.5/README.md
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)     3890 2024-05-03 15:06:22.000000 double_indent_shiku-0.1.5/double_indent.py
-drwxr-xr-x   0 konovalyuk.d   (501) staff       (20)        0 2024-05-03 15:36:07.099479 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1714 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/PKG-INFO
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)      305 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/SOURCES.txt
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)        1 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/dependency_links.txt
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)       53 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/entry_points.txt
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)       12 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/requires.txt
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)       14 2024-05-03 15:36:07.000000 double_indent_shiku-0.1.5/double_indent_shiku.egg-info/top_level.txt
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1152 2024-05-03 15:36:07.100086 double_indent_shiku-0.1.5/setup.cfg
--rw-r--r--   0 konovalyuk.d   (501) staff       (20)       37 2024-05-03 11:41:41.000000 double_indent_shiku-0.1.5/setup.py
+drwxr-xr-x   0 konovalyuk.d   (501) staff       (20)        0 2024-05-06 07:07:01.329104 double_indent_shiku-0.1.6/
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1714 2024-05-06 07:07:01.329038 double_indent_shiku-0.1.6/PKG-INFO
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1094 2024-05-06 06:07:31.000000 double_indent_shiku-0.1.6/README.md
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)     3838 2024-05-06 07:00:54.000000 double_indent_shiku-0.1.6/double_indent.py
+drwxr-xr-x   0 konovalyuk.d   (501) staff       (20)        0 2024-05-06 07:07:01.328817 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1714 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/PKG-INFO
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)      305 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/SOURCES.txt
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)        1 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/dependency_links.txt
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)       53 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/entry_points.txt
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)       12 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/requires.txt
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)       14 2024-05-06 07:07:01.000000 double_indent_shiku-0.1.6/double_indent_shiku.egg-info/top_level.txt
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)     1152 2024-05-06 07:07:01.329404 double_indent_shiku-0.1.6/setup.cfg
+-rw-r--r--   0 konovalyuk.d   (501) staff       (20)       37 2024-05-06 06:07:31.000000 double_indent_shiku-0.1.6/setup.py
```

### Comparing `double_indent_shiku-0.1.5/PKG-INFO` & `double_indent_shiku-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: double_indent_shiku
-Version: 0.1.5
+Version: 0.1.6
 Summary: a code formatter indenting function and method definitions twice. Fork to indent function calls
 Home-page: https://github.com/shiku-shi/double-indent
 Author: Shiku Shi
 Author-email: shiku-shi@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `double_indent_shiku-0.1.5/README.md` & `double_indent_shiku-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `double_indent_shiku-0.1.5/double_indent.py` & `double_indent_shiku-0.1.6/double_indent.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,19 +52,17 @@
         end: int,
         indent: int,
         offset: int,
 ) -> None:
     idx = start
     while idx < end - 2:
         if tokens[idx].name == "NL":
-            if (
-                    tokens[idx + 1].name == "UNIMPORTANT_WS"
-                    and len(tokens[idx + 1].src) != (indent * 2) + offset
-            ):
-                new_indent = " " * ((indent * 2) + offset)
+            if tokens[idx + 1].name == "UNIMPORTANT_WS":
+                old_indent = tokens[idx + 1].src.count(" ")
+                new_indent = " " * (indent + old_indent)
                 tokens[idx + 1] = tokens[idx + 1]._replace(src=new_indent)
         idx += 1
 
 
 def _fix_src(contents_text: str, indent: int) -> str:
     tokens = src_to_tokens(contents_text)
     for idx, token in reversed_enumerate(tokens):
```

### Comparing `double_indent_shiku-0.1.5/double_indent_shiku.egg-info/PKG-INFO` & `double_indent_shiku-0.1.6/double_indent_shiku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: double_indent_shiku
-Version: 0.1.5
+Version: 0.1.6
 Summary: a code formatter indenting function and method definitions twice. Fork to indent function calls
 Home-page: https://github.com/shiku-shi/double-indent
 Author: Shiku Shi
 Author-email: shiku-shi@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `double_indent_shiku-0.1.5/setup.cfg` & `double_indent_shiku-0.1.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = double_indent_shiku
-version = 0.1.5
+version = 0.1.6
 description = a code formatter indenting function and method definitions twice. Fork to indent function calls
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shiku-shi/double-indent
 author = Shiku Shi
 author_email = shiku-shi@users.noreply.github.com
 license = MIT
```

