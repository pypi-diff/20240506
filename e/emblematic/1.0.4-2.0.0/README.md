# Comparing `tmp/emblematic-1.0.4.tar.gz` & `tmp/emblematic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emblematic-1.0.4.tar", max compression
+gzip compressed data, was "emblematic-2.0.0.tar", max compression
```

## Comparing `emblematic-1.0.4.tar` & `emblematic-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    13827 2023-11-19 03:43:02.182883 emblematic-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0      309 2023-11-19 03:43:02.182883 emblematic-1.0.4/README.md
--rw-r--r--   0        0        0       85 2023-11-19 03:43:02.186883 emblematic-1.0.4/emblematic/__init__.py
--rw-r--r--   0        0        0     2927 2023-11-19 03:43:02.186883 emblematic-1.0.4/emblematic/__main__.py
--rw-r--r--   0        0        0     1252 2023-11-19 03:43:02.186883 emblematic-1.0.4/emblematic/compose.py
--rw-r--r--   0        0        0      378 2023-11-19 03:43:02.186883 emblematic-1.0.4/emblematic/files.py
--rw-r--r--   0        0        0     4410 2023-11-19 03:43:02.186883 emblematic-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 emblematic-1.0.4/setup.py
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 emblematic-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-05-05 22:53:16.242353 emblematic-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      392 2024-05-06 00:30:45.767822 emblematic-2.0.0/README.md
+-rw-r--r--   0        0        0       85 2024-05-05 22:53:16.248353 emblematic-2.0.0/emblematic/__init__.py
+-rw-r--r--   0        0        0     4454 2024-05-06 00:43:54.642886 emblematic-2.0.0/emblematic/__main__.py
+-rw-r--r--   0        0        0     1247 2024-05-06 01:05:37.860990 emblematic-2.0.0/emblematic/compose.py
+-rw-r--r--   0        0        0      378 2024-05-05 22:53:16.248353 emblematic-2.0.0/emblematic/files.py
+-rw-r--r--   0        0        0     4390 2024-05-06 01:24:32.476081 emblematic-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 emblematic-2.0.0/PKG-INFO
```

### Comparing `emblematic-1.0.4/LICENSE.txt` & `emblematic-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emblematic-1.0.4/emblematic/compose.py` & `emblematic-2.0.0/emblematic/compose.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     background.attrs["height"] = "100%"
 
     icon = icon.__copy__()
     icon.attrs["id"] = "emblematic-icon"
     icon.attrs["width"] = "63%"
     icon.attrs["height"] = "63%"
     icon.attrs["preserveAspectRatio"] = "xMidYMid meet"
-    icon.attrs["transform"] = f"translate({width * 0.37 / 2}, {height * 0.37 / 2})"
+    icon.attrs["x"] = width * 0.37 / 2
+    icon.attrs["y"] = height * 0.37 / 2
 
     doc = bs4.BeautifulSoup(f"""
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 {width} {height}">
     </svg>
     """, features="lxml-xml")
     container: bs4.Tag = doc.svg
     container.append(background)
```

### Comparing `emblematic-1.0.4/pyproject.toml` & `emblematic-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "emblematic"
 
 # The version of the package.
-version = "1.0.4"
+version = "2.0.0"
 
 # A brief, one-sentence description about your project.
 description = "Generate emblems from an icon and a background"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
@@ -129,21 +129,20 @@
 #         ^3.10.1  →  == 3      && >= 3.10.1
 # ~X.X.X means "newer releases with this minor version"
 #         ~3.10.1  →  == 3.10   && >= 3.10.1
 # nothing means "this specific release"
 #          3.10.1  →  == 3.10.1
 
 python = "^3.10"
-cairosvg = "^2.6.0"
-click = "^8.1.3"
-beautifulsoup4 = "^4.11.2"
-lxml = "^4.9.2"
+click = "^8.1.7"
+beautifulsoup4 = "^4.12.3"
+lxml = "^5.2.1"
 
-Sphinx = { version = "^7.2.6", optional = true }
-sphinx-rtd-theme = { version = "^1.2.0", optional = true }
+Sphinx = { version = "^7.3.7", optional = true }
+sphinx-rtd-theme = { version = "^2.0.0", optional = true }
 
 
 [tool.poetry.extras]
 ####################
 # Package extras   #
 ####################
 # ADVANCED: specify optional dependency groups.
```

### Comparing `emblematic-1.0.4/PKG-INFO` & `emblematic-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emblematic
-Version: 1.0.4
+Version: 2.0.0
 Summary: Generate emblems from an icon and a background
 Home-page: https://github.com/Steffo99/emblematic/
 License: EUPL-1.2
 Keywords: icon,avatar,emblem,logo,symbol
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
@@ -13,33 +13,35 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Typing :: Typed
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=7.2.6,<8.0.0) ; extra == "docs"
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: cairosvg (>=2.6.0,<3.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
+Requires-Dist: Sphinx (>=7.3.7,<8.0.0) ; extra == "docs"
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0) ; extra == "docs"
 Project-URL: Documentation, https://emblematic.readthedocs.io/latest/
 Project-URL: Repository, https://github.com/Steffo99/emblematic/
 Description-Content-Type: text/markdown
 
 # ![](media/icon-round-100x100.png) Emblematic
 
 Generate emblems from an icon and a background
 
+## Requirements
+
+Emblematic requires Inkscape to be installed and in the PATH.
+
 ## Links
 
 [![PyPI](https://img.shields.io/pypi/v/emblematic)](https://pypi.org/project/emblematic)
  
 [![Documentation](https://img.shields.io/readthedocs/emblematic
-)](https://emblematic.readthedocs.io/latest/)
+)](https://emblematic.readthedocs.io/en/latest/)
```

