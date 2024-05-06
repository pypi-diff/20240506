# Comparing `tmp/vnai-0.0.5.tar.gz` & `tmp/vnai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnai-0.0.5.tar", last modified: Mon May  6 16:10:47 2024, max compression
+gzip compressed data, was "vnai-0.0.6.tar", last modified: Mon May  6 17:06:30 2024, max compression
```

## Comparing `vnai-0.0.5.tar` & `vnai-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:10:47.759779 vnai-0.0.5/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 16:10:47.759667 vnai-0.0.5/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.5/pyproject.toml
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:10:47.757859 vnai-0.0.5/raw/
--rw-r--r--   0 mrthinh    (501) staff       (20)    14715 2024-05-06 16:04:41.000000 vnai-0.0.5/raw/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    14534 2024-04-28 17:10:37.000000 vnai-0.0.5/raw/analytics.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      204 2024-04-26 15:44:24.000000 vnai-0.0.5/raw/setup.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 16:10:47.760038 vnai-0.0.5/setup.cfg
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:10:47.758303 vnai-0.0.5/vnai/
--rw-r--r--   0 mrthinh    (501) staff       (20)    14715 2024-05-06 16:10:02.000000 vnai-0.0.5/vnai/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 16:10:47.759295 vnai-0.0.5/vnai.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 16:10:47.000000 vnai-0.0.5/vnai.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      226 2024-05-06 16:10:47.000000 vnai-0.0.5/vnai.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-06 16:10:47.000000 vnai-0.0.5/vnai.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-06 16:10:47.000000 vnai-0.0.5/vnai.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        9 2024-05-06 16:10:47.000000 vnai-0.0.5/vnai.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:06:30.594173 vnai-0.0.6/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 17:06:30.594092 vnai-0.0.6/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.6/pyproject.toml
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:06:30.592618 vnai-0.0.6/raw/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14715 2024-05-06 16:04:41.000000 vnai-0.0.6/raw/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14534 2024-04-28 17:10:37.000000 vnai-0.0.6/raw/analytics.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      204 2024-04-26 15:44:24.000000 vnai-0.0.6/raw/setup.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 17:06:30.594490 vnai-0.0.6/setup.cfg
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:06:30.592757 vnai-0.0.6/vnai/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    15323 2024-05-06 17:04:56.000000 vnai-0.0.6/vnai/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:06:30.593703 vnai-0.0.6/vnai.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 17:06:30.000000 vnai-0.0.6/vnai.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      226 2024-05-06 17:06:30.000000 vnai-0.0.6/vnai.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-06 17:06:30.000000 vnai-0.0.6/vnai.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-06 17:06:30.000000 vnai-0.0.6/vnai.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        9 2024-05-06 17:06:30.000000 vnai-0.0.6/vnai.egg-info/top_level.txt
```

### Comparing `vnai-0.0.5/PKG-INFO` & `vnai-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.5
+Version: 0.0.6
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnai-0.0.5/raw/__init__.py` & `vnai-0.0.6/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `vnai-0.0.5/raw/analytics.py` & `vnai-0.0.6/raw/analytics.py`

 * *Files identical despite different names*

### Comparing `vnai-0.0.5/setup.cfg` & `vnai-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnai
-version = 0.0.5
+version = 0.0.6
 author = Vnstock HQ
 author_email = support@vnstock.site
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `vnai-0.0.5/vnai/__init__.py` & `vnai-0.0.6/vnai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,25 +99,38 @@
             from IPython import get_ipython
             if 'IPKernelApp' not in get_ipython().config:  # Check if not in IPython kernel
                 if sys.stdout.isatty():
                     environment = "Terminal"
                 else:
                     environment = "Other"  # Non-interactive environment (e.g., script executed from an IDE)
             else:
-                if 'google.colab' in sys.modules:
-                    environment = "Google Colab"
-                else:
-                    environment = "Jupyter"
+                environment = "Jupyter"
         except (ImportError, AttributeError):
             # Fallback if IPython isn't installed or other checks fail
             if sys.stdout.isatty():
                 environment = "Terminal"
             else:
                 environment = "Other"
 
+        try:
+            if 'google.colab' in sys.modules:
+                hosting_service = "Google Colab"
+            elif 'CODESPACE_NAME' in os.environ:
+                hosting_service = "Github Codespace"
+            elif 'GITPOD_WORKSPACE_CLUSTER_HOST' in os.environ:
+                hosting_service = "Gitpod"
+            elif 'REPLIT_USER' in os.environ:
+                hosting_service = "Replit"
+            elif 'KAGGLE_CONTAINER_NAME' in os.environ:
+                hosting_service = "Kaggle"
+            elif '.hf.space' in os.environ['SPACE_HOST']:
+                hosting_service = "Hugging Face Spaces"
+        except:
+            hosting_service = "Local or Unknown"
+
         # System information
         os_info = platform.uname()
 
         # CPU information
         cpu_arch = platform.processor()  
         cpu_logical_cores = psutil.cpu_count(logical=True)
         cpu_cores = psutil.cpu_count(logical=False)
@@ -131,14 +144,15 @@
 
         mac = ':'.join(['{:02x}'.format((uuid.getnode() >> elements) & 0xff) for elements in range(0, 2 * 6, 2)])
 
         # Combine information into a dictionary
         info = {
             "uuid": machine_id,
             "environment": environment,
+            "hosting_service": hosting_service,
             "python_version": platform.python_version(),
             "os_name": os_info.system,
             "os_version": os_info.version,
             "machine": os_info.machine,
             "cpu_model": cpu_arch,
             "cpu_cores": cpu_cores,
             "cpu_logical_cores": cpu_logical_cores,
```

### Comparing `vnai-0.0.5/vnai.egg-info/PKG-INFO` & `vnai-0.0.6/vnai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.5
+Version: 0.0.6
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

