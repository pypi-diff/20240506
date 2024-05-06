# Comparing `tmp/geoparser-0.1.5.tar.gz` & `tmp/geoparser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoparser-0.1.5.tar", last modified: Sat May  4 17:19:45 2024, max compression
+gzip compressed data, was "geoparser-0.1.6.tar", last modified: Mon May  6 11:25:33 2024, max compression
```

## Comparing `geoparser-0.1.5.tar` & `geoparser-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.709174 geoparser-0.1.5/
--rw-rw-rw-   0        0        0     1083 2024-05-04 16:50:30.000000 geoparser-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     5547 2024-05-04 17:19:45.708176 geoparser-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5145 2024-05-04 16:50:30.000000 geoparser-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.691173 geoparser-0.1.5/geoparser/
--rw-rw-rw-   0        0        0       34 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/__init__.py
--rw-rw-rw-   0        0        0      890 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/__main__.py
--rw-rw-rw-   0        0        0     6101 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/database.py
--rw-rw-rw-   0        0        0     2663 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/downloader.py
--rw-rw-rw-   0        0        0     1525 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/entities.py
--rw-rw-rw-   0        0        0    11661 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/geoparser.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.707174 geoparser-0.1.5/geoparser.egg-info/
--rw-rw-rw-   0        0        0     5547 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 17:19:45.709174 geoparser-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      763 2024-05-04 16:50:30.000000 geoparser-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:25:33.215005 geoparser-0.1.6/
+-rw-rw-rw-   0        0        0     1083 2024-05-04 16:50:30.000000 geoparser-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6416 2024-05-06 11:25:33.215005 geoparser-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5817 2024-05-06 10:54:34.000000 geoparser-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:25:33.200004 geoparser-0.1.6/geoparser/
+-rw-rw-rw-   0        0        0       34 2024-05-04 16:50:30.000000 geoparser-0.1.6/geoparser/__init__.py
+-rw-rw-rw-   0        0        0      890 2024-05-04 16:50:30.000000 geoparser-0.1.6/geoparser/__main__.py
+-rw-rw-rw-   0        0        0     6101 2024-05-04 16:50:30.000000 geoparser-0.1.6/geoparser/database.py
+-rw-rw-rw-   0        0        0     2663 2024-05-04 16:50:30.000000 geoparser-0.1.6/geoparser/downloader.py
+-rw-rw-rw-   0        0        0     1525 2024-05-04 16:50:30.000000 geoparser-0.1.6/geoparser/entities.py
+-rw-rw-rw-   0        0        0    12396 2024-05-06 10:24:09.000000 geoparser-0.1.6/geoparser/geoparser.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:25:33.214004 geoparser-0.1.6/geoparser.egg-info/
+-rw-rw-rw-   0        0        0     6416 2024-05-06 11:25:33.000000 geoparser-0.1.6/geoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-06 11:25:33.000000 geoparser-0.1.6/geoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:25:33.000000 geoparser-0.1.6/geoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-06 11:25:33.000000 geoparser-0.1.6/geoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 11:25:33.000000 geoparser-0.1.6/geoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:25:33.215005 geoparser-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-05-06 10:37:33.000000 geoparser-0.1.6/setup.py
```

### Comparing `geoparser-0.1.5/LICENSE` & `geoparser-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.5/PKG-INFO` & `geoparser-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: geoparser
-Version: 0.1.5
-Summary: A geoparsing library for English texts
-Author: Diego Gomes
-Author-email: diego.gomes@uzh.ch
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Geoparser
 
 Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and fine-tuned SentenceTransformer models for toponym resolution.
 
 ## Installation
 
 Install Geoparser using pip:
@@ -113,25 +100,37 @@
 - `country_name`: The name of the country.
 - `feature_name`: The type of geographical feature (e.g., mountain, lake).
 - `latitude`: The latitude of the location.
 - `longitude`: The longitude of the location.
 - `elevation`: The elevation of the location in meters.
 - `population`: The population of the location.
 
+### Geocoding Scope
+
+You can limit the scope of geocoding by specifying one or more countries and [GeoNames feature classes](https://www.geonames.org/export/codes.html). This ensures that Geoparser only encodes locations within the specified countries, and can limit the types of geographical features to consider. To use this feature, use the `country_filter` and `feature_filter` parameters in the `parse` method:
+
+```python
+docs = geo.parse(texts, country_filter=['CH', 'DE', 'AT'], feature_filter=['A', 'P'])
+```
+
 ## Example
 
 Here's an example illustrating how the library might be used:
 
 ```python
 from geoparser import Geoparser
 
 geo = Geoparser()
 
-text = "Zurich is a city rich in history."
+texts = [
+    "Zurich is a city rich in history.",
+    "Geneva is known for its role in international diplomacy.",
+    "Munich is famous for its annual Oktoberfest celebration."
+]    
 
-docs = geo.parse([text])
+docs = geo.parse([texts])
 
 for doc in docs:
     for toponym in doc.toponyms:
         if toponym.location:
             print(toponym, "->", toponym.location)
 ```
```

### Comparing `geoparser-0.1.5/README.md` & `geoparser-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: geoparser
+Version: 0.1.6
+Summary: A geoparsing library for English texts
+Author: Diego Gomes
+Author-email: diego.gomes@uzh.ch
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: spacy
+Requires-Dist: sentence_transformers
+Requires-Dist: tqdm
+Requires-Dist: torch
+Requires-Dist: requests
+Requires-Dist: appdirs
+
 # Geoparser
 
 Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and fine-tuned SentenceTransformer models for toponym resolution.
 
 ## Installation
 
 Install Geoparser using pip:
@@ -100,25 +121,37 @@
 - `country_name`: The name of the country.
 - `feature_name`: The type of geographical feature (e.g., mountain, lake).
 - `latitude`: The latitude of the location.
 - `longitude`: The longitude of the location.
 - `elevation`: The elevation of the location in meters.
 - `population`: The population of the location.
 
+### Geocoding Scope
+
+You can limit the scope of geocoding by specifying one or more countries and [GeoNames feature classes](https://www.geonames.org/export/codes.html). This ensures that Geoparser only encodes locations within the specified countries, and can limit the types of geographical features to consider. To use this feature, use the `country_filter` and `feature_filter` parameters in the `parse` method:
+
+```python
+docs = geo.parse(texts, country_filter=['CH', 'DE', 'AT'], feature_filter=['A', 'P'])
+```
+
 ## Example
 
 Here's an example illustrating how the library might be used:
 
 ```python
 from geoparser import Geoparser
 
 geo = Geoparser()
 
-text = "Zurich is a city rich in history."
+texts = [
+    "Zurich is a city rich in history.",
+    "Geneva is known for its role in international diplomacy.",
+    "Munich is famous for its annual Oktoberfest celebration."
+]    
 
-docs = geo.parse([text])
+docs = geo.parse([texts])
 
 for doc in docs:
     for toponym in doc.toponyms:
         if toponym.location:
             print(toponym, "->", toponym.location)
 ```
```

### Comparing `geoparser-0.1.5/geoparser/__main__.py` & `geoparser-0.1.6/geoparser/__main__.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.5/geoparser/database.py` & `geoparser-0.1.6/geoparser/database.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.5/geoparser/downloader.py` & `geoparser-0.1.6/geoparser/downloader.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.5/geoparser/entities.py` & `geoparser-0.1.6/geoparser/entities.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.5/geoparser/geoparser.py` & `geoparser-0.1.6/geoparser/geoparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         self.model_max_length = self.tokenizer.model_max_length
 
     def ensure_spacy_model(self, model_name):
         if not spacy.util.is_package(model_name):
             print(f"Downloading spaCy model '{model_name}'...")
             spacy.cli.download(model_name)
 
-    def parse(self, texts: List[str]):
+    def parse(self, texts: List[str], country_filter: List[str] = None, feature_filter: List[str] = None):
         if not isinstance(texts, list) or not all(isinstance(text, str) for text in texts):
             raise TypeError("Input must be a list of strings")
 
         documents = [Document(text) for text in texts]
         for document in documents:
             self.extract_toponyms(document)
-        self.resolve_toponyms(documents)
+        self.resolve_toponyms(documents, country_filter, feature_filter)
         return documents
 
     def extract_toponyms(self, document: Document):
         doc = self.nlp(document.text)
         sentences = list(doc.sents)
         total_tokens = len(self.tokenizer.tokenize(document.text))
 
@@ -48,24 +48,24 @@
                 text, start_char, end_char = self.clean_ent(ent)
                 context = document.text if total_tokens <= self.model_max_length else self.truncate_context(sentences, ent)
                 document.toponyms.append(Toponym(text, start_char, end_char, context))
 
     def clean_ent(self, ent):
         # remove leading lowercase 'the'
         original_text = ent.text
-        new_text = re.sub(r"^the\s+", "", original_text)
+        new_text = re.sub(r"^the\s+", "", original_text).lstrip('"')
         if new_text != original_text:
             new_text = new_text.lstrip()
             start_char = ent.start_char + (len(original_text) - len(new_text))
         else:
             start_char = ent.start_char
 
         # remove trailing possessive 's
         original_text = new_text
-        new_text = re.sub(r"\'s$", "", original_text)
+        new_text = re.sub(r"\'s$", "", original_text).rstrip('"')
         if new_text != original_text:
             new_text = new_text.rstrip()
             end_char = start_char + len(new_text)
         else:
             end_char = start_char + len(original_text)
 
         return new_text, start_char, end_char
@@ -103,19 +103,19 @@
 
             # Break if no sentences were added in the last iteration
             if not expanded:
                 break
 
         return ' '.join(context_sentences)
 
-    def resolve_toponyms(self, documents: List[Document]):
+    def resolve_toponyms(self, documents: List[Document], country_filter: List[str] = None, feature_filter: List[str] = None):
         all_candidates = set()
         for document in documents:
             for toponym in document.toponyms:
-                candidates = self.fetch_candidates(toponym.name)
+                candidates = self.fetch_candidates(toponym.name, country_filter, feature_filter)
                 all_candidates.update(candidates)
                 toponym.candidates = candidates
 
         if all_candidates:
             all_candidates = list(all_candidates)
             pseudotexts = self.fetch_pseudotexts(all_candidates)
             candidate_embeddings = self.transformer.encode(pseudotexts, batch_size=8, show_progress_bar=True, convert_to_tensor=True)
@@ -142,51 +142,68 @@
 
     def execute_query(self, query, params=None):
         with sqlite3.connect(self.db_path) as conn:
             cursor = conn.cursor()
             cursor.execute(query, params or ())
             return cursor.fetchall()
                     
-    def fetch_candidates(self, toponym):
-        # Note: The name 'US' was not considered an alternatename of the United States.
-        #       It has now been added to the GeoNames database (03.05.2024).
-        #       The following line is a temporary fix until the GeoNames download server updates the files.
-        toponym = 'U.S.' if toponym == 'US' else toponym
+    def fetch_candidates(self, toponym, country_filter=None, feature_filter=None):
+
+        toponym = re.sub(r"\"", "", toponym).strip()
 
         toponym = ' '.join([f'"{word}"' for word in toponym.split()])
 
-        query = '''
+        base_query = '''
             WITH MinRankAllCountries AS (
                 SELECT MIN(rank) AS MinRank FROM allCountries_fts WHERE allCountries_fts MATCH ?
             ),
             MinRankAlternateNames AS (
                 SELECT MIN(rank) AS MinRank FROM alternateNames_fts WHERE alternateNames_fts MATCH ?
             ),
             CombinedResults AS (
                 SELECT allCountries_fts.rowid as geonameid, allCountries_fts.rank as rank
                 FROM allCountries_fts
                 WHERE allCountries_fts MATCH ?
-                
+
                 UNION
-                
+
                 SELECT alternateNames.geonameid, alternateNames_fts.rank as rank
-                FROM alternateNames
-                JOIN alternateNames_fts ON alternateNames_fts.rowid = alternateNames.alternateNameId
+                FROM alternateNames_fts
+                JOIN alternateNames ON alternateNames_fts.rowid = alternateNames.alternateNameId
                 WHERE alternateNames_fts MATCH ?
             )
-            SELECT geonameid
-            FROM CombinedResults
-            WHERE rank = (SELECT MinRank FROM MinRankAllCountries)
-            OR rank = (SELECT MinRank FROM MinRankAlternateNames)
-            GROUP BY geonameid
-            ORDER BY rank
+            SELECT ac.geonameid
+            FROM CombinedResults cr
+            JOIN allCountries ac ON cr.geonameid = ac.geonameid
+            WHERE (cr.rank = (SELECT MinRank FROM MinRankAllCountries)
+                   OR cr.rank = (SELECT MinRank FROM MinRankAlternateNames))
         '''
-        params = (toponym, toponym, toponym, toponym)
-        result = self.execute_query(query, params)
-        return [(row[0]) for row in result]
+
+        where_clauses = []
+        params = [toponym, toponym, toponym, toponym]
+
+        # Adding filters for country codes
+        if country_filter:
+            where_clauses.append(f"ac.country_code IN ({','.join(['?' for _ in country_filter])})")
+            params.extend(country_filter)
+
+        # Adding filters for feature classes
+        if feature_filter:
+            where_clauses.append(f"ac.feature_class IN ({','.join(['?' for _ in feature_filter])})")
+            params.extend(feature_filter)
+
+        # Append additional filters if present
+        if where_clauses:
+            base_query += f" AND {' AND '.join(where_clauses)}"
+
+        base_query += " GROUP BY ac.geonameid ORDER BY cr.rank"
+
+        # Execute query with the constructed parameters
+        result = self.execute_query(base_query, tuple(params))
+        return [row[0] for row in result]
 
     def fetch_pseudotexts(self, candidate_ids, batch_size=500):
         chunks = [candidate_ids[i:i + batch_size] for i in range(0, len(candidate_ids), batch_size)]
         results_dict = {}
         for chunk in chunks:
             placeholders = ', '.join(['?' for _ in chunk])
             query = f"""
```

### Comparing `geoparser-0.1.5/geoparser.egg-info/PKG-INFO` & `geoparser-0.1.6/geoparser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: geoparser
-Version: 0.1.5
+Version: 0.1.6
 Summary: A geoparsing library for English texts
 Author: Diego Gomes
 Author-email: diego.gomes@uzh.ch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: spacy
+Requires-Dist: sentence_transformers
+Requires-Dist: tqdm
+Requires-Dist: torch
+Requires-Dist: requests
+Requires-Dist: appdirs
 
 # Geoparser
 
 Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and fine-tuned SentenceTransformer models for toponym resolution.
 
 ## Installation
 
@@ -113,25 +121,37 @@
 - `country_name`: The name of the country.
 - `feature_name`: The type of geographical feature (e.g., mountain, lake).
 - `latitude`: The latitude of the location.
 - `longitude`: The longitude of the location.
 - `elevation`: The elevation of the location in meters.
 - `population`: The population of the location.
 
+### Geocoding Scope
+
+You can limit the scope of geocoding by specifying one or more countries and [GeoNames feature classes](https://www.geonames.org/export/codes.html). This ensures that Geoparser only encodes locations within the specified countries, and can limit the types of geographical features to consider. To use this feature, use the `country_filter` and `feature_filter` parameters in the `parse` method:
+
+```python
+docs = geo.parse(texts, country_filter=['CH', 'DE', 'AT'], feature_filter=['A', 'P'])
+```
+
 ## Example
 
 Here's an example illustrating how the library might be used:
 
 ```python
 from geoparser import Geoparser
 
 geo = Geoparser()
 
-text = "Zurich is a city rich in history."
+texts = [
+    "Zurich is a city rich in history.",
+    "Geneva is known for its role in international diplomacy.",
+    "Munich is famous for its annual Oktoberfest celebration."
+]    
 
-docs = geo.parse([text])
+docs = geo.parse([texts])
 
 for doc in docs:
     for toponym in doc.toponyms:
         if toponym.location:
             print(toponym, "->", toponym.location)
 ```
```

### Comparing `geoparser-0.1.5/setup.py` & `geoparser-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='geoparser',
-    version='0.1.5',
+    version='0.1.6',
     author='Diego Gomes',
     author_email='diego.gomes@uzh.ch',
     packages=find_packages(),
     description='A geoparsing library for English texts',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

