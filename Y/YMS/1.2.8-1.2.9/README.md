# Comparing `tmp/YMS-1.2.8.tar.gz` & `tmp/YMS-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-1.2.8.tar", last modified: Mon May  6 10:18:26 2024, max compression
+gzip compressed data, was "YMS-1.2.9.tar", last modified: Mon May  6 10:31:56 2024, max compression
```

## Comparing `YMS-1.2.8.tar` & `YMS-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.774043 YMS-1.2.8/
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:18:26.774043 YMS-1.2.8/PKG-INFO
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5359 2024-02-19 11:08:39.000000 YMS-1.2.8/README.md
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.770043 YMS-1.2.8/YMS.egg-info/
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)      399 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        1 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       15 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/requires.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        6 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/top_level.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:18:26.774043 YMS-1.2.8/setup.cfg
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)      734 2024-05-06 10:17:39.000000 YMS-1.2.8/setup.py
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.774043 YMS-1.2.8/yamas/
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     6420 2024-03-07 12:02:41.000000 YMS-1.2.8/yamas/__init__.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)       30 2023-10-30 09:49:55.000000 YMS-1.2.8/yamas/config.json
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    20526 2024-02-19 10:15:25.000000 YMS-1.2.8/yamas/create_visualization.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     2633 2024-03-07 12:06:45.000000 YMS-1.2.8/yamas/dataset_downloading.py
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    14620 2024-02-19 10:27:35.000000 YMS-1.2.8/yamas/export_data.py
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     6455 2024-03-07 12:34:34.000000 YMS-1.2.8/yamas/fastq_visualization.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1900 2023-11-14 07:32:14.000000 YMS-1.2.8/yamas/prerun_configs.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)    10075 2024-05-06 10:16:15.000000 YMS-1.2.8/yamas/qiita_visualization.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1183 2023-10-30 09:49:55.000000 YMS-1.2.8/yamas/utilities.py
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:31:56.506023 YMS-1.2.9/
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:31:56.506023 YMS-1.2.9/PKG-INFO
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5359 2024-02-19 11:08:39.000000 YMS-1.2.9/README.md
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:31:56.506023 YMS-1.2.9/YMS.egg-info/
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)      399 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        1 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       15 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/requires.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        6 2024-05-06 10:31:56.000000 YMS-1.2.9/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:31:56.506023 YMS-1.2.9/setup.cfg
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)      734 2024-05-06 10:31:28.000000 YMS-1.2.9/setup.py
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:31:56.506023 YMS-1.2.9/yamas/
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     6420 2024-03-07 12:02:41.000000 YMS-1.2.9/yamas/__init__.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)       30 2023-10-30 09:49:55.000000 YMS-1.2.9/yamas/config.json
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    20526 2024-02-19 10:15:25.000000 YMS-1.2.9/yamas/create_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     2633 2024-03-07 12:06:45.000000 YMS-1.2.9/yamas/dataset_downloading.py
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    14620 2024-02-19 10:27:35.000000 YMS-1.2.9/yamas/export_data.py
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     6455 2024-03-07 12:34:34.000000 YMS-1.2.9/yamas/fastq_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1900 2023-11-14 07:32:14.000000 YMS-1.2.9/yamas/prerun_configs.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)    10075 2024-05-06 10:16:15.000000 YMS-1.2.9/yamas/qiita_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1181 2024-05-06 10:31:28.000000 YMS-1.2.9/yamas/utilities.py
```

### Comparing `YMS-1.2.8/PKG-INFO` & `YMS-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YMS
-Version: 1.2.8
+Version: 1.2.9
 Summary: YOLO Microbiome Analysis System
 Home-page: UNKNOWN
 Author: Yarin Bekor, Shani Finkelstein
 Author-email: yarin.bekor@gmail.com, shaninn123@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `YMS-1.2.8/README.md` & `YMS-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/YMS.egg-info/PKG-INFO` & `YMS-1.2.9/YMS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YMS
-Version: 1.2.8
+Version: 1.2.9
 Summary: YOLO Microbiome Analysis System
 Home-page: UNKNOWN
 Author: Yarin Bekor, Shani Finkelstein
 Author-email: yarin.bekor@gmail.com, shaninn123@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `YMS-1.2.8/setup.py` & `YMS-1.2.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="YMS",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.2.8",
+    version="1.2.9",
     author="Yarin Bekor, Shani Finkelstein",
     author_email="yarin.bekor@gmail.com, shaninn123@gmail.com",
     description="YOLO Microbiome Analysis System",
     license='MIT',
     entry_points={
         'console_scripts': [
             'yamas = yamas:main',
```

### Comparing `YMS-1.2.8/yamas/__init__.py` & `YMS-1.2.9/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/create_visualization.py` & `YMS-1.2.9/yamas/create_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/dataset_downloading.py` & `YMS-1.2.9/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/export_data.py` & `YMS-1.2.9/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/fastq_visualization.py` & `YMS-1.2.9/yamas/fastq_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/prerun_configs.py` & `YMS-1.2.9/yamas/prerun_configs.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/qiita_visualization.py` & `YMS-1.2.9/yamas/qiita_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.8/yamas/utilities.py` & `YMS-1.2.9/yamas/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 @dataclass(frozen=True)
 class ReadsData:
     dir_path: str
     fwd: bool = True
     rev: bool = False
 
-
 def run_cmd(command: list):
     os.system(" ".join(command))
 
 
 def qiime2_version():
     o, e = run_cmd(["conda", "env", "list"])
     qiime_version = ""
```

