# Comparing `tmp/nwb4fp-0.6.1.1.tar.gz` & `tmp/nwb4fp-0.6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.1.1.tar", last modified: Mon Apr 29 14:41:10 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.1.3.tar", last modified: Mon May  6 11:46:34 2024, max compression
```

## Comparing `nwb4fp-0.6.1.1.tar` & `nwb4fp-0.6.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:10.349249 nwb4fp-0.6.1.1/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.1/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-04-29 14:41:10.342250 nwb4fp-0.6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 14:41:10.364244 nwb4fp-0.6.1.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-29 14:41:06.000000 nwb4fp-0.6.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:09.881254 nwb4fp-0.6.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:09.953245 nwb4fp-0.6.1.1/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.1/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:10.034245 nwb4fp-0.6.1.1/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.1/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.1/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:10.140245 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    13220 2024-04-26 10:54:41.000000 nwb4fp-0.6.1.1/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:10.237245 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8199 2024-04-29 14:39:37.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.1/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:09.907247 nwb4fp-0.6.1.1/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:09.907247 nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-04-29 13:39:41.000000 nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1425 2024-04-28 10:02:22.000000 nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:41:10.014245 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-04-29 14:41:09.000000 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2024-04-29 14:41:09.000000 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:41:09.000000 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-04-29 14:41:09.000000 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 14:41:09.000000 nwb4fp-0.6.1.1/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:35.048332 nwb4fp-0.6.1.3/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-05-06 11:46:35.041328 nwb4fp-0.6.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:46:35.064329 nwb4fp-0.6.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-05-06 11:46:31.000000 nwb4fp-0.6.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.623328 nwb4fp-0.6.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.679330 nwb4fp-0.6.1.3/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.3/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.754331 nwb4fp-0.6.1.3/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.3/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.3/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.834331 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    13322 2024-05-06 11:46:07.000000 nwb4fp-0.6.1.3/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.845334 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8240 2024-04-30 15:13:00.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.3/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.644331 nwb4fp-0.6.1.3/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.644331 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-04-29 13:39:41.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1425 2024-05-03 13:28:01.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:46:34.736330 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 11:46:34.000000 nwb4fp-0.6.1.3/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.1.1/LICENSE` & `nwb4fp-0.6.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/PKG-INFO` & `nwb4fp-0.6.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.1
+Version: 0.6.1.3
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.1/README.md` & `nwb4fp-0.6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/setup.py` & `nwb4fp-0.6.1.3/setup.py`

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
-    version='0.6.1.1',
+    version='0.6.1.3',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.1.3/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.1.3/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,17 +203,20 @@
     we1 = analyzer.compute("templates")
     #get potential merging sorting objects
     print("processing potential merge...\n")
     
     sort_merge = get_potential_merge(sorting, analyzer)
     analyzer1 = si.create_sorting_analyzer(sorting=sorting, recording=rec_w, format='binary_folder', folder=fr"{temp_folder}_analy",overwrite=True)
     we = analyzer1.compute("random_spikes","waveforms")
+    
     we = analyzer1.compute("waveforms")
     we = analyzer1.compute("noise_levels")
     we = analyzer1.compute("templates")
+    we = analyzer1.compute("spike_amplitudes")
+    we = analyzer1.compute("template_metrics")
     we = analyzer1.compute("quality_metrics")
     ccg = analyzer1.compute(input="correlograms",
                             window_ms=1000.0,
                             bin_ms=10.0,
                             method="auto")
     
     sim = analyzer1.compute("template_similarity", method="cosine_similarity")
```

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     job_kwargs = dict(n_jobs=12,
                               chunk_duration="5s",
                               progress_bar=True)
     print("processing lfp data...")
     base_folder = Path("C:/temp_lfp")
     preprocessed = "_" + "preprocessed_temp"
     lfp.save(folder=base_folder / preprocessed, overwrite=True, **job_kwargs)
+    print(fr"LFP shape is {lfp.shape}")
     recording_rec = si.load_extractor(base_folder / preprocessed)
     return recording_rec
 
 def add_lfp2nwb(filename,channel2selec,folder1_path):
 
     with NWBHDF5IO(filename, "r+") as io:
         read_nwbfile = io.read()
```

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.1.3/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def main():
     import os
     import sys
     base_path = Path("Q:/Sachuriga/Sachuriga_Python")
     base_data_folder = Path("S:/Sachuriga/")
     sex = "F"
-    animals = ["65283"] 
+    animals = ["65935"] 
     age = "P45+"
     project_name = "CR_CA1"
     species = "Mus musculus"
     vedio_search_directory = base_data_folder/fr"Ephys_Vedio/CR_CA1/"
     path_save = base_data_folder/fr"nwb"
     temp_folder = Path(r'C:/temp_waveform/')
     save_path_test=(r"S:\Sachuriga/Ephys_Recording/4nwb_check.csv")
```

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.1.3/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.1
+Version: 0.6.1.3
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.1/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.1.3/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

