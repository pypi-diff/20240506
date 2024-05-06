# Comparing `tmp/font_fjallaone-0.1.3.tar.gz` & `tmp/font_fjallaone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font_fjallaone-0.1.3.tar", max compression
+gzip compressed data, was "font_fjallaone-0.1.4.tar", max compression
```

## Comparing `font_fjallaone-0.1.3.tar` & `font_fjallaone-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1904 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/README.md
--rw-r--r--   0        0        0      472 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/font_fjallaone/__init__.py
--rw-r--r--   0        0        0    34848 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/font_fjallaone/files/FjallaOne-Regular.ttf
--rw-r--r--   0        0        0     1460 2024-04-14 19:36:13.439016 font_fjallaone-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 font_fjallaone-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1904 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/README.md
+-rw-r--r--   0        0        0      397 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/font_fjallaone/__init__.py
+-rw-r--r--   0        0        0    34848 2024-05-06 16:37:44.936934 font_fjallaone-0.1.4/font_fjallaone/files/FjallaOne-Regular.ttf
+-rw-r--r--   0        0        0     1348 2024-05-06 16:38:00.424793 font_fjallaone-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 font_fjallaone-0.1.4/PKG-INFO
```

### Comparing `font_fjallaone-0.1.3/README.md` & `font_fjallaone-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `font_fjallaone-0.1.3/font_fjallaone/files/FjallaOne-Regular.ttf` & `font_fjallaone-0.1.4/font_fjallaone/files/FjallaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `font_fjallaone-0.1.3/pyproject.toml` & `font_fjallaone-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 [tool.poetry]
 name = "font-fjallaone"
-version = "v0.1.3" # 0.0.0 placeholder is replaced on release
+version = "v0.1.4" # 0.0.0 placeholder is replaced on release
 description = "Fjalla One from from Sorkin Type as distributed by Google Fonts"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 readme = "README.md"
 packages = [
     { include = "font_fjallaone"},
 ]
 include = ["font_fjallaone/files"]
 
 [tool.poetry.plugins."fonts_ttf"]
 fjallaone = "font_fjallaone:font_files"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.1"
-pytest-cov = ">=4.1,<6.0"
-wheel = ">=0.42,<0.44"
 flake8 = "^7.0.0"
 flake8-docstrings = "^1.7.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 freezegun = "^1.4.0"
-black = "^24.2.0"
-isort = "^5.13.2"
+pytest = "^8.0.1"
+pytest-cov = ">=4.1,<6.0"
 pytest-mypy = "^0.10.3"
-pytest-pylint = "^0.21.0"
 pytest-random-order = "^1.1.1"
+pytest-ruff = "^0.3.1"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.10"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.1"
 mkdocs-section-index = "^0.3.8"
 mkdocs-autorefs = ">=0.5,<1.1"
-mkdocstrings = {extras = ["python"], version = "^0.24.0"}
-
-[tool.isort]
-line_length = 120
-profile = "black"
-
-[tool.pylint.format]
-max-line-lenth = 120
+mkdocstrings = {extras = ["python"], version = ">=0.24,<0.26"}
+wheel = ">=0.42,<0.44"
+ruff = "^0.4.2"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
-addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=font_fjallaone --cov-fail-under=100 --pylint --mypy --ignore=docs/"
+addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=font_fjallaone --cov-fail-under=100 --ruff --mypy --ignore=docs/"
 filterwarnings = [
     "ignore::DeprecationWarning:pylint"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `font_fjallaone-0.1.3/PKG-INFO` & `font_fjallaone-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: font-fjallaone
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fjalla One from from Sorkin Type as distributed by Google Fonts
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Python Package with Fjalla One Font
 
 Python Package with [Fjalla One](https://fonts.google.com/specimen/Fjalla+One) from
```

