# Comparing `tmp/dataextractoroeg-0.4.5.tar.gz` & `tmp/dataextractoroeg-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.5.tar", last modified: Mon May  6 10:57:15 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.6.tar", last modified: Mon May  6 11:05:07 2024, max compression
```

## Comparing `dataextractoroeg-0.4.5.tar` & `dataextractoroeg-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.034284 dataextractoroeg-0.4.5/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.5/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.020921 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3078 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3078 2024-05-06 10:57:15.030195 dataextractoroeg-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.018060 dataextractoroeg-0.4.5/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.020921 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/name_doi_papers.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.5/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8448 2024-05-06 10:55:59.000000 dataextractoroeg-0.4.5/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.5/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4119 2024-05-06 10:43:20.000000 dataextractoroeg-0.4.5/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-06 10:57:15.034284 dataextractoroeg-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-06 10:56:57.000000 dataextractoroeg-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:05:07.377722 dataextractoroeg-0.4.6/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.6/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-06 11:05:07.366873 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3078 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 11:05:07.000000 dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3078 2024-05-06 11:05:07.366873 dataextractoroeg-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:05:07.362124 dataextractoroeg-0.4.6/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:05:07.366873 dataextractoroeg-0.4.6/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.6/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.6/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.6/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8448 2024-05-06 10:55:59.000000 dataextractoroeg-0.4.6/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2475 2024-05-06 11:04:34.000000 dataextractoroeg-0.4.6/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4119 2024-05-06 10:43:20.000000 dataextractoroeg-0.4.6/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:05:07.378722 dataextractoroeg-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-06 11:04:59.000000 dataextractoroeg-0.4.6/setup.py
```

### Comparing `dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.6/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.5
+Version: 0.4.6
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.5/LICENSE.txt` & `dataextractoroeg-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/PKG-INFO` & `dataextractoroeg-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.5
+Version: 0.4.6
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.5/README.md` & `dataextractoroeg-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.6/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.6/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.6/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/doiExtractor/main.py` & `dataextractoroeg-0.4.6/doiExtractor/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,23 @@
 
         # ExistingPapers
         papers = find_file_by_name(os.getcwd(),"name_doi_papers.csv")
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
-        # Delete contents of the files if already created
-        if os.path.exists(csv_filename):
-            open(csv_filename, 'w').close()
-        if os.path.exists(txt_filename):
-            open(txt_filename, 'w').close()
-        if os.path.exists(json_filename):
-            open(json_filename, 'w').close()
+        # Delete files if they exist
+        for filename in [csv_filename, txt_filename, json_filename]:
+            if os.path.exists(filename):
+                os.remove(filename)
+
+        # Create empty files
+        open(csv_filename, 'a').close()
+        open(txt_filename, 'a').close()
+        open(json_filename, 'a').close()
 
         # Extract dois from url
         search_papers(url, url_docs, csv_filename)
 
         # Merge them with the existing from the papers
         merge_csv(csv_filename, papers)
```

### Comparing `dataextractoroeg-0.4.5/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.6/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.5/setup.py` & `dataextractoroeg-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.5",
+    version="0.4.6",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

