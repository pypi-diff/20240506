# Comparing `tmp/vcf2seq-0.6.0a0.tar.gz` & `tmp/vcf2seq-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.6.0a0.tar", last modified: Mon May  6 06:58:36 2024, max compression
+gzip compressed data, was "vcf2seq-0.6.1a0.tar", last modified: Mon May  6 08:56:19 2024, max compression
```

## Comparing `vcf2seq-0.6.0a0.tar` & `vcf2seq-0.6.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.0a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.0a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.6.0a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.0a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.6.0a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.0a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-06 06:57:18.000000 vcf2seq-0.6.0a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12110 2024-05-06 06:55:09.000000 vcf2seq-0.6.0a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 06:58:36.617589 vcf2seq-0.6.0a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 06:58:36.000000 vcf2seq-0.6.0a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.1a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.1a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.6.1a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.1a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.521192 vcf2seq-0.6.1a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.1a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.1a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      248 2024-05-06 08:37:16.000000 vcf2seq-0.6.1a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12874 2024-05-06 08:36:49.000000 vcf2seq-0.6.1a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 08:56:19.525192 vcf2seq-0.6.1a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2231 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 08:56:19.000000 vcf2seq-0.6.1a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.6.0a0/LICENCE.md` & `vcf2seq-0.6.1a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.0a0/PKG-INFO` & `vcf2seq-0.6.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.0a0
+Version: 0.6.1a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `vcf2seq-0.6.0a0/README.md` & `vcf2seq-0.6.1a0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.0a0/setup.py` & `vcf2seq-0.6.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.0a0/vcf2seq/ascii.py` & `vcf2seq-0.6.1a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.0a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.6.1a0/vcf2seq/vcf2seq.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,57 +29,67 @@
         chr_dict = pyfaidx.Fasta(args.genome) # if fai file doesn't exists, it will be automatically created
     except pyfaidx.FastaNotFoundError as err:
         sys.exit(f"FastaNotFoundError: {err}")
     except OSError as err:
         sys.exit(f"\n{COL.RED}WriteError: directory {os.path.dirname(args.genome)!r} may not be "
                   "writable.\nIf you can't change the rights, you can create a symlink and target "
                   f"it. For example:\n  ln -s {args.genome} $HOME\n{COL.END}")
-    vcf_ctrl(args, chr_dict)
+    vcf_ok, vcf_msg = input_ctrl(args, chr_dict)
+    if not vcf_ok:
+        sys.exit(f"{COL.RED}{vcf_msg}")
     results, warnings = compute(args, chr_dict)
     write(args, results, warnings)
 
 
-def vcf_ctrl(args, chr_dict):
-    with open(args.vcf.name) as fh:
+def input_ctrl(args, chr_dict):
+    with open(args.input.name) as fh:
         for row in fh:
             if row.startswith('#'):
                 continue
-            chr, pos, id, ref, alt, *rest = row.rstrip('\n').split('\t')
+            try:
+                chr, pos, id, ref, alt, *rest = row.rstrip('\n').split('\t')
+            except ValueError:
+                msg = ("ErrorVcfFormat: not enough columns for a vcf (expected at least 5).")
+                return False, msg
 
             ### Check some commonly issues
             if not pos.isdigit():
-                sys.exit(f"{COL.RED}ErrorVcfFormat: second column is the position. It must be a "
+                msg = (f"ErrorVcfFormat: second column is the position. It must be a "
                          f"digit (found: {pos!r}).\n"
-                          "A commonly issue is that headers are not commented by a '#' ")
+                          "A commonly issue is that the header is not commented by a '#' ")
+                return False, msg
             if chr not in chr_dict:
-                sys.exit(f"{COL.RED}ErrorChr: Chromosomes are not named in the same way in the "
+                msg (f"{COL.RED}ErrorChr: Chromosomes are not named in the same way in the "
                           "query and the genome file. Below the first chromosome found: \n"
                          f" your query: {chr}\n"
                          f" genome: {next(iter(chr_dict.keys()))}\n"
                          f"Please, correct your request (or modify the file '{args.genome}.fai').")
+                return False, msg
             break
+    return True, "ok"
 
 
 def compute(args, chr_dict):
     res_ref = []
     res_alt = []
     warnings = []
     num_row = 0
     cols_id = ascii.get_index(args.add_columns)    # columns chars are converted as index, ex: AA -> 27
-    for variant in args.vcf:
+    for variant in args.input:
         num_row += 1
         if not variant.rstrip('\n') or variant.startswith('#'):
             continue
         fields = variant.rstrip('\n').split('\t')
         chr, position, id, ref, alts = fields[:5]
 
         ### check if --add-columns is compatible with number of columns
         if args.add_columns and max(cols_id) > len(fields):
-            sys.exit(f"\n{COL.RED}Error: vcf file has {len(fields)} columns, but you asked for "
-                  f"{max(args.add_columns)}.{COL.END}\n")
+            warnings.append(f"Error: vcf file has {len(fields)} columns, but you asked for "
+                  f"{max(args.add_columns)} (line {num_row}).")
+            return None, warnings
 
         alts = alts.split(',')
         for alt in alts:
 
             header = f"{chr}_{position}_{ref}_{alt}"
 
             ### WARNING: event bigger than kmer size
@@ -87,17 +97,17 @@
                 warnings.append(f"Warning: large alteration ({chr}_{position}_{ref}_{alt}), truncated in output.")
 
 
             ### ERROR: REF base is not valid
             NUC = ["A", "T", "C", "G", args.blank]
             for nuc in (ref[0], alt[0]):
                 if nuc not in NUC:
-                    sys.exit(f"{COL.RED}Error: REF base {nuc!r} is not valid "
-                            f"(line {num_row}).\n       You might add the '--blank {nuc}' "
-                            "option or check your VCF file.")
+                    warnings.append(f"Warning: REF base {nuc!r} is not valid at line {num_row}, ignored.\n"
+                            f"        You might add the '--blank {nuc}' option or check your VCF file."
+                            )
 
             #####################################################################################
             #                Some explanations on variable naming                               #
             #                                                                                   #
             #  l = length                                                                       #
             #  ps = position start                                                              #
             #  pe = position end                                                                #
@@ -120,53 +130,59 @@
                 if len(alt)&1 and alt != args.blank: corr_alt += 1  # corr_alt + 1 if ALT length is unpair
             else:                                               # k is unpair
                 if not len(ref)&1: corr_ref += 1                    # corr_ref + 1 if REF length is pair
                 if not len(alt)&1: corr_alt += 1                    # corr_alt + 1 if ALT length is pair
                 if ref == args.blank: corr_ref += 1                 # missing value for REF
                 if alt == args.blank: corr_alt += 1                 # missing value for ALT
 
-            ## define REF kmer
-            l_ref2  = 0 if ref == args.blank else len(ref)
-            l_ref1  = (args.size - l_ref2) // 2
-            l_ref3  = l_ref1 + corr_ref
-            ps_ref2 = int(position)-1                               # -1 for pyfaidx
-            ps_ref1 = ps_ref2 - l_ref1
-            pe_ref3 = ps_ref2 + l_ref2 + l_ref3
-            ref_seq = chr_dict[chr][ps_ref1:pe_ref3]
-
-            ## define ALT kmer
-            l_alt2 = 0 if alt == args.blank else len(alt)
-            l_alt1 = (args.size - l_alt2) // 2
-            l_alt3 = (args.size - l_alt2) // 2 + corr_alt
-            ps_alt2 = ps_ref2 - (l_alt2 - l_ref2) // 2
-            ps_alt1 = ps_ref2 - l_alt1
-            ps_alt3 = ps_ref2 + l_ref2
-            pe_alt3 = ps_alt3 + l_alt3
-            seq_alt1 = chr_dict[chr][ps_alt1:ps_ref2]
-            alt = alt if alt != args.blank else ""
-            seq_alt3 = chr_dict[chr][ps_alt3:pe_alt3]
-            alt_seq = f"{seq_alt1}{alt}{seq_alt3}"
+            try:
+                ## define REF kmer
+                l_ref2  = 0 if ref == args.blank else len(ref)
+                l_ref1  = (args.size - l_ref2) // 2
+                l_ref3  = l_ref1 + corr_ref
+                ps_ref2 = int(position)-1                               # -1 for pyfaidx
+                ps_ref1 = ps_ref2 - l_ref1
+                pe_ref3 = ps_ref2 + l_ref2 + l_ref3
+                ref_seq = chr_dict[chr][ps_ref1:pe_ref3]
+
+                ## define ALT kmer
+                l_alt2 = 0 if alt == args.blank else len(alt)
+                l_alt1 = (args.size - l_alt2) // 2
+                l_alt3 = (args.size - l_alt2) // 2 + corr_alt
+                ps_alt2 = ps_ref2 - (l_alt2 - l_ref2) // 2
+                ps_alt1 = ps_ref2 - l_alt1
+                ps_alt3 = ps_ref2 + l_ref2
+                pe_alt3 = ps_alt3 + l_alt3
+                seq_alt1 = chr_dict[chr][ps_alt1:ps_ref2]
+                alt = alt if alt != args.blank else ""
+                seq_alt3 = chr_dict[chr][ps_alt3:pe_alt3]
+                alt_seq = f"{seq_alt1}{alt}{seq_alt3}"
+            except:
+                warnings.append(f"Warning: something went wrong at line {num_row}, ignored.")
+                break
 
             ### WARNING: REF bases must be the same as the calculated position
             seq_ref2 = chr_dict[chr][ps_ref2:ps_ref2+l_ref2]
             if l_ref2 and not ref == seq_ref2:
                 warnings.append("Warning: mismatch between REF and genome "
-                                f"at line {num_row} ({chr}:{ps_ref2+1}).\n"
-                                f"    - REF on the vcf file: {ref!r}\n"
-                                f"    - Found on the genome: '{seq_ref2}'\n"
-                                "    Please check if the given genome is appropriate.\n")
+                                f"at line {num_row} (chr{chr}:{ps_ref2+1}).\n"
+                                f"    - REF in the vcf file: {ref!r}\n"
+                                f"    - Found in the genome: '{seq_ref2}'\n"
+                                "    Please check if the given genome is appropriate.")
             col_sep = ' ' if args.output_format == 'fa' else '\t'
             col_txt =  col_sep.join([fields[num-1] for num in cols_id])
             if len(ref_seq) == args.size == len(alt_seq):
                 res_ref.append(f"{header}_ref{col_sep}{col_txt}\n{ref_seq}")
                 res_alt.append(f"{header}_alt{col_sep}{col_txt}\n{alt_seq}")
             elif len(alt_seq) > args.size:
-                warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence ({args.size} bp) at line {num_row}, ignored.")
+                warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence "
+                                f"({args.size} bp) at line {num_row}, ignored.")
             else:
-                warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored ({len(alt_seq)} != {args.size}).")
+                warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored"
+                                "f({len(alt_seq)} != {args.size}).")
 
     if args.type == 'alt':
         res = res_alt
     elif args.type == 'ref':
         res = res_ref
     else:
         res = list()
@@ -174,37 +190,37 @@
             res.append(res_ref[i])
             res.append(res_alt[i])
     return res, warnings
 
 
 
 def write(args, results, warnings):
-    ### RESULTS
+    ### OUTPUT RESULTS
     ext = args.output_format
     ## define output file
     if not args.output:
-        name, _ = os.path.splitext(os.path.basename(args.vcf.name))
+        name, _ = os.path.splitext(os.path.basename(args.input.name))
         args.output = f"{name}-vcf2seq.{ext}"
-    ## write results in file
-    with open(args.output, 'w') as fh:
-        if not results:
-            return
-        if ext == 'fa':
-            fh.write(">" + '\n>'.join([a for a in results]) + "\n")
-        else:
-            for row in results:
-                header, seq = row.split('\n')
-                fh.write(f"{seq}\t")
-                fh.write(f"{header}\n")
 
+    ## write results in file
+    if results:
+        with open(args.output, 'w') as fh:
+            if ext == 'fa':
+                fh.write(">" + '\n>'.join([a for a in results]) + "\n")
+            else:
+                for row in results:
+                    header, seq = row.split('\n')
+                    fh.write(f"{seq}\t")
+                    fh.write(f"{header}\n")
 
     ### WARNINGS
     if warnings:
-        print(COL.PURPLE)
-        print(*warnings, sep='\n')
+        for warning in warnings:
+            color = COL.RED if warning.startswith('Error') else COL.PURPLE
+            print(f"{color}{warning}\n")
         print(COL.END)
 
 
 class COL:
     PURPLE = '\033[95m'
     CYAN = '\033[96m'
     DARKCYAN = '\033[36m'
@@ -217,15 +233,15 @@
     END = '\033[0m'
 
 
 def usage():
     doc_sep = '=' * min(80, os.get_terminal_size(2)[0])
     parser = argparse.ArgumentParser(description= f'{doc_sep}{__doc__}{doc_sep}',
                                      formatter_class=argparse.RawDescriptionHelpFormatter,)
-    parser.add_argument("vcf",
+    parser.add_argument("input",
                         help="vcf file (mandatory)",
                         type=argparse.FileType('r'),
                        )
     parser.add_argument("-g", "--genome",
                         help="genome as fasta file (mandatory)",
                         metavar="genome",
                         required=True,
@@ -260,16 +276,16 @@
                         default='fa',
                         help=f"Output file format (default: fa)",
                         )
     parser.add_argument('-v', '--version',
                         action='version',
                         version=f"{parser.prog} v{info.VERSION}",
                        )
-    ### Go to "usage()" without arguments or stdin
-    if len(sys.argv) == 1 and sys.stdin.isatty():
+    ### Go to "usage()" without arguments
+    if len(sys.argv) == 1:
         parser.print_help()
         sys.exit()
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vcf2seq-0.6.0a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.6.1a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.0a0
+Version: 0.6.1a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

