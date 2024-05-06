# Comparing `tmp/composio_julep-0.2.47.tar.gz` & `tmp/composio_julep-0.2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.47.tar", last modified: Thu May  2 08:02:12 2024, max compression
+gzip compressed data, was "composio_julep-0.2.48.tar", last modified: Sun May  5 16:56:13 2024, max compression
```

## Comparing `composio_julep-0.2.47.tar` & `composio_julep-0.2.48.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:12.577844 composio_julep-0.2.47/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-02 08:02:12.577656 composio_julep-0.2.47/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3933 2024-05-02 07:58:37.000000 composio_julep-0.2.47/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:12.576279 composio_julep-0.2.47/composio_julep/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      157 2024-05-02 07:58:37.000000 composio_julep-0.2.47/composio_julep/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1619 2024-05-02 07:58:37.000000 composio_julep-0.2.47/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-02 08:02:12.577443 composio_julep-0.2.47/composio_julep.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-02 08:02:12.000000 composio_julep-0.2.47/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      267 2024-05-02 08:02:12.000000 composio_julep-0.2.47/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-02 08:02:12.000000 composio_julep-0.2.47/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-02 08:02:12.000000 composio_julep-0.2.47/composio_julep.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-05-02 08:02:12.000000 composio_julep-0.2.47/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-02 08:02:12.577883 composio_julep-0.2.47/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      842 2024-05-02 08:00:55.000000 composio_julep-0.2.47/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:13.997903 composio_julep-0.2.48/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     4463 2024-05-05 16:56:13.997673 composio_julep-0.2.48/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3933 2024-05-05 16:54:48.000000 composio_julep-0.2.48/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:13.996457 composio_julep-0.2.48/composio_julep/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      157 2024-05-05 16:54:48.000000 composio_julep-0.2.48/composio_julep/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1619 2024-05-05 16:54:48.000000 composio_julep-0.2.48/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-05 16:56:13.997439 composio_julep-0.2.48/composio_julep.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     4463 2024-05-05 16:56:13.000000 composio_julep-0.2.48/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      267 2024-05-05 16:56:13.000000 composio_julep-0.2.48/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-05 16:56:13.000000 composio_julep-0.2.48/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-05 16:56:13.000000 composio_julep-0.2.48/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       15 2024-05-05 16:56:13.000000 composio_julep-0.2.48/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-05 16:56:13.997954 composio_julep-0.2.48/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      842 2024-05-05 16:55:57.000000 composio_julep-0.2.48/setup.py
```

### Comparing `composio_julep-0.2.47/PKG-INFO` & `composio_julep-0.2.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.47
+Version: 0.2.48
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.47
+Requires-Dist: composio_openai===0.2.48
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.47/README.md` & `composio_julep-0.2.48/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.47/composio_julep/julep_toolspec.py` & `composio_julep-0.2.48/composio_julep/julep_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.47/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.48/composio_julep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.47
+Version: 0.2.48
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.47
+Requires-Dist: composio_openai===0.2.48
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.47/setup.py` & `composio_julep-0.2.48/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.47",
+    version="0.2.48",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
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
-        "composio_openai===0.2.47",
+        "composio_openai===0.2.48",
         "julep>=0.3.2"
     ],
     include_package_data=True,
 )
```

