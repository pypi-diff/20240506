# Comparing `tmp/nwb4fp-0.6.1.3.tar.gz` & `tmp/nwb4fp-0.6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.1.3.tar", last modified: Mon May  6 11:46:34 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.1.4.tar", last modified: Mon May  6 11:49:26 2024, max compression
```

## Comparing `nwb4fp-0.6.1.3.tar` & `nwb4fp-0.6.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:35.048332 nwb4fp-0.6.1.3/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.3/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-05-06 11:46:35.041328 nwb4fp-0.6.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 11:46:35.064329 nwb4fp-0.6.1.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-05-06 11:46:31.000000 nwb4fp-0.6.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.623328 nwb4fp-0.6.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.679330 nwb4fp-0.6.1.3/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.3/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.754331 nwb4fp-0.6.1.3/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.3/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.3/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.834331 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    13322 2024-05-06 11:46:07.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.845334 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8240 2024-04-30 15:13:00.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.644331 nwb4fp-0.6.1.3/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.644331 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-04-29 13:39:41.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1425 2024-05-03 13:28:01.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.736330 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.682268 nwb4fp-0.6.1.4/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-05-06 11:49:26.675266 nwb4fp-0.6.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:49:26.697279 nwb4fp-0.6.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-05-06 11:49:22.000000 nwb4fp-0.6.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.095273 nwb4fp-0.6.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.113267 nwb4fp-0.6.1.4/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.4/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.104269 nwb4fp-0.6.1.4/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.4/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.4/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.109271 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    13322 2024-05-06 11:46:07.000000 nwb4fp-0.6.1.4/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.113267 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8240 2024-04-30 15:13:00.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.4/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.119267 nwb4fp-0.6.1.4/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.643278 nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-04-29 13:39:41.000000 nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1425 2024-05-03 13:28:01.000000 nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:49:26.100268 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-05-06 11:49:25.000000 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2024-05-06 11:49:26.000000 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:49:25.000000 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-05-06 11:49:25.000000 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 11:49:25.000000 nwb4fp-0.6.1.4/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.1.3/LICENSE` & `nwb4fp-0.6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/PKG-INFO` & `nwb4fp-0.6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.3
+Version: 0.6.1.4
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.3/README.md` & `nwb4fp-0.6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/setup.py` & `nwb4fp-0.6.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.1.3',
+    version='0.6.1.4',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.1.4/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,21 @@
     path = r"S:/Sachuriga/Ephys_Recording/CR_CA1/65410/65410_2023-11-25_13-57-58_A_phy_k_manual"
     add_wf_cor(path)
 
 def add_wf_cor(path):
 
     path_cluster_group = Path(fr"{path}/cluster_group.tsv")
     path_cluster_metrix = Path(fr"{path}/waveformsfm/extensions/quality_metrics/metrics.csv")
+    path_templates = Path(fr"{path}/waveformsfm/extensions/templates_metrics/metrics.csv")
     path_ulocation = Path(fr"{path}/waveformsfm/extensions/unit_locations/unit_locations.npy")
     df0 = pd.read_csv(path_cluster_group, index_col=0, sep='\t')
-    df1 = pd.read_csv(path_cluster_metrix)
+    df11 = pd.read_csv(path_cluster_metrix)
+    df111 = pd.read_csv(path_cluster_metrix)
+    
+    df1 = pd.merge(df11, df111,left_index=True,right_index=True)
     df2 = pd.DataFrame(np.load(path_ulocation),columns=['x', 'y','z'])
     df3 = pd.merge(df0, df1,left_index=True,right_index=True)
     df4 = pd.merge(df3, df2,left_index=True,right_index=True)
 
     # List all files in the current directory
     files = os.listdir(path)
     # Filter out files that match the pattern "cluster**.tsv"
```

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.1.4/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.1.4/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.1.4/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.1.4/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.1.4/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.1.4/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.1.4/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.3
+Version: 0.6.1.4
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.1.4/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.1.4/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

