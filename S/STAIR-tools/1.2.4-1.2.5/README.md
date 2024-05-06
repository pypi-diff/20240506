# Comparing `tmp/STAIR-tools-1.2.4.tar.gz` & `tmp/STAIR-tools-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.2.4.tar", last modified: Sun May  5 07:43:21 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.5.tar", last modified: Mon May  6 15:44:10 2024, max compression
```

## Comparing `STAIR-tools-1.2.4.tar` & `STAIR-tools-1.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.830361 STAIR-tools-1.2.4/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 07:43:21.829929 STAIR-tools-1.2.4/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.4/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.820789 STAIR-tools-1.2.4/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.4/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.821098 STAIR-tools-1.2.4/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.4/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.4/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-05-05 07:41:17.000000 STAIR-tools-1.2.4/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.827386 STAIR-tools-1.2.4/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.4/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.4/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3933 2024-05-05 07:43:06.000000 STAIR-tools-1.2.4/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.4/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.4/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.4/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.4/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.4/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.4/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.829045 STAIR-tools-1.2.4/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.4/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.4/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.4/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.4/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.4/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.4/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.4/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-05 07:43:21.829686 STAIR-tools-1.2.4/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-05 07:43:21.000000 STAIR-tools-1.2.4/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-05 07:43:21.000000 STAIR-tools-1.2.4/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-05 07:43:21.000000 STAIR-tools-1.2.4/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-05 07:43:21.000000 STAIR-tools-1.2.4/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-05 07:43:21.830416 STAIR-tools-1.2.4/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-05 07:43:16.000000 STAIR-tools-1.2.4/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.667342 STAIR-tools-1.2.5/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 15:44:10.667026 STAIR-tools-1.2.5/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.5/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.662051 STAIR-tools-1.2.5/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.5/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.662386 STAIR-tools-1.2.5/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.5/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.664597 STAIR-tools-1.2.5/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.5/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.5/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6022 2024-05-06 15:43:27.000000 STAIR-tools-1.2.5/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.5/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.5/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.666191 STAIR-tools-1.2.5/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.5/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.5/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.5/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-06 15:44:10.666804 STAIR-tools-1.2.5/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-06 15:44:10.000000 STAIR-tools-1.2.5/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-06 15:44:10.667412 STAIR-tools-1.2.5/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-06 15:43:42.000000 STAIR-tools-1.2.5/setup.py
```

### Comparing `STAIR-tools-1.2.4/README.md` & `STAIR-tools-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.5/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/emb_alignment.py` & `STAIR-tools-1.2.5/STAIR/emb_alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             slice_key = self.batch_key
         
         self.data_hgat, self.kernals, self.index_dict = hgat_data(  self.adata, 
                                                                     batch_key = slice_key, 
                                                                     batch_order = slice_order, 
                                                                     spatial_key = spatial_key, 
                                                                     n_neigh_hom = n_neigh_hom, 
-                                                                    n_radius_het = 1-c_neigh_het,
+                                                                    c_neigh_het = c_neigh_het,
                                                                     kernal_thresh = kernal_thresh)
         
         if self.make_log:
             self.makeLog(f"Module parameter set of HGAT")
             self.makeLog(f"  Spatial key: {spatial_key}")
             self.makeLog(f"  Neighbor number of intra-slice: {n_neigh_hom}")
             self.makeLog(f"  Similarity cutoff of inter-slice: {c_neigh_het}")
```

### Comparing `STAIR-tools-1.2.4/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.2.5/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/embedding/loss.py` & `STAIR-tools-1.2.5/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.5/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.5/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.5/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/loc_alignment.py` & `STAIR-tools-1.2.5/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/loc_prediction.py` & `STAIR-tools-1.2.5/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/location/align_fine.py` & `STAIR-tools-1.2.5/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/location/align_init.py` & `STAIR-tools-1.2.5/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.5/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.5/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/location/transformation.py` & `STAIR-tools-1.2.5/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR/utils.py` & `STAIR-tools-1.2.5/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.4/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.5/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

