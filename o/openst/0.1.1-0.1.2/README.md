# Comparing `tmp/openst-0.1.1.tar.gz` & `tmp/openst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openst-0.1.1.tar", max compression
+gzip compressed data, was "openst-0.1.2.tar", max compression
```

## Comparing `openst-0.1.1.tar` & `openst-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0      896 2024-04-18 14:20:31.331344 openst-0.1.1/LICENSE
--rw-r--r--   0        0        0     4265 2024-04-25 15:58:08.164649 openst-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-04-25 15:58:08.252649 openst-0.1.1/openst/__init__.py
--rw-r--r--   0        0        0      358 2024-04-25 16:16:49.572600 openst-0.1.1/openst/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.1.1/openst/alignment/__init__.py
--rw-r--r--   0        0        0     5878 2024-04-26 07:55:53.608030 openst-0.1.1/openst/alignment/apply_transform.py
--rw-r--r--   0        0        0    12248 2024-04-25 16:16:49.576600 openst-0.1.1/openst/alignment/feature_matching.py
--rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.1.1/openst/alignment/fiducial_detection.py
--rw-r--r--   0        0        0    51422 2024-04-26 18:04:33.636901 openst-0.1.1/openst/alignment/manual_pairwise_aligner.py
--rw-r--r--   0        0        0    23898 2024-04-25 16:16:49.580600 openst-0.1.1/openst/alignment/pairwise_aligner.py
--rw-r--r--   0        0        0     6620 2024-04-26 07:18:57.894428 openst-0.1.1/openst/alignment/transcript_assign.py
--rw-r--r--   0        0        0      798 2024-04-18 13:23:51.825039 openst-0.1.1/openst/alignment/transformation.py
--rw-r--r--   0        0        0    47711 2024-04-25 16:16:49.584600 openst-0.1.1/openst/cli.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.1.1/openst/metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.1.1/openst/metadata/classes/__init__.py
--rw-r--r--   0        0        0     2899 2024-04-25 16:16:49.588600 openst-0.1.1/openst/metadata/classes/base.py
--rw-r--r--   0        0        0     3539 2024-04-25 16:16:49.592600 openst-0.1.1/openst/metadata/classes/pairwise_alignment.py
--rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.1.1/openst/metadata/classes/segmentation.py
--rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.1.1/openst/metadata/example_json.json
--rw-r--r--   0        0        0     1450 2024-04-18 13:23:51.849039 openst-0.1.1/openst/metadata/report.py
--rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.1.1/openst/metadata/templates/pairwise_alignment.html
--rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.1.1/openst/preprocessing/CUT/README.md
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.1.1/openst/preprocessing/CUT/__init__.py
--rw-r--r--   0        0        0     3157 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/__init__.py
--rw-r--r--   0        0        0    11347 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/base_model.py
--rw-r--r--   0        0        0    10006 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/cut_model.py
--rw-r--r--   0        0        0    59845 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/networks.py
--rw-r--r--   0        0        0     2317 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/patchnce.py
--rw-r--r--   0        0        0     6013 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/template_model.py
--rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.1.1/openst/preprocessing/CUT/options/__init__.py
--rw-r--r--   0        0        0     8760 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/options/base_options.py
--rw-r--r--   0        0        0     1006 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/options/test_options.py
--rw-r--r--   0        0        0      132 2024-04-25 15:58:08.264649 openst-0.1.1/openst/preprocessing/CUT/util/__init__.py
--rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.1.1/openst/preprocessing/CUT/util/util.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.1.1/openst/preprocessing/__init__.py
--rw-r--r--   0        0        0     4102 2024-04-25 16:16:49.596600 openst-0.1.1/openst/preprocessing/barcode_preprocessing.py
--rw-r--r--   0        0        0     7323 2024-04-25 15:58:08.264649 openst-0.1.1/openst/preprocessing/image_preprocess.py
--rw-r--r--   0        0        0     4607 2024-04-18 13:23:51.877039 openst-0.1.1/openst/preprocessing/image_stitch.py
--rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.1.1/openst/preprocessing/imagej_macros/keyence_stitch.ijm
--rw-r--r--   0        0        0      833 2024-04-18 13:23:51.885039 openst-0.1.1/openst/preprocessing/merge_modalities.py
--rw-r--r--   0        0        0     8996 2024-04-18 13:23:51.893039 openst-0.1.1/openst/preprocessing/spatial_stitch.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.1.1/openst/segmentation/__init__.py
--rw-r--r--   0        0        0    14694 2024-04-25 15:58:08.264649 openst-0.1.1/openst/segmentation/segment.py
--rw-r--r--   0        0        0     3842 2024-04-18 13:23:51.913039 openst-0.1.1/openst/segmentation/segment_merge.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.1.1/openst/threed/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-18 13:23:51.925039 openst-0.1.1/openst/threed/from_3d_registration.py
--rw-r--r--   0        0        0     2500 2024-04-18 13:23:51.933039 openst-0.1.1/openst/threed/to_3d_registration.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.1.1/openst/utils/__init__.py
--rw-r--r--   0        0        0     9843 2024-04-25 16:16:49.596600 openst-0.1.1/openst/utils/file.py
--rw-r--r--   0        0        0    13953 2024-04-18 13:23:51.953039 openst-0.1.1/openst/utils/from_spacemake.py
--rw-r--r--   0        0        0     3401 2024-04-26 07:21:44.301924 openst-0.1.1/openst/utils/molecular_dynamics.py
--rw-r--r--   0        0        0     9680 2024-04-25 16:16:49.600600 openst-0.1.1/openst/utils/pimage.py
--rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.1.1/openst/utils/points.py
--rw-r--r--   0        0        0     2419 2024-04-18 13:23:51.969039 openst-0.1.1/openst/utils/preview.py
--rw-r--r--   0        0        0    10060 2024-04-25 16:16:49.604600 openst-0.1.1/openst/utils/pseudoimage.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.1.1/openst/utils/scanpy/__init__.py
--rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.1.1/openst/utils/scanpy/pp/__init__.py
--rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.1.1/openst/utils/scanpy/pp/_qc.py
--rw-r--r--   0        0        0     3737 2024-04-18 13:23:51.997039 openst-0.1.1/openst/utils/spacemake.py
--rw-r--r--   0        0        0     1991 2024-04-26 18:04:33.640901 openst-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 openst-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      896 2024-04-18 14:20:31.331344 openst-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4265 2024-04-25 15:58:08.164649 openst-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 15:58:08.252649 openst-0.1.2/openst/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-25 16:16:49.572600 openst-0.1.2/openst/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.1.2/openst/alignment/__init__.py
+-rw-r--r--   0        0        0     6086 2024-05-06 12:17:24.062983 openst-0.1.2/openst/alignment/apply_transform.py
+-rw-r--r--   0        0        0    12248 2024-04-25 16:16:49.576600 openst-0.1.2/openst/alignment/feature_matching.py
+-rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.1.2/openst/alignment/fiducial_detection.py
+-rw-r--r--   0        0        0    51422 2024-04-26 18:04:33.636901 openst-0.1.2/openst/alignment/manual_pairwise_aligner.py
+-rw-r--r--   0        0        0    24124 2024-05-04 18:11:32.433108 openst-0.1.2/openst/alignment/pairwise_aligner.py
+-rw-r--r--   0        0        0     6620 2024-04-26 07:18:57.894428 openst-0.1.2/openst/alignment/transcript_assign.py
+-rw-r--r--   0        0        0      798 2024-04-18 13:23:51.825039 openst-0.1.2/openst/alignment/transformation.py
+-rw-r--r--   0        0        0    47711 2024-04-25 16:16:49.584600 openst-0.1.2/openst/cli.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.1.2/openst/metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.1.2/openst/metadata/classes/__init__.py
+-rw-r--r--   0        0        0     2899 2024-04-25 16:16:49.588600 openst-0.1.2/openst/metadata/classes/base.py
+-rw-r--r--   0        0        0     3539 2024-04-25 16:16:49.592600 openst-0.1.2/openst/metadata/classes/pairwise_alignment.py
+-rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.1.2/openst/metadata/classes/segmentation.py
+-rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.1.2/openst/metadata/example_json.json
+-rw-r--r--   0        0        0     1450 2024-04-18 13:23:51.849039 openst-0.1.2/openst/metadata/report.py
+-rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.1.2/openst/metadata/templates/pairwise_alignment.html
+-rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.1.2/openst/preprocessing/CUT/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.1.2/openst/preprocessing/CUT/__init__.py
+-rw-r--r--   0        0        0     3157 2024-04-25 15:58:08.256649 openst-0.1.2/openst/preprocessing/CUT/models/__init__.py
+-rw-r--r--   0        0        0    11347 2024-04-25 15:58:08.256649 openst-0.1.2/openst/preprocessing/CUT/models/base_model.py
+-rw-r--r--   0        0        0    10006 2024-04-25 15:58:08.256649 openst-0.1.2/openst/preprocessing/CUT/models/cut_model.py
+-rw-r--r--   0        0        0    59845 2024-04-25 15:58:08.260649 openst-0.1.2/openst/preprocessing/CUT/models/networks.py
+-rw-r--r--   0        0        0     2317 2024-04-25 15:58:08.260649 openst-0.1.2/openst/preprocessing/CUT/models/patchnce.py
+-rw-r--r--   0        0        0     6013 2024-04-25 15:58:08.260649 openst-0.1.2/openst/preprocessing/CUT/models/template_model.py
+-rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.1.2/openst/preprocessing/CUT/options/__init__.py
+-rw-r--r--   0        0        0     8760 2024-04-25 15:58:08.260649 openst-0.1.2/openst/preprocessing/CUT/options/base_options.py
+-rw-r--r--   0        0        0     1006 2024-04-25 15:58:08.260649 openst-0.1.2/openst/preprocessing/CUT/options/test_options.py
+-rw-r--r--   0        0        0      132 2024-04-25 15:58:08.264649 openst-0.1.2/openst/preprocessing/CUT/util/__init__.py
+-rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.1.2/openst/preprocessing/CUT/util/util.py
+-rw-r--r--   0        0        0        0 2024-05-04 19:25:34.053904 openst-0.1.2/openst/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3832 2024-05-04 20:10:11.679024 openst-0.1.2/openst/preprocessing/barcode_preprocessing.py
+-rw-r--r--   0        0        0     7323 2024-04-25 15:58:08.264649 openst-0.1.2/openst/preprocessing/image_preprocess.py
+-rw-r--r--   0        0        0     4607 2024-04-18 13:23:51.877039 openst-0.1.2/openst/preprocessing/image_stitch.py
+-rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.1.2/openst/preprocessing/imagej_macros/keyence_stitch.ijm
+-rw-r--r--   0        0        0      833 2024-04-18 13:23:51.885039 openst-0.1.2/openst/preprocessing/merge_modalities.py
+-rw-r--r--   0        0        0     8996 2024-04-18 13:23:51.893039 openst-0.1.2/openst/preprocessing/spatial_stitch.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.1.2/openst/segmentation/__init__.py
+-rw-r--r--   0        0        0    14694 2024-04-25 15:58:08.264649 openst-0.1.2/openst/segmentation/segment.py
+-rw-r--r--   0        0        0     3842 2024-04-18 13:23:51.913039 openst-0.1.2/openst/segmentation/segment_merge.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.1.2/openst/threed/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-18 13:23:51.925039 openst-0.1.2/openst/threed/from_3d_registration.py
+-rw-r--r--   0        0        0     2500 2024-04-18 13:23:51.933039 openst-0.1.2/openst/threed/to_3d_registration.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.1.2/openst/utils/__init__.py
+-rw-r--r--   0        0        0     9843 2024-04-25 16:16:49.596600 openst-0.1.2/openst/utils/file.py
+-rw-r--r--   0        0        0    13953 2024-04-18 13:23:51.953039 openst-0.1.2/openst/utils/from_spacemake.py
+-rw-r--r--   0        0        0     9680 2024-04-25 16:16:49.600600 openst-0.1.2/openst/utils/pimage.py
+-rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.1.2/openst/utils/points.py
+-rw-r--r--   0        0        0     2418 2024-05-06 09:25:18.498645 openst-0.1.2/openst/utils/preview.py
+-rw-r--r--   0        0        0    10060 2024-04-25 16:16:49.604600 openst-0.1.2/openst/utils/pseudoimage.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.1.2/openst/utils/scanpy/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.1.2/openst/utils/scanpy/pp/__init__.py
+-rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.1.2/openst/utils/scanpy/pp/_qc.py
+-rw-r--r--   0        0        0     3737 2024-04-18 13:23:51.997039 openst-0.1.2/openst/utils/spacemake.py
+-rw-r--r--   0        0        0     1991 2024-05-06 12:19:02.306722 openst-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 openst-0.1.2/PKG-INFO
```

### Comparing `openst-0.1.1/LICENSE` & `openst-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/README.md` & `openst-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/alignment/apply_transform.py` & `openst-0.1.2/openst/alignment/apply_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import json
 import h5py
-import shutil
 
 import numpy as np
 from skimage.transform import estimate_transform as ski_estimate_transform
 
 from openst.alignment.transformation import apply_transform
-from openst.utils.file import (check_adata_structure, check_directory_exists,
-                               check_file_exists, load_properties_from_adata)
+from openst.utils.file import (check_adata_structure, check_file_exists,
+                               load_properties_from_adata)
 
 def estimate_transform(model: str, src: np.ndarray, dst: np.ndarray):
     """
     TODO: write documentation
     returns sklearn transform and True/False depending on whether flip needs to be applied to the src points before tform
     """
     tform_points = ski_estimate_transform(model, src, dst)
@@ -67,16 +66,20 @@
                 continue
             mkpts = keypoints[f'{tile_code}']
             mkpts_fine0, mkpts_fine1 = np.array(mkpts['point_src']).astype(float), np.array(mkpts['point_dst']).astype(float)
 
             _t_valid_coords = tile_id.codes == tile_code
             tform_points, needs_flip = estimate_transform("similarity", mkpts_fine1, mkpts_fine0)
             if needs_flip:
+                if len(mkpts_fine1) < 3:
+                    logging.warn(f"Skipping tile {tile_code}: optimal transform required flipping but supported by < 3 keypoints")
+                    continue
+        
                 # this applies flipping to the coordinates
-                sts_coords_transformed[..., 0] = (sts_coords_transformed[..., 0]*-1) - ((mkpts_fine1[..., 1]*-1).min() - (mkpts_fine1[..., 1]).min())
+                sts_coords_transformed[..., 0][_t_valid_coords] = ((sts_coords_transformed[..., 0]*-1) - ((mkpts_fine1[..., 1]*-1).min() - (mkpts_fine1[..., 1]).min()))[_t_valid_coords]
 
             sts_coords_transformed[..., :2][_t_valid_coords] = apply_transform(sts_coords_transformed[..., :2][_t_valid_coords], tform_points, check_bounds=check_bounds)[..., :2][..., ::-1]
 
     return sts_coords_transformed
 
 def keypoints_json_to_dict(keypoints_json):
     keypoints_by_key = {}
```

### Comparing `openst-0.1.1/openst/alignment/feature_matching.py` & `openst-0.1.2/openst/alignment/feature_matching.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/alignment/fiducial_detection.py` & `openst-0.1.2/openst/alignment/fiducial_detection.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/alignment/manual_pairwise_aligner.py` & `openst-0.1.2/openst/alignment/manual_pairwise_aligner.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/alignment/pairwise_aligner.py` & `openst-0.1.2/openst/alignment/pairwise_aligner.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,18 @@
             staining_image_rescaled.shape,
             _t_valid_coords,
             recenter=False,
             rescale=True,
             values=_t_counts,
         )
 
+        # assign same coarse coordinates if the tile falls outside of the image
+        if len(_t_sts_pseudoimage['coords_rescaled']) == 0:
+            out_coords_output_fine[_t_tile_id] = out_coords_output_coarse[_t_tile_id]
+
         # Axis limits to crop both modalities to tile region
         _t_sts_coords_to_transform = _t_sts_pseudoimage["coords_rescaled"] * _t_sts_pseudoimage["rescaling_factor"]
 
         min_lim, max_lim = _t_sts_coords_to_transform[_t_valid_coords].min(axis=0).astype(
             int
         ), _t_sts_coords_to_transform[_t_valid_coords].max(axis=0).astype(int)
         x_min, y_min = min_lim
@@ -453,15 +457,15 @@
 
         # Compute similarity matrix and compute point transformation
         if len(_t_mkpts0) > args.min_matches:
             _t_tform_points = estimate_transform("similarity", _t_mkpts0, _t_mkpts1)
 
             _t_sts_coords_fine_transformed = apply_transform(
                 _t_sts_coords_fine_to_transform, _t_tform_points, check_bounds=True
-            )[:, :-1]
+            )[:, :2]
 
             _tform_params = _t_tform_points.params.tolist()
         else:
             logging.warning(f"There were not enough matching points ({len(_t_mkpts0)} out of selected {args.min_matches})")
             _t_sts_coords_fine_transformed = _t_sts_coords_fine_to_transform[:, ::-1]
             _tform_params = None
```

### Comparing `openst-0.1.1/openst/alignment/transcript_assign.py` & `openst-0.1.2/openst/alignment/transcript_assign.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/alignment/transformation.py` & `openst-0.1.2/openst/alignment/transformation.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/cli.py` & `openst-0.1.2/openst/cli.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/classes/base.py` & `openst-0.1.2/openst/metadata/classes/base.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/classes/pairwise_alignment.py` & `openst-0.1.2/openst/metadata/classes/pairwise_alignment.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/classes/segmentation.py` & `openst-0.1.2/openst/metadata/classes/segmentation.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/example_json.json` & `openst-0.1.2/openst/metadata/example_json.json`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/report.py` & `openst-0.1.2/openst/metadata/report.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/metadata/templates/pairwise_alignment.html` & `openst-0.1.2/openst/metadata/templates/pairwise_alignment.html`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/README.md` & `openst-0.1.2/openst/preprocessing/CUT/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/__init__.py` & `openst-0.1.2/openst/preprocessing/CUT/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/base_model.py` & `openst-0.1.2/openst/preprocessing/CUT/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/cut_model.py` & `openst-0.1.2/openst/preprocessing/CUT/models/cut_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/networks.py` & `openst-0.1.2/openst/preprocessing/CUT/models/networks.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/patchnce.py` & `openst-0.1.2/openst/preprocessing/CUT/models/patchnce.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/models/template_model.py` & `openst-0.1.2/openst/preprocessing/CUT/models/template_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/options/base_options.py` & `openst-0.1.2/openst/preprocessing/CUT/options/base_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/options/test_options.py` & `openst-0.1.2/openst/preprocessing/CUT/options/test_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/CUT/util/util.py` & `openst-0.1.2/openst/preprocessing/CUT/util/util.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/barcode_preprocessing.py` & `openst-0.1.2/openst/preprocessing/barcode_preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 import gzip
 import os
 import time
 
 import pandas as pd
 
 import logging
-
+import dnaio
 
 tab = str.maketrans("ACTG", "TGAC")
 
-
 def reverse_complement_table(seq):
     return seq.translate(tab)[::-1]
 
 
 def get_tile_number_and_coordinates(read_name):
     read_name = read_name.split(" ")[0].split(":")[-3:]
     return read_name
 
 
 def process_multiple_tiles(
     in_fastq: str, out_path: str, out_prefix: str, out_suffix: str, sequence_preprocessor: callable = None
 ):
     current_tile_number = None
-    sequences, xcoords, ycoords = [[], [], []]
-    idx = 0
-    with gzip.open(in_fastq, "rt") as f:
+    n_written = 0
+    with dnaio.open(in_fastq) as f:
         for line in f:
-            if idx % 4 == 0:
-                tile_number, xcoord, ycoord = get_tile_number_and_coordinates(line.strip())
-                if current_tile_number is None:
-                    current_tile_number = tile_number
-
-                if tile_number != current_tile_number:
-                    logging.info(f"Writing {len(sequences):,} barcodes of file {current_tile_number} to disk")
-                    df = pd.DataFrame({"cell_bc": sequences, "xcoord": xcoords, "ycoord": ycoords})
-                    df.to_csv(
-                        os.path.join(
-                            out_path,
-                            out_prefix + current_tile_number + out_suffix,
-                        ),
-                        index=False,
-                        sep="\t",
-                    )
-                    current_tile_number = tile_number
-                    sequences, xcoords, ycoords = [[], [], []]
-            elif idx % 4 == 1:
-                sequence = sequence_preprocessor(line) if sequence_preprocessor is not None else line
-                sequences.append(sequence)
-                xcoords.append(xcoord)
-                ycoords.append(ycoord)
+            tile_number, xcoord, ycoord = get_tile_number_and_coordinates(line.name)
+            if current_tile_number != tile_number:
 
-            idx += 1
+                if current_tile_number is not None:
+                    logging.info(f"Written {n_written} spatial barcodes to {current_tile_number}")
+                    tile_file.close()
+
+                current_tile_number = tile_number
+
+                tile_fname = os.path.join(
+                                out_path,
+                                out_prefix + current_tile_number + out_suffix,
+                            )
+
+                tile_file = open(tile_fname, "w")
+                tile_file.write("\t".join(["cell_bc", "xcoord", "ycoord"])+"\n")
+                n_written = 0
+
+            sequence = sequence_preprocessor(line.sequence) if sequence_preprocessor is not None else line.sequence
+            tile_file.write("\t".join([sequence, xcoord, ycoord])+"\n")
+            n_written += 1
 
 
 def process_single_tile(in_fastq: str, sequence_preprocessor: callable = None) -> pd.DataFrame:
     all_tile_numbers = set()
     sequences, xcoords, ycoords = [[], [], []]
     idx = 0
     with gzip.open(in_fastq, "rt") as f:
```

### Comparing `openst-0.1.1/openst/preprocessing/image_preprocess.py` & `openst-0.1.2/openst/preprocessing/image_preprocess.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/image_stitch.py` & `openst-0.1.2/openst/preprocessing/image_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/imagej_macros/keyence_stitch.ijm` & `openst-0.1.2/openst/preprocessing/imagej_macros/keyence_stitch.ijm`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/merge_modalities.py` & `openst-0.1.2/openst/preprocessing/merge_modalities.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/preprocessing/spatial_stitch.py` & `openst-0.1.2/openst/preprocessing/spatial_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/segmentation/segment.py` & `openst-0.1.2/openst/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/segmentation/segment_merge.py` & `openst-0.1.2/openst/segmentation/segment_merge.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/threed/from_3d_registration.py` & `openst-0.1.2/openst/threed/from_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/threed/to_3d_registration.py` & `openst-0.1.2/openst/threed/to_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/file.py` & `openst-0.1.2/openst/utils/file.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/from_spacemake.py` & `openst-0.1.2/openst/utils/from_spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/pimage.py` & `openst-0.1.2/openst/utils/pimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/points.py` & `openst-0.1.2/openst/utils/points.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/preview.py` & `openst-0.1.2/openst/utils/preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     print(d)
     
 
 def _run_preview(args):
     from openst.utils.file import check_file_exists
     
     check_file_exists(args.h5_in)
-    adata = h5py.File(args.h5_in, 'r+')
+    adata = h5py.File(args.h5_in, 'r')
 
     if args.file_structure:
         logging.info(f"Showing structure from {args.h5_in}")
         _show_tree(adata, args)
     else:
         logging.info(f"Opening napari for {args.h5_in}")
         _show_viewer(adata, args)
```

### Comparing `openst-0.1.1/openst/utils/pseudoimage.py` & `openst-0.1.2/openst/utils/pseudoimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/scanpy/pp/_qc.py` & `openst-0.1.2/openst/utils/scanpy/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/openst/utils/spacemake.py` & `openst-0.1.2/openst/utils/spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.1/pyproject.toml` & `openst-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openst"
-version = "0.1.1"
+version = "0.1.2"
 description = "The computational pipeline for the Open-ST method."
 license = "GPL-2.0"
 authors = [
     "Daniel León-Periñán <daniel.leonperinan@mdc-berlin.de>",
     "Nikolaos Karaiskos <nikolaos.karaiskos@mdc-berlin.de>",
 ]
 maintainers = [
```

### Comparing `openst-0.1.1/PKG-INFO` & `openst-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openst
-Version: 0.1.1
+Version: 0.1.2
 Summary: The computational pipeline for the Open-ST method.
 License: GPL-2.0
 Author: Daniel León-Periñán
 Author-email: daniel.leonperinan@mdc-berlin.de
 Maintainer: Daniel León-Periñán
 Maintainer-email: daniel.leonperinan@mdc-berlin.de
 Requires-Python: >3.8,<3.12
```

