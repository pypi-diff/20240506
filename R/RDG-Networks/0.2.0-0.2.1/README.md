# Comparing `tmp/RDG-Networks-0.2.0.tar.gz` & `tmp/RDG-Networks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RDG-Networks-0.2.0.tar", last modified: Mon May  6 18:38:12 2024, max compression
+gzip compressed data, was "RDG-Networks-0.2.1.tar", last modified: Mon May  6 18:45:02 2024, max compression
```

## Comparing `RDG-Networks-0.2.0.tar` & `RDG-Networks-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.154549 RDG-Networks-0.2.0/
--rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.2.0/LICENSE.txt
--rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:38:12.154357 RDG-Networks-0.2.0/PKG-INFO
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.153073 RDG-Networks-0.2.0/RDG_Networks.egg-info/
--rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/PKG-INFO
--rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/entry_points.txt
--rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/requires.txt
--rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-06 18:38:12.000000 RDG-Networks-0.2.0/RDG_Networks.egg-info/top_level.txt
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:38:12.154130 RDG-Networks-0.2.0/RDG_networks/
--rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.0/RDG_networks/Classes.py
--rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.0/RDG_networks/__init__.py
--rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.0/RDG_networks/draw_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_network.py
--rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     7180 2024-05-06 18:31:43.000000 RDG-Networks-0.2.0/RDG_networks/generate_line_segments_dynamic.py
--rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.0/RDG_networks/get_intersection_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.0/RDG_networks/sample_in_polygon.py
--rw-r--r--   0 5746604    (501) staff       (20)     1392 2024-05-06 18:33:00.000000 RDG-Networks-0.2.0/README.md
--rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-06 18:38:12.154594 RDG-Networks-0.2.0/setup.cfg
--rw-r--r--   0 5746604    (501) staff       (20)     1117 2024-05-06 18:38:08.000000 RDG-Networks-0.2.0/setup.py
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.212053 RDG-Networks-0.2.1/
+-rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.2.1/LICENSE.txt
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:45:02.211866 RDG-Networks-0.2.1/PKG-INFO
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.210615 RDG-Networks-0.2.1/RDG_Networks.egg-info/
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/entry_points.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/requires.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/top_level.txt
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.211654 RDG-Networks-0.2.1/RDG_networks/
+-rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.1/RDG_networks/Classes.py
+-rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.1/RDG_networks/__init__.py
+-rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.1/RDG_networks/draw_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_network.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     7318 2024-05-06 18:44:46.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_segments_dynamic.py
+-rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.1/RDG_networks/get_intersection_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.1/RDG_networks/sample_in_polygon.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1392 2024-05-06 18:33:00.000000 RDG-Networks-0.2.1/README.md
+-rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-06 18:45:02.212099 RDG-Networks-0.2.1/setup.cfg
+-rw-r--r--   0 5746604    (501) staff       (20)     1117 2024-05-06 18:44:43.000000 RDG-Networks-0.2.1/setup.py
```

### Comparing `RDG-Networks-0.2.0/LICENSE.txt` & `RDG-Networks-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/PKG-INFO` & `RDG-Networks-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.0/RDG_Networks.egg-info/PKG-INFO` & `RDG-Networks-0.2.1/RDG_Networks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.0/RDG_Networks.egg-info/SOURCES.txt` & `RDG-Networks-0.2.1/RDG_Networks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/Classes.py` & `RDG-Networks-0.2.1/RDG_networks/Classes.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/__init__.py` & `RDG-Networks-0.2.1/RDG_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/draw_segments.py` & `RDG-Networks-0.2.1/RDG_networks/draw_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/generate_line_network.py` & `RDG-Networks-0.2.1/RDG_networks/generate_line_network.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/generate_line_segments.py` & `RDG-Networks-0.2.1/RDG_networks/generate_line_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/generate_line_segments_dynamic.py` & `RDG-Networks-0.2.1/RDG_networks/generate_line_segments_dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,23 +150,24 @@
         neighbors = [s1['neighbors_initial'], s2['neighbors_initial']]
         
         line_segment = LineSegment(start=start, end=end, id=id, neighbors_initial=neighbors)
         segments.append(line_segment)
         
     return segments
 
-def generate_line_segments_dynamic(size: int, dt: float, epsilon: float, time: float) -> List[LineSegment]:
+def generate_line_segments_dynamic(size: int, dt: float, epsilon: float, time: float, angles='uniform') -> List[LineSegment]:
     """
     Generate line segments dynamically based on growth and intersection conditions.
 
     Args:
         size (int): The desired number of line segments.
         dt (float): Time increment.
         epsilon (float): Growth rate of the lines.
         time (float): Interval at which new lines are added.
+        angles (str or List): The allowed angles in the system (default is 'uniform' for random angles).
 
     Returns:
         List[LineSegment]: A list of LineSegment objects representing standard line segments.
     """
     lines = []
     line_id, t, t_total = 1, 0, 0
 
@@ -179,15 +180,15 @@
         if t > time and len(lines) / 2 < size:
             
             if time == 0:
                 number_of_lines_to_add = size
             else:
                 number_of_lines_to_add = int(t - (t % time))
             for _ in range(number_of_lines_to_add):
-                lines = add_new_line(lines, line_id, t_total)
+                lines = add_new_line(lines, line_id, t_total, angles=angles)
                 line_id += 1
             
                 t = 0
 
         lines = grow_lines(lines, epsilon)
         lines = update_for_border_intersections(lines)
         lines = check_and_update_when_intersect(lines, epsilon)
```

### Comparing `RDG-Networks-0.2.0/RDG_networks/get_intersection_segments.py` & `RDG-Networks-0.2.1/RDG_networks/get_intersection_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/RDG_networks/sample_in_polygon.py` & `RDG-Networks-0.2.1/RDG_networks/sample_in_polygon.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/README.md` & `RDG-Networks-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.0/setup.py` & `RDG-Networks-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RDG-Networks',
-    version='0.2.0',
+    version='0.2.1',
     author='Niek Mooij',
     author_email='mooij.niek@gmail.com',
     description='Most of the code from the RDG Networks project',
     long_description=open('README.md').read(),
     url='https://github.com/NiekMooij/RDG_networks',
     classifiers=[
             'Programming Language :: Python :: 3',
```

