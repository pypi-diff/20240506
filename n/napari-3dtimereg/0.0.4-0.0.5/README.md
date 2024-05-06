# Comparing `tmp/napari-3dtimereg-0.0.4.tar.gz` & `tmp/napari_3dtimereg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-3dtimereg-0.0.4.tar", last modified: Fri Apr  5 13:43:26 2024, max compression
+gzip compressed data, was "napari_3dtimereg-0.0.5.tar", last modified: Mon May  6 16:32:25 2024, max compression
```

## Comparing `napari-3dtimereg-0.0.4.tar` & `napari_3dtimereg-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1523 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/LICENSE
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       96 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/MANIFEST.in
--rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5726 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/PKG-INFO
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     4332 2024-04-05 13:25:59.000000 napari-3dtimereg-0.0.4/README.md
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1175 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/pyproject.toml
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1470 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/setup.cfg
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       37 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/src/napari_3dtimereg/
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     8152 2024-04-04 15:55:42.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg/Utils.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg/__init__.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)    20585 2024-04-05 13:42:43.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg/movieRegistration.py
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      350 2024-03-10 14:54:02.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-04-05 13:43:26.435606 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/
--rw-r--r--   0 gaelle    (1001) gaelle    (1001)     5726 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/PKG-INFO
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      467 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/SOURCES.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/dependency_links.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       66 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/entry_points.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      107 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/requires.txt
--rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       17 2024-04-05 13:43:26.000000 napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1523 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/LICENSE
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       96 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/MANIFEST.in
+-rw-r--r--   0 gaelle    (1001) gaelle    (1001)     6360 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/PKG-INFO
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     4966 2024-05-06 16:30:38.000000 napari_3dtimereg-0.0.5/README.md
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1175 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/pyproject.toml
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     1470 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/setup.cfg
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       37 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/src/napari_3dtimereg/
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)     8152 2024-04-04 15:55:42.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg/Utils.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg/__init__.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)    21174 2024-05-06 16:30:20.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg/movieRegistration.py
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      350 2024-03-10 14:54:02.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2024-05-06 16:32:25.057670 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/
+-rw-r--r--   0 gaelle    (1001) gaelle    (1001)     6360 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/PKG-INFO
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      467 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)        1 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       66 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/entry_points.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)      107 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/requires.txt
+-rwxrwxrwx   0 gaelle    (1001) gaelle    (1001)       17 2024-05-06 16:32:25.000000 napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/top_level.txt
```

### Comparing `napari-3dtimereg-0.0.4/LICENSE` & `napari_3dtimereg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.4/PKG-INFO` & `napari_3dtimereg-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3dtimereg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Registration of 3D movies applied to all channels
 Home-page: https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/napari-3dtimereg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/napari-3dtimereg#README.md
@@ -40,14 +40,16 @@
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
+For a tutorial on using `elastix` for registration, see [this tutorial](https://m-albert.github.io/elastix_tutorial/intro.html).
+
 
 ----------------------------------
 ## Installation
 
 * You can install the plugin directly in `Napari` by going to `Plugins>Install/Uninstall plugins` and search for `napari-3dtimereg`
 
 * Or you can install `napari-3dtimereg` via [pip]:
@@ -61,25 +63,30 @@
 
 ### Choose movie and reference chanel
 
 First, choose select the movie that you want to register. The plugin will create a folder `aligned` in the folder of your selected movie where the results will be saved.
 
 Choose the color chanel on which to calculate the registration (`reference chanel`). Color chanels are numbered from 0 to nchanels, and you can see their respective number in the layer list on the left panel of Napari. Click on `Update` when the correct chanel is selected to go to the registration calculation step.
 
-### Calculate alignement
+### Calculate temporal alignement
 
-If the `reference frame` parameter is set to `previous`, the registration of each frame will be calculated by comparing it to its previous frame (previously aligned). You can also choose to calculate the alignement of all frames compared to the middle (temporally) frame or all frames compared to the first frame of the movie.
+The registration is calculated iteratively from one frame to another. Thus the first frame is not moved and all the other frames are aligned to it.
+You can tune several parameters in this plugin:
 
 ![parameters screenshot](./imgs/parameters.png "Registration parameters")
 
 The other parameters are parameters to use [itk-elastix](https://elastix.lumc.nl/) to calculate the registration.
 * `show log`: to see the log of Elastix calculation
 * `do rigid`: performs a rigid (affine) transformation step, that allowed to correct for translations/rotations.
 * `do bspline`: performs a b-spline based transformation step, that allowed for local deformations in the image.
 * `show advanced parameters`: to control the parameters used in the rigid and/or bspline transformations. These parameters control the size of the local registrations calculated, the resolutions at which the transformations are calculated, and can thus greatly impact the results.
+* `final order`: is the final order of the B-Splines used for the registration. 
+* `resolution`: is the number of consecutives resolutions at which the registration will be made. First the registration is made at the lowest level of resolution, correcting global deformations/motions, then at each step, the registration is done on higher resolution, allowing to correct for more local deformations.
+* `final spacing`: is the physical spacing of the smallest resolution.
+* `iterations`: are the maximum number of iterations allowed to minimize the distance between the two images for each resolution and type of registration.
 
 If both rigid and bspline transformations, the program first applies the rigid transformation to allow for a global registration of the images. Then it will performs the second step of b-spline transformation that can includes local deformations.
 
 For each frame, after calculating the registration on the reference chanel, the plugin will apply the calculated transformation to all the other color chanels of the initial movie. All results are saved as separated images in the `aligned` folder during the computation.
 
 ### Create the final aligned movie
```

### Comparing `napari-3dtimereg-0.0.4/README.md` & `napari_3dtimereg-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
+For a tutorial on using `elastix` for registration, see [this tutorial](https://m-albert.github.io/elastix_tutorial/intro.html).
+
 
 ----------------------------------
 ## Installation
 
 * You can install the plugin directly in `Napari` by going to `Plugins>Install/Uninstall plugins` and search for `napari-3dtimereg`
 
 * Or you can install `napari-3dtimereg` via [pip]:
@@ -25,25 +27,30 @@
 
 ### Choose movie and reference chanel
 
 First, choose select the movie that you want to register. The plugin will create a folder `aligned` in the folder of your selected movie where the results will be saved.
 
 Choose the color chanel on which to calculate the registration (`reference chanel`). Color chanels are numbered from 0 to nchanels, and you can see their respective number in the layer list on the left panel of Napari. Click on `Update` when the correct chanel is selected to go to the registration calculation step.
 
-### Calculate alignement
+### Calculate temporal alignement
 
-If the `reference frame` parameter is set to `previous`, the registration of each frame will be calculated by comparing it to its previous frame (previously aligned). You can also choose to calculate the alignement of all frames compared to the middle (temporally) frame or all frames compared to the first frame of the movie.
+The registration is calculated iteratively from one frame to another. Thus the first frame is not moved and all the other frames are aligned to it.
+You can tune several parameters in this plugin:
 
 ![parameters screenshot](./imgs/parameters.png "Registration parameters")
 
 The other parameters are parameters to use [itk-elastix](https://elastix.lumc.nl/) to calculate the registration.
 * `show log`: to see the log of Elastix calculation
 * `do rigid`: performs a rigid (affine) transformation step, that allowed to correct for translations/rotations.
 * `do bspline`: performs a b-spline based transformation step, that allowed for local deformations in the image.
 * `show advanced parameters`: to control the parameters used in the rigid and/or bspline transformations. These parameters control the size of the local registrations calculated, the resolutions at which the transformations are calculated, and can thus greatly impact the results.
+* `final order`: is the final order of the B-Splines used for the registration. 
+* `resolution`: is the number of consecutives resolutions at which the registration will be made. First the registration is made at the lowest level of resolution, correcting global deformations/motions, then at each step, the registration is done on higher resolution, allowing to correct for more local deformations.
+* `final spacing`: is the physical spacing of the smallest resolution.
+* `iterations`: are the maximum number of iterations allowed to minimize the distance between the two images for each resolution and type of registration.
 
 If both rigid and bspline transformations, the program first applies the rigid transformation to allow for a global registration of the images. Then it will performs the second step of b-spline transformation that can includes local deformations.
 
 For each frame, after calculating the registration on the reference chanel, the plugin will apply the calculated transformation to all the other color chanels of the initial movie. All results are saved as separated images in the `aligned` folder during the computation.
 
 ### Create the final aligned movie
```

### Comparing `napari-3dtimereg-0.0.4/pyproject.toml` & `napari_3dtimereg-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.4/setup.cfg` & `napari_3dtimereg-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-3dtimereg
-version = 0.0.4
+version = 0.0.5
 description = Registration of 3D movies applied to all channels
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 license = BSD-3-Clause
```

### Comparing `napari-3dtimereg-0.0.4/src/napari_3dtimereg/Utils.py` & `napari_3dtimereg-0.0.5/src/napari_3dtimereg/Utils.py`

 * *Files identical despite different names*

### Comparing `napari-3dtimereg-0.0.4/src/napari_3dtimereg/movieRegistration.py` & `napari_3dtimereg-0.0.5/src/napari_3dtimereg/movieRegistration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import napari
 import tifffile
 from magicgui import magicgui
 from napari.utils.notifications import show_info
 import itk
-import random
+import random, math
 import numpy as np
 import pathlib
-import os, glob
+import os, glob, csv
 import napari_3dtimereg.Utils as ut
 from qtpy.QtWidgets import QFileDialog
 from napari.utils.history import get_save_history, update_save_history
 from webbrowser import open_new_tab
+from skimage.measure import label, regionprops
 
 """
 Napari - 3D Time Reg
 
 Napari plugin to do movie registration with possible deformation. Uses elastix library.
 Registration is calculated on one reference chanel and applied to the others.
 
@@ -32,49 +33,62 @@
         filename = dialog.selectedFiles()
     if filename:
         return filename[0]
     else:
         return None
 
 def start():
-    global viewer, aligndir, imagedir
+    global viewer, aligndir, imagedir, ptsdir
     global refimg, refchanel
     global resimg
     global imagename
     global scaleXY, scaleZ
     global colchan, dim
+    global refpts
+    refpts = None
     refchanel = 0
     viewer = napari.current_viewer()
     viewer.title = "3dTimeReg"
     filename = get_filename()
     if filename is None:
         print("No file selected")
         return
     refimg, scaleXY, scaleZ, names = ut.open_image(filename, verbose=True)
-    print(refimg.shape)
+    global pixel_spacing
+    #pixel_spacing = [scaleXY, scaleXY]
+    pixel_spacing = [1, 1]
+    if (scaleZ is not None) and (scaleZ>0):
+        #pixel_spacing = [scaleZ/scaleXY, scaleZ/scaleXY, 1]
+        #pixel_spacing.append(scaleZ)
+        pixel_spacing.append(scaleZ/scaleXY)
+    print("Image size: "+str(refimg.shape))
+    print("Scale: "+str(pixel_spacing))
+
     ## test if 2d or 3d movie (several chanels assumed)
     if len(refimg.shape)==4:
         colchan = 1
         dim = 2
         scaleZ = -1
     else:
         colchan = 2
         dim = 3
     imagename, imagedir, aligndir = ut.extract_names( filename, subname="aligned" )
+    ptsdir = os.path.join(imagedir, "regpoints")
     update_save_history(imagedir)
     for chan in range(refimg.shape[colchan]):
         cmap = ut.colormapname(chan)
         if dim == 3:
             cview = viewer.add_image( refimg[:,:,chan,:,:], name="Movie_"+"C"+str(chan), blending="additive", colormap = cmap )
             quants = tuple( np.quantile( refimg[:,:,chan,:,:], [0.01, 0.9999]) )
         else:
             cview = viewer.add_image( refimg[:,chan,:,:], name="Movie_"+"C"+str(chan), blending="additive", colormap = cmap )
             quants = tuple( np.quantile( refimg[:,chan,:,:], [0.01, 0.9999]) )
         cview.contrast_limits = quants
         cview.gamma = 0.95
+    
     return getChanels()
 
 def show_help_chanel():
     """ Open the gitlab page with the documentation """
     import webbrowser
     webbrowser.open_new_tab("https://gitlab.pasteur.fr/gletort/napari-3dtimereg/#choose-movie-and-reference-chanel")
     return
@@ -116,253 +130,288 @@
                 resimg = np.copy(refimg[:,refchanel,:,:])
             else:
                 resimg = np.copy(refimg[:,:,refchanel,:,:])
             resimg[0] = resimg[0] - np.min(resimg[0])
             cview = viewer.add_image( resimg, name="ResMovie", blending="additive", colormap = "red") 
             #quants = tuple( np.quantile( resimg, [0.01, 0.9999]) )
             #cview.contrast_limits = quants
-            do_registration()
+            iterative_registration()
     
 
     get_chanel.help.clicked.connect(show_help_chanel)
     wid = viewer.window.add_dock_widget(get_chanel, name="Choose chanel")
     return wid
 
 def itk_to_layer(img, name, color):
     lay = layer_from_image(img)
     lay.blending = "additive"
     lay.colormap = color
     lay.name = name
     viewer.add_layer( lay )
+        
+def img_to_itk(img):
+    """ Convert image array to itk image """
+    image_itk = itk.GetImageFromArray(img)
+    #fimage = itk.image_view_from_array((resimg[0]))
+    image_itk.SetSpacing( tuple( [float(v) for v in pixel_spacing] ) )
+    image_itk = image_itk.astype(itk.F)
+    return image_itk
 
-def do_registration():
-    """ use Elastix to perform registration with possible deformation """
-    
-    def calc_registration( time ):
-        """ Calculate the registration between two consecutive frames """
-        global resimg, dim
-        global results_transform_parameters_aff, results_transform_parameters
-        if get_paras.reference_frame.value == "first frame":
-            if time == 0:
-                save_images(0)
-                return None
-            fimage = itk.image_view_from_array((resimg[0]))
-        if get_paras.reference_frame.value == "middle frame":
-            halftime = int(resimg.shape[0]/2)
-            if time == halftime:
-                save_images(halftime)
-                return None
-            fimage = itk.image_view_from_array((resimg[halftime]))
-        if get_paras.reference_frame.value == "previous":
-            if time == 0:
-                save_images(0)
-                return None
-            fimage = itk.image_view_from_array((resimg[time-1]))
-        fimage = fimage.astype(itk.F)
-        mimage = itk.image_view_from_array((resimg[time]))
-        mimage = mimage.astype(itk.F)
-        affimage = mimage 
-        
-        elastix_object = None
-        results_transform_parameters_aff = None
-
-        if get_paras.do_rigid.value == True:
-            parameter_object = None
-            parameter_object = itk.ParameterObject.New()
-            parameter_map_rigid = parameter_object.GetDefaultParameterMap('rigid')
-            parameter_map_rigid['MaximumNumberOfIterations'] = [str(get_paras.iterations.value)]
-            parameter_map_rigid['MaximumStepLength'] = [str(get_paras.max_step_length.value)]
-            parameter_map_rigid["NumberOfResolutions"] = [str(get_paras.resolution.value)]
-            parameter_map_rigid['NumberOfSpatialSamples'] = ['10000']
-            parameter_map_rigid['MaximumNumberOfSamplingAttempts'] = ['8']
-            parameter_map_rigid['RequiredRatioOfValidSamples'] = ['0.05']
-            parameter_map_rigid['CheckNumberOfSamples'] = ['false']
-            final = int(get_paras.final_spacing.value)
-            parameter_map_rigid['FinalGridSpacingInPhysicalUnits'] = [str(final)]
-            parameter_map_rigid['Registration'] = ['MultiMetricMultiResolutionRegistration']
-            parameter_map_rigid["AutomaticTransformInitialization"] = ['true']
-            parameter_map_rigid["AutomaticTransformInitializationMethod"] = ['CenterOfGravity']
-            space_one = int(get_paras.spacing_one.value)
-            #gridspace = [str(space_one*10)+" "+str(space_one*10)+" "+str(int(space_one*2))]
-            if dim == 3:
-                gridspace = [str(space_one*1)+" "+str(space_one*4)+" "+str(int(space_one*4))]
-            else:
-                gridspace = [str(space_one)]
-            resolution = int(get_paras.resolution.value)
-            if resolution > 1:
-                space_two = int(get_paras.spacing_two.value)
-                #gridspace.append(str(space_two*5)+" "+str(space_two*5)+" "+str(int(space_two)))
-                if dim == 3:
-                    gridspace.append(str(space_two*1)+" "+str(space_two*2)+" "+str(int(space_two*2)))
-                else:
-                    gridspace.append(str(space_two))
-            if resolution > 2:
-                space_three = int(get_paras.spacing_three.value)
-                #gridspace.append(str(space_three*5)+" "+str(space_three*5)+" "+str(space_three))
-                if dim == 3:
-                    gridspace.append(str(space_three*1)+" "+str(space_three*1)+" "+str(space_three))
-                else:
-                    gridspace.append(str(space_three*1))
-            if resolution > 3:
-                space_four = int(get_paras.spacing_four.value)
-                if dim == 3:
-                    gridspace.append(str(space_four*1)+" "+str(space_four*1)+" "+str(space_four))
-                else:
-                    gridspace.append(str(space_four*1))
-            if resolution > 4:
-                gridspace.append(str(int(get_paras.spacing_four.value)))
-            parameter_map_rigid['GridSpacingSchedule'] = gridspace
-            original_metric = parameter_map_rigid['Metric']
-            parameter_object.AddParameterMap(parameter_map_rigid)
-        
-            elastix_object = None
-            elastix_object = itk.ElastixRegistrationMethod.New(fimage, mimage)
-            elastix_object.SetParameterObject(parameter_object)
-            
-            # Set additional options
-            elastix_object.SetLogToConsole(get_paras.show_log.value==True)
+def iterative_registration():
+    """ use Elastix to perform registration with possible deformation, iteratively in time """
+
+    def rigid_map():
+        """ Set-up rigid (affine) transformation parameters """
+        
+        parameter_object = itk.ParameterObject.New()
+        parameter_map_rigid = parameter_object.GetDefaultParameterMap('rigid')
+        parameter_map_rigid['MaximumNumberOfIterations'] = [str(get_paras.iterations.value)]
+        parameter_map_rigid['MaximumStepLength'] = ['2.0']
+        parameter_map_rigid["NumberOfResolutions"] = [str(get_paras.resolution.value)]
+        parameter_map_rigid['NumberOfSpatialSamples'] = ['10000']
+        parameter_map_rigid['MaximumNumberOfSamplingAttempts'] = ['10']
+        parameter_map_rigid['RequiredRatioOfValidSamples'] = ['0.05']
+        parameter_map_rigid['CheckNumberOfSamples'] = ['false']
+        final = int(get_paras.final_spacing.value)
+        parameter_map_rigid['FinalGridSpacingInPhysicalUnits'] = [str(final)]
+        parameter_map_rigid['Registration'] = ['MultiMetricMultiResolutionRegistration']
+        parameter_map_rigid["AutomaticTransformInitialization"] = ['true']
+        parameter_map_rigid["AutomaticTransformInitializationMethod"] = ['CenterOfGravity']
+        
+        original_metric = parameter_map_rigid['Metric']    
+        if get_paras.use_reference_points.value==True:
+            parameter_map_rigid['Metric'] = [original_metric[0], 'CorrespondingPointsEuclideanDistanceMetric']
+        
+        return parameter_map_rigid
+
+        
+    def bspline_map():
+        """ Set-up bspline transformation parameters """
+        preset = "bspline"
+        parameter_object = itk.ParameterObject.New()
+        parameter_map = parameter_object.GetDefaultParameterMap(preset)
+        
+        parameter_map["NumberOfResolutions"] = [str(get_paras.resolution.value)]
+        parameter_map["WriteIterationInfo"] = ["false"]
+        parameter_map['MaximumStepLength'] = ['2.0']
+        parameter_map['NumberOfSpatialSamples'] = ['10000']
+        parameter_map['MaximumNumberOfSamplingAttempts'] = ['10']
+        parameter_map['RequiredRatioOfValidSamples'] = ['0.05']
+        parameter_map['MaximumNumberOfIterations'] = [str(get_paras.iterations.value)]
+        parameter_map['FinalBSplineInterpolationOrder'] = [str(get_paras.final_order.value)]
+        parameter_map['BSplineInterpolationOrder'] = [str(3)]
+        parameter_map['HowToCombineTransform'] = ['Compose']
+        nres = int(get_paras.resolution.value)
+        spaces = []
+        for step in range(nres):
+            spaces.append( math.pow(2, nres-1-step) )
+        parameter_map['GridSpacingSchedule'] = [str(v) for v in spaces ]
+        parameter_map['FinalGridSpacingInPhysicalUnits'] = [str(v) for v in [get_paras.final_spacing.value]*int(get_paras.resolution.value)]
 
-            # Update filter object (required)
-            elastix_object.UpdateLargestPossibleRegion()
+        return parameter_map
 
-            # Results of Registration
-            affimage = elastix_object.GetOutput()
-            results_transform_parameters_aff = elastix_object.GetTransformParameterObject()
+    def time_registration():
+        """ Go for frame by frame registration """
+        
+        ## Build registration parameter maps from GUI parameters
+        registration_parameter_object = itk.ParameterObject.New()
+        nmap = 0
+        if get_paras.do_rigid.value:
+            pmap_rigid = rigid_map()
+            registration_parameter_object.AddParameterMap(pmap_rigid)
+            nmap = nmap + 1
+        if get_paras.do_bspline.value:
+            pmap_spline = bspline_map()
+            registration_parameter_object.AddParameterMap(pmap_spline)
+            nmap = nmap + 1
             
-            # Show intermediate layer
-            if get_paras.show_intermediate_layer.value==True:
-                resimage = affimage
-                resclayer = layer_from_image(resimage)
-                resclayer.blending = "additive"
-                resclayer.name = "AfterAffineRegistration"
-                viewer.add_layer( resclayer )
-        
-        # first rigid transformation
-        if get_paras.do_bspline.value == True:
-            parameter_object = None
-            preset = "bspline"
-            parameter_object = itk.ParameterObject.New()
-            parameter_map = parameter_object.GetDefaultParameterMap(preset)
-            parameter_map["NumberOfResolutions"] = [str(get_paras.resolution.value)]
-            parameter_map["WriteIterationInfo"] = ["false"]
-            parameter_map['MaximumStepLength'] = [str(get_paras.max_step_length.value)]
-            parameter_map['NumberOfSpatialSamples'] = ['10000']
-            parameter_map['MaximumNumberOfSamplingAttempts'] = ['10']
-            parameter_map['RequiredRatioOfValidSamples'] = ['0.05']
-            parameter_map['MaximumNumberOfIterations'] = [str(get_paras.iterations.value)]
-            parameter_map['FinalGridSpacingInPhysicalUnits'] = [str(get_paras.final_spacing.value)]
-            #final = int(get_paras.final_spacing.value)
-            #parameter_map['FinalGridSpacingInPhysicalUnits'] = [str(final)+" "+str(final)+" "+str(int(final/5))]
-            parameter_map['FinalBSplineInterpolationOrder'] = [str(3)]
-            parameter_map['BSplineInterpolationOrder'] = [str(3)]
-            parameter_map['HowToCombineTransform'] = ['Compose']
-            gridspace = [str(get_paras.spacing_one.value)]
-            space_one = int(get_paras.spacing_one.value)
-            #gridspace = [str(space_one*5)+" "+str(space_one*5)+" "+str(int(space_one))]
-            resolution = int(get_paras.resolution.value)
-            if resolution > 1:
-                gridspace.append(str(get_paras.spacing_two.value))
-                space_two = int(get_paras.spacing_two.value)
-                #gridspace.append(str(space_two*5)+" "+str(space_two*5)+" "+str(int(space_two)))
-            if resolution > 2:
-                gridspace.append(str(get_paras.spacing_three.value))
-                space_three = int(get_paras.spacing_three.value)
-                #gridspace.append(str(space_three*5)+" "+str(space_three*5)+" "+str(space_three))
-            if resolution > 3:
-                gridspace.append(str(get_paras.spacing_four.value))
-                space_four = int(get_paras.spacing_four.value)
-                #gridspace.append(str(space_four*5)+" "+str(space_four*5)+" "+str(space_four))
-            if resolution > 4:
-                gridspace.append(str(int(get_paras.spacing_four.value/2)))
-            parameter_map['GridSpacingSchedule'] = gridspace
-            parameter_object.AddParameterMap(parameter_map)
-    
-            # Load Elastix Image Filter Object
-            elastix_object = itk.ElastixRegistrationMethod.New(fimage, affimage)
-            elastix_object.SetParameterObject(parameter_object)
-            elastix_object.SetLogToConsole(get_paras.show_log.value==True)
-
-            # Update filter object (required)
-            elastix_object.UpdateLargestPossibleRegion()
-
-        # Results of Registration
-        result_image = elastix_object.GetOutput()
-        results_transform_parameters = elastix_object.GetTransformParameterObject()
-
-        data = (itk.array_view_from_image(result_image))
-        data[data<0] = 0
-        data = np.array(data)
-        #data = data - np.min(data)
-        resimg[time] = data
-        viewer.layers["ResMovie"].refresh()
+        ## apply "alignement" to first frame
+        apply_registration(0, None)
 
-        ut.writeTif( data, os.path.join(aligndir, imagename+"_C"+str(refchanel)+"_T"+"{:04d}".format(time)+".tif"), scaleXY, scaleZ, "uint16" )
-        return 1
+        # initialise a parameter object to which the transforms will be appended that result from the pairwise slice registrations
+        curr_transform_object = itk.ParameterObject.New()
+
+        # the first fixed image will be the reference slice
+        fixed_image_itk = img_to_itk(resimg[0])
+
+        ## Register all frames to previous one and add it
+        for t in range(resimg.shape[0]):
+            print("Calculate registration for time point "+str(t))
+
+            if t > 0:
+                # the moving image is the current slice
+                moving_image_itk = img_to_itk(resimg[t])
+
+                # perform the pairwise registration between two slices
+                elastix_object = itk.ElastixRegistrationMethod.New(fixed_image_itk, moving_image_itk)
+                elastix_object.SetParameterObject(registration_parameter_object)
+            
+                if get_paras.use_reference_points.value:
+                    elastix_object.SetFixedPointSetFileName(os.path.join(aligndir, imagename+"_refpts_fixed.txt"))
+                    elastix_object.SetMovingPointSetFileName(os.path.join(aligndir, imagename+"_refpts_moving.txt"))
             
+                elastix_object.SetLogToConsole(get_paras.show_log.value==True)
+
+                # Update filter object (required)
+                elastix_object.UpdateLargestPossibleRegion()
+
+                # Results of Registration
+                #affimage = elastix_object.GetOutput()
+                results_transform_parameters = elastix_object.GetTransformParameterObject()
+
+                # set the current moving image as the fixed image for the registration in the next iteration
+                fixed_image_itk = moving_image_itk
 
+                # append the obtained transform to the transform parameter object
+                for i in range(nmap):
+                    curr_transform_object.AddParameterMap(results_transform_parameters.GetParameterMap(i))
+
+                # transform the current slice and append it to the reconstructed stack
+                apply_registration(t, curr_transform_object)
+
+    
     @magicgui(call_button="Go", 
-            reference_frame={"choices":["previous","first frame", "middle frame"]},
-            max_step_length={"widget_type":"LiteralEvalLineEdit"}, 
             resolution={"widget_type":"LiteralEvalLineEdit"}, 
             iterations={"widget_type":"LiteralEvalLineEdit"}, 
             final_spacing={"widget_type":"LiteralEvalLineEdit"}, 
-            spacing_one={"widget_type":"LiteralEvalLineEdit"}, 
-            spacing_two={"widget_type":"LiteralEvalLineEdit"}, 
-            spacing_three={"widget_type":"LiteralEvalLineEdit"}, 
-            spacing_four={"widget_type":"LiteralEvalLineEdit"}, 
+            final_order={"widget_type":"LiteralEvalLineEdit"}, 
             help={"widget_type":"PushButton", "value": False, "name": "help"}, 
             )
-    def get_paras( reference_frame = "previous",
-            show_log = False,
-            do_rigid = False,
+    def get_paras( 
+            show_log = True,
+            #use_reference_points = False,
+            #refpoints_file = pathlib.Path(os.path.join(imagedir, imagename+"_reference_points.csv")),
+            do_rigid = True,
             do_bspline = True,
             show_advanced_parameters = False,
-            show_intermediate_layer = False,
-            resolution=2,
-            max_step_length = 2,
+            resolution=4,
             iterations=1000,
-            final_spacing=25, 
-            spacing_one=4,
-            spacing_two=2,
-            spacing_three=1,
-            spacing_four=1,
+            final_spacing=30, 
+            final_order = 1,
             help = False,
             ):
         
-        global results_transform_parameters_aff, results_transform_parameters
+        global move_points
         reslay = viewer.layers["ResMovie"]
-        results_transform_para_aff = None
+        use_reference_points = False
+        if use_reference_points:
+            read_points()
+            move_points = True
         
-        for t in range(reslay.data.shape[0]):
-            time = t 
-            print("Calculate registration for time point "+str(time))
-            done = calc_registration(time)
-            if done is not None:
-                apply_alignement(time)
-
+        time_registration()
         finish_image()
-
-
     
     def show_advanced(booly):
-        get_paras.show_intermediate_layer.visible = booly
         get_paras.resolution.visible = booly
-        get_paras.max_step_length.visible = booly
         get_paras.iterations.visible = booly
         get_paras.final_spacing.visible = booly
-        get_paras.spacing_one.visible = booly
-        get_paras.spacing_two.visible = booly
-        get_paras.spacing_three.visible = booly
-        get_paras.spacing_four.visible = booly
+
+    def show_spline():
+        get_paras.final_order.visible = get_paras.do_bspline.value
 
     show_advanced(False)
+    show_spline()
     get_paras.show_advanced_parameters.changed.connect(show_advanced)
+    get_paras.do_bspline.changed.connect(show_spline)
     get_paras.help.clicked.connect(show_help_align)
     wid = viewer.window.add_dock_widget(get_paras, name="Calculate alignement")
-    return wid
+
+    
+def get_ref_points(time0, time1):
+        """ Get the reference points common between time0 and time1 and put them to file """
+        global refpts
+        pttime0 = refpts[refpts[:,4]==time0,]
+        pttime1 = refpts[refpts[:,4]==time1,]
+        inter, ind1, ind0 = np.intersect1d(pttime1[:,0], pttime0[:,0], return_indices=True)
+        write_ref_file(ind1, pttime1, "moving")
+        write_ref_file(ind0, pttime0, "fixed")
+
+def get_closest_label(pts, tid):
+    """ Find closest pt id to tid """
+    closest = pts[0]
+    dist = 1000
+    for pt in pts:
+        d = abs(pt[0]-tid)
+        if d < dist:
+            dist = d
+            closest = pt
+    return closest
+    
+def update_points(mask, time):
+    """ Update the points coordinates at time from the mask """
+    global refpts
+    pttime = refpts[refpts[:,4]==time,]
+    masknp = itk.array_from_image(mask)
+    masknp[masknp<0] = 0
+    masknp = np.array(masknp)
+        #res = res - np.min(res)
+    #masknp = masknp
+    masknp = np.ceil(masknp)
+    print(np.unique(masknp))
+    masknp = np.uint16(masknp)
+    print(np.unique(masknp))
+    lab = label(masknp)
+    props = regionprops(lab, masknp)
+    if len(props) != len(pttime):
+        print(len(props))
+        print(len(pttime))
+        print("Point missing ?????")
+        print(pttime)
+        print(props)
+    print(pttime)
+    for prop in props:
+        cent = prop.centroid
+        tid = prop.intensity_max-20
+        pt = get_closest_label(pttime, tid)
+        print(tid)
+        print(pt)
+        #print(cent)
+        pt[1] = cent[1]
+        pt[2] = cent[2]
+        pt[3] = cent[0]
+        #print(pt)
+
+def points_to_mask(time):
+        """ Get the reference points and put them to image """
+        global refpts
+        pttime = refpts[refpts[:,4]==time,]
+        if dim == 2:
+            imshape = refimg.shape[2:4]
+        else:
+            imshape = (refimg.shape[1],)+refimg.shape[3:5]
+            print(imshape)
+        img = np.zeros( imshape, np.uint8)
+        for pt in pttime:
+            img[ pt[3], pt[2], pt[1] ] = (pt[0]+20)  ## put the label value
+            print(pt)
+        return img
+
+def write_ref_file(inds, pts, fixed):
+    """ Write points of inds in file for time """
+    filepath = os.path.join(aligndir, imagename+"_refpts_"+fixed+".txt")
+    f = open(filepath, "w")
+    f.write("index\n")
+    f.write(str(len(inds))+"\n")
+    for ind in inds:
+        pt = pts[ind,]
+        y = pt[2]
+        #if imsize is not None:
+        #    y = imsize - pt[1]
+        f.write(str(int(pt[1]))+" "+str(int(y))+" "+str(int(pt[3]))+"\n")
+        #f.write(str(y)+" "+str(pt[1])+"\n")
+    f.close()
+    
+def save_points():
+    """ Save updated points coordinates """
+    global refpts
+    outfile = os.path.join(aligndir, imagename+"_refpts_moved.csv")
+    with open(outfile, "w") as infile:
+        csvwriter = csv.writer(infile)
+        csvwriter.writerow(["TrackID", "X", "Y", "Z", "T"])
+        csvwriter.writerows( refpts.tolist())
 
 def layer_from_image(img):
     data = np.array(itk.array_view_from_image(img))
     image_layer = napari.layers.Image(data)
     return image_layer
 
 def save_images(time):
@@ -380,64 +429,73 @@
             ut.writeTif( res, os.path.join(aligndir, imagename+"_C"+str(chan)+"_T"+"{:04d}".format(time)+".tif"), scaleXY, scaleZ, "uint16" )
         else:
             res = np.copy(refimg[time,chan,:,:])
             #res = res - np.min(res)
             res = np.uint16(res)
             ut.writeTif( res, os.path.join(aligndir, imagename+"_C"+str(chan)+"_T"+"{:04d}".format(time)+".tif"), scaleXY, -1, "uint16" )
 
-def apply_alignement(time):
+def apply_registration(time, results_transform):
     """ Apply caclulated registration to the other chanels """
     global dim
-    global results_transform_parameters_aff, results_transform_parameters
+    global move_points
     if dim == 2:
-        chanellist = list(range(refimg.shape[1]))
+        align_chanels = list(range(refimg.shape[1]))
     else:
-        chanellist = list(range(refimg.shape[2]))
-    align_chanels = []
-    for chan in chanellist:
-        if chan != refchanel:
-            align_chanels.append(chan)
+        align_chanels = list(range(refimg.shape[2]))
 
     print("Apply alignment to "+str(align_chanels))
+    pt_image = None
+    moved_pts = False
+
     for chan in align_chanels:
         if dim == 2:
             img = refimg[time,chan,:,:]
         else:
             img = refimg[time,:,chan,:,:]
         res = []
-        itkimage = itk.image_view_from_array(img)
-        itkimage = itkimage.astype(itk.F)
+        itkimage = img_to_itk(img)
         ImageType = itk.Image[itk.F, dim]
-        if results_transform_parameters_aff is not None:
-            transformix_filter = itk.TransformixFilter[ImageType].New()
-            transformix_filter.SetMovingImage(itkimage)
-            transformix_filter.SetTransformParameterObject(results_transform_parameters_aff)
-            aff_image = transformix_filter.GetOutput()
-        else:
-            aff_image = itkimage
         
-        if results_transform_parameters is not None:
+        if results_transform is not None:
             transformix = itk.TransformixFilter[ImageType].New()
-            transformix.SetMovingImage(aff_image)
-            transformix.SetTransformParameterObject(results_transform_parameters)
+            transformix.SetMovingImage(itkimage)
+            transformix.SetTransformParameterObject(results_transform)
             res_image = transformix.GetOutput()
+            #if (not moved_pts) and move_points:
+            #    if pt_image is None:
+            #        ptimg = points_to_mask(time)
+            #        pt_image = itk.image_view_from_array(ptimg)
+            #        pt_image = pt_image.astype(itk.F)
+                #transformix.SetMovingImage(itkimage)
+                #transformix.SetTransformParameterObject(results_transform_parameters)
+                #pt_image = transformix.GetOutput()
+                #resclayerm = layer_from_image(pt_image)
+                #resclayerm.blending = "additive"
+                #resclayerm.name = "MovingPointsAfter"
+                #viewer.add_layer( resclayerm )
+            #res = itk.array_from_image(res_image)
+            res = np.array(res_image)
         else:
-            res_image = aff_image
+            res = img
 
-        res = itk.array_from_image(res_image)
         res[res<0] = 0
         res = np.array(res)
         #res = res - np.min(res)
         res = np.uint16(res)
+
+        #if pt_image is not None:
+        #    update_points(pt_image, time)
         
         ut.writeTif( res, os.path.join(aligndir, imagename+"_C"+str(chan)+"_T"+"{:04d}".format(time)+".tif"), scaleXY, scaleZ, "uint16" )
 
 def finish_image():
     """ End, create composite image """
-    global movimg
+    global movimg, refpts
+    if refpts is not None:
+        save_points()
     remove_widget("Calculate alignement")
     remove_layer("ResMovie")
     create_result_image()
 
 def remove_layer(layname):
     if layname in viewer.layers:
         viewer.layers.remove(layname)
@@ -460,23 +518,29 @@
         else:
             nchans = refimg.shape[2]
 
         for chan in range(nchans):
             for time in range(refimg.shape[0]):
                 filename = os.path.join(aligndir, imagename+"_C"+str(chan)+"_T"+"{:04d}".format(time)+".tif")
                 img, tscaleXY, tscaleZ, names = ut.open_image(filename, verbose=False)
-                resimg[time, chan, :,:] = img
+                if dim == 2:
+                    resimg[time, chan, :,:] = img
+                else:
+                    resimg[time, :, chan, :,:] = img
                 os.remove(filename)
 
         viewer.add_image(resimg, name="Res", blending="additive")
         for lay in viewer.layers:
             if lay.name != "Res":
                 remove_layer(lay)
         imgname = os.path.join(aligndir, imagename+".tif")
         resimg = np.array(resimg, "uint16")
         # move the chanel axis after the Z axis (imageJ format)
         if dim == 3:
             resimg = np.moveaxis(resimg, 0, 1)
-        tifffile.imwrite(imgname, resimg, imagej=True, resolution=[1./scaleXY, 1./scaleXY], metadata={'PhysicalSizeX': scaleXY, 'spacing': scaleZ, 'unit': 'um', 'axes': 'ZCYX'})
+            print(resimg.shape)
+            tifffile.imwrite(imgname, resimg, imagej=True, resolution=[1./scaleXY, 1./scaleXY], metadata={'PhysicalSizeX': scaleXY, 'spacing': scaleZ, 'unit': 'um', 'axes': 'TZCYX'})
+        else:
+            tifffile.imwrite(imgname, resimg, imagej=True, resolution=[1./scaleXY, 1./scaleXY], metadata={'PhysicalSizeX': scaleXY, 'unit': 'um', 'axes': 'TCYX'})
         show_info("Image "+imgname+" saved")
     
     viewer.window.add_dock_widget(get_files, name="Concatenate")
```

### Comparing `napari-3dtimereg-0.0.4/src/napari_3dtimereg.egg-info/PKG-INFO` & `napari_3dtimereg-0.0.5/src/napari_3dtimereg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-3dtimereg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Registration of 3D movies applied to all channels
 Home-page: https://gitlab.pasteur.fr/gletort/napari-3dtimereg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/napari-3dtimereg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/napari-3dtimereg#README.md
@@ -40,14 +40,16 @@
 [![PyPI](https://img.shields.io/pypi/v/napari-3dtimereg.svg?color=green)](https://pypi.org/project/napari-3dtimereg)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-3dtimereg.svg?color=green)](https://python.org)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-3dtimereg)](https://napari-hub.org/plugins/napari-3dtimereg)
 
 Temporal registration of 2D/3D movies on one channel based on [itk-elastix](https://pypi.org/project/itk-elastix/), and transpose alignement to the other channels.
 
 Adaptated from [multireg](https://gitlab.pasteur.fr/gletort/multireg) for temporal movies.
+For a tutorial on using `elastix` for registration, see [this tutorial](https://m-albert.github.io/elastix_tutorial/intro.html).
+
 
 ----------------------------------
 ## Installation
 
 * You can install the plugin directly in `Napari` by going to `Plugins>Install/Uninstall plugins` and search for `napari-3dtimereg`
 
 * Or you can install `napari-3dtimereg` via [pip]:
@@ -61,25 +63,30 @@
 
 ### Choose movie and reference chanel
 
 First, choose select the movie that you want to register. The plugin will create a folder `aligned` in the folder of your selected movie where the results will be saved.
 
 Choose the color chanel on which to calculate the registration (`reference chanel`). Color chanels are numbered from 0 to nchanels, and you can see their respective number in the layer list on the left panel of Napari. Click on `Update` when the correct chanel is selected to go to the registration calculation step.
 
-### Calculate alignement
+### Calculate temporal alignement
 
-If the `reference frame` parameter is set to `previous`, the registration of each frame will be calculated by comparing it to its previous frame (previously aligned). You can also choose to calculate the alignement of all frames compared to the middle (temporally) frame or all frames compared to the first frame of the movie.
+The registration is calculated iteratively from one frame to another. Thus the first frame is not moved and all the other frames are aligned to it.
+You can tune several parameters in this plugin:
 
 ![parameters screenshot](./imgs/parameters.png "Registration parameters")
 
 The other parameters are parameters to use [itk-elastix](https://elastix.lumc.nl/) to calculate the registration.
 * `show log`: to see the log of Elastix calculation
 * `do rigid`: performs a rigid (affine) transformation step, that allowed to correct for translations/rotations.
 * `do bspline`: performs a b-spline based transformation step, that allowed for local deformations in the image.
 * `show advanced parameters`: to control the parameters used in the rigid and/or bspline transformations. These parameters control the size of the local registrations calculated, the resolutions at which the transformations are calculated, and can thus greatly impact the results.
+* `final order`: is the final order of the B-Splines used for the registration. 
+* `resolution`: is the number of consecutives resolutions at which the registration will be made. First the registration is made at the lowest level of resolution, correcting global deformations/motions, then at each step, the registration is done on higher resolution, allowing to correct for more local deformations.
+* `final spacing`: is the physical spacing of the smallest resolution.
+* `iterations`: are the maximum number of iterations allowed to minimize the distance between the two images for each resolution and type of registration.
 
 If both rigid and bspline transformations, the program first applies the rigid transformation to allow for a global registration of the images. Then it will performs the second step of b-spline transformation that can includes local deformations.
 
 For each frame, after calculating the registration on the reference chanel, the plugin will apply the calculated transformation to all the other color chanels of the initial movie. All results are saved as separated images in the `aligned` folder during the computation.
 
 ### Create the final aligned movie
```

