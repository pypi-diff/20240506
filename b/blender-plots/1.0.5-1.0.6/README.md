# Comparing `tmp/blender-plots-1.0.5.tar.gz` & `tmp/blender-plots-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender-plots-1.0.5.tar", last modified: Sat Feb 10 13:50:58 2024, max compression
+gzip compressed data, was "blender-plots-1.0.6.tar", last modified: Mon May  6 16:38:00 2024, max compression
```

## Comparing `blender-plots-1.0.5.tar` & `blender-plots-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-02-10 13:50:58.208871 blender-plots-1.0.5/
--rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.5/LICENSE
--rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-02-10 13:50:58.208871 blender-plots-1.0.5/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.5/README.md
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-02-10 13:50:58.208871 blender-plots-1.0.5/blender_plots/
--rw-rw-r--   0 linus     (1000) linus     (1000)      278 2024-02-02 17:38:40.000000 blender-plots-1.0.5/blender_plots/__init__.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.5/blender_plots/arrows.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     8676 2024-02-02 19:57:15.000000 blender-plots-1.0.5/blender_plots/blender_utils.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5488 2024-02-02 20:38:03.000000 blender-plots-1.0.5/blender_plots/plots_base.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     9386 2024-02-10 13:48:12.000000 blender-plots-1.0.5/blender_plots/scatter.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.5/blender_plots/surface.py
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-02-10 13:50:58.208871 blender-plots-1.0.5/blender_plots.egg-info/
--rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-02-10 13:50:58.000000 blender-plots-1.0.5/blender_plots.egg-info/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)      333 2024-02-10 13:50:58.000000 blender-plots-1.0.5/blender_plots.egg-info/SOURCES.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-02-10 13:50:58.000000 blender-plots-1.0.5/blender_plots.egg-info/dependency_links.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-02-10 13:50:58.000000 blender-plots-1.0.5/blender_plots.egg-info/top_level.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-02-10 13:50:58.208871 blender-plots-1.0.5/setup.cfg
--rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-02-10 13:49:14.000000 blender-plots-1.0.5/setup.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/
+-rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.6/LICENSE
+-rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-05-06 16:38:00.528768 blender-plots-1.0.6/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.6/README.md
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/blender_plots/
+-rw-rw-r--   0 linus     (1000) linus     (1000)      216 2024-05-06 16:17:21.000000 blender-plots-1.0.6/blender_plots/__init__.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.6/blender_plots/arrows.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     9481 2024-05-06 15:10:45.000000 blender-plots-1.0.6/blender_plots/blender_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     2269 2024-05-06 16:34:56.000000 blender-plots-1.0.6/blender_plots/marker_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5453 2024-05-06 15:17:02.000000 blender-plots-1.0.6/blender_plots/plots_base.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     9484 2024-05-06 15:54:55.000000 blender-plots-1.0.6/blender_plots/scatter.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.6/blender_plots/surface.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/blender_plots.egg-info/
+-rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)      363 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/SOURCES.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/dependency_links.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/top_level.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-05-06 16:38:00.528768 blender-plots-1.0.6/setup.cfg
+-rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-05-06 16:21:03.000000 blender-plots-1.0.6/setup.py
```

### Comparing `blender-plots-1.0.5/LICENSE` & `blender-plots-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.5/README.md` & `blender-plots-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.5/blender_plots/arrows.py` & `blender-plots-1.0.6/blender_plots/arrows.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.5/blender_plots/blender_utils.py` & `blender-plots-1.0.6/blender_plots/blender_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,24 +76,37 @@
 
 
 def delete(obj, with_children=False):
     """Delete blender object and its children"""
     if with_children:
         for child in obj.children:
             delete(child, with_children=True)
-    bpy.data.objects.remove(obj, do_unlink=True)
+    if isinstance(obj, bpy.types.Object):
+        bpy.data.objects.remove(obj, do_unlink=True)
+    elif isinstance(obj, bpy.types.Collection):
+        bpy.data.collections.remove(obj, do_unlink=True)
+    else:
+        raise ValueError(f'Failed to delete object {obj}: unrecognized type')
 
+def new_collection(name):
+    if name in bpy.data.collections:
+        delete(bpy.data.collections[name], with_children=True)
+    collection = bpy.data.collections.new(name)
+    bpy.context.collection.children.link(collection)
+    return collection
 
-def new_empty(name, object_data=None, select=True):
+def new_empty(name, object_data=None, select=True, collection=None):
     """Create new empty blender object with specified name and data, deletes any previous object with the same name."""
     if name in bpy.data.objects:
         delete(bpy.data.objects[name], with_children=True)
 
     new_object = bpy.data.objects.new(name, object_data)
-    bpy.context.collection.objects.link(new_object)
+    if collection is None:
+        collection = bpy.context.collection
+    collection.objects.link(new_object)
 
     if select:
         bpy.context.view_layer.objects.active = new_object
 
     return new_object
 
 
@@ -167,14 +180,22 @@
     color_node = material.node_tree.nodes.new("ShaderNodeAttribute")
     color_node.attribute_name = Constants.MARKER_COLOR
 
     material.node_tree.links.new(color_node.outputs["Color"],
                                  material.node_tree.nodes["Principled BSDF"].inputs["Base Color"])
     return material
 
+def add_mesh_color(mesh, color):
+    """Add uniform color to mesh."""
+    if len(color) == 3:
+        color = (*color, 1)
+    material = bpy.data.materials.new("color")
+    material.diffuse_color = color
+    mesh.materials.append(material)
+
 def get_frame_selection_node(modifier, n_frames):
     """Add node that filters points based on the Frame Index property."""
     node_linker = NodeLinker(modifier.node_group)
     frame_index = node_linker.new_node(
         "GeometryNodeInputNamedAttribute",
         data_type="FLOAT",
         name=Constants.FRAME_INDEX,
```

### Comparing `blender-plots-1.0.5/blender_plots/plots_base.py` & `blender-plots-1.0.6/blender_plots/plots_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 class Plot:
     def __init__(self, x, y, z, color=None, name="plot", n_dims=1):
         self.name = name
         self.mesh = bpy.data.meshes.new(self.name)
         self.base_object = bu.new_empty(self.name, self.mesh)
         self.color_material = None
-        self.color_material = None
         self._points = None
         self.modifier = self.base_object.modifiers.new(type="NODES", name=name)
 
         points, self.n_frames, *self.dims = get_points_array(x, y, z, n_dims)
         self.points = points
         self.color = color
```

### Comparing `blender-plots-1.0.5/blender_plots/scatter.py` & `blender-plots-1.0.6/blender_plots/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,26 @@
     """
 
     def __init__(
             self, x, y=None, z=None, color=None, name="scatter",
             marker_type="ico_spheres", marker_scale=None, marker_rotation=None,
             randomize_rotation=False, **marker_kwargs
         ):
-        super(Scatter, self).__init__(x, y, z, color=color, name=name, n_dims=1)
+        super().__init__(x, y, z, color=color, name=name, n_dims=1)
 
         if marker_type == "spheres":
             node_linker = add_sphere_markers(self.modifier, n_frames=self.n_frames, **marker_kwargs)
         elif marker_type is not None:
             node_linker = add_mesh_markers(
                 self.modifier,
                 randomize_rotation=randomize_rotation,
                 marker_type=marker_type,
                 set_scale=marker_scale is not None,
                 n_frames=self.n_frames,
+                with_color=color is not None,
                 **marker_kwargs
             )
         else:
             node_linker = bu.get_node_linker(self.modifier)
             node_linker.new_input_socket('Point Color', 'NodeSocketMaterial')
 
         self.modifier[node_linker.input_sockets['Point Color']] = self.color_material
@@ -103,55 +104,56 @@
             marker_rotation, rotation_dims = self.tile_data(self._marker_rotation, [[3], [3, 3]], "marker rotation")
             if rotation_dims == [3, 3]:
                 marker_rotation = np.stack([np.array(mu.Matrix(r).to_euler()) for r in marker_rotation])
             bu.set_vertex_attribute(self.mesh, Constants.MARKER_ROTATION, marker_rotation, "FLOAT_VECTOR")
 
 
 def add_mesh_markers(base_modifier, marker_type, randomize_rotation=False, set_scale=False,
-                     n_frames=0, **marker_kwargs):
+                     n_frames=0, with_color=False, **marker_kwargs):
     """Create a geometry node modifier that instances a mesh on each vertex.
     Args:
         base_modifier: modifier to add markers to.
         marker_type: name of marker type (see MARKER_TYPES), or a blender mesh/object to use as marker
         randomize_rotation: if True each mesh instance will be given a random rotation (uniform euler angles)
         set_scale: if True use the MARKER_SCALE attribute to set the marker scale
         n_frames: number of frames to animate, no animation if set to 0.
         marker_kwargs: additional arguments for configuring markers
     """
     node_linker = bu.get_node_linker(base_modifier)
     node_linker.new_input_socket('Point Color', 'NodeSocketMaterial')
-    node_linker.new_input_socket('Point Instance', 'NodeSocketObject')
 
     points_socket = node_linker.new_node(
         "GeometryNodeMeshToPoints",
         mesh=node_linker.group_input.outputs["Geometry"]
     ).outputs["Points"]
 
     if marker_type in Constants.MARKER_TYPES:
+        # use one of the default marker types
         mesh_socket = node_linker.new_node(node_type=Constants.MARKER_TYPES[marker_type], **marker_kwargs).outputs["Mesh"]
-    elif isinstance(marker_type, bpy.types.Mesh) or isinstance(marker_type, bpy.types.Object):
-        # use the supplied mesh by adding it as an input socket to the base_modifier
+    elif isinstance(marker_type, (bpy.types.Object, bpy.types.Collection)):
+        # use custom object or collection as marker
+        subtype = marker_type.__class__.__name__
+        node_linker.new_input_socket('Point Instance', f'NodeSocket{subtype}')
         base_modifier[node_linker.input_sockets['Point Instance']] = marker_type
-        base_modifier.show_viewport = False
-        base_modifier.show_viewport = True
         mesh_socket = node_linker.new_node(
-            "GeometryNodeObjectInfo",
-            Object=node_linker.group_input.outputs["Point Instance"]
-        ).outputs["Geometry"]
+            f"GeometryNode{subtype}Info",
+            **{subtype: node_linker.group_input.outputs["Point Instance"]}
+        ).outputs[{'Object': 'Geometry', 'Collection': 'Instances'}[subtype]]
         marker_type.hide_viewport = True
         marker_type.hide_render = True
     else:
-        raise TypeError(f"Invalid marker type: {marker_type}, expected bpy.types.Mesh, bpy.Types.Object, "
+        raise TypeError(f"Invalid marker type: {marker_type}, expected Object or Collection, "
                         f"or one of: {', '.join(Constants.MARKER_TYPES)}")
 
-    colored_mesh = node_linker.new_node(
-        "GeometryNodeSetMaterial",
-        geometry=mesh_socket,
-        material=node_linker.group_input.outputs["Point Color"]
-    ).outputs["Geometry"]
+    if with_color:
+        mesh_socket = node_linker.new_node(
+            "GeometryNodeSetMaterial",
+            geometry=mesh_socket,
+            material=node_linker.group_input.outputs["Point Color"]
+        ).outputs["Geometry"]
 
     marker_scale = node_linker.new_node(
         "GeometryNodeInputNamedAttribute",
         data_type="FLOAT_VECTOR",
         name=Constants.MARKER_SCALE,
     )
     marker_rotation = node_linker.new_node(
@@ -159,15 +161,15 @@
         data_type="FLOAT_VECTOR",
         name=Constants.MARKER_ROTATION,
     )
     instance_on_points_node = node_linker.new_node(
         "GeometryNodeInstanceOnPoints",
         points=points_socket,
         selection=None if n_frames is None else bu.get_frame_selection_node(base_modifier, n_frames).outputs["Value"],
-        instance=colored_mesh,
+        instance=mesh_socket,
         rotation=marker_rotation.outputs["Attribute"],
         scale=marker_scale.outputs["Attribute"] if set_scale else [1, 1, 1],
     )
     if randomize_rotation:
         # these rotation are not uniform (some orientations will be more likely than others)
         # but it usually looks decent
         random_euler = node_linker.new_node("FunctionNodeRandomValue")
```

### Comparing `blender-plots-1.0.5/blender_plots/surface.py` & `blender-plots-1.0.6/blender_plots/surface.py`

 * *Files identical despite different names*

