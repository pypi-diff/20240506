# Comparing `tmp/satsync-0.0.4.tar.gz` & `tmp/satsync-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsync-0.0.4.tar", max compression
+gzip compressed data, was "satsync-0.0.5.tar", max compression
```

## Comparing `satsync-0.0.4.tar` & `satsync-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.4/LICENSE
--rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.4/README.md
--rw-r--r--   0        0        0     1987 2024-05-06 09:17:29.374107 satsync-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.4/satsync/__init__.py
--rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.4/satsync/ecc.py
--rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.4/satsync/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.4/satsync/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.4/satsync/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.4/satsync/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.4/satsync/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.4/satsync/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.4/satsync/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.4/satsync/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.4/satsync/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.4/satsync/lightglue/viz2d.py
--rw-r--r--   0        0        0    14350 2024-05-06 09:16:25.363915 satsync-0.0.4/satsync/main.py
--rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.4/satsync/pcc.py
--rw-r--r--   0        0        0    13287 2024-05-06 08:25:49.514397 satsync-0.0.4/satsync/utils.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 satsync-0.0.4/setup.py
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 satsync-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.5/README.md
+-rw-r--r--   0        0        0     1987 2024-05-06 09:33:13.547331 satsync-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.5/satsync/__init__.py
+-rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.5/satsync/ecc.py
+-rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.5/satsync/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.5/satsync/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.5/satsync/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.5/satsync/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.5/satsync/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.5/satsync/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.5/satsync/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.5/satsync/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.5/satsync/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.5/satsync/lightglue/viz2d.py
+-rw-r--r--   0        0        0    14350 2024-05-06 09:16:25.363915 satsync-0.0.5/satsync/main.py
+-rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.5/satsync/pcc.py
+-rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satsync-0.0.5/satsync/utils.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 satsync-0.0.5/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 satsync-0.0.5/PKG-INFO
```

### Comparing `satsync-0.0.4/LICENSE` & `satsync-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/README.md` & `satsync-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/pyproject.toml` & `satsync-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satsync"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python package to align satellite images."
 authors = ["Cesar Aybar <fcesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satsync"
 documentation = "https://csaybar.github.io/satsync/"
 readme = "README.md"
 packages = [
   {include = "satsync"}
```

### Comparing `satsync-0.0.4/satsync/ecc.py` & `satsync-0.0.5/satsync/ecc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lgm.py` & `satsync-0.0.5/satsync/lgm.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/aliked.py` & `satsync-0.0.5/satsync/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/disk.py` & `satsync-0.0.5/satsync/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/dog_hardnet.py` & `satsync-0.0.5/satsync/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/lightglue.py` & `satsync-0.0.5/satsync/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/sift.py` & `satsync-0.0.5/satsync/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/superpoint.py` & `satsync-0.0.5/satsync/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/utils.py` & `satsync-0.0.5/satsync/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/lightglue/viz2d.py` & `satsync-0.0.5/satsync/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/main.py` & `satsync-0.0.5/satsync/main.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/pcc.py` & `satsync-0.0.5/satsync/pcc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.4/satsync/utils.py` & `satsync-0.0.5/satsync/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import rasterio as rio
 import xarray as xr
 
-
 def create_array(
     path: Union[str, pathlib.Path],
     outdata: Union[str, pathlib.Path]
 ) -> xr.DataArray:
     """Create a xarray DataArray from an folder of S2 images.
 
     Args:
@@ -169,18 +168,18 @@
     raw_cube_img = np.transpose(raw_cube_img, (1, 2, 0))
 
     to_display1 = (raw_cube_img * intensity_factor).clip(0, 1)
     to_display2 = (warped_cube_img * intensity_factor).clip(0, 1)
 
     fig, axs = plt.subplots(1, 2, figsize=(10, 5))
     axs[0].imshow(to_display1)
-    axs[0].set_title(f"Original Cube - {dates[index]}")
+    axs[0].set_title(f"Original Cube - {str(dates[index])}")
     axs[0].axis("off")
     axs[1].imshow(to_display2)
-    axs[1].set_title(f"Aligned Cube - {dates[index]}")
+    axs[1].set_title(f"Aligned Cube - {str(dates[index])}")
     axs[1].axis("off")
 
     return fig, axs
 
 
 def plot_animation1(
     warped_cube: np.ndarray,
@@ -212,14 +211,17 @@
     Raises:
         ValueError: The two cubes must have the same shape
         ValueError: The error creating the gif
 
     Returns:
         pathlib.Path: The path to the gif file.
     """
+    # check if the system has ImageMagick installed
+    if os.system("convert -version") != 0:
+        raise ValueError("You need to install ImageMagick to create the gif")
 
     # create folder is not exists
     png_output_folder = pathlib.Path(png_output_folder)
     png_output_folder.mkdir(parents=True, exist_ok=True)
 
     # both images must have the same shape
     if warped_cube.shape != raw_cube.shape:
@@ -344,14 +346,17 @@
         rgb_band (Union[int, list, None], optional): The RGB bands to use.
             Defaults to [3, 2, 1].
         intensity_factor (int, optional): The intensity factor, used to scale
             the pixel values. Defaults to 3.
         gif_delay (int, optional): The delay between the images. Defaults to 20.
         gif_loop (int, optional): The number of loops. Defaults to 0.    
     """
+    # check if the system has ImageMagick installed
+    if os.system("convert -version") != 0:
+        raise ValueError("You need to install ImageMagick to create the gif")
 
     # create folder is not exists
     png_output_folder = pathlib.Path(png_output_folder)
     png_output_folder.mkdir(parents=True, exist_ok=True)
 
     # both images must have the same shape
     if warped_cube.shape != raw_cube.shape:
```

### Comparing `satsync-0.0.4/setup.py` & `satsync-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rasterio>=1.3.10',
  'scikit-image>=0.19.3',
  'torch>=2.2.0',
  'xarray>=2023.7.0']
 
 setup_kwargs = {
     'name': 'satsync',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'A python package to align satellite images.',
     'long_description': '# satsync\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satsync)](https://img.shields.io/github/v/release/csaybar/satsync)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satsync/main.yml?branch=main)](https://github.com/csaybar/satsync/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satsync/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satsync)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satsync)](https://img.shields.io/github/commit-activity/m/csaybar/satsync)\n[![License](https://img.shields.io/github/license/csaybar/satsync)](https://img.shields.io/github/license/csaybar/satsync)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satsync/>\n- **Documentation** <https://csaybar.github.io/satsync/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satsync.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satsync/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satsync/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'fcesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satsync',
```

### Comparing `satsync-0.0.4/PKG-INFO` & `satsync-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsync
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package to align satellite images.
 Home-page: https://github.com/csaybar/satsync
 Author: Cesar Aybar
 Author-email: fcesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

