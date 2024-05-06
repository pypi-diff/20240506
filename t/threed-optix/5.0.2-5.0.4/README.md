# Comparing `tmp/threed_optix-5.0.2.tar.gz` & `tmp/threed_optix-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-5.0.2.tar", last modified: Thu May  2 07:22:09 2024, max compression
+gzip compressed data, was "threed_optix-5.0.4.tar", last modified: Mon May  6 11:41:54 2024, max compression
```

## Comparing `threed_optix-5.0.2.tar` & `threed_optix-5.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.2/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.2/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-02 07:22:09.501516 threed_optix-5.0.2/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.2/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46819 2024-05-01 11:13:46.000000 threed_optix-5.0.2/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46929 2024-05-01 11:13:46.000000 threed_optix-5.0.2/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-02 07:22:09.501516 threed_optix-5.0.2/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1242 2024-05-01 11:13:46.000000 threed_optix-5.0.2/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      832 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23704 2024-05-02 07:18:42.000000 threed_optix-5.0.2/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.2/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43188 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.2/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.2/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.2/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19082 2024-05-02 07:20:24.000000 threed_optix-5.0.2/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    59843 2024-05-02 07:18:42.000000 threed_optix-5.0.2/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15018 2024-05-01 13:31:16.000000 threed_optix-5.0.2/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.2/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-02 07:22:09.501516 threed_optix-5.0.2/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-02 07:22:09.000000 threed_optix-5.0.2/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-02 07:22:09.000000 threed_optix-5.0.2/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-02 07:22:09.000000 threed_optix-5.0.2/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-05-02 07:22:09.000000 threed_optix-5.0.2/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-02 07:22:09.000000 threed_optix-5.0.2/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.4/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.4/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-06 11:41:54.939089 threed_optix-5.0.4/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.4/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.4/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.4/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-06 11:41:54.939089 threed_optix-5.0.4/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.4/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23704 2024-05-06 11:40:41.000000 threed_optix-5.0.4/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43529 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.4/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19129 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.4/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.4/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-06 11:41:54.939089 threed_optix-5.0.4/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-06 11:41:54.000000 threed_optix-5.0.4/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-5.0.2/LICENSE.txt` & `threed_optix-5.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/PKG-INFO` & `threed_optix-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 5.0.2
+Version: 5.0.4
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.2/README.md` & `threed_optix-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/help/SDK help text.txt` & `threed_optix-5.0.4/help/SDK help text.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Optical Simulation SDK
-
 ## Begin
 
 Our optical simulation SDK is released in a beta version and has only limited features support at the moment.
 We are working on supporting more features and you can expect new versions to come out soon.
 
 #### Install
 
@@ -45,21 +44,14 @@
 `tdo.Setup` are the objects that represent your simulation setups in the SDK.
 You could access their information:
 
 - `setup.name` is the setup name. It is not neceseraliy unique.
 - `setup.id` is the id of the setup. It is unique.
 - `setup.parts` is a list of `tdo.Part` objects that the setup contains.
 
-#### Get a list of your 3DOptix setups:
-
-```python
-#'setups' will be a list of your simulation setups as a `tdo.Setup` objects
-setups = client.get_setups()
-```
-
 #### Create a `tdo.Setup`
 
 You could create a new setup with `client.create_setup` method. The method has the following arguments:
 - `name`: str, The name of the setup.
 - `description`: str, The description of the setup.
 - `labels`: list[str], the labels of the setup. Can be anything from `tdo.SETUP_LABELS`.
 - `units`: str, 'mm' or 'inch'. Default to 'mm'.
@@ -74,16 +66,16 @@
 
 #### Find a setup:
 
 First, we need to identify the setup we want to work on:
 
 ```python
 #Examine the setups:
-for s in setups:
-    print(s.name, s.id)
+for setup in client:
+    print(setup.name, setup.id)
 ```
 
 > **Note**
 > A setup id is unique, but the name is not unique
 
 Then, we can get the setup object by using `client.get(name)` and `client[id]` methods:
 
@@ -93,44 +85,23 @@
 setup = client.get(setup_name)
 
 #Get setup by id
 setup_id = '<your setup id'
 setup = client[setup_id]
 ```
 
-If the setups is not found, `client[setup_id]` **will** lead to an error, and `client.get(setup_name)` will **not**.
-
-Another way to do this is by looping over the setps list:
-
-```python
-#Chosen setup id
-setup_id = '<your setup id>'
-
-#Get the 'Setup' object to work on
-setup = None
-for s in setups:
-    #Get your setup by name
-    if s.id == setup_id:
-        setup = s
-        break
-
-assert setup is not None, "Setup was not found"
-```
-
 ### Parts:
 
 `tdo.Part` are the objects that represent your setup parts in the SDK.
 You could access their information:
 
 - `part.label` is the label of the part. It is not neceseraliy unique.
 - `part.id` is the id of the setup. It is unique.
 - `part.surfaces` is a list of `tdo.Surface` objects that the part has.
 - `part.pose` is a list of 6 floats representing the part's position and rotation relative to their associated coordinate system.
-- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
-- `part.optical_data` in the case that the part is `tdo.Optic` part.
 
 > **Warning**
 > Setups with parts that were loaded from a CAD file are not supported fully at the moment.
 > These CAD parts will not lead to an error, but they might lead to unexpected behavior.
 
 `tdo.Detector` is the object used to represent detectors. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing detectors within the SDK.
 `tdo.Detector` has the following additional information:
@@ -147,37 +118,43 @@
 - `ls.vis_count`
 - `ls.count_type`
 - `ls.opacity`
 - `ls.color`
 - `ls.source_type`
 - And information that changes with respect to `source_type`.
 
+`tdo.Optic` is the object used to represent optics. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing optics within the SDK.
+`tdo.Optic` has the following additional information:
+- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
+- `part.optical_data` contains all the data that's specific to the optical properties of the part, such as its geometry, shape, brand, physical data, etc.
+
+
 **You could see a full description of these objects, as well as how to modify them, later on this document**.
 
 #### Add a `tdo.Part`:
 To add a detector to the setup:
 ```python
-detector = setup.add_detector(label = label,
-                              pose = pose)
+detector = setup.add_detector(**kwargs)
 ```
 
 To add a light source to the setup:
 ```python
-ls = setup.add_light_source(label = label,
-                              pose = pose)
+ls = setup.add_light_source(**kwargs)
 ```
 
 To add optic to the setup, we will have to find its `db_id` from the product catalog or take the number id of the created optic from `client.create_xxx` methods.
 ```python
 ls = setup.add_optics(db_id = db_id,
-                            label = label,
-                            pose = pose)
+                      **kwargs)
 ```
 You could get the part number id in the `ID` column in the product catalog, or take the number id of the part you created.
 
+>> **Note**
+>> You can add parts with any keyword arguments from part.change_config to add and change properties with the same command.
+
 #### Find a part:
 
 Almost identical to finding a setup.
 
 ```python
 #Examine the parts of the setup
 for part in setup:
@@ -197,47 +174,30 @@
 #Get part by id
 part_id = '<your part id'
 part = setup[part_id]
 ```
 
 If the part is not found, `setup[part_id]` **will** lead to an error, and `setup.get(part_label)` will **not**.
 
-Or, alternatively, looping over the `tdo.Setup` object:
-
-```python
-#Chosen part id
-part_id = '<the id of the part to change>'
-
-#Get the 'Part' object to work on
-part = None
-for p in setup:
-    #Get part by id
-    if p.id == part_id:
-       part = p
-       break
-
-assert part is not None, "Part was not found"
-```
-
 #### Delete a part from the setup:
 In order to remove a part from the setup, we simply use `setup.delete_part` method as follows:
 ```python
-part_to_delete = setup.get('<part_to_delete_label')
+part_to_delete = setup.get('<part_to_delete_label>')
 setup.delete_part(part_to_delete)
 ```
 And that's it! The part is removed from the setup.
 
 ### Surface
 
 `tdo.Surface` are the objects that represent the surfaces of the part in the SDK.
 You could access their information:
 
 - `surface.name` is the name of the surface. It is not neceseraliy unique.
 - `surface.id` is the id of the setup. It is unique.
-- `surface.analyses` is a list of `tdo.Analysis` objects that the surface has. Later on we discuss how to add new and run them.
+- If the surface is the front of a detector, you could access the analyses with `surface.analyses`. It is a list of `tdo.Analysis` objects that the surface has. Later on we discuss how to create, find and run them.
 
 #### Create or add a `tdo.Surface`
 
 Creation of new surfaces is not possible.
 
 #### Find a surface:
 
@@ -256,94 +216,76 @@
 surface = part.get(surface_name)
 
 #Get surface by id
 surface_id = '<your surface id>'
 surface = part[surface_id]
 ```
 
-If the surface is not found, `part[surface_id]` **will** lead to an error, and `part.get(surface_name)` will **not**.
-
-Or looping over the part:
-
-```python
-#Choose surface id
-surface_id = '<the id of the surface to perform analysis on>'
-
-#Get the 'tdo.Surface' object:
-surface = None
-for s in part:
-    #Get surface by id
-    if s.id == surface_id:
-      surface = s
-      break
-
-assert surface is not None, "Surface was not found"
-```
-
 ### Scattering
 Each surface of `tdo.Optic` part can have scattering properties.
 To examine them, check `surface.scattering` property.
 If the surface does not have scattering, it will return `False`.
 #### Disable Surface Scattering
-If a surface has a scattering that you want to disable, simply use `surface.disable_scatterin` method.
+If a surface has a scattering that you want to disable, simply use `surface.disable_scattering` method.
 ```python
 surface.diasble_scattering()
 if not surface.scattering:
     print('Success!')
 ```
 #### Add Or Change Scattering
 Scattering can be added or changed with `surface.XXX_scattering` methods.
 Each of them acccepts the following arguments:
-- `transmittance`, `absorption`, `reflection`: float, The relative part of transmittance, absorption and reflection of the scattering.
-- `num_of_rays`: int,
-- `relative_power_threshold`: float,
+- `transmittance`, `absorption`, `reflection`: float, The proportion of  the light that is transmitted, absorbed and reflected by the surface.
+- `split_ratio`: int, number of ray that each ray split to.
+- `power_threshold`: float, Relative power threshold used for terminating the ray tracing simulation. It represents the minimum amount of remaining power below which rays are terminated.
+
 ##### Cos-nth
 Requires also `n` parameter, which defaults to 1.5.
 ```python
 surface.cos_scattering(transmittance = 0.5,
                         reflection = 0.3,
                         absorption = 0.1,
-                        num_of_rays = 10,
-                        relative_power_threshold = 5,
+                        split_ratio = 10,
+                        power_threshold = 5,
                         n = 2)
 ```
 ##### Gaussian
 Requires also `sigma_x`, `sigma_y` and `azimuth_theta` parameters.
 ```python
 surface.gaussian_scattering(transmittance = 0.99,
                             reflection = 0.01,
                             absorption = 0,
-                            num_of_rays = 5,
-                            relative_power_threshold = 2
+                            split_ratio = 5,
+                            power_threshold = 2
                             sigma_x = 10,
                             sigma_y = 15,
                             azimuth_theta = 0)
 ```
 
 ##### ABG
 Requires also `a`, `b` and `g` parameters.
 ```python
 surface.abg_scattering(transmittance = 0.95,
                             reflection = 0.025,
                             absorption = 0.025,
-                            num_of_rays = 7,
-                            relative_power_threshold = 4
+                            split_ratio = 7,
+                            power_threshold = 4
                             a = 1,
                             b = 2,
                             g = 2)
 ```
 
 ##### Lambertian
 Does not require unique parameters.
 ```python
-surface.lembertian_scattering(transmittance = 0.97,
+surface.lambartian_scattering(transmittance = 0.97,
                             reflection = 0.03,
                             absorption = 0.01,
-                            num_of_rays = 10,
-                            relative_power_threshold = 5,
+                            split_ratio = 10,
+                            power_threshold = 5,
                             )
 ```
 
 ### Coordinate Systems
 #### Part Coordinate System
 You can see all of the coordinate systems that a part has in `part.cs` list.
 Every `CoordinateSystem` object has `name`, `pose`, and `id` properties.
@@ -352,38 +294,38 @@
 for cs in part.cs:
     print(cs.name, cs.id, cs.pose)
 
 lcs = part.lcs
 rcs, reference_part = part.rcs
 ```
 #### The World Coordinate System
-The world coordinate system is stored in `tdo.WORLD` object. You can use it as a coordinate system.
+The world coordinate system is stored in `tdo.GLOBAL` object. You can use it as a coordinate system.
 
 #### Change lcs and rcs
 You can change lcs and rcs with `part.change_cs` method. It accepts the following arguments:
 - `lcs`: CoordinateSystem, if defined, it will be the new local coordinate system of the part.
-- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part.
+- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part. use `tdo.GLOBAL` cs to defined the global cs as the rcs.
 ```python
 lens.change_cs(lcs = lens.cs[1])
 detector.change_cs(rcs = lens.cs[0])
-ls.change_cs(lcs = ls.cs[0], rcs = tdo.WORLD)
+ls.change_cs(lcs = ls.cs[0], rcs = tdo.GLOBAL)
 ```
 
 ### Materials
 #### Find Materials From Database
 Some mmethods require specific materials from our database. In order to find them, use `client.search_materials` method.
 ```python
 materials = client.search_materials('N-BK7')
 ```
-`materials` is now a list of `Material` object.
+`materials` is now a list of `tdo.Material` object.
 ```python
 for m in materials:
-    print(m.id, m.name, m.company)
+    m.describe()
 ```
-Finally, you can use the chosen material object of directly in the material id.
+Finally, you can use the chosen material object or its material id directly.
 
 ### Analysis
 `tdo.Analysis` are the objects that represent analyses that can be performed on a surface.
 They are defined by:
 
 - `id`: The unique id of the analysis.
 - `surface`: The `tdo.Surface` object on which the analysis will be made.
@@ -394,15 +336,15 @@
 A surface can contain several analysis with identical properties and different ids.
 However, each analysis consumes your account resources, since analysis id holds its results.
 When you run the analysis again, the last result is deleted from 3DOptix systems.
 So, we reccomend storing iterations of the same analysis locally and use duplicated analyses only when you think it's necessary.
 
 #### Find existing analysis
 
-Every new analysis consumes storage resources for you account.
+Every new analysis consumes storage resources for your account.
 So, we reccomend sticking to the same analysis if they have the same properties instead of creating new ones.
 You could get a list of the `tdo.Analysis` of the surface like this:
 
 ```python
 setup = client.get('example')
 detector = setup.get('my_detector')
 detector_front = detector.get('front')
@@ -415,15 +357,14 @@
 ```
 
 Or get an existing analyses with required parameters, if the id doesn't matter:
 
 ```python
 detector_front = setup.get('my_detector').get('front')
 analysis = detector_front.find_analysis(name = name, rays = rays, resolution = resolution)
-assert analysis
 ```
 
 #### Create and add analysis
 
 If you want to create an analysis that doesn't exist for the surface yet, or you want to create a duplicated analysis, we can create one:
 
 ```python
@@ -436,18 +377,22 @@
 
 For example:
 
 ```python
 laser = setup.get('ls')
 surface = detector.get('front')
 
-analysis = tdo.Analysis(
-                        surface = surface,
-                        resolution = [500, 500],
-                        rays = {laser: 1e5},
+analysis1 = tdo.Analysis(surface = surface,
+                        resolution = [100, 200],
+                        rays = {laser: 1e5, laser2: 1e4},
+                        name = "Spot (Incoherent Irradiance)"
+                        )
+analysis2 = tdo.Analysis(surface = surface,
+                        resolution = 100, #for equal height and width pixels
+                        rays = 1e6, #for all of the lasers in the setup
                         name = "Spot (Incoherent Irradiance)"
                         )
 ```
 
 > **Reminder**
 > You can always access all the possible analysis names with `tdo.ANALYSIS_NAMES`
 
@@ -470,42 +415,14 @@
 results = setup.run(analysis)
 analysis.show()
 surface.delete_analysis(analysis)
 ```
 
 ## Make Changes
 
-#### Backup
-
-Before making any changes, we reccomend storing the original part or setup, before any changes:
-
-```python
-#Backup the part
-part = setup.get('part_label')
-part.backup()
-
-#Some code...
-
-#Restore the original state of the part
-part.restore()
-```
-
-In the case of multiple changes to multiple parts, you might find this easier:
-
-```python
-# Backup the setup
-setup = client['setup_id']
-setup.backup()
-
-#Some code...
-
-#Restore the original state of the part
-setup.restore()
-```
-
 #### Transformations
 
 You could move and rotate part using `part.change_pose()` method that moves the part to a location on the three axis (x, y, z) and rotates it in respect to them (alpha, beta, gamma).
 
 All six numbers indicating absolute future value in respect to the part's coordinate system, **not** change and **not** with respect to the global coordinate system.
 if you want to change coordinate systems, please check `part.change_cs` method.
 
@@ -547,27 +464,21 @@
 Detectors have a `detector.change_opacity()` and `detector.change_size()` methods, that changes the detector's opacity and size, accordingly.
 This is how you use them:
 
 ```python
 # Get the detector
 detector = setup.get('detector_label')
 
-#Backup the original detector's state
-detector.backup()
-
 #Apply changes
 detector.change_size([new_half_height, new_half_width])
 detector.change_opacity(new_opacity)
 detector.change_pose([x, y, z, alpha, beta, gamma])
 
 #Verify change
 print(detector.size, detector.opacity, detector.pose)
-
-# Restore if needed
-detector.restore()
 ```
 
 At the beginning, we reccomend frequent sanity-checks in the GUI to make sure you got everything right.
 
 ### Modify Light Sources
 
 #### Change wavelengths
@@ -602,37 +513,32 @@
 
 At the beginning, we reccomend frequent sanity-checks in the GUI to make sure you got everything right.
 
 **Create normal distribution**
 If you want to create wavelengths spectrum with a normal disribution, you could use `tdo.utils.wavelengths_normal_distribution`:
 
 ```python
-import threed_optix.utils as tu
-
 # Define the spectrum
-wavelengths_spectrum = tu.wavelengths_normal_distribution(mean_wavelength, std_dev, num_wavelengths)
+wavelengths_spectrum = tdo.wavelengths_normal_distribution(mean_wavelength, std_dev, num_wavelengths)
 
 # Modify the light source
 light_source.change_wavelengths(wavelengths_spectrum)
 ```
-
 Where:
 
 - `mean_wavelength` is the mean wavelength of the distribution
 - `std_dev` is the standard deveation of the distribution
 - `num_wavelengths` is the number of the wavelengths that will be sampled.
 
 **Create uniform distribution**
 Similarly, If you want to create wavelengths spectrum with a uniform disribution, you could use `tdo.utils.wavelengths_uniform_distribution`:
 
 ```python
-import threed_optix.utils as tu
-
 # Define the spectrum
-wavelengths_spectrum = tu.wavelengths_uniform_distribution(min_wavelength, max_wavelength, num_wavelengths)
+wavelengths_spectrum = tdo.wavelengths_uniform_distribution(min_wavelength, max_wavelength, num_wavelengths)
 
 # Modify the light source
 light_source.change_wavelengths(wavelengths_spectrum)
 ```
 
 Where:
 
@@ -942,61 +848,50 @@
 > Otherwise, choose the existing analysis and run it instead. This helps optimizing your system memory credits usage.
 
 #### Results
 
 Even if we didn't store it in another variable, we can view and analize the latest results in a raw form:
 
 ```python
+# For jupyter notebooks or HTML
+display(analysis.results)
+
+# For scripts
 print(analysis.results)
 ```
 
-The result will be a JSON where each key is a wavelength in the analysis results.
-Each wavelength contains the `np.ndarray` matrices for each polarization.
+The result will be a pandas dataframe (`pd.DataFrame`) with all the different matrices.
+The columns of the dataframe are:
+    - `data`: The matrix of the results for that row's configuration.
+    - `polarization`: The polarization of the data.
+    - `wl`: The wavelength of the data.
+    - `spot_target_kind`: Can be either 'Source', 'Group' or 'Total', indicating if the data is the result of a single source, coherent group or the total results of all the light sources.
+    - `spot_target`: The id of the light source\coherent group.
+
 For example, let's say I am looking for the _"X"_ polarization, _400 nm_ rays hit matrix:
 
 ```python
-matrix = results[400]['X']
+mask = (results.wl == 400) & (results.polarization == 'X')
+matrices = results[mask].data
 ```
-
-For analysis without polarization, polarization kind is "NONE".
+and, ofcourse, any `pd.DataFrame` manipulation will work as usuall.
 
 > **Note**
 > If you plan on running the anlysis again, it is really important to store a deepcopy of analysis.results in the `matrix` variable.
 > Otherwise, the variable will hold the pointer to the `results` property of the analysis, and the previous results will be overriden.
-> Another option is to store the results of `analysis()` in another variable
+> Another option is to store the results of `setup.run(analysis)` in another variable, since it outputs a copy anyway.
 
 If we want to see the matrices as a images, we can simply:
 
 ```python
 #for static figure
-analysis.show()
+tdo.show_matrix(matrix)
 
 #for interactive figure
-analysis.show_interactive()
-```
-
-**Arguments**
-
-- **`upscale`**: Upscales the image (smooth the pixels over) by using `upscale = True`.
-- **`polarizations`**: Presents only selected polarization by passing a list of strings to the argument.
-- **`wavelengths`**: Presents only selected wavelengths by passing a list of integers to the argumet.
-- **`figsize`**: Determines the size of the presented figure in inches.
-
-```python
-analysis.show(upscale = True,
-              polarizations = ['X'],
-              wavelengths = [550, 600],
-              figsize = (15, 15))
-```
-
-```python
-analysis.show_interactive(upscale = True,
-                          polarizations = ['Y', 'Z'],
-                          wavelengths = [500, 700],
-                          figsize = (20, 20))
+tdo.show_matrix(matrix, interactive = True)
 ```
 
 ## Create a new `tdo.Optics` in your product catalog
 As for now, the SDK supports creating spherical and conic lenses.
 ### Create Lenses
 #### Spherical Lenses
 To create spherical lens, we can use `client.create_spherical_lens` method. The arguments are:
@@ -1048,25 +943,25 @@
 - `r1_x`, `r1_y`: float, the first radius of curvature.
 - `r2_x`, `r2_y`: float, the second radius of curvature.
 - `k1_x`, `k1_y`, `k2_x`, `k2_y`: float, the conic coefficients of the lens. Default to 0.
 
 The method returns the number id of the created element.
 ```python
 lens_db_id = client.create_spherical_lens(name = name,
-                                              material = material,
-                                              diameter = diameter,
-                                              thickness = thickness,
-                                              r1_x = r1_x,
-                                              r1_y = r1_y,
-                                              r2_x = r2_x,
-                                              r2_y = r2_y,
-                                              k1_x = k1_x,
-                                              k1_y = k1_y,
-                                              k2_x = k2_x,
-                                              k2_y = k2_y)
+                                          material = material,
+                                          diameter = diameter,
+                                          thickness = thickness,
+                                          r1_x = r1_x,
+                                          r1_y = r1_y,
+                                          r2_x = r2_x,
+                                          r2_y = r2_y,
+                                          k1_x = k1_x,
+                                          k1_y = k1_y,
+                                          k2_x = k2_x,
+                                          k2_y = k2_y)
 ```
 ### Create Grating
 You can create a new grating in the database with `client.create_grating` method.
 It requires the following arguments:
 - `name`: str, The name of the grating in the database.
 - `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
 - `grooves`: int, Number of grooves on the grating.
@@ -1112,46 +1007,44 @@
 ## Advanced
 ### Utils Module
 #### Get spot size
 
 `tdo.utils.calculate_spot_size(matrix)` calculates the diameter of the blocking circle of the biggest contours of the matrix, in pixels.
 
 ```python
-import threed_optix.utils as tu
 
 # Assuming that this analysis exists already
 setup = client['setup_id']
 detector = setup.get('detector_label')
 detector_front = detector.get('front')
 
 analysis = detector_front.analysis_with(name ="Spot (Incoherent Irradiance)",
                                         rays = {laser1: 2.5e6, laser2: 2.5e6},
                                         resolution = (1000, 1000)
                                         )
 # Run the analysis
 results = setup.run(analysis)
 
 # Calculate spot size
-matrix = results[550]['X']
-spot_size_dia = tu.calculate_spot_size(matrix)
+spot_size_dia = tdo.calculate_spot_size(results.data[0])
 print(f'Analysis spot size diameter for X polarization at 550 nm is {spot_size_dia}')
 ```
 
 `tdo.utils.encircled_energy(matrix, percent)` calculates the diameter of the circle that centers at the center of energy mass, and contains `percantage` of the matrix's total energy.
 
 ```python
-encircled_energy_radius, center = tu.encircled_energy(matrix, 0.9)
-print(f'Analysis encircled 90% energy radius for X polarization at 550 nm is {encircled_energy_radius}')
+encircled_energy_radius, center = tdo.encircled_energy(matrix, 0.9)
+print(f'Analysis encircled 90% energy radius for X polarization at 550 nm is {encircled_energy_radius} with the center at {center}')
 ```
 
-Of course, these values are pixel values. In order to get absolute values, use `tdo.utils.absolute_pixel_size`:
+Of course, these values are pixel values. In order to get absolute values in length units, use `tdo.utils.absolute_pixel_size`:
 
 ```python
-pixel_radius, center = tu.encircled_energy(matrix, 0.95)
-absolute_radius = tu.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius
+pixel_radius, center = tdo.encircled_energy(matrix, 0.95)
+absolute_radius = tdo.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius # Assuming that the resolution is symmetrical
 print(f'95% Encircled energy radius is {absolute_radius} mm')
 ```
 
 #### Scans
 
 In order to perform a scan, all we need to do is to define an analysis:
 
@@ -1175,17 +1068,14 @@
 ```
 
 Then, we need to iteratively change the properties of some part in the setup and store the results.
 
 ```python
 def scan_z(lens, analysis, dz_range, steps):
 
-    # Make a backup
-    lens.backup()
-
     # Store the original pose
     original_pose = lens.pose.copy()
 
     # Store the results here
     results_history = []
 
     # Iterate over the lens location in the z axis
@@ -1201,43 +1091,28 @@
         # Run analysis
         results = setup.run(analysis)
         results = {"dz": dz, "results": results}
 
         # Store them
         results_history.append(results)
 
-    lens.restore()
-
     return results_history
 
 results = scan_z(lens, analysis, (-1, 1), 0.1)
 ```
 
 Similarly, you will be able to perform grid scan, changing multiple parameters together.
-If we want, we can always store a version of the system at each iteration and restore it afterwards:
-
-```python
-for i, config in lens_configs:
-    lens.change_config(**config)
-    lens.backup(name = i)
-    results = setup.run(analysis)
-    results_history.append(results)
-
-# Choose the best version
-lens.restore(name = best_i)
-```
 
 #### Optimizations
 
 If you have a merit or loss function you wish to optimize or minimize, consider using `tdo.optimize`.
 Here are few examples:
 
 ```python
 import threed_optix.optimize as opt
-import threed_optix.utils as tu
 
 def loss(new_yz):
 
     # Define absolute new pose
     y, z = new_yz
     new_pose = original_pose.copy()
     new_pose[1] = y
@@ -1246,25 +1121,24 @@
     # Change len's pose
     lens.change_pose(new_pose)
 
     # Run analysis
     results = setup.run(analysis)
 
     # Get the right image
-    image = results[550]['X']
+    image = results.data[1] # Assuming that the second line is the matrix of interst
 
     # Calculate spot size can be any function that returns a scalar you want to minimize.
-    spot_size_diameter = tu.calculate_spot_size(image)
+    spot_size_diameter = tdo.calculate_spot_size(image)
 
     print(f"dz: {dz}, dy: {dy}, spot size: {spot_size_diameter}")
     return spot_size_diameter
 
 # Assuming the initial guess is the current lens position
 lens = setup.get('lens1')
-lens.backup(name = 'before_optimization')
 original_pose = lens.pose.copy()
 
 y = original_pose[1]
 z = original_pose[2]
 initial_guess = [y, z]
 
 # Define bounds to avoid getting out of desired range
@@ -1273,17 +1147,14 @@
 low_z = z -1
 high_z = z + 1
 bounds = [(low_y, high_y), (low_z, high_z)]
 
 # Execute search
 result = opt.minimize(loss, initial_guess, method='Nelder-Mead', bounds = bounds)
 
-# Restore backup values
-lens.restore(name = 'before_optimization')
-
 # Get the optimized values
 best_y, best_z = result.x
 
 # Output the best values found
 print(f"Best z: {best_z}, Best y: {best_y}")
 
 best_pose = original_pose.copy()
@@ -1292,40 +1163,14 @@
 lens.change_pose(best_pose)
 ```
 
 Ofcourse, the optimization will be done up to the point where there is no change in the pixel radius.
 In order to bypass this, you could make the detector smaller and smaller as the iteration goes.
 If you do so, you should return the absolute value, rather then pixel one.
 
-```python
-detector = setup['detector_id']
-lens = setup['lens_id']
-
-def loss(new_yz):
-    y, z = new_yz
-    new_pose = detector.pose
-    new_pose[1] = y
-    new_pose[2] = z
-    # Change len's pose
-    lens.change_pose(new_pose)
-    # Run analysis
-    results = setup.run(analysis)
-    # Get the right image
-    image = results[550]['X']
-    # Calculate spot size can be any function that returns a scalar you want to minimize.
-    pixel_radius, center = tu.encircled_energy(image, percent = 0.9)
-    # Assuming your resolution and detector size are squares. Otherwise, ofcourse, further modifications are required.
-    absolute_radius = tu.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius
-    # Make the detector smaller to increase optimization accuracy
-    size = max(min(absolute_radius * 5, 200), minimum_search_size)
-    detector.change_size([size, size])
-
-    return absolute_radius
-```
-
 #### Matlab code
 
 If you have a **general** matlab code you wish to use in our SDK, you could simply translate it to python. We recommend using `matlab2python` library from the github repo:
 
 ```bash
 pip install matlab2python@git+https://github.com/ebranlard/matlab2python.git#egg=m
 atlab2python
@@ -1344,19 +1189,10 @@
 print(pylines)
 ```
 
 > **Warning**
 > This is an external library that's not part of our SDK, nor was built by us.
 > Use output code with caution.
 
-#### Send Feedback
-
-We would love to hear you feedback and suggestions.
-Please send any thoughts and ideas you have to us by using `client.feedback()` method.
-
-```python
-client.feedback('Thanks for reading so far!')
-```
-
 # License
 
 3DOptix API is available with [MIT License](https://choosealicense.com/licenses/mit/).
```

### Comparing `threed_optix-5.0.2/help/SDK help.md` & `threed_optix-5.0.4/help/SDK help.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Optical Simulation SDK
-
 ## Begin
 
 Our optical simulation SDK is released in a beta version and has only limited features support at the moment.
 We are working on supporting more features and you can expect new versions to come out soon.
 
 #### Install
 
@@ -45,21 +44,14 @@
 `tdo.Setup` are the objects that represent your simulation setups in the SDK.
 You could access their information:
 
 - `setup.name` is the setup name. It is not neceseraliy unique.
 - `setup.id` is the id of the setup. It is unique.
 - `setup.parts` is a list of `tdo.Part` objects that the setup contains.
 
-#### Get a list of your 3DOptix setups:
-
-```python
-#'setups' will be a list of your simulation setups as a `tdo.Setup` objects
-setups = client.get_setups()
-```
-
 #### Create a `tdo.Setup`
 
 You could create a new setup with `client.create_setup` method. The method has the following arguments:
 - `name`: str, The name of the setup.
 - `description`: str, The description of the setup.
 - `labels`: list[str], the labels of the setup. Can be anything from `tdo.SETUP_LABELS`.
 - `units`: str, 'mm' or 'inch'. Default to 'mm'.
@@ -74,16 +66,16 @@
 
 #### Find a setup:
 
 First, we need to identify the setup we want to work on:
 
 ```python
 #Examine the setups:
-for s in setups:
-    print(s.name, s.id)
+for setup in client:
+    print(setup.name, setup.id)
 ```
 
 > **Note**
 > A setup id is unique, but the name is not unique
 
 Then, we can get the setup object by using `client.get(name)` and `client[id]` methods:
 
@@ -93,44 +85,23 @@
 setup = client.get(setup_name)
 
 #Get setup by id
 setup_id = '<your setup id'
 setup = client[setup_id]
 ```
 
-If the setups is not found, `client[setup_id]` **will** lead to an error, and `client.get(setup_name)` will **not**.
-
-Another way to do this is by looping over the setps list:
-
-```python
-#Chosen setup id
-setup_id = '<your setup id>'
-
-#Get the 'Setup' object to work on
-setup = None
-for s in setups:
-    #Get your setup by name
-    if s.id == setup_id:
-        setup = s
-        break
-
-assert setup is not None, "Setup was not found"
-```
-
 ### Parts:
 
 `tdo.Part` are the objects that represent your setup parts in the SDK.
 You could access their information:
 
 - `part.label` is the label of the part. It is not neceseraliy unique.
 - `part.id` is the id of the setup. It is unique.
 - `part.surfaces` is a list of `tdo.Surface` objects that the part has.
 - `part.pose` is a list of 6 floats representing the part's position and rotation relative to their associated coordinate system.
-- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
-- `part.optical_data` in the case that the part is `tdo.Optic` part.
 
 > **Warning**
 > Setups with parts that were loaded from a CAD file are not supported fully at the moment.
 > These CAD parts will not lead to an error, but they might lead to unexpected behavior.
 
 `tdo.Detector` is the object used to represent detectors. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing detectors within the SDK.
 `tdo.Detector` has the following additional information:
@@ -147,39 +118,42 @@
 - `ls.vis_count`
 - `ls.count_type`
 - `ls.opacity`
 - `ls.color`
 - `ls.source_type`
 - And information that changes with respect to `source_type`.
 
+`tdo.Optic` is the object used to represent optics. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing optics within the SDK.
+`tdo.Optic` has the following additional information:
+- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
+- `part.optical_data` contains all the data that's specific to the optical properties of the part, such as its geometry, shape, brand, physical data, etc.
+
+
 **You could see a full description of these objects, as well as how to modify them, later on this document**.
 
 #### Add a `tdo.Part`:
 To add a detector to the setup:
 ```python
-detector = setup.add_detector(label = label,
-                              pose = pose)
+detector = setup.add_detector(**kwargs)
 ```
 
 To add a light source to the setup:
 ```python
-ls = setup.add_light_source(label = label,
-                              pose = pose)
+ls = setup.add_light_source(**kwargs)
 ```
 
 To add optic to the setup, we will have to find its `db_id` from the product catalog or take the number id of the created optic from `client.create_xxx` methods.
 ```python
 ls = setup.add_optics(db_id = db_id,
-                            label = label,
-                            pose = pose)
+                      **kwargs)
 ```
 You could get the part number id in the `ID` column in the product catalog, or take the number id of the part you created.
 
 >> **Note**
->> You can add parts with any keywords from part.change_config to add and change properties with the same command.
+>> You can add parts with any keyword arguments from part.change_config to add and change properties with the same command.
 
 #### Find a part:
 
 Almost identical to finding a setup.
 
 ```python
 #Examine the parts of the setup
@@ -200,47 +174,30 @@
 #Get part by id
 part_id = '<your part id'
 part = setup[part_id]
 ```
 
 If the part is not found, `setup[part_id]` **will** lead to an error, and `setup.get(part_label)` will **not**.
 
-Or, alternatively, looping over the `tdo.Setup` object:
-
-```python
-#Chosen part id
-part_id = '<the id of the part to change>'
-
-#Get the 'Part' object to work on
-part = None
-for p in setup:
-    #Get part by id
-    if p.id == part_id:
-       part = p
-       break
-
-assert part is not None, "Part was not found"
-```
-
 #### Delete a part from the setup:
 In order to remove a part from the setup, we simply use `setup.delete_part` method as follows:
 ```python
-part_to_delete = setup.get('<part_to_delete_label')
+part_to_delete = setup.get('<part_to_delete_label>')
 setup.delete_part(part_to_delete)
 ```
 And that's it! The part is removed from the setup.
 
 ### Surface
 
 `tdo.Surface` are the objects that represent the surfaces of the part in the SDK.
 You could access their information:
 
 - `surface.name` is the name of the surface. It is not neceseraliy unique.
 - `surface.id` is the id of the setup. It is unique.
-- `surface.analyses` is a list of `tdo.Analysis` objects that the surface has. Later on we discuss how to add new and run them.
+- If the surface is the front of a detector, you could access the analyses with `surface.analyses`. It is a list of `tdo.Analysis` objects that the surface has. Later on we discuss how to create, find and run them.
 
 #### Create or add a `tdo.Surface`
 
 Creation of new surfaces is not possible.
 
 #### Find a surface:
 
@@ -259,94 +216,76 @@
 surface = part.get(surface_name)
 
 #Get surface by id
 surface_id = '<your surface id>'
 surface = part[surface_id]
 ```
 
-If the surface is not found, `part[surface_id]` **will** lead to an error, and `part.get(surface_name)` will **not**.
-
-Or looping over the part:
-
-```python
-#Choose surface id
-surface_id = '<the id of the surface to perform analysis on>'
-
-#Get the 'tdo.Surface' object:
-surface = None
-for s in part:
-    #Get surface by id
-    if s.id == surface_id:
-      surface = s
-      break
-
-assert surface is not None, "Surface was not found"
-```
-
 ### Scattering
 Each surface of `tdo.Optic` part can have scattering properties.
 To examine them, check `surface.scattering` property.
 If the surface does not have scattering, it will return `False`.
 #### Disable Surface Scattering
-If a surface has a scattering that you want to disable, simply use `surface.disable_scatterin` method.
+If a surface has a scattering that you want to disable, simply use `surface.disable_scattering` method.
 ```python
 surface.diasble_scattering()
 if not surface.scattering:
     print('Success!')
 ```
 #### Add Or Change Scattering
 Scattering can be added or changed with `surface.XXX_scattering` methods.
 Each of them acccepts the following arguments:
-- `transmittance`, `absorption`, `reflection`: float, The relative part of transmittance, absorption and reflection of the scattering.
-- `num_of_rays`: int,
-- `relative_power_threshold`: float,
+- `transmittance`, `absorption`, `reflection`: float, The proportion of  the light that is transmitted, absorbed and reflected by the surface.
+- `split_ratio`: int, number of ray that each ray split to.
+- `power_threshold`: float, Relative power threshold used for terminating the ray tracing simulation. It represents the minimum amount of remaining power below which rays are terminated.
+
 ##### Cos-nth
 Requires also `n` parameter, which defaults to 1.5.
 ```python
 surface.cos_scattering(transmittance = 0.5,
                         reflection = 0.3,
                         absorption = 0.1,
-                        num_of_rays = 10,
-                        relative_power_threshold = 5,
+                        split_ratio = 10,
+                        power_threshold = 5,
                         n = 2)
 ```
 ##### Gaussian
 Requires also `sigma_x`, `sigma_y` and `azimuth_theta` parameters.
 ```python
 surface.gaussian_scattering(transmittance = 0.99,
                             reflection = 0.01,
                             absorption = 0,
-                            num_of_rays = 5,
-                            relative_power_threshold = 2
+                            split_ratio = 5,
+                            power_threshold = 2
                             sigma_x = 10,
                             sigma_y = 15,
                             azimuth_theta = 0)
 ```
 
 ##### ABG
 Requires also `a`, `b` and `g` parameters.
 ```python
 surface.abg_scattering(transmittance = 0.95,
                             reflection = 0.025,
                             absorption = 0.025,
-                            num_of_rays = 7,
-                            relative_power_threshold = 4
+                            split_ratio = 7,
+                            power_threshold = 4
                             a = 1,
                             b = 2,
                             g = 2)
 ```
 
 ##### Lambertian
 Does not require unique parameters.
 ```python
-surface.lembertian_scattering(transmittance = 0.97,
+surface.lambartian_scattering(transmittance = 0.97,
                             reflection = 0.03,
                             absorption = 0.01,
-                            num_of_rays = 10,
-                            relative_power_threshold = 5,
+                            split_ratio = 10,
+                            power_threshold = 5,
                             )
 ```
 
 ### Coordinate Systems
 #### Part Coordinate System
 You can see all of the coordinate systems that a part has in `part.cs` list.
 Every `CoordinateSystem` object has `name`, `pose`, and `id` properties.
@@ -355,38 +294,38 @@
 for cs in part.cs:
     print(cs.name, cs.id, cs.pose)
 
 lcs = part.lcs
 rcs, reference_part = part.rcs
 ```
 #### The World Coordinate System
-The world coordinate system is stored in `tdo.WORLD` object. You can use it as a coordinate system.
+The world coordinate system is stored in `tdo.GLOBAL` object. You can use it as a coordinate system.
 
 #### Change lcs and rcs
 You can change lcs and rcs with `part.change_cs` method. It accepts the following arguments:
 - `lcs`: CoordinateSystem, if defined, it will be the new local coordinate system of the part.
-- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part.
+- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part. use `tdo.GLOBAL` cs to defined the global cs as the rcs.
 ```python
 lens.change_cs(lcs = lens.cs[1])
 detector.change_cs(rcs = lens.cs[0])
-ls.change_cs(lcs = ls.cs[0], rcs = tdo.WORLD)
+ls.change_cs(lcs = ls.cs[0], rcs = tdo.GLOBAL)
 ```
 
 ### Materials
 #### Find Materials From Database
 Some mmethods require specific materials from our database. In order to find them, use `client.search_materials` method.
 ```python
 materials = client.search_materials('N-BK7')
 ```
-`materials` is now a list of `Material` object.
+`materials` is now a list of `tdo.Material` object.
 ```python
 for m in materials:
     m.describe()
 ```
-Finally, you can use the chosen material object or directly in the material id.
+Finally, you can use the chosen material object or its material id directly.
 
 ### Analysis
 `tdo.Analysis` are the objects that represent analyses that can be performed on a surface.
 They are defined by:
 
 - `id`: The unique id of the analysis.
 - `surface`: The `tdo.Surface` object on which the analysis will be made.
@@ -397,15 +336,15 @@
 A surface can contain several analysis with identical properties and different ids.
 However, each analysis consumes your account resources, since analysis id holds its results.
 When you run the analysis again, the last result is deleted from 3DOptix systems.
 So, we reccomend storing iterations of the same analysis locally and use duplicated analyses only when you think it's necessary.
 
 #### Find existing analysis
 
-Every new analysis consumes storage resources for you account.
+Every new analysis consumes storage resources for your account.
 So, we reccomend sticking to the same analysis if they have the same properties instead of creating new ones.
 You could get a list of the `tdo.Analysis` of the surface like this:
 
 ```python
 setup = client.get('example')
 detector = setup.get('my_detector')
 detector_front = detector.get('front')
@@ -418,15 +357,14 @@
 ```
 
 Or get an existing analyses with required parameters, if the id doesn't matter:
 
 ```python
 detector_front = setup.get('my_detector').get('front')
 analysis = detector_front.find_analysis(name = name, rays = rays, resolution = resolution)
-assert analysis
 ```
 
 #### Create and add analysis
 
 If you want to create an analysis that doesn't exist for the surface yet, or you want to create a duplicated analysis, we can create one:
 
 ```python
@@ -439,18 +377,22 @@
 
 For example:
 
 ```python
 laser = setup.get('ls')
 surface = detector.get('front')
 
-analysis = tdo.Analysis(
-                        surface = surface,
-                        resolution = [500, 500],
-                        rays = {laser: 1e5},
+analysis1 = tdo.Analysis(surface = surface,
+                        resolution = [100, 200],
+                        rays = {laser: 1e5, laser2: 1e4},
+                        name = "Spot (Incoherent Irradiance)"
+                        )
+analysis2 = tdo.Analysis(surface = surface,
+                        resolution = 100, #for equal height and width pixels
+                        rays = 1e6, #for all of the lasers in the setup
                         name = "Spot (Incoherent Irradiance)"
                         )
 ```
 
 > **Reminder**
 > You can always access all the possible analysis names with `tdo.ANALYSIS_NAMES`
 
@@ -473,42 +415,14 @@
 results = setup.run(analysis)
 analysis.show()
 surface.delete_analysis(analysis)
 ```
 
 ## Make Changes
 
-#### Backup
-
-Before making any changes, we reccomend storing the original part or setup, before any changes:
-
-```python
-#Backup the part
-part = setup.get('part_label')
-part.backup()
-
-#Some code...
-
-#Restore the original state of the part
-part.restore()
-```
-
-In the case of multiple changes to multiple parts, you might find this easier:
-
-```python
-# Backup the setup
-setup = client['setup_id']
-setup.backup()
-
-#Some code...
-
-#Restore the original state of the part
-setup.restore()
-```
-
 #### Transformations
 
 You could move and rotate part using `part.change_pose()` method that moves the part to a location on the three axis (x, y, z) and rotates it in respect to them (alpha, beta, gamma).
 
 All six numbers indicating absolute future value in respect to the part's coordinate system, **not** change and **not** with respect to the global coordinate system.
 if you want to change coordinate systems, please check `part.change_cs` method.
 
@@ -550,27 +464,21 @@
 Detectors have a `detector.change_opacity()` and `detector.change_size()` methods, that changes the detector's opacity and size, accordingly.
 This is how you use them:
 
 ```python
 # Get the detector
 detector = setup.get('detector_label')
 
-#Backup the original detector's state
-detector.backup()
-
 #Apply changes
 detector.change_size([new_half_height, new_half_width])
 detector.change_opacity(new_opacity)
 detector.change_pose([x, y, z, alpha, beta, gamma])
 
 #Verify change
 print(detector.size, detector.opacity, detector.pose)
-
-# Restore if needed
-detector.restore()
 ```
 
 At the beginning, we reccomend frequent sanity-checks in the GUI to make sure you got everything right.
 
 ### Modify Light Sources
 
 #### Change wavelengths
@@ -605,37 +513,32 @@
 
 At the beginning, we reccomend frequent sanity-checks in the GUI to make sure you got everything right.
 
 **Create normal distribution**
 If you want to create wavelengths spectrum with a normal disribution, you could use `tdo.utils.wavelengths_normal_distribution`:
 
 ```python
-import threed_optix.utils as tu
-
 # Define the spectrum
-wavelengths_spectrum = tu.wavelengths_normal_distribution(mean_wavelength, std_dev, num_wavelengths)
+wavelengths_spectrum = tdo.wavelengths_normal_distribution(mean_wavelength, std_dev, num_wavelengths)
 
 # Modify the light source
 light_source.change_wavelengths(wavelengths_spectrum)
 ```
-
 Where:
 
 - `mean_wavelength` is the mean wavelength of the distribution
 - `std_dev` is the standard deveation of the distribution
 - `num_wavelengths` is the number of the wavelengths that will be sampled.
 
 **Create uniform distribution**
 Similarly, If you want to create wavelengths spectrum with a uniform disribution, you could use `tdo.utils.wavelengths_uniform_distribution`:
 
 ```python
-import threed_optix.utils as tu
-
 # Define the spectrum
-wavelengths_spectrum = tu.wavelengths_uniform_distribution(min_wavelength, max_wavelength, num_wavelengths)
+wavelengths_spectrum = tdo.wavelengths_uniform_distribution(min_wavelength, max_wavelength, num_wavelengths)
 
 # Modify the light source
 light_source.change_wavelengths(wavelengths_spectrum)
 ```
 
 Where:
 
@@ -945,61 +848,50 @@
 > Otherwise, choose the existing analysis and run it instead. This helps optimizing your system memory credits usage.
 
 #### Results
 
 Even if we didn't store it in another variable, we can view and analize the latest results in a raw form:
 
 ```python
+# For jupyter notebooks or HTML
+display(analysis.results)
+
+# For scripts
 print(analysis.results)
 ```
 
-The result will be a JSON where each key is a wavelength in the analysis results.
-Each wavelength contains the `np.ndarray` matrices for each polarization.
+The result will be a pandas dataframe (`pd.DataFrame`) with all the different matrices.
+The columns of the dataframe are:
+    - `data`: The matrix of the results for that row's configuration.
+    - `polarization`: The polarization of the data.
+    - `wl`: The wavelength of the data.
+    - `spot_target_kind`: Can be either 'Source', 'Group' or 'Total', indicating if the data is the result of a single source, coherent group or the total results of all the light sources.
+    - `spot_target`: The id of the light source\coherent group.
+
 For example, let's say I am looking for the _"X"_ polarization, _400 nm_ rays hit matrix:
 
 ```python
-matrix = results[400]['X']
+mask = (results.wl == 400) & (results.polarization == 'X')
+matrices = results[mask].data
 ```
-
-For analysis without polarization, polarization kind is "NONE".
+and, ofcourse, any `pd.DataFrame` manipulation will work as usuall.
 
 > **Note**
 > If you plan on running the anlysis again, it is really important to store a deepcopy of analysis.results in the `matrix` variable.
 > Otherwise, the variable will hold the pointer to the `results` property of the analysis, and the previous results will be overriden.
-> Another option is to store the results of `analysis()` in another variable
+> Another option is to store the results of `setup.run(analysis)` in another variable, since it outputs a copy anyway.
 
 If we want to see the matrices as a images, we can simply:
 
 ```python
 #for static figure
-analysis.show()
+tdo.show_matrix(matrix)
 
 #for interactive figure
-analysis.show_interactive()
-```
-
-**Arguments**
-
-- **`upscale`**: Upscales the image (smooth the pixels over) by using `upscale = True`.
-- **`polarizations`**: Presents only selected polarization by passing a list of strings to the argument.
-- **`wavelengths`**: Presents only selected wavelengths by passing a list of integers to the argumet.
-- **`figsize`**: Determines the size of the presented figure in inches.
-
-```python
-analysis.show(upscale = True,
-              polarizations = ['X'],
-              wavelengths = [550, 600],
-              figsize = (15, 15))
-```
-
-```python
-analysis.show_interactive(upscale = True,
-                          polarizations = ['Y', 'Z'],
-                          wavelengths = [500, 700],
-                          figsize = (20, 20))
+tdo.show_matrix(matrix, interactive = True)
 ```
 
 ## Create a new `tdo.Optics` in your product catalog
 As for now, the SDK supports creating spherical and conic lenses.
 ### Create Lenses
 #### Spherical Lenses
 To create spherical lens, we can use `client.create_spherical_lens` method. The arguments are:
@@ -1051,25 +943,25 @@
 - `r1_x`, `r1_y`: float, the first radius of curvature.
 - `r2_x`, `r2_y`: float, the second radius of curvature.
 - `k1_x`, `k1_y`, `k2_x`, `k2_y`: float, the conic coefficients of the lens. Default to 0.
 
 The method returns the number id of the created element.
 ```python
 lens_db_id = client.create_spherical_lens(name = name,
-                                              material = material,
-                                              diameter = diameter,
-                                              thickness = thickness,
-                                              r1_x = r1_x,
-                                              r1_y = r1_y,
-                                              r2_x = r2_x,
-                                              r2_y = r2_y,
-                                              k1_x = k1_x,
-                                              k1_y = k1_y,
-                                              k2_x = k2_x,
-                                              k2_y = k2_y)
+                                          material = material,
+                                          diameter = diameter,
+                                          thickness = thickness,
+                                          r1_x = r1_x,
+                                          r1_y = r1_y,
+                                          r2_x = r2_x,
+                                          r2_y = r2_y,
+                                          k1_x = k1_x,
+                                          k1_y = k1_y,
+                                          k2_x = k2_x,
+                                          k2_y = k2_y)
 ```
 ### Create Grating
 You can create a new grating in the database with `client.create_grating` method.
 It requires the following arguments:
 - `name`: str, The name of the grating in the database.
 - `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
 - `grooves`: int, Number of grooves on the grating.
@@ -1115,46 +1007,44 @@
 ## Advanced
 ### Utils Module
 #### Get spot size
 
 `tdo.utils.calculate_spot_size(matrix)` calculates the diameter of the blocking circle of the biggest contours of the matrix, in pixels.
 
 ```python
-import threed_optix.utils as tu
 
 # Assuming that this analysis exists already
 setup = client['setup_id']
 detector = setup.get('detector_label')
 detector_front = detector.get('front')
 
 analysis = detector_front.analysis_with(name ="Spot (Incoherent Irradiance)",
                                         rays = {laser1: 2.5e6, laser2: 2.5e6},
                                         resolution = (1000, 1000)
                                         )
 # Run the analysis
 results = setup.run(analysis)
 
 # Calculate spot size
-matrix = results[550]['X']
-spot_size_dia = tu.calculate_spot_size(matrix)
+spot_size_dia = tdo.calculate_spot_size(results.data[0])
 print(f'Analysis spot size diameter for X polarization at 550 nm is {spot_size_dia}')
 ```
 
 `tdo.utils.encircled_energy(matrix, percent)` calculates the diameter of the circle that centers at the center of energy mass, and contains `percantage` of the matrix's total energy.
 
 ```python
-encircled_energy_radius, center = tu.encircled_energy(matrix, 0.9)
-print(f'Analysis encircled 90% energy radius for X polarization at 550 nm is {encircled_energy_radius}')
+encircled_energy_radius, center = tdo.encircled_energy(matrix, 0.9)
+print(f'Analysis encircled 90% energy radius for X polarization at 550 nm is {encircled_energy_radius} with the center at {center}')
 ```
 
-Of course, these values are pixel values. In order to get absolute values, use `tdo.utils.absolute_pixel_size`:
+Of course, these values are pixel values. In order to get absolute values in length units, use `tdo.utils.absolute_pixel_size`:
 
 ```python
-pixel_radius, center = tu.encircled_energy(matrix, 0.95)
-absolute_radius = tu.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius
+pixel_radius, center = tdo.encircled_energy(matrix, 0.95)
+absolute_radius = tdo.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius # Assuming that the resolution is symmetrical
 print(f'95% Encircled energy radius is {absolute_radius} mm')
 ```
 
 #### Scans
 
 In order to perform a scan, all we need to do is to define an analysis:
 
@@ -1178,17 +1068,14 @@
 ```
 
 Then, we need to iteratively change the properties of some part in the setup and store the results.
 
 ```python
 def scan_z(lens, analysis, dz_range, steps):
 
-    # Make a backup
-    lens.backup()
-
     # Store the original pose
     original_pose = lens.pose.copy()
 
     # Store the results here
     results_history = []
 
     # Iterate over the lens location in the z axis
@@ -1204,43 +1091,28 @@
         # Run analysis
         results = setup.run(analysis)
         results = {"dz": dz, "results": results}
 
         # Store them
         results_history.append(results)
 
-    lens.restore()
-
     return results_history
 
 results = scan_z(lens, analysis, (-1, 1), 0.1)
 ```
 
 Similarly, you will be able to perform grid scan, changing multiple parameters together.
-If we want, we can always store a version of the system at each iteration and restore it afterwards:
-
-```python
-for i, config in lens_configs:
-    lens.change_config(**config)
-    lens.backup(name = i)
-    results = setup.run(analysis)
-    results_history.append(results)
-
-# Choose the best version
-lens.restore(name = best_i)
-```
 
 #### Optimizations
 
 If you have a merit or loss function you wish to optimize or minimize, consider using `tdo.optimize`.
 Here are few examples:
 
 ```python
 import threed_optix.optimize as opt
-import threed_optix.utils as tu
 
 def loss(new_yz):
 
     # Define absolute new pose
     y, z = new_yz
     new_pose = original_pose.copy()
     new_pose[1] = y
@@ -1249,25 +1121,24 @@
     # Change len's pose
     lens.change_pose(new_pose)
 
     # Run analysis
     results = setup.run(analysis)
 
     # Get the right image
-    image = results[550]['X']
+    image = results.data[1] # Assuming that the second line is the matrix of interst
 
     # Calculate spot size can be any function that returns a scalar you want to minimize.
-    spot_size_diameter = tu.calculate_spot_size(image)
+    spot_size_diameter = tdo.calculate_spot_size(image)
 
     print(f"dz: {dz}, dy: {dy}, spot size: {spot_size_diameter}")
     return spot_size_diameter
 
 # Assuming the initial guess is the current lens position
 lens = setup.get('lens1')
-lens.backup(name = 'before_optimization')
 original_pose = lens.pose.copy()
 
 y = original_pose[1]
 z = original_pose[2]
 initial_guess = [y, z]
 
 # Define bounds to avoid getting out of desired range
@@ -1276,17 +1147,14 @@
 low_z = z -1
 high_z = z + 1
 bounds = [(low_y, high_y), (low_z, high_z)]
 
 # Execute search
 result = opt.minimize(loss, initial_guess, method='Nelder-Mead', bounds = bounds)
 
-# Restore backup values
-lens.restore(name = 'before_optimization')
-
 # Get the optimized values
 best_y, best_z = result.x
 
 # Output the best values found
 print(f"Best z: {best_z}, Best y: {best_y}")
 
 best_pose = original_pose.copy()
@@ -1295,40 +1163,14 @@
 lens.change_pose(best_pose)
 ```
 
 Ofcourse, the optimization will be done up to the point where there is no change in the pixel radius.
 In order to bypass this, you could make the detector smaller and smaller as the iteration goes.
 If you do so, you should return the absolute value, rather then pixel one.
 
-```python
-detector = setup['detector_id']
-lens = setup['lens_id']
-
-def loss(new_yz):
-    y, z = new_yz
-    new_pose = detector.pose
-    new_pose[1] = y
-    new_pose[2] = z
-    # Change len's pose
-    lens.change_pose(new_pose)
-    # Run analysis
-    results = setup.run(analysis)
-    # Get the right image
-    image = results[550]['X']
-    # Calculate spot size can be any function that returns a scalar you want to minimize.
-    pixel_radius, center = tu.encircled_energy(image, percent = 0.9)
-    # Assuming your resolution and detector size are squares. Otherwise, ofcourse, further modifications are required.
-    absolute_radius = tu.absolute_pixel_size(detector.size, analysis.resolution)[0] * pixel_radius
-    # Make the detector smaller to increase optimization accuracy
-    size = max(min(absolute_radius * 5, 200), minimum_search_size)
-    detector.change_size([size, size])
-
-    return absolute_radius
-```
-
 #### Matlab code
 
 If you have a **general** matlab code you wish to use in our SDK, you could simply translate it to python. We recommend using `matlab2python` library from the github repo:
 
 ```bash
 pip install matlab2python@git+https://github.com/ebranlard/matlab2python.git#egg=m
 atlab2python
@@ -1347,19 +1189,10 @@
 print(pylines)
 ```
 
 > **Warning**
 > This is an external library that's not part of our SDK, nor was built by us.
 > Use output code with caution.
 
-#### Send Feedback
-
-We would love to hear you feedback and suggestions.
-Please send any thoughts and ideas you have to us by using `client.feedback()` method.
-
-```python
-client.feedback('Thanks for reading so far!')
-```
-
 # License
 
 3DOptix API is available with [MIT License](https://choosealicense.com/licenses/mit/).
```

### Comparing `threed_optix-5.0.2/setup.py` & `threed_optix-5.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     keywords=["Optics", "Optical Design", "Optical Simulation", "Optical Design Software", "3DOptix"],
     install_requires=[
         'requests',
         'pandas',
         'matplotlib',
         'plotly',
         'colorama',
-        'nbformat',
         'numpy',
         'scikit-image',
         'scipy',
         'opencv-python',
         'dill',
         "ply",
         "networkx",
```

### Comparing `threed_optix-5.0.2/src/threed_optix/__init__.py` & `threed_optix-5.0.4/src/threed_optix/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .client import ThreedOptixAPI, Client
+from .client import ThreedOptixAPI, Client, Material
 from .analyses import Analysis
 from .simulations import Setup
-from .parts import Part, Surface, LightSource, Detector, WORLD
+from .parts import Part, Surface, LightSource, Detector, GLOBAL
 from .utils import *
 from . import package_utils
 from . import optimize
 
 # Allow users to easily access the enums
 from .package_utils.vars import eOpticsSubtypes, ANALYSIS_NAMES, Setups, Coating, SETUP_LABELS
+
 GRATING_SUBTYPES = eOpticsSubtypes.GRATING_SUBTYPES
 SETUP_LABELS = Setups.SETUP_LABELS
 
 # Enter debug mode, which will print out pretty much every step of the way.
 def debug(boolean = None):
 
     # If the user has specified a boolean, set the debug mode to that value.
```

### Comparing `threed_optix-5.0.2/src/threed_optix/analyses.py` & `threed_optix-5.0.4/src/threed_optix/analyses.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix/beams.py` & `threed_optix-5.0.4/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix/client.py` & `threed_optix-5.0.4/src/threed_optix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,25 +134,25 @@
         materials_data = au._get_materials(api_key=self.api_key,
                                            material_name=material_name)
         # Create the Material objects
         materials = [Material._new(_api=self, _data=material_data) for material_data in materials_data['materials']]
         return materials
 
     def create_setup(self,
-                     name,
-                     description,
-                     labels,
-                     units = 'mm',
-                     private = False,
-                     associated = False,
-                     link = None,
-                     title = None,
-                     authors = None,
-                     journal = None,
-                     abstract = None,
+                     name: str,
+                     description: str,
+                     labels: List[str],
+                     units: str = 'mm',
+                     private: bool = False,
+                     associated: bool = False,
+                     link: str = None,
+                     title: str= None,
+                     authors: str = None,
+                     journal: str = None,
+                     abstract: str = None,
                      ):
         '''
         This function creates a new setup with the specified parameters.
         Args:
             name (str): The name of the setup.
             description (str): The description of the setup.
             labels (list): The labels of the setup. enum is in `tdo.SETUP_LABELS`
@@ -174,14 +174,23 @@
             if not set(labels).issubset(set(v.SETUP_LABELS)):
                 errors.append(f"""All labels must one of {', '.join(v.SETUP_LABELS)}""")
 
             # Check if the units are valid
             if units not in v.SETUP_UNITS:
                 errors.append(f"""Units must be one of {', '.join(v.SETUP_UNITS)}""")
 
+            if len(name) == 0:
+                errors.append("Name cannot be empty")
+
+            if len(description) == 0:
+                errors.append("Description cannot be empty")
+
+            if len(labels) == 0:
+                errors.append("Labels cannot be empty")
+
             return errors
 
         # Verify the parameters
         errors = verify()
         # Raise an exception if there are errors
         if len(errors) > 0:
             raise Exception('\n'.join(errors))
@@ -847,19 +856,19 @@
         return parts
 
     def _get_part(self, part_id: str, setup_id) -> dict:
         '''
         Private.
         Shouldn't be called directly. Returns a dictionary of the specified part.
         '''
-        part = au._get_part(setup_id,part_id,  self.api_key)[0]
-        if part is None:
+        part = au._get_part(setup_id,part_id,  self.api_key)
+        if part[0] is None:
             raise Exception(f"Part with id {part_id} not found.")
 
-        return part
+        return part[0]
 
     def _extract_setup_object(self, setup):
         '''
         Private.
         Shouldn't be called directly. Returns the setup object from the specified setup.
         '''
         if isinstance(setup, str):
```

### Comparing `threed_optix-5.0.2/src/threed_optix/package_utils/api.py` & `threed_optix-5.0.4/src/threed_optix/package_utils/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix/package_utils/general.py` & `threed_optix-5.0.4/src/threed_optix/package_utils/general.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.4/src/threed_optix/package_utils/math.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix/package_utils/vars.py` & `threed_optix-5.0.4/src/threed_optix/package_utils/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import numpy as np
 import re
 
 DEBUG = False
 BASE_BACKUP = 'DEFAULT'
 VALID_RESPONSE_CODES = [200, 201, 202, 204]
 # Take the version of the package
-VERSION = "5.0.2"
+VERSION = "5.0.4"
 
 
 #Base API URL
 API_URL = "https://api.3doptix.com/v1"
 
+class Surfaces:
+    DETECTOR_FRONT = 'front'
+
 class Analyses:
     DEFAULT_NUM_RAYS = 30
 
 class Endpoints:
     GET_MATERIALS_ENDPOINT = 'material/name/{material_name}'
     GET_SURFACE_DATA = 'setups/{setup_id}/parts/{part_id}/surfaces/{surface_id}'
     DELETE_ANALYSIS = 'setups/{setup_id}/parts/{part_id}/surfaces/{surface_id}/analyses/{analysis_id}'
@@ -571,15 +574,15 @@
     }
 
 class APIMessages:
     PART_MODIFIED = 'Part Modified'
 
 class CoordinateSystems:
     WORLD = 0
-    WORLD_DATA = {'ref_pose': {'position': [0, 0, 0], 'rotation': [0, 0, 0]}, 'name': 'World'}
+    WORLD_DATA = {'ref_pose': {'position': [0, 0, 0], 'rotation': [0, 0, 0]}, 'name': 'Global'}
 
 class ScatteringModels:
     LAMBERTIAN = "LAMBERTIAN"
     GAUSSIAN = "GAUSSIAN"
     COS_NTH = "COS_NTH"
     ABG = "ABG"
 class Scattering:
```

### Comparing `threed_optix-5.0.2/src/threed_optix/parts.py` & `threed_optix-5.0.4/src/threed_optix/parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,30 @@
         return self._data.get('name', '')
 
 class WorldCS(CoordinateSystem):
     @classmethod
     def _new(cls):
         return super()._new(id = v.CoordinateSystems.WORLD, _data = v.CoordinateSystems.WORLD_DATA, part = None)
 
-WORLD = WorldCS._new()
+GLOBAL = WorldCS._new()
 
 class Surface:
     def __init__(self):
         '''
         Private
         '''
         raise TypeError("Cannot directly create an instance of Surface.")
 
     @classmethod
     def _new(cls, _part, _data):
         '''
         Private
         '''
+        if v.DEBUG:
+            print(f'Creating general surface')
         surface = object.__new__(cls)
         surface.name = _data['name']
         surface.id = _data['id']
         surface._part = _part
         surface._analyses = None
         surface._data = None
         return surface
@@ -72,35 +74,43 @@
                                  type = analysis['type'],
                                  name = analysis['name'],
                                  )
                 for id, analysis in analysis_data.items()
                 ]
         return self._analyses
 
-
-
     def __str__(self):
         '''
         Returns a string representation of the surface: name, id, part id, and part label.
         '''
         string = f'Surface with {len(self.analyses)} analyses:\n'
         for analysis in self.analyses:
             string += f'''{analysis.name} ({analysis.id})\n'''
         return string
 
+class DetectorSurface(Surface):
+
+    @classmethod
+    def _new(cls, _part, _data):
+        if v.DEBUG:
+            print(f'Creating detector front')
+        surface_obj = super()._new(_part, _data)
+        surface_obj.__dict__ = surface_obj.__dict__
+        return surface_obj
+
     def find_analysis(self, name: str, rays: Union[dict, int], resolution: Union[tuple, list]):
 
         if isinstance(rays, int):
             rays = {ls: rays for ls in self._part._setup.light_sources}
 
         wanted_analysis = an.Analysis(surface = self, resolution = resolution, name = name, rays = rays)
         for analysis in self.analyses:
             if analysis == wanted_analysis:
                 return analysis
-        return None
+        raise KeyError(f"Analysis with name {name} not found in surface.")
 
     def add_analysis(self, analysis: an.Analysis, force = False):
         data = self._part._setup._api._add_analysis(analysis, force = force)
         analysis._added = True
         analysis.id = data['id']
         self.analyses.append(analysis)
         return
@@ -149,26 +159,26 @@
         self._part._change_scattering(surface_id = self.id, scattering = scattering)
         self.data['scattering'] = scattering
 
     def change_scattering(self,
                           transmittance,
                           reflectance,
                           absorption,
-                          num_of_rays,
-                          relative_power_threshold,
+                          split_ratio,
+                          power_threshold,
                           scatter_model,
                           bsdf = None
                           ):
 
         parameters = {
             "transmittance": transmittance,
             "reflectance": reflectance,
             "absorption": absorption,
-            "numberOfRays": num_of_rays,
-            "relativePowerThreshold": relative_power_threshold,
+            "numberOfRays": split_ratio,
+            "relativePowerThreshold": power_threshold,
             "scatterModel": scatter_model,
         }
 
         if bsdf is not None:
             parameters['bsdfParams'] = bsdf
 
         scattering_data = {
@@ -183,59 +193,59 @@
         self.data['scattering'] = scattering
         return None
 
     def lambartian_scattering(self,
                           transmittance = v.Scattering.DEFAULT_TRANS,
                           reflectance = v.Scattering.DEFAULT_REF,
                           absorption = v.Scattering.DEFAULT_ABS,
-                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
-                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                          split_ratio = v.Scattering.DEFAULT_NUMBER_OF,
+                          power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
                           ):
 
         scatter_model = v.ScatteringModels.LAMBERTIAN
         self.change_scattering(transmittance = transmittance,
                                reflectance = reflectance,
                                absorption = absorption,
-                               num_of_rays = num_of_rays,
-                               relative_power_threshold = relative_power_threshold,
+                               split_ratio = split_ratio,
+                               power_threshold = power_threshold,
                                scatter_model = scatter_model,
                                )
 
     def abg_scattering(self,
                           transmittance = v.Scattering.DEFAULT_TRANS,
                           reflectance = v.Scattering.DEFAULT_REF,
                           absorption = v.Scattering.DEFAULT_ABS,
-                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
-                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                          split_ratio = v.Scattering.DEFAULT_NUMBER_OF,
+                          power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
                           a = v.Scattering.DEFAULT_A,
                           b  =v.Scattering.DEFAULT_B,
                           g = v.Scattering.DEFAULT_G
                           ):
 
         scatter_model = v.ScatteringModels.ABG
         bsdf = {
             "a": a,
             "b": b,
             "g": g
         }
         self.change_scattering(transmittance = transmittance,
                                reflectance = reflectance,
                                absorption = absorption,
-                               num_of_rays = num_of_rays,
-                               relative_power_threshold = relative_power_threshold,
+                               split_ratio = split_ratio,
+                               power_threshold = power_threshold,
                                scatter_model = scatter_model,
                                bsdf=bsdf
                                )
 
     def gaussian_scattering(self,
                           transmittance = v.Scattering.DEFAULT_TRANS,
                           reflectance = v.Scattering.DEFAULT_REF,
                           absorption = v.Scattering.DEFAULT_ABS,
-                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
-                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                          split_ratio = v.Scattering.DEFAULT_NUMBER_OF,
+                          power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
                         sigma_x = v.Scattering.DEFAULT_SIGMAX,
                         sigma_y = v.Scattering.DEFAULT_SIGMAY,
                         azimuth_theta = v.Scattering.DEFAULT_AZIMUTH_THETA
                         ):
 
         scatter_model = v.ScatteringModels.GAUSSIAN
         bsdf = {
@@ -243,39 +253,39 @@
             "sigmaY": sigma_y,
             "azimuth_theta": azimuth_theta
             }
 
         self.change_scattering(transmittance = transmittance,
                                reflectance = reflectance,
                                absorption = absorption,
-                               num_of_rays = num_of_rays,
-                               relative_power_threshold = relative_power_threshold,
+                               split_ratio = split_ratio,
+                               power_threshold = power_threshold,
                                scatter_model = scatter_model,
                                bsdf=bsdf
                                )
 
     def cos_scattering(self,
                         transmittance = v.Scattering.DEFAULT_TRANS,
                         reflectance = v.Scattering.DEFAULT_REF,
                         absorption = v.Scattering.DEFAULT_ABS,
-                        num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
-                        relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                        split_ratio = v.Scattering.DEFAULT_NUMBER_OF,
+                        power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
                         n = v.Scattering.DEFAULT_N
                         ):
 
         scatter_model = v.ScatteringModels.COS_NTH
         bsdf = {
             "n": n
             }
 
         self.change_scattering(transmittance = transmittance,
                                reflectance = reflectance,
                                absorption = absorption,
-                               num_of_rays = num_of_rays,
-                               relative_power_threshold = relative_power_threshold,
+                               split_ratio = split_ratio,
+                               power_threshold = power_threshold,
                                scatter_model = scatter_model,
                                bsdf=bsdf
                                )
 
 
 class Part:
 
@@ -384,15 +394,15 @@
         return self._lcs
 
     @property
     def rcs(self):
         if self._rcs is None:
 
             if self.cs_data.get('rcs') is None:
-                self._rcs = (WORLD, None)
+                self._rcs = (GLOBAL, None)
 
             else:
                 for part in self._setup:
                     for cs in part.cs:
                         if cs.id == self.cs_data['rcs']:
                             self._rcs = (cs, cs._part)
                             break
@@ -460,14 +470,16 @@
         return self._parameters['materialID']
 
     @property
     def surfaces(self):
         '''
         Returns a list of the part's surfaces as tdo.Surface objects.
         '''
+        if v.DEBUG:
+            print(f'Creating surfaces of part {self.id}')
         if self._surfaces is None:
             self._surfaces = [Surface._new(self, surface) for surface in self.data.get('surfaces', []) if 'name' in surface]
         return self._surfaces
 
     @surfaces.setter
     def surfaces(self, value):
         raise AttributeError("Cannot set surfaces directly.")
@@ -494,15 +506,15 @@
 
         Returns:
             surface (tdo.Surface): The requested Surface object. If the surface is not found, returns None.
         """
         for surface in self:
             if surface.name == name:
                 return surface
-        return None
+        raise KeyError(f"Surface with name {name} not found in the part.")
 
     def change_pose(self,
                     vector: Union[list, tuple],
                     radians: bool = False
                     ):
 
         self.backup_data = copy.deepcopy(self.data)
@@ -720,14 +732,31 @@
         if not self._changes.get('detector_data'):
             self._changes['detector_data'] = {}
 
         self._changes['detector_data']['size'] = {'half_width': size[0], 'half_height': size[1]}
         return None
 
     @property
+    def surfaces(self):
+        '''
+        Returns a list of the part's surfaces as tdo.Surface objects.
+        '''
+        if v.DEBUG:
+            print(f'Getting surfaces for detector {self.id}')
+
+        if self._surfaces is None:
+            self._surfaces = [
+                create_detector_surface(_part = self, _data = surface_data)
+                for surface_data in self.data.get('surfaces', [])
+                if 'name' in surface_data
+                ]
+        return self._surfaces
+
+
+    @property
     def size(self):
         return tuple(self.data['detector_data']['size'].values())
 
     @size.setter
     def size(self, value):
         raise AttributeError("Cannot set size directly. Use change_size() method instead.")
 
@@ -1532,14 +1561,23 @@
     @property
     def shape(self):
         return self._parameters['shape']
 
     def _change_scattering(self, surface_id, scattering):
         return self._setup._change_scattering(surface_id=surface_id, scattering=scattering, part_id = self.id)
 
+def create_detector_surface(_part, _data):
+    if v.DEBUG:
+        print(f"Creating detector surface with data: {_data}")
+
+    if _data['name'] == v.Surfaces.DETECTOR_FRONT:
+        return DetectorSurface._new(_part, _data)
+
+    return Surface._new(_part, _data)
+
 def create_part(_setup, id, type_):
     '''
     Private
     '''
     # part = _setup._get_part(id)
     # _data = part.get(id)
     # if _data.get('detector_data'):
```

### Comparing `threed_optix-5.0.2/src/threed_optix/simulations.py` & `threed_optix-5.0.4/src/threed_optix/simulations.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from typing import Union
 from io import BytesIO
 
 import numpy as np
 import pandas as pd
 
-
 import threed_optix.package_utils.math as mu
 import threed_optix.package_utils.general as gu
 import threed_optix.package_utils.api as au
 import threed_optix.package_utils.vars as v
 import threed_optix.analyses as tdo_analyses
 import threed_optix.parts as tdo_parts
 
@@ -400,15 +399,16 @@
         part = tdo_parts.create_part(_setup=self,
                                      id=part_id,
                                      type_ = type_
                                      )
 
         self.parts.append(part)
 
-        part.change_config(**kwargs)
+        if kwargs != {}:
+            part.change_config(**kwargs)
 
         return part
 
     def _change_cs(self, part_id, lcs_id, rcs_id):
         return self._api._change_cs(setup_id = self.id, part_id = part_id, lcs_id = lcs_id, rcs_id = rcs_id)
 
     def _change_scattering(self, part_id, surface_id, scattering):
```

### Comparing `threed_optix-5.0.2/src/threed_optix/utils.py` & `threed_optix-5.0.4/src/threed_optix/utils.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.2/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.4/src/threed_optix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 5.0.2
+Version: 5.0.4
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.2/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.4/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

