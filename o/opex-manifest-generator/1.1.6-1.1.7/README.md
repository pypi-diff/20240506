# Comparing `tmp/opex_manifest_generator-1.1.6.tar.gz` & `tmp/opex_manifest_generator-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.6.tar", last modified: Sat May  4 20:41:59 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.7.tar", last modified: Mon May  6 06:55:04 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.6.tar` & `opex_manifest_generator-1.1.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.872850 opex_manifest_generator-1.1.6/
--rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.6/.gitignore
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.6/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-05-04 20:41:59.860877 opex_manifest_generator-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    21573 2024-04-21 18:27:56.000000 opex_manifest_generator-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.417107 opex_manifest_generator-1.1.6/assets/
--rw-rw-rw-   0        0        0     8271 2024-04-12 14:39:11.000000 opex_manifest_generator-1.1.6/assets/Column Headers.png
--rw-rw-rw-   0        0        0    27359 2024-04-12 14:49:33.000000 opex_manifest_generator-1.1.6/assets/FullName Column.png
--rw-rw-rw-   0        0        0    16064 2024-04-12 14:57:04.000000 opex_manifest_generator-1.1.6/assets/Hash Headers.png
--rw-rw-rw-   0        0        0     4920 2024-04-12 14:58:52.000000 opex_manifest_generator-1.1.6/assets/Identifiers Headers.png
--rw-rw-rw-   0        0        0     2602 2024-04-12 15:01:06.000000 opex_manifest_generator-1.1.6/assets/XML Headers.png
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.482435 opex_manifest_generator-1.1.6/opex_manifest_generator/
--rw-rw-rw-   0        0        0      476 2024-04-21 18:41:39.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6046 2024-04-21 18:36:34.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/hash.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.694088 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/
--rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/DublinCore Template.xml
--rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/EAD Template.xml
--rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/GDPR Template.xml
--rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/MODS Template.xml
--rw-rw-rw-   0        0        0    28824 2024-05-04 20:39:09.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/opex_manifest.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.742864 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/
--rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/Opex.xml
--rw-rw-rw-   0        0        0    24938 2024-04-12 14:50:52.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.849778 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/
--rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/dctemplate.xlsx
--rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
--rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
--rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/modstemplate.xlsx
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.856500 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1221 2024-05-04 20:41:59.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2024-05-04 20:40:54.000000 opex_manifest_generator-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 20:41:59.874874 opex_manifest_generator-1.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.617000 opex_manifest_generator-1.1.7/
+-rw-rw-rw-   0        0        0      124 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.7/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-05-06 06:55:04.583000 opex_manifest_generator-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    21573 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:03.402000 opex_manifest_generator-1.1.7/assets/
+-rw-rw-rw-   0        0        0     8271 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Column Headers.png
+-rw-rw-rw-   0        0        0    27359 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/FullName Column.png
+-rw-rw-rw-   0        0        0    16064 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Hash Headers.png
+-rw-rw-rw-   0        0        0     4920 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Identifiers Headers.png
+-rw-rw-rw-   0        0        0     2602 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/XML Headers.png
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:03.688000 opex_manifest_generator-1.1.7/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      476 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6485 2024-05-06 06:50:52.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0     1025 2024-05-06 06:38:56.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/hash.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.095000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/
+-rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/DublinCore Template.xml
+-rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/EAD Template.xml
+-rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/GDPR Template.xml
+-rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/MODS Template.xml
+-rw-rw-rw-   0        0        0    30563 2024-05-06 06:50:43.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0      313 2024-04-07 11:10:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/pstats_test.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.201000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/
+-rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/Opex.xml
+-rw-rw-rw-   0        0        0    24938 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.505000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/
+-rw-rw-rw-   0        0        0    22794 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/dctemplate.xlsx
+-rw-rw-rw-   0        0        0    19299 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
+-rw-rw-rw-   0        0        0    18662 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
+-rw-rw-rw-   0        0        0    19509 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/modstemplate.xlsx
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.557000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1260 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-05-06 06:54:04.000000 opex_manifest_generator-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:55:04.611000 opex_manifest_generator-1.1.7/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.6/LICENSE.md` & `opex_manifest_generator-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/PKG-INFO` & `opex_manifest_generator-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.6
+Version: 1.1.7
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.6/README.md` & `opex_manifest_generator-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/assets/Column Headers.png` & `opex_manifest_generator-1.1.7/assets/Column Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/assets/FullName Column.png` & `opex_manifest_generator-1.1.7/assets/FullName Column.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/assets/Hash Headers.png` & `opex_manifest_generator-1.1.7/assets/Hash Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/assets/Identifiers Headers.png` & `opex_manifest_generator-1.1.7/assets/Identifiers Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/assets/XML Headers.png` & `opex_manifest_generator-1.1.7/assets/XML Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.7/opex_manifest_generator/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,77 +8,80 @@
 import argparse
 import os
 import time
 from opex_manifest_generator.opex_manifest import OpexManifestGenerator
 import importlib.metadata
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="OPEX Manifest Generator for Preservica Uploads")
-    parser.add_argument('root',default=os.getcwd())
-    parser.add_argument("-c","--autoclass",required=False,choices=['catalog','c','accession','a','both','b','generic','g','catalog-generic','cg',"accession-generic","ag","both-generic","bg"],type=str.lower)
-    parser.add_argument("-p","--prefix",required=False, nargs='+')
-    parser.add_argument("-fx","--fixity",required=False,const="SHA-1",default=None, nargs='?', choices=['NONE','SHA-1','MD5','SHA-256','SHA-512'],type=str.upper)
-    parser.add_argument("-rme","--remove-empty",required=False,action='store_true',default=False)
-    parser.add_argument("-o","--output",required=False,nargs=1)
-    parser.add_argument("-clr","--clear-opex",required=False,action='store_true',default=False)
-    parser.add_argument("-s","--start-ref",required=False,nargs='?',default=1)
-    parser.add_argument("-m","--metadata",required=False,const='e',default='none',nargs='?',choices=['none','n','exact','e','flat','f'],type=str.lower)
-    parser.add_argument("-dmd", "--disable-meta-dir",required=False,action='store_false')
-    parser.add_argument("-ex","--export",required=False,action='store_true',default=False)
-    parser.add_argument("-i","--input",required=False)
-    parser.add_argument("-rm","--remove",required=False,action="store_true",default=False)
-    parser.add_argument("-z","--zip", required=False,action='store_true')
-    parser.add_argument("-fmt", "--output-format",required=False,default="xlsx", choices=['xlsx','csv'])
-    parser.add_argument("-v", "--version",action='version',version='%(prog)s {version}'.format(version=importlib.metadata.version("opex_manifest_generator")))
-    parser.add_argument("--hidden",required=False,action='store_true',default=False)
+    parser = argparse.ArgumentParser(description = "OPEX Manifest Generator for Preservica Uploads")
+    parser.add_argument('root', default = os.getcwd())
+    parser.add_argument("-c", "--autoclass", required = False, choices = ['catalog', 'c', 'accession', 'a', 'both', 'b', 'generic', 'g', 'catalog-generic', 'cg', "accession-generic", "ag", "both-generic", "bg"], type = str.lower)
+    parser.add_argument("-p", "--prefix", required = False, nargs = '+')
+    parser.add_argument("-fx", "--fixity", required = False, const = "SHA-1", default = None, nargs = '?', choices = ['NONE', 'SHA-1', 'MD5', 'SHA-256', 'SHA-512'], type = str.upper)
+    parser.add_argument("-rme", "--remove-empty", required = False, action = 'store_true', default = False)
+    parser.add_argument("-o", "--output", required = False, nargs = 1)
+    parser.add_argument("-clr", "--clear-opex", required = False, action = 'store_true', default = False)
+    parser.add_argument("-s", "--start-ref", required = False, nargs = '?', default = 1)
+    parser.add_argument("-m", "--metadata", required = False, const = 'e', default = 'none', nargs = '?', choices = ['none', 'n', 'exact', 'e', 'flat', 'f'], type = str.lower)
+    parser.add_argument("-dmd", "--disable-meta-dir", required = False, action = 'store_false')
+    parser.add_argument("-ex", "--export", required = False, action = 'store_true', default = False)
+    parser.add_argument("-i", "--input", required = False)
+    parser.add_argument("-rm", "--remove", required = False, action = "store_true", default = False)
+    parser.add_argument("-z", "--zip", required = False, action = 'store_true')
+    parser.add_argument("-fmt", "--output-format", required = False, default = "xlsx", choices = ['xlsx', 'csv'])
+    parser.add_argument("-v", "--version", action = 'version', version = '%(prog)s {version}'.format(version = importlib.metadata.version("opex_manifest_generator")))
+    parser.add_argument("--hidden", required = False, action = 'store_true', default = False)
+    parser.add_argument("--print-xmls", required = False, action = "store_true", default = False)
     args = parser.parse_args()
     return args
 
 def run_cli():
-    args = parse_args()
-    os.chdir(args.root)
-    
+    args = parse_args()    
     print(f"Running Opex Generation on: {args.root}")
     if not args.output:
         args.output = os.path.abspath(args.root)
         print(f'Output path defaulting to root directory: {args.output}')
     else:
         args.output = os.path.abspath(args.output[0])
         print(f'Output path set to: {args.output}')    
     if args.input and args.autoclass:
         print(f'Both Input and Auto-Class options have been selected, please use only one...')
         time.sleep(5); raise SystemExit()
-    if not args.metadata in {'none','n'} and not args.input:
+    if not args.metadata in {'none', 'n'} and not args.input:
         print(f'Warning: Metadata Flag has been given without Input. Metadata won\'t be generated.')
         time.sleep(5)
+    if args.print_xmls:
+        OpexManifestGenerator.print_descriptive_xmls()
     if args.autoclass:
         pass
         # if not args.prefix:
         #     print('A prefix must be set when using Auto-Classification, stopping operation')
         #     time.sleep(3); raise SystemExit()
     acc_prefix = None
     if args.prefix:
-        if args.autoclass in {"both","b","both-generic","bg"}:
+        if args.autoclass in {"both", "b", "both-generic", "bg"}:
             if len(args.prefix) < 2 or len(args.prefix) > 2:
                 print('"Both" option is selected, please pass only two prefixes: [-p CATALOG_PREFIX ACCESSION_PREFIX]');
                 time.sleep(3); raise SystemExit
-            for n,a in enumerate(args.prefix):
-                if n == 0: args.prefix = str(a)
-                elif n == 1: acc_prefix = str(a)
+            for n, a in enumerate(args.prefix):
+                if n == 0:
+                    args.prefix = str(a)
+                elif n == 1:
+                    acc_prefix = str(a)
             print(f"Prefixes are set as: \t Catalog: {args.prefix} \t Acc: {acc_prefix}")
-        elif args.autoclass in {"accession","a","accession-generic","ag"}:
+        elif args.autoclass in {"accession", "a", "accession-generic", "ag"}:
             for a in args.prefix:
                 acc_prefix = str(a)
             print('Prefix is set as: ' + acc_prefix)                        
-        elif args.autoclass in {"catalog","c","catalog-generic","cg"}:
+        elif args.autoclass in {"catalog", "c", "catalog-generic", "cg"}:
             acc_prefix = None
             for a in args.prefix: 
                 args.prefix = str(a)
             print('Prefix is set as: ' + args.prefix)
-        elif args.autoclass in {"generic","g"}:
+        elif args.autoclass in {"generic", "g"}:
             pass
         else:
             print('''An invalid option has been selected, please select a valid option: 
                   {c, catalog
                    a, accession
                    b, both
                    g, generic
@@ -90,25 +93,26 @@
     if args.fixity:
         print(f'Fixity is activated, using {args.fixity} algorithm')
     if args.remove:
         i = "y"
         # i = input(inspect.cleandoc("""You have enabled the remove functionality.
         #                         This action will remove files listed for removal, it is irreversible.
         #                         Please type Y to confirm, otherwise program will close: """))
-        if not i.lower() == "y": print("Closing program..."); time.sleep(3); raise SystemExit()
+        if not i.lower() == "y":
+            print("Closing program..."); time.sleep(3); raise SystemExit()
     time.sleep(3)
-    OpexManifestGenerator(root=args.root,
-                          output_path=args.output,
-                          autoclass_flag=args.autoclass,
-                          prefix=args.prefix,
-                          acc_prefix=acc_prefix,
-                          empty_flag=args.remove_empty,
-                          remove_flag=args.remove,
-                          clear_opex_flag=args.clear_opex,
-                          algorithm = args.fixity,
-                          startref=args.start_ref,
-                          export_flag=args.export,
-                          meta_dir_flag=args.disable_meta_dir,
-                          metadata_flag = args.metadata,
-                          zip_flag = args.zip,
-                          input=args.input,
-                          output_format=args.output_format).main()
+    OpexManifestGenerator(root = args.root, 
+                          output_path = args.output, 
+                          autoclass_flag = args.autoclass, 
+                          prefix = args.prefix, 
+                          acc_prefix = acc_prefix, 
+                          empty_flag = args.remove_empty, 
+                          remove_flag = args.remove, 
+                          clear_opex_flag = args.clear_opex, 
+                          algorithm = args.fixity, 
+                          startref = args.start_ref, 
+                          export_flag = args.export, 
+                          meta_dir_flag = args.disable_meta_dir, 
+                          metadata_flag = args.metadata, 
+                          zip_flag = args.zip, 
+                          input = args.input, 
+                          output_format = args.output_format).main()
```

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.7/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.7/opex_manifest_generator/hash.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 import hashlib
 
 class HashGenerator():
     def __init__(self,algorithm="SHA-1"):
         self.algorithm = algorithm
         self.buffer = 4096
 
-    def hash_generator(self,file_path):
-        if self.algorithm == "SHA-1": hash = hashlib.sha1()
-        elif self.algorithm == "MD5": hash = hashlib.md5()
-        elif self.algorithm == "SHA-256": hash = hashlib.sha256()
-        elif self.algorithm == "SHA-512": hash = hashlib.sha512()
-        else: hash = hashlib.sha1()
-        print(f'Generating Fixity using {self.algorithm} for: {file_path}')#,end="\r") 
-        with open(file_path,"rb") as f:
+    def hash_generator(self,file_path: str):
+        if self.algorithm == "SHA-1":
+            hash = hashlib.sha1()
+        elif self.algorithm == "MD5":
+            hash = hashlib.md5()
+        elif self.algorithm == "SHA-256":
+            hash = hashlib.sha256()
+        elif self.algorithm == "SHA-512":
+            hash = hashlib.sha512()
+        else:
+            hash = hashlib.sha1()
+        print(f'Generating Fixity using {self.algorithm} for: {file_path}')
+        with open(file_path, "rb") as f:
             while True:
                 buff = f.read(self.buffer)
                 if not buff:
                     break
                 hash.update(buff)
             f.close()
         return hash.hexdigest().upper()
```

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/DublinCore Template.xml` & `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/DublinCore Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/EAD Template.xml` & `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/EAD Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/MODS Template.xml` & `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/MODS Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.7/opex_manifest_generator/opex_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 from opex_manifest_generator.hash import HashGenerator
 from opex_manifest_generator.common import *
 import stat
 import shutil
 
 class OpexManifestGenerator():
     def __init__(self,
-                 root,
-                 output_path=os.getcwd(),
-                 meta_dir_flag=True,
-                 metadata_dir=os.path.join(os.path.dirname(os.path.realpath(__file__)), "metadata"),
-                 metadata_flag='none',
-                 autoclass_flag=False,
-                 prefix=None,
-                 acc_prefix=None,
-                 startref=1,
-                 algorithm=None,
-                 empty_flag=False,
-                 remove_flag=False,
-                 clear_opex_flag=False,
-                 export_flag=False,
-                 input=False,
-                 zip_flag=False,
-                 hidden_flag=False,
-                 output_format="xlsx"):
+                 root: str,
+                 output_path: os.path = os.getcwd(),
+                 meta_dir_flag: bool = True,
+                 metadata_dir: bool = os.path.join(os.path.dirname(os.path.realpath(__file__)), "metadata"),
+                 metadata_flag: str = 'none',
+                 autoclass_flag: str = None,
+                 prefix: str = None,
+                 acc_prefix: str = None,
+                 startref: int = 1,
+                 algorithm: str = None,
+                 empty_flag: bool = False,
+                 remove_flag: bool = False,
+                 clear_opex_flag: bool = False,
+                 export_flag: bool = False,
+                 input: str = None,
+                 zip_flag: bool = False,
+                 hidden_flag: bool = False,
+                 output_format: str = "xlsx",
+                 print_xmls_flag: bool = False):
         
         self.root = os.path.abspath(root)
         self.opexns = "http://www.openpreservationexchange.org/opex/v1.2"        
         self.list_path = []
         self.list_fixity = []
         self.start_time = datetime.now()
         self.algorithm = algorithm
@@ -65,48 +66,55 @@
         self.sourceid_flag = False
         self.hash_from_spread = False        
         self.hidden_flag = hidden_flag
         self.zip_flag = zip_flag
         self.output_format = output_format
         self.metadata_flag = metadata_flag
         self.metadata_dir = metadata_dir
+        self.print_xmls_flag = print_xmls_flag
         
     def print_running_time(self):
         print(f'Running time: {datetime.now() - self.start_time}')
         time.sleep(1)
     
     def index_df_lookup(self, path: str):
         idx = self.df['FullName'].index[self.df['FullName'] == path]
         return idx
 
-    def meta_df_lookup(self, idx):
+    def meta_df_lookup(self, idx: pd.Index):
         try:
             if idx.empty:
                 title = None
                 description = None
                 security = None
             else:
                     if self.title_flag:
                         title = self.df['Title'].loc[idx].item()
-                        if str(title).lower() in {"nan","nat"}: title = None
-                    else: title = None
-                    if self.description_flag: 
+                        if str(title).lower() in {"nan","nat"}:
+                            title = None
+                    else:
+                        title = None
+                    if self.description_flag:
                         description = self.df['Description'].loc[idx].item()
-                        if str(description).lower() in {"nan","nat"}: description = None
-                    else: description = None
-                    if self.security_flag: 
+                        if str(description).lower() in {"nan","nat"}:
+                            description = None
+                    else:
+                        description = None
+                    if self.security_flag:
                         security = self.df['Security'].loc[idx].item()
-                        if str(security).lower() in {"nan","nat"}: security = None
-                    else: security = None
+                        if str(security).lower() in {"nan","nat"}:
+                            security = None
+                    else:
+                        security = None
             return title,description,security
         except Exception as e:
             print('Error Looking up XIP Metadata')
             print(e)
     
-    def remove_df_lookup(self, path: str, idx):
+    def remove_df_lookup(self, path: str, idx: pd.Index):
         try:
             if idx.empty:
                 return False
             else:
                 remove = self.df['Removals'].loc[idx].item()
                 if str(remove).lower() in {"nan","nat"}:
                     return False
@@ -120,15 +128,15 @@
                     return True
                 else:
                     return False
         except Exception as e:
             print('Error looking up Removals')
             print(e)
                 
-    def ignore_df_lookup(self, idx):
+    def ignore_df_lookup(self, idx: pd.Index):
         try:
             if idx.empty:
                 return False
             else:
                 ignore = self.df['Ignore'].loc[idx].item()
             if str(ignore).lower() in {"nan","nat"}:
                 return False
@@ -136,30 +144,30 @@
                 return True
             elif str(ignore).lower() in {"false", "0.0"}:
                 return False
         except Exception as e:
             print('Error looking up Removals')
             print(e)
 
-    def sourceid_df_lookup(self, xml_element, idx):
+    def sourceid_df_lookup(self, xml_element: ET.SubElement, idx: pd.Index):
         try:
             if idx.empty:
                 pass
             else:
                 sourceid = self.df['SourceID'].loc[idx].item()
                 if str(sourceid) in {"nan","nat"}:
                     pass
                 else:
                     source_xml = ET.SubElement(xml_element,f"{{{self.opexns}}}SourceID")
                     source_xml.text = str(sourceid)
         except Exception as e:
             print('Error looking up SourceID')
             print(e)
 
-    def hash_df_lookup(self, file_path, xml_fixities, idx):
+    def hash_df_lookup(self, file_path: str, xml_fixities: ET.SubElement, idx: pd.Index):
         try:
             if idx.empty:
                 pass
             else:
                 if "Hash" in self.column_headers and "Algorithm" in self.column_headers:
                     self.fixity = ET.SubElement(xml_fixities,f"{{{self.opexns}}}Fixity")        
                     self.hash = self.df["Hash"].loc[idx].item()
@@ -167,15 +175,15 @@
                     self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
                     self.fixity.set("type", self.algorithm)
                     self.fixity.set("value",self.hash)
         except Exception as e:
             print('Error looking up Removals')
             print(e)
 
-    def ident_df_lookup(self, idx, key_override = None):
+    def ident_df_lookup(self, idx: pd.Index, key_override: str = None):
         try:
             if idx.empty:
                 ident = "ERROR"
                 self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
                 if key_override is None:
                     key_name = "code"
                 else:
@@ -191,33 +199,35 @@
                         elif key_override is None:
                             if 'Archive_Reference' in header:
                                 key_name = "code"
                             elif 'Accession_Reference' in header:
                                 key_name = "accref"
                             elif 'Identifier' in header:
                                 key_name = "code"
-                        else: 
+                        else:
                             key_name = key_override
-                    else: ident = None
-                    if str(ident).lower() in {"nan","nat"} or not ident: pass
                     else:
-                        self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
-                        self.identifier.set("type",key_name)
+                        ident = None
+                    if str(ident).lower() in {"nan", "nat"} or not ident:
+                        pass
+                    else:
+                        self.identifier = ET.SubElement(self.identifiers, f"{{{self.opexns}}}Identifier") 
+                        self.identifier.set("type", key_name)
                         self.identifier.text = str(ident)
         except Exception as e:
             print('Error looking up Identifiers')
             print(e)            
     
-    def check_opex(self, opex_path):
+    def check_opex(self, opex_path: str):
         if os.path.exists(win_256_check(opex_path)):
             return False
         else:
             return True
 
-    def write_opex(self, path, opexxml):
+    def write_opex(self, path: str, opexxml: ET.Element):
         opex_path = str(win_256_check(path)) + ".opex"
         opex = ET.indent(opexxml, "  ")
         opex = ET.tostring(opexxml, pretty_print=True, xml_declaration=True, encoding="UTF-8", standalone=True)
         with open(f'{opex_path}', 'w', encoding="UTF-8") as writer:
             writer.write(opex.decode('UTF-8'))
             print('Saved Opex File to: ' + opex_path)
         return opex_path
@@ -226,15 +236,15 @@
         if self.autoclass_flag:
             if self.autoclass_flag in {"catalog", "c", "catalog-generic", "cg"}:
                 ac = ClassificationGenerator(self.root, output_path = self.output_path, prefix = self.prefix, start_ref = self.startref, empty_flag = self.empty_flag, accession_flag = False)
             elif self.autoclass_flag in {"accession", "a", "accession-generic", "ag", "both", "b", "both-generic", "bg"}:
                 ac = ClassificationGenerator(self.root, output_path = self.output_path, prefix = self.prefix, accprefix = self.acc_prefix, start_ref = self.startref, empty_flag = self.empty_flag, accession_flag="File")
             self.df = ac.init_dataframe()
             if self.autoclass_flag in {"accession", "a", "accesion-generic", "ag"}:
-                self.df = self.df.drop('Archive_Reference',axis=1)
+                self.df = self.df.drop('Archive_Reference', axis=1)
             self.column_headers = self.df.columns.values.tolist()
             if self.export_flag:
                 output_path = define_output_file(self.output_path, self.root, meta_dir_flag = self.meta_dir_flag, output_format = self.output_format)                
                 if self.output_format == "xlsx":
                     export_xl(self.df, output_path)
                 elif self.output_format == "csv":
                     export_csv(self.df, output_path)
@@ -247,17 +257,17 @@
             self.set_input_flags()
         else:
             self.df = None
             self.column_headers = None
                 
     def clear_opex(self):
         walk = list(os.walk(self.root))
-        for dir,_,files in walk[::-1]:
+        for dir, _, files in walk[::-1]:
             for file in files:
-                file_path = win_256_check(os.path.join(dir,file))   
+                file_path = win_256_check(os.path.join(dir, file))   
                 if str(file_path).endswith('.opex'):
                     os.remove(file_path)
                     print(f'Cleared Opex: {file_path}')
     
     def set_input_flags(self):
         if 'Title' in self.column_headers:
             self.title_flag = True
@@ -272,297 +282,319 @@
         if 'Hash' in self.column_headers and 'Algorithm' in self.column_headers:
             self.hash_from_spread = True
             print("Hash detected in Spreadsheet; taking hashes from spreadsheet")
             time.sleep(3)
 
     def print_descriptive_xmls(self):
         for file in os.scandir(self.metadata_dir):
-            path = os.path.join(self.metadata_dir,file.name)
+            path = os.path.join(self.metadata_dir, file.name)
             print(path)
             xml_file = ET.parse(path)
             root_element = ET.QName(xml_file.find('.'))
             root_element_ln = root_element.localname
             for elem in xml_file.findall(".//"):
                 elem_path = xml_file.getelementpath(elem)
                 elem = ET.QName(elem)
-                elem_lnpath = elem_path.replace(f"{{{elem.namespace}}}",root_element_ln + ":")
+                elem_lnpath = elem_path.replace(f"{{{elem.namespace}}}", root_element_ln + ":")
                 print(elem_lnpath)
 
     def init_generate_descriptive_metadata(self):
         self.xml_files = []
         for file in os.scandir(self.metadata_dir):
             if file.name.endswith('xml'):
                 """
                 Generates info on the elements of the XML Files placed in the Metadata directory.
                 Composed as a list of dictionaries.
                 """
-                path = os.path.join(self.metadata_dir,file)
+                path = os.path.join(self.metadata_dir, file)
                 xml_file = ET.parse(path)
                 root_element = ET.QName(xml_file.find('.'))
                 root_element_ln = root_element.localname
                 root_element_ns = root_element.namespace
                 elements_list = []
                 for elem in xml_file.findall('.//'):
                     elem_path = xml_file.getelementpath(elem)
                     elem = ET.QName(elem)
                     elem_ln = elem.localname
                     elem_ns = elem.namespace
-                    elem_lnpath = elem_path.replace(f"{{{elem_ns}}}",root_element_ln + ":")
-                    elements_list.append({"Name":root_element_ln + ":" + elem_ln,"Namespace":elem_ns,"Path":elem_lnpath})
+                    elem_lnpath = elem_path.replace(f"{{{elem_ns}}}", root_element_ln + ":")
+                    elements_list.append({"Name": root_element_ln + ":" + elem_ln, "Namespace": elem_ns, "Path": elem_lnpath})
 
                 """
                 Compares the column headers in the Spreadsheet against the headers. Filters out non-matching data.
                 """
                 list_xml = []
                 for elem_dict in elements_list:
                     if elem_dict.get('Name') in self.column_headers or elem_dict.get('Path') in self.column_headers:
-                        list_xml.append({"Name":elem_dict.get('Name'),"Namespace":elem_dict.get('Namespace'),"Path":elem_dict.get('Path')})
+                        list_xml.append({"Name": elem_dict.get('Name'), "Namespace": elem_dict.get('Namespace'), "Path": elem_dict.get('Path')})
             if len(list_xml) > 0:
-                self.xml_files.append({'data':list_xml, 'localname':root_element_ln, 'xmlfile': path})
+                self.xml_files.append({'data': list_xml, 'localname': root_element_ln, 'xmlfile': path})
 
-    def generate_descriptive_metadata(self,xml_desc, idx):
+    def generate_descriptive_metadata(self, xml_desc: ET.Element, idx: int):
         for xml_file in self.xml_files:
             list_xml = xml_file.get('data')
             localname = xml_file.get('localname')
             """
             Composes the data into an xml file.
             """
             if len(list_xml):
                 if not idx.empty:
                     xml_new = ET.parse(xml_file.get('xmlfile'))
                     for elem_dict in list_xml:
                         name = elem_dict.get('Name')
                         path = elem_dict.get('Path')
                         ns = elem_dict.get('Namespace')
                         try:
-                            if self.metadata_flag in {'e','exact'}:
-                                val = self.df.loc[idx,path].values[0]
-                            elif self.metadata_flag in {'f','flat'}:
-                                val = self.df.loc[idx,name].values[0]
-                            if pd.isnull(val): continue
+                            if self.metadata_flag in {'e', 'exact'}:
+                                val = self.df.loc[idx, path].values[0]
+                            elif self.metadata_flag in {'f', 'flat'}:
+                                val = self.df.loc[idx, name].values[0]
+                            if pd.isnull(val):
+                                continue
                             else:
                                 if is_datetime64_any_dtype(val):
                                     val = pd.to_datetime(val)
-                                    val = datetime.strftime(val,"%Y-%m-%dT%H-%M-%S.00Z")
+                                    val = datetime.strftime(val, "%Y-%m-%dT%H-%M-%S.00Z")
                         except KeyError as e:
                             print('Key Error: please ensure column header\'s are an exact match...')
                             print(f'Missing Column: {e}')
                             print('Alternatively use flat mode...')
                             time.sleep(3)
                             raise SystemError()
                         except IndexError as e:
                             print("""Index Error; it is likely you have removed or added a file/folder to the directory \
                                 after generating the spreadsheet. An opex will still be generated but with no xml metadata. \
                                 To ensure metadata match up please regenerate the spreadsheet...""")
                             print(f'Error: {e}')
                             time.sleep(3)
                             break
-                        if str(val).lower() in {"nan","nat"}:
+                        if str(val).lower() in {"nan", "nat"}:
                             continue
                         if self.metadata_flag in {'e','exact'}:
                             n = path.replace(localname + ":", f"{{{ns}}}")
                             elem = xml_new.find(f'/{n}')
-                        elif self.metadata_flag in {'f','flat'}:
+                        elif self.metadata_flag in {'f', 'flat'}:
                             n = name.split(':')[-1]
                             elem = xml_new.find(f'//{{{ns}}}{n}')
                         elem.text = str(val)    
                     xml_desc.append(xml_new.find('.'))
-                else: pass
-            else: pass
+                else:
+                    pass
+            else:
+                pass
 
-    def generate_opex_properties(self, xmlroot, idx, title=None,description=None,security=None):
-        self.properties = ET.SubElement(xmlroot,f"{{{self.opexns}}}Properties")
-        self.identifiers = ET.SubElement(self.properties,f"{{{self.opexns}}}Identifiers")
+    def generate_opex_properties(self, xmlroot: ET.Element, idx: int, 
+                                 title: str = None, description: str = None, security: str = None):
+        self.properties = ET.SubElement(xmlroot, f"{{{self.opexns}}}Properties")
+        self.identifiers = ET.SubElement(self.properties, f"{{{self.opexns}}}Identifiers")
         if title:
-            self.titlexml = ET.SubElement(self.properties,f"{{{self.opexns}}}Title")
+            self.titlexml = ET.SubElement(self.properties, f"{{{self.opexns}}}Title")
             self.titlexml.text = str(title)
         if description:
-            self.descriptionxml = ET.SubElement(self.properties,f"{{{self.opexns}}}Description")
+            self.descriptionxml = ET.SubElement(self.properties, f"{{{self.opexns}}}Description")
             self.descriptionxml.text = str(description)      
         if security:
-            self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
+            self.securityxml = ET.SubElement(self.properties, f"{{{self.opexns}}}SecurityDescriptor")
             self.securityxml.text = str(security)
-        if self.autoclass_flag in {"generic","g"}:
+        if self.autoclass_flag in {"generic", "g"}:
             self.properties.remove(self.identifiers)
-        elif self.autoclass_flag or self.input:
+        elif self.autoclass_flag not in {"generic", "g"} or self.input:
             self.ident_df_lookup(idx)
         if self.identifiers is None:
             self.properties.remove(self.identifiers)
         if self.properties is None:
             xmlroot.remove(self.properties)
 
-    def genererate_opex_fixity(self, file_path):
+    def genererate_opex_fixity(self, file_path: str):
         self.fixity = ET.SubElement(self.fixities, f"{{{self.opexns}}}Fixity")        
-        self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
+        self.hash = HashGenerator(algorithm = self.algorithm).hash_generator(file_path)
         self.fixity.set("type", self.algorithm)
         self.fixity.set("value", self.hash)
         self.OMG.list_fixity.append([self.algorithm, self.hash, file_path])
         self.OMG.list_path.append(file_path)
 
     def main(self):
+        if self.print_xmls_flag:
+            self.print_descriptive_xmls()
+            input("Press Key to Close")
+            raise SystemExit()
         print(f"Start time: {self.start_time}")        
         if self.clear_opex_flag:
             self.clear_opex()
             if self.autoclass_flag or self.algorithm or self.input:
                 pass
-            else: 
+            else:
                 self.print_running_time()
                 print('Cleared OPEXES. No additional arguments passed, so ending program.'); time.sleep(3)
                 raise SystemExit()
         if self.empty_flag:
-            ClassificationGenerator(self.root,self.output_path,meta_dir_flag=self.meta_dir_flag).remove_empty_directories()
-        if not self.autoclass_flag in {"g","generic"}:
+            ClassificationGenerator(self.root, self.output_path, meta_dir_flag = self.meta_dir_flag).remove_empty_directories()
+        if not self.autoclass_flag in {"g", "generic"}:
             self.init_df()
         self.count = 1
-        if not self.metadata_flag in {'none','n'}: self.init_generate_descriptive_metadata()
-        OpexDir(self,self.root).generate_opex_dirs(self.root)
+        if not self.metadata_flag in {'none', 'n'}:
+            self.init_generate_descriptive_metadata()
+        OpexDir(self, self.root).generate_opex_dirs(self.root)
         if self.algorithm:
-            output_path = define_output_file(self.output_path,self.root,self.meta_dir_flag,output_suffix="_Fixities",output_format="txt")
-            export_list_txt(self.list_fixity,output_path)
+            output_path = define_output_file(self.output_path, self.root, self.meta_dir_flag, output_suffix = "_Fixities", output_format = "txt")
+            export_list_txt(self.list_fixity, output_path)
         self.print_running_time()
 
 class OpexDir(OpexManifestGenerator):
-    def __init__(self,OMG,folder_path,title=None,description=None,security=None):
+    def __init__(self, OMG: OpexManifestGenerator, folder_path: str, title: str = None, description: str = None, security: str = None):
         self.OMG = OMG
         self.root = self.OMG.root
         self.opexns = self.OMG.opexns
         if folder_path.startswith(u'\\\\?\\'):
-            self.folder_path = folder_path.replace(u'\\\\?\\',"")
+            self.folder_path = folder_path.replace(u'\\\\?\\', "")
         else:
             self.folder_path = folder_path
-        if self.OMG.autoclass_flag is None:
-            pass
-        elif self.OMG.input or not self.OMG.autoclass_flag in {"g","generic","none"} or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
+        if self.OMG.input or self.OMG.autoclass_flag in {"c", "catalog", "a", "accession", "b", "both", "cg", "catalog-generic", "ag", "accession-generic", "bg", "both-generic"} \
+             or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag \
+             or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
                 self.index = self.OMG.index_df_lookup(self.folder_path)
+        elif self.OMG.autoclass_flag is None or self.OMG.autoclass_flag in {"g", "generic"}:
+            self.index = None
         if self.OMG.ignore_flag or self.OMG.remove_flag:
             if self.OMG.ignore_flag:
                 self.ignore = self.OMG.ignore_df_lookup(self.index)
                 if self.ignore:
                     return
             if self.OMG.remove_flag:
                 self.removal = self.OMG.remove_df_lookup(self.folder_path, self.index)
                 if self.removal:
                     return        
         else:
             self.ignore = False
             self.removal = False
 
-        self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
-        self.transfer = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}Transfer")
-        self.manifest = ET.SubElement(self.transfer,f"{{{self.opexns}}}Manifest")
-        self.folders = ET.SubElement(self.manifest,f"{{{self.opexns}}}Folders")
-        self.files = ET.SubElement(self.manifest,f"{{{self.opexns}}}Files")
+        self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata", nsmap={"opex":self.opexns})
+        self.transfer = ET.SubElement(self.xmlroot, f"{{{self.opexns}}}Transfer")
+        self.manifest = ET.SubElement(self.transfer, f"{{{self.opexns}}}Manifest")
+        self.folders = ET.SubElement(self.manifest, f"{{{self.opexns}}}Folders")
+        self.files = ET.SubElement(self.manifest, f"{{{self.opexns}}}Files")
 
         if self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
-            self.title,self.description,self.security = self.OMG.meta_df_lookup(self.folder_path,self.index) 
-        elif self.OMG.autoclass_flag in {"generic","g","catalog-generic","cg","accession-generic","ag","both-generic","bg"}:
+            self.title, self.description, self.security = self.OMG.meta_df_lookup(self.index) 
+        elif self.OMG.autoclass_flag in {"generic", "g", "catalog-generic", "cg", "accession-generic", "ag", "both-generic", "bg"}:
             self.title = os.path.basename(self.folder_path)
             self.description = os.path.basename(self.folder_path)
             self.security = "open"
         else:
             self.title = title
             self.description = description
             self.security = security
         if self.OMG.sourceid_flag:
-            self.OMG.sourceid_df_lookup(self.transfer,self.folder_path, self.index)
+            self.OMG.sourceid_df_lookup(self.transfer, self.folder_path, self.index)
         if self.OMG.autoclass_flag or self.OMG.input:
-            self.OMG.generate_opex_properties(self.xmlroot,self.folder_path,self.index,title=self.title,description=self.description,security=self.security)
-            if not self.OMG.metadata_flag in {'none','n'}:
+            self.OMG.generate_opex_properties(self.xmlroot, self.index, 
+                                              title = self.title,
+                                              description = self.description,
+                                              security = self.security)
+            if not self.OMG.metadata_flag in {'none', 'n'}:
                 self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
-                self.OMG.generate_descriptive_metadata(self.xmlroot,self.folder_path, idx = self.index)
+                self.OMG.generate_descriptive_metadata(self.xmlroot, self.folder_path, idx = self.index)
 
-    def filter_directories(self,directory):    #Sorts the list Alphabetically and Ignores: 1. Hidden Directories starting with '.', 2. '.opex' files, 3. Folders titled 'meta', 4. Script file 5. Output file. 
+    def filter_directories(self, directory: str):
         if not self.OMG.hidden_flag:
-            list_directories = sorted([os.path.join(directory,f.name) for f in os.scandir(directory)
+            list_directories = sorted([os.path.join(directory, f.name) for f in os.scandir(directory)
                                        if not f.name.startswith('.')
-                                       and not bool(os.stat(os.path.join(directory,f.name)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN)
+                                       and not bool(os.stat(os.path.join(directory, f.name)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN)
                                        and f.name != 'meta'
-                                       and f.name != os.path.basename(__file__)],
-                                       key=str.casefold)
+                                       and f.name != os.path.basename(__file__)]
+                                       , key=str.casefold)
         else:
-            list_directories = sorted([os.path.join(directory,f.name) for f in os.scandir(directory) \
+            list_directories = sorted([os.path.join(directory, f.name) for f in os.scandir(directory) \
                                        if f.name != 'meta' \
-                                       and f.name != os.path.basename(__file__)],key=str.casefold)
+                                       and f.name != os.path.basename(__file__)], key=str.casefold)
         return list_directories
         
-    def generate_opex_dirs(self,path):
-        self = OpexDir(self.OMG,path)
-        opex_path = os.path.join(os.path.abspath(self.folder_path),os.path.basename(self.folder_path))
+    def generate_opex_dirs(self, path: str):
+        self = OpexDir(self.OMG, path)
+        opex_path = os.path.join(os.path.abspath(self.folder_path), os.path.basename(self.folder_path))
         if self.OMG.check_opex(opex_path):
             for f_path in self.filter_directories(path):
                 if f_path.endswith('.opex'):
                     pass
                 elif os.path.isdir(f_path):
                     if not self.ignore:
-                        self.folder = ET.SubElement(self.folders,f"{{{self.opexns}}}Folder")
+                        self.folder = ET.SubElement(self.folders, f"{{{self.opexns}}}Folder")
                         self.folder.text = str(os.path.basename(f_path))
                     self.generate_opex_dirs(f_path)
                 else:
-                    OpexFile(self.OMG,f_path,self.OMG.algorithm)
+                    OpexFile(self.OMG, f_path, self.OMG.algorithm)
             if not self.ignore:
                 for f_path in self.filter_directories(path):
                     if os.path.isfile(f_path):
-                        file = ET.SubElement(self.files,f"{{{self.opexns}}}File")
-                        if f_path.endswith('.opex'): 
-                            file.set("type","metadata")
+                        file = ET.SubElement(self.files, f"{{{self.opexns}}}File")
+                        if f_path.endswith('.opex'):
+                            file.set("type", "metadata")
                         else:
-                            file.set("type","content")
-                            file.set("size",str(os.path.getsize(f_path)))
+                            file.set("type", "content")
+                            file.set("size", str(os.path.getsize(f_path)))
                         file.text = str(os.path.basename(f_path))
-                self.OMG.write_opex(opex_path,self.xmlroot)
+                self.OMG.write_opex(opex_path, self.xmlroot)
         else:
-            print(f"Opex exists: {opex_path}: Avoiding override")
+            print(f"Avoiding override, Opex exists at: {opex_path}")
 
 class OpexFile(OpexManifestGenerator):
-    def __init__(self,OMG,file_path,algorithm = None,title=None,description=None,security=None):
+    def __init__(self, OMG: OpexManifestGenerator, file_path: str, algorithm: str = None, title: str = None, description: str = None, security: str = None):
         self.OMG = OMG
         self.opexns = self.OMG.opexns  
         if file_path.startswith(u'\\\\?\\'):
-            self.file_path = file_path.replace(u'\\\\?\\',"")
+            self.file_path = file_path.replace(u'\\\\?\\', "")
         else:
             self.file_path = file_path
         if self.OMG.check_opex(self.file_path + ".opex"):
-            if self.OMG.input or self.OMG.autoclass_flag or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
-                self.index = self.OMG.index_df_lookup(self.file_path)
-            if self.OMG.ignore_flag: 
-                self.ignore = self.OMG.ignore_df_lookup(self.file_path,self.index)
+            if self.OMG.input or self.OMG.autoclass_flag in {"c","catalog","a","accession","b","both","cg","catalog-generic","ag","accession-generic","bg","both-generic"} \
+                or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag \
+                or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
+                    self.index = self.OMG.index_df_lookup(self.file_path)
+            elif self.OMG.autoclass_flag is None or self.OMG.autoclass_flag in {"g","generic"}:
+                self.index = None
+            if self.OMG.ignore_flag:
+                self.ignore = self.OMG.ignore_df_lookup(self.file_path, self.index)
                 if self.ignore:
                     return
             if self.OMG.remove_flag:
-                removal = self.OMG.remove_df_lookup(self.file_path,self.index)
+                removal = self.OMG.remove_df_lookup(self.file_path, self.index)
                 if removal:
                     return                
             else:
                 self.ignore = False
             self.algorithm = algorithm
             if self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
-                self.title,self.description,self.security = self.OMG.meta_df_lookup(self.file_path,self.index) 
-            elif self.OMG.autoclass_flag in {"generic","g","catalog-generic","cg","accession-generic","ag","both-generic","bg"}:
+                self.title, self.description, self.security = self.OMG.meta_df_lookup(self.index) 
+            elif self.OMG.autoclass_flag in {"generic", "g", "catalog-generic", "cg", "accession-generic", "ag", "both-generic", "bg"}:
                 self.title = os.path.splitext(os.path.basename(self.file_path))[0]
                 self.description = os.path.splitext(os.path.basename(self.file_path))[0]
                 self.security = "open"
             else:
                 self.title = title
                 self.description = description
                 self.security = security
             if self.OMG.algorithm or self.OMG.autoclass_flag or self.OMG.input:
-                self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
-                self.transfer = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}Transfer")
+                self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata", nsmap={"opex":self.opexns})
+                self.transfer = ET.SubElement(self.xmlroot, f"{{{self.opexns}}}Transfer")
                 if self.OMG.sourceid_flag:
-                    self.OMG.sourceid_df_lookup(self.transfer,self.file_path)
+                    self.OMG.sourceid_df_lookup(self.transfer, self.file_path)
                 if self.OMG.algorithm:
-                    self.fixities = ET.SubElement(self.transfer,f"{{{self.opexns}}}Fixities")
+                    self.fixities = ET.SubElement(self.transfer, f"{{{self.opexns}}}Fixities")
                     if self.OMG.hash_from_spread:
-                        self.OMG.hash_df_lookup(self.file_path,self.fixities,self.index)  
+                        self.OMG.hash_df_lookup(self.file_path, self.fixities, self.index)  
                     else:
                         self.genererate_opex_fixity(self.file_path)
                 if self.transfer is None:
                     self.xmlroot.remove(self.transfer)
                 if self.OMG.autoclass_flag or self.OMG.input:
-                    self.OMG.generate_opex_properties(self.xmlroot,self.file_path,self.index,title=self.title,description=self.description,security=self.security)
+                    self.OMG.generate_opex_properties(self.xmlroot, self.index,
+                                                      title = self.title,
+                                                      description = self.description,
+                                                      security = self.security)
                     if not self.OMG.metadata_flag in {'none','n'}:
-                        self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
+                        self.xml_descmeta = ET.SubElement(self.xmlroot, f"{{{self.opexns}}}DescriptiveMetadata")
                         self.OMG.generate_descriptive_metadata(self.xml_descmeta, self.file_path, self.index)
-                opex_path = self.OMG.write_opex(self.file_path,self.xmlroot)
+                opex_path = self.OMG.write_opex(self.file_path, self.xmlroot)
                 if self.OMG.zip_flag:
-                    zip_opex(self.file_path,opex_path)
-        else: print(f"Opex exists for: {self.file_path}: Avoiding override")
+                    zip_opex(self.file_path, opex_path)
+        else:
+            print(f"Opex exists for: {self.file_path}: Avoiding override")
```

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx` & `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/dctemplate.xlsx` & `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/dctemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/eadtemplate.xlsx` & `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/eadtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx` & `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/modstemplate.xlsx` & `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/modstemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.6
+Version: 1.1.7
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 assets/Identifiers Headers.png
 assets/XML Headers.png
 opex_manifest_generator/__init__.py
 opex_manifest_generator/cli.py
 opex_manifest_generator/common.py
 opex_manifest_generator/hash.py
 opex_manifest_generator/opex_manifest.py
+opex_manifest_generator/pstats_test.py
 opex_manifest_generator/test_cli.py
 opex_manifest_generator.egg-info/PKG-INFO
 opex_manifest_generator.egg-info/SOURCES.txt
 opex_manifest_generator.egg-info/dependency_links.txt
 opex_manifest_generator.egg-info/entry_points.txt
 opex_manifest_generator.egg-info/requires.txt
 opex_manifest_generator.egg-info/top_level.txt
```

### Comparing `opex_manifest_generator-1.1.6/pyproject.toml` & `opex_manifest_generator-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 746f 6f6c 732d 7363 6d22 5d0d 0a62 7569  tools-scm"]..bui
 00000040: 6c64 2d62 6163 6b65 6e64 203d 2022 7365  ld-backend = "se
 00000050: 7475 7074 6f6f 6c73 2e62 7569 6c64 5f6d  tuptools.build_m
 00000060: 6574 6122 0d0a 0d0a 5b70 726f 6a65 6374  eta"....[project
 00000070: 5d0d 0a6e 616d 6520 3d20 226f 7065 785f  ]..name = "opex_
 00000080: 6d61 6e69 6665 7374 5f67 656e 6572 6174  manifest_generat
 00000090: 6f72 220d 0a76 6572 7369 6f6e 203d 2022  or"..version = "
-000000a0: 312e 312e 3622 0d0a 6175 7468 6f72 7320  1.1.6"..authors 
+000000a0: 312e 312e 3722 0d0a 6175 7468 6f72 7320  1.1.7"..authors 
 000000b0: 3d20 5b0d 0a20 2020 207b 6e61 6d65 3d22  = [..    {name="
 000000c0: 4368 7269 7374 6f70 6865 7220 5072 696e  Christopher Prin
 000000d0: 6365 222c 2065 6d61 696c 3d22 632e 706a  ce", email="c.pj
 000000e0: 2e70 7269 6e63 6540 676d 6169 6c2e 636f  .prince@gmail.co
 000000f0: 6d22 7d0d 0a20 2020 205d 0d0a 6465 7363  m"}..    ]..desc
 00000100: 7269 7074 696f 6e20 3d20 224f 7065 7820  ription = "Opex 
 00000110: 4d61 6e69 6665 7374 2047 656e 6572 6174  Manifest Generat
```

