# Comparing `tmp/aposteriori-2.3.0.tar.gz` & `tmp/aposteriori-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aposteriori-2.3.0.tar", last modified: Wed Dec 20 10:51:05 2023, max compression
+gzip compressed data, was "aposteriori-2.4.0.tar", last modified: Mon Apr 22 12:27:28 2024, max compression
```

## Comparing `aposteriori-2.3.0.tar` & `aposteriori-2.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.099775 aposteriori-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-20 10:47:39.000000 aposteriori-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 10:47:39.000000 aposteriori-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2023-12-20 10:51:05.099775 aposteriori-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2023-12-20 10:47:39.000000 aposteriori-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-20 10:47:39.000000 aposteriori-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 10:51:05.099775 aposteriori-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-20 10:47:39.000000 aposteriori-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.095775 aposteriori-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.099775 aposteriori-2.3.0/src/aposteriori/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-20 10:47:39.000000 aposteriori-2.3.0/src/aposteriori/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2023-12-20 10:47:39.000000 aposteriori-2.3.0/src/aposteriori/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.099775 aposteriori-2.3.0/src/aposteriori/data_prep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:47:39.000000 aposteriori-2.3.0/src/aposteriori/data_prep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2023-12-20 10:47:39.000000 aposteriori-2.3.0/src/aposteriori/data_prep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    60652 2023-12-20 10:47:39.000000 aposteriori-2.3.0/src/aposteriori/data_prep/create_frame_data_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.099775 aposteriori-2.3.0/src/aposteriori.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-20 10:51:05.000000 aposteriori-2.3.0/src/aposteriori.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:51:05.099775 aposteriori-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32805 2023-12-20 10:47:39.000000 aposteriori-2.3.0/tests/test_create_frame_data_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.428696 aposteriori-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-22 12:24:07.000000 aposteriori-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 12:24:07.000000 aposteriori-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-22 12:27:28.428696 aposteriori-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-22 12:24:07.000000 aposteriori-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-22 12:24:07.000000 aposteriori-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:27:28.428696 aposteriori-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 12:24:07.000000 aposteriori-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.424696 aposteriori-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.424696 aposteriori-2.4.0/src/aposteriori/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 12:24:07.000000 aposteriori-2.4.0/src/aposteriori/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-22 12:24:07.000000 aposteriori-2.4.0/src/aposteriori/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.428696 aposteriori-2.4.0/src/aposteriori/data_prep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:24:07.000000 aposteriori-2.4.0/src/aposteriori/data_prep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-22 12:24:07.000000 aposteriori-2.4.0/src/aposteriori/data_prep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60640 2024-04-22 12:24:07.000000 aposteriori-2.4.0/src/aposteriori/data_prep/create_frame_data_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.428696 aposteriori-2.4.0/src/aposteriori.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 12:27:28.000000 aposteriori-2.4.0/src/aposteriori.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:27:28.428696 aposteriori-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33466 2024-04-22 12:24:07.000000 aposteriori-2.4.0/tests/test_create_frame_data_set.py
```

### Comparing `aposteriori-2.3.0/LICENSE` & `aposteriori-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aposteriori-2.3.0/PKG-INFO` & `aposteriori-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aposteriori
-Version: 2.3.0
+Version: 2.4.0
 Summary: A library for the voxelization of protein structures for protein design.
 Home-page: https://github.com/wells-wood-research/aposteriori
 Author: Wells Wood Research Group
 Author-email: chris.wood@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aposteriori-2.3.0/README.md` & `aposteriori-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aposteriori-2.3.0/setup.py` & `aposteriori-2.4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="aposteriori",
-    version="2.3.0",
+    version="2.4.0",
     author="Wells Wood Research Group",
     author_email="chris.wood@ed.ac.uk",
     description="A library for the voxelization of protein structures for protein design.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wells-wood-research/aposteriori",
     classifiers=[
```

### Comparing `aposteriori-2.3.0/src/aposteriori/config.py` & `aposteriori-2.4.0/src/aposteriori/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 
 from ampal.data import ELEMENT_DATA
 
 # Config paths
-MAKE_FRAME_DATASET_VER = "2.3.0"
+MAKE_FRAME_DATASET_VER = "2.4.0"
 PROJECT_ROOT_DIR = pathlib.Path(__file__).parent
 DATA_FOLDER = PROJECT_ROOT_DIR / "data"
 DATA_FOLDER.mkdir(parents=True, exist_ok=True)
 ATOM_COLORS = {
     # Atomic number : Color
     0: ELEMENT_DATA["C"]["CPK"],  # Carbon
     1: ELEMENT_DATA["N"]["CPK"],  # Nitrogen
```

### Comparing `aposteriori-2.3.0/src/aposteriori/data_prep/cli.py` & `aposteriori-2.4.0/src/aposteriori/data_prep/cli.py`

 * *Files identical despite different names*

### Comparing `aposteriori-2.3.0/src/aposteriori/data_prep/create_frame_data_set.py` & `aposteriori-2.4.0/src/aposteriori/data_prep/create_frame_data_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,15 +446,15 @@
         # The transpose changes arrays of [y], [x], [z] into [y, x, z]
         for voxel_coord in np.array(xyz_coordinates).T:
             # Extract voxel coords:
             vy, vx, vz = voxel_coord
             # Calculate Density:
             voxel_density = np.exp(
                 -((vx - x) ** 2 + (vy - y) ** 2 + (vz - z) ** 2)
-                / wanderwaal_radius**2
+                / wanderwaal_radius ** 2
             )
             # Add density to frame:
             gaussian_frame[vy, vx, vz] = voxel_density
 
     # Normalize so that values add up to 1:
     norm_gaussian_frame = gaussian_frame / np.sum(gaussian_frame)
 
@@ -579,20 +579,33 @@
     frame_slice += density_matrix_slice
     # Add to original array:
     density_frame[:, :, :, atom_idx] += empty_frame_voxels
 
     return density_frame
 
 
+def charge_polar_property(res: ampal.Residue, codec: Codec):
+    if "P" in codec.atomic_labels:
+        if res.mol_letter in standard_amino_acids.keys():
+            res_property = -1 if polarity_Zimmerman[res.mol_letter] < 20 else 1
+        else:
+            res_property = 0
+    elif "Q" in codec.atomic_labels:
+        res_property = residue_charge[res.mol_letter]
+    else:
+        res_property = 0
+    return res_property
+
+
 def create_residue_frame(
     residue: ampal.Residue,
     frame_edge_length: float,
     voxels_per_side: int,
     encode_cb: bool,
-    codec: object,
+    codec: Codec,
     voxels_as_gaussian: bool = False,
 ) -> np.ndarray:
     """Creates a discrete representation of a volume of space around a residue.
 
     Notes
     -----
     We use the term "frame" to refer to a cube of space around a residue.
@@ -630,23 +643,14 @@
         * If any voxel is already occupied
         * If the central voxel in the frame is not carbon as it should the the CA atom
     """
     assert voxels_per_side % 2, "The number of voxels per side should be odd."
     voxel_edge_length = frame_edge_length / voxels_per_side
     assembly = residue.parent.parent
     chain = residue.parent
-    if "P" in codec.atomic_labels:
-        if residue.mol_letter in standard_amino_acids.keys():
-            res_property = -1 if polarity_Zimmerman[residue.mol_letter] < 20 else 1
-        else:
-            res_property = 0
-        # res_property = -1 if res_property < 20 else 1
-    elif "Q" in codec.atomic_labels:
-        res_property = residue_charge[residue.mol_letter]
-
     align_to_residue_plane(residue)
 
     frame = np.zeros(
         (voxels_per_side, voxels_per_side, voxels_per_side, codec.encoder_length),
     )
     # Change frame type to float if gaussian else use bool:
     frame = frame.astype(np.float16) if voxels_as_gaussian else frame.astype(np.bool)
@@ -678,14 +682,15 @@
             # If the voxel is a gaussian, there may be remnants of a nearby atom
             # hence this test would fail
         if not voxels_as_gaussian:
             if not atom.res_label == "CB":
                 np.testing.assert_array_equal(
                     frame[indices], np.array([False] * len(frame[indices]), dtype=bool)
                 )
+        res_property = charge_polar_property(res, codec)
         # Encode atoms:
         if voxels_as_gaussian:
             modifiers_triple = calculate_atom_coord_modifier_within_voxel(
                 atom, voxel_edge_length, indices, adjust_by=voxels_per_side // 2
             )
             # Get Gaussian encoding
             gaussian_matrix, atom_idx = Codec.encode_gaussian_atom(
@@ -695,19 +700,15 @@
             # Add at position:
             frame = add_gaussian_at_position(
                 main_matrix=frame,
                 secondary_matrix=gaussian_atom,
                 atom_coord=indices,
                 atom_idx=atom_idx,
             )
-            if (
-                "Q" in codec.atomic_labels
-                or "P" in codec.atomic_labels
-                and res_property != 0
-            ):
+            if res_property != 0:
                 gaussian_atom = gaussian_matrix[:, :, :, atom_idx] * float(res_property)
                 # Add at position:
                 frame = add_gaussian_at_position(
                     main_matrix=frame,
                     secondary_matrix=gaussian_atom,
                     atom_coord=indices,
                     atom_idx=5,
@@ -1636,15 +1637,15 @@
     total_files = len(filtered_structure_files)
     processed_files = 0
     number_of_frames = 0
 
     print(f"Will attempt to process {total_files} structure file/s.")
     print(f"Output file will be written to `{output_file_path.resolve()}`.")
     voxel_edge_length = frame_edge_length / voxels_per_side
-    max_voxel_distance = np.sqrt(voxel_edge_length**2 * 3)
+    max_voxel_distance = np.sqrt(voxel_edge_length ** 2 * 3)
     print(f"Frame edge length = {frame_edge_length:.2f} A")
     print(f"Voxels per side = {voxels_per_side}")
     print(f"Voxels will have an edge length of {voxel_edge_length:.2f} A.")
     print(f"Max internal distance of each voxel will be {max_voxel_distance:.2f} A.")
     if require_confirmation:
         print("Do you want to continue? [y]/n")
         response = input()
```

### Comparing `aposteriori-2.3.0/src/aposteriori.egg-info/PKG-INFO` & `aposteriori-2.4.0/src/aposteriori.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aposteriori
-Version: 2.3.0
+Version: 2.4.0
 Summary: A library for the voxelization of protein structures for protein design.
 Home-page: https://github.com/wells-wood-research/aposteriori
 Author: Wells Wood Research Group
 Author-email: chris.wood@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aposteriori-2.3.0/tests/test_create_frame_data_set.py` & `aposteriori-2.4.0/tests/test_create_frame_data_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,19 @@
                     ),
                 )
                 charge = residue_charge[ampal_1ubq["A"][residue_number].mol_letter]
                 if charge > 0:
                     assert np.max(test_residue[:, :, :, 5]) > 0
                 if charge < 0:
                     assert np.min(test_residue[:, :, :, 5]) < 0
+                if residue_number == "32" or residue_number == "33":
+                    assert (
+                        np.max(test_residue[:, :, :, 5]) > 0
+                        and np.min(test_residue[:, :, :, 5]) < 0
+                    ), "Frame 32 and 33 should have both positive and negative values as the residues are Lys and Asp"
 
 
 def test_make_frame_dataset_as_gaussian_cnocacbp():
     """Tests the creation of a frame data set."""
     test_file = TEST_DATA_DIR / "1ubq.pdb"
     frame_edge_length = 18.0
     voxels_per_side = 31
@@ -479,19 +484,19 @@
             voxels_as_gaussian=True,
         )
         with h5py.File(output_file_path, "r") as dataset:
             for n in range(1, 77):
                 # check that the frame for all the data frames match between the input
                 # arrays and the ones that come out of the HDF5 data set
                 residue_number = str(n)
-                residue_test = array_test[n - 1]
+                test_residue = array_test[n - 1]
                 hdf5_array = dataset["1ubq"]["A"][residue_number][()]
                 npt.assert_array_equal(
                     hdf5_array,
-                    residue_test,
+                    test_residue,
                     err_msg=(
                         "The frame in the HDF5 data set should be the same as the "
                         "input frame."
                     ),
                 )
             if (
                 ampal_1ubq["A"][residue_number].mol_letter
@@ -502,18 +507,22 @@
                     if polarity_Zimmerman[ampal_1ubq["A"][residue_number].mol_letter]
                     < 20
                     else 1
                 )
             else:
                 polarity = 0
             if polarity == 1:
-                assert np.max(residue_test[:, :, :, 5]) > 0
+                assert np.max(test_residue[:, :, :, 5]) > 0
             if polarity == 0:
-                assert np.min(residue_test[:, :, :, 5]) < 0
-
+                assert np.min(test_residue[:, :, :, 5]) < 0
+            if residue_number == "5" or residue_number == "6":
+                assert (
+                    np.max(test_residue[:, :, :, 5]) > 0
+                    and np.min(test_residue[:, :, :, 5]) < 0
+                ), "Frame 5 and 6 should have both positive and negative values as the residues are Lys and Asp"
 
 @settings(deadline=700)
 @given(integers(min_value=0, max_value=214))
 def test_default_atom_filter(residue_number: int):
     assembly = ampal.load_pdb(str(TEST_DATA_DIR / "3qy1.pdb"))
     focus_residue = assembly[0][residue_number]
     backbone_atoms = ("N", "CA", "C", "O")
```

