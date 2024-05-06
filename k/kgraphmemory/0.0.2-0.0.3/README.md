# Comparing `tmp/kgraphmemory-0.0.2.tar.gz` & `tmp/kgraphmemory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphmemory-0.0.2.tar", last modified: Mon May  6 20:36:06 2024, max compression
+gzip compressed data, was "kgraphmemory-0.0.3.tar", last modified: Mon May  6 20:37:55 2024, max compression
```

## Comparing `kgraphmemory-0.0.2.tar` & `kgraphmemory-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322675 kgraphmemory-0.0.2/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.2/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:36:06.322483 kgraphmemory-0.0.2/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.2/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.320571 kgraphmemory-0.0.2/kgraphmemory/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.2/kgraphmemory/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.321601 kgraphmemory-0.0.2/kgraphmemory/entitymodel/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 16:38:02.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 16:38:31.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/entitymodel.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2844 2024-05-01 16:50:59.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/spacy_en_core_web_model.py
--rw-r--r--   0 hadfield   (501) staff       (20)    13263 2024-05-05 23:20:01.000000 kgraphmemory-0.0.2/kgraphmemory/kginteraction_graph.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-05 01:39:33.000000 kgraphmemory-0.0.2/kgraphmemory/kgraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)     3283 2024-05-05 19:08:16.000000 kgraphmemory-0.0.2/kgraphmemory/kgraph_memory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      402 2024-05-05 21:09:58.000000 kgraphmemory-0.0.2/kgraphmemory/kgresult_list.py
--rw-r--r--   0 hadfield   (501) staff       (20)      858 2024-05-05 20:50:12.000000 kgraphmemory-0.0.2/kgraphmemory/kgresult_match.py
--rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-05 19:53:28.000000 kgraphmemory-0.0.2/kgraphmemory/kgstatus.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.321852 kgraphmemory-0.0.2/kgraphmemory/utils/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-05 02:58:49.000000 kgraphmemory-0.0.2/kgraphmemory/utils/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      288 2024-05-05 03:06:01.000000 kgraphmemory-0.0.2/kgraphmemory/utils/uri_generator.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322260 kgraphmemory-0.0.2/kgraphmemory.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      659 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 20:36:06.322714 kgraphmemory-0.0.2/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      906 2024-05-06 13:31:04.000000 kgraphmemory-0.0.2/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322085 kgraphmemory-0.0.2/test/
--rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 22:59:09.000000 kgraphmemory-0.0.2/test/test_domain_objects.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 23:04:55.000000 kgraphmemory-0.0.2/test/test_graph_collection.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.422319 kgraphmemory-0.0.3/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.3/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:37:55.422099 kgraphmemory-0.0.3/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.3/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.420419 kgraphmemory-0.0.3/kgraphmemory/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.3/kgraphmemory/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.421293 kgraphmemory-0.0.3/kgraphmemory/entitymodel/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 16:38:02.000000 kgraphmemory-0.0.3/kgraphmemory/entitymodel/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 16:38:31.000000 kgraphmemory-0.0.3/kgraphmemory/entitymodel/entitymodel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2844 2024-05-01 16:50:59.000000 kgraphmemory-0.0.3/kgraphmemory/entitymodel/spacy_en_core_web_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    13263 2024-05-05 23:20:01.000000 kgraphmemory-0.0.3/kgraphmemory/kginteraction_graph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-05 01:39:33.000000 kgraphmemory-0.0.3/kgraphmemory/kgraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     3283 2024-05-05 19:08:16.000000 kgraphmemory-0.0.3/kgraphmemory/kgraph_memory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      402 2024-05-05 21:09:58.000000 kgraphmemory-0.0.3/kgraphmemory/kgresult_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      858 2024-05-05 20:50:12.000000 kgraphmemory-0.0.3/kgraphmemory/kgresult_match.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-05 19:53:28.000000 kgraphmemory-0.0.3/kgraphmemory/kgstatus.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.421487 kgraphmemory-0.0.3/kgraphmemory/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-05 02:58:49.000000 kgraphmemory-0.0.3/kgraphmemory/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      288 2024-05-05 03:06:01.000000 kgraphmemory-0.0.3/kgraphmemory/utils/uri_generator.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.420965 kgraphmemory-0.0.3/kgraphmemory.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:37:55.000000 kgraphmemory-0.0.3/kgraphmemory.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      659 2024-05-06 20:37:55.000000 kgraphmemory-0.0.3/kgraphmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 20:37:55.000000 kgraphmemory-0.0.3/kgraphmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-06 20:37:55.000000 kgraphmemory-0.0.3/kgraphmemory.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-06 20:37:55.000000 kgraphmemory-0.0.3/kgraphmemory.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 20:37:55.422358 kgraphmemory-0.0.3/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      906 2024-05-06 20:37:26.000000 kgraphmemory-0.0.3/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:37:55.421686 kgraphmemory-0.0.3/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 22:59:09.000000 kgraphmemory-0.0.3/test/test_domain_objects.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 23:04:55.000000 kgraphmemory-0.0.3/test/test_graph_collection.py
```

### Comparing `kgraphmemory-0.0.2/LICENSE` & `kgraphmemory-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/PKG-INFO` & `kgraphmemory-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgraphmemory
-Version: 0.0.2
+Version: 0.0.3
 Summary: KGraph Memory
 Home-page: https://github.com/vital-ai/kgraphmemory
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kgraphmemory-0.0.2/kgraphmemory/entitymodel/spacy_en_core_web_model.py` & `kgraphmemory-0.0.3/kgraphmemory/entitymodel/spacy_en_core_web_model.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/kgraphmemory/kginteraction_graph.py` & `kgraphmemory-0.0.3/kgraphmemory/kginteraction_graph.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/kgraphmemory/kgraph_memory.py` & `kgraphmemory-0.0.3/kgraphmemory/kgraph_memory.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/kgraphmemory/kgresult_match.py` & `kgraphmemory-0.0.3/kgraphmemory/kgresult_match.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/kgraphmemory.egg-info/PKG-INFO` & `kgraphmemory-0.0.3/kgraphmemory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgraphmemory
-Version: 0.0.2
+Version: 0.0.3
 Summary: KGraph Memory
 Home-page: https://github.com/vital-ai/kgraphmemory
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `kgraphmemory-0.0.2/kgraphmemory.egg-info/SOURCES.txt` & `kgraphmemory-0.0.3/kgraphmemory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.2/setup.py` & `kgraphmemory-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphmemory',
-    version='0.0.2',
+    version='0.0.3',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Memory',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphmemory',
     packages=find_packages(exclude=["test"]),
```

### Comparing `kgraphmemory-0.0.2/test/test_graph_collection.py` & `kgraphmemory-0.0.3/test/test_graph_collection.py`

 * *Files identical despite different names*

