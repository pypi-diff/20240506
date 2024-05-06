# Comparing `tmp/cvmtrans-0.0.7.tar.gz` & `tmp/cvmtrans-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvmtrans-0.0.7.tar", last modified: Tue Apr 30 08:00:20 2024, max compression
+gzip compressed data, was "cvmtrans-0.0.8.tar", last modified: Mon May  6 13:06:52 2024, max compression
```

## Comparing `cvmtrans-0.0.7.tar` & `cvmtrans-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 08:00:20.998221 cvmtrans-0.0.7/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2503 2024-04-30 08:00:20.998091 cvmtrans-0.0.7/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1754 2024-04-30 07:58:39.000000 cvmtrans-0.0.7/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 08:00:20.996974 cvmtrans-0.0.7/cvmtrans/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:59:54.000000 cvmtrans-0.0.7/cvmtrans/__init__.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8775 2024-04-08 10:09:38.000000 cvmtrans-0.0.7/cvmtrans/cvmtrans.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 07:49:13.000000 cvmtrans-0.0.7/cvmtrans/cvmtrans_cut_tags.py
--rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-30 07:49:15.000000 cvmtrans-0.0.7/cvmtrans/cvmtrans_extract_reads.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.7/cvmtrans/data_process.sh
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.7/cvmtrans/embl_parse.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.7/cvmtrans/embl_parse_test.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.7/cvmtrans/gb2fa.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.7/cvmtrans/parse_bam.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 08:00:20.997879 cvmtrans-0.0.7/cvmtrans.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2503 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      167 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 08:00:20.000000 cvmtrans-0.0.7/cvmtrans.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.7/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 08:00:20.998271 cvmtrans-0.0.7/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2281 2024-04-30 07:54:32.000000 cvmtrans-0.0.7/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-05-06 13:06:52.350255 cvmtrans-0.0.8/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2491 2024-05-06 13:06:52.350120 cvmtrans-0.0.8/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1742 2024-04-30 08:02:08.000000 cvmtrans-0.0.8/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-05-06 13:06:52.349063 cvmtrans-0.0.8/cvmtrans/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-05-06 13:06:33.000000 cvmtrans-0.0.8/cvmtrans/__init__.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8775 2024-05-06 13:05:28.000000 cvmtrans-0.0.8/cvmtrans/cvmtrans.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3784 2024-05-06 13:05:14.000000 cvmtrans-0.0.8/cvmtrans/cvmtrans_cut_tags.py
+-rwx------   0 cuiqingpo   (501) staff       (20)     3602 2024-05-06 13:05:35.000000 cvmtrans-0.0.8/cvmtrans/cvmtrans_extract_reads.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.8/cvmtrans/data_process.sh
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.8/cvmtrans/embl_parse.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.8/cvmtrans/embl_parse_test.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.8/cvmtrans/gb2fa.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.8/cvmtrans/parse_bam.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-05-06 13:06:52.349941 cvmtrans-0.0.8/cvmtrans.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2491 2024-05-06 13:06:51.000000 cvmtrans-0.0.8/cvmtrans.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-05-06 13:06:52.000000 cvmtrans-0.0.8/cvmtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-05-06 13:06:51.000000 cvmtrans-0.0.8/cvmtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      167 2024-05-06 13:06:51.000000 cvmtrans-0.0.8/cvmtrans.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-05-06 13:06:51.000000 cvmtrans-0.0.8/cvmtrans.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-05-06 13:06:51.000000 cvmtrans-0.0.8/cvmtrans.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.8/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-05-06 13:06:52.350300 cvmtrans-0.0.8/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2281 2024-04-30 07:54:32.000000 cvmtrans-0.0.8/setup.py
```

### Comparing `cvmtrans-0.0.7/PKG-INFO` & `cvmtrans-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.7
+Version: 0.0.8
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # cvmtrans
 
 ![PYPI](https://img.shields.io/pypi/v/cvmtrans)
-![Static Badge](https://img.shields.io/badge/OS-_Windows_%7C_Mac_%7C_Linux-steelblue)
+![Static Badge](https://img.shields.io/badge/OS-_Mac_%7C_Linux-steelblue)
 
 
 ## Installation
 
 pip3 install cvmtrans
```

### Comparing `cvmtrans-0.0.7/README.md` & `cvmtrans-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # cvmtrans
 
 ![PYPI](https://img.shields.io/pypi/v/cvmtrans)
-![Static Badge](https://img.shields.io/badge/OS-_Windows_%7C_Mac_%7C_Linux-steelblue)
+![Static Badge](https://img.shields.io/badge/OS-_Mac_%7C_Linux-steelblue)
 
 
 ## Installation
 
 pip3 install cvmtrans
```

### Comparing `cvmtrans-0.0.7/cvmtrans/cvmtrans.py` & `cvmtrans-0.0.8/cvmtrans/cvmtrans.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.7/cvmtrans/cvmtrans_cut_tags.py` & `cvmtrans-0.0.8/cvmtrans/cvmtrans_cut_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,17 @@
     else:
         return True
 
 
 def main():
     args = args_parse()
     input_fq = os.path.abspath(args.i)
-    current_path = os.path.abspath(os.path.dirname(__file__))
+    # resolve output file bug
+    # current_path = os.path.abspath(os.path.dirname(__file__))
+    current_path = os.getcwd()
     output_fq = os.path.join(current_path, args.o)
     tag5 = args.tag_5
     tag3 = args.tag_3
 
     if tag5 is None and tag3 is None:
         print("The tag sequence must provide!")
         sys.exit(1)
```

### Comparing `cvmtrans-0.0.7/cvmtrans/cvmtrans_extract_reads.py` & `cvmtrans-0.0.8/cvmtrans/cvmtrans_extract_reads.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     # print(f'Saved reads: {saved_reads}')
     return total_reads, saved_reads
 
 
 def main():
     args = args_parse()
     input_fq = os.path.abspath(args.i)
-    current_path = os.path.abspath(os.path.dirname(__file__))
+    # resolve output file bug
+    # current_path = os.path.abspath(os.path.dirname(__file__))
+    current_path = os.getcwd()
     output_fq = os.path.join(current_path, args.o)
     tag = args.tag
     # print(tag)
     # print(input_fq)
     # print(output_fq)
     # print(tag)
     print(f'Start processing {args.i} ...')
```

### Comparing `cvmtrans-0.0.7/cvmtrans/data_process.sh` & `cvmtrans-0.0.8/cvmtrans/data_process.sh`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.7/cvmtrans/embl_parse.py` & `cvmtrans-0.0.8/cvmtrans/embl_parse.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.7/cvmtrans/embl_parse_test.py` & `cvmtrans-0.0.8/cvmtrans/embl_parse_test.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.7/cvmtrans/parse_bam.py` & `cvmtrans-0.0.8/cvmtrans/parse_bam.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.7/cvmtrans.egg-info/PKG-INFO` & `cvmtrans-0.0.8/cvmtrans.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.7
+Version: 0.0.8
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # cvmtrans
 
 ![PYPI](https://img.shields.io/pypi/v/cvmtrans)
-![Static Badge](https://img.shields.io/badge/OS-_Windows_%7C_Mac_%7C_Linux-steelblue)
+![Static Badge](https://img.shields.io/badge/OS-_Mac_%7C_Linux-steelblue)
 
 
 ## Installation
 
 pip3 install cvmtrans
```

### Comparing `cvmtrans-0.0.7/setup.py` & `cvmtrans-0.0.8/setup.py`

 * *Files identical despite different names*

