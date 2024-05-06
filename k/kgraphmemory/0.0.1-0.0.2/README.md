# Comparing `tmp/kgraphmemory-0.0.1.tar.gz` & `tmp/kgraphmemory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphmemory-0.0.1.tar", last modified: Wed May  1 12:34:20 2024, max compression
+gzip compressed data, was "kgraphmemory-0.0.2.tar", last modified: Mon May  6 20:36:06 2024, max compression
```

## Comparing `kgraphmemory-0.0.1.tar` & `kgraphmemory-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-01 12:34:20.827424 kgraphmemory-0.0.1/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.1/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      548 2024-05-01 12:34:20.827234 kgraphmemory-0.0.1/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.1/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-01 12:34:20.826460 kgraphmemory-0.0.1/kgraphmemory/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.1/kgraphmemory/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-01 12:29:33.000000 kgraphmemory-0.0.1/kgraphmemory/kgraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 12:30:18.000000 kgraphmemory-0.0.1/kgraphmemory/kgraph_memory.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-01 12:34:20.827038 kgraphmemory-0.0.1/kgraphmemory.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      548 2024-05-01 12:34:20.000000 kgraphmemory-0.0.1/kgraphmemory.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      283 2024-05-01 12:34:20.000000 kgraphmemory-0.0.1/kgraphmemory.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-01 12:34:20.000000 kgraphmemory-0.0.1/kgraphmemory.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       31 2024-05-01 12:34:20.000000 kgraphmemory-0.0.1/kgraphmemory.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-01 12:34:20.000000 kgraphmemory-0.0.1/kgraphmemory.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-01 12:34:20.827462 kgraphmemory-0.0.1/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      730 2024-05-01 12:26:54.000000 kgraphmemory-0.0.1/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322675 kgraphmemory-0.0.2/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.2/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:36:06.322483 kgraphmemory-0.0.2/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.2/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.320571 kgraphmemory-0.0.2/kgraphmemory/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.2/kgraphmemory/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.321601 kgraphmemory-0.0.2/kgraphmemory/entitymodel/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 16:38:02.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 16:38:31.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/entitymodel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2844 2024-05-01 16:50:59.000000 kgraphmemory-0.0.2/kgraphmemory/entitymodel/spacy_en_core_web_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    13263 2024-05-05 23:20:01.000000 kgraphmemory-0.0.2/kgraphmemory/kginteraction_graph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-05 01:39:33.000000 kgraphmemory-0.0.2/kgraphmemory/kgraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     3283 2024-05-05 19:08:16.000000 kgraphmemory-0.0.2/kgraphmemory/kgraph_memory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      402 2024-05-05 21:09:58.000000 kgraphmemory-0.0.2/kgraphmemory/kgresult_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      858 2024-05-05 20:50:12.000000 kgraphmemory-0.0.2/kgraphmemory/kgresult_match.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-05 19:53:28.000000 kgraphmemory-0.0.2/kgraphmemory/kgstatus.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.321852 kgraphmemory-0.0.2/kgraphmemory/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-05 02:58:49.000000 kgraphmemory-0.0.2/kgraphmemory/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      288 2024-05-05 03:06:01.000000 kgraphmemory-0.0.2/kgraphmemory/utils/uri_generator.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322260 kgraphmemory-0.0.2/kgraphmemory.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      710 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      659 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-06 20:36:06.000000 kgraphmemory-0.0.2/kgraphmemory.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 20:36:06.322714 kgraphmemory-0.0.2/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      906 2024-05-06 13:31:04.000000 kgraphmemory-0.0.2/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 20:36:06.322085 kgraphmemory-0.0.2/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 22:59:09.000000 kgraphmemory-0.0.2/test/test_domain_objects.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 23:04:55.000000 kgraphmemory-0.0.2/test/test_graph_collection.py
```

### Comparing `kgraphmemory-0.0.1/LICENSE` & `kgraphmemory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.1/setup.py` & `kgraphmemory-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphmemory',
-    version='0.0.1',
+    version='0.0.2',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Memory',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphmemory',
-    packages=find_packages(),
+    packages=find_packages(exclude=["test"]),
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns',
+            'vital-ai-vitalsigns==0.1.3',
             'six',
-            'pyyaml'
-        ],
+            'pyyaml',
+            'vital-ai-haley-kg==0.1.3',
+            'rdflib==7.0.0',
+            'SPARQLWrapper==2.0.0',
+            'networkx',
+            'matplotlib',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
-)
+)
```

