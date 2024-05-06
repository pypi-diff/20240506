# Comparing `tmp/vital-ai-haley-taxonomy-0.1.3.tar.gz` & `tmp/vital-ai-haley-taxonomy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-haley-taxonomy-0.1.3.tar", last modified: Sat May  4 22:32:06 2024, max compression
+gzip compressed data, was "vital-ai-haley-taxonomy-0.1.4.tar", last modified: Mon May  6 21:53:32 2024, max compression
```

## Comparing `vital-ai-haley-taxonomy-0.1.3.tar` & `vital-ai-haley-taxonomy-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:32:06.856016 vital-ai-haley-taxonomy-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)      504 2024-05-04 22:32:06.855807 vital-ai-haley-taxonomy-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:54:08.000000 vital-ai-haley-taxonomy-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:32:06.851590 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:32:06.854036 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1793 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:32:06.854854 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/Property_hasDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/Property_hasExternalID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/Property_isLeafCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/Property_isRootCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/Property_isSelectable.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 22:32:06.856060 vital-ai-haley-taxonomy-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      929 2024-05-04 22:30:41.000000 vital-ai-haley-taxonomy-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:32:06.855569 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      504 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)     1569 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       92 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       22 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       34 2024-05-04 22:32:06.000000 vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:53:32.493593 vital-ai-haley-taxonomy-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)      504 2024-05-06 21:53:32.493340 vital-ai-haley-taxonomy-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:54:08.000000 vital-ai-haley-taxonomy-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:53:32.489054 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:53:32.491479 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1419 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1793 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:53:32.492315 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/Property_hasDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/Property_hasExternalID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/Property_isLeafCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/Property_isRootCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 22:21:50.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/Property_isSelectable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:53:32.493642 vital-ai-haley-taxonomy-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      929 2024-05-06 21:52:14.000000 vital-ai-haley-taxonomy-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:53:32.493062 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      504 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)     1569 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       92 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       22 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       34 2024-05-06 21:53:32.000000 vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/top_level.txt
```

### Comparing `vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.py` & `vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasBroaderCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.py` & `vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasEquivalentCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.py` & `vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasNarrowerCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.py` & `vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/Edge_hasRelatedCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-taxonomy-0.1.3/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.py` & `vital-ai-haley-taxonomy-0.1.4/com_vitalai_haley_taxonomy_domain/model/TaxonomyNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-taxonomy-0.1.3/setup.py` & `vital-ai-haley-taxonomy-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-haley-taxonomy',
-    version='0.1.3',
+    version='0.1.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns haley taxonomy domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-haley',
     packages=find_packages(),
@@ -16,15 +16,15 @@
         ]
     },
     package_data={
          '': ['*.pyi'],
     },
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-haley==0.1.3',
+            'vital-ai-haley>=0.1.4',
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

### Comparing `vital-ai-haley-taxonomy-0.1.3/vital_ai_haley_taxonomy.egg-info/SOURCES.txt` & `vital-ai-haley-taxonomy-0.1.4/vital_ai_haley_taxonomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

