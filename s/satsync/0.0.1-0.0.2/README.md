# Comparing `tmp/satsync-0.0.1.tar.gz` & `tmp/satsync-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsync-0.0.1.tar", max compression
+gzip compressed data, was "satsync-0.0.2.tar", max compression
```

## Comparing `satsync-0.0.1.tar` & `satsync-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.1/LICENSE
--rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.1/README.md
--rw-r--r--   0        0        0     1944 2024-05-05 19:10:26.490908 satsync-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-05 19:08:04.718906 satsync-0.0.1/satsync/__init__.py
--rw-r--r--   0        0        0     1903 2024-05-05 19:08:04.714907 satsync-0.0.1/satsync/ecc.py
--rw-r--r--   0        0        0     6768 2024-05-05 19:08:04.714907 satsync-0.0.1/satsync/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.1/satsync/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.1/satsync/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.1/satsync/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.1/satsync/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.1/satsync/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.1/satsync/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.1/satsync/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.1/satsync/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.1/satsync/lightglue/viz2d.py
--rw-r--r--   0        0        0     9951 2024-05-05 19:07:59.611050 satsync-0.0.1/satsync/main.py
--rw-r--r--   0        0        0     2642 2024-05-05 19:08:04.710907 satsync-0.0.1/satsync/pcc.py
--rw-r--r--   0        0        0    10516 2024-05-05 19:08:04.714907 satsync-0.0.1/satsync/utils.py
--rw-r--r--   0        0        0     3374 1970-01-01 00:00:00.000000 satsync-0.0.1/setup.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 satsync-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.2/README.md
+-rw-r--r--   0        0        0     1962 2024-05-06 08:26:23.189437 satsync-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.2/satsync/__init__.py
+-rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.2/satsync/ecc.py
+-rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.2/satsync/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.2/satsync/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.2/satsync/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.2/satsync/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.2/satsync/lightglue/viz2d.py
+-rw-r--r--   0        0        0    14302 2024-05-06 08:18:46.478456 satsync-0.0.2/satsync/main.py
+-rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.2/satsync/pcc.py
+-rw-r--r--   0        0        0    13287 2024-05-06 08:25:49.514397 satsync-0.0.2/satsync/utils.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 satsync-0.0.2/setup.py
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 satsync-0.0.2/PKG-INFO
```

### Comparing `satsync-0.0.1/LICENSE` & `satsync-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/README.md` & `satsync-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/pyproject.toml` & `satsync-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satsync"
-version = "0.0.1"
+version = "0.0.2"
 description = "A python package to align satellite images."
 authors = ["Cesar Aybar <fcesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satsync"
 documentation = "https://csaybar.github.io/satsync/"
 readme = "README.md"
 packages = [
   {include = "satsync"}
@@ -14,14 +14,15 @@
 python = ">=3.10,<4.0"
 numpy = "^1.26.4"
 xarray = "^2024.3.0"
 rasterio = "^1.3.10"
 scikit-image = "^0.23.2"
 opencv-python = "^4.9.0.80"
 pandas = "^2.2.2"
+kornia = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `satsync-0.0.1/satsync/lgm.py` & `satsync-0.0.2/satsync/lgm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,45 @@
-"""
-This module implements the eo-learn co-registration (Enhanced Cross 
-Correlation). The code has been adapted from the `eo-learn` library.
-The original code can be found at: 
-
-https://github.com/sentinel-hub/eo-learn/blob/master/eolearn/coregistration/coregistration.py 
-
-This source code is licensed under the MIT license.
-"""
-
 import warnings
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import torch
-from opensr_test.lightglue import (ALIKED, DISK, SIFT, DoGHardNet, LightGlue,
-                                   SuperPoint)
-from opensr_test.lightglue.utils import rbd
-
-from satsync.main import SuperAlignmentAbstract
 
+from satsync.lightglue import (ALIKED, DISK, SIFT, DoGHardNet, LightGlue,
+                               SuperPoint)
+from satsync.lightglue.utils import rbd
+from satsync.main import SatSync
 
-class LGM(SuperAlignmentAbstract):
-    """
-    Multi-temporal image co-registration using Phase Cross-Correlation
-    """
 
+class LGM(SatSync):
     def __init__(
         self,
         datacube: np.ndarray,
         reference: np.ndarray,
         feature_model: str = "superpoint",
         matcher_model: str = "lightglue",
         max_num_keypoints: int = 2048,
         device: str = "cpu",
         **kwargs,
     ):
-        """Constructor for the LGM class
+        """
 
         Args:
-            datacube (np.ndarray): The data cube to be aligned.
-            reference (np.ndarray): The reference feature.
-            feature_model (str, optional): The feature extractor.
-                Defaults to 'superpoint'. Options are: 'superpoint',
+            datacube (xr.DataArray): The data cube to be aligned. The data cube
+                needs to have the following dimensions: (time, bands, height, width).
+            reference (Optional[xr.DataArray], optional): The reference image.
+                The reference image needs to have the following dimensions:
+                (bands, height, width).
+            feature_model (str, optional): The feature extractor model. Defaults to
+                'superpoint'. Options are: 'superpoint'. Options are: 'superpoint',
                 'disk', 'sift', 'aliked', 'doghardnet'.
-            matcher_model (str, optional): The matcher. Defaults to
-                'lightglue'.
-            max_num_keypoints (int, optional): The maximum number of
-                keypoints. Defaults to 2048.
-            device (str, optional): The device to use. Defaults to
-                'cpu'.
+            matcher_model (str, optional): The matcher model. Defaults to 'lightglue'.
+            max_num_keypoints (int, optional): The maximum number of keypoints. Defaults
+                to 2048.
+            device (str, optional): The device to use. Defaults to 'cpu'.
         """
         super().__init__(datacube=datacube, reference=reference, **kwargs)
 
         # General attributes
         self.datacube = datacube
         self.reference = reference
 
@@ -66,32 +53,51 @@
         self.feature_model = self.feature_model.eval().to(device)
         self.matcher_model = self.matcher_model.eval().to(device)
         self.device = device
 
         # Create the reference points
         self.reference_points = self.get_reference_points()
 
-    def find_warp(self, reference_image, moving_image):
+    def find_warp(
+        self,
+        reference_image: np.ndarray,
+        moving_image: np.ndarray,
+    ) -> np.ndarray:
+        """
+        Find the warp matrix that aligns the source and
+        destination image.
+
+        Args:
+            reference_image (numpy.ndarray): The source image
+            moving_image (numpy.ndarray): The destination image
+
+        Raises:
+            ValueError: No keypoints found in the moving image.
+            ValueError: No matching points found.
+
+        Returns:
+            numpy.ndarray: The aligned source image
+        """
 
         # Load the reference points
-        feats1 = self.reference_points.copy()
+        feats1 = self.reference_points
 
-        # Moving image to torch (1xHxW)
+        # Moving feature image to torch (1 x H x W)
         moving_image_torch = (
             torch.from_numpy(moving_image).float()[None].to(self.device)
         )
 
-        # Get the reference points from the moving image
+        # Get the reference points from the moving image feature
         with torch.no_grad():
             feats0 = self.feature_model.extract(moving_image_torch, resize=None)
             if feats0["keypoints"].shape[1] == 0:
                 warnings.warn("No keypoints found in the moving image")
                 return self.warp_matrix
 
-        # Match the points
+        # Run the matcher model
         matches01 = self.matcher_model({"image0": feats0, "image1": feats1})
 
         # remove batch dimension
         feats0, feats1, matches01 = [rbd(x) for x in [feats0, feats1, matches01]]
         matches = matches01["matches"]
         points0 = feats0["keypoints"][matches[..., 0]]
         points1 = feats1["keypoints"][matches[..., 1]]
@@ -118,29 +124,33 @@
 
     def spatial_setup_model(
         self,
         feature_model: str,
         matcher_model: str,
         max_num_keypoints: int,
         device: str,
-    ) -> tuple:
+    ) -> Tuple[Union[SuperPoint, DISK, SIFT, ALIKED, DoGHardNet], LightGlue]:
         """Setup the model for spatial check
 
         Args:
-            features (str, optional): The feature extractor. Defaults to 'superpoint'.
-            matcher (str, optional): The matcher. Defaults to 'lightglue'.
-            max_num_keypoints (int, optional): The maximum number of keypoints. Defaults to 2048.
+            feature_model (str, optional): The feature extractor model. Defaults to
+                'superpoint'. Options are: 'superpoint'. Options are: 'superpoint',
+                'disk', 'sift', 'aliked', 'doghardnet'.
+            matcher_model (str, optional): The matcher model. Defaults to 'lightglue'.
+            max_num_keypoints (int, optional): The maximum number of keypoints. Defaults
+                to 2048.
             device (str, optional): The device to use. Defaults to 'cpu'.
 
         Raises:
-            ValueError: If the feature extractor or the matcher are not valid
-            ValueError: If the device is not valid
+            ValueError: Unknown feature extractor model
+            ValueError: Unknown matcher model
 
         Returns:
-            tuple: The feature extractor and the matcher models
+            Tuple[Union[SuperPoint, DISK, SIFT, ALIKED, DoGHardNet], LightGlue]: The
+                feature and matcher models
         """
 
         # Local feature extractor
         if feature_model == "superpoint":
             extractor = (
                 SuperPoint(max_num_keypoints=max_num_keypoints).eval().to(device)
             )
@@ -161,27 +171,32 @@
         if matcher_model == "lightglue":
             matcher = LightGlue(features=feature_model).eval().to(device)
         else:
             raise ValueError(f"Unknown matcher {matcher_model}")
 
         return extractor, matcher
 
-    def get_reference_points(self):
+    def get_reference_points(self) -> dict:
+        """Since the reference image is static, we extract the reference points
+        only once. This function extracts the reference points from the reference
+
+
+        Raises:
+            ValueError: No keypoints found in the reference image.
+
+        Returns:
+            dict: The reference points from the reference image (metadata)
+        """
 
         # Create the reference layer (H x W) to torch
         reference_layer = self.create_layer(img=self.reference[self.rgb_bands])
-
         reference_layer_torch = (
             torch.from_numpy(reference_layer).float()[None].to(self.device)
         )
 
         # Get the reference points from the reference image
         with torch.no_grad():
             feats0 = self.feature_model.extract(reference_layer_torch, resize=None)
             if feats0["keypoints"].shape[1] == 0:
                 raise ValueError("No keypoints found in the reference image")
 
         return feats0
-
-
-# self = LGM(datacube=s2cube, reference=reference_image)
-# self.shape
```

### Comparing `satsync-0.0.1/satsync/lightglue/aliked.py` & `satsync-0.0.2/satsync/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/disk.py` & `satsync-0.0.2/satsync/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/dog_hardnet.py` & `satsync-0.0.2/satsync/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/lightglue.py` & `satsync-0.0.2/satsync/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/sift.py` & `satsync-0.0.2/satsync/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/superpoint.py` & `satsync-0.0.2/satsync/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/utils.py` & `satsync-0.0.2/satsync/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/lightglue/viz2d.py` & `satsync-0.0.2/satsync/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.1/satsync/main.py` & `satsync-0.0.2/satsync/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,276 +1,381 @@
-"""
-An abstract class for multi-temporal image co-registration
-
-This source code is licensed under the MIT license.
-"""
-
 import concurrent.futures
 import warnings
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
+import xarray as xr
 
-
-class SuperAlignmentAbstract(ABC):
+class SatSync(ABC):
     """
     An abstract class for multi-temporal image co-registration
 
     The task uses a temporal stack of images of the same location
-    and a reference timeless feature to estimate a transformation
-    that aligns each frame of the temporal stack to the reference
-    feature.
+    and a reference timeless image to estimate a translation
+    matrix that aligns each frame of the temporal datacube to the
+    reference image.
 
     Each transformation is calculated using only a single channel
     of the images. The estimated transformations are applied to
     each of the specified features.
     """
 
     def __init__(
         self,
-        datacube: np.ndarray,
-        reference: np.ndarray,
-        channel: Union[int, str] = "luminance",
+        datacube: Union[xr.DataArray, np.ndarray],
+        reference: Union[xr.DataArray, np.ndarray],
+        channel: Union[int, str] = "mean",
         interpolation: int = cv2.INTER_LINEAR + cv2.WARP_FILL_OUTLIERS,
         crop_center: Optional[int] = None,
         rgb_bands: List[int] = [3, 2, 1],
         border_mode: int = cv2.BORDER_REPLICATE,
         num_threads: int = 4,
         max_translations: int = 5.0,
         border_value: int = 0,
     ):
         """
 
         Args:
-            datacube (xr.DataArray): The data cube to be aligned.
-            reference (Optional[xr.DataArray], optional): The reference feature.
-                Defaults to median of the images after 2022-01-01.
-            channel (Union[int, str], optional): The channel to be used for
-                alignment. Defaults to "gradients".
+            datacube (xr.DataArray): The data cube to be aligned. The data cube
+                needs to have the following dimensions: (time, bands, height, width).
+            reference (Optional[xr.DataArray], optional): The reference image.
+                The reference image needs to have the following dimensions:
+                (bands, height, width).
+            channel (Union[int, str], optional): The channel or feature to be used for
+                alignment. Defaults to "gradients". The options are:
+                - "gradients": The gradients of the image. It uses the Sobel operator
+                    to calculate the gradients.
+                - "mean": The mean of all the bands.
+                - "luminance": The luminance of the image. It uses the following
+                    formula: 0.299 * R + 0.587 * G + 0.114 * B.
+                - int: The index of the band to be used.
             interpolation (int, optional): Interpolation type used when transforming
-                the stack of images. Defaults to cv2.INTER_LINEAR.
+                the stack of images. Defaults to cv2.INTER_LINEAR + cv2.WARP_FILL_OUTLIERS.
             crop_center (Optional[int], optional): If this parameter is set, the
                 images will be cropped with respect to the center of the image to
-                calculate the warp matrix. The affine transformation will be applied
+                calculate the warp matrix. The resulted warp matrix will be applied
                 to the original image size. This can be useful for large images
                 increasing the speed of the algorithm. Defaults to None, which means
                 no cropping.
-            rgb_bands (Tuple[int, int, int], optional): The RGB bands to be used
-                when finding the gradient. Defaults to (3, 2, 1).
-            border_mode (int, optional): Defines the padding strategy when transforming
-                the images with estimated transformation. Defaults to cv2.BORDER_REPLICATE.
-            num_threads (int, optional): Number of threads used to estimate the warp.
+            rgb_bands (Tuple[int, int, int], optional): The RGB bands to be used to estimate
+                the image features when the channel is set to "gradients" or "luminance".
+                Defaults to [3, 2, 1].
+            border_mode (int, optional): Defines the padding strategy when the warp matrix
+                affects the border of the image. Defaults to cv2.BORDER_REPLICATE.
+            num_threads (int, optional): Number of threads used to estimate the warp matrix.
+                Only used in run_multicore method. The only method that supports multiple
+                threads in a safe way is PCC. If ECC needs to be used, the cv2
+                package have to be compiled with the flag WITH_TBB. Defaults to 4.
             max_translations (int, optional): Estimated transformations are considered
                 incorrect when the norm of the translation component is larger than
                 this parameter. Defaults to 5.0.
         """
 
-        # Set the class attributes
+        # Set the class attributes (REQUIRED)
         self.datacube = datacube
         self.reference = reference
+
+        # Set the class attributes (OPTIONAL)
         self.channel = channel
         self.interpolation = interpolation
         self.rgb_bands = rgb_bands
         self.border_mode = border_mode
         self.crop_center = crop_center
         self.num_threads = num_threads
         self.max_translations = max_translations
         self.border_value = border_value
 
-        # Global reference
+        # We do no support homography for now (AUTOMATIC)
         self.warp_matrix_size = (2, 3)
         self.warp_matrix: np.ndarray = np.eye(*self.warp_matrix_size, dtype=np.float32)
 
     @abstractmethod
-    def find_warp(self, reference_image, moving_image):
+    def find_warp(
+        self,
+        reference_image: np.ndarray,
+        moving_image: np.ndarray,
+    ) -> np.ndarray:
         """
-        Find the transformation between the source
-        and destination image.
+        Find the warp matrix that aligns the source and
+        destination image.
 
         Args:
             reference_image (numpy.ndarray): The source image
             moving_image (numpy.ndarray): The destination image
 
         Returns:
             numpy.ndarray: The aligned source image
         """
         pass
 
-    def warp(
-        self,
-        img: np.ndarray,
-        warp_matrix: np.ndarray,
-        shape: Tuple[int, int],
-        flags: int,
-    ) -> np.ndarray:
-        """
-        Method that applies the estimated transformation
-        to the source image
-
-        Args:
-            img (numpy.ndarray): The source image
-            warp_matrix (numpy.ndarray): The transformation matrix
-            shape (Tuple[int, int]): The shape of the destination image
-            flags (int): The flags for the transformation
-        """
-
-        return cv2.warpAffine(
-            img.astype(np.float32),
-            warp_matrix,
-            shape,
-            borderMode=self.border_mode,
-            flags=flags,
-            borderValue=self.border_value,
-        )
-
     def warp_feature(self, img: np.ndarray, warp_matrix: np.ndarray) -> np.ndarray:
         """
         Function to warp input image given an estimated
-        2D linear transformation
+        affine transformation matrix.
 
         Args:
             img (numpy.ndarray): The input image
-            warp_matrix (numpy.ndarray): The estimated
-                transformation matrix
+
+        Returns:
+            numpy.ndarray: The warped image
         """
 
         height, width = img.shape[-2:]
         warped_img = np.zeros_like(img, dtype=np.float32)
 
-        # Apply the transformation to the image
+        # Apply the transformation to each image
         for idx in range(img.shape[0]):
-            warped_img[idx, ...] = self.warp(
-                img=img[idx, ...].astype(np.float32),
-                warp_matrix=warp_matrix,
-                shape=(width, height),
+            warped_img[idx, ...] = cv2.warpAffine(
+                src=img[idx, ...].astype(np.float32),
+                M=warp_matrix,
+                dsize=(width, height),
+                borderMode=self.border_mode,
                 flags=self.interpolation,
+                borderValue=self.border_value,
             )
 
         return warped_img.astype(img.dtype)
 
     def is_translation_large(self, warp_matrix: np.ndarray) -> bool:
         """Method that checks if estimated linear translation
         could be implausible.
 
         This function checks whether the norm of the estimated
         translation in pixels exceeds a predefined value.
 
         Args:
-            warp_matrix (numpy.ndarray): The estimated transformation
-                matrix
+            warp_matrix (numpy.ndarray): The estimated warp matrix
         """
         idist = np.linalg.norm(warp_matrix[:, 2]).astype(np.float32)
         return idist > self.max_translations
 
     def create_layer(self, img: np.ndarray) -> np.ndarray:
         """
-        Method that creates a gradient image from the input image
+        Method that generate a feature image from the input image
 
         Args:
             img (numpy.ndarray): The input image
+
+        Returns:
+            numpy.ndarray: The feature image
         """
+
         # If the image has more than 3 bands, select the RGB bands
         C, H, W = img.shape
 
         if C > 3:
-            layer = img[self.rgb_bands].copy()
+            layer = img[self.rgb_bands]
         else:
-            layer = img.copy()
+            layer = img
 
         # Crop the image with respect to the centroid
         if self.crop_center is not None:
-            # if crop_center > to the original image
+
             if self.crop_center > H or self.crop_center > W:
                 raise ValueError("The crop_center should be less than the image size")
+
             radius_x = (img.shape[-1] - self.crop_center) // 2
             radius_y = (img.shape[-2] - self.crop_center) // 2
             layer = layer[:, radius_y:-radius_y, radius_x:-radius_x]
 
-        # From RGB to grayscale
-        if self.channel == "gradients":
-            global_reference = cv2.Sobel(
-                layer.mean(0).astype(np.float32), cv2.CV_32F, 1, 1
-            )
-        elif self.channel == "mean":
-            global_reference = layer.mean(0)
-        elif self.channel == "luminance":
-            global_reference = layer[0] * 0.299 + layer[1] * 0.587 + layer[2] * 0.114
+        # From RGB to grayscale (image feature)
+        if isinstance(self.channel, str):
+            if self.channel == "gradients":
+                global_reference = cv2.Sobel(
+                    layer.mean(0).astype(np.float32), cv2.CV_32F, 1, 1
+                )
+            elif self.channel == "mean":
+                global_reference = layer.mean(0)
+            elif self.channel == "luminance":
+                global_reference = (
+                    layer[0] * 0.299 + layer[1] * 0.587 + layer[2] * 0.114
+                )
+        elif isinstance(self.channel, int):
+            global_reference = layer[self.channel].copy()
         else:
-            global_reference = self.reference[self.channel]
+            raise ValueError(
+                "The channel should be a string (a specific method) or an integer (a band index)"
+            )
 
         return global_reference
 
     def get_warped_image(
-        self, reference_image: np.ndarray, moving_image: np.ndarray
-    ) -> np.ndarray:
+        self, reference_image_feature: np.ndarray, moving_image: np.ndarray
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Warp the moving image to the reference image, using the
+        estimated warp matrix.
+
+
+        Args:
+            reference_image (np.ndarray): The reference image
+            moving_image (np.ndarray): The moving image
+
+        Returns:
+            Tuple[np.ndarray, np.ndarray]: The warped image and the
+            estimated warp matrix
+        """
 
         # Obtain the warp matrix
         warp_matrix = self.find_warp(
-            reference_image=reference_image,
+            reference_image=reference_image_feature,
             moving_image=self.create_layer(moving_image),
         )
 
         # Check if the translation is large
         if self.is_translation_large(warp_matrix):
             warnings.warn("Estimated translation is too large")
             warp_matrix = self.warp_matrix
 
-        # Warp the datacube layer
+        # Warp the image using the estimated warp matrix
         warped_image = self.warp_feature(img=moving_image, warp_matrix=warp_matrix)
 
         return warped_image, warp_matrix
 
-    def run(self) -> np.ndarray:
+    def run_xarray(self) -> xr.Dataset:
         """
-        Method that estimates registrations and warps the datacube
+        Run sequantially the get_warped_image method; input is xarray
         """
+        # Create the reference feature using the reference image
+        reference_layer = self.create_layer(self.reference.values)
+
+        # Run iteratively the get_warped_image method
+        warp_matrices = []
+        warped_cube = np.zeros_like(self.datacube.values, dtype=self.datacube.dtype)
+        for index, img in enumerate(self.datacube.values):
+            # Obtain the warp matrix
+            warped_image, warp_matrix = self.get_warped_image(
+                reference_image=reference_layer,
+                moving_image=img.values,
+            )
+
+            # Save the warp matrix ... copy here makes cv2 happy
+            # weird bug that makes in the final list have the same values
+            # TODO: check in the future
+            warp_matrices.append(warp_matrix.copy())
+            warped_cube[index] = warped_image.copy()
+
+        # Create the xarray dataset
+        return xr.DataArray(
+            data=warped_cube,
+            coords=self.datacube.coords,
+            dims=self.datacube.dims,
+            attrs=self.datacube.attrs,
+        )
 
-        # Create the global reference
+    def run_numpy(self) -> np.ndarray:
+        """
+        Run sequantially the get_warped_image method; input is numpy
+        """
+
+        # Create the reference feature using the reference image
         reference_layer = self.create_layer(self.reference)
 
-        warped_cube = np.zeros_like(self.datacube, dtype=self.datacube.dtype)
+        # Run iteratively the get_warped_image method
         warp_matrices = []
+        warped_cube = np.zeros_like(self.datacube, dtype=self.datacube.dtype)
         for index, img in enumerate(self.datacube):
-            # Get the warp matrix
+            # Obtain the warp matrix
             warped_image, warp_matrix = self.get_warped_image(
                 reference_image=reference_layer, moving_image=img
             )
 
-            # Save the warp matrix ... copy makes cv2 be less buggy
+            # Save the warp matrix ... copy here makes cv2 happy
+            # weird bug that makes in the final list have the same values
+            # TODO: check in the future
             warp_matrices.append(warp_matrix.copy())
             warped_cube[index] = warped_image.copy()
 
         return warped_cube, warp_matrices
 
-    def run_multicore(self) -> np.ndarray:
+    def run_multicore_numpy(self) -> np.ndarray:
         """
-        Method that estimates registrations and warps the datacube
-        using multiple threads
+        Run the get_warped_image method using multiple threads
         """
-        # Create the global reference
+
+        # Create the reference feature using the reference image
         reference_layer = self.create_layer(self.reference)
 
         # Create the executor
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=self.num_threads
         ) as executor:
+
             futures = []
             for index, img in enumerate(self.datacube):
                 futures.append(
                     executor.submit(
                         self.get_warped_image,
                         reference_image=reference_layer,
                         moving_image=img,
                     )
                 )
 
-            # Get the results in the same order
+            # Save the results in the final list
             warped_cube = np.zeros_like(self.datacube, dtype=self.datacube.dtype)
             warp_matrices = []
             for index, future in enumerate(futures):
                 warped_image, warp_matrix = future.result()
                 warped_cube[index] = warped_image
                 warp_matrices.append(warp_matrix)
 
         return warped_cube, warp_matrices
+
+    def run_multicore_xarray(self) -> xr.Dataset:
+        """
+        Run the get_warped_image method using multiple threads
+        """
+
+        # Create the reference feature using the reference image
+        reference_layer = self.create_layer(self.reference.values)
+
+        # Create the executor
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=self.num_threads
+        ) as executor:
+
+            futures = []
+            for index, img in enumerate(self.datacube.values):
+                futures.append(
+                    executor.submit(
+                        self.get_warped_image,
+                        reference_image=reference_layer,
+                        moving_image=img.values
+                    )
+                )
+
+            # Save the results in the final list
+            warped_cube = np.zeros_like(self.datacube.values, dtype=self.datacube.dtype)
+            warp_matrices = []
+            for index, future in enumerate(futures):
+                warped_image, warp_matrix = future.result()
+                warped_cube[index] = warped_image
+                warp_matrices.append(warp_matrix)
+
+        # Create the xarray dataset
+        return xr.DataArray(
+            data=warped_cube,
+            coords=self.datacube.coords,
+            dims=self.datacube.dims,
+            attrs=self.datacube.attrs,
+        )
+
+    def run(self) -> Union[xr.Dataset, np.ndarray]:
+        """
+        Run the alignment method
+        """
+
+        if isinstance(self.datacube, xr.DataArray):
+            return self.run_xarray()
+        else:
+            return self.run_numpy()
+        
+    def run_multicore(self) -> Union[xr.Dataset, np.ndarray]:
+        """
+        Run the alignment method using multiple threads
+        """
+
+        if isinstance(self.datacube, xr.DataArray):
+            return self.run_multicore_xarray()
+        else:
+            return self.run_multicore_numpy()
```

### Comparing `satsync-0.0.1/setup.py` & `satsync-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 packages = \
 ['satsync', 'satsync.lightglue']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.26.4,<2.0.0',
+['kornia>=0.7.2,<0.8.0',
+ 'numpy>=1.26.4,<2.0.0',
  'opencv-python>=4.9.0.80,<5.0.0.0',
  'pandas>=2.2.2,<3.0.0',
  'rasterio>=1.3.10,<2.0.0',
  'scikit-image>=0.23.2,<0.24.0',
  'xarray>=2024.3.0,<2025.0.0']
 
 setup_kwargs = {
     'name': 'satsync',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'A python package to align satellite images.',
     'long_description': '# satsync\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satsync)](https://img.shields.io/github/v/release/csaybar/satsync)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satsync/main.yml?branch=main)](https://github.com/csaybar/satsync/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satsync/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satsync)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satsync)](https://img.shields.io/github/commit-activity/m/csaybar/satsync)\n[![License](https://img.shields.io/github/license/csaybar/satsync)](https://img.shields.io/github/license/csaybar/satsync)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satsync/>\n- **Documentation** <https://csaybar.github.io/satsync/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satsync.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satsync/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satsync/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'fcesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satsync',
```

### Comparing `satsync-0.0.1/PKG-INFO` & `satsync-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: satsync
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to align satellite images.
 Home-page: https://github.com/csaybar/satsync
 Author: Cesar Aybar
 Author-email: fcesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: kornia (>=0.7.2,<0.8.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: rasterio (>=1.3.10,<2.0.0)
 Requires-Dist: scikit-image (>=0.23.2,<0.24.0)
 Requires-Dist: xarray (>=2024.3.0,<2025.0.0)
 Project-URL: Documentation, https://csaybar.github.io/satsync/
```

