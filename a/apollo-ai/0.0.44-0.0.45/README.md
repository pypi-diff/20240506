# Comparing `tmp/apollo-ai-0.0.44.tar.gz` & `tmp/apollo-ai-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-ai-0.0.44.tar", last modified: Thu May  2 15:40:38 2024, max compression
+gzip compressed data, was "apollo-ai-0.0.45.tar", last modified: Mon May  6 01:26:58 2024, max compression
```

## Comparing `apollo-ai-0.0.44.tar` & `apollo-ai-0.0.45.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:38.059880 apollo-ai-0.0.44/
--rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.44/LICENSE
--rw-rw-rw-   0        0        0     9511 2024-05-02 15:40:38.057857 apollo-ai-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.44/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:37.980303 apollo-ai-0.0.44/apollo/
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:38.011299 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/
--rw-rw-rw-   0        0        0     9511 2024-05-02 15:40:37.000000 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-02 15:40:37.000000 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:40:37.000000 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2024-05-02 15:40:37.000000 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-02 15:40:37.000000 apollo-ai-0.0.44/apollo/apollo_ai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:38.027297 apollo-ai-0.0.44/apollo/argus/
--rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/argus/__init__.py
--rw-rw-rw-   0        0        0    12224 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/argus/argus.py
--rw-rw-rw-   0        0        0     6904 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/argus/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:38.041297 apollo-ai-0.0.44/apollo/lyre/
--rw-rw-rw-   0        0        0      233 2023-11-11 21:10:51.000000 apollo-ai-0.0.44/apollo/lyre/__init__.py
--rw-rw-rw-   0        0        0    13458 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/lyre/lyre.py
--rw-rw-rw-   0        0        0      848 2023-11-10 23:08:26.000000 apollo-ai-0.0.44/apollo/lyre/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:40:38.054316 apollo-ai-0.0.44/apollo/pythia/
--rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/pythia/__init__.py
--rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/pythia/pythia.py
--rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.44/apollo/pythia/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-02 15:40:38.060891 apollo-ai-0.0.44/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-02 15:40:32.000000 apollo-ai-0.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:58.013621 apollo-ai-0.0.45/
+-rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.45/LICENSE
+-rw-rw-rw-   0        0        0     9511 2024-05-06 01:26:58.010625 apollo-ai-0.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.45/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:57.882619 apollo-ai-0.0.45/apollo/
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:57.931611 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/
+-rw-rw-rw-   0        0        0     9511 2024-05-06 01:26:56.000000 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-06 01:26:57.000000 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 01:26:56.000000 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      596 2024-05-06 01:26:56.000000 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 01:26:56.000000 apollo-ai-0.0.45/apollo/apollo_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:57.954608 apollo-ai-0.0.45/apollo/argus/
+-rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.45/apollo/argus/__init__.py
+-rw-rw-rw-   0        0        0    12278 2024-05-06 01:23:56.000000 apollo-ai-0.0.45/apollo/argus/argus.py
+-rw-rw-rw-   0        0        0     6864 2024-05-06 01:24:34.000000 apollo-ai-0.0.45/apollo/argus/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:57.965643 apollo-ai-0.0.45/apollo/lyre/
+-rw-rw-rw-   0        0        0      149 2024-05-06 00:09:56.000000 apollo-ai-0.0.45/apollo/lyre/__init__.py
+-rw-rw-rw-   0        0        0     9151 2024-05-06 00:33:58.000000 apollo-ai-0.0.45/apollo/lyre/lyre.py
+-rw-rw-rw-   0        0        0     3140 2024-05-06 00:05:59.000000 apollo-ai-0.0.45/apollo/lyre/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:26:58.005622 apollo-ai-0.0.45/apollo/pythia/
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.45/apollo/pythia/__init__.py
+-rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.45/apollo/pythia/pythia.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.45/apollo/pythia/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 01:26:58.014624 apollo-ai-0.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-06 01:26:45.000000 apollo-ai-0.0.45/setup.py
```

### Comparing `apollo-ai-0.0.44/LICENSE` & `apollo-ai-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.44/PKG-INFO` & `apollo-ai-0.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.44
+Version: 0.0.45
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.44/README.md` & `apollo-ai-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.44/apollo/apollo_ai.egg-info/PKG-INFO` & `apollo-ai-0.0.45/apollo/apollo_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.44
+Version: 0.0.45
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.44/apollo/apollo_ai.egg-info/requires.txt` & `apollo-ai-0.0.45/apollo/apollo_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.44/apollo/argus/argus.py` & `apollo-ai-0.0.45/apollo/argus/argus.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from sixdrepnet import SixDRepNet
 from face_detection import RetinaFace
 from scipy.spatial import distance
 import matplotlib.pyplot as plt
 from scipy.signal import savgol_filter
 import numpy as np
 import time
+import json
 import logging
 import math
 from .utils import (
     plot_pose_cube,
     filter_video_data,
     plot_head_data_mov,
     plot_head_data_speed
@@ -18,15 +19,15 @@
 from .utils import ensure_dir_created
 
 logging.basicConfig(format='APOLLO: (%(asctime)s): %(message)s', datefmt='%d/%m/%Y %I:%M:%S %p',
                     level=logging.DEBUG)
 
 
 def mouth_movement(filepath: str, focal_length_mm: int, output_dir='./output', plot=False,
-                   normalize=False, lim: list[float, float] = None) -> dict:
+                   normalize=False, lim: list[float, float] = None) -> str:
     """
     Generates the face data points for a given video, it currently accepts a small variety of part indices in the face
 
     :param filepath:
     :param focal_length_mm:
     :param output_dir:
     :param plot:
@@ -128,31 +129,31 @@
     y_values = distances_data['Distance'].tolist()
 
     data = {"x_values": x_values, "y_values": y_values, "fps": fps_general, "min_distance": min_distance,
             "max_distance": max_distance, "frame_width": frame_width, "frame_height": frame_height}
 
     if plot:
         # Middle line value to specify the mouth closing region
-        threshold = ((max_distance + min_distance) / 2) * 0.6
+        threshold = ((max_distance + min_distance) / 2) * 0.9
 
         plt.figure(figsize=(10, 6))
         plt.plot(x_values, y_values, label="Part Opening Distance", color='b')
         plt.xlabel("Timestamp (s)")
         plt.ylabel("Distance (mm)")
         plt.title("Distance vs. Timestamp")
         plt.axhline(y=threshold, color='r', linestyle='--', label='Threshold')
         plt.grid(True)
         plt.legend()
         plt.savefig(f'{file_direction}.png')
 
-    return data
+    return json.dumps(data)
 
 
 def head_position(filepath: str, output_dir="./output", plot=False, real_head_width=145,
-                  lim: list[float, float] = None) -> dict:
+                  lim: list[float, float] = None) -> str:
     """
     Estimates the head position over time
 
     :param filepath:
     :param output_dir:
     :param plot:
     :param real_head_width:
@@ -314,16 +315,18 @@
                            roll_vals=roll_vals)
 
         plot_head_data_speed(file_direction=file_direction,
                              time_in_seconds=x_head_speed,
                              head_speeds_mm=head_speeds_smooth,
                              threshold_mm=threshold_mm)
 
-    return {"x_head_speed": x_head_speed,
+    data = {"x_head_speed": x_head_speed,
             "y_head_speed": head_speeds_smooth,
             "x_head_movement": time_in_seconds,
             "y_pitch_values": pitch_vals,
             "y_yaw_values": yaw_vals,
             "y_roll_values": roll_vals,
             "threshold_speed": threshold_mm,
             "average_speed": mean_speed}
 
+    return json.dumps(data)
+
```

### Comparing `apollo-ai-0.0.44/apollo/argus/utils.py` & `apollo-ai-0.0.45/apollo/argus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
         # Calculate the normalization based on min and max values
         if normalize:
             max_value = df['Distance'].max()
             min_value = df['Distance'].min()
             df['Distance'] = (df['Distance'] - min_value) / (max_value - min_value)
 
-        # Smooth the data using scipy and Savitzky-Golay Filter
-        df['Distance'] = signal.savgol_filter(df["Distance"], 260, 3)
+        df['Distance'] = signal.savgol_filter(df["Distance"], min(len(df["Distance"]), 51), 3)
 
         return df
     except Exception as e:
         raise Exception("Error normalizing the data: {0}".format(e))
 
 
 def plot_pose_cube(img, yaw, pitch, roll, tdx=None, tdy=None, size=150.):
```

### Comparing `apollo-ai-0.0.44/apollo/pythia/pythia.py` & `apollo-ai-0.0.45/apollo/pythia/pythia.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.44/apollo/pythia/utils.py` & `apollo-ai-0.0.45/apollo/pythia/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.44/setup.py` & `apollo-ai-0.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="apollo-ai",
-    version="0.0.44",
+    version="0.0.45",
     description="Framework to process 3 channels in one: Video, Audio & Text",
     package_dir={"": "apollo"},
     packages=find_packages(where="apollo"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VerbaNexAI/APOLLO.AI",
     author="VerbaNex, Riddle",
```

