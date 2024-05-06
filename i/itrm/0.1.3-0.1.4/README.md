# Comparing `tmp/itrm-0.1.3.tar.gz` & `tmp/itrm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.3.tar", last modified: Mon May  6 19:38:06 2024, max compression
+gzip compressed data, was "itrm-0.1.4.tar", last modified: Mon May  6 19:49:18 2024, max compression
```

## Comparing `itrm-0.1.3.tar` & `itrm-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.491167 itrm-0.1.3/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.3/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:38:06.491044 itrm-0.1.3/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.3/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.3/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:38:06.491428 itrm-0.1.3/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.489276 itrm-0.1.3/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.490010 itrm-0.1.3/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.3/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    48595 2024-05-06 19:35:25.000000 itrm-0.1.3/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.490814 itrm-0.1.3/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.049425 itrm-0.1.4/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.4/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:49:18.049304 itrm-0.1.4/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.4/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.4/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:49:18.049650 itrm-0.1.4/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.047679 itrm-0.1.4/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.048373 itrm-0.1.4/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.4/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    48599 2024-05-06 19:47:46.000000 itrm-0.1.4/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.049121 itrm-0.1.4/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.3/LICENSE.txt` & `itrm-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.3/PKG-INFO` & `itrm-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.3/README.md` & `itrm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.3/setup.cfg` & `itrm-0.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.3
+version = 0.1.4
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.3/src/itrm/itrm.py` & `itrm-0.1.4/src/itrm/itrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.subrows = subrows
         self.subcols = subcols
 
 # ------------------
 # Plotting functions
 # ------------------
 
-def plot(x, y=None, label='', rows=1, cols=1, equal=0):
+def plot(x, y=None, label=None, rows=1, cols=1, equal=0):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
     plot. Otherwise, the default dimensions (config.cols, config.rows) will be
     used. Note that this function does not plot connecting lines, only the
     points specified by the (`x`, `y`) pairs.
 
@@ -126,15 +126,15 @@
     ranges = f"({ftostr(lims.x_min)}:{ftostr(lims.x_max)}, " \
             + f"{ftostr(lims.y_min)}:{ftostr(lims.y_max)})"
 
     # Draw the plot.
     draw_graph(C, ranges, label, F, row_zero)
 
 
-def iplot(x, y=None, label='', rows=1, cols=1):
+def iplot(x, y=None, label=None, rows=1, cols=1):
     """
     Create an interactive, text-based plot of the path defined by (`x`, `y`)
     using characters. If the size of the terminal can be found, that will be
     used for sizing the plot. Otherwise, the default dimensions (config.cols,
     config.rows) will be used. Note that this function does not plot connecting
     lines, only the points specified by the (`x`, `y`) pairs. Once the function
     has been called, the terminal will be in interactive mode. The user can then
```

### Comparing `itrm-0.1.3/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.4/src/itrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

