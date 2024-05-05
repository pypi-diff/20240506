# Comparing `tmp/sphinxcontrib-screenshot-0.1.0.tar.gz` & `tmp/sphinxcontrib_screenshot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-screenshot-0.1.0.tar", last modified: Fri Mar 29 01:30:48 2024, max compression
+gzip compressed data, was "sphinxcontrib_screenshot-0.1.1.tar", last modified: Sun May  5 22:41:25 2024, max compression
```

## Comparing `sphinxcontrib-screenshot-0.1.0.tar` & `sphinxcontrib_screenshot-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2024-03-29 01:30:48.332075 sphinxcontrib-screenshot-0.1.0/
--rw-r-----   0 tushuhei (175101) primarygroup (89939)    11358 2024-03-29 01:10:26.000000 sphinxcontrib-screenshot-0.1.0/LICENSE
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     2987 2024-03-29 01:30:48.332075 sphinxcontrib-screenshot-0.1.0/PKG-INFO
--rw-r-----   0 tushuhei (175101) primarygroup (89939)     1691 2024-03-29 01:26:08.000000 sphinxcontrib-screenshot-0.1.0/README.md
--rw-r-----   0 tushuhei (175101) primarygroup (89939)     1104 2024-03-29 01:30:48.332075 sphinxcontrib-screenshot-0.1.0/setup.cfg
--rw-r-----   0 tushuhei (175101) primarygroup (89939)      613 2024-03-29 01:10:26.000000 sphinxcontrib-screenshot-0.1.0/setup.py
-drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2024-03-29 01:30:48.328075 sphinxcontrib-screenshot-0.1.0/sphinxcontrib/
--rw-r-----   0 tushuhei (175101) primarygroup (89939)     5985 2024-03-29 01:17:56.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib/screenshot.py
-drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2024-03-29 01:30:48.328075 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/
--rw-r--r--   0 tushuhei (175101) primarygroup (89939)     2987 2024-03-29 01:30:48.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/PKG-INFO
--rw-r-----   0 tushuhei (175101) primarygroup (89939)      320 2024-03-29 01:30:48.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/SOURCES.txt
--rw-r-----   0 tushuhei (175101) primarygroup (89939)        1 2024-03-29 01:30:48.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/dependency_links.txt
--rw-r-----   0 tushuhei (175101) primarygroup (89939)      160 2024-03-29 01:30:48.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/requires.txt
--rw-r-----   0 tushuhei (175101) primarygroup (89939)       14 2024-03-29 01:30:48.000000 sphinxcontrib-screenshot-0.1.0/sphinxcontrib_screenshot.egg-info/top_level.txt
-drwxr-x---   0 tushuhei (175101) primarygroup (89939)        0 2024-03-29 01:30:48.328075 sphinxcontrib-screenshot-0.1.0/tests/
--rw-r-----   0 tushuhei (175101) primarygroup (89939)     1950 2024-03-29 01:16:08.000000 sphinxcontrib-screenshot-0.1.0/tests/test_it.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:41:25.342570 sphinxcontrib_screenshot-0.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11358 2024-04-24 07:32:32.000000 sphinxcontrib_screenshot-0.1.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3652 2024-05-05 22:41:25.342570 sphinxcontrib_screenshot-0.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2312 2024-05-05 22:20:16.000000 sphinxcontrib_screenshot-0.1.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1118 2024-05-05 22:41:25.342570 sphinxcontrib_screenshot-0.1.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      613 2024-04-24 07:32:32.000000 sphinxcontrib_screenshot-0.1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:41:25.338570 sphinxcontrib_screenshot-0.1.1/sphinxcontrib/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5985 2024-05-05 22:40:33.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib/screenshot.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:41:25.338570 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3652 2024-05-05 22:41:25.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-05-05 22:41:25.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-05 22:41:25.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      173 2024-05-05 22:41:25.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2024-05-05 22:41:25.000000 sphinxcontrib_screenshot-0.1.1/sphinxcontrib_screenshot.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:41:25.338570 sphinxcontrib_screenshot-0.1.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1950 2024-04-24 07:32:32.000000 sphinxcontrib_screenshot-0.1.1/tests/test_it.py
```

### Comparing `sphinxcontrib-screenshot-0.1.0/LICENSE` & `sphinxcontrib_screenshot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-screenshot-0.1.0/setup.cfg` & `sphinxcontrib_screenshot-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 	beautifulsoup4
 	build
 	flake8
 	isort
 	mypy
 	Pillow
 	pytest
+	sphinx[test]
 	toml
 	twine
 	types-beautifulsoup4
 	types-docutils
 	types-Pillow
 	types-setuptools
 	yapf
```

### Comparing `sphinxcontrib-screenshot-0.1.0/setup.py` & `sphinxcontrib_screenshot-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-screenshot-0.1.0/sphinxcontrib/screenshot.py` & `sphinxcontrib_screenshot-0.1.1/sphinxcontrib/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Meta = typing.TypedDict('Meta', {
     'version': str,
     'parallel_read_safe': bool,
     'parallel_write_safe': bool
 })
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 
 class ScreenshotDirective(SphinxDirective):
   """Sphinx Screenshot Dirctive.
 
   This directive embeds a screenshot of a webpage.
```

### Comparing `sphinxcontrib-screenshot-0.1.0/tests/test_it.py` & `sphinxcontrib_screenshot-0.1.1/tests/test_it.py`

 * *Files identical despite different names*

