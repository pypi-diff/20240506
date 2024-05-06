# Comparing `tmp/genmq-0.6.0.tar.gz` & `tmp/genmq-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genmq-0.6.0.tar", last modified: Sun Apr 28 13:59:57 2024, max compression
+gzip compressed data, was "genmq-0.6.2.tar", last modified: Mon May  6 06:16:47 2024, max compression
```

## Comparing `genmq-0.6.0.tar` & `genmq-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.891221 genmq-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 13:59:54.000000 genmq-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-28 13:59:57.891221 genmq-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-28 13:59:54.000000 genmq-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-28 13:59:54.000000 genmq-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:59:57.891221 genmq-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.887221 genmq-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:59:57.891221 genmq-0.6.0/src/genmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 13:59:57.000000 genmq-0.6.0/src/genmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-28 13:59:54.000000 genmq-0.6.0/src/genmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:16:47.924241 genmq-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 06:16:44.000000 genmq-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 06:16:47.924241 genmq-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-06 06:16:44.000000 genmq-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-06 06:16:44.000000 genmq-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:16:47.924241 genmq-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:16:47.924241 genmq-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:16:47.924241 genmq-0.6.2/src/genmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 06:16:47.000000 genmq-0.6.2/src/genmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 06:16:47.000000 genmq-0.6.2/src/genmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:16:47.000000 genmq-0.6.2/src/genmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 06:16:47.000000 genmq-0.6.2/src/genmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 06:16:47.000000 genmq-0.6.2/src/genmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-05-06 06:16:44.000000 genmq-0.6.2/src/genmq.py
```

### Comparing `genmq-0.6.0/LICENSE` & `genmq-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genmq-0.6.0/PKG-INFO` & `genmq-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genmq
-Version: 0.6.0
+Version: 0.6.2
 Summary: Moodle quiz generator
 Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://ccaprani.github.io/genmq/
 Project-URL: Documentation, https://ccaprani.github.io/genmq/
 Project-URL: Source, https://github.com/ccaprani/genmq/
 Project-URL: Tracker, https://github.com/ccaprani/genmq/issues/
```

### Comparing `genmq-0.6.0/README.md` & `genmq-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `genmq-0.6.0/pyproject.toml` & `genmq-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "genmq"
-version = "0.6.0"
+version = "0.6.2"
 description = "Moodle quiz generator"
 keywords = ["moodle", "quiz", "question bank"]
 authors = [{name = "Colin Caprani", email = "colin.caprani@monash.edu"}]
 license = {text = "GNU General Public License v3.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Education :: Computer Aided Instruction (CAI)",
```

### Comparing `genmq-0.6.0/src/genmq.egg-info/PKG-INFO` & `genmq-0.6.2/src/genmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genmq
-Version: 0.6.0
+Version: 0.6.2
 Summary: Moodle quiz generator
 Author-email: Colin Caprani <colin.caprani@monash.edu>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://ccaprani.github.io/genmq/
 Project-URL: Documentation, https://ccaprani.github.io/genmq/
 Project-URL: Source, https://github.com/ccaprani/genmq/
 Project-URL: Tracker, https://github.com/ccaprani/genmq/issues/
```

### Comparing `genmq-0.6.0/src/genmq.py` & `genmq-0.6.2/src/genmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.jinja_template = self.make_template(self.templatefile)
         df, keys = self.generic(self.csvfile)
 
         df_gq = df
         if self.compile_number is not None:
             df_gq = df.head(self.compile_number)
         elif self.compile_index is not None:
-            i = abs(self.compile_index)
+            i = abs(self.compile_index-1)  # Zero based indexing in dataframe
             # double brackets to extract row as DataFrame not Series
             df_gq = df.iloc[[i]]
 
         # Create the progress bar
         tqdm.pandas()
 
         # Apply function to each row of df
@@ -362,24 +362,29 @@
         """
         Writes the first 'number' of questions to a new XML file
         """
         root, q_list = self.read_xml_file()
 
         self.split_q_per_file(root, q_list, number_q, number_f)
 
-    def split_by_size(self, maxfilesize):
+    def split_by_size(self, maxfilesize, nfiles=None):
         root, q_list = self.read_xml_file()
 
         maxfilesize *= 2**20  # MB to bytes: 2^20 = 1 MB
         filesize = self.xmlfile.stat().st_size
-        n_files = math.ceil(filesize / maxfilesize)
+        max_n_files = math.ceil(filesize / maxfilesize)
+        if nfiles is not None and nfiles > 0:
+            n_files = min(max_n_files, nfiles)
+            print(f"{nfiles=}, {n_files=}, {max_n_files=}, {maxfilesize=}")
+        else:
+            n_files = max_n_files
         print(f"Writing {n_files} files")
 
         total_no_questions = len(q_list)
-        q_per_file = math.floor(total_no_questions / n_files)
+        q_per_file = math.floor(total_no_questions / max_n_files)
         print(f"Approx. no. of questions per file: {q_per_file}")
 
         self.split_q_per_file(root, q_list, q_per_file, n_files)
 
     def write_xml_file(self, tree, fname):
         base_xml = ET.ElementTree(tree)
         base_xml.write(fname, encoding="utf-8", xml_declaration=True)
@@ -494,16 +499,17 @@
         const=100,
         type=int,
     )
 
     splitmodeargs.add_argument(
         "-f",
         "--splitnofiles",
-        help="Split by putting -q questions each into this number of files (default is 1)",
+        help="Limit splitting to this number of files (default is 1)",
         nargs="?",
+        default=None,
         const=1,
         type=int,
     )
 
     mergemodeargs = parser.add_argument_group("Merge XML files mode required arguments")
     mergemodeargs.add_argument(
         "-m",
@@ -516,17 +522,18 @@
 
     if normalmode:
         gmq = GenMoodleQuiz(args)
         gmq.run()
     elif splitmode:
         xml_splitter = Splitter(args.splitxml)
         if args.splitqsperfile is not None:
-            xml_splitter.split_by_number(args.splitqsperfile, args.splitnofiles)
+            nfiles = 1 if args.splitnofiles is None else args.splitnofiles
+            xml_splitter.split_by_number(args.splitqsperfile, nfiles)
         else:
-            xml_splitter.split_by_size(args.maxfilesize)
+            xml_splitter.split_by_size(args.maxfilesize, args.splitnofiles)
     elif mergemode:
         xml_files = glob.glob("*.xml")
         gmq = GenMoodleQuiz(args)
         # if extension provided, strip it
         filename = args.mergexml.rsplit(".", 1)[0]
         gmq.merge_xml(filename, xml_files)
     else:
```

