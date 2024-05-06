# Comparing `tmp/AdroitFisherman-0.0.25.tar.gz` & `tmp/AdroitFisherman-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.25.tar", last modified: Sat May  4 05:59:24 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.26.tar", last modified: Mon May  6 13:15:33 2024, max compression
```

## Comparing `AdroitFisherman-0.0.25.tar` & `AdroitFisherman-0.0.26.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.310963 AdroitFisherman-0.0.25/
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.295006 AdroitFisherman-0.0.25/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.305977 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/
--rw-rw-rw-   0        0        0      701 2024-04-29 14:10:00.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SequentialList.py
--rw-rw-rw-   0        0        0      843 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedList.py
--rw-rw-rw-   0        0        0      882 2024-05-04 05:30:33.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
--rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.306974 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/
--rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
--rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.25/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.307971 AdroitFisherman-0.0.25/AdroitFisherman/__pycache__/
--rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.25/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.310963 AdroitFisherman-0.0.25/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5147 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.h
--rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.c
--rw-rw-rw-   0        0        0     8093 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.h
--rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
--rw-rw-rw-   0        0        0     9086 2024-05-04 05:59:20.000000 AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
-drwxrwxrwx   0        0        0        0 2024-05-04 05:59:24.300990 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     3192 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-04 05:59:24.000000 AdroitFisherman-0.0.25/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.25/MANIFEST.in
--rw-rw-rw-   0        0        0     3192 2024-05-04 05:59:24.311961 AdroitFisherman-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.25/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 05:59:24.312958 AdroitFisherman-0.0.25/setup.cfg
--rw-rw-rw-   0        0        0     1472 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.124081 AdroitFisherman-0.0.26/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.102141 AdroitFisherman-0.0.26/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.117099 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0      937 2024-05-06 10:26:31.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/CircularSingleLinkedList.py
+-rw-rw-rw-   0        0        0      763 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0      903 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0      942 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.119093 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
+-rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.26/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.120091 AdroitFisherman-0.0.26/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.26/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.123082 AdroitFisherman-0.0.26/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.c
+-rw-rw-rw-   0        0        0     8255 2024-05-06 13:15:10.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.h
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5147 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8093 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.h
+-rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+-rw-rw-rw-   0        0        0     9086 2024-05-04 05:59:20.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
+drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.108125 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     3192 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     3192 2024-05-06 13:15:33.124081 AdroitFisherman-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.26/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:15:33.126076 AdroitFisherman-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     1641 2024-05-06 10:23:43.000000 AdroitFisherman-0.0.26/setup.py
```

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SequentialList.py` & `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SequentialList.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,7 +22,10 @@
         return self.__list.get_elem(index)
 
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
+
+    def __del__(self):
+        self.__list.destroy_list()
```

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedList.py` & `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedList.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,7 +28,10 @@
         return self.__list.add_after(elem)
 
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
+
+    def __del__(self):
+        self.__list.destroy_list()
```

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py` & `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,7 +28,10 @@
         return self.__list.add_after(elem)
 
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
+
+    def __del__(self):
+        self.__list.destroy_list()
```

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc` & `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.c` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedList.h` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h` & `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.26/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.25
+Version: 0.0.26
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.25/PKG-INFO` & `AdroitFisherman-0.0.26/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.25
+Version: 0.0.26
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.25/README.md` & `AdroitFisherman-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.25/setup.py` & `AdroitFisherman-0.0.26/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup,Extension
 SeqList=Extension("AdroitFisherman.SequentialList",sources=['AdroitFisherman/includes/SeqList.c'])
 SingleLinkedList=Extension("AdroitFisherman.SingleLinkedList",sources=['AdroitFisherman/includes/SingleLinkedList.c'])
 SingleLinkedListWithoutHeadNode=Extension("AdroitFisherman.SingleLinkedListWithoutHeadNode",sources=['AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c'])
+CircularSingleLinkedList=Extension("AdroitFisherman.CircularSingleLinkedList",sources=['AdroitFisherman/includes/CircularSingleLinkedList.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.25",
+    version="0.0.26",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
@@ -21,10 +22,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Topic :: Utilities"
     ],
     include_package_data=True,
     packages=['AdroitFisherman.Utilities'],
-    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode]
+    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode,CircularSingleLinkedList]
 )
 read_me.close()
```

