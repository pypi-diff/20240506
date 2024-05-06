# Comparing `tmp/pyviz3d-0.3.0.tar.gz` & `tmp/pyviz3d-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviz3d-0.3.0.tar", last modified: Sat Mar  9 18:59:08 2024, max compression
+gzip compressed data, was "pyviz3d-0.3.1.tar", last modified: Sun May  5 20:42:58 2024, max compression
```

## Comparing `pyviz3d-0.3.0.tar` & `pyviz3d-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.979757 pyviz3d-0.3.0/
--rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/LICENSE
--rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/MANIFEST.in
--rw-r--r--   0 francis    (501) staff       (20)     6266 2024-03-09 18:59:08.979571 pyviz3d-0.3.0/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)     4461 2024-03-09 16:57:36.000000 pyviz3d-0.3.0/README.md
--rw-r--r--   0 francis    (501) staff       (20)      684 2024-03-09 18:49:33.000000 pyviz3d-0.3.0/pyproject.toml
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.976007 pyviz3d-0.3.0/pyviz3d/
--rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/__init__.py
--rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.0/pyviz3d/arrow.py
--rw-r--r--   0 francis    (501) staff       (20)     1135 2024-03-09 12:06:52.000000 pyviz3d-0.3.0/pyviz3d/camera.py
--rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.0/pyviz3d/circles_2d.py
--rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.0/pyviz3d/cuboid.py
--rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.0/pyviz3d/labels.py
--rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.0/pyviz3d/lines.py
--rw-r--r--   0 francis    (501) staff       (20)     1691 2024-03-09 12:43:48.000000 pyviz3d-0.3.0/pyviz3d/mesh.py
--rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.0/pyviz3d/points.py
--rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.0/pyviz3d/polyline.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.977330 pyviz3d-0.3.0/pyviz3d/src/
--rw-r--r--   0 francis    (501) staff       (20)     7059 2024-03-09 17:00:06.000000 pyviz3d-0.3.0/pyviz3d/src/blender_tools.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.977626 pyviz3d-0.3.0/pyviz3d/src/css/
--rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/src/css/bootstrap.min.css
--rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/src/favicon.ico
--rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/src/index.html
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.978891 pyviz3d-0.3.0/pyviz3d/src/js/
--rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/src/js/bootstrap.min.js
--rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.0/pyviz3d/src/js/jquery.min.js
--rw-r--r--   0 francis    (501) staff       (20)    24441 2024-03-09 11:09:14.000000 pyviz3d-0.3.0/pyviz3d/src/js/scene.js
--rw-r--r--   0 francis    (501) staff       (20)    11418 2024-03-09 15:36:48.000000 pyviz3d-0.3.0/pyviz3d/visualizer.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-03-09 18:59:08.979353 pyviz3d-0.3.0/pyviz3d.egg-info/
--rw-r--r--   0 francis    (501) staff       (20)     6266 2024-03-09 18:59:08.000000 pyviz3d-0.3.0/pyviz3d.egg-info/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)      599 2024-03-09 18:59:08.000000 pyviz3d-0.3.0/pyviz3d.egg-info/SOURCES.txt
--rw-r--r--   0 francis    (501) staff       (20)        1 2024-03-09 18:59:08.000000 pyviz3d-0.3.0/pyviz3d.egg-info/dependency_links.txt
--rw-r--r--   0 francis    (501) staff       (20)        6 2024-03-09 18:59:08.000000 pyviz3d-0.3.0/pyviz3d.egg-info/requires.txt
--rw-r--r--   0 francis    (501) staff       (20)        8 2024-03-09 18:59:08.000000 pyviz3d-0.3.0/pyviz3d.egg-info/top_level.txt
--rw-r--r--   0 francis    (501) staff       (20)       38 2024-03-09 18:59:08.979804 pyviz3d-0.3.0/setup.cfg
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.646658 pyviz3d-0.3.1/
+-rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/LICENSE
+-rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/MANIFEST.in
+-rw-r--r--   0 francis    (501) staff       (20)     6512 2024-05-05 20:42:58.646453 pyviz3d-0.3.1/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)     4707 2024-03-09 19:10:08.000000 pyviz3d-0.3.1/README.md
+-rw-r--r--   0 francis    (501) staff       (20)      684 2024-05-05 20:34:58.000000 pyviz3d-0.3.1/pyproject.toml
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.641844 pyviz3d-0.3.1/pyviz3d/
+-rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/__init__.py
+-rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.1/pyviz3d/arrow.py
+-rw-r--r--   0 francis    (501) staff       (20)     1135 2024-03-09 12:06:52.000000 pyviz3d-0.3.1/pyviz3d/camera.py
+-rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.1/pyviz3d/circles_2d.py
+-rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.1/pyviz3d/cuboid.py
+-rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.1/pyviz3d/labels.py
+-rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.1/pyviz3d/lines.py
+-rw-r--r--   0 francis    (501) staff       (20)     1635 2024-05-05 18:13:27.000000 pyviz3d-0.3.1/pyviz3d/mesh.py
+-rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.1/pyviz3d/points.py
+-rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.1/pyviz3d/polyline.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.643998 pyviz3d-0.3.1/pyviz3d/src/
+-rw-r--r--   0 francis    (501) staff       (20)    10204 2024-05-05 20:18:23.000000 pyviz3d-0.3.1/pyviz3d/src/blender_tools.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.644369 pyviz3d-0.3.1/pyviz3d/src/css/
+-rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/css/bootstrap.min.css
+-rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/favicon.ico
+-rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/index.html
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.645721 pyviz3d-0.3.1/pyviz3d/src/js/
+-rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/js/bootstrap.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.1/pyviz3d/src/js/jquery.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    25452 2024-05-05 19:26:19.000000 pyviz3d-0.3.1/pyviz3d/src/js/scene.js
+-rw-r--r--   0 francis    (501) staff       (20)    16896 2024-05-05 20:03:20.000000 pyviz3d-0.3.1/pyviz3d/visualizer.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-05 20:42:58.646115 pyviz3d-0.3.1/pyviz3d.egg-info/
+-rw-r--r--   0 francis    (501) staff       (20)     6512 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)      599 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/SOURCES.txt
+-rw-r--r--   0 francis    (501) staff       (20)        1 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/dependency_links.txt
+-rw-r--r--   0 francis    (501) staff       (20)        6 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/requires.txt
+-rw-r--r--   0 francis    (501) staff       (20)        8 2024-05-05 20:42:58.000000 pyviz3d-0.3.1/pyviz3d.egg-info/top_level.txt
+-rw-r--r--   0 francis    (501) staff       (20)       38 2024-05-05 20:42:58.646697 pyviz3d-0.3.1/setup.cfg
```

### Comparing `pyviz3d-0.3.0/LICENSE` & `pyviz3d-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/PKG-INFO` & `pyviz3d-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.0
+Version: 0.3.1
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip install pyviz3d```
+- Install: ```pip3 install pyviz3d```
 - [Documentation](https://francisengelmann.github.io/PyViz3D/)
 - [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
 - [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
 
 ### Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
@@ -105,14 +105,21 @@
 <!-- Under View, lock camera to view.   -->
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
+# Deployment
+- Make sure twine is installed: `python3 -m pip install build twine`
+- Create source archive and wheel: `python3 -m build`
+- Check that it will render properly on PyPi: `twine check dist/*`
+- Upload to PyPi: `twine upload dist/*`
+
+
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
   year={2019},
```

### Comparing `pyviz3d-0.3.0/README.md` & `pyviz3d-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip install pyviz3d```
+- Install: ```pip3 install pyviz3d```
 - [Documentation](https://francisengelmann.github.io/PyViz3D/)
 - [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
 - [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
 
 ### Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
@@ -68,14 +68,21 @@
 <!-- Under View, lock camera to view.   -->
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
+# Deployment
+- Make sure twine is installed: `python3 -m pip install build twine`
+- Create source archive and wheel: `python3 -m build`
+- Check that it will render properly on PyPi: `twine check dist/*`
+- Upload to PyPi: `twine upload dist/*`
+
+
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
   year={2019},
```

### Comparing `pyviz3d-0.3.0/pyproject.toml` & `pyviz3d-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyviz3d"
-version = "0.3.0"
+version = "0.3.1"
 description = "PyViz3D is a python package to visualize 3D scenes."
 readme = "README.md"
 authors = [{ name = "Francis Engelmann", email = "francis.engelmann@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyviz3d-0.3.0/pyviz3d/arrow.py` & `pyviz3d-0.3.1/pyviz3d/arrow.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/camera.py` & `pyviz3d-0.3.1/pyviz3d/camera.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/circles_2d.py` & `pyviz3d-0.3.1/pyviz3d/circles_2d.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/cuboid.py` & `pyviz3d-0.3.1/pyviz3d/cuboid.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/labels.py` & `pyviz3d-0.3.1/pyviz3d/labels.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/lines.py` & `pyviz3d-0.3.1/pyviz3d/lines.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/points.py` & `pyviz3d-0.3.1/pyviz3d/points.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/polyline.py` & `pyviz3d-0.3.1/pyviz3d/polyline.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/blender_tools.py` & `pyviz3d-0.3.1/pyviz3d/src/blender_tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,30 +23,61 @@
     if o.type == 'MESH':
         o.select_set(True)
     else:
         o.select_set(False)
   bpy.ops.object.delete()
 
 
-def render(path, file_format='PNG', color_mode='RGBA'):
+def render(path, file_format='PNG', color_mode='RGBA', animation=False):
   """
   :path: the file path of the rendered image
   :file_format: {PNG, JPEG}
   """
   C.scene.render.image_settings.file_format=file_format
   C.scene.render.filepath = path
-
+  print(path)
+  
   # C.scene.view_settings.view_transform = 'Standard'
   # D.worlds["World"].node_tree.nodes["Background"].inputs[0].default_value = (1, 1, 1, 1)
   # bpy.context.scene.world.use_nodes = False
   # bpy.context.scene.world.color = (1, 1, 1)
   # C.scene.render.alpha_mode = 'SKY'
-  bpy.ops.render.render(use_viewport=True, write_still=True)
+  
+  bpy.ops.render.render(use_viewport=True, animation=animation, write_still=True)
+  # bpy.data.scenes['Scene'].render.ffmpeg. 
   print('Saved rendered file to:', os.path.abspath(path))
+  if animation:
 
+    bpy.ops.curve.primitive_bezier_circle_add(radius=1, enter_editmode=False, align='WORLD', location=(0, 0, 0), scale=(1, 1, 1))
+    bpy.context.object.data.path_duration = 100
+    bpy.context.scene.frame_end = 100
+    bpy.context.scene.render.resolution_y = 406
+    bpy.context.scene.render.resolution_x = 720
+    bpy.context.scene.cycles.samples = 10
+    bpy.data.scenes['Scene'].render.ffmpeg.codec = 'H264'
+
+    light = C.scene.objects['Point']
+    light.location = [0.0, 0.0, 0.0]
+    light.data.energy = 60
+    light.data.shadow_soft_size = 0.1
+
+    cam = C.scene.objects['Camera']
+    cam.select_set(True)
+    bpy.context.view_layer.objects.active = cam
+    cam.matrix_world = mathutils.Matrix(np.eye(4))
+    cam.location = [0.0, 0.0, 0.5]
+    bpy.ops.object.constraint_add(type='FOLLOW_PATH')
+    cam.constraints["Follow Path"].target = bpy.data.objects["BezierCircle"]
+    bpy.ops.object.constraint_add(type='TRACK_TO')
+    cam.constraints["Track To"].target = bpy.data.objects["Point"]
+    bpy.ops.constraint.followpath_path_animate(constraint="Follow Path", owner='OBJECT')
+
+    output_filepath = os.path.join(path, path.split('/')[-2]+'.mp4')
+    subprocess.run(["ffmpeg", "-i", f'{path}/%04d.png', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
+    subprocess.run(["ffmpeg", "-i", output_filepath, "-pix_fmt", "rgb24", output_filepath[:-3]+'gif'])
 
 def save_blender_scene(path: str) -> None:
   bpy.ops.wm.save_as_mainfile(filepath=path)
 
 
 def compute_object_center(object):
   local_bbox_center = 0.125 * sum((mathutils.Vector(b) for b in object.bound_box),
@@ -63,66 +94,76 @@
   u = d.cross(r).normalized()
   camera.matrix_world = mathutils.Matrix(((r.x, u.x, d.x, eye.x),
                                           (r.y, u.y, d.y, eye.y),
                                           (r.z, u.z, d.z, eye.z),
                                           (0.0, 0.0, 0.0, 1.0)))
 
 
-def create_video(input_dir, pattern, output_filepath):
-  trans_to_white = "format=yuva444p,\
-  geq=\
-  'if(lte(alpha(X,Y),16),255,p(X,Y))':\
-  'if(lte(alpha(X,Y),16),128,p(X,Y))':\
-  'if(lte(alpha(X,Y),16),128,p(X,Y))'"
-
-  # f = "color=white,format=rgb24[c];[c][0]scale2ref[c][i];[c][i]overlay=format=auto:shortest=1,setsar=1"
-  # cmd = ["ffmpeg", "-i", pattern, '-filter_complex', f, '-y', output_filepath]
-  # subprocess.run(cmd)
-
-  import glob
-  for fi in glob.glob(f'{input_dir}/output_*.png'):
-    subprocess.run(["convert", "-flatten", fi, fi])
-    # subprocess.run(["convert", fi, "-background", "white", "-alpha", "remove", "-flatten", "-alpha", "off", fi])
-  # subprocess.run(["ffmpeg", "-i", pattern, '-y', output_filepath])
-  subprocess.run(["ffmpeg", "-i", f'{input_dir}/{pattern}', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
-  # subprocess.run(["convert", "-delay", "1", "-loop", "0", "*.png", "myimage.gif"])
+# def create_video(input_dir, pattern, output_filepath):
+#   trans_to_white = "format=yuva444p,\
+#   geq=\
+#   'if(lte(alpha(X,Y),16),255,p(X,Y))':\
+#   'if(lte(alpha(X,Y),16),128,p(X,Y))':\
+#   'if(lte(alpha(X,Y),16),128,p(X,Y))'"
+
+#   # f = "color=white,format=rgb24[c];[c][0]scale2ref[c][i];[c][i]overlay=format=auto:shortest=1,setsar=1"
+#   # cmd = ["ffmpeg", "-i", pattern, '-filter_complex', f, '-y', output_filepath]
+#   # subprocess.run(cmd)
+
+#   import glob
+#   for fi in glob.glob(f'{input_dir}/output_*.png'):
+#     subprocess.run(["convert", "-flatten", fi, fi])
+#     # subprocess.run(["convert", fi, "-background", "white", "-alpha", "remove", "-flatten", "-alpha", "off", fi])
+#   # subprocess.run(["ffmpeg", "-i", pattern, '-y', output_filepath])
+#   subprocess.run(["ffmpeg", "-i", f'{input_dir}/{pattern}', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
+#   # subprocess.run(["convert", "-delay", "1", "-loop", "0", "*.png", "myimage.gif"])
 
 
 def init_scene(resolution_x=800, resolution_y=600):
   # render stuff
   C.scene.render.resolution_x = resolution_x
   C.scene.render.resolution_y = resolution_y
   D.scenes["Scene"].render.film_transparent = True
   C.scene.render.image_settings.color_mode = 'RGBA'
   C.scene.view_settings.look = 'AgX - Medium High Contrast'
   C.scene.view_settings.view_transform = 'Standard'
   C.scene.render.engine = 'CYCLES'
   C.scene.cycles.device = 'GPU'
-  C.scene.cycles.preview_samples = 100
-  C.scene.cycles.samples = 150
-  C.scene.frame_end = 60
+  C.scene.cycles.preview_samples = 50
+  C.scene.cycles.samples = 50
+
   # Add lights
   C.scene.objects['Light'].data.shadow_soft_size = 1.0
   C.scene.objects['Light'].data.cycles.cast_shadow = False
   bpy.ops.object.light_add(type='POINT', radius=1, align='WORLD', location=(-1, 1, 10), scale=(1, 1, 1))
   C.scene.objects['Point'].data.energy = 7000.0
   C.scene.objects['Point'].data.shadow_soft_size = 3
 
+  for i in range(4):
+    bpy.ops.object.light_add(type='POINT', radius=0.1, align='WORLD', location=(i%2, i//2, 1), scale=(1, 1, 1))
+    C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.energy = 5.0
+    C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.shadow_soft_size = 0.1
+    C.scene.objects[f'Point.{str(i+1).zfill(3)}'].data.color = (1, 0.795182, 0.375358)
 
-def create_mat(obj):
+def create_mat(obj, color=None):
     mat = bpy.data.materials.new(name="test")
     mat.use_backface_culling = True
     obj.data.materials.append(mat)
     mat.use_nodes = True
     mat.node_tree.nodes.new(type="ShaderNodeVertexColor")
-    mat.node_tree.nodes["Color Attribute"].layer_name = "Col"
-    mat.node_tree.links.new(
-      mat.node_tree.nodes["Principled BSDF"].inputs["Base Color"],
-      mat.node_tree.nodes["Color Attribute"].outputs["Color"])
     mat.node_tree.nodes["Principled BSDF"].inputs[7].default_value = 0  # specular
+    mat.node_tree.nodes["Principled BSDF"].inputs[12].default_value = 0  #
+    if color:
+      mat.node_tree.nodes["Principled BSDF"].inputs[0].default_value = (color[0]/255.0, color[1]/255.0, color[2]/255.0, 1.0)
+    else:
+      mat.node_tree.nodes["Color Attribute"].layer_name = "Col"
+      mat.node_tree.links.new(
+        mat.node_tree.nodes["Principled BSDF"].inputs["Base Color"],
+        mat.node_tree.nodes["Color Attribute"].outputs["Color"])
+
 
 
 def cylinder_between(x1, y1, z1, x2, y2, z2, r, color, alpha):
     dx = x2 - x1
     dy = y2 - y1
     dz = z2 - z1    
     dist = math.sqrt(dx**2 + dy**2 + dz**2)
@@ -155,37 +196,54 @@
     for name, properties in nodes_dict.items():
         print(name, properties)
         if properties['type'] == 'points':
            bpy.ops.wm.ply_import(filepath=name+'.ply')
            bpy.ops.object.shade_smooth()
            obj = bpy.data.objects[name]
            create_mat(obj)
+
         if properties['type'] == 'camera':
            eye = mathutils.Vector(properties['position'])
            at = mathutils.Vector(properties['look_at'])
            up = mathutils.Vector(properties['up'])
            look_at(C.scene.objects['Camera'], eye, at, up)
            C.scene.objects['Camera'].data.lens = properties['focal_length']
+        
         if properties['type'] == 'cuboid':
            obj = bpy.ops.mesh.primitive_cube_add(size=1, enter_editmode=False, align='WORLD',
                                            location=mathutils.Vector(properties['position']),
                                            scale=mathutils.Vector(properties['size']))
+        
         if properties['type'] == 'polyline':
             if len(properties['positions']) <= 1:
                 continue
             for i in range(len(properties['positions']) - 1):
                 x1 = properties['positions'][i][0]
                 y1 = properties['positions'][i][1]
                 z1 = properties['positions'][i][2]
                 x2 = properties['positions'][i + 1][0]
                 y2 = properties['positions'][i + 1][1]
                 z2 = properties['positions'][i + 1][2]
                 obj = cylinder_between(x1, y1, z1, x2, y2, z2, properties['edge_width'] * 2, properties['color'], properties['alpha'])
+        
+        if properties['type'] == 'mesh':
+          if properties['filename'].split('.')[-1] == 'ply':
+            bpy.ops.wm.ply_import(filepath=properties['filename'], forward_axis='Y', up_axis='Z')
+          if properties['filename'].split('.')[-1] == 'obj':
+            bpy.ops.wm.obj_import(filepath=properties['filename'], forward_axis='Y', up_axis='Z')          
+          bpy.ops.object.shade_smooth()
+          obj = bpy.data.objects[properties['filename'].split('.')[0]]
+          obj.scale = [properties['scale'][0], properties['scale'][1], properties['scale'][2]]
+          obj.rotation_mode = 'QUATERNION'  # blender quats are WXYZ
+          obj.rotation_quaternion = [properties['rotation'][3], properties['rotation'][0], properties['rotation'][1], properties['rotation'][2]]
+          obj.location = [properties['translation'][0], properties['translation'][1], properties['translation'][2]]
+          create_mat(obj, properties['color'])
 
-    output_blender_file = f'blender_scene.blend'
+
+    # Render if output filename is provided
     if len(argv) > 0:
         render(argv[0])
 
+    output_blender_file = f'blender_scene.blend'
     output_blender_file = os.path.abspath(output_blender_file)
     save_blender_scene(output_blender_file)
     print('Saved blender file to:', output_blender_file)
-
```

### Comparing `pyviz3d-0.3.0/pyviz3d/src/css/bootstrap.min.css` & `pyviz3d-0.3.1/pyviz3d/src/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/favicon.ico` & `pyviz3d-0.3.1/pyviz3d/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/index.html` & `pyviz3d-0.3.1/pyviz3d/src/index.html`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/js/bootstrap.min.js` & `pyviz3d-0.3.1/pyviz3d/src/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/js/jquery.min.js` & `pyviz3d-0.3.1/pyviz3d/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.0/pyviz3d/src/js/scene.js` & `pyviz3d-0.3.1/pyviz3d/src/js/scene.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,17 @@
 import {
     OrbitControls
 } from 'three/addons/controls/OrbitControls.js';
 import {
     OBJLoader
 } from 'three/addons/loaders/OBJLoader.js';
 import {
+    PLYLoader
+} from 'three/addons/loaders/PLYLoader.js';
+import {
     GUI
 } from 'three/addons/libs/lil-gui.module.min.js';
 import {
     CSS2DRenderer,
     CSS2DObject
 } from 'three/addons/renderers/CSS2DRenderer.js';
 
@@ -206,57 +209,71 @@
         const label_2d = new CSS2DObject(labelDiv);
         label_2d.position.set(properties['positions'][i][0], properties['positions'][i][1], properties['positions'][i][2]);
         labels.add(label_2d);
     }
     return labels
 }
 
-function get_obj(properties) {
+function get_mesh(properties) {
     var container = new THREE.Object3D();
 
-    function loadModel(object) {
-        object.traverse(
-            function(child) {
-                if (child.isMesh) {
-                    let r = properties['color'][0]
-                    let g = properties['color'][1]
-                    let b = properties['color'][2]
-                    let colorString = "rgb(" + r + "," + g + ", " + b + ")"
-                    child.material.color.set(new THREE.Color(colorString));
-                }
-            });
-        object.translateX(properties['translation'][0])
-        object.translateY(properties['translation'][1])
-        object.translateZ(properties['translation'][2])
-
-        const q = new THREE.Quaternion(
-            properties['rotation'][1],
-            properties['rotation'][2],
-            properties['rotation'][3],
-            properties['rotation'][0])
-        object.setRotationFromQuaternion(q)
+    function loadModel(geometry) {
+        let object;
+        let r = properties['color'][0]
+        let g = properties['color'][1]
+        let b = properties['color'][2]
+        let colorString = "rgb(" + r + "," + g + ", " + b + ")"
+        if (geometry.isObject3D) { // obj
+            object = geometry;
+            object.traverse(
+                function(child) {
+                    if (child.isMesh) {
+                        child.material.color.set(new THREE.Color(colorString));
+                    }
+                });
+        } else { // ply
+            const materialShader = (geometry.hasAttribute('normal')) ? THREE.MeshPhongMaterial : THREE.MeshBasicMaterial
+            const material = new materialShader({
+                vertexColors: geometry.hasAttribute('color')
+            })
+            if (!geometry.hasAttribute) {
+                material.color.set(new THREE.Color(colorString));
+            }
+            object = new THREE.Mesh(geometry, material);
+        }
 
         object.scale.set(properties['scale'][0], properties['scale'][1], properties['scale'][2])
-
+        object.setRotationFromQuaternion(new THREE.Quaternion(properties['rotation'][0], properties['rotation'][1], properties['rotation'][2], properties['rotation'][3]))
+        object.position.set(properties['translation'][0], properties['translation'][1], properties['translation'][2])
         container.add(object)
         step_progress_bar();
         render();
     }
+    const filename_extension = properties['filename'].split('.').pop()
+    console.log(filename_extension)
 
-    const loader = new OBJLoader();
+    let loader;
+    if (filename_extension === 'ply') {
+        loader = new PLYLoader();
+    } else if (filename_extension === 'obj') {
+        loader = new OBJLoader();
+    } else {
+        console.log('Unknown mesh extension: ' + filename_extension);
+    }
     loader.load(properties['filename'], loadModel,
         function(xhr) { // called when loading is in progresses
             console.log((xhr.loaded / xhr.total * 100) + '% loaded');
         },
         function(error) { // called when loading has errors
-            console.log('An error happened');
+            console.log('An error happened: ' + error);
         });
     return container
 }
 
+
 function get_material(alpha) {
     let uniforms = {
         alpha: {
             value: alpha
         },
         shading_type: {
             value: 1
@@ -384,18 +401,18 @@
     cuboid.add(corner_03)
     cuboid.add(corner_10)
     cuboid.add(corner_11)
     cuboid.add(corner_12)
     cuboid.add(corner_13)
 
     const q = new THREE.Quaternion(
+        properties['orientation'][0],
         properties['orientation'][1],
         properties['orientation'][2],
-        properties['orientation'][3],
-        properties['orientation'][0])
+        properties['orientation'][3])
     cuboid.setRotationFromQuaternion(q)
     cuboid.position.set(properties['position'][0], properties['position'][1], properties['position'][2])
     return cuboid
 }
 
 function get_polyline(properties) {
     const radius_top = properties['edge_width']
@@ -587,14 +604,20 @@
         if (String(object_properties['type']).localeCompare('lines') == 0) {
             threejs_objects[object_name] = get_lines(object_properties);
             render();
         }
         if (String(object_properties['type']).localeCompare('obj') == 0) {
             threejs_objects[object_name] = get_obj(object_properties);
         }
+        if (String(object_properties['type']).localeCompare('ply') == 0) {
+            threejs_objects[object_name] = get_ply(object_properties);
+        }
+        if (String(object_properties['type']).localeCompare('mesh') == 0) {
+            threejs_objects[object_name] = get_mesh(object_properties);
+        }
         if (String(object_properties['type']).localeCompare('cuboid') == 0) {
             threejs_objects[object_name] = get_cuboid(object_properties);
             step_progress_bar();
             render();
         }
         if (String(object_properties['type']).localeCompare('polyline') == 0) {
             threejs_objects[object_name] = get_polyline(object_properties);
```

### Comparing `pyviz3d-0.3.0/pyviz3d/visualizer.py` & `pyviz3d-0.3.1/pyviz3d/visualizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,29 @@
 from .circles_2d import Circles2D
 
 import os
 import sys
 import shutil
 import json
 import numpy as np
+import open3d as o3d
 
+def euler_to_quaternion(x: float, y: float, z: float):
+    cr = np.cos(x * 0.5)
+    sr = np.sin(x * 0.5)
+    cp = np.cos(y * 0.5)
+    sp = np.sin(y * 0.5)
+    cy = np.cos(z * 0.5)
+    sy = np.sin(z * 0.5)
+    q = np.zeros([4])
+    q[0] = sr * cp * cy - cr * sp * sy  # x
+    q[1] = cr * sp * cy + sr * cp * sy  # y
+    q[2] = cr * cp * sy - sr * sp * cy  # z
+    q[3] = cr * cp * cy + sr * sp * sy  # w
+    return q
 
 class Visualizer:
     def __init__(self,
                  position: np.array = np.array([3.0, 3.0, 3.0]),
                  look_at: np.array = np.array([0.0, 0.0, 0.0]),
                  up: np.array = np.array([0.0, 0.0, 1.0]),
                  focal_length: float = 28.0):
@@ -234,28 +248,28 @@
         lines_end = lines_end.astype(np.float32)
         self.elements[self.__parse_name(name)] = Lines(lines_start, lines_end, colors, colors, visible)
 
     def add_bounding_box(self,
                          name: str,
                          position: np.array,
                          size: np.array,
-                         rotation: np.array=np.array([1.0, 0.0, 0.0, 0.0]),
+                         rotation: np.array=np.array([0.0, 0.0, 0.0, 1.0]),
                          color: np.array=np.array([255, 0, 0]),
                          alpha: float=1.0,
                          edge_width: float=0.01,
                          visible: bool=True):
         """Add oriented 3D bounding box."""
         rotation /= np.linalg.norm(rotation)  # normalize the orientation
         self.elements[self.__parse_name(name)] = Cuboid(position, size, rotation, color, alpha, edge_width, visible)
 
     def add_mesh(self,
                  name: str,
                  path: str,
                  translation: np.array=np.array([0.0, 0.0, 0.0]),
-                 rotation: np.array=np.array([0, 0, 0, 1]),
+                 rotation: np.array=np.array([0.0, 0.0, 0.0, 1.0]),  # [x, y, z, w] - rotate w degrees rad around the axis xyz
                  scale: np.array=np.array([1, 1, 1]),
                  color: np.array=np.array([255, 255, 255]),
                  visible: bool=True):
         """Adds a polygon mesh to the scene as specified in the path.
          
           The path is currently limited to .obj files and the color is the uniform color of the objetc.
         """
@@ -277,14 +291,113 @@
         :param alpha: The transparency. (float32)
         :param edge_width: The width of the edges. (float32)
         :param visible: Bool, whether visible or not.
         """
 
         self.elements[self.__parse_name(name)] = Polyline(positions, color, alpha, edge_width, visible)
 
+    def add_superquadric(self,
+        name: str,
+        scalings: np.array=np.array([1.0, 1.0, 1.0]),
+        exponents: np.array=np.array([2.0, 2.0, 2.0]),
+        translation: np.array=np.array([0.0, 0.0, 0.0]),
+        rotation: np.array=np.array([1.0, 0.0, 0.0, 0.0]),
+        color: np.array=np.array([255, 255, 255]),
+        resolution: int=30,
+        visible: bool=True):
+        """Adds a superqiadroc mesh to the scene."""
+
+        def create_superquadric_mesh(A, B, C, r, s, t, N):
+            def f(o, m):
+                return np.sign(np.sin(o)) * np.abs(np.sin(o))**m
+            def g(o, m):
+                return np.sign(np.cos(o)) * np.abs(np.cos(o))**m
+            u = np.linspace(-np.pi, np.pi, N, endpoint=True)
+            v = np.linspace(-np.pi/2.0, np.pi/2.0, N, endpoint=True)
+            u = np.tile(u, N)
+            v = np.repeat(v, N)
+            triangles = []
+
+            x = A * g(v, 2.0 / r) * g(u, 2.0 / r)
+            y = B * g(v, 2.0 / s) * f(u, 2.0 / s)
+            z = C * f(v, 2.0 / t)
+            vertices =  np.concatenate([np.expand_dims(x, 1),
+                                        np.expand_dims(y, 1),
+                                        np.expand_dims(z, 1)], axis=1)
+            triangles = []
+            for i in range(N-1):
+                for j in range(N-1):
+                    triangles.append([i*N+j, (i+1)*N+j+1, (i+1)*N+j])
+                    triangles.append([i*N+j, i*N+(j+1), (i+1)*N+(j+1)])
+            return vertices, triangles
+
+        vertices, triangles = create_superquadric_mesh(scalings[0], scalings[1], scalings[2],
+                                                       exponents[0], exponents[1], exponents[2],
+                                                       resolution)
+        mesh_sq = o3d.geometry.TriangleMesh()
+        mesh_sq.vertices = o3d.utility.Vector3dVector(vertices)
+        mesh_sq.triangles = o3d.utility.Vector3iVector(triangles)
+        o3d.io.write_triangle_mesh(f"{name}.obj", mesh_sq, write_ascii=True, compressed=False, write_vertex_normals=False, write_vertex_colors=False, write_triangle_uvs=False, print_progress=False)
+
+        rotation /= np.linalg.norm(rotation)  # normalize the orientation
+        scale = np.array([1.0, 1.0, 1.0])
+        self.elements[self.__parse_name(name)] = Mesh(f"{name}.obj", translation=translation, rotation=rotation, scale=scale, color=color, visible=visible)
+
+    def add_superquadric_rot_mat(self,
+        name: str,
+        scalings: np.array=np.array([1.0, 1.0, 1.0]),
+        exponents: np.array=np.array([2.0, 2.0, 2.0]),
+        translation: np.array=np.array([0.0, 0.0, 0.0]),
+        rotation: np.array=np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 0.0],[0.0, 0.0,1.0]]),
+        color: np.array=np.array([255, 255, 255]),
+        resolution: int=30,
+        visible: bool=True):
+        """Adds a superqiadroc mesh to the scene."""
+
+        def create_superquadric_mesh(A, B, C, r, s, t, N):
+            def f(o, m):
+                return np.sign(np.sin(o)) * np.abs(np.sin(o))**m
+            def g(o, m):
+                return np.sign(np.cos(o)) * np.abs(np.cos(o))**m
+            u = np.linspace(-np.pi, np.pi, N, endpoint=True)
+            v = np.linspace(-np.pi/2.0, np.pi/2.0, N, endpoint=True)
+            u = np.tile(u, N)
+            v = np.repeat(v, N)
+            triangles = []
+
+            x = A * g(v, 2.0 / r) * g(u, 2.0 / r)
+            y = B * g(v, 2.0 / s) * f(u, 2.0 / s)
+            z = C * f(v, 2.0 / t)
+            vertices =  np.concatenate([np.expand_dims(x, 1),
+                                        np.expand_dims(y, 1),
+                                        np.expand_dims(z, 1)], axis=1)
+            vertices = vertices @ rotation # apply rotation 
+
+            triangles = []
+            for i in range(N-1):
+                for j in range(N-1):
+                    triangles.append([i*N+j, (i+1)*N+j+1, (i+1)*N+j])
+                    triangles.append([i*N+j, i*N+(j+1), (i+1)*N+(j+1)])
+            return vertices, triangles
+
+        vertices, triangles = create_superquadric_mesh(scalings[0], scalings[1], scalings[2],
+                                                    exponents[0], exponents[1], exponents[2],
+                                                    resolution)
+
+        mesh_sq = o3d.geometry.TriangleMesh()
+        mesh_sq.vertices = o3d.utility.Vector3dVector(vertices)
+        mesh_sq.triangles = o3d.utility.Vector3iVector(triangles)
+        if not os.path.exists("objs"):
+            os.makedirs("objs")
+        o3d.io.write_triangle_mesh(f"objs/{name}.obj", mesh_sq, write_ascii=True, compressed=False, write_vertex_normals=False, write_vertex_colors=False, write_triangle_uvs=False, print_progress=False)
+        
+        id_rot_quat = np.array([1,0,0,0])
+        scale = np.array([1.0, 1.0, 1.0])
+        self.elements[self.__parse_name(name)] = Mesh(f"objs/{name}.obj", translation=translation, rotation=id_rot_quat, scale=scale, color=color, visible=visible)
+
     def add_arrow(self,
                   name:str,
                   start: np.array,
                   end: np.array,
                   color: np.array=np.array([255, 0, 0]),
                   alpha: float=1.0,
                   stroke_width: float=0.01,
```

### Comparing `pyviz3d-0.3.0/pyviz3d.egg-info/PKG-INFO` & `pyviz3d-0.3.1/pyviz3d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.0
+Version: 0.3.1
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 <p align="center"><img width="40%" src="docs/img/pyviz3d-logo.png" /></p>
 
 ----
 PyViz3D is a python package to visualize 3D scenes directly in your browser, and create beautiful renderings with blender.
 
 #### Links
 
-- Install: ```pip install pyviz3d```
+- Install: ```pip3 install pyviz3d```
 - [Documentation](https://francisengelmann.github.io/PyViz3D/)
 - [Examples](https://github.com/francisengelmann/PyViz3D/tree/master/examples)
 - [Blender Instructions](https://github.com/francisengelmann/PyViz3D/tree/master?tab=readme-ov-file#blender)
 
 ### Examples
 Scene graph example, including blender rendering.
 [[Show Code]](https://github.com/francisengelmann/PyViz3D/blob/master/examples/example_graph.py)
@@ -105,14 +105,21 @@
 <!-- Under View, lock camera to view.   -->
 <!-- Control the camera with the small coordinate frame on the top right. -->
 <!-- 5. This will render an `output.png` -->
 <!-- 6. The scene can also be opened in blender `bunny.blend` -->
 <!-- 7. Need to install ffmpeg and convert (on mac via brew)   -->
 <!-- brew install ffmpeg -->
 
+# Deployment
+- Make sure twine is installed: `python3 -m pip install build twine`
+- Create source archive and wheel: `python3 -m build`
+- Check that it will render properly on PyPi: `twine check dist/*`
+- Upload to PyPi: `twine upload dist/*`
+
+
 # BibTeX
 Please consider citing PyViz3D in your publications if it helps your research.
 ```
 @misc{engelmann2019pyviz3d,
   title={PyViz3D},
   author={Francis Engelmann},
   year={2019},
```

### Comparing `pyviz3d-0.3.0/pyviz3d.egg-info/SOURCES.txt` & `pyviz3d-0.3.1/pyviz3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

