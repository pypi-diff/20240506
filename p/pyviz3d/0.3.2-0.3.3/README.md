# Comparing `tmp/pyviz3d-0.3.2.tar.gz` & `tmp/pyviz3d-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviz3d-0.3.2.tar", last modified: Mon May  6 17:42:57 2024, max compression
+gzip compressed data, was "pyviz3d-0.3.3.tar", last modified: Mon May  6 18:39:54 2024, max compression
```

## Comparing `pyviz3d-0.3.2.tar` & `pyviz3d-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.146322 pyviz3d-0.3.2/
--rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/LICENSE
--rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/MANIFEST.in
--rw-r--r--   0 francis    (501) staff       (20)     7358 2024-05-06 17:42:57.146094 pyviz3d-0.3.2/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)     5553 2024-05-06 16:20:27.000000 pyviz3d-0.3.2/README.md
--rw-r--r--   0 francis    (501) staff       (20)      684 2024-05-06 17:40:05.000000 pyviz3d-0.3.2/pyproject.toml
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.140814 pyviz3d-0.3.2/pyviz3d/
--rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/__init__.py
--rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.2/pyviz3d/arrow.py
--rw-r--r--   0 francis    (501) staff       (20)     1236 2024-05-06 17:21:54.000000 pyviz3d-0.3.2/pyviz3d/camera.py
--rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.2/pyviz3d/circles_2d.py
--rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.2/pyviz3d/cuboid.py
--rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.2/pyviz3d/labels.py
--rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.2/pyviz3d/lines.py
--rw-r--r--   0 francis    (501) staff       (20)     1635 2024-05-05 18:13:27.000000 pyviz3d-0.3.2/pyviz3d/mesh.py
--rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.2/pyviz3d/points.py
--rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.2/pyviz3d/polyline.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.142642 pyviz3d-0.3.2/pyviz3d/src/
--rw-r--r--   0 francis    (501) staff       (20)    10346 2024-05-06 17:23:06.000000 pyviz3d-0.3.2/pyviz3d/src/blender_tools.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.142929 pyviz3d-0.3.2/pyviz3d/src/css/
--rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/src/css/bootstrap.min.css
--rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/src/favicon.ico
--rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/src/index.html
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.145412 pyviz3d-0.3.2/pyviz3d/src/js/
--rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/src/js/bootstrap.min.js
--rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.2/pyviz3d/src/js/jquery.min.js
--rw-r--r--   0 francis    (501) staff       (20)    25452 2024-05-05 19:26:19.000000 pyviz3d-0.3.2/pyviz3d/src/js/scene.js
--rw-r--r--   0 francis    (501) staff       (20)    17121 2024-05-06 17:19:59.000000 pyviz3d-0.3.2/pyviz3d/visualizer.py
-drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 17:42:57.145822 pyviz3d-0.3.2/pyviz3d.egg-info/
--rw-r--r--   0 francis    (501) staff       (20)     7358 2024-05-06 17:42:57.000000 pyviz3d-0.3.2/pyviz3d.egg-info/PKG-INFO
--rw-r--r--   0 francis    (501) staff       (20)      599 2024-05-06 17:42:57.000000 pyviz3d-0.3.2/pyviz3d.egg-info/SOURCES.txt
--rw-r--r--   0 francis    (501) staff       (20)        1 2024-05-06 17:42:57.000000 pyviz3d-0.3.2/pyviz3d.egg-info/dependency_links.txt
--rw-r--r--   0 francis    (501) staff       (20)        6 2024-05-06 17:42:57.000000 pyviz3d-0.3.2/pyviz3d.egg-info/requires.txt
--rw-r--r--   0 francis    (501) staff       (20)        8 2024-05-06 17:42:57.000000 pyviz3d-0.3.2/pyviz3d.egg-info/top_level.txt
--rw-r--r--   0 francis    (501) staff       (20)       38 2024-05-06 17:42:57.146365 pyviz3d-0.3.2/setup.cfg
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.836043 pyviz3d-0.3.3/
+-rw-r--r--   0 francis    (501) staff       (20)     1104 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/LICENSE
+-rw-r--r--   0 francis    (501) staff       (20)       65 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/MANIFEST.in
+-rw-r--r--   0 francis    (501) staff       (20)     7358 2024-05-06 18:39:54.835808 pyviz3d-0.3.3/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)     5553 2024-05-06 16:20:27.000000 pyviz3d-0.3.3/README.md
+-rw-r--r--   0 francis    (501) staff       (20)      684 2024-05-06 18:37:20.000000 pyviz3d-0.3.3/pyproject.toml
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.831366 pyviz3d-0.3.3/pyviz3d/
+-rw-r--r--   0 francis    (501) staff       (20)        0 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/__init__.py
+-rw-r--r--   0 francis    (501) staff       (20)     1143 2024-03-09 12:28:48.000000 pyviz3d-0.3.3/pyviz3d/arrow.py
+-rw-r--r--   0 francis    (501) staff       (20)     1236 2024-05-06 17:21:54.000000 pyviz3d-0.3.3/pyviz3d/camera.py
+-rw-r--r--   0 francis    (501) staff       (20)     1266 2024-02-29 09:08:24.000000 pyviz3d-0.3.3/pyviz3d/circles_2d.py
+-rw-r--r--   0 francis    (501) staff       (20)     1168 2024-03-09 12:18:04.000000 pyviz3d-0.3.3/pyviz3d/cuboid.py
+-rw-r--r--   0 francis    (501) staff       (20)     1060 2024-03-09 12:21:05.000000 pyviz3d-0.3.3/pyviz3d/labels.py
+-rw-r--r--   0 francis    (501) staff       (20)     1501 2024-03-09 12:38:54.000000 pyviz3d-0.3.3/pyviz3d/lines.py
+-rw-r--r--   0 francis    (501) staff       (20)     1635 2024-05-05 18:13:27.000000 pyviz3d-0.3.3/pyviz3d/mesh.py
+-rw-r--r--   0 francis    (501) staff       (20)     2350 2024-03-01 13:43:38.000000 pyviz3d-0.3.3/pyviz3d/points.py
+-rw-r--r--   0 francis    (501) staff       (20)      935 2024-03-01 13:14:50.000000 pyviz3d-0.3.3/pyviz3d/polyline.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.833094 pyviz3d-0.3.3/pyviz3d/src/
+-rw-r--r--   0 francis    (501) staff       (20)    10378 2024-05-06 18:31:38.000000 pyviz3d-0.3.3/pyviz3d/src/blender_tools.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.833431 pyviz3d-0.3.3/pyviz3d/src/css/
+-rw-r--r--   0 francis    (501) staff       (20)   194856 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/src/css/bootstrap.min.css
+-rw-r--r--   0 francis    (501) staff       (20)     1406 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/src/favicon.ico
+-rw-r--r--   0 francis    (501) staff       (20)     4889 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/src/index.html
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.834857 pyviz3d-0.3.3/pyviz3d/src/js/
+-rw-r--r--   0 francis    (501) staff       (20)    60363 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/src/js/bootstrap.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    89664 2023-09-12 17:27:05.000000 pyviz3d-0.3.3/pyviz3d/src/js/jquery.min.js
+-rw-r--r--   0 francis    (501) staff       (20)    25452 2024-05-05 19:26:19.000000 pyviz3d-0.3.3/pyviz3d/src/js/scene.js
+-rw-r--r--   0 francis    (501) staff       (20)    16786 2024-05-06 18:22:46.000000 pyviz3d-0.3.3/pyviz3d/visualizer.py
+drwxr-xr-x   0 francis    (501) staff       (20)        0 2024-05-06 18:39:54.835306 pyviz3d-0.3.3/pyviz3d.egg-info/
+-rw-r--r--   0 francis    (501) staff       (20)     7358 2024-05-06 18:39:54.000000 pyviz3d-0.3.3/pyviz3d.egg-info/PKG-INFO
+-rw-r--r--   0 francis    (501) staff       (20)      599 2024-05-06 18:39:54.000000 pyviz3d-0.3.3/pyviz3d.egg-info/SOURCES.txt
+-rw-r--r--   0 francis    (501) staff       (20)        1 2024-05-06 18:39:54.000000 pyviz3d-0.3.3/pyviz3d.egg-info/dependency_links.txt
+-rw-r--r--   0 francis    (501) staff       (20)        6 2024-05-06 18:39:54.000000 pyviz3d-0.3.3/pyviz3d.egg-info/requires.txt
+-rw-r--r--   0 francis    (501) staff       (20)        8 2024-05-06 18:39:54.000000 pyviz3d-0.3.3/pyviz3d.egg-info/top_level.txt
+-rw-r--r--   0 francis    (501) staff       (20)       38 2024-05-06 18:39:54.836092 pyviz3d-0.3.3/setup.cfg
```

### Comparing `pyviz3d-0.3.2/LICENSE` & `pyviz3d-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/PKG-INFO` & `pyviz3d-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyviz3d-0.3.2/README.md` & `pyviz3d-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyproject.toml` & `pyviz3d-0.3.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyviz3d"
-version = "0.3.2"
+version = "0.3.3"
 description = "PyViz3D is a python package to visualize 3D scenes."
 readme = "README.md"
 authors = [{ name = "Francis Engelmann", email = "francis.engelmann@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyviz3d-0.3.2/pyviz3d/arrow.py` & `pyviz3d-0.3.3/pyviz3d/arrow.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/camera.py` & `pyviz3d-0.3.3/pyviz3d/camera.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/circles_2d.py` & `pyviz3d-0.3.3/pyviz3d/circles_2d.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/cuboid.py` & `pyviz3d-0.3.3/pyviz3d/cuboid.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/labels.py` & `pyviz3d-0.3.3/pyviz3d/labels.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/lines.py` & `pyviz3d-0.3.3/pyviz3d/lines.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/mesh.py` & `pyviz3d-0.3.3/pyviz3d/mesh.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/points.py` & `pyviz3d-0.3.3/pyviz3d/points.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/polyline.py` & `pyviz3d-0.3.3/pyviz3d/polyline.py`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/blender_tools.py` & `pyviz3d-0.3.3/pyviz3d/src/blender_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,37 +23,34 @@
     if o.type == 'MESH':
         o.select_set(True)
     else:
         o.select_set(False)
   bpy.ops.object.delete()
 
 
-def render(path, file_format='PNG', color_mode='RGBA', animation=False):
+def render(output_prefix, file_format='PNG', color_mode='RGBA', animation=False):
   """
   :path: the file path of the rendered image
   :file_format: {PNG, JPEG}
   """
   C.scene.render.image_settings.file_format=file_format
-  C.scene.render.filepath = path
-  print(path)
+  C.scene.render.filepath = output_prefix
+  print('output_prefix:', output_prefix)
   
   # C.scene.view_settings.view_transform = 'Standard'
   # D.worlds["World"].node_tree.nodes["Background"].inputs[0].default_value = (1, 1, 1, 1)
   # bpy.context.scene.world.use_nodes = False
   # bpy.context.scene.world.color = (1, 1, 1)
   # C.scene.render.alpha_mode = 'SKY'
   
-  bpy.ops.render.render(use_viewport=True, animation=animation, write_still=True)
-  # bpy.data.scenes['Scene'].render.ffmpeg. 
-  print('Saved rendered file to:', os.path.abspath(path))
   if animation:
-
     bpy.ops.curve.primitive_bezier_circle_add(radius=1, enter_editmode=False, align='WORLD', location=(0, 0, 0), scale=(1, 1, 1))
-    bpy.context.object.data.path_duration = 100
-    bpy.context.scene.frame_end = 100
+    animation_length = 60
+    bpy.context.object.data.path_duration = animation_length
+    bpy.context.scene.frame_end = animation_length
     bpy.context.scene.render.resolution_y = 406
     bpy.context.scene.render.resolution_x = 720
     bpy.context.scene.cycles.samples = 10
     bpy.data.scenes['Scene'].render.ffmpeg.codec = 'H264'
 
     light = C.scene.objects['Point']
     light.location = [0.0, 0.0, 0.0]
@@ -67,16 +64,19 @@
     cam.location = [0.0, 0.0, 0.5]
     bpy.ops.object.constraint_add(type='FOLLOW_PATH')
     cam.constraints["Follow Path"].target = bpy.data.objects["BezierCircle"]
     bpy.ops.object.constraint_add(type='TRACK_TO')
     cam.constraints["Track To"].target = bpy.data.objects["Point"]
     bpy.ops.constraint.followpath_path_animate(constraint="Follow Path", owner='OBJECT')
 
-    output_filepath = os.path.join(path, path.split('/')[-2]+'.mp4')
-    subprocess.run(["ffmpeg", "-i", f'{path}/%04d.png', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
+  bpy.ops.render.render(use_viewport=True, animation=animation, write_still=True)
+
+  if animation:
+    output_filepath = output_prefix + '.mp4'
+    subprocess.run(["ffmpeg", "-i", f'{output_prefix}%04d.png', "-vcodec", "libx264", "-vf", "format=yuv420p", "-y", output_filepath])
     subprocess.run(["ffmpeg", "-i", output_filepath, "-pix_fmt", "rgb24", output_filepath[:-3]+'gif'])
 
 
 def save_blender_scene(path: str) -> None:
   bpy.ops.wm.save_as_mainfile(filepath=path)
 
 
@@ -93,16 +93,15 @@
   d = (eye - at).normalized()
   r = up.cross(d).normalized()
   u = d.cross(r).normalized()
   camera.matrix_world = mathutils.Matrix(((r.x, u.x, d.x, eye.x),
                                           (r.y, u.y, d.y, eye.y),
                                           (r.z, u.z, d.z, eye.z),
                                           (0.0, 0.0, 0.0, 1.0)))
-
-
+  
 # def create_video(input_dir, pattern, output_filepath):
 #   trans_to_white = "format=yuva444p,\
 #   geq=\
 #   'if(lte(alpha(X,Y),16),255,p(X,Y))':\
 #   'if(lte(alpha(X,Y),16),128,p(X,Y))':\
 #   'if(lte(alpha(X,Y),16),128,p(X,Y))'"
 
@@ -239,13 +238,14 @@
           obj.rotation_quaternion = [properties['rotation'][3], properties['rotation'][0], properties['rotation'][1], properties['rotation'][2]]
           obj.location = [properties['translation'][0], properties['translation'][1], properties['translation'][2]]
           create_mat(obj, properties['color'])
         # somwhere here parse the blender parameters
 
     # Render if output filename is provided
     if len(argv) > 0:
-        render(argv[0], animation=animation)
+        print(argv)
+        render(os.path.abspath(argv[0]), animation=animation)
 
     output_blender_file = f'blender_scene.blend'
     output_blender_file = os.path.abspath(output_blender_file)
     save_blender_scene(output_blender_file)
     print('Saved blender file to:', output_blender_file)
```

### Comparing `pyviz3d-0.3.2/pyviz3d/src/css/bootstrap.min.css` & `pyviz3d-0.3.3/pyviz3d/src/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/favicon.ico` & `pyviz3d-0.3.3/pyviz3d/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/index.html` & `pyviz3d-0.3.3/pyviz3d/src/index.html`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/js/bootstrap.min.js` & `pyviz3d-0.3.3/pyviz3d/src/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/js/jquery.min.js` & `pyviz3d-0.3.3/pyviz3d/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/src/js/scene.js` & `pyviz3d-0.3.3/pyviz3d/src/js/scene.js`

 * *Files identical despite different names*

### Comparing `pyviz3d-0.3.2/pyviz3d/visualizer.py` & `pyviz3d-0.3.3/pyviz3d/visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,14 @@
         """
         return name.replace(':', ';')
 
     def save(self,
             path: str,
             port: int=6008,
             blender_args: dict=None,
-            # show_in_blender: bool=False,
-            # blender_output_path=None,
-            # blender_executable_path=None,
             verbose=True):
         """Creates the visualization and displays the link to it.
 
         :param path: The path to save the visualization files.
         :param port: The port to show the visualization.
         :param verbose: Whether to print the web-server message or not.
         """
@@ -111,37 +108,34 @@
         print("2) Open in browser:")
         print("    http://localhost:" + str(port))
         print(
             "************************************************************************"
         )
 
         if blender_args:
-            # self.show_in_blender(path, blender_output_path, blender_executable_path, verbose)
             self.show_in_blender(path, blender_args, verbose)
 
     def show_in_blender(self,
                         path: str,
                         blender_args: dict,
-                        # blender_output_path: str,
-                        # blender_executable_path: str,
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
 
         cmd = "cd " + directory_destination + "; " + blender_args['executable_path'] + " --background --python blender_script.py"
-        if blender_args['executable_path']:
-            cmd = cmd + " -- " + blender_args['executable_path']
+        if blender_args['output_prefix']:
+            cmd = cmd + " -- " + blender_args['output_prefix']
         os.system(cmd)
 
         if verbose:
             print("")
             print("************************************************************************")
             print("Blender instructions")
             print(cmd)
```

### Comparing `pyviz3d-0.3.2/pyviz3d.egg-info/PKG-INFO` & `pyviz3d-0.3.3/pyviz3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyviz3d-0.3.2/pyviz3d.egg-info/SOURCES.txt` & `pyviz3d-0.3.3/pyviz3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

