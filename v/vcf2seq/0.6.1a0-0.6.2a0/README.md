# Comparing `tmp/vcf2seq-0.6.1a0.tar.gz` & `tmp/vcf2seq-0.6.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.6.1a0.tar", last modified: Mon May  6 08:56:19 2024, max compression
+gzip compressed data, was "vcf2seq-0.6.2a0.tar", last modified: Mon May  6 09:16:05 2024, max compression
```

## Comparing `vcf2seq-0.6.1a0.tar` & `vcf2seq-0.6.2a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.1a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.1a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.6.1a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.1a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.521192 vcf2seq-0.6.1a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.1a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.1a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-06 08:37:16.000000 vcf2seq-0.6.1a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12874 2024-05-06 08:36:49.000000 vcf2seq-0.6.1a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.2a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.2a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.2a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 09:16:05.545802 vcf2seq-0.6.2a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.2a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.2a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.2a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-06 09:14:13.000000 vcf2seq-0.6.2a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12874 2024-05-06 08:36:49.000000 vcf2seq-0.6.2a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.6.1a0/LICENCE.md` & `vcf2seq-0.6.2a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.1a0/PKG-INFO` & `vcf2seq-0.6.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.1a0
+Version: 0.6.2a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
-Author-email: benoit.guibert@inserm.fr
+Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
@@ -46,18 +46,20 @@
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
                         genome as fasta file (mandatory)
-  -s SIZE, --size SIZE  size of the output sequence (defalt: 31)
+  -s SIZE, --size SIZE  size of the output sequence (default: 31)
   -t {alt,ref,both}, --type {alt,ref,both}
                         alt, ref, or both output? (default: alt)
   -b BLANK, --blank BLANK
                         Missing nucleotide character, default is dot (.)
   -a ADD_COLUMNS [ADD_COLUMNS ...], --add-columns ADD_COLUMNS [ADD_COLUMNS ...]
                         Add one or more columns to header (ex: '-a 3 AA' will add columns 3 and 27). The first column is '1' (or 'A')
   -o OUTPUT, --output OUTPUT
-                        Output file (default: <input_file>-vcf2seq.fa)
+                        Output file (default: <input_file>-vcf2seq.fa/tsv)
+  -f {fa,tsv}, --output-format {fa,tsv}
+                        Output file format (default: fa)
   -v, --version         show program's version number and exit
 ```
```

### Comparing `vcf2seq-0.6.1a0/README.md` & `vcf2seq-0.6.2a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,18 +29,20 @@
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
                         genome as fasta file (mandatory)
-  -s SIZE, --size SIZE  size of the output sequence (defalt: 31)
+  -s SIZE, --size SIZE  size of the output sequence (default: 31)
   -t {alt,ref,both}, --type {alt,ref,both}
                         alt, ref, or both output? (default: alt)
   -b BLANK, --blank BLANK
                         Missing nucleotide character, default is dot (.)
   -a ADD_COLUMNS [ADD_COLUMNS ...], --add-columns ADD_COLUMNS [ADD_COLUMNS ...]
                         Add one or more columns to header (ex: '-a 3 AA' will add columns 3 and 27). The first column is '1' (or 'A')
   -o OUTPUT, --output OUTPUT
-                        Output file (default: <input_file>-vcf2seq.fa)
+                        Output file (default: <input_file>-vcf2seq.fa/tsv)
+  -f {fa,tsv}, --output-format {fa,tsv}
+                        Output file format (default: fa)
   -v, --version         show program's version number and exit
 ```
```

### Comparing `vcf2seq-0.6.1a0/setup.py` & `vcf2seq-0.6.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.1a0/vcf2seq/ascii.py` & `vcf2seq-0.6.2a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.1a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.6.2a0/vcf2seq/vcf2seq.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.1a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.6.2a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.1a0
+Version: 0.6.2a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
-Author-email: benoit.guibert@inserm.fr
+Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
@@ -46,18 +46,20 @@
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
                         genome as fasta file (mandatory)
-  -s SIZE, --size SIZE  size of the output sequence (defalt: 31)
+  -s SIZE, --size SIZE  size of the output sequence (default: 31)
   -t {alt,ref,both}, --type {alt,ref,both}
                         alt, ref, or both output? (default: alt)
   -b BLANK, --blank BLANK
                         Missing nucleotide character, default is dot (.)
   -a ADD_COLUMNS [ADD_COLUMNS ...], --add-columns ADD_COLUMNS [ADD_COLUMNS ...]
                         Add one or more columns to header (ex: '-a 3 AA' will add columns 3 and 27). The first column is '1' (or 'A')
   -o OUTPUT, --output OUTPUT
-                        Output file (default: <input_file>-vcf2seq.fa)
+                        Output file (default: <input_file>-vcf2seq.fa/tsv)
+  -f {fa,tsv}, --output-format {fa,tsv}
+                        Output file format (default: fa)
   -v, --version         show program's version number and exit
 ```
```

