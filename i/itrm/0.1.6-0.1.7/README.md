# Comparing `tmp/itrm-0.1.6.tar.gz` & `tmp/itrm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.6.tar", last modified: Mon May  6 20:27:15 2024, max compression
+gzip compressed data, was "itrm-0.1.7.tar", last modified: Mon May  6 20:33:34 2024, max compression
```

## Comparing `itrm-0.1.6.tar` & `itrm-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.318417 itrm-0.1.6/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.6/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:27:15.318290 itrm-0.1.6/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.6/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.6/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:27:15.318658 itrm-0.1.6/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.316415 itrm-0.1.6/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.317252 itrm-0.1.6/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.6/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      320 2024-05-06 20:25:41.000000 itrm-0.1.6/src/itrm/eg_iplot.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    49282 2024-05-06 20:23:16.000000 itrm-0.1.6/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.318071 itrm-0.1.6/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.557486 itrm-0.1.7/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.7/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:33:34.557366 itrm-0.1.7/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.7/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.7/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:33:34.557735 itrm-0.1.7/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.555518 itrm-0.1.7/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.556353 itrm-0.1.7/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.7/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      308 2024-05-06 20:32:31.000000 itrm-0.1.7/src/itrm/eg_iplot.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    49282 2024-05-06 20:32:52.000000 itrm-0.1.7/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.557172 itrm-0.1.7/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.6/LICENSE.txt` & `itrm-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.6/PKG-INFO` & `itrm-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.6/README.md` & `itrm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.6/setup.cfg` & `itrm-0.1.7/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.6
+version = 0.1.7
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.6/src/itrm/itrm.py` & `itrm-0.1.7/src/itrm/itrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     # Check and (possibly) adjust the shapes of x and y.
     x, y = shape_xy(x, y)
     J, K = x.shape
 
     # Get the canvas size.
     tws = screen_size(rows, cols)
     if overlay:
-        print(f"\x1b[{persistent.rows_last + 2}A", end='', flush=True)
+        print(f"\x1b[{persistent.rows_last + 1}A", end='', flush=True)
 
     # Get the data limits, adjusting for the terminal window size.
     lims, _ = limits_xy(x, y, tws, 0) # ignore row_zero
 
     # --------------------
     # Draw a blank canvas.
     # --------------------
```

### Comparing `itrm-0.1.6/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.7/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

