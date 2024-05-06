# Comparing `tmp/pyviz3d-0.3.1.tar.gz` & `tmp/pyviz3d-0.3.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviz3d-0.3.1.tar", last modified: Sun May  5 20:42:58 2024, max compression
+gzip compressed data, was "pyviz3d-0.3.221.tar", last modified: Mon May  6 17:38:49 2024, max compression
```

## Comparing `pyviz3d-0.3.1.tar` & `pyviz3d-0.3.221.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.646658 pyviz3d-0.3.1/
--rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/LICENSE
--rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/MANIFEST.in
--rw-r--r--   0 francis    (501) staff       (20)     6512 2024-05-05 20:42:58.646453 pyviz3d-0.3.1/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)     4707 2024-03-09 19:10:08.000000 pyviz3d-0.3.1/README.md
--rw-r--r--   0 francis    (501) staff       (20)      684 2024-05-05 20:34:58.000000 pyviz3d-0.3.1/pyproject.toml
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.641844 pyviz3d-0.3.1/pyviz3d/
--rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/__init__.py
--rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.1/pyviz3d/arrow.py
--rw-r--r--   0 francis    (501) staff       (20)     1135 2024-03-09 12:06:52.000000 pyviz3d-0.3.1/pyviz3d/camera.py
--rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.1/pyviz3d/circles_2d.py
--rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.1/pyviz3d/cuboid.py
--rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.1/pyviz3d/labels.py
--rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.1/pyviz3d/lines.py
--rw-r--r--   0 francis    (501) staff       (20)     1635 2024-05-05 18:13:27.000000 pyviz3d-0.3.1/pyviz3d/mesh.py
--rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.1/pyviz3d/points.py
--rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.1/pyviz3d/polyline.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.643998 pyviz3d-0.3.1/pyviz3d/src/
--rw-r--r--   0 francis    (501) staff       (20)    10204 2024-05-05 20:18:23.000000 pyviz3d-0.3.1/pyviz3d/src/blender_tools.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.644369 pyviz3d-0.3.1/pyviz3d/src/css/
--rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/css/bootstrap.min.css
--rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/favicon.ico
--rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/index.html
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.645721 pyviz3d-0.3.1/pyviz3d/src/js/
--rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/js/bootstrap.min.js
--rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/js/jquery.min.js
--rw-r--r--   0 francis    (501) staff       (20)    25452 2024-05-05 19:26:19.000000 pyviz3d-0.3.1/pyviz3d/src/js/scene.js
--rw-r--r--   0 francis    (501) staff       (20)    16896 2024-05-05 20:03:20.000000 pyviz3d-0.3.1/pyviz3d/visualizer.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.646115 pyviz3d-0.3.1/pyviz3d.egg-info/
--rw-r--r--   0 francis    (501) staff       (20)     6512 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)      599 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/SOURCES.txt
--rw-r--r--   0 francis    (501) staff       (20)        1 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/dependency_links.txt
--rw-r--r--   0 francis    (501) staff       (20)        6 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/requires.txt
--rw-r--r--   0 francis    (501) staff       (20)        8 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/top_level.txt
--rw-r--r--   0 francis    (501) staff       (20)       38 2024-05-05 20:42:58.646697 pyviz3d-0.3.1/setup.cfg
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.502642 pyviz3d-0.3.221/
+-rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/LICENSE
+-rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/MANIFEST.in
+-rw-r--r--   0 francis    (501) staff       (20)     7360 2024-05-06 17:38:49.502384 pyviz3d-0.3.221/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)     5553 2024-05-06 16:20:27.000000 pyviz3d-0.3.221/README.md
+-rw-r--r--   0 francis    (501) staff       (20)      686 2024-05-06 17:38:29.000000 pyviz3d-0.3.221/pyproject.toml
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.495904 pyviz3d-0.3.221/pyviz3d/
+-rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/__init__.py
+-rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.221/pyviz3d/arrow.py
+-rw-r--r--   0 francis    (501) staff       (20)     1236 2024-05-06 17:21:54.000000 pyviz3d-0.3.221/pyviz3d/camera.py
+-rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.221/pyviz3d/circles_2d.py
+-rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.221/pyviz3d/cuboid.py
+-rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.221/pyviz3d/labels.py
+-rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.221/pyviz3d/lines.py
+-rw-r--r--   0 francis    (501) staff       (20)     1635 2024-05-05 18:13:27.000000 pyviz3d-0.3.221/pyviz3d/mesh.py
+-rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.221/pyviz3d/points.py
+-rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.221/pyviz3d/polyline.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.498119 pyviz3d-0.3.221/pyviz3d/src/
+-rw-r--r--   0 francis    (501) staff       (20)    10346 2024-05-06 17:23:06.000000 pyviz3d-0.3.221/pyviz3d/src/blender_tools.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.498482 pyviz3d-0.3.221/pyviz3d/src/css/
+-rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/src/css/bootstrap.min.css
+-rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/src/favicon.ico
+-rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/src/index.html
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.499976 pyviz3d-0.3.221/pyviz3d/src/js/
+-rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/src/js/bootstrap.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.221/pyviz3d/src/js/jquery.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    25452 2024-05-05 19:26:19.000000 pyviz3d-0.3.221/pyviz3d/src/js/scene.js
+-rw-r--r--   0 francis    (501) staff       (20)    17121 2024-05-06 17:19:59.000000 pyviz3d-0.3.221/pyviz3d/visualizer.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:38:49.502043 pyviz3d-0.3.221/pyviz3d.egg-info/
+-rw-r--r--   0 francis    (501) staff       (20)     7360 2024-05-06 17:38:49.000000 pyviz3d-0.3.221/pyviz3d.egg-info/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)      599 2024-05-06 17:38:49.000000 pyviz3d-0.3.221/pyviz3d.egg-info/SOURCES.txt
+-rw-r--r--   0 francis    (501) staff       (20)        1 2024-05-06 17:38:49.000000 pyviz3d-0.3.221/pyviz3d.egg-info/dependency_links.txt
+-rw-r--r--   0 francis    (501) staff       (20)        6 2024-05-06 17:38:49.000000 pyviz3d-0.3.221/pyviz3d.egg-info/requires.txt
+-rw-r--r--   0 francis    (501) staff       (20)        8 2024-05-06 17:38:49.000000 pyviz3d-0.3.221/pyviz3d.egg-info/top_level.txt
+-rw-r--r--   0 francis    (501) staff       (20)       38 2024-05-06 17:38:49.502694 pyviz3d-0.3.221/setup.cfg
```

### Comparing `pyviz3d-0.3.1/LICENSE` & `pyviz3d-0.3.221/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/PKG-INFO` & `pyviz3d-0.3.221/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.1
+Version: 0.3.221
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,20 +38,19 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip3 install pyviz3d```
-- [Documentation](https://francisengelmann.github.io/PyViz3D/)
-- [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
-- [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
+- Install: ```python -m pip install pyviz3d```
+- [Examples](#examples)
+- [Deployment](#deployment)
 
-### Examples
+# Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/graph/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_graph.png" />
   <img width="45%" src="docs/img/example_graph_blender.png" />
 </p>
@@ -60,44 +59,54 @@
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_blender.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/blender/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_blender.png" />
   <img width="45%" src="docs/img/example_blender_blender.png" />
 </p>
 
-Polygon meshes example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+Arrow example.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
 
 Bounding boxes example.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_bounding_boxes.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_bounding_boxes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 
-Polyline example.
+Polygon meshes (.obj and .ply).
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+
+Point clouds, segments and normals.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_normals.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+
+Polylines.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_polylines.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_polylines.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 
-Arrow example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-
-Point clouds and segments example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
-[<p align="center"><img width="60%" src="docs/img/example.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+Superquadrics.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_superquadrics.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_superquadrics.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+
+Text Labels.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_text.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_text.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
 
-# Blender
+<!-- # Blender
 To create beautiful illustrations with blender consider the following points:
 - Install Blender from https://www.blender.org/ (tested version 4.0).
 - Calling `v.save(..., show_in_blender=True)` creates a `.blend` file which you can open in blender.
-- Check `examples/examples_graph.py` for a complete example.
+- Check `examples/examples_graph.py` for a complete example. -->
 <!-- 2. Set up alias in you ~/.bashrc or ~/.zshrc etc. -->
 <!-- `alias blender="/Applications/Blender.app/Contents/MacOS/Blender"` -->
 <!-- then `source ~/.zshrc` -->
 <!-- 2. `blender myscene.blend --background --python blender.py` -->
 <!-- currently there is no myscene.blend to remove that: `blender --background --python blender.py` -->
 <!-- Select camera: View/Cameras/Active Camera     -->
 <!-- Lock camera to view:   -->
@@ -106,19 +115,32 @@
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
 # Deployment
-- Make sure twine is installed: `python3 -m pip install build twine`
-- Create source archive and wheel: `python3 -m build`
-- Check that it will render properly on PyPi: `twine check dist/*`
-- Upload to PyPi: `twine upload dist/*`
 
+[Instructions for PyPi](https://packaging.python.org/en/latest/tutorials/packaging-projects/) and [API Token](https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#create-an-account).
+
+One time setup:
+```
+vim ~/.pypirc  # put __token__ as username 
+python3 -m pip install build twine
+python3 -m pip install --upgrade build
+```
+
+Upload latest version to pypi:
+```
+vim pyproject.toml  # update version
+rm -rf dist
+rm -rf example_*
+python3 -m build
+python3 -m twine upload --repository testpypi dist/*
+```
 
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
```

### Comparing `pyviz3d-0.3.1/README.md` & `pyviz3d-0.3.221/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip3 install pyviz3d```
-- [Documentation](https://francisengelmann.github.io/PyViz3D/)
-- [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
-- [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
+- Install: ```python -m pip install pyviz3d```
+- [Examples](#examples)
+- [Deployment](#deployment)
 
-### Examples
+# Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/graph/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_graph.png" />
   <img width="45%" src="docs/img/example_graph_blender.png" />
 </p>
@@ -23,44 +22,54 @@
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_blender.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/blender/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_blender.png" />
   <img width="45%" src="docs/img/example_blender_blender.png" />
 </p>
 
-Polygon meshes example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+Arrow example.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
 
 Bounding boxes example.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_bounding_boxes.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_bounding_boxes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 
-Polyline example.
+Polygon meshes (.obj and .ply).
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+
+Point clouds, segments and normals.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_normals.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+
+Polylines.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_polylines.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_polylines.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 
-Arrow example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-
-Point clouds and segments example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
-[<p align="center"><img width="60%" src="docs/img/example.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+Superquadrics.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_superquadrics.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_superquadrics.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+
+Text Labels.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_text.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_text.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
 
-# Blender
+<!-- # Blender
 To create beautiful illustrations with blender consider the following points:
 - Install Blender from https://www.blender.org/ (tested version 4.0).
 - Calling `v.save(..., show_in_blender=True)` creates a `.blend` file which you can open in blender.
-- Check `examples/examples_graph.py` for a complete example.
+- Check `examples/examples_graph.py` for a complete example. -->
 <!-- 2. Set up alias in you ~/.bashrc or ~/.zshrc etc. -->
 <!-- `alias blender="/Applications/Blender.app/Contents/MacOS/Blender"` -->
 <!-- then `source ~/.zshrc` -->
 <!-- 2. `blender myscene.blend --background --python blender.py` -->
 <!-- currently there is no myscene.blend to remove that: `blender --background --python blender.py` -->
 <!-- Select camera: View/Cameras/Active Camera     -->
 <!-- Lock camera to view:   -->
@@ -69,19 +78,32 @@
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
 # Deployment
-- Make sure twine is installed: `python3 -m pip install build twine`
-- Create source archive and wheel: `python3 -m build`
-- Check that it will render properly on PyPi: `twine check dist/*`
-- Upload to PyPi: `twine upload dist/*`
 
+[Instructions for PyPi](https://packaging.python.org/en/latest/tutorials/packaging-projects/) and [API Token](https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#create-an-account).
+
+One time setup:
+```
+vim ~/.pypirc  # put __token__ as username 
+python3 -m pip install build twine
+python3 -m pip install --upgrade build
+```
+
+Upload latest version to pypi:
+```
+vim pyproject.toml  # update version
+rm -rf dist
+rm -rf example_*
+python3 -m build
+python3 -m twine upload --repository testpypi dist/*
+```
 
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
```

### Comparing `pyviz3d-0.3.1/pyproject.toml` & `pyviz3d-0.3.221/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyviz3d"
-version = "0.3.1"
+version = "0.3.221"
 description = "PyViz3D is a python package to visualize 3D scenes."
 readme = "README.md"
 authors = [{ name = "Francis Engelmann", email = "francis.engelmann@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyviz3d-0.3.1/pyviz3d/arrow.py` & `pyviz3d-0.3.221/pyviz3d/arrow.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/camera.py` & `pyviz3d-0.3.221/pyviz3d/camera.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Camera related functionality."""
 import numpy as np
 
 
 class Camera:
     """Camera class looking at the scene"""
 
-    def __init__(self, position, look_at, up, focal_length):
+    def __init__(self, position, look_at, up, focal_length, animation):
         self.position = position.astype(np.float32)
         self.look_at = look_at.astype(np.float32)
         self.up = up.astype(np.float32)
         self.focal_length = float(focal_length)
+        self.animation = animation
 
     def get_properties(self, binary_filename):
         """Get the camera properties, they are written into json and interpreted by javascript.
 
         :return: A dict conteining object properties.
         """
         json_dict = {
             'type': 'camera',
             'position': self.position.tolist(),
             'look_at': self.look_at.tolist(),
             'up': self.up.tolist(),
-            'focal_length': self.focal_length}
+            'focal_length': self.focal_length,
+            'animation': self.animation,
+            }
         return json_dict
 
     def write_binary(self, path):
         """Write camera to binary file."""
         bin_position = self.position.tobytes()
         with open(path, "wb") as f:
             f.write(bin_position)
```

### Comparing `pyviz3d-0.3.1/pyviz3d/circles_2d.py` & `pyviz3d-0.3.221/pyviz3d/circles_2d.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/cuboid.py` & `pyviz3d-0.3.221/pyviz3d/cuboid.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/labels.py` & `pyviz3d-0.3.221/pyviz3d/labels.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/lines.py` & `pyviz3d-0.3.221/pyviz3d/lines.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/mesh.py` & `pyviz3d-0.3.221/pyviz3d/mesh.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/points.py` & `pyviz3d-0.3.221/pyviz3d/points.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/polyline.py` & `pyviz3d-0.3.221/pyviz3d/polyline.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/blender_tools.py` & `pyviz3d-0.3.221/pyviz3d/src/blender_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     cam.constraints["Track To"].target = bpy.data.objects["Point"]
     bpy.ops.constraint.followpath_path_animate(constraint="Follow Path", owner='OBJECT')
 
     output_filepath = os.path.join(path, path.split('/')[-2]+'.mp4')
     subprocess.run(["ffmpeg", "-i", f'{path}/%04d.png', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
     subprocess.run(["ffmpeg", "-i", output_filepath, "-pix_fmt", "rgb24", output_filepath[:-3]+'gif'])
 
+
 def save_blender_scene(path: str) -> None:
   bpy.ops.wm.save_as_mainfile(filepath=path)
 
 
 def compute_object_center(object):
   local_bbox_center = 0.125 * sum((mathutils.Vector(b) for b in object.bound_box),
                                    mathutils.Vector())
@@ -140,14 +141,15 @@
 
   for i in range(4):
     bpy.ops.object.light_add(type='POINT', radius=0.1, align='WORLD', location=(i%2, i//2, 1), scale=(1, 1, 1))
     C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.energy = 5.0
     C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.shadow_soft_size = 0.1
     C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.color = (1, 0.795182, 0.375358)
 
+
 def create_mat(obj, color=None):
     mat = bpy.data.materials.new(name="test")
     mat.use_backface_culling = True
     obj.data.materials.append(mat)
     mat.use_nodes = True
     mat.node_tree.nodes.new(type="ShaderNodeVertexColor")
     mat.node_tree.nodes["Principled BSDF"].inputs[7].default_value = 0  # specular
@@ -157,15 +159,14 @@
     else:
       mat.node_tree.nodes["Color Attribute"].layer_name = "Col"
       mat.node_tree.links.new(
         mat.node_tree.nodes["Principled BSDF"].inputs["Base Color"],
         mat.node_tree.nodes["Color Attribute"].outputs["Color"])
 
 
-
 def cylinder_between(x1, y1, z1, x2, y2, z2, r, color, alpha):
     dx = x2 - x1
     dy = y2 - y1
     dz = z2 - z1    
     dist = math.sqrt(dx**2 + dy**2 + dz**2)
     bpy.ops.mesh.primitive_cylinder_add(
         radius = r, 
@@ -188,29 +189,30 @@
 def main():
     clear_scene()
     init_scene()
 
     path_json = f'nodes.json'
     with open(path_json) as f:
         nodes_dict = json.load(f)
-
+    animation = False
     for name, properties in nodes_dict.items():
         print(name, properties)
         if properties['type'] == 'points':
            bpy.ops.wm.ply_import(filepath=name+'.ply')
            bpy.ops.object.shade_smooth()
            obj = bpy.data.objects[name]
            create_mat(obj)
 
         if properties['type'] == 'camera':
            eye = mathutils.Vector(properties['position'])
            at = mathutils.Vector(properties['look_at'])
            up = mathutils.Vector(properties['up'])
            look_at(C.scene.objects['Camera'], eye, at, up)
            C.scene.objects['Camera'].data.lens = properties['focal_length']
+           animation = properties['animation']
         
         if properties['type'] == 'cuboid':
            obj = bpy.ops.mesh.primitive_cube_add(size=1, enter_editmode=False, align='WORLD',
                                            location=mathutils.Vector(properties['position']),
                                            scale=mathutils.Vector(properties['size']))
         
         if properties['type'] == 'polyline':
@@ -233,17 +235,17 @@
           bpy.ops.object.shade_smooth()
           obj = bpy.data.objects[properties['filename'].split('.')[0]]
           obj.scale = [properties['scale'][0], properties['scale'][1], properties['scale'][2]]
           obj.rotation_mode = 'QUATERNION'  # blender quats are WXYZ
           obj.rotation_quaternion = [properties['rotation'][3], properties['rotation'][0], properties['rotation'][1], properties['rotation'][2]]
           obj.location = [properties['translation'][0], properties['translation'][1], properties['translation'][2]]
           create_mat(obj, properties['color'])
-
+        # somwhere here parse the blender parameters
 
     # Render if output filename is provided
     if len(argv) > 0:
-        render(argv[0])
+        render(argv[0], animation=animation)
 
     output_blender_file = f'blender_scene.blend'
     output_blender_file = os.path.abspath(output_blender_file)
     save_blender_scene(output_blender_file)
     print('Saved blender file to:', output_blender_file)
```

### Comparing `pyviz3d-0.3.1/pyviz3d/src/css/bootstrap.min.css` & `pyviz3d-0.3.221/pyviz3d/src/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/favicon.ico` & `pyviz3d-0.3.221/pyviz3d/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/index.html` & `pyviz3d-0.3.221/pyviz3d/src/index.html`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/js/bootstrap.min.js` & `pyviz3d-0.3.221/pyviz3d/src/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/js/jquery.min.js` & `pyviz3d-0.3.221/pyviz3d/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/src/js/scene.js` & `pyviz3d-0.3.221/pyviz3d/src/js/scene.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.1/pyviz3d/visualizer.py` & `pyviz3d-0.3.221/pyviz3d/visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,40 +32,42 @@
     return q
 
 class Visualizer:
     def __init__(self,
                  position: np.array = np.array([3.0, 3.0, 3.0]),
                  look_at: np.array = np.array([0.0, 0.0, 0.0]),
                  up: np.array = np.array([0.0, 0.0, 1.0]),
-                 focal_length: float = 28.0):
+                 focal_length: float = 28.0, animation=False):
 
         self.camera = Camera(
             position=np.array(position),
             look_at=np.array(look_at),
             up=np.array(up),
-            focal_length=focal_length
+            focal_length=focal_length,
+            animation=animation
         )
         self.elements = {"Camera_0": self.camera}
 
     def __parse_name(self,
                      name: str) -> str:
         """Makes sure the name does not contain invalid character combinations.
 
         :param name:
         :return:
         """
         return name.replace(':', ';')
 
     def save(self,
-             path: str,
-             port: int=6008,
-             show_in_blender: bool=False,
-             blender_output_path=None,
-             blender_executable_path=None,
-             verbose=True):
+            path: str,
+            port: int=6008,
+            blender_args: dict=None,
+            # show_in_blender: bool=False,
+            # blender_output_path=None,
+            # blender_executable_path=None,
+            verbose=True):
         """Creates the visualization and displays the link to it.
 
         :param path: The path to save the visualization files.
         :param port: The port to show the visualization.
         :param verbose: Whether to print the web-server message or not.
         """
 
@@ -80,15 +82,15 @@
 
         # Assemble binary data files
         nodes_dict = {}
         for name, e in self.elements.items():
             binary_file_path = os.path.join(directory_destination, name + ".bin")
             nodes_dict[name] = e.get_properties(name + ".bin")
             e.write_binary(binary_file_path)
-            if show_in_blender:
+            if blender_args:
                 blender_file_oath = os.path.join(directory_destination, name + ".ply")
                 e.write_blender(blender_file_oath)
 
         # Write json file containing all scene elements
         json_file = os.path.join(directory_destination, "nodes.json")
         with open(json_file, "w") as outfile:
             json.dump(nodes_dict, outfile)
@@ -108,36 +110,38 @@
         print("    cd " + directory_destination + "; " + http_server_string)
         print("2) Open in browser:")
         print("    http://localhost:" + str(port))
         print(
             "************************************************************************"
         )
 
-        if show_in_blender:
-            self.show_in_blender(path, blender_output_path, blender_executable_path, verbose)
+        if blender_args:
+            # self.show_in_blender(path, blender_output_path, blender_executable_path, verbose)
+            self.show_in_blender(path, blender_args, verbose)
 
     def show_in_blender(self,
                         path: str,
-                        blender_output_path: str,
-                        blender_executable_path: str,
+                        blender_args: dict,
+                        # blender_output_path: str,
+                        # blender_executable_path: str,
                         verbose: bool=True):
 
         directory_destination = os.path.abspath(path)
         blender_script_path = os.path.join(directory_destination, "blender_script.py")
         with open(blender_script_path, "w") as outfile:
             outfile.write(
 "import bpy\nimport os\n\
 import sys\n\
 sys.path.append(os.getcwd())\n\
 import blender_tools\n\
 blender_tools.main()")
 
-        cmd = "cd " + directory_destination + "; " + blender_executable_path + " --background --python blender_script.py"
-        if blender_output_path:
-            cmd = cmd + " -- " + blender_output_path
+        cmd = "cd " + directory_destination + "; " + blender_args['executable_path'] + " --background --python blender_script.py"
+        if blender_args['executable_path']:
+            cmd = cmd + " -- " + blender_args['executable_path']
         os.system(cmd)
 
         if verbose:
             print("")
             print("************************************************************************")
             print("Blender instructions")
             print(cmd)
```

### Comparing `pyviz3d-0.3.1/pyviz3d.egg-info/PKG-INFO` & `pyviz3d-0.3.221/pyviz3d.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.1
+Version: 0.3.221
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,20 +38,19 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip3 install pyviz3d```
-- [Documentation](https://francisengelmann.github.io/PyViz3D/)
-- [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
-- [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
+- Install: ```python -m pip install pyviz3d```
+- [Examples](#examples)
+- [Deployment](#deployment)
 
-### Examples
+# Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/graph/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_graph.png" />
   <img width="45%" src="docs/img/example_graph_blender.png" />
 </p>
@@ -60,44 +59,54 @@
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_blender.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/blender/index.html)
 <p align="center">
   <img width="45%" src="docs/img/example_blender.png" />
   <img width="45%" src="docs/img/example_blender_blender.png" />
 </p>
 
-Polygon meshes example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+Arrow example.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
 
 Bounding boxes example.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_bounding_boxes.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_bounding_boxes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/bounding_boxes/index.html)
 
-Polyline example.
+Polygon meshes (.obj and .ply).
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_meshes.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_meshes.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/meshes/index.html)
+
+Point clouds, segments and normals.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_normals.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+
+Polylines.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_polylines.py)
 [[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 [<p align="center"><img width="60%" src="docs/img/example_polylines.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/polylines/index.html)
 
-Arrow example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_arrows.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-[<p align="center"><img width="60%" src="docs/img/example_arrows.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/arrows/index.html)
-
-Point clouds and segments example.
-[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_normals.py)
-[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
-[<p align="center"><img width="60%" src="docs/img/example.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/normals/index.html)
+Superquadrics.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_superquadrics.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_superquadrics.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/superquadrics/index.html)
+
+Text Labels.
+[[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_text.py)
+[[Show Demo]](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
+[<p align="center"><img width="60%" src="docs/img/example_text.png" /></p>](https://francisengelmann.github.io/pyviz3d_examples/text/index.html)
 
-# Blender
+<!-- # Blender
 To create beautiful illustrations with blender consider the following points:
 - Install Blender from https://www.blender.org/ (tested version 4.0).
 - Calling `v.save(..., show_in_blender=True)` creates a `.blend` file which you can open in blender.
-- Check `examples/examples_graph.py` for a complete example.
+- Check `examples/examples_graph.py` for a complete example. -->
 <!-- 2. Set up alias in you ~/.bashrc or ~/.zshrc etc. -->
 <!-- `alias blender="/Applications/Blender.app/Contents/MacOS/Blender"` -->
 <!-- then `source ~/.zshrc` -->
 <!-- 2. `blender myscene.blend --background --python blender.py` -->
 <!-- currently there is no myscene.blend to remove that: `blender --background --python blender.py` -->
 <!-- Select camera: View/Cameras/Active Camera     -->
 <!-- Lock camera to view:   -->
@@ -106,19 +115,32 @@
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
 # Deployment
-- Make sure twine is installed: `python3 -m pip install build twine`
-- Create source archive and wheel: `python3 -m build`
-- Check that it will render properly on PyPi: `twine check dist/*`
-- Upload to PyPi: `twine upload dist/*`
 
+[Instructions for PyPi](https://packaging.python.org/en/latest/tutorials/packaging-projects/) and [API Token](https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#create-an-account).
+
+One time setup:
+```
+vim ~/.pypirc  # put __token__ as username 
+python3 -m pip install build twine
+python3 -m pip install --upgrade build
+```
+
+Upload latest version to pypi:
+```
+vim pyproject.toml  # update version
+rm -rf dist
+rm -rf example_*
+python3 -m build
+python3 -m twine upload --repository testpypi dist/*
+```
 
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
```

### Comparing `pyviz3d-0.3.1/pyviz3d.egg-info/SOURCES.txt` & `pyviz3d-0.3.221/pyviz3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

