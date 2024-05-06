# Comparing `tmp/spleenseg-1.2.40.tar.gz` & `tmp/spleenseg-1.2.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleenseg-1.2.40.tar", last modified: Sat May  4 00:01:20 2024, max compression
+gzip compressed data, was "spleenseg-1.2.42.tar", last modified: Mon May  6 14:38:06 2024, max compression
```

## Comparing `spleenseg-1.2.40.tar` & `spleenseg-1.2.42.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.2.40/LICENSE
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10727 2024-05-04 00:01:20.610953 spleenseg-1.2.40/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8973 2024-05-02 02:07:10.000000 spleenseg-1.2.40/README.md
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9551 2024-05-04 00:01:18.000000 spleenseg-1.2.40/README.rst
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      238 2024-04-26 18:25:29.000000 spleenseg-1.2.40/requirements.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-05-04 00:01:20.610953 spleenseg-1.2.40/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1903 2024-04-30 22:21:09.000000 spleenseg-1.2.40/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.607620 spleenseg-1.2.40/spleenseg/
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg/comms/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4878 2024-04-30 22:32:17.000000 spleenseg-1.2.40/spleenseg/comms/rpc.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg/core/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    24201 2024-04-26 18:36:17.000000 spleenseg-1.2.40/spleenseg/core/neuralnet.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg/models/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3221 2024-04-26 18:36:17.000000 spleenseg-1.2.40/spleenseg/models/data.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg/plotting/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2113 2024-05-04 00:00:29.000000 spleenseg-1.2.40/spleenseg/plotting/plotting.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8826 2024-05-04 00:00:25.000000 spleenseg-1.2.40/spleenseg/spleenseg.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7133 2024-05-01 23:25:29.000000 spleenseg-1.2.40/spleenseg/splparser.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg/transforms/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7650 2024-04-24 22:01:17.000000 spleenseg-1.2.40/spleenseg/transforms/transforms.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-04 00:01:20.610953 spleenseg-1.2.40/spleenseg.egg-info/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10727 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      442 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      251 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       98 2024-05-04 00:01:20.000000 spleenseg-1.2.40/spleenseg.egg-info/top_level.txt
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.421744 spleenseg-1.2.42/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.2.42/LICENSE
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10727 2024-05-06 14:38:06.421744 spleenseg-1.2.42/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8973 2024-05-02 02:07:10.000000 spleenseg-1.2.42/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9551 2024-05-06 14:38:04.000000 spleenseg-1.2.42/README.rst
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      238 2024-04-26 18:25:29.000000 spleenseg-1.2.42/requirements.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-05-06 14:38:06.421744 spleenseg-1.2.42/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1903 2024-04-30 22:21:09.000000 spleenseg-1.2.42/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/comms/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4878 2024-04-30 22:32:17.000000 spleenseg-1.2.42/spleenseg/comms/rpc.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/core/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    24201 2024-04-26 18:36:17.000000 spleenseg-1.2.42/spleenseg/core/neuralnet.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/models/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3221 2024-04-26 18:36:17.000000 spleenseg-1.2.42/spleenseg/models/data.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/plotting/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2113 2024-05-04 00:00:29.000000 spleenseg-1.2.42/spleenseg/plotting/plotting.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8826 2024-05-06 14:37:29.000000 spleenseg-1.2.42/spleenseg/spleenseg.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7133 2024-05-01 23:25:29.000000 spleenseg-1.2.42/spleenseg/splparser.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg/transforms/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7650 2024-04-24 22:01:17.000000 spleenseg-1.2.42/spleenseg/transforms/transforms.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-06 14:38:06.418410 spleenseg-1.2.42/spleenseg.egg-info/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10727 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      442 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      251 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       98 2024-05-06 14:38:06.000000 spleenseg-1.2.42/spleenseg.egg-info/top_level.txt
```

### Comparing `spleenseg-1.2.40/LICENSE` & `spleenseg-1.2.42/LICENSE`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/PKG-INFO` & `spleenseg-1.2.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.2.40
+Version: 1.2.42
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `spleenseg-1.2.40/README.md` & `spleenseg-1.2.42/README.md`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/README.rst` & `spleenseg-1.2.42/README.rst`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/setup.py` & `spleenseg-1.2.42/setup.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/comms/rpc.py` & `spleenseg-1.2.42/spleenseg/comms/rpc.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/core/neuralnet.py` & `spleenseg-1.2.42/spleenseg/core/neuralnet.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/models/data.py` & `spleenseg-1.2.42/spleenseg/models/data.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/plotting/plotting.py` & `spleenseg-1.2.42/spleenseg/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/spleenseg.py` & `spleenseg-1.2.42/spleenseg/spleenseg.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ██╔════╝██╔══██╗██║     ██╔════╝██╔════╝████╗  ██║██╔════╝██╔════╝██╔════╝
 ███████╗██████╔╝██║     █████╗  █████╗  ██╔██╗ ██║███████╗█████╗  ██║  ███╗
 ╚════██║██╔═══╝ ██║     ██╔══╝  ██╔══╝  ██║╚██╗██║╚════██║██╔══╝  ██║   ██║
 ███████║██║     ███████╗███████╗███████╗██║ ╚████║███████║███████╗╚██████╔╝
 ╚══════╝╚═╝     ╚══════╝╚══════╝╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝ ╚═════╝
 """
 
-__version__ = "1.2.40"
+__version__ = "1.2.42"
 import spleenseg.splparser as spl
 
 description: str = """
 A ChRIS DS plugin based on Project MONAI 3D Spleen Segmentation.
 This plugin implements both training and inference, with some
 refactoring and pervasive type hinting.
 """
@@ -203,15 +203,15 @@
 
 
 @chris_plugin(
     parser=sparser,
     title="Spleen 3D image segmentation (MONAI)",
     category="",  # ref. https://chrisstore.co/plugins
     min_memory_limit="24Gi",  # supported units: Mi, Gi
-    min_cpu_limit="8000m",  # millicores, e.g. "1000m" = 1 CPU core
+    min_cpu_limit="2000m",  # millicores, e.g. "1000m" = 1 CPU core
     min_gpu_limit=1,  # set min_gpu_limit=1 to enable GPU
     max_gpu_limit=2,
 )
 def main(options: Namespace, inputdir: Path, outputdir: Path):
     """
     *ChRIS* plugins usually have two positional arguments: an **input directory** containing
     input files and an **output directory** where to write output files. Command-line arguments
```

### Comparing `spleenseg-1.2.40/spleenseg/splparser.py` & `spleenseg-1.2.42/spleenseg/splparser.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg/transforms/transforms.py` & `spleenseg-1.2.42/spleenseg/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.40/spleenseg.egg-info/PKG-INFO` & `spleenseg-1.2.42/spleenseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.2.40
+Version: 1.2.42
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

