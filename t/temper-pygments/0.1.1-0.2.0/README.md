# Comparing `tmp/temper_pygments-0.1.1.tar.gz` & `tmp/temper_pygments-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_pygments-0.1.1.tar", max compression
+gzip compressed data, was "temper_pygments-0.2.0.tar", max compression
```

## Comparing `temper_pygments-0.1.1.tar` & `temper_pygments-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      627 2023-08-04 17:20:48.737120 temper_pygments-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-04-28 18:18:11.562467 temper_pygments-0.1.1/README.md
--rw-r--r--   0        0        0       84 2023-04-28 19:43:49.952098 temper_pygments-0.1.1/temper_pygments/__init__.py
--rw-r--r--   0        0        0     1795 2023-05-02 11:52:30.257645 temper_pygments-0.1.1/temper_pygments/adapt.py
--rw-r--r--   0        0        0      704 2023-04-28 23:09:13.160673 temper_pygments-0.1.1/temper_pygments/lexer.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 temper_pygments-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-08-07 13:56:22.116986 temper_pygments-0.2.0/README.md
+-rw-r--r--   0        0        0      627 2024-05-06 17:33:06.817227 temper_pygments-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-08-07 13:56:22.116986 temper_pygments-0.2.0/temper_pygments/__init__.py
+-rw-r--r--   0        0        0     1899 2024-05-04 00:15:33.423258 temper_pygments-0.2.0/temper_pygments/adapt.py
+-rw-r--r--   0        0        0      651 2024-05-04 00:47:09.686064 temper_pygments-0.2.0/temper_pygments/lexer.py
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 temper_pygments-0.2.0/PKG-INFO
```

### Comparing `temper_pygments-0.1.1/pyproject.toml` & `temper_pygments-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "temper-pygments"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Tom <tom@temper.systems>"]
 readme = "README.md"
 packages = [{include = "temper_pygments"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pygments = "^2.12.0"
-temper-core = "0.0.5"
-temper-syntax = "0.1.1"
+temper-core = "0.2.1"
+temper-syntax = "0.2.0"
 
 [tool.poetry.plugins."pygments.lexers"]
 temper = "temper_pygments:TemperLexer"
 tempermd = "temper_pygments:TemperMdLexer"
 
 [tool.poetry.scripts]
 bundle = 'scripts:bundle'
```

### Comparing `temper_pygments-0.1.1/temper_pygments/adapt.py` & `temper_pygments-0.2.0/temper_pygments/adapt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import pygments.unistring as uni
-from pygments.lexer import Lexer, bygroups, include, inherit, using
+import temper_syntax.pygments as tsp
+from pygments.lexer import Lexer, bygroups, default, include, inherit, using
 from pygments.token import Token
-from temper_syntax.pygments import ByGroups, Kind, Include, Inherit, Rule, Using
 
 
 def adapt_kind(kind):
-    if isinstance(kind, ByGroups):
+    if isinstance(kind, tsp.ByGroups):
         return bygroups(*[adapt_kind(sub) for sub in kind.kinds])
-    elif isinstance(kind, Kind):
+    elif isinstance(kind, tsp.Kind):
         return kinds[kind.name]
-    elif isinstance(kind, Using):
+    elif isinstance(kind, tsp.Using):
         return using(lexers[kind.lexer])
     raise ValueError(f"unknown kind: {kind}")
 
 
 def adapt_regex(regex: str):
     return regex.replace("<<Lu>>", uni.Lu).replace("<<Ll>>", uni.Ll)
 
 
 def adapt_rule(rule):
-    if isinstance(rule, Include):
+    if isinstance(rule, tsp.Default):
+        return default(rule.state)
+    elif isinstance(rule, tsp.Include):
         return include(rule.state)
-    elif isinstance(rule, Inherit):
+    elif isinstance(rule, tsp.Inherit):
         return inherit
-    elif isinstance(rule, Rule):
+    elif isinstance(rule, tsp.Rule):
         result = (adapt_regex(rule.regex), adapt_kind(rule.kind))
         if rule.state is not None:
             result = (*result, rule.state)
         return result
     raise ValueError(f"unknown rule type: {rule}")
 
 
@@ -49,11 +51,12 @@
     "Name.Builtin": Token.Name.Builtin,
     "Name.Decorator": Token.Name.Decorator,
     "Number": Token.Number,
     "Operator": Token.Operator,
     "Punctuation": Token.Punctuation,
     "String": Token.String,
     "String.Interpol": Token.String.Interpol,
+    "String.Regex": Token.String.Regex,
     "Whitespace": Token.Whitespace,
 }
 
 lexers: dict[str, Lexer] = {}
```

### Comparing `temper_pygments-0.1.1/temper_pygments/lexer.py` & `temper_pygments-0.2.0/temper_pygments/lexer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pygments.lexer import RegexLexer
 from pygments.lexers.markup import MarkdownLexer
 from temper_pygments.adapt import adapt_tokens, lexers
 from temper_syntax import temper_pygments as t
-from temper_syntax import tempermd_pygments as tmd
 
 
 _temper = t.TemperLexer()
-_tempermd = tmd.TemperMdLexer()
+_tempermd = t.TemperMdLexer()
 
 
 class TemperLexer(RegexLexer):
     name = _temper.name
     aliases = _temper.aliases
     filenames = _temper.filenames
     tokens = adapt_tokens(_temper.tokens)
```

### Comparing `temper_pygments-0.1.1/PKG-INFO` & `temper_pygments-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: temper-pygments
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Tom
 Author-email: tom@temper.systems
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pygments (>=2.12.0,<3.0.0)
-Requires-Dist: temper-core (==0.0.5)
-Requires-Dist: temper-syntax (==0.1.1)
+Requires-Dist: temper-core (==0.2.1)
+Requires-Dist: temper-syntax (==0.2.0)
 Description-Content-Type: text/markdown
 
 Pygments lexer for Temper.
```

