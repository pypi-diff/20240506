# Comparing `tmp/re_ircbot-2.0.5.dev0.tar.gz` & `tmp/re_ircbot-2.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.5.dev0.tar", last modified: Sun May  5 19:20:31 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.6.dev0.tar", last modified: Sun May  5 22:01:30 2024, max compression
```

## Comparing `re_ircbot-2.0.5.dev0.tar` & `re_ircbot-2.0.6.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54808 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5004 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/format.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18286 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-05 22:01:22.000000 re_ircbot-2.0.6.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-05 22:01:22.000000 re_ircbot-2.0.6.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54808 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5594 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18286 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/setup.py
```

### Comparing `re_ircbot-2.0.5.dev0/LICENSE` & `re_ircbot-2.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/PKG-INFO` & `re_ircbot-2.0.6.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.5.dev0
+Version: 2.0.6.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.5.dev0/README.md` & `re_ircbot-2.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/client.py` & `re_ircbot-2.0.6.dev0/ircbot/client.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/dcc.py` & `re_ircbot-2.0.6.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/format.py` & `re_ircbot-2.0.6.dev0/ircbot/format.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 import re
 
 
 class Style:
     reset = "\x0F"
+    str: str
 
 
 class TextStyle(Style):
     """Text styles enum.
     https://modern.ircdocs.horse/formatting
     """
 
@@ -155,15 +156,15 @@
             from pygments import formatters, lexers
             from pygments.util import ClassNotFound
         except ImportError:
             raise ImportError("You need to install pygments to use syntax highlighting. pip install pygments")
         try:
             Lexer = lexers.find_lexer_class_by_name(lang)
         except ClassNotFound:
-            Lexer = lexers.BashLexer
+            Lexer = lexers.TextLexer
 
         return pygments.highlight(content, Lexer(), formatters.IRCFormatter(bg="dark"))
 
     def replace_simple(text: str) -> str:
         for k, v in translation_map.items():
             regex = re.compile(f"{k}(.+?){k}")
             text = regex.sub(f"{v}\\1{TextStyle.reset}", text)
@@ -175,11 +176,26 @@
             for i, inner in enumerate(part.split("`")):
                 if i % 2 == 0:
                     output += replace_simple(inner)
                 else:
                     output += Color(f" {inner} ", fg=Color.light_gray, bg=Color.black).str
         else:
             lang, code = part.split("\n", 1)
-            for line in code.split("\n"):
-                output += highlight_code(line, lang.strip() or "bash")
+            highlighted_text = highlight_code(code, lang.strip() or "bash")
+
+            # We need to restore the unclosed escape sequences for each of the lines
+            color = ""
+            for line in highlighted_text.split("\n"):
+                if color:
+                    line = color + line
+
+                output += line + "\n"
+
+                for i, char in enumerate(line):
+                    if char == Color.esc:
+                        match = re.search(r"\x03\d{1,2}(,\d{1,2})?.*$", line[i:])
+                        if match:
+                            color = f"\x03{match[0]}{match[1] or ''}"
+                        else:
+                            color = ""
 
     return output
```

### Comparing `re_ircbot-2.0.5.dev0/ircbot/hooks.py` & `re_ircbot-2.0.6.dev0/ircbot/hooks.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/message.py` & `re_ircbot-2.0.6.dev0/ircbot/message.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.6.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.6.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/ircbot/utils.py` & `re_ircbot-2.0.6.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.5.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.6.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.5.dev0
+Version: 2.0.6.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.5.dev0/setup.py` & `re_ircbot-2.0.6.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.5-dev"
+VERSION = "2.0.6-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

