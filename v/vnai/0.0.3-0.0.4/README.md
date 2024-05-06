# Comparing `tmp/vnai-0.0.3.tar.gz` & `tmp/vnai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnai-0.0.3.tar", last modified: Mon May  6 15:57:34 2024, max compression
+gzip compressed data, was "vnai-0.0.4.tar", last modified: Mon May  6 16:05:06 2024, max compression
```

## Comparing `vnai-0.0.3.tar` & `vnai-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 15:57:34.714931 vnai-0.0.3/
--rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 15:57:34.714836 vnai-0.0.3/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.3/pyproject.toml
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 15:57:34.712891 vnai-0.0.3/raw/
--rw-r--r--   0 mrthinh    (501) staff       (20)    14590 2024-05-06 15:56:20.000000 vnai-0.0.3/raw/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    14534 2024-04-28 17:10:37.000000 vnai-0.0.3/raw/analytics.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      204 2024-04-26 15:44:24.000000 vnai-0.0.3/raw/setup.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      563 2024-05-06 15:57:34.715201 vnai-0.0.3/setup.cfg
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 15:57:34.713295 vnai-0.0.3/vnai/
--rw-r--r--   0 mrthinh    (501) staff       (20)    14590 2024-05-06 15:53:15.000000 vnai-0.0.3/vnai/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 15:57:34.714479 vnai-0.0.3/vnai.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 15:57:34.000000 vnai-0.0.3/vnai.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      226 2024-05-06 15:57:34.000000 vnai-0.0.3/vnai.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-06 15:57:34.000000 vnai-0.0.3/vnai.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)       42 2024-05-06 15:57:34.000000 vnai-0.0.3/vnai.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        9 2024-05-06 15:57:34.000000 vnai-0.0.3/vnai.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:05:06.924967 vnai-0.0.4/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 16:05:06.924878 vnai-0.0.4/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.4/pyproject.toml
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:05:06.923145 vnai-0.0.4/raw/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14715 2024-05-06 16:04:41.000000 vnai-0.0.4/raw/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14534 2024-04-28 17:10:37.000000 vnai-0.0.4/raw/analytics.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      204 2024-04-26 15:44:24.000000 vnai-0.0.4/raw/setup.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      563 2024-05-06 16:05:06.925219 vnai-0.0.4/setup.cfg
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:05:06.923529 vnai-0.0.4/vnai/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14590 2024-05-06 15:53:15.000000 vnai-0.0.4/vnai/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:05:06.924521 vnai-0.0.4/vnai.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 16:05:06.000000 vnai-0.0.4/vnai.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      226 2024-05-06 16:05:06.000000 vnai-0.0.4/vnai.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-06 16:05:06.000000 vnai-0.0.4/vnai.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       42 2024-05-06 16:05:06.000000 vnai-0.0.4/vnai.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        9 2024-05-06 16:05:06.000000 vnai-0.0.4/vnai.egg-info/top_level.txt
```

### Comparing `vnai-0.0.3/PKG-INFO` & `vnai-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.3
+Version: 0.0.4
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnai-0.0.3/raw/__init__.py` & `vnai-0.0.4/vnai/__init__.py`

 * *Files identical despite different names*

### Comparing `vnai-0.0.3/raw/analytics.py` & `vnai-0.0.4/raw/analytics.py`

 * *Files identical despite different names*

### Comparing `vnai-0.0.3/setup.cfg` & `vnai-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnai
-version = 0.0.3
+version = 0.0.4
 author = Vnstock HQ
 author_email = support@vnstock.site
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `vnai-0.0.3/vnai/__init__.py` & `vnai-0.0.4/raw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,18 @@
             from IPython import get_ipython
             if 'IPKernelApp' not in get_ipython().config:  # Check if not in IPython kernel
                 if sys.stdout.isatty():
                     environment = "Terminal"
                 else:
                     environment = "Other"  # Non-interactive environment (e.g., script executed from an IDE)
             else:
-                environment = "Jupyter"
+                if 'google.colab' in sys.modules:
+                    environment = "Google Colab"
+                else:
+                    environment = "Jupyter"
         except (ImportError, AttributeError):
             # Fallback if IPython isn't installed or other checks fail
             if sys.stdout.isatty():
                 environment = "Terminal"
             else:
                 environment = "Other"
```

### Comparing `vnai-0.0.3/vnai.egg-info/PKG-INFO` & `vnai-0.0.4/vnai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.3
+Version: 0.0.4
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

