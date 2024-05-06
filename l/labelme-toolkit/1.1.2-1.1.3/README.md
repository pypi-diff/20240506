# Comparing `tmp/labelme_toolkit-1.1.2.tar.gz` & `tmp/labelme_toolkit-1.1.3.tar.gz`

## Comparing `labelme_toolkit-1.1.2.tar` & `labelme_toolkit-1.1.3.tar`

### file list

```diff
@@ -1,45 +1,43 @@
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/Makefile
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/__main__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_formats.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_json.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_labelme.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_migrations.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_paths.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_testing.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_browsers/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_browsers/_images.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_browsers/css/modern-normalize.min.css
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/__init__.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_extract_image.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_extract_image_test.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_install_toolkit_pro.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_mask.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_mask_test.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_visualization.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_visualization_test.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_list_labels.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_cli/_list_labels_test.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/.gitignore
--rw-r--r--   0        0        0   891941 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/dogs.json
--rw-r--r--   0        0        0   396616 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.zip
--rwxr-xr-x   0        0        0   147408 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.jpg
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.json
--rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.jpg
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.json
--rwxr-xr-x   0        0        0   136977 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000025.jpg
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000025.json
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.jpg
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.json
--rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.jpg
--rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.json
--rwxr-xr-x   0        0        0   147408 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000003.jpg
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000003.json
--rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000006.jpg
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000006.json
--rwxr-xr-x   0        0        0   136977 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000025.jpg
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.export/2011_000025.json
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/Makefile
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/.readme/dogs_json_to_mask.jpg
+-rw-r--r--   0        0        0   161718 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/.readme/icon.png
+-rw-r--r--   0        0        0   108316 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/.readme/toolkit_guide.jpg
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/__main__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_formats.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_json.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_labelme.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_migrations.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_paths.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_testing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_browsers/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_browsers/_images.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_browsers/css/modern-normalize.min.css
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/__init__.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_extract_image.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_extract_image_test.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_install_toolkit_pro.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_mask.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_mask_test.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_visualization.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_visualization_test.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_list_labels.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_cli/_list_labels_test.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/.gitignore
+-rw-r--r--   0        0        0  2094047 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/dogs.json
+-rw-r--r--   0        0        0  2083338 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/dogs_rectangle.json
+-rw-r--r--   0        0        0   396616 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset.zip
+-rwxr-xr-x   0        0        0   147408 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.jpg
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.json
+-rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.jpg
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.json
+-rwxr-xr-x   0        0        0   136977 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000025.jpg
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000025.json
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.jpg
+-rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.json
+-rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.jpg
+-rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.json
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.3/PKG-INFO
```

### Comparing `labelme_toolkit-1.1.2/Makefile` & `labelme_toolkit-1.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/.github/workflows/ci.yml` & `labelme_toolkit-1.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_labelme.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_labelme.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,67 @@
 import dataclasses
+from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import PIL.Image
 import PIL.ImageDraw
 
+from . import _json
+
 
 @dataclasses.dataclass
 class Shape:
     type: str
     points: np.ndarray
     label: str
+    mask: Optional[np.ndarray] = None
 
     def __post_init__(self):
         self.points = np.asarray(self.points)
 
-        if self.type not in ["circle", "rectangle", "polygon"]:
+        if self.type not in ["circle", "rectangle", "polygon", "mask"]:
             raise ValueError(f"Unsupported shape type={self.type!r}")
-        if self.points.ndim == 2 and self.points.shape[1] != 2:
+        if not (self.points.ndim == 2 and self.points.shape[1] == 2):
             raise ValueError(f"Invalid shape points.shape={self.points.shape!r}")
         if self.type in ["circle", "rectangle"] and self.points.shape != (2, 2):
             raise ValueError(
                 f"Invalid shape points.shape={self.points.shape!r} for "
                 f"type={self.type!r}"
             )
+        if self.type == "mask":
+            if self.mask is None:
+                raise ValueError(f"shape.type={self.type!r} requires mask")
+            if self.mask.ndim != 2:
+                raise ValueError(f"expected mask.ndim=2, but got {self.mask.ndim}")
+            if self.mask.dtype != bool:
+                raise ValueError(f"expected mask.dtype=bool, but got {self.mask.dtype}")
+            if self.points.size != 4:
+                raise ValueError(
+                    f"expected shape.points.size=4, but got {self.points.size}"
+                )
+
+            mask_height, mask_width = self.mask.shape
+            (xmin, ymin), (xmax, ymax) = self.points
+            if xmax - xmin + 1 != mask_width or ymax - ymin + 1 != mask_height:
+                raise ValueError(
+                    f"shape.points={self.points!r} does not match "
+                    f"mask.shape={self.mask.shape!r}"
+                )
+
+    def to_json(self):
+        return {
+            "label": self.label,
+            "points": self.points.tolist(),
+            "shape_type": self.type,
+            "mask": None
+            if self.mask is None
+            else _json.image_ndarray_to_b64data(ndarray=self.mask),
+        }
 
 
 def shape_to_mask(shape: Shape, image_height: int, image_width: int) -> np.ndarray:
     mask: np.ndarray = np.zeros((image_height, image_width), dtype=np.uint8)
 
     mask_pil: PIL.Image.Image = PIL.Image.fromarray(mask)
     draw_shape_(image=mask_pil, shape=shape, fill_color=1, line_color=1)
```

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_paths.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_paths.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_browsers/_images.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_browsers/_images.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_browsers/css/modern-normalize.min.css` & `labelme_toolkit-1.1.3/labelme_toolkit/_browsers/css/modern-normalize.min.css`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/__init__.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_extract_image.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_extract_image.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_extract_image_test.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_extract_image_test.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_install_toolkit_pro.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_install_toolkit_pro.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os.path as osp
 import subprocess
 import urllib.request
 
 import click
 from loguru import logger
 
 
@@ -39,15 +38,15 @@
 
     """
     logger.info("Installing the Labelme Toolkit Pro...")
     logger.info(f"Access key: {access_key}")
 
     url_path = f"https://labelmeai.github.io/toolkit-pro/{access_key}"
 
-    with urllib.request.urlopen(osp.join(url_path, "versions")) as response:
+    with urllib.request.urlopen(f"{url_path}/versions") as response:
         data = response.read()
         versions = [version.strip() for version in data.decode("utf-8").splitlines()]
 
     if list_versions:
         for version in versions:
             click.echo(version)
         return
@@ -66,15 +65,15 @@
             click.echo("Installation is canceled.")
             return
 
     cmd = [
         "pip",
         "install",
         "-I",
-        osp.join(url_path, f"labelme_toolkit_pro-{version}-py3-none-any.whl"),
+        f"{url_path}/labelme_toolkit_pro-{version}-py3-none-any.whl",
     ]
     logger.info(f"Running command: {' '.join(cmd)}")
     try:
         subprocess.check_call(cmd)
     except subprocess.CalledProcessError:
         logger.error("Failed to install. Is the access key correct?")
         return
```

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_mask.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_mask.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_mask_test.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_mask_test.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_visualization.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_visualization.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_json_to_visualization_test.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_json_to_visualization_test.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_cli/_list_labels.py` & `labelme_toolkit-1.1.3/labelme_toolkit/_cli/_list_labels.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset.zip` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset.zip`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.jpg` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.json` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.jpg` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.json` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000025.jpg` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000025.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000025.json` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000025.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.jpg` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.json` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000003.export/2011_000003.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.jpg` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.json` & `labelme_toolkit-1.1.3/labelme_toolkit/_data/small_dataset/2011_000006.export/2011_000006.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.2/pyproject.toml` & `labelme_toolkit-1.1.3/pyproject.toml`

 * *Files identical despite different names*

