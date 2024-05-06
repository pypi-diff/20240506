# Comparing `tmp/RDG-Networks-0.1.8.tar.gz` & `tmp/RDG-Networks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RDG-Networks-0.1.8.tar", last modified: Mon Mar  4 14:52:45 2024, max compression
+gzip compressed data, was "RDG-Networks-0.2.0.tar", last modified: Mon May  6 18:38:12 2024, max compression
```

## Comparing `RDG-Networks-0.1.8.tar` & `RDG-Networks-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-03-04 14:52:45.578154 RDG-Networks-0.1.8/
--rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.1.8/LICENSE.txt
--rw-r--r--   0 5746604    (501) staff       (20)     1756 2024-03-04 14:52:45.577955 RDG-Networks-0.1.8/PKG-INFO
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-03-04 14:52:45.576825 RDG-Networks-0.1.8/RDG_Networks.egg-info/
--rw-r--r--   0 5746604    (501) staff       (20)     1756 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/PKG-INFO
--rw-r--r--   0 5746604    (501) staff       (20)      480 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 5746604    (501) staff       (20)        1 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 5746604    (501) staff       (20)      268 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/entry_points.txt
--rw-r--r--   0 5746604    (501) staff       (20)       36 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/requires.txt
--rw-r--r--   0 5746604    (501) staff       (20)       13 2024-03-04 14:52:45.000000 RDG-Networks-0.1.8/RDG_Networks.egg-info/top_level.txt
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-03-04 14:52:45.577738 RDG-Networks-0.1.8/RDG_networks/
--rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.1.8/RDG_networks/Classes.py
--rw-r--r--   0 5746604    (501) staff       (20)      759 2024-03-01 13:28:56.000000 RDG-Networks-0.1.8/RDG_networks/__init__.py
--rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.1.8/RDG_networks/draw_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.1.8/RDG_networks/generate_line_network.py
--rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-03-04 14:31:49.000000 RDG-Networks-0.1.8/RDG_networks/generate_line_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.1.8/RDG_networks/get_intersection_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.1.8/RDG_networks/sample_in_polygon.py
--rw-r--r--   0 5746604    (501) staff       (20)     1252 2024-03-01 13:27:45.000000 RDG-Networks-0.1.8/README.md
--rw-r--r--   0 5746604    (501) staff       (20)       38 2024-03-04 14:52:45.578199 RDG-Networks-0.1.8/setup.cfg
--rw-r--r--   0 5746604    (501) staff       (20)     1022 2024-03-04 14:52:42.000000 RDG-Networks-0.1.8/setup.py
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.154549 RDG-Networks-0.2.0/
+-rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.2.0/LICENSE.txt
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:38:12.154357 RDG-Networks-0.2.0/PKG-INFO
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.153073 RDG-Networks-0.2.0/RDG_Networks.egg-info/
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/entry_points.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/requires.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/top_level.txt
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.154130 RDG-Networks-0.2.0/RDG_networks/
+-rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.0/RDG_networks/Classes.py
+-rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.0/RDG_networks/__init__.py
+-rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.0/RDG_networks/draw_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_network.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     7180 2024-05-06 18:31:43.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_segments_dynamic.py
+-rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.0/RDG_networks/get_intersection_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.0/RDG_networks/sample_in_polygon.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1392 2024-05-06 18:33:00.000000 RDG-Networks-0.2.0/README.md
+-rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-06 18:38:12.154594 RDG-Networks-0.2.0/setup.cfg
+-rw-r--r--   0 5746604    (501) staff       (20)     1117 2024-05-06 18:38:08.000000 RDG-Networks-0.2.0/setup.py
```

### Comparing `RDG-Networks-0.1.8/LICENSE.txt` & `RDG-Networks-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/PKG-INFO` & `RDG-Networks-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.1.8
+Version: 0.2.0
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 - [Contact](#contact)
 
 ## Features
 
 - **generate_line_segments:** Function that determines the linesegments of a RDG network.
 - **generate_line_network:** Function that makes the underlying network of the linesegments.
 - **get_intersection_segments:** Function that determines the intersection segments of a RDG network.
+- **generate_line_segments_dynamic:** Function that determines the segments of a dynamic RDG network (with increasing linelengths in time).
 - **draw_segments:** Function that draws the segments.
 
 
 ## Installation
 You can install the package using pip:
 
 ```bash
```

### Comparing `RDG-Networks-0.1.8/RDG_Networks.egg-info/PKG-INFO` & `RDG-Networks-0.2.0/RDG_Networks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.1.8
+Version: 0.2.0
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 - [Contact](#contact)
 
 ## Features
 
 - **generate_line_segments:** Function that determines the linesegments of a RDG network.
 - **generate_line_network:** Function that makes the underlying network of the linesegments.
 - **get_intersection_segments:** Function that determines the intersection segments of a RDG network.
+- **generate_line_segments_dynamic:** Function that determines the segments of a dynamic RDG network (with increasing linelengths in time).
 - **draw_segments:** Function that draws the segments.
 
 
 ## Installation
 You can install the package using pip:
 
 ```bash
```

### Comparing `RDG-Networks-0.1.8/RDG_networks/Classes.py` & `RDG-Networks-0.2.0/RDG_networks/Classes.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/RDG_networks/draw_segments.py` & `RDG-Networks-0.2.0/RDG_networks/draw_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/RDG_networks/generate_line_network.py` & `RDG-Networks-0.2.0/RDG_networks/generate_line_network.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/RDG_networks/generate_line_segments.py` & `RDG-Networks-0.2.0/RDG_networks/generate_line_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/RDG_networks/get_intersection_segments.py` & `RDG-Networks-0.2.0/RDG_networks/get_intersection_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/RDG_networks/sample_in_polygon.py` & `RDG-Networks-0.2.0/RDG_networks/sample_in_polygon.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.1.8/README.md` & `RDG-Networks-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - [Contact](#contact)
 
 ## Features
 
 - **generate_line_segments:** Function that determines the linesegments of a RDG network.
 - **generate_line_network:** Function that makes the underlying network of the linesegments.
 - **get_intersection_segments:** Function that determines the intersection segments of a RDG network.
+- **generate_line_segments_dynamic:** Function that determines the segments of a dynamic RDG network (with increasing linelengths in time).
 - **draw_segments:** Function that draws the segments.
 
 
 ## Installation
 You can install the package using pip:
 
 ```bash
```

### Comparing `RDG-Networks-0.1.8/setup.py` & `RDG-Networks-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RDG-Networks',
-    version='0.1.8',
+    version='0.2.0',
     author='Niek Mooij',
     author_email='mooij.niek@gmail.com',
     description='Most of the code from the RDG Networks project',
     long_description=open('README.md').read(),
     url='https://github.com/NiekMooij/RDG_networks',
     classifiers=[
             'Programming Language :: Python :: 3',
@@ -21,11 +21,12 @@
         'typing'
     ],
     entry_points={
         'console_scripts': [
             'generate_line_segments=RDG_networks.generate_line_segments:main',
             'generate_line_network=RDG_networks.generate_line_network:main',
             'get_intersection_segments=RDG_networks.get_intersection_segments:main',
+            'generate_line_segments_dynamic=RDG_networks.generate_line_segments_dynamic:main',
             'draw_segments=RDG_networks.draw_segments:main'
         ],
     },
 )
```

