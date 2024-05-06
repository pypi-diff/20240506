# Comparing `tmp/snapquery-0.0.4.tar.gz` & `tmp/snapquery-0.0.5.tar.gz`

## Comparing `snapquery-0.0.4.tar` & `snapquery-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,36 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.4/.pydevproject
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.4/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/install
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/scholia.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_view.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_cmdline.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_endpoints.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_namedqueries.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_restful_api.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_scholia.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_wd_query_parsing.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.4/LICENSE
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.4/README.md
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 snapquery-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 snapquery-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.5/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.5/.pydevproject
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery.puml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.5/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 snapquery-0.0.5/samples/ceur-ws.json
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 snapquery-0.0.5/samples/scholia.json
+-rw-r--r--   0        0        0   249023 2020-02-02 00:00:00.000000 snapquery-0.0.5/samples/wikidata-examples.json
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.5/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.5/scripts/install
+-rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 snapquery-0.0.5/scripts/restore_db
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.5/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/__init__.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/mwlogin.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/qimport.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/qimport_view.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/scholia.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    21153 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/snapquery_view.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.5/snapquery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_cmdline.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_endpoints.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_import.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_oauth.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_restful_api.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_scholia.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 snapquery-0.0.5/tests/test_wd_query_parsing.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 snapquery-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 snapquery-0.0.5/README.md
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 snapquery-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 snapquery-0.0.5/PKG-INFO
```

### Comparing `snapquery-0.0.4/.github/workflows/build.yml` & `snapquery-0.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.4/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.5/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.4/snapquery/snapquery_core.py` & `snapquery-0.0.5/snapquery/snapquery_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,88 @@
 
 @author: wf
 """
 
 import json
 import os
 import re
-import requests
-from dataclasses import field
+import uuid
+import datetime
+from dataclasses import field, fields
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Type
 
+import requests
 from lodstorage.csv import CSV
 from lodstorage.query import Endpoint, EndpointManager, Format, Query
 from lodstorage.sparql import SPARQL
 from lodstorage.sql import SQLDB, EntityInfo
 from lodstorage.yamlable import lod_storable
 from ngwidgets.widgets import Link
 
+@lod_storable
+class QueryStats:
+    """
+    statistics about a query
+    """
+    stats_id: str = field(init=False)
+    query_id: str # foreign key
+    endpoint_name: str # foreign key
+    time_stamp: datetime.datetime = field(init=False)
+    duration: float = field(init=False, default=None)  # duration in seconds
+    error_msg: Optional[str]=None
+    
+    def __post_init__(self):
+        """
+        Post-initialization processing to construct a unique identifier for the query
+        and record the timestamp when the query stats object is created.
+        """
+        self.stats_id = str(uuid.uuid4())
+        self.time_stamp = datetime.datetime.now()
 
+    def done(self):
+        """
+        Set the duration by calculating the elapsed time since the `time_stamp`.
+        """
+        self.duration = (datetime.datetime.now() - self.time_stamp).total_seconds()
+
+    def error(self, ex: Exception):
+        """
+        Handle exception of query
+        """
+        self.duration = None
+        self.error_msg = str(ex)
+
+    def as_record(self) -> Dict:
+        record = {}
+        for field in fields(self):
+            # Include field in the record dictionary if it has already been initialized (i.e., not None or has default)
+            if hasattr(self, field.name):
+                record[field.name] = getattr(self, field.name)
+        return record
+    
+    @classmethod
+    def get_samples(cls) -> dict[str, "QueryStats"]:
+        """
+        get samples
+        """
+        samples = {
+            "wikidata-examples": [
+                QueryStats(
+                    query_id="wikidata-examples.cats",
+                    endpoint_name="wikidata",
+                )
+            ]
+        }
+        # Set the duration for each sample instance
+        for sample_list in samples.values():
+            for sample in sample_list:
+                sample.duration = 0.5
+        return samples
+                
 @lod_storable
 class NamedQuery:
     """
     A named query that encapsulates the details and SPARQL query for a specific purpose.
 
     Attributes:
         namespace (str): The namespace of the query, which helps in categorizing the query.
@@ -38,73 +99,123 @@
 
     # namespace
     namespace: str
     # name/id
     name: str
     # sparql query (to be hidden later)
     sparql: str
-    # the url of the source code of the query 
-    url: Optional[str]=None
+    # the url of the source code of the query
+    url: Optional[str] = None
     # one line title
-    title: Optional[str]=None
+    title: Optional[str] = None
     # multiline description
-    description: Optional[str]=None
-  
+    description: Optional[str] = None
+
     def __post_init__(self):
         """
         Post-initialization processing to construct a unique identifier for the query
         based on its namespace and name.
         """
         self.query_id = f"{self.namespace}.{self.name}"
+        
+    @classmethod
+    def get_samples(cls) -> dict[str, "NamedQuery"]:
+        """
+        get samples
+        """
+        samples = {
+            "wikidata-examples": [
+            NamedQuery(
+                namespace="wikidata-examples",
+                name="cats",
+                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Cats",
+                title="Cats on Wikidata",
+                description="This query retrieves all items classified under 'house cat' (Q146) on Wikidata.",
+                sparql="""
+SELECT ?item ?itemLabel
+WHERE {
+  ?item wdt:P31 wd:Q146. # Must be a cat
+  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+}
+""",
+            ),
+            NamedQuery(
+                namespace="wikidata-examples",
+                name="horses",
+                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Horses_(showing_some_info_about_them)",
+                title="Horses on Wikidata",
+                description="This query retrieves information about horses, including parents, gender, and approximate birth and death years.",
+                sparql="""
+SELECT DISTINCT ?horse ?horseLabel ?mother ?motherLabel ?father ?fatherLabel 
+(year(?birthdate) as ?birthyear) (year(?deathdate) as ?deathyear) ?genderLabel
+WHERE {
+  ?horse wdt:P31/wdt:P279* wd:Q726 .     # Instance and subclasses of horse (Q726)
+  OPTIONAL{?horse wdt:P25 ?mother .}     # Mother
+  OPTIONAL{?horse wdt:P22 ?father .}     # Father
+  OPTIONAL{?horse wdt:P569 ?birthdate .} # Birth date
+  OPTIONAL{?horse wdt:P570 ?deathdate .} # Death date
+  OPTIONAL{?horse wdt:P21 ?gender .}     # Gender
+  SERVICE wikibase:label {
+    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],fr,ar,be,bg,bn,ca,cs,da,de,el,en,es,et,fa,fi,he,hi,hu,hy,id,it,ja,jv,ko,nb,nl,eo,pa,pl,pt,ro,ru,sh,sk,sr,sv,sw,te,th,tr,uk,yue,vec,vi,zh"
+  }
+}
+ORDER BY ?horse
+""",
+            )
+        ]
+        }
+        return samples
 
     def as_link(self) -> str:
         """
         get me as a link
         """
         url = f"/query/{self.namespace}/{self.name}"
         text = self.name
         tooltip = "query details"
         link = Link.create(url, text, tooltip)
         return link
 
     @classmethod
     def from_record(cls, record: Dict) -> "NamedQuery":
         """
-        Class method to instantiate NamedQuery from a dictionary record.
+        Class method to instantiate NamedQuery 
+        from a dictionary record.
         """
         return cls(
             namespace=record["namespace"],
             name=record["name"],
-            title=record["title"],
-            url=record["url"],
-            description=record["description"],
-            sparql=record["sparql"],
+            title=record.get("title"),
+            url=record.get("url"),
+            description=record.get("description"),
+            sparql=record.get("sparql"),
         )
-        
-    def as_record(self)->Dict:
+
+    def as_record(self) -> Dict:
         record = {
+            "query_id": self.query_id,
             "namespace": self.namespace,
             "name": self.name,
             "url": self.url,
             "title": self.title,
             "description": self.description,
             "sparql": self.sparql,
         }
         return record
 
     def as_viewrecord(self) -> Dict:
         """
         Return a dictionary representing the NamedQuery with keys ordered as Name, Namespace, Title, Description.
         """
+        url_link = Link.create(self.url, self.url)
         return {
             "name": self.as_link(),
             "namespace": self.namespace,
             "title": self.title,
-            "description": self.description,
-            "url": self.url
+            "url": url_link,
         }
 
 
 class QueryBundle:
     """
     Bundles a named query, a query, and an endpoint into a single manageable object, facilitating the execution of SPARQL queries.
 
@@ -124,16 +235,16 @@
             query (Query): An instance of Query containing the SPARQL query string.
             endpoint (Endpoint): An instance of Endpoint representing the SPARQL endpoint URL.
         """
         self.named_query = named_query
         self.query = query
         self.endpoint = endpoint
         self.sparql = SPARQL(endpoint.endpoint)
-        
-    def raw_query(self,resultFormat, mime_type:str=None, timeout:float=10.0):
+
+    def raw_query(self, resultFormat, mime_type: str = None, timeout: float = 10.0):
         """
         returns raw result of the endpoint
 
         Args:
             resultFormat(str): format of the result
             mime_type(str): mime_type to use (if any)
             timeout(float): timeout in seconds
@@ -146,28 +257,49 @@
         if mime_type:
             headers = {"Accept": mime_type}
         else:
             headers = {}
         endpoint_url = self.endpoint.endpoint
         method = self.endpoint.method
         response = requests.request(
-            method, endpoint_url, headers=headers, data=payload, params=params,timeout=timeout
+            method,
+            endpoint_url,
+            headers=headers,
+            data=payload,
+            params=params,
+            timeout=timeout,
         )
         return response.text
 
     def get_lod(self) -> List[dict]:
         """
         Executes the stored query using the SPARQL service and returns the results as a list of dictionaries.
 
         Returns:
             List[dict]: A list where each dictionary represents a row of results from the SPARQL query.
         """
         lod = self.sparql.queryAsListOfDicts(self.query.query)
         return lod
 
+    def get_lod_with_stats(self) -> tuple[list[dict], QueryStats]:
+        """
+        Executes the stored query using the SPARQL service and returns the results as a list of dictionaries.
+
+        Returns:
+            List[dict]: A list where each dictionary represents a row of results from the SPARQL query.
+        """
+        query_stat = QueryStats(query_id=self.query.name, endpoint_name=self.endpoint.name)
+        try:
+            lod = self.sparql.queryAsListOfDicts(self.query.query)
+            query_stat.done()
+        except Exception as ex:
+            lod = None
+            query_stat.error(ex)
+        return (lod, query_stat)
+
     def format_result(
         self,
         qlod: List[Dict[str, Any]] = None,
         r_format: Format = Format.json,
     ) -> Optional[str]:
         """
         Formats the query results based on the specified format and prints them.
@@ -195,15 +327,15 @@
         elif r_format == Format.json:
             return json.dumps(qlod, indent=2, sort_keys=True, default=str)
         return None  # In case no format is matched or needed
 
     def set_limit(self, limit: int = None):
         """
         set the limit of my query
-        
+
         Args:
             limit(int): the limit to set - default: None
         """
         if limit:
             sparql_query = self.query.query
             # @TODO - this is too naive for cases where
             # there are SPARQL elements hat have a "limit" in the name e.g. "height_limit"
@@ -265,97 +397,101 @@
         """
         if db_path is None:
             db_path = cls.get_cache_path()
 
         nqm = NamedQueryManager(debug=debug)
         path_obj = Path(db_path)
         if not path_obj.exists() or path_obj.stat().st_size == 0:
-            sample_records=cls.get_sample_records()
-            entityInfo = EntityInfo(
-                sample_records, name="NamedQuery", primaryKey="query_id"
-            )
-            nqm.sql_db.createTable(sample_records, "NamedQuery", withDrop=True)
-            nqm.sql_db.store(sample_records, entityInfo)
+            for (source_class,pk) in [
+                (NamedQuery,"query_id"),
+                (QueryStats,"stats_id")
+            ]:
+                # Fetch sample records from the specified class
+                sample_records = cls.get_sample_records(source_class=source_class)
+            
+                # Define entity information dynamically based on the class and primary key
+                entityInfo = EntityInfo(
+                    sample_records, name=source_class.__name__, primaryKey=pk
+                )
+            
+                # Create and populate the table specific to each class
+                nqm.sql_db.createTable(sample_records, source_class.__name__, withDrop=True)
+                nqm.sql_db.store(sample_records, entityInfo,fixNone=True, replace=True)
         return nqm
-    
-    def store(self,lod):
+
+    def store(self, lod: List[Dict[str, Any]], source_class: Type=NamedQuery, primary_key:str="query_id") -> None:
         """
-        store the given list of dicts
+        Stores the given list of dictionaries in the database using entity information
+        derived from a specified source class.
+    
+        Args:
+            lod (List[Dict[str, Any]]): List of dictionaries that represent the records to be stored.
+            source_class (Type): The class from which the entity information is derived. This class
+                should have an attribute or method that defines its primary key and must have a `__name__` attribute.
+            primary_key(str): the primary key to use
+        Raises:
+            AttributeError: If the source class does not have the necessary method or attribute to define the primary key.
         """
-        sample_records=NamedQueryManager.get_sample_records()
+        # Fetch sample records to define the structure of data and to extract entity information.
+        sample_records = NamedQueryManager.get_sample_records(source_class=source_class)
+        
+        # Define entity information based on the source class
         entityInfo = EntityInfo(
-            sample_records, name="NamedQuery", primaryKey="query_id"
+            sample_records, name=source_class.__name__, primaryKey=primary_key
         )
-        self.sql_db.store(lod, entityInfo,fixNone=True,replace=True)
         
-    @classmethod
-    def get_sample_records(cls):
-        sample_queries = cls.get_samples()
-        list_of_records = []
-        for _query_name, named_query in sample_queries.items():
-            record=named_query.as_record()
-            list_of_records.append(record)
-        return list_of_records
-
+        # Store the list of dictionaries in the database using the defined entity information
+        self.sql_db.store(lod, entityInfo, fixNone=True, replace=True)
 
     @classmethod
-    def get_samples(cls) -> dict[str, NamedQuery]:
+    def get_sample_records(cls, source_class: Type) -> List[Dict[str, Any]]:
         """
-        get samples
+        Generates a list of dictionary records based on the sample instances
+        provided by a source class. This method utilizes the `get_samples` method
+        of the source class, which should return a dictionary of sample instances.
+    
+        Args:
+            source_class (Type): The class from which to fetch sample instances.
+                This class must implement a `get_samples` method that returns
+                a dictionary of instances categorized by some key.
+    
+        Returns:
+            List[Dict[str, Any]]: A list of dictionaries where each dictionary
+                is a record that corresponds to a sample instance from the source class.
+    
+        Raises:
+            AttributeError: If the source_class does not have a `get_samples` method.
         """
-        samples = {
-            "wikidata-examples.cats": NamedQuery(
-                namespace="wikidata-examples",
-                name="cats",
-                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Cats",
-                title="Cats on Wikidata",
-                description="This query retrieves all items classified under 'house cat' (Q146) on Wikidata.",
-                sparql="""
-SELECT ?item ?itemLabel
-WHERE {
-  ?item wdt:P31 wd:Q146. # Must be a cat
-  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
-}
-""",
-            ),
-            "wikidata-examples.horses": NamedQuery(
-                namespace="wikidata-examples",
-                name="horses",
-                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Horses_(showing_some_info_about_them)",
-                title="Horses on Wikidata",
-                description="This query retrieves information about horses, including parents, gender, and approximate birth and death years.",
-                sparql="""
-SELECT DISTINCT ?horse ?horseLabel ?mother ?motherLabel ?father ?fatherLabel 
-(year(?birthdate) as ?birthyear) (year(?deathdate) as ?deathyear) ?genderLabel
-WHERE {
-  ?horse wdt:P31/wdt:P279* wd:Q726 .     # Instance and subclasses of horse (Q726)
-  OPTIONAL{?horse wdt:P25 ?mother .}     # Mother
-  OPTIONAL{?horse wdt:P22 ?father .}     # Father
-  OPTIONAL{?horse wdt:P569 ?birthdate .} # Birth date
-  OPTIONAL{?horse wdt:P570 ?deathdate .} # Death date
-  OPTIONAL{?horse wdt:P21 ?gender .}     # Gender
-  SERVICE wikibase:label {
-    bd:serviceParam wikibase:language "[AUTO_LANGUAGE],fr,ar,be,bg,bn,ca,cs,da,de,el,en,es,et,fa,fi,he,hi,hu,hy,id,it,ja,jv,ko,nb,nl,eo,pa,pl,pt,ro,ru,sh,sk,sr,sv,sw,te,th,tr,uk,yue,vec,vi,zh"
-  }
-}
-ORDER BY ?horse
-""",
-            ),
-        }
-        return samples
+        if not hasattr(source_class, "get_samples"):
+            raise AttributeError(f"The class {source_class.__name__} must have a 'get_samples' method.")
+    
+        sample_instances = source_class.get_samples()
+        list_of_records = []
+    
+        # Assuming each key in the returned dictionary of get_samples corresponds to a list of instances
+        for instance_group in sample_instances.values():
+            for instance in instance_group:
+                # Ensure that the instance has an 'as_record' method to convert it to a dictionary
+                if hasattr(instance, "as_record"):
+                    record = instance.as_record()
+                    list_of_records.append(record)
+                else:
+                    raise AttributeError(f"The instance of class {source_class.__name__} does not have an 'as_record' method.")
+    
+        return list_of_records
 
-    def lookup(self, name: str, namespace: str) -> NamedQuery:
+    def lookup(self, name: str, namespace: str,lenient:bool=True) -> NamedQuery:
         """
         lookup the named query for the given name and namespace
 
 
         Args:
             name (str): The name of the named query to execute.
             namespace (str): The namespace of the named query, default is 'wikidata-examples'.
-
+            lenient(bool): if True handle errors as warnings
         Returns:
             NamedQuery: the named query
         """
         sql_query = """SELECT 
     *
 FROM 
     NamedQuery 
@@ -366,15 +502,18 @@
         if not query_records:
             msg = f"NamedQuery not found for the specified name '{name}' and namespace '{namespace}'."
             raise ValueError(msg)
 
         query_count = len(query_records)
         if query_count != 1:
             msg = f"multiple entries ({query_count}) for name '{name}' and namespace '{namespace}'"
-            raise ValueError(msg)
+            if lenient:
+                print(f"warning: {msg}")
+            else:
+                raise ValueError(msg)
 
         record = query_records[0]
         named_query = NamedQuery.from_record(record)
         return named_query
 
     def get_query(
         self,
@@ -405,16 +544,14 @@
             name=name,
             query=sparql_query,
             lang="sparql",
             endpoint=endpoint.endpoint,
             limit=limit,
         )
         endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
-        query.tryItUrl = endpointConf.website
+        query.tryItUrl = query.getTryItUrl(endpoint.website, endpoint.database)
         query.database = endpointConf.database
         query_bundle = QueryBundle(
-            named_query=named_query, 
-            query=query, 
-            endpoint=endpoint
+            named_query=named_query, query=query, endpoint=endpoint
         )
         query_bundle.set_limit(limit)
         return query_bundle
```

### Comparing `snapquery-0.0.4/snapquery/snapquery_view.py` & `snapquery-0.0.5/snapquery/snapquery_view.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 @author: wf
 """
 
 import asyncio
 from typing import List
 
+from lodstorage.query import QuerySyntaxHighlight, ValueFormatter
 from ngwidgets.input_webserver import InputWebSolution
 from ngwidgets.lod_grid import ListOfDictsGrid
 from ngwidgets.widgets import Link
-from nicegui import ui, run, background_tasks
+from nicegui import background_tasks, run, ui
 
-from snapquery.snapquery_core import NamedQuery, QueryBundle
+from snapquery.snapquery_core import NamedQuery, QueryBundle, QueryStats
 
 
 class NamedQueryView:
     """
     display a named Query
     """
 
@@ -29,14 +30,16 @@
         self.solution = solution
         self.nqm = self.solution.nqm
         self.query_bundle = query_bundle
         self.r_format_str = r_format_str
         self.load_task = None
         self.limit = 200
         self.timeout = 20.0
+        # preload ValueFormatter
+        ValueFormatter.getFormats()
         self.setup_ui()
 
     def setup_ui(self):
         """
         setup my user interface
         """
         nq = self.query_bundle.named_query
@@ -48,23 +51,44 @@
             with ui.row() as self.query_parms_row:
                 ui.number(label="limit").bind_value(self, "limit")
                 ui.number(label="time out").bind_value(self, "timeout")
             with ui.row() as self.query_row:
                 self.try_it_link = ui.html(link)
                 ui.label(nq.description)
                 ui.button(icon="play_arrow", on_click=self.run_query)
+            with ui.row():
+                with ui.expansion("Show Query", icon="manage_search").classes("w-full"):
+                    query_syntax_highlight = QuerySyntaxHighlight(
+                        self.query_bundle.query
+                    )
+                    syntax_highlight_css = (
+                        query_syntax_highlight.formatter.get_style_defs()
+                    )
+                    ui.add_css(syntax_highlight_css)
+                    ui.html(query_syntax_highlight.highlight())
             self.grid_row = ui.row()
             pass
 
     async def load_query_results(self):
         """
         (re) load the query results
         """
         self.query_bundle.set_limit(int(self.limit))
-        lod = await run.io_bound(self.query_bundle.get_lod)
+        (lod, stats) = await run.io_bound(self.query_bundle.get_lod_with_stats)
+        self.nqm.store([stats.as_record()], source_class=QueryStats, primary_key="stats_id")
+        query=self.query_bundle.query
+        query.formats=["*:wikidata"]
+        tablefmt="html"
+        query.preFormatWithCallBacks(lod, tablefmt=tablefmt)
+        query.formatWithValueFormatters(lod, tablefmt=tablefmt)
+        for record in lod:
+            for key,value in record.items():
+                if isinstance(value,str):
+                    if value.startswith("http"):
+                        record[key]=Link.create(value,value)
         self.grid_row.clear()
         with self.grid_row:
             self.lod_grid = ListOfDictsGrid()
             self.lod_grid.load_lod(lod)
         self.grid_row.update()
 
     async def run_query(self, _args):
@@ -103,28 +127,28 @@
         self.name = ""
 
     def setup_ui(self):
         """
         setup my user interface
         """
         with ui.row() as self.search_row:
-            self.namespace_search_input = (
-                ui.input(label="namespace", on_change=self.on_search_change)
-                .bind_value(self, "namespace")
-                .props("size=80")
-            )
             self.name_search_input = (
                 ui.input(label="name", on_change=self.on_search_change)
                 .bind_value(self, "name")
                 .props("size=80")
             )
-        with ui.row() as self.search_result_row:
-            self.search_result_grid = ListOfDictsGrid()
+            self.namespace_search_input = (
+                ui.input(label="namespace", on_change=self.on_search_change)
+                .bind_value(self, "namespace")
+                .props("size=40")
+            )
+        self.search_result_row = ui.row()
+        ui.timer(0.0, self.on_search_change, once=True)
 
-    async def on_search_change(self, _args):
+    async def on_search_change(self, _args=None):
         """
         react on changes in the search input
         """
         # Cancel the existing search task if it's still waiting
         if self.search_debounce_task:
             self.search_debounce_task.cancel()
 
@@ -153,18 +177,18 @@
         except Exception as ex:
             self.solution.handle_exception(ex)
 
     def show_lod(self, q_lod: List):
         """
         show the given list of dicts
         """
+        self.search_result_row.clear()
         view_lod = []
         for record in self.q_lod:
             nq = NamedQuery.from_record(record)
             vr = nq.as_viewrecord()
             view_lod.append(vr)
-        if self.search_result_row:
-            with self.search_result_row:
-                ui.notify(f"found {len(q_lod)} queries")
-                self.search_result_grid.load_lod(view_lod)
-                # self.search_result_grid.set_checkbox_selection("#")
-                self.search_result_grid.update()
+        with self.search_result_row:
+            self.search_result_grid = ListOfDictsGrid()
+            ui.notify(f"found {len(q_lod)} queries")
+            self.search_result_grid.load_lod(view_lod)
+        self.search_result_row.update()
```

### Comparing `snapquery-0.0.4/snapquery/snapquery_webserver.py` & `snapquery-0.0.5/snapquery/snapquery_webserver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Created on 2024-05-03
 @author: wf
 """
 
 from fastapi import HTTPException
-from fastapi.responses import HTMLResponse, PlainTextResponse
+from fastapi.responses import FileResponse, HTMLResponse, PlainTextResponse
 from lodstorage.query import Format
 from ngwidgets.input_webserver import InputWebserver, InputWebSolution, WebserverConfig
+from ngwidgets.login import Login
+from ngwidgets.users import Users
 from nicegui import app, ui
 from nicegui.client import Client
+from starlette.responses import RedirectResponse
 
-from snapquery.snapquery_core import NamedQueryManager
+from snapquery.snapquery_core import NamedQueryManager, QueryStats
 from snapquery.snapquery_view import NamedQuerySearch, NamedQueryView
+from snapquery.qimport_view import QueryImportView
 from snapquery.version import Version
 
 
 class SnapQueryWebServer(InputWebserver):
     """
     server to supply named Queries
     """
@@ -35,16 +39,33 @@
         server_config = WebserverConfig.get(config)
         server_config.solution_class = SnapQuerySolution
         return server_config
 
     def __init__(self):
         """Constructs all the necessary attributes for the WebServer object."""
         InputWebserver.__init__(self, config=SnapQueryWebServer.get_config())
+        users = Users("~/.solutions/snapquery")
+        self.login = Login(self, users)
         self.nqm = NamedQueryManager.from_samples()
 
+        @ui.page("/admin")
+        async def admin(client: Client):
+            if not self.login.authenticated():
+                return RedirectResponse("/login")
+            return await self.page(client, SnapQuerySolution.admin_ui)
+
+        @ui.page("/login")
+        async def login(client: Client):
+            return await self.page(client, SnapQuerySolution.login_ui)
+
+        @ui.page("/logout")
+        async def logout(client: Client) -> RedirectResponse:
+            await self.login.logout()
+            return RedirectResponse("/")
+
         @ui.page("/query/{namespace}/{name}")
         async def query_page(
             client: Client,
             namespace: str,
             name: str,
             endpoint_name: str = "wikidata",
             limit: int = None,
@@ -59,14 +80,19 @@
                 namespace=namespace,
                 name=name,
                 endpoint_name=endpoint_name,
                 limit=limit,
                 r_format_str=format,
             )
 
+        @app.get("/api/endpoints")
+        def get_endpoints():
+            endpoints = self.nqm.endpoints
+            return endpoints
+
         @app.get("/api/sparql/{namespace}/{name}")
         def sparql(
             namespace: str,
             name: str,
             endpoint_name: str = "wikidata",
             limit: int = None,
         ) -> PlainTextResponse:
@@ -145,15 +171,16 @@
             name = name[: name.rfind(".")]
         else:
             r_format_str = "html"
 
         try:
             r_format = Format[r_format_str]
             qb = self.nqm.get_query(name, namespace, endpoint_name, limit)
-            qlod = qb.get_lod()
+            (qlod, stats) = qb.get_lod_with_stats()
+            self.nqm.store([stats.as_record()], source_class=QueryStats, primary_key="stats_id")
             content = qb.format_result(qlod, r_format)
             return content
         except Exception as e:
             # Handling specific exceptions can be more detailed based on what nqm.get_sparql and nqm.query can raise
             raise HTTPException(status_code=404, detail=str(e))
 
 
@@ -179,26 +206,53 @@
         """
         add additional settings
         """
         self.add_select("default Endpoint", list(self.nqm.endpoints.keys())).bind_value(
             self, "endpoint_name"
         )
 
+    def setup_menu(self, detailed: bool = None):
+        """
+        setup the menu
+        """
+        super().setup_menu(detailed=detailed)
+        with self.header:
+            if self.webserver.login.authenticated():
+                self.link_button("logout", "/logout", "logout", new_tab=False)
+                self.link_button("admin", "/admin", "supervisor_account", new_tab=False)
+            else:
+                self.link_button("login", "/login", "login", new_tab=False)
+
+    async def admin_ui(self):
+        """
+        admin ui
+        """
+
+        def show():
+            """ """
+            self.query_import_view = QueryImportView(self)
+
+        await self.setup_content_div(show)
+
+    async def login_ui(self):
+        """
+        login ui
+        """
+        await self.webserver.login.login(self)
+
     def setup_ui(self):
         """
         setup my user interface
         """
         self.search = NamedQuerySearch(self)
 
     async def home(
         self,
     ):
-        """Generates the home page with a selection of examples and
-        svg display
-        """
+        """Generates the home page"""
         await self.setup_content_div(self.setup_ui)
 
     async def query_page(
         self,
         namespace: str,
         name: str,
         endpoint_name: str = "wikidata",
```

### Comparing `snapquery-0.0.4/snapquery/version.py` & `snapquery-0.0.5/snapquery/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Version handling for nicepdf
     """
 
     name = "snapquery"
     version = snapquery.__version__
     date = "2024-05-03"
-    updated = "2024-05-04"
+    updated = "2024-05-05"
     description = "Introduce Named Queries and Named Query Middleware to wikidata"
 
     authors = "Wolfgang Fahl"
 
     doc_url = "https://wiki.bitplan.com/index.php/snapquery"
     chat_url = "https://github.com/WolfgangFahl/snapquery/discussions"
     cm_url = "https://github.com/WolfgangFahl/snapquery"
```

### Comparing `snapquery-0.0.4/tests/test_cmdline.py` & `snapquery-0.0.5/tests/test_cmdline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Created on 2024-05-04
 
 @author: wf
 """
-
+import contextlib
 import json
 import sys
+import unittest
 from io import StringIO
 
 from ngwidgets.basetest import Basetest
 
 from snapquery import snapquery_cmd
 
 
@@ -22,21 +23,17 @@
         Basetest.setUp(self, debug=debug, profile=profile)
 
     def capture_stdout(self, callback, *args, **kwargs):
         """
         Executes a callback with given arguments and captures stdout.
         """
         capture = StringIO()
-        original_stdout = sys.stdout
-        sys.stdout = capture
-        try:
+        with contextlib.redirect_stdout(capture):
             callback(*args, **kwargs)
-            return capture.getvalue()
-        finally:
-            sys.stdout = original_stdout
+        return capture.getvalue()
 
     def test_list_endpoints(self):
         """
         test listing endpoints
 
         """
 
@@ -45,14 +42,15 @@
 
         # Capture the output of running the command
         output = self.capture_stdout(run_cmd)
         if self.debug:
             print(output)
         self.assertTrue("wikidata:https://query.wikidata.org" in output)
 
+    @unittest.skipIf(Basetest.inPublicCI(), "reading stdout in CI returns None")
     def test_namedquery(self):
         """
         test a named query via command line
         """
         limit = 10
 
         def run_cmd():
```

### Comparing `snapquery-0.0.4/tests/test_endpoints.py` & `snapquery-0.0.5/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.4/tests/test_restful_api.py` & `snapquery-0.0.5/tests/test_restful_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+import json
 
 from ngwidgets.webserver_test import WebserverTest
 
 from snapquery.snapquery_cmd import SnapQueryCmd
 from snapquery.snapquery_webserver import SnapQueryWebServer
 
 
 class TestRestFulApi(WebserverTest):
     """
     test endpoint handling according to https://github.com/WolfgangFahl/snapquery/issues/1
     """
 
-    def setUp(self, debug=True, profile=True):
+    def setUp(self, debug=False, profile=True):
         server_class = SnapQueryWebServer
         cmd_class = SnapQueryCmd
         WebserverTest.setUp(self, server_class, cmd_class, debug=debug, profile=profile)
 
     def testDemoWebserver(self):
         """
         test API docs access
         """
         # self.debug=True
         html = self.getHtml("/docs")
         self.assertTrue("Swagger" in html)
 
+    def testEndpointApi(self):
+        """
+        test the endpoints api
+        """
+        endpoints_data = self.get_json("/api/endpoints")
+        if self.debug:
+            print(endpoints_data)
+        self.assertTrue("wikidata" in endpoints_data)
+
     def testSparqlApi(self):
         """
         test the plaintext SPARQL API
         """
         for example in ["cats", "horses"]:
             path = f"/api/sparql/wikidata-examples/{example}?limit=10"
             sparql_query = self.getHtml(path)
```

### Comparing `snapquery-0.0.4/tests/test_wd_query_parsing.py` & `snapquery-0.0.5/tests/test_namedqueries.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,70 @@
 """
-Created on 2024-05-04
+Created on 2024-05-03
 
-@author: tholzheim
+@author: wf
 """
 
-import pprint
-import re
-import requests
-import wikitextparser as wtp
-from wikitextparser import Section, Template
+import json
+import tempfile
+import unittest
+
 from ngwidgets.basetest import Basetest
-from snapquery.snapquery_core import NamedQuery, NamedQueryManager
 
-class TestWdQueryParsing(Basetest):
+from snapquery.snapquery_core import NamedQuery, NamedQueryManager, QueryStats
+
+
+class TestNamedQueryManager(Basetest):
     """
-    test wikidata query parsing
+    test the named query Manager
     """
-    
-    def setUp(self, debug=True, profile=True):
+
+    def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
-        self.base_url = "https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples"
-        
-    def _get_examples_wikitext(self) -> str:
-        """Get wiki text with SPARQL query examples"""
-        res = requests.get(f"{self.base_url}?action=raw")
-        return res.text
-
-    def _extract_query_from_section(self, section: Section) -> NamedQuery:
-        """
-        Extract named query from section
-        """
-        query = self._get_sparql_template(section.templates)
-        named_query = None
-        if query:
-            desc = section.plain_text()
-            title = self._sanitize_title(section.title).strip()
-            named_query = NamedQuery(
-                namespace="wikidata-examples",
-                name=title,
-                title=title,
-                description=desc,
-                url=self.base_url,
-                sparql=query.arguments[0].value,
-            )
-        return named_query
-
-    def _sanitize_title(self, section_title: str) -> str:
-        """
-        Sanitize section title by removing translate tags
-        """
-        pattern = r"""<translate><!--T:\d+-->(?P<name>[\w\d\s.\-,\\=<>/|{}()"'&]+)<\/translate>"""
-        match = re.search(pattern, section_title)
-        if match:
-            title = match.group("name")
-        else:
-            title = section_title
-        return title
-
-    def _get_sparql_template(self, templates: list[Template]) -> Template:
-        """
-        Get sparql template of the list of templates
-        If the list contains more than one sparql template None is returned.
-        """
-        queries = []
-        for template in templates:
-            if template.name == "SPARQL":
-                queries.append(template)
-        # ToDo: Handle sections with multiple queries
-        return queries[0] if len(queries) == 1 else None
-
-    def test_wikidata_examples_query_extraction(self):
-        """
-        test extraction and parsing of wikidata example queries to NamedQueries
-
-        Queries can be found at https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples
-        """
-        wikitext = self._get_examples_wikitext()
-        parsed = wtp.parse(wikitext)
-        lod = []
-        for section in parsed.sections:
-            nq = self._extract_query_from_section(section)
-            if nq:
-                lod.append(nq.as_record())
+
+    def testNamedQueries(self):
+        """
+        test getting a named query manager
+        """
+        db_path = "/tmp/named_queries.db"
+        nqm = NamedQueryManager.from_samples(db_path=db_path)
+        for name, ex_count in [("x-invalid", -1), ("cats", 223)]:
+            try:
+                query_bundle = nqm.get_query(name)
+                lod = query_bundle.get_lod()
                 if self.debug:
-                    pprint.pprint(nq)
-        if self.debug:
-            print(f"found {len(lod)} queries")
+                    print(f"{name}:")
+                    print(json.dumps(lod, default=str, indent=2))
+                self.assertEqual(ex_count, len(lod))
+            except Exception as ex:
+                if self.debug:
+                    print(f"{name}:Exception {str(ex)}")
+                self.assertEqual(-1, ex_count)
+
+    def test_query_with_stats(self):
+        """
+        tests executing a query with stats
+        """
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            nqm = NamedQueryManager.from_samples(db_path=tmpfile.name)
+            query_bundle = nqm.get_query("cats")
+            lod, query_stats = query_bundle.get_lod_with_stats()
+            self.assertEqual(query_bundle.query.name, query_stats.query_id)
+            self.assertEqual(query_stats.endpoint_name, query_bundle.endpoint.name)
+            self.assertIsNone(query_stats.error_msg)
+            self.assertIsNotNone(query_stats.duration)
+
+    @unittest.skip
+    def test_query_with_stats_evaluation(self):
+        """
+        test query stats evaluation and storage on a bunch of queries
+        """
         nqm = NamedQueryManager.from_samples()
-        nqm.store(lod)
+        query_records = nqm.sql_db.query("SELECT * FROM NamedQuery LIMIT 20")
+        query_stats = []
+        for query_record in query_records:
+            named_query = NamedQuery.from_record(query_record)
+            query_bundle = nqm.get_query(named_query.name, named_query.namespace)
+            lod, query_stat = query_bundle.get_lod_with_stats()
+            query_stats.append(query_stat)
+        stat_lod = [qs.as_record() for qs in query_stats]
+        nqm.store(stat_lod, source_class=QueryStats, primary_key="stats_id")
```

### Comparing `snapquery-0.0.4/.gitignore` & `snapquery-0.0.5/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+# Nicegui
+.nicegui
```

### Comparing `snapquery-0.0.4/LICENSE` & `snapquery-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.4/README.md` & `snapquery-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,157 @@
 # snapQuery
-Tool that helps users preview, annotate, rate, comment, run and explore Wikidata queries on different sparql backends seamlessly. 
-It enhances the user experience by storing the results and comparing the results from different backends and comparing over time. 
 
-The purpose of the tool is to help users curate and collaborate on queries together and make sure they work as expected over time. 
-Developers and data consumers can get access to the data via APIs.
+A tool that simplifies the process of previewing, annotating, rating, commenting, running, and exploring Wikidata
+queries across different SPARQL backends. It enhances user experience by storing query results and allowing easy
+comparison across various backends and over time.
+
+This tool is designed to assist users in curating and collaborating on queries, ensuring their continued functionality
+over time. Developers and data consumers can access data conveniently through APIs, streamlining their workflow.
 
 [![Join the discussion at https://github.com/WolfgangFahl/snapquery/discussions](https://img.shields.io/github/discussions/WolfgangFahl/snapquery)](https://github.com/WolfgangFahl/snapquery/discussions)
 [![pypi](https://img.shields.io/pypi/pyversions/snapquery)](https://pypi.org/project/snapquery/)
 [![Github Actions Build](https://github.com/WolfgangFahl/snapquery/actions/workflows/build.yml/badge.svg)](https://github.com/WolfgangFahl/snapquery/actions/workflows/build.yml)
 [![PyPI Status](https://img.shields.io/pypi/v/snapquery.svg)](https://pypi.python.org/pypi/snapquery/)
 [![GitHub issues](https://img.shields.io/github/issues/WolfgangFahl/snapquery.svg)](https://github.com/WolfgangFahl/snapquery/issues)
 [![GitHub issues](https://img.shields.io/github/issues-closed/WolfgangFahl/snapquery.svg)](https://github.com/WolfgangFahl/snapquery/issues/?q=is%3Aissue+is%3Aclosed)
 [![GitHub](https://img.shields.io/github/license/WolfgangFahl/snapquery)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Demos
+
 * [BITPlan](https://snapquery.bitplan.com)
 * [RWTH Aachen i5](https://snapquery.wikidata.dbis.rwth-aachen.de/)
 
+## Background
+
+In the Wikimedia ecosystem, we now boast several SPARQL engines and backends housing the complete Wikidata graph for
+querying purposes.
+
+Over recent years, WDQS has encountered escalating timeouts as the graph expands. Users desire alternative endpoints
+without grappling with disparities among SPARQL engines and their impact on query construction.
+
+Recognizing the needs of Wikidata data consumers, we aim to establish a system that simplifies:
+
+- Discovering pre-existing queries
+- Facilitating easy forking, sharing, rating, and monitoring of queries
+- Executing queries (or their variations) on diverse endpoints
+- Comparing query results over time and/or across multiple endpoints
+- Cultivating a collaborative community for query construction
+- Ensuring the reliability of query results
+- Providing alerts if a query no longer yields the expected results
+- Developing tools that access data from dependable, middleware-cached
+  queries via an accessible API, eliminating delays for downstream users.
+
+# Links
+
+* [Phabricator Task: Introduce Named Queries and Named Query Middleware to wikidata](https://phabricator.wikimedia.org/T363894)
+* [Named Queries prototype by Tim Holzheim](https://github.com/tholzheim/named-queries/tree/master)
+
+## Docs
+
+* [Wiki](https://wiki.bitplan.com/index.php/Snapquery)
+* [API documentation](https://snapquery.bitplan.com/docs)
+
+### Model
+
+![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/WolfgangFahl/snapquery/main/snapquery.puml?fmt=svg&version=3)
+
+## Authors
 
+* [Wolfgang Fahl](http://www.bitplan.com/Wolfgang_Fahl)
+* [Tim Holzheim](https://rwthcontacts.rwth-aachen.de/person/PER-46LT8TU)
 
 # Features
+
 ## Planned
+
 These are the planned features
+
+* support for naming queries ([#9][i9]) ✅
+* support for sharing queries (unique identifier) ([#2][i2]) ✅
 * query multiple backends simultaneously and repeatedly
 * stores queries and adaptations needed for different backends
 * support user login
 * support for spam protection
-* support for naming queries
 * support for rating queries
-* support for sharing queries (unique identifier)
 * support for commenting on queries
 * support for detecting when a query returns different results between different backends
 * support for query states: reliable, needs investigation, need verification
-* support for autodetecting when a query returns fewer results than before (change in underlying data/model in Wikidata) -> needs investigation
+* support for autodetecting when a query returns fewer results than before (change in underlying data/model in
+  Wikidata) -> needs investigation
 * support for marking queries as reliable query by users
 * support for seeing a state history per query
 * support for storing query results so you don’t have to wait
 * support for adding metadata to queries
-  * add main subject (QID) to query
-  * author -> id of author in the system
-  * forked from x
-* has REST API for data consumers e.g. LLM developers who want to present user-verified queries and data to users to increase reliability
+    * add main subject (QID) to query
+    * author -> id of author in the system
+    * forked from x
+* has REST API for data consumers e.g. LLM developers who want to present user-verified queries and data to users to
+  increase reliability
 
 ## User stories
+
 * as a user I want to know in advance if the query is returning what I expect
 * as a user I want to find all the bands in Wikidata without having to know how it is modeled
 * as a user I want pay someone to help me get the information from Wikidata that I need
-* as a user I want to know how a query performed in the past so I can trust that the underlying model is stable and I get the expected results
+* as a user I want to know how a query performed in the past so I can trust that the underlying model is stable and I
+  get the expected results
 * as a user I want to comment on a query
 * as a user I want to read comments from others on a query so I get and idea how reliable it is
 * as a user I want to rate a query with 1-5 stars
 * as a user I want to get information from multiple sparql engines at the same time
-* as a user I don’t want to wait for a fresh query to finish and just get the information from the latest time a query succeeded.
+* as a user I don’t want to wait for a fresh query to finish and just get the information from the latest time a query
+  succeeded.
 * as a user I want a list of queries in the middleware
 * as a user I want to sort the list based on the rate of queries
 * as a user I want to annotate a query with a name
 * as a user I want to annotate a query with a wikidata item as main subject
 * as a user I want to see a list of queries that is tagged with a certain topic (wikidata item)
 * as a user I want an API to get information from the middleware about queries
 * as a user I want an api endpoint /list that gives me all queries with the main subject=Qxxxx
-* as a user I want the system to warn me and annotate a query that no longer returns the data the user expects, ie. if a query suddenly start returning no results or fewer results
+* as a user I want the system to warn me and annotate a query that no longer returns the data the user expects, ie. if a
+  query suddenly start returning no results or fewer results
 * as a user I want to see a state on a query
 * as a user I want to log in using github to avoid the hassle of creating another account
 * as a user I want to log in using gitlab to avoid the hassle of creating another account
 * as a user I want to log in using facebook to avoid the hassle of creating another account
 * as a user I want to know how many backends a query is working on, so I get an overview
 * as a user I want to get query results immediately if possible so I don’t have to wait
 * as a user I want to import a query by copy pasting a url from WDQS
 * as a user I want to run a query on multiple backends with one click
 * as a user I want to fork a query and build on it
+* as a user I want an email if a query I'm watching needs investigation
+* as a user I want settings to control whether I get email notifications or not for all queries I'm watching
+* as a user I want to watch a query
+* as a user I want to see the history of actions of other users
+* as a user I want to know who created a query
+* as a user I want a setting to get email about new comments on queries I'm watching
+* as a user I want a setting to get emails about new queries every day, week, month
+* as a user I want to star a query
+* as a user I want to browse queries and sort by number of stars
+* as a user I want to see who starred a query
+* as a user I want to see a list of my notifications
 * as a wikidata contributor I want to be able to override the “bad query” state
-* as a wikidata user I want to be able to log in using my wmf credentials to avoid the hassle of creating another account
+* as a wikidata user I want to be able to log in using my wmf credentials to avoid the hassle of creating another
+  account
 * as a wikidata user I want to link my current account to my wmf account so others can find me by username
 * as a developer I want to expose the data in API endpoints
-* as a LLM developer I want to consume the queries and use them to improve my LLM so it can suggest KNOWN GOOD queries to users
+* as a LLM developer I want to consume the queries and use them to improve my LLM so it can suggest KNOWN GOOD queries
+  to users
+
+[i10]: https://github.com/WolfgangFahl/snapquery/issues/10
+[i9]: https://github.com/WolfgangFahl/snapquery/issues/9
+
+[i8]: https://github.com/WolfgangFahl/snapquery/issues/8
+
+[i7]: https://github.com/WolfgangFahl/snapquery/issues/7
+
+[i6]: https://github.com/WolfgangFahl/snapquery/issues/6
+
+[i5]: https://github.com/WolfgangFahl/snapquery/issues/5
+
+[i4]: https://github.com/WolfgangFahl/snapquery/issues/4
+
+[i3]: https://github.com/WolfgangFahl/snapquery/issues/3
+
+[i2]: https://github.com/WolfgangFahl/snapquery/issues/2
+
+[i1]: https://github.com/WolfgangFahl/snapquery/issues/1
```

### Comparing `snapquery-0.0.4/pyproject.toml` & `snapquery-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,28 @@
   {name = "Wolfgang Fahl", email = "wf@WolfgangFahl.com"}
 ]
 maintainers = [
   { name = "Wolfgang Fahl", email = "wf@WolfgangFahl.com" },
 ]
 readme = "README.md"
 license = {text = "Apache-2.0"}
+
+
 dependencies = [
 	# https://github.com/WolfgangFahl/nicegui_widgets
-	"ngwidgets>=0.14.2",
+	"ngwidgets>=0.15.0",
     # https://pypi.org/project/pyLodStorage/
     "pyLodStorage>=0.10.5",
     "wikitextparser",
-    "requests"
+    "requests",
+    # https://pypi.org/project/mwoauth/
+    "mwoauth>=0.4.0",
+    #"mwoauth@git+https://github.com/mediawiki-utilities/python-mwoauth"
+    #https://pypi.org/project/tqdm/
+    "tqdm>=4.66.4"
 ]
 
 requires-python = ">=3.9"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
@@ -41,14 +48,17 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
     ]
 dynamic = ["version"]
 [tool.hatch.version]
 path = "snapquery/__init__.py"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [project.urls]
 Home = "https://github.com/WolfgangFahl/snapquery"
 Documentation = "https://wiki.bitplan.com/index.php/snapquery"
 Source = "https://github.com/WolfgangFahl/snapquery"
 
 [project.optional-dependencies]
 test = [
```

