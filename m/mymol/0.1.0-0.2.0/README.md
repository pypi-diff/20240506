# Comparing `tmp/mymol-0.1.0.tar.gz` & `tmp/mymol-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymol-0.1.0.tar", last modified: Thu May  2 16:22:21 2024, max compression
+gzip compressed data, was "mymol-0.2.0.tar", last modified: Mon May  6 17:44:10 2024, max compression
```

## Comparing `mymol-0.1.0.tar` & `mymol-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:22:21.283302 mymol-0.1.0/
--rw-rw-rw-   0        0        0     1087 2024-05-02 16:16:08.000000 mymol-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1648 2024-05-02 16:22:21.282017 mymol-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      949 2024-05-02 16:14:25.000000 mymol-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 16:22:21.281021 mymol-0.1.0/mymol.egg-info/
--rw-rw-rw-   0        0        0     1648 2024-05-02 16:22:21.000000 mymol-0.1.0/mymol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-02 16:22:21.000000 mymol-0.1.0/mymol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:22:21.000000 mymol-0.1.0/mymol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 16:22:21.000000 mymol-0.1.0/mymol.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 16:22:21.280017 mymol-0.1.0/packages/
--rw-rw-rw-   0        0        0      117 2024-05-02 16:19:25.000000 mymol-0.1.0/packages/__init__.py
--rw-rw-rw-   0        0        0     5580 2024-05-02 16:01:46.000000 mymol-0.1.0/packages/mymol.py
--rw-rw-rw-   0        0        0       42 2024-05-02 16:22:21.283302 mymol-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      850 2024-05-02 16:17:41.000000 mymol-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:44:10.798425 mymol-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-02 16:16:08.000000 mymol-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1640 2024-05-06 17:44:10.797426 mymol-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2024-05-02 16:14:25.000000 mymol-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:44:10.796427 mymol-0.2.0/mymol.egg-info/
+-rw-rw-rw-   0        0        0     1640 2024-05-06 17:44:10.000000 mymol-0.2.0/mymol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-06 17:44:10.000000 mymol-0.2.0/mymol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:44:10.000000 mymol-0.2.0/mymol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 17:44:10.000000 mymol-0.2.0/mymol.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 17:44:10.795427 mymol-0.2.0/packages/
+-rw-rw-rw-   0        0        0      119 2024-05-06 17:07:01.000000 mymol-0.2.0/packages/__init__.py
+-rw-rw-rw-   0        0        0     6798 2024-05-06 17:04:19.000000 mymol-0.2.0/packages/mymol.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:44:10.798425 mymol-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-05-06 17:06:45.000000 mymol-0.2.0/setup.py
```

### Comparing `mymol-0.1.0/LICENSE.txt` & `mymol-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mymol-0.1.0/PKG-INFO` & `mymol-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mymol
-Version: 0.1.0
+Version: 0.2.0
 Summary: An usefull python module
-Home-page: https://github.com/your-username/your-module
+Home-page: https://github.com/tureluurtje/mymol
 Author: Arthur Kwak
 Author-email: arthurmichielkwak@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mymol-0.1.0/README.md` & `mymol-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mymol-0.1.0/mymol.egg-info/PKG-INFO` & `mymol-0.2.0/mymol.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mymol
-Version: 0.1.0
+Version: 0.2.0
 Summary: An usefull python module
-Home-page: https://github.com/your-username/your-module
+Home-page: https://github.com/tureluurtje/mymol
 Author: Arthur Kwak
 Author-email: arthurmichielkwak@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mymol-0.1.0/setup.py` & `mymol-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mymol',
-    version='0.1.0',
+    version='0.2.0',
     author='Arthur Kwak',
     author_email='arthurmichielkwak@gmail.com',
     description='An usefull python module',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/your-username/your-module',
+    url='https://github.com/tureluurtje/mymol',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

