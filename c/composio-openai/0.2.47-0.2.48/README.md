# Comparing `tmp/composio_openai-0.2.47.tar.gz` & `tmp/composio_openai-0.2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.47.tar", last modified: Thu May  2 08:02:36 2024, max compression
+gzip compressed data, was "composio_openai-0.2.48.tar", last modified: Sun May  5 16:56:24 2024, max compression
```

## Comparing `composio_openai-0.2.47.tar` & `composio_openai-0.2.48.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:36.586223 composio_openai-0.2.47/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2615 2024-05-02 08:02:36.585197 composio_openai-0.2.47/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2107 2024-05-02 07:58:37.000000 composio_openai-0.2.47/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:36.583275 composio_openai-0.2.47/composio_openai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      182 2024-05-02 07:58:37.000000 composio_openai-0.2.47/composio_openai/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2869 2024-05-02 07:58:37.000000 composio_openai-0.2.47/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:36.584282 composio_openai-0.2.47/composio_openai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2615 2024-05-02 08:02:36.000000 composio_openai-0.2.47/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-05-02 08:02:36.000000 composio_openai-0.2.47/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-02 08:02:36.000000 composio_openai-0.2.47/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       23 2024-05-02 08:02:36.000000 composio_openai-0.2.47/composio_openai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-05-02 08:02:36.000000 composio_openai-0.2.47/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-02 08:02:36.586351 composio_openai-0.2.47/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      826 2024-05-02 08:00:55.000000 composio_openai-0.2.47/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:24.958658 composio_openai-0.2.48/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-05 16:56:24.958439 composio_openai-0.2.48/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-05-05 16:54:48.000000 composio_openai-0.2.48/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:24.957108 composio_openai-0.2.48/composio_openai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      182 2024-05-05 16:54:48.000000 composio_openai-0.2.48/composio_openai/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2869 2024-05-05 16:54:48.000000 composio_openai-0.2.48/composio_openai/openai_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:24.958226 composio_openai-0.2.48/composio_openai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-05 16:56:24.000000 composio_openai-0.2.48/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      275 2024-05-05 16:56:24.000000 composio_openai-0.2.48/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-05 16:56:24.000000 composio_openai-0.2.48/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       23 2024-05-05 16:56:24.000000 composio_openai-0.2.48/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-05-05 16:56:24.000000 composio_openai-0.2.48/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-05 16:56:24.958701 composio_openai-0.2.48/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      826 2024-05-05 16:55:57.000000 composio_openai-0.2.48/setup.py
```

### Comparing `composio_openai-0.2.47/PKG-INFO` & `composio_openai-0.2.48/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.47
+Version: 0.2.48
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.47
+Requires-Dist: composio_core===0.2.48
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.47/README.md` & `composio_openai-0.2.48/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.47/composio_openai/openai_toolspec.py` & `composio_openai-0.2.48/composio_openai/openai_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.47/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.2.48/composio_openai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.47
+Version: 0.2.48
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.47
+Requires-Dist: composio_core===0.2.48
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.47/setup.py` & `composio_openai-0.2.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.2.47",
+    version="0.2.48",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_core===0.2.47",
+        "composio_core===0.2.48",
     ],
     include_package_data=True,
 )
```

