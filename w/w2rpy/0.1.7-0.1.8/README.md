# Comparing `tmp/w2rpy-0.1.7.tar.gz` & `tmp/w2rpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.7.tar", last modified: Mon May  6 19:46:42 2024, max compression
+gzip compressed data, was "w2rpy-0.1.8.tar", last modified: Mon May  6 19:49:40 2024, max compression
```

## Comparing `w2rpy-0.1.7.tar` & `w2rpy-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:46:42.609265 w2rpy-0.1.7/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      379 2024-05-06 19:46:42.608260 w2rpy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.7/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 19:46:42.610260 w2rpy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-05-06 19:44:23.000000 w2rpy-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:46:42.608260 w2rpy-0.1.7/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      379 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    28193 2024-05-06 19:30:27.000000 w2rpy-0.1.7/w2rpy.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:49:40.610445 w2rpy-0.1.8/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:49:40.610445 w2rpy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.8/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:49:40.611451 w2rpy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-05-06 19:49:12.000000 w2rpy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:49:40.609444 w2rpy-0.1.8/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28231 2024-05-06 19:48:33.000000 w2rpy-0.1.8/w2rpy.py
```

### Comparing `w2rpy-0.1.7/LICENSE` & `w2rpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.7/setup.py` & `w2rpy-0.1.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from distutils.core import setup
 
 setup(
   name = 'w2rpy',    
   py_modules=['w2rpy'],
-  version = '0.1.7',     
+  version = '0.1.8',     
   license='MIT',        
   description = 'Water Resource Functions For Fluvial Systems',   
   author = 'Luke Russell',                   
   author_email = 'lrussell@wolfwaterresources.com',      
   install_requires=['pandas',
                     'numpy',
                     'shapely',
```

### Comparing `w2rpy-0.1.7/w2rpy.py` & `w2rpy-0.1.8/w2rpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     grid.clip_to(catch)
 
     # Extract river network to geodataframe 
     branches = grid.extract_river_network(terrain.fdir, terrain.acc > threshold)
     file = str(branches)
     
     lines = gpd.read_file(file)
+    lines['FID'] = range(len(lines))
     lines['upstream'] = [[np.nan]]*len(lines)
     lines['downstream'] = [[np.nan]]*len(lines)
     
     # for each line...
     for i in lines.FID:
         ind = lines.loc[lines.FID==i].index[0]
         cl = lines.loc[lines.FID==i, 'geometry'].values[0]
```

