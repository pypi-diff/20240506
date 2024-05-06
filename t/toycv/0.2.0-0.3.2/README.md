# Comparing `tmp/toycv-0.2.0.tar.gz` & `tmp/toycv-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toycv-0.2.0.tar", last modified: Sun Mar 24 19:34:23 2024, max compression
+gzip compressed data, was "toycv-0.3.2.tar", last modified: Mon May  6 15:27:24 2024, max compression
```

## Comparing `toycv-0.2.0.tar` & `toycv-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.168221 toycv-0.2.0/
--rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.2.0/LICENSE
--rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.2.0/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-03-24 19:34:23.168083 toycv-0.2.0/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.2.0/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)      106 2024-03-24 19:34:17.000000 toycv-0.2.0/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-03-24 19:34:23.168264 toycv-0.2.0/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1961 2024-03-24 19:34:04.000000 toycv-0.2.0/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.166821 toycv-0.2.0/toycv/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.2.0/toycv/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      796 2024-03-17 20:17:39.000000 toycv-0.2.0/toycv/common.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.167683 toycv-0.2.0/toycv/file/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.2.0/toycv/file/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     7541 2024-03-17 21:34:58.000000 toycv-0.2.0/toycv/file/image.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1858 2024-03-17 21:35:16.000000 toycv-0.2.0/toycv/file/path.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.167786 toycv-0.2.0/toycv/pytorch/
--rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.2.0/toycv/pytorch/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.167895 toycv-0.2.0/toycv/visualization/
--rw-r--r--   0 xiangyang   (501) staff       (20)     7791 2024-03-17 19:08:25.000000 toycv-0.2.0/toycv/visualization/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-03-24 19:34:23.167375 toycv-0.2.0/toycv.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-03-24 19:34:23.000000 toycv-0.2.0/toycv.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      353 2024-03-24 19:34:23.000000 toycv-0.2.0/toycv.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-03-24 19:34:23.000000 toycv-0.2.0/toycv.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)      106 2024-03-24 19:34:23.000000 toycv-0.2.0/toycv.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-03-24 19:34:23.000000 toycv-0.2.0/toycv.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868742 toycv-0.3.2/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.3.2/LICENSE
+-rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.3.2/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-06 15:27:24.868549 toycv-0.3.2/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.3.2/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-06 15:27:22.000000 toycv-0.3.2/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-05-06 15:27:24.868795 toycv-0.3.2/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1958 2024-05-06 15:27:10.000000 toycv-0.3.2/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.866951 toycv-0.3.2/toycv/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.3.2/toycv/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     8409 2024-05-06 06:23:06.000000 toycv-0.3.2/toycv/common.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.867736 toycv-0.3.2/toycv/file/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.3.2/toycv/file/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)    12851 2024-05-06 06:24:19.000000 toycv-0.3.2/toycv/file/image.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1873 2024-04-09 03:48:43.000000 toycv-0.3.2/toycv/file/path.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      300 2024-04-26 09:56:43.000000 toycv-0.3.2/toycv/metrics.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868171 toycv-0.3.2/toycv/pytorch/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.3.2/toycv/pytorch/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      417 2024-05-06 14:41:56.000000 toycv-0.3.2/toycv/pytorch/datasets.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2686 2024-05-06 14:44:19.000000 toycv-0.3.2/toycv/pytorch/transform.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      502 2024-04-26 08:43:20.000000 toycv-0.3.2/toycv/string.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868315 toycv-0.3.2/toycv/visualization/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     7792 2024-05-06 07:31:32.000000 toycv-0.3.2/toycv/visualization/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.867446 toycv-0.3.2/toycv.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      439 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/top_level.txt
```

### Comparing `toycv-0.2.0/LICENSE` & `toycv-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toycv-0.2.0/PKG-INFO` & `toycv-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.2.0
+Version: 0.3.2
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

### Comparing `toycv-0.2.0/setup.py` & `toycv-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='toycv',  # 包名
     python_requires='>=3.8.0',  # python环境
-    version='0.2.0',  # 包的版本
+    version='0.3.2',  # 包的版本
     description="A simple and flexible tool for building and training neural network models.",  # 包简介，显示在PyPI上
 
     long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
     long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
     # 作者相关信息
     author="Yang Xiang",
@@ -49,9 +49,9 @@
 pipreqs ./ --encoding=utf8 --force --mode no-pin
 python3 setup.py sdist 
 twine upload --repository testpypi dist/*
 pip install -i https://test.pypi.org/simple/ -U toycv
 
 twine upload --repository pypi dist/*
 
-pip install -e .
+pip install .
 """
```

### Comparing `toycv-0.2.0/toycv/file/path.py` & `toycv-0.3.2/toycv/file/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 import queue
 import re
 
 
-def ensure_dirs(file_path, file_has_suffix=True):
+def ensure_dirs(file_path: str, file_has_suffix: str = True) -> str:
     if file_has_suffix and "." in os.path.basename(file_path):
         directory = os.path.dirname(file_path)
     else:
         directory = file_path
 
     directory = os.path.abspath(directory)
 
@@ -18,15 +18,15 @@
     return file_path
 
 
 def home_path():
     return os.path.expanduser('~')
 
 
-def dir_and_file_ext(file_path):
+def dir_file_ext(file_path):
     return os.path.dirname(file_path), os.path.basename(file_path), os.path.splitext(file_path)[1]
 
 
 def glob_re(root_dir, path_re="**"):
     """
     Match file paths based on regular expressions.
```

### Comparing `toycv-0.2.0/toycv/pytorch/__init__.py` & `toycv-0.3.2/toycv/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `toycv-0.2.0/toycv/visualization/__init__.py` & `toycv-0.3.2/toycv/visualization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         image.seek(0)
         image = Image.open(image)
 
         return numpy.array(image)
 
 
-def show_images(images: List[numpy.array], subtitles=None, col_num: int = 3, title: str = None,
+def show_images(*images: List[numpy.array], subtitles=None, col_num: int = 3, title: str = None,
                 each_size=(8, 7), show: bool = True, save_path: str = None):
     """
     Display or save a collection of images with optional subtitles.
 
     :param images: List of images to be displayed or saved.
     :param subtitles: List of subtitles for the images. If the number of subtitles is less than the number of images, None will be appended to the subtitles list.
     :param col_num: Number of columns for the image grid. Default is 3.
```

### Comparing `toycv-0.2.0/toycv.egg-info/PKG-INFO` & `toycv-0.3.2/toycv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.2.0
+Version: 0.3.2
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

