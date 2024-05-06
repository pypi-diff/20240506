# Comparing `tmp/extradecorators-0.1.tar.gz` & `tmp/extradecorators-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extradecorators-0.1.tar", last modified: Sun May  5 18:37:26 2024, max compression
+gzip compressed data, was "extradecorators-0.2.tar", last modified: Mon May  6 16:24:37 2024, max compression
```

## Comparing `extradecorators-0.1.tar` & `extradecorators-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:37:26.667037 extradecorators-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:37:26.651910 extradecorators-0.1/ExtraDecorators/
--rw-rw-rw-   0        0        0      106 2024-05-05 17:46:27.000000 extradecorators-0.1/ExtraDecorators/__init__.py
--rw-rw-rw-   0        0        0     1007 2024-05-05 17:43:23.000000 extradecorators-0.1/ExtraDecorators/private.py
--rw-rw-rw-   0        0        0      749 2024-05-05 17:16:28.000000 extradecorators-0.1/ExtraDecorators/read_only.py
--rw-rw-rw-   0        0        0     2696 2024-05-05 18:34:58.000000 extradecorators-0.1/ExtraDecorators/validatetyping.py
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 extradecorators-0.1/LICENCE
--rw-rw-rw-   0        0        0     1329 2024-05-05 18:37:26.666530 extradecorators-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      654 2024-05-05 18:36:24.000000 extradecorators-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:37:26.665507 extradecorators-0.1/extradecorators.egg-info/
--rw-rw-rw-   0        0        0     1329 2024-05-05 18:37:26.000000 extradecorators-0.1/extradecorators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-05 18:37:26.000000 extradecorators-0.1/extradecorators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:37:26.000000 extradecorators-0.1/extradecorators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 18:37:26.000000 extradecorators-0.1/extradecorators.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 18:37:26.667037 extradecorators-0.1/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-05 17:14:55.000000 extradecorators-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:24:37.712836 extradecorators-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:24:37.698143 extradecorators-0.2/ExtraDecorators/
+-rw-rw-rw-   0        0        0      106 2024-05-05 17:46:27.000000 extradecorators-0.2/ExtraDecorators/__init__.py
+-rw-rw-rw-   0        0        0     1007 2024-05-05 17:43:23.000000 extradecorators-0.2/ExtraDecorators/private.py
+-rw-rw-rw-   0        0        0      860 2024-05-05 19:17:46.000000 extradecorators-0.2/ExtraDecorators/read_only.py
+-rw-rw-rw-   0        0        0     1588 2024-05-06 16:23:19.000000 extradecorators-0.2/ExtraDecorators/restoreAttributeTypeIntegrity.py
+-rw-rw-rw-   0        0        0      596 2024-05-06 15:59:27.000000 extradecorators-0.2/ExtraDecorators/validatetyping.py
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 extradecorators-0.2/LICENCE
+-rw-rw-rw-   0        0        0     3504 2024-05-06 16:24:37.712336 extradecorators-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2024-05-06 16:24:18.000000 extradecorators-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:24:37.711175 extradecorators-0.2/extradecorators.egg-info/
+-rw-rw-rw-   0        0        0     3504 2024-05-06 16:24:37.000000 extradecorators-0.2/extradecorators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-05-06 16:24:37.000000 extradecorators-0.2/extradecorators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:24:37.000000 extradecorators-0.2/extradecorators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 16:24:37.000000 extradecorators-0.2/extradecorators.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 16:24:37.712836 extradecorators-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-06 16:24:32.000000 extradecorators-0.2/setup.py
```

### Comparing `extradecorators-0.1/ExtraDecorators/private.py` & `extradecorators-0.2/ExtraDecorators/private.py`

 * *Files identical despite different names*

### Comparing `extradecorators-0.1/LICENCE` & `extradecorators-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `extradecorators-0.1/setup.py` & `extradecorators-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extradecorators',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='A package that contains some useful decorators for any case.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

