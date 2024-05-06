# Comparing `tmp/algophon-0.0.8.tar.gz` & `tmp/algophon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.8.tar", last modified: Wed Apr 24 23:35:16 2024, max compression
+gzip compressed data, was "algophon-0.0.9.tar", last modified: Mon May  6 15:46:32 2024, max compression
```

## Comparing `algophon-0.0.8.tar` & `algophon-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.081493 algophon-0.0.8/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.8/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-24 23:35:16.080694 algophon-0.0.8/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.8/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.066433 algophon-0.0.8/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.8/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.074730 algophon-0.0.8/algophon/dist/
--rw-r--r--   0 u6052607   (503) staff       (20)     4045 2024-04-19 14:52:46.000000 algophon-0.0.8/algophon/dist/edit_distance.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.075919 algophon-0.0.8/algophon/ipa/
--rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.8/algophon/ipa/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1347 2024-04-19 14:16:56.000000 algophon-0.0.8/algophon/ipa/convert.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.8/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.8/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.8/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5834 2024-04-24 23:33:05.000000 algophon-0.0.8/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-04-24 23:29:56.000000 algophon-0.0.8/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.8/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.080019 algophon-0.0.8/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      472 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-24 23:35:16.000000 algophon-0.0.8/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-24 23:34:44.000000 algophon-0.0.8/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-24 23:35:16.081566 algophon-0.0.8/setup.cfg
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-24 23:35:16.079156 algophon-0.0.8/tests/
--rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.8/tests/test_natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.8/tests/test_seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     2746 2024-04-24 23:34:28.000000 algophon-0.0.8/tests/test_seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.0.8/tests/test_segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.8/tests/tester.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.514066 algophon-0.0.9/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.9/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     9638 2024-05-06 15:46:32.513321 algophon-0.0.9/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.9/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.473955 algophon-0.0.9/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      245 2024-05-05 22:24:11.000000 algophon-0.0.9/algophon/__init__.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.487633 algophon-0.0.9/algophon/distance/
+-rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-05 22:11:24.000000 algophon-0.0.9/algophon/distance/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5222 2024-05-06 15:22:54.000000 algophon-0.0.9/algophon/distance/edit_distance.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.493350 algophon-0.0.9/algophon/ipa/
+-rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.9/algophon/ipa/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3081 2024-05-03 14:26:54.000000 algophon-0.0.9/algophon/ipa/convert.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350576 2024-04-25 00:16:18.000000 algophon-0.0.9/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.9/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.9/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5850 2024-04-25 00:03:43.000000 algophon-0.0.9/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-05-06 15:42:02.000000 algophon-0.0.9/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      178 2024-04-25 00:14:05.000000 algophon-0.0.9/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.512549 algophon-0.0.9/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     9638 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      560 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)       12 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/requires.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-05-06 15:46:32.000000 algophon-0.0.9/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      829 2024-05-06 15:45:42.000000 algophon-0.0.9/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-05-06 15:46:32.514159 algophon-0.0.9/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-06 15:46:32.511666 algophon-0.0.9/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)     1240 2024-05-05 22:45:04.000000 algophon-0.0.9/tests/test_distance.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.9/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.9/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2746 2024-04-24 23:34:28.000000 algophon-0.0.9/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.0.9/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      884 2024-05-05 22:29:23.000000 algophon-0.0.9/tests/tester.py
```

### Comparing `algophon-0.0.8/LICENSE` & `algophon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/PKG-INFO` & `algophon-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.24
 
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
```

### Comparing `algophon-0.0.8/README.md` & `algophon-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/algophon/ipa.txt` & `algophon-0.0.9/algophon/ipa.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6362,7 +6362,8 @@
 ɫ̩	+	+	+	+	0	+	-	0	+	-	-	+	+	-	-	-	-	+	-	-	0	-	0	0
 ʟ̩	+	+	+	+	0	+	-	0	+	-	-	-	-	0	-	+	-	0	-	-	0	-	0	0
 ʎ̩	+	+	+	+	0	+	-	0	+	-	-	-	+	+	-	+	-	-	-	-	0	-	0	0
 h̩	+	+	+	+	-	-	-	0	-	-	-	-	-	0	-	-	-	-	-	-	0	-	0	0
 ɦ̩	+	+	+	+	-	-	-	0	+	-	-	-	-	0	-	-	-	-	-	-	0	-	0	0
 l̩	+	+	+	+	-	+	-	0	+	-	-	+	+	-	-	-	-	-	-	-	0	-	0	0
 l̪̩	+	+	+	+	-	+	-	0	+	-	-	+	+	+	-	-	-	-	-	-	0	-	0	0
+_	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0	0
```

### Comparing `algophon-0.0.8/algophon/natclass.py` & `algophon-0.0.9/algophon/natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/algophon/seg.py` & `algophon-0.0.9/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/algophon/seginv.py` & `algophon-0.0.9/algophon/seginv.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     
     def __len__(self) -> int:
         return len(self.segs)
     
     def __iter__(self):
         return self.segs.__iter__()
     
-    def __contains__(self, seg: object):
+    def __contains__(self, seg: object) -> bool:
         '''
         :seg: Can be any of the following:
             - str IPA symbol
             - Seg object
 
         :return: True if the :seg: is in the alphabet, False if not
         '''
         return seg in self.segs
     
-    def __getitem__(self, seg: object):
+    def __getitem__(self, seg: object) -> Seg:
         '''
         :seg: Can be any of the following:
             - str IPA symbol
             - Seg object
 
         :return: the Seg object corresponding to :seg: if present, otherwise KeyError is raised
         '''
@@ -78,15 +78,15 @@
 
         if self.ipa_file_path is None:
             # make ord('g') == 103 and ord('ɡ') == 609 the same, since panphon only as 609
             self._seg_to_feat_vec['g'] = self._seg_to_feat_vec['ɡ']
 
     def add(self, ipa_seg: str) -> None:
         '''
-        :ipa_seg: a IPA segment in str form
+        :ipa_seg: an IPA segment in str form
 
         :return: None
         '''
         if ipa_seg in self:
             return
         if ipa_seg not in self._seg_to_feat_vec:
             raise KeyError(f'Segment {ipa_seg} is not in the IPA data from {self._ipa_source}.')
```

### Comparing `algophon-0.0.8/algophon/segstr.py` & `algophon-0.0.9/algophon/segstr.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/algophon.egg-info/PKG-INFO` & `algophon-0.0.9/algophon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.24
 
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
```

### Comparing `algophon-0.0.8/pyproject.toml` & `algophon-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
@@ -19,13 +19,16 @@
     "natural language processing",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "numpy >= 1.24",
+]
 
 [tool.setuptools.package-data]
 algophon = ["ipa.txt"]
 
 [project.urls]
 Homepage = "https://github.com/cbelth/algophon"
```

### Comparing `algophon-0.0.8/tests/test_natclass.py` & `algophon-0.0.9/tests/test_natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/tests/test_seg.py` & `algophon-0.0.9/tests/test_seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/tests/test_seginv.py` & `algophon-0.0.9/tests/test_seginv.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.8/tests/test_segstr.py` & `algophon-0.0.9/tests/test_segstr.py`

 * *Files identical despite different names*

