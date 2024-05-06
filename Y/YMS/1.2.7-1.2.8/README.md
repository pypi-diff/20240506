# Comparing `tmp/YMS-1.2.7.tar.gz` & `tmp/YMS-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-1.2.7.tar", last modified: Mon Feb 19 11:10:52 2024, max compression
+gzip compressed data, was "YMS-1.2.8.tar", last modified: Mon May  6 10:18:26 2024, max compression
```

## Comparing `YMS-1.2.7.tar` & `YMS-1.2.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-02-19 11:10:52.312437 YMS-1.2.7/
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-02-19 11:10:52.312437 YMS-1.2.7/PKG-INFO
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5359 2024-02-19 11:08:39.000000 YMS-1.2.7/README.md
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-02-19 11:10:52.188437 YMS-1.2.7/YMS.egg-info/
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)      370 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        1 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       15 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/requires.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        6 2024-02-19 11:10:52.000000 YMS-1.2.7/YMS.egg-info/top_level.txt
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-02-19 11:10:52.312437 YMS-1.2.7/setup.cfg
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)      734 2024-02-19 10:15:52.000000 YMS-1.2.7/setup.py
-drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-02-19 11:10:52.260437 YMS-1.2.7/yamas/
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     5878 2024-02-19 10:15:25.000000 YMS-1.2.7/yamas/__init__.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)       30 2023-10-30 09:49:55.000000 YMS-1.2.7/yamas/config.json
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    20526 2024-02-19 10:15:25.000000 YMS-1.2.7/yamas/create_visualization.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     2284 2023-12-22 15:07:55.000000 YMS-1.2.7/yamas/dataset_downloading.py
--rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    14620 2024-02-19 10:27:35.000000 YMS-1.2.7/yamas/export_data.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1900 2023-11-14 07:32:14.000000 YMS-1.2.7/yamas/prerun_configs.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)    10075 2024-01-11 07:50:12.000000 YMS-1.2.7/yamas/qiita_visualization.py
--rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1183 2023-10-30 09:49:55.000000 YMS-1.2.7/yamas/utilities.py
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.774043 YMS-1.2.8/
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:18:26.774043 YMS-1.2.8/PKG-INFO
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5359 2024-02-19 11:08:39.000000 YMS-1.2.8/README.md
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.770043 YMS-1.2.8/YMS.egg-info/
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     5637 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)      399 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        1 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       15 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/requires.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)        6 2024-05-06 10:18:26.000000 YMS-1.2.8/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)       38 2024-05-06 10:18:26.774043 YMS-1.2.8/setup.cfg
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)      734 2024-05-06 10:17:39.000000 YMS-1.2.8/setup.py
+drwxrwxr-x   0 shanif3   (1002) shanif3   (1002)        0 2024-05-06 10:18:26.774043 YMS-1.2.8/yamas/
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     6420 2024-03-07 12:02:41.000000 YMS-1.2.8/yamas/__init__.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)       30 2023-10-30 09:49:55.000000 YMS-1.2.8/yamas/config.json
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    20526 2024-02-19 10:15:25.000000 YMS-1.2.8/yamas/create_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     2633 2024-03-07 12:06:45.000000 YMS-1.2.8/yamas/dataset_downloading.py
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)    14620 2024-02-19 10:27:35.000000 YMS-1.2.8/yamas/export_data.py
+-rw-rw-r--   0 shanif3   (1002) shanif3   (1002)     6455 2024-03-07 12:34:34.000000 YMS-1.2.8/yamas/fastq_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1900 2023-11-14 07:32:14.000000 YMS-1.2.8/yamas/prerun_configs.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)    10075 2024-05-06 10:16:15.000000 YMS-1.2.8/yamas/qiita_visualization.py
+-rw-rw-rw-   0 shanif3   (1002) shanif3   (1002)     1183 2023-10-30 09:49:55.000000 YMS-1.2.8/yamas/utilities.py
```

### Comparing `YMS-1.2.7/PKG-INFO` & `YMS-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YMS
-Version: 1.2.7
+Version: 1.2.8
 Summary: YOLO Microbiome Analysis System
 Home-page: UNKNOWN
 Author: Yarin Bekor, Shani Finkelstein
 Author-email: yarin.bekor@gmail.com, shaninn123@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `YMS-1.2.7/README.md` & `YMS-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `YMS-1.2.7/YMS.egg-info/PKG-INFO` & `YMS-1.2.8/YMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YMS
-Version: 1.2.7
+Version: 1.2.8
 Summary: YOLO Microbiome Analysis System
 Home-page: UNKNOWN
 Author: Yarin Bekor, Shani Finkelstein
 Author-email: yarin.bekor@gmail.com, shaninn123@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `YMS-1.2.7/yamas/__init__.py` & `YMS-1.2.8/yamas/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pkg_resources
 from .dataset_downloading import download
 from .dataset_downloading import continue_from
 from .dataset_downloading import continue_from_fastq
 from .export_data import export
 from .prerun_configs import set_environment
 from .dataset_downloading import download_qiita
+from .dataset_downloading import download_fastq
 
 
 def main():
     # Initialize the argument parser with a description.
     parser = argparse.ArgumentParser(description='YMS package')
 
     # Add an argument for displaying the version of the YMS package.
@@ -21,14 +22,16 @@
 
     parser.add_argument('--qiita', nargs=3, metavar=("PREPROCESSED FASTQ PATH", "METADATA PATH", "DATA_TYPE"), help= "All can be found in https://qiita.ucsd.edu/ \n Where preprocessed fastq can be found? \n click the study description --> in the graph click on demultiplexed --> scroll down and download 'preprocessed fastq' \n Where metadata can be found? \n   click the study description --> download 'Prep info' ")
 
     parser.add_argument('--continue_from', nargs=3, metavar=('DATASET_ID','PATH', 'DATA_TYPE'), help='Continue processing from a specific path with a given data type')
 
     parser.add_argument('--continue_from_fastq', nargs=3, metavar=('DATASET_ID','PATH', 'DATA_TYPE'), help='Continue downloading from a specific path with a given data type')
 
+    parser.add_argument('--fastq', nargs=4, metavar=("PREPROCESSED FASTQ PATH", "PREPROCESSED FASTQ PATH","METADATA PATH", "DATA_TYPE"), help= "All can be found in https://qiita.ucsd.edu/ \n Where preprocessed fastq can be found? \n click the study description --> in the graph click on demultiplexed --> scroll down and download 'preprocessed fastq' \n Where metadata can be found? \n   click the study description --> download 'Prep info' ")
+
     # Add an argument for specifying datasets to be downloaded.
     parser.add_argument('--download', nargs='+', help='Add datasets to be downloaded')
 
     # Add an argument for specifying the type of data to be downloaded (16S or Shotgun).
     parser.add_argument('--type', nargs=1, choices=['16S','18S', 'Shotgun'], help='Type of data to be downloaded')
 
     # Add an argument for specifying export parameters.
@@ -105,20 +108,21 @@
         if data_type=='16S' or data_type=='18S' or data_type=='Shotgun':
             continue_from(dataset_id,continue_path,data_type, args.verbose, specific_location)
 
         else:
             # Ensure that a dataset type is specified when downloading datasets.
             raise ValueError("Missing dataset type. Use --type 16S/18S/Shotgun")
 
-    if args.qiita:
-        fastq_path= args.qiita[0]
-        metadata_path= args.qiita[1]
-        data_type= args.qiita[2]
+    if args.fastq:
+        fastq_path= args.fastq[0]
+        barcode_path= args.fastq[1]
+        metadata_path= args.qiita[2]
+        data_type= args.qiita[3]
         if data_type=='16S' or data_type=='18S' or data_type=='Shotgun':
-            download_qiita(fastq_path,metadata_path,data_type, args.verbose)
+            download_fastq(fastq_path,barcode_path,metadata_path,data_type, args.verbose)
 
         else:
             # Ensure that a dataset type is specified when downloading datasets.
             raise ValueError("Missing dataset type. Use --type 16S/18S/Shotgun")
```

### Comparing `YMS-1.2.7/yamas/create_visualization.py` & `YMS-1.2.8/yamas/create_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.7/yamas/dataset_downloading.py` & `YMS-1.2.8/yamas/dataset_downloading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .create_visualization import visualization
 from .create_visualization import visualization_continue
 from .create_visualization import visualization_continue_fastq
 from .qiita_visualization import qiita_visualization
+from .fastq_visualization import fastq_visualization
 
 import os
 
 
 # This function downloads the accession list for the specified project (Using the SRA databse, which holds all the necessery metadata.)
 def get_acc_list(bio_project_name, verbose_print):
     get_run_info_command = f'esearch -db sra -query {bio_project_name} | efetch -format runinfo > {bio_project_name}_run_info.csv'
@@ -48,7 +49,16 @@
 def download_qiita(fastq_path,metadata_path,data_type, verbose):
     verbose_print = print if verbose else lambda *a, **k: None
 
     verbose_print("\n")
     verbose_print("download starts.")
 
     qiita_visualization(fastq_path,metadata_path,data_type, verbose_print)
+
+
+def download_fastq(fastq_path,barcode_path,metadata_path,data_type, verbose):
+    verbose_print = print if verbose else lambda *a, **k: None
+
+    verbose_print("\n")
+    verbose_print("download starts.")
+
+    fastq_visualization(fastq_path,barcode_path, metadata_path, data_type, verbose_print)
```

### Comparing `YMS-1.2.7/yamas/export_data.py` & `YMS-1.2.8/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.7/yamas/prerun_configs.py` & `YMS-1.2.8/yamas/prerun_configs.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.7/yamas/qiita_visualization.py` & `YMS-1.2.8/yamas/qiita_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-1.2.7/yamas/utilities.py` & `YMS-1.2.8/yamas/utilities.py`

 * *Files identical despite different names*

