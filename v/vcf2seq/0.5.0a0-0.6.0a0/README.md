# Comparing `tmp/vcf2seq-0.5.0a0.tar.gz` & `tmp/vcf2seq-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.5.0a0.tar", last modified: Fri May  3 14:57:48 2024, max compression
+gzip compressed data, was "vcf2seq-0.6.0a0.tar", last modified: Mon May  6 06:58:36 2024, max compression
```

## Comparing `vcf2seq-0.5.0a0.tar` & `vcf2seq-0.6.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.5.0a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.5.0a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.5.0a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.5.0a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.5.0a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.5.0a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-03 13:44:44.000000 vcf2seq-0.5.0a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    11561 2024-05-03 14:01:59.000000 vcf2seq-0.5.0a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-03 14:57:48.386566 vcf2seq-0.5.0a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-03 14:57:48.000000 vcf2seq-0.5.0a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.0a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.6.0a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.0a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.6.0a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.0a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-06 06:57:18.000000 vcf2seq-0.6.0a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12110 2024-05-06 06:55:09.000000 vcf2seq-0.6.0a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.5.0a0/LICENCE.md` & `vcf2seq-0.6.0a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.5.0a0/PKG-INFO` & `vcf2seq-0.6.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `vcf2seq-0.5.0a0/README.md` & `vcf2seq-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.5.0a0/setup.py` & `vcf2seq-0.6.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.5.0a0/vcf2seq/ascii.py` & `vcf2seq-0.6.0a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.5.0a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.6.0a0/vcf2seq/vcf2seq.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if args.add_columns and max(cols_id) > len(fields):
             sys.exit(f"\n{COL.RED}Error: vcf file has {len(fields)} columns, but you asked for "
                   f"{max(args.add_columns)}.{COL.END}\n")
 
         alts = alts.split(',')
         for alt in alts:
 
-            header = f">{chr}_{position}_{ref}_{alt}"
+            header = f"{chr}_{position}_{ref}_{alt}"
 
             ### WARNING: event bigger than kmer size
             if max(len(ref), len(alt)) > args.size :
                 warnings.append(f"Warning: large alteration ({chr}_{position}_{ref}_{alt}), truncated in output.")
 
 
             ### ERROR: REF base is not valid
@@ -150,19 +150,19 @@
             seq_ref2 = chr_dict[chr][ps_ref2:ps_ref2+l_ref2]
             if l_ref2 and not ref == seq_ref2:
                 warnings.append("Warning: mismatch between REF and genome "
                                 f"at line {num_row} ({chr}:{ps_ref2+1}).\n"
                                 f"    - REF on the vcf file: {ref!r}\n"
                                 f"    - Found on the genome: '{seq_ref2}'\n"
                                 "    Please check if the given genome is appropriate.\n")
-
-            col_txt =  ' '.join([fields[num-1] for num in cols_id])
+            col_sep = ' ' if args.output_format == 'fa' else '\t'
+            col_txt =  col_sep.join([fields[num-1] for num in cols_id])
             if len(ref_seq) == args.size == len(alt_seq):
-                res_ref.append(f"{header}_ref {col_txt}\n{ref_seq}")
-                res_alt.append(f"{header}_alt {col_txt}\n{alt_seq}")
+                res_ref.append(f"{header}_ref{col_sep}{col_txt}\n{ref_seq}")
+                res_alt.append(f"{header}_alt{col_sep}{col_txt}\n{alt_seq}")
             elif len(alt_seq) > args.size:
                 warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence ({args.size} bp) at line {num_row}, ignored.")
             else:
                 warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored ({len(alt_seq)} != {args.size}).")
 
     if args.type == 'alt':
         res = res_alt
@@ -175,23 +175,31 @@
             res.append(res_alt[i])
     return res, warnings
 
 
 
 def write(args, results, warnings):
     ### RESULTS
+    ext = args.output_format
     ## define output file
     if not args.output:
-        name, ext = os.path.splitext(os.path.basename(args.vcf.name))
-        args.output = f"{name}-vcf2seq.fa"
+        name, _ = os.path.splitext(os.path.basename(args.vcf.name))
+        args.output = f"{name}-vcf2seq.{ext}"
     ## write results in file
     with open(args.output, 'w') as fh:
         if not results:
             return
-        fh.write('\n'.join([a for a in results]) + "\n")
+        if ext == 'fa':
+            fh.write(">" + '\n>'.join([a for a in results]) + "\n")
+        else:
+            for row in results:
+                header, seq = row.split('\n')
+                fh.write(f"{seq}\t")
+                fh.write(f"{header}\n")
+
 
     ### WARNINGS
     if warnings:
         print(COL.PURPLE)
         print(*warnings, sep='\n')
         print(COL.END)
 
@@ -241,15 +249,20 @@
     parser.add_argument("-a", "--add-columns",
                         help="Add one or more columns to header (ex: '-a 3 AA' will add columns "
                              "3 and 27). The first column is '1' (or 'A')",
                         nargs= '+',
                         )
     parser.add_argument("-o", "--output",
                         type=str,
-                        help=f"Output file (default: <input_file>-{info.APPNAME}.fa)",
+                        help=f"Output file (default: <input_file>-{info.APPNAME}.fa/tsv)",
+                        )
+    parser.add_argument("-f", "--output-format",
+                        choices=['fa', 'tsv'],
+                        default='fa',
+                        help=f"Output file format (default: fa)",
                         )
     parser.add_argument('-v', '--version',
                         action='version',
                         version=f"{parser.prog} v{info.VERSION}",
                        )
     ### Go to "usage()" without arguments or stdin
     if len(sys.argv) == 1 and sys.stdin.isatty():
```

### Comparing `vcf2seq-0.5.0a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.6.0a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

