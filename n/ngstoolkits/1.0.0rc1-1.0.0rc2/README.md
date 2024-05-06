# Comparing `tmp/ngstoolkits-1.0.0rc1.tar.gz` & `tmp/ngstoolkits-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-9t8w5zie/ngstoolkits-1.0.0rc1.tar", last modified: Mon Apr 29 06:59:22 2024, max compression
+gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-h06qxnah/ngstoolkits-1.0.0rc2.tar", last modified: Mon May  6 09:39:08 2024, max compression
```

## Comparing `ngstoolkits-1.0.0rc1.tar` & `ngstoolkits-1.0.0rc2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.383310 ngstoolkits-1.0.0rc1/
--rw-r--r--   0 liubo      (501) staff       (20)      594 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.coveragerc
--rw-r--r--   0 liubo      (501) staff       (20)      566 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)      530 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.readthedocs.yml
--rw-r--r--   0 liubo      (501) staff       (20)       80 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/AUTHORS.md
--rw-r--r--   0 liubo      (501) staff       (20)      115 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0 liubo      (501) staff       (20)    13529 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/LICENSE.txt
--rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-04-29 06:59:22.383063 ngstoolkits-1.0.0rc1/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     1323 2024-04-29 06:03:51.000000 ngstoolkits-1.0.0rc1/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.370253 ngstoolkits-1.0.0rc1/docs/
--rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/Makefile
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.371210 ngstoolkits-1.0.0rc1/docs/_static/
--rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/_static/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/authors.md
--rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/changelog.md
--rw-r--r--   0 liubo      (501) staff       (20)    10054 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/conf.py
--rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/contributing.md
--rw-r--r--   0 liubo      (501) staff       (20)      956 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/index.md
--rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/license.md
--rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/readme.md
--rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-29 06:45:11.000000 ngstoolkits-1.0.0rc1/docs/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)      354 2024-04-29 06:52:27.000000 ngstoolkits-1.0.0rc1/pyproject.toml
--rw-r--r--   0 liubo      (501) staff       (20)     1225 2024-04-29 06:59:22.385547 ngstoolkits-1.0.0rc1/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)      982 2024-04-29 06:21:59.000000 ngstoolkits-1.0.0rc1/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.353069 ngstoolkits-1.0.0rc1/src/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.374088 ngstoolkits-1.0.0rc1/src/ngstoolkits/
--rw-r--r--   0 liubo      (501) staff       (20)      373 2024-04-29 06:59:08.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)    10740 2024-04-29 06:17:19.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/ngs_class.py
--rw-r--r--   0 liubo      (501) staff       (20)      725 2024-04-29 06:45:25.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/sequence.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.381195 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)      671 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:53:14.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/not-zip-safe
--rw-r--r--   0 liubo      (501) staff       (20)       86 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)       12 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/top_level.txt
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.380163 ngstoolkits-1.0.0rc1/tests/
--rw-r--r--   0 liubo      (501) staff       (20)      279 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/tests/conftest.py
--rw-r--r--   0 liubo      (501) staff       (20)      738 2024-04-29 06:03:05.000000 ngstoolkits-1.0.0rc1/tests/test_class.py
--rw-r--r--   0 liubo      (501) staff       (20)     2861 2024-04-29 06:44:15.000000 ngstoolkits-1.0.0rc1/tox.ini
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.326117 ngstoolkits-1.0.0rc2/
+-rw-r--r--   0 liubo      (501) staff       (20)      594 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/.coveragerc
+-rw-r--r--   0 liubo      (501) staff       (20)      566 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)      530 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/.readthedocs.yml
+-rw-r--r--   0 liubo      (501) staff       (20)       80 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/AUTHORS.md
+-rw-r--r--   0 liubo      (501) staff       (20)       49 2024-04-29 07:00:11.000000 ngstoolkits-1.0.0rc2/CHANGELOG.md
+-rw-r--r--   0 liubo      (501) staff       (20)    13529 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/LICENSE.txt
+-rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-05-06 09:39:08.325922 ngstoolkits-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     1323 2024-04-29 06:03:51.000000 ngstoolkits-1.0.0rc2/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.309300 ngstoolkits-1.0.0rc2/docs/
+-rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/Makefile
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.310313 ngstoolkits-1.0.0rc2/docs/_static/
+-rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/_static/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/authors.md
+-rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/changelog.md
+-rw-r--r--   0 liubo      (501) staff       (20)    10054 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/conf.py
+-rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/contributing.md
+-rw-r--r--   0 liubo      (501) staff       (20)      956 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/index.md
+-rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/license.md
+-rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/docs/readme.md
+-rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-29 06:45:11.000000 ngstoolkits-1.0.0rc2/docs/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      353 2024-05-06 09:35:30.000000 ngstoolkits-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 liubo      (501) staff       (20)     1225 2024-05-06 09:39:08.327507 ngstoolkits-1.0.0rc2/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)      982 2024-04-29 06:21:59.000000 ngstoolkits-1.0.0rc2/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.286757 ngstoolkits-1.0.0rc2/src/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.313528 ngstoolkits-1.0.0rc2/src/ngstoolkits/
+-rw-r--r--   0 liubo      (501) staff       (20)        8 2024-05-06 09:38:20.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits/VERSION
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2024-05-06 09:38:58.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10835 2024-04-29 07:53:05.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits/ngs_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)      725 2024-04-29 06:45:25.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits/sequence.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.323906 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-05-06 09:39:08.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)      695 2024-05-06 09:39:08.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-05-06 09:39:08.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:53:14.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/not-zip-safe
+-rw-r--r--   0 liubo      (501) staff       (20)       86 2024-05-06 09:39:08.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       12 2024-05-06 09:39:08.000000 ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/top_level.txt
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-05-06 09:39:08.322859 ngstoolkits-1.0.0rc2/tests/
+-rw-r--r--   0 liubo      (501) staff       (20)      279 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc2/tests/conftest.py
+-rw-r--r--   0 liubo      (501) staff       (20)      738 2024-04-29 06:03:05.000000 ngstoolkits-1.0.0rc2/tests/test_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2861 2024-04-29 06:44:15.000000 ngstoolkits-1.0.0rc2/tox.ini
```

### Comparing `ngstoolkits-1.0.0rc1/.coveragerc` & `ngstoolkits-1.0.0rc2/.coveragerc`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/.gitignore` & `ngstoolkits-1.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/.readthedocs.yml` & `ngstoolkits-1.0.0rc2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/CONTRIBUTING.md` & `ngstoolkits-1.0.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/LICENSE.txt` & `ngstoolkits-1.0.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/PKG-INFO` & `ngstoolkits-1.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: ngstools
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `ngstoolkits-1.0.0rc1/README.md` & `ngstoolkits-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/docs/Makefile` & `ngstoolkits-1.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/docs/conf.py` & `ngstoolkits-1.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/docs/index.md` & `ngstoolkits-1.0.0rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/setup.cfg` & `ngstoolkits-1.0.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ngstoolkits
-versison = 1.0.0rc1
+versison = 1.0.0rc2
 description = Add a short description here!
 author = Ben-unbelieveable
 author_email = 614347533@qq.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
```

### Comparing `ngstoolkits-1.0.0rc1/setup.py` & `ngstoolkits-1.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/src/ngstoolkits/ngs_class.py` & `ngstoolkits-1.0.0rc2/src/ngstoolkits/ngs_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pysam
 from collections import namedtuple
+from functools import lru_cache
 
 class cpra():
     """
     descriptrion a mutation in cpra( eg: chr1, 100, A, T)
     and get some useful information with Bam or reference genome:
     """
 
@@ -35,23 +36,23 @@
         Init a mutation object,
         param chrom: eg: chr1
         param pos: eg: 100
         param ref: eg: A
         param alt: eg: T
         """
         self.chrom = CHROM
-        self.pos =  POS
+        self.pos =  int(POS)
         self.ref = REF
         self.alt = ALT
 
     @property
     def muttype(self):
-        if len(self.REF)>len(self.ALT):
+        if len(self.ref)>len(self.alt):
             return "DEL"
-        elif len(self.REF)<len(self.ALT):
+        elif len(self.ref)<len(self.alt):
             return "INS"
         else:
             return "SNV"
 
     @property
     def flank(self, length:int=10):
         '''获取变异的侧翼序列
@@ -89,117 +90,120 @@
         self.cover_readsID_list = []
         if self.muttype == "SNV":
             self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_snv_support_reads(self, bam_file, ref,coverflank)
         elif self.muttype == "INS":
             self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_ins_support_reads(self, bam_file, ref,coverflank)
         elif self.muttype == "DEL":
             self.support_reads,self.support_readsID_list,self.cover_readsID_list = self.get_del_support_reads(self, bam_file, ref,coverflank)
-
+    @property
+    @lru_cache
     def get_snv_support_reads(VcfMut, bam_file, ref,coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         Read = namedtuple('Read', ['read_name', 'pair', 'strand'])
         support_reads = []
         cover_reads = []
         start_reads = {}
-        EndSite = VcfMut.POS + len(VcfMut.REF)
-        for pileup_column in bam_file.pileup(region=str(VcfMut.CHROM) + ':' + str(VcfMut.POS) + '-' + str(VcfMut.POS),mapq=mapq , baseq = baseq,
+        EndSite = VcfMut.pos + len(VcfMut.ref)
+        for pileup_column in bam_file.pileup(region=str(VcfMut.chrom) + ':' + str(VcfMut.pos) + '-' + str(VcfMut.pos),mapq=mapq , baseq = baseq,
                                             stepper=stepper, fastaFile=ref, max_depth=200000, **{"truncate": True}):
             if pileup_column.nsegments > 0:
                 for pileup_read in pileup_column.pileups:
                     aln = pileup_read.alignment
                     read_name = aln.query_name
                     pair = 'pe1' if aln.is_read1 else 'pe2'
                     strand = '-' if aln.is_reverse else '+'
                     read = Read(read_name, pair, strand)
                     if pileup_read.is_del or pileup_read.is_refskip or (aln.flag > 1024) or (aln.mapping_quality < mapq) or \
                             aln.query_qualities[pileup_read.query_position] < baseq:
                         continue
                     start_reads[read] = [pileup_read.query_position, aln]
-        for pileup_column in bam_file.pileup(region=str(VcfMut.CHROM) + ':' + str(EndSite) + '-' + str(EndSite),
+        for pileup_column in bam_file.pileup(region=str(VcfMut.chrom) + ':' + str(EndSite) + '-' + str(EndSite),
                                             stepper=stepper, fastaFile=ref, max_depth=200000, **{"truncate": True}):
             if pileup_column.nsegments > 0:
                 for pileup_read in pileup_column.pileups:
                     aln = pileup_read.alignment
                     read_name = aln.query_name
                     pair = 'pe1' if aln.is_read1 else 'pe2'
                     strand = '-' if aln.is_reverse else '+'
                     read = Read(read_name, pair, strand)
                     if pileup_read.is_del or pileup_read.is_refskip:
                         continue
                     if read in start_reads:
                         start_query_position, start_aln = start_reads[read]
                         seq = start_aln.query_sequence[start_query_position:pileup_read.query_position]
                         cover_reads.append(aln)
-                        if seq.upper() == VcfMut.ALT.upper():
+                        if seq.upper() == VcfMut.alt.upper():
                             support_reads.append(aln)
         support_readIDs = []
         cover_readID_list = []
         for aln in cover_reads:
             cover_readID_list.append(aln.query_name)
         for aln in support_reads:
             support_readIDs.append(aln.query_name)
         return [support_reads,support_readIDs,cover_readID_list]
 
+    @lru_cache
     def get_ins_support_reads(VcfMut, bam_file, ref, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         support_reads = []
         cover_reads = []
         bam = {}
-        EndSite = VcfMut.POS + len(VcfMut.REF)
-        CoverStart = VcfMut.POS-coverflank
+        EndSite = VcfMut.pos + len(VcfMut.ref)
+        CoverStart = VcfMut.pos-coverflank
         CoverEnd = EndSite + coverflank
-        insLength=len(VcfMut.ALT)-len(VcfMut.REF)
-        for pileup_column in bam_file.pileup(region=str(VcfMut.CHROM) + ':' + str(VcfMut.POS) + '-' + str(VcfMut.POS), mapq=mapq, baseq=baseq, stepper=stepper, fastaFile=ref, max_depth=200000, **{"truncate": True}):
+        insLength=len(VcfMut.alt)-len(VcfMut.ref)
+        for pileup_column in bam_file.pileup(region=str(VcfMut.chrom) + ':' + str(VcfMut.pos) + '-' + str(VcfMut.pos), mapq=mapq, baseq=baseq, stepper=stepper, fastaFile=ref, max_depth=200000, **{"truncate": True}):
             if pileup_column.nsegments > 0:
                 for pileup_read in pileup_column.pileups:
                     aln = pileup_read.alignment
                     bam[aln.query_name] = pileup_read
                     if (CoverStart in aln.positions) and (CoverEnd in aln.positions):
                         cover_reads.append(aln)
                         if pileup_read.query_position and aln.cigarstring.find("I") > 0:
                             start = pileup_read.query_position-1
-                            altstop = pileup_read.query_position - 1 +len(VcfMut.ALT)
-                            refstop = pileup_read.query_position-1 + len(VcfMut.REF)
-                            if aln.query_sequence[start:altstop].upper() == VcfMut.ALT.upper() and \
-                                    aln.get_reference_sequence()[start:refstop].upper() == VcfMut.REF.upper():
+                            altstop = pileup_read.query_position - 1 +len(VcfMut.alt)
+                            refstop = pileup_read.query_position-1 + len(VcfMut.ref)
+                            if aln.query_sequence[start:altstop].upper() == VcfMut.alt.upper() and \
+                                    aln.get_reference_sequence()[start:refstop].upper() == VcfMut.ref.upper():
                                 support_reads.append(aln)
-                            elif aln.query_sequence[pileup_read.query_position-insLength:pileup_read.query_position -insLength+ len(VcfMut.ALT)].upper() == VcfMut.ALT.upper() and \
-                                aln.get_reference_sequence()[pileup_read.query_position-insLength:pileup_read.query_position - insLength + len(VcfMut.REF)].upper() == VcfMut.REF.upper():
+                            elif aln.query_sequence[pileup_read.query_position-insLength:pileup_read.query_position -insLength+ len(VcfMut.alt)].upper() == VcfMut.alt.upper() and \
+                                aln.get_reference_sequence()[pileup_read.query_position-insLength:pileup_read.query_position - insLength + len(VcfMut.ref)].upper() == VcfMut.ref.upper():
                                 support_reads.append(aln)
-                            elif aln.query_sequence[pileup_read.query_position:pileup_read.query_position + len(VcfMut.ALT)].upper() == VcfMut.ALT.upper() and \
-                                aln.get_reference_sequence()[pileup_read.query_position:pileup_read.query_position + len(VcfMut.REF)].upper() == VcfMut.REF.upper():
+                            elif aln.query_sequence[pileup_read.query_position:pileup_read.query_position + len(VcfMut.alt)].upper() == VcfMut.alt.upper() and \
+                                aln.get_reference_sequence()[pileup_read.query_position:pileup_read.query_position + len(VcfMut.ref)].upper() == VcfMut.ref.upper():
                                 support_reads.append(aln)
         support_readID_list = []
         cover_readID_list = []
         for aln in cover_reads:
             cover_readID_list.append(aln.query_name)
         for aln in support_reads:
             support_readID_list.append(aln.query_name)
         return [support_reads,support_readID_list,cover_readID_list]
 
+    @lru_cache
     def get_del_support_reads(VcfMut, bam_file, ref, coverflank=5, mapq=20, baseq=20, overlaps=True, stepper="all", orphans=True):
         support_reads = []
         cover_reads = []
         bam = {}
-        EndSite = VcfMut.POS + len(VcfMut.REF)
-        CoverStart = VcfMut.POS-coverflank
+        EndSite = VcfMut.pos + len(VcfMut.ref)
+        CoverStart = VcfMut.pos-coverflank
         CoverEnd = EndSite + coverflank
-        for pileup_column in bam_file.pileup(region=str(VcfMut.CHROM) + ':' + str(VcfMut.POS) + '-' + str(EndSite), mapq=mapq , baseq = baseq,
+        for pileup_column in bam_file.pileup(region=str(VcfMut.chrom) + ':' + str(VcfMut.pos) + '-' + str(EndSite), mapq=mapq , baseq = baseq,
                                             stepper=stepper, fastaFile=ref, max_depth=200000, **{"truncate": True}):
             if pileup_column.nsegments > 0:
                 for pileup_read in pileup_column.pileups:
                     aln = pileup_read.alignment
                     bam[aln.query_name]=pileup_read
                     if (CoverStart in aln.positions) and (CoverEnd in aln.positions):
                         cover_reads.append(aln)
                         if pileup_read.query_position_or_next and aln.cigarstring.find("D") > 0:
                             start = pileup_read.query_position_or_next - 1
-                            refstop = pileup_read.query_position_or_next + len(VcfMut.REF) - 1
-                            altstop = pileup_read.query_position_or_next +len(VcfMut.ALT) -1
-                            if aln.get_reference_sequence()[start:refstop].upper() == VcfMut.REF.upper() and aln.query_sequence[start:altstop].upper() == VcfMut.ALT.upper():
+                            refstop = pileup_read.query_position_or_next + len(VcfMut.ref) - 1
+                            altstop = pileup_read.query_position_or_next +len(VcfMut.alt) -1
+                            if aln.get_reference_sequence()[start:refstop].upper() == VcfMut.ref.upper() and aln.query_sequence[start:altstop].upper() == VcfMut.alt.upper():
                                 support_reads.append(aln)
-                            elif aln.get_reference_sequence()[start+1:refstop+1].upper() == VcfMut.REF.upper() and aln.query_sequence[start+1:altstop+1].upper() == VcfMut.ALT.upper():
+                            elif aln.get_reference_sequence()[start+1:refstop+1].upper() == VcfMut.ref.upper() and aln.query_sequence[start+1:altstop+1].upper() == VcfMut.alt.upper():
                                 support_reads.append(aln)
         support_readsID_list = []
         cover_readID_list = []
         for aln in cover_reads:
             cover_readID_list.append(aln.query_name)
         for aln in support_reads:
             support_readsID_list.append(aln.query_name)
```

### Comparing `ngstoolkits-1.0.0rc1/src/ngstoolkits/sequence.py` & `ngstoolkits-1.0.0rc2/src/ngstoolkits/sequence.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO` & `ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: ngstools
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt` & `ngstoolkits-1.0.0rc2/src/ngstoolkits.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/license.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
+src/ngstoolkits/VERSION
 src/ngstoolkits/__init__.py
 src/ngstoolkits/ngs_class.py
 src/ngstoolkits/sequence.py
 src/ngstoolkits.egg-info/PKG-INFO
 src/ngstoolkits.egg-info/SOURCES.txt
 src/ngstoolkits.egg-info/dependency_links.txt
 src/ngstoolkits.egg-info/not-zip-safe
```

### Comparing `ngstoolkits-1.0.0rc1/tests/test_class.py` & `ngstoolkits-1.0.0rc2/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `ngstoolkits-1.0.0rc1/tox.ini` & `ngstoolkits-1.0.0rc2/tox.ini`

 * *Files identical despite different names*

