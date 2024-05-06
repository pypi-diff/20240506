# Comparing `tmp/dataextractoroeg-0.4.3.tar.gz` & `tmp/dataextractoroeg-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.3.tar", last modified: Fri May  3 08:03:57 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.4.tar", last modified: Mon May  6 10:13:15 2024, max compression
```

## Comparing `dataextractoroeg-0.4.3.tar` & `dataextractoroeg-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 08:03:57.598410 dataextractoroeg-0.4.3/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.3/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-03 08:03:57.592864 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3078 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 08:03:57.000000 dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3078 2024-05-03 08:03:57.594427 dataextractoroeg-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 08:03:57.506065 dataextractoroeg-0.4.3/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-03 08:03:57.537204 dataextractoroeg-0.4.3/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.3/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.3/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-05-03 08:03:57.586017 dataextractoroeg-0.4.3/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0        0 2024-05-02 10:56:36.000000 dataextractoroeg-0.4.3/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    54972 2024-05-02 11:00:54.000000 dataextractoroeg-0.4.3/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.3/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.3/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-02 11:30:33.000000 dataextractoroeg-0.4.3/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.3/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4105 2024-05-02 11:18:31.000000 dataextractoroeg-0.4.3/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-03 08:03:57.598619 dataextractoroeg-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-03 08:03:35.000000 dataextractoroeg-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.945494 dataextractoroeg-0.4.4/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.4/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.940333 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3078 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 10:13:15.000000 dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3078 2024-05-06 10:13:15.940333 dataextractoroeg-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.906793 dataextractoroeg-0.4.4/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-06 10:13:15.928941 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.4/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-02 11:30:33.000000 dataextractoroeg-0.4.4/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.4/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4351 2024-05-06 10:12:33.000000 dataextractoroeg-0.4.4/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 10:13:15.945494 dataextractoroeg-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-06 10:12:58.000000 dataextractoroeg-0.4.4/setup.py
```

### Comparing `dataextractoroeg-0.4.3/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.4/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.3
+Version: 0.4.4
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.3/LICENSE.txt` & `dataextractoroeg-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/PKG-INFO` & `dataextractoroeg-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.3
+Version: 0.4.4
 Author: Pablo Torija Martínez
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.3/README.md` & `dataextractoroeg-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.4/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.4/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/doiExtractor/main.py` & `dataextractoroeg-0.4.4/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.3/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.4/doiExtractor/openAlex.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,18 @@
             if page_url:
                 row["DOI"] = page_url[1]
                 print(f"Searching in OpenAlex for DOI of {name}: {page_url[1]}")
         else:
             page_url = get_primary_location_by_doi(name, doi)
         
         if page_url is not None:
+            if page_url[0].startswith("https://doi.org/"):
+                doi_from_url = page_url[0].replace("https://doi.org/", "")
+                row["DOI"] = doi_from_url
+                print("Adding missing DOI from primary location")
             row["PRIMARY_LOCATION"] = page_url[0]
             print(f"Searching in OpenAlex for {name} \nFounded link:{page_url[0]}")
         else:
             row["PRIMARY_LOCATION"] = "None"
             print(f"Searching in OpenAlex for {name}: No primary location")
         print("-----------------------------------------------------------------")
```

### Comparing `dataextractoroeg-0.4.3/setup.py` & `dataextractoroeg-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.3",
+    version="0.4.4",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

