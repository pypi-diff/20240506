# Comparing `tmp/astro_SPLASH-0.0.4.tar.gz` & `tmp/astro_SPLASH-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_SPLASH-0.0.4.tar", last modified: Mon May  6 04:36:37 2024, max compression
+gzip compressed data, was "astro_SPLASH-0.0.5.tar", last modified: Mon May  6 04:37:15 2024, max compression
```

## Comparing `astro_SPLASH-0.0.4.tar` & `astro_SPLASH-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:36:37.704533 astro_SPLASH-0.0.4/
--rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:36:37.704104 astro_SPLASH-0.0.4/PKG-INFO
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:36:37.700085 astro_SPLASH-0.0.4/SPLASH/
--rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:09.000000 astro_SPLASH-0.0.4/SPLASH/__init__.py
--rw-r--r--   0 adamboesky   (501) staff       (20)    12044 2024-05-06 03:59:39.000000 astro_SPLASH-0.0.4/SPLASH/pipeline.py
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:36:37.700963 astro_SPLASH-0.0.4/SPLASH/trained_models/
--rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:22.000000 astro_SPLASH-0.0.4/SPLASH/trained_models/__init__.py
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:36:37.702974 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/
--rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:36:37.000000 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/PKG-INFO
--rw-r--r--   0 adamboesky   (501) staff       (20)      438 2024-05-06 04:36:37.000000 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/SOURCES.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)        1 2024-05-06 04:36:37.000000 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/dependency_links.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)       22 2024-05-06 04:36:37.000000 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/requires.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)        7 2024-05-06 04:36:37.000000 astro_SPLASH-0.0.4/astro_SPLASH.egg-info/top_level.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)       38 2024-05-06 04:36:37.704679 astro_SPLASH-0.0.4/setup.cfg
--rw-r--r--   0 adamboesky   (501) staff       (20)      687 2024-05-06 04:36:33.000000 astro_SPLASH-0.0.4/setup.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:37:15.279715 astro_SPLASH-0.0.5/
+-rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:37:15.279416 astro_SPLASH-0.0.5/PKG-INFO
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:37:15.275930 astro_SPLASH-0.0.5/SPLASH/
+-rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:09.000000 astro_SPLASH-0.0.5/SPLASH/__init__.py
+-rw-r--r--   0 adamboesky   (501) staff       (20)    12044 2024-05-06 03:59:39.000000 astro_SPLASH-0.0.5/SPLASH/pipeline.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:37:15.276773 astro_SPLASH-0.0.5/SPLASH/trained_models/
+-rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:22.000000 astro_SPLASH-0.0.5/SPLASH/trained_models/__init__.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:37:15.278688 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/
+-rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:37:15.000000 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/PKG-INFO
+-rw-r--r--   0 adamboesky   (501) staff       (20)      438 2024-05-06 04:37:15.000000 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/SOURCES.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)        1 2024-05-06 04:37:15.000000 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/dependency_links.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)       27 2024-05-06 04:37:15.000000 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/requires.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)        7 2024-05-06 04:37:15.000000 astro_SPLASH-0.0.5/astro_SPLASH.egg-info/top_level.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)       38 2024-05-06 04:37:15.279844 astro_SPLASH-0.0.5/setup.cfg
+-rw-r--r--   0 adamboesky   (501) staff       (20)      692 2024-05-06 04:37:13.000000 astro_SPLASH-0.0.5/setup.py
```

### Comparing `astro_SPLASH-0.0.4/SPLASH/pipeline.py` & `astro_SPLASH-0.0.5/SPLASH/pipeline.py`

 * *Files identical despite different names*

### Comparing `astro_SPLASH-0.0.4/setup.py` & `astro_SPLASH-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name='astro_SPLASH',
-    version='0.0.4',
+    version='0.0.5',
     author='Adam Boesky',
     author_email='apboesky@gmail.com',
     description='SPLASH (Supernova classification Pipeline Leveraging Attributes of Supernova Hosts)',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.11',
     install_requires=['pytorch',
                       'numpy',
-                      'sklearn'],
+                      'scikit-learn'],
 )
 
 # To republish:
 # 1. bump version nuber
 # 2. python setup.py sdist
 # 3. twine upload dist/*
```

