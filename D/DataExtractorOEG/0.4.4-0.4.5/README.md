# Comparing `tmp/dataextractoroeg-0.4.4.tar.gz` & `tmp/dataextractoroeg-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.4.tar", last modified: Mon May  6 10:13:15 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.5.tar", last modified: Mon May  6 10:57:15 2024, max compression
```

## Comparing `dataextractoroeg-0.4.4.tar` & `dataextractoroeg-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.945494 dataextractoroeg-0.4.4/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.4/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.940333 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3078 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3078 2024-05-06 10:13:15.940333 dataextractoroeg-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.906793 dataextractoroeg-0.4.4/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.928941 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/name_doi_papers.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.4/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-02 11:30:33.000000 dataextractoroeg-0.4.4/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.4/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4351 2024-05-06 10:12:33.000000 dataextractoroeg-0.4.4/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-06 10:13:15.945494 dataextractoroeg-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-06 10:12:58.000000 dataextractoroeg-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.034284 dataextractoroeg-0.4.5/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.5/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.020921 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3078 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 10:57:14.000000 dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3078 2024-05-06 10:57:15.030195 dataextractoroeg-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.018060 dataextractoroeg-0.4.5/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-06 10:57:15.020921 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.5/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8448 2024-05-06 10:55:59.000000 dataextractoroeg-0.4.5/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.5/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4119 2024-05-06 10:43:20.000000 dataextractoroeg-0.4.5/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 10:57:15.034284 dataextractoroeg-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-06 10:56:57.000000 dataextractoroeg-0.4.5/setup.py
```

### Comparing `dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.5/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.4
+Version: 0.4.5
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.4/LICENSE.txt` & `dataextractoroeg-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.4/PKG-INFO` & `dataextractoroeg-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.4
+Version: 0.4.5
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.4/README.md` & `dataextractoroeg-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.5/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.4/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.5/doiExtractor/doiExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,8 +196,10 @@
     df.to_json(json_file, orient='records', indent=4)
 
 
 def find_file_by_name(path, name):
     for root, dirs, files in os.walk(path):
         if name in files:
             print(f"Found existing papers")
-            return os.path.join(root, name)
+            return os.path.join(root, name)
+        
+csv_to_json("doiExtractor/Outputs/results.csv", "doiExtractor/Outputs/results.json")
```

### Comparing `dataextractoroeg-0.4.4/doiExtractor/main.py` & `dataextractoroeg-0.4.5/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.4/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.5/doiExtractor/openAlex.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,27 +68,23 @@
         rows = list(reader)
 
     for row in rows:
         name = row["NAME"]
         doi = row["DOI"] 
 
         # If doi is None, add the doi founded in OpenAlex
-        if doi == "None":
+        if doi == "":
             page_url = get_primary_location_by_title(name, doi, include_doi=True)
-            if page_url:
+            if page_url[1] is not None:
                 row["DOI"] = page_url[1]
                 print(f"Searching in OpenAlex for DOI of {name}: {page_url[1]}")
         else:
             page_url = get_primary_location_by_doi(name, doi)
         
-        if page_url is not None:
-            if page_url[0].startswith("https://doi.org/"):
-                doi_from_url = page_url[0].replace("https://doi.org/", "")
-                row["DOI"] = doi_from_url
-                print("Adding missing DOI from primary location")
+        if page_url[0] is not None:
             row["PRIMARY_LOCATION"] = page_url[0]
             print(f"Searching in OpenAlex for {name} \nFounded link:{page_url[0]}")
         else:
             row["PRIMARY_LOCATION"] = "None"
             print(f"Searching in OpenAlex for {name}: No primary location")
         print("-----------------------------------------------------------------")
```

### Comparing `dataextractoroeg-0.4.4/setup.py` & `dataextractoroeg-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.4",
+    version="0.4.5",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

