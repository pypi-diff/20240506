# Comparing `tmp/hamu-tool-0.0.7.tar.gz` & `tmp/hamu-tool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamu-tool-0.0.7.tar", last modified: Tue Apr 30 09:32:24 2024, max compression
+gzip compressed data, was "hamu-tool-0.0.8.tar", last modified: Tue Apr 30 10:01:54 2024, max compression
```

## Comparing `hamu-tool-0.0.7.tar` & `hamu-tool-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.601727 hamu-tool-0.0.7/
--rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 09:38:40.591727 hamu-tool-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1325 2024-03-15 09:30:00.000000 hamu-tool-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.231730 hamu-tool-0.0.7/hamu_tool/
--rw-rw-r--   0 root         (0) root         (0)       21 2024-04-30 09:38:11.000000 hamu-tool-0.0.7/hamu_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.551728 hamu-tool-0.0.7/hamu_tool/dataset/
--rw-rw-r--   0 root         (0) root         (0)       37 2024-03-12 06:06:56.000000 hamu-tool-0.0.7/hamu_tool/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2047 2024-04-30 06:08:48.000000 hamu-tool-0.0.7/hamu_tool/dataset/arguana_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2283 2024-04-30 06:09:22.000000 hamu-tool-0.0.7/hamu_tool/dataset/bioasq_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2143 2024-04-30 06:09:25.000000 hamu-tool-0.0.7/hamu_tool/dataset/climate_fever_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2497 2024-04-30 08:19:11.000000 hamu-tool-0.0.7/hamu_tool/dataset/data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     5753 2024-04-29 23:54:14.000000 hamu-tool-0.0.7/hamu_tool/dataset/data_loader_base.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-30 06:09:31.000000 hamu-tool-0.0.7/hamu_tool/dataset/dbpedia_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-30 06:09:34.000000 hamu-tool-0.0.7/hamu_tool/dataset/fever_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     1996 2024-04-30 06:09:36.000000 hamu-tool-0.0.7/hamu_tool/dataset/fiqa_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2112 2024-04-30 06:09:38.000000 hamu-tool-0.0.7/hamu_tool/dataset/hotpotqa_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-30 06:09:41.000000 hamu-tool-0.0.7/hamu_tool/dataset/msmarco_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2227 2024-04-30 06:09:43.000000 hamu-tool-0.0.7/hamu_tool/dataset/nfcorpus_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     1952 2024-04-30 06:09:47.000000 hamu-tool-0.0.7/hamu_tool/dataset/nq_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     1953 2024-04-30 06:09:50.000000 hamu-tool-0.0.7/hamu_tool/dataset/quora_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 06:09:55.000000 hamu-tool-0.0.7/hamu_tool/dataset/robust04_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2708 2024-04-30 09:21:46.000000 hamu-tool-0.0.7/hamu_tool/dataset/scidocs_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2110 2024-04-30 06:09:59.000000 hamu-tool-0.0.7/hamu_tool/dataset/scifact_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 06:10:02.000000 hamu-tool-0.0.7/hamu_tool/dataset/signal1m_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-04-30 08:18:43.000000 hamu-tool-0.0.7/hamu_tool/dataset/touche_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2344 2024-04-30 08:18:55.000000 hamu-tool-0.0.7/hamu_tool/dataset/touche_v2_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2287 2024-04-30 06:10:04.000000 hamu-tool-0.0.7/hamu_tool/dataset/trec_covid_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2387 2024-04-30 06:10:07.000000 hamu-tool-0.0.7/hamu_tool/dataset/trec_news_data_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.583727 hamu-tool-0.0.7/hamu_tool/utils/
--rw-rw-r--   0 root         (0) root         (0)      108 2024-03-15 04:53:55.000000 hamu-tool-0.0.7/hamu_tool/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7220 2024-03-12 08:20:43.000000 hamu-tool-0.0.7/hamu_tool/utils/bib_extractor.py
--rw-rw-r--   0 root         (0) root         (0)     8776 2024-04-25 06:49:16.000000 hamu-tool-0.0.7/hamu_tool/utils/corpus_reader.py
--rw-r--r--   0 root         (0) root         (0)     4915 2024-03-16 04:32:45.000000 hamu-tool-0.0.7/hamu_tool/utils/pprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.371729 hamu-tool-0.0.7/hamu_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-30 09:38:40.000000 hamu-tool-0.0.7/hamu_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 04:25:55.000000 hamu-tool-0.0.7/hamu_tool.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:38:40.602727 hamu-tool-0.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      593 2024-04-30 09:38:32.000000 hamu-tool-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:08:10.424132 hamu-tool-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 10:08:10.404132 hamu-tool-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-30 10:06:54.000000 hamu-tool-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:08:09.775137 hamu-tool-0.0.8/hamu_tool/
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-04-30 10:05:28.000000 hamu-tool-0.0.8/hamu_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:08:10.247133 hamu-tool-0.0.8/hamu_tool/dataset/
+-rw-rw-r--   0 root         (0) root         (0)       37 2024-03-12 06:06:56.000000 hamu-tool-0.0.8/hamu_tool/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-30 10:00:49.000000 hamu-tool-0.0.8/hamu_tool/dataset/arguana_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-30 10:01:02.000000 hamu-tool-0.0.8/hamu_tool/dataset/bioasq_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-04-30 10:01:19.000000 hamu-tool-0.0.8/hamu_tool/dataset/climate_fever_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2497 2024-04-30 08:19:11.000000 hamu-tool-0.0.8/hamu_tool/dataset/data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     5753 2024-04-29 23:54:14.000000 hamu-tool-0.0.8/hamu_tool/dataset/data_loader_base.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-30 10:01:31.000000 hamu-tool-0.0.8/hamu_tool/dataset/dbpedia_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-30 10:01:48.000000 hamu-tool-0.0.8/hamu_tool/dataset/fever_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     1996 2024-04-30 10:01:56.000000 hamu-tool-0.0.8/hamu_tool/dataset/fiqa_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-30 10:02:06.000000 hamu-tool-0.0.8/hamu_tool/dataset/hotpotqa_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-30 10:02:16.000000 hamu-tool-0.0.8/hamu_tool/dataset/msmarco_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2227 2024-04-30 10:02:23.000000 hamu-tool-0.0.8/hamu_tool/dataset/nfcorpus_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-30 10:02:32.000000 hamu-tool-0.0.8/hamu_tool/dataset/nq_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-04-30 10:02:41.000000 hamu-tool-0.0.8/hamu_tool/dataset/quora_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 10:02:52.000000 hamu-tool-0.0.8/hamu_tool/dataset/robust04_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2708 2024-04-30 10:03:01.000000 hamu-tool-0.0.8/hamu_tool/dataset/scidocs_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2110 2024-04-30 10:03:10.000000 hamu-tool-0.0.8/hamu_tool/dataset/scifact_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 10:03:18.000000 hamu-tool-0.0.8/hamu_tool/dataset/signal1m_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-30 10:03:30.000000 hamu-tool-0.0.8/hamu_tool/dataset/touche_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-30 10:03:38.000000 hamu-tool-0.0.8/hamu_tool/dataset/touche_v2_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-30 10:03:44.000000 hamu-tool-0.0.8/hamu_tool/dataset/trec_covid_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-30 10:04:10.000000 hamu-tool-0.0.8/hamu_tool/dataset/trec_news_data_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:08:10.390132 hamu-tool-0.0.8/hamu_tool/utils/
+-rw-rw-r--   0 root         (0) root         (0)      108 2024-03-15 04:53:55.000000 hamu-tool-0.0.8/hamu_tool/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7220 2024-03-12 08:20:43.000000 hamu-tool-0.0.8/hamu_tool/utils/bib_extractor.py
+-rw-rw-r--   0 root         (0) root         (0)     8776 2024-04-25 06:49:16.000000 hamu-tool-0.0.8/hamu_tool/utils/corpus_reader.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2024-03-16 04:32:45.000000 hamu-tool-0.0.8/hamu_tool/utils/pprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:08:09.954136 hamu-tool-0.0.8/hamu_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 10:08:09.000000 hamu-tool-0.0.8/hamu_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-30 10:08:09.000000 hamu-tool-0.0.8/hamu_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:08:09.000000 hamu-tool-0.0.8/hamu_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 04:25:55.000000 hamu-tool-0.0.8/hamu_tool.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-30 10:08:09.000000 hamu-tool-0.0.8/hamu_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 10:08:09.000000 hamu-tool-0.0.8/hamu_tool.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:08:10.424132 hamu-tool-0.0.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-04-30 10:05:34.000000 hamu-tool-0.0.8/setup.py
```

### Comparing `hamu-tool-0.0.7/README.md` & `hamu-tool-0.0.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,52 +3,57 @@
 
 Please join our [discord](https://discord.gg/m93jftsr7g) for any help.
 
 ## Dataset
 ### DataLoader
 - Full list of available dataset: [HAMU Dataset](http://research.hamu.me/dataset/)
 
-- How to load dataset
+- How to iterate all data
 ```py
 from hamu_tool.dataset import DataLoader
 
-loader = DataLoader.load('beir/nfcorpus')
+loader = DataLoader.load('beir/arguana')
 
 for doc in loader.get_docs():
-    print(doc['id'], doc['title'], doc['text'])
+    print(doc.id, doc.text, doc.title)
     break
 
 for query in loader.get_qeuries():
-    print(query['id'], query['text'])
+    print(query.id, query.title)
     break
 
-for qrel in loader.get_qrels():
-    print(qrel['qid'], qrel['did'], qrel['score'])
+for qrel in loader.get_qrels('[mode]'):
+    print(qrel.qid, qrel.did, qrel.score)
     break
 ```
 
-- How to fetch a document or a query
+- How to fetch a single item
 ```py
 from hamu_tool.dataset import DataLoader
 
-loader = DataLoader.load('beir/nfcorpus')
-doc = loader.get_doc('MED-10')
-query = loader.get_query('PLAIN-3')
+loader = DataLoader.load('beir/arguana')
+
+doc = loader.get_doc(['did'])
+print(doc)
+
+query = loader.get_query('[qid]')
+print(query)
+
+qrel = loader.get_qrel('[mode]', '[qid]')
+print(qrel)
 ```
 
 ## Utils
 ### CorpusReader
 - How to build and load index
 ```py
 from hamu_tool.utils import CorpusReader
 
 CorpusReader.build_index('data_file.jsonl', 'index_file.idx')
 reader = CorpusReader('index_file.idx')
 print(reader[0]) # get document by index
-print(reader['doc_id']) # get document by id
+print(reader['[did]']) # get document by id
 ```
 - Format of `data_file.jsonl`: each line of `data_file.jsonl` should be a dictionary
 ```json
 {"id": "doc_1", "text": "doc_text_1"}
 ```
-
-### BIBExtractor
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/arguana_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/arguana_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return instance
 
     def get_docs(self) -> Iterator[ArguanaDocInstance]:
         for doc in self.reader_doc:
             instance = ArguanaDocInstance(id=doc['id'], text=doc['text'], title=doc['title'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[ArguanaQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[ArguanaQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(ArguanaQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/bioasq_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/bioasq_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return instance
 
     def get_docs(self) -> Iterator[BioASQDocInstance]:
         for doc in self.reader_doc:
             instance = BioASQDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], journal=doc['journal'], year=doc['year'], pmid=doc['pmid'], mesh_major=doc['mesh_major'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[BioASQQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[BioASQQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(BioASQQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/climate_fever_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/climate_fever_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return instance
 
     def get_docs(self) -> Iterator[ClimateFEVERDocInstance]:
         for doc in self.reader_doc:
             instance = ClimateFEVERDocInstance(id=doc['id'], text=doc['text'], title=doc['title'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[ClimateFEVERQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[ClimateFEVERQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(ClimateFEVERQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/data_loader.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/data_loader_base.py` & `hamu-tool-0.0.8/hamu_tool/dataset/data_loader_base.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/dbpedia_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/dbpedia_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return instance
 
     def get_docs(self) -> Iterator[DBPediaDocInstance]:
         for doc in self.reader_doc:
             instance = DBPediaDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], url=doc['url'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[DBPediaQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[DBPediaQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(DBPediaQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/fever_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/fever_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return instance
 
     def get_docs(self) -> Iterator[FEVERDocInstance]:
         for doc in self.reader_doc:
             instance = FEVERDocInstance(id=doc['id'], text=doc['text'], title=doc['title'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[FEVERQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[FEVERQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(FEVERQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/fiqa_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/fiqa_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return instance
 
     def get_docs(self) -> Iterator[FiQADocInstance]:
         for doc in self.reader_doc:
             instance = FiQADocInstance(id=doc['id'], text=doc['text'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[FiQAQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[FiQAQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(FiQAQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/hotpotqa_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/hotpotqa_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return instance
 
     def get_docs(self) -> Iterator[HotpotQADocInstance]:
         for doc in self.reader_doc:
             instance = HotpotQADocInstance(id=doc['id'], text=doc['text'], title=doc['title'], url=doc['url'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[HotpotQAQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[HotpotQAQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(HotpotQAQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/msmarco_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/msmarco_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return instance
 
     def get_docs(self) -> Iterator[MSMARCODocInstance]:
         for doc in self.reader_doc:
             instance = MSMARCODocInstance(id=doc['id'], text=doc['text'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[MSMARCOQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[MSMARCOQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(MSMARCOQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/nfcorpus_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/nfcorpus_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return instance
 
     def get_docs(self) -> Iterator[NFCorpusDocInstance]:
         for doc in self.reader_doc:
             instance = NFCorpusDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], url=doc['url'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[NFCorpusQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[NFCorpusQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(NFCorpusQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/nq_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/nq_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return instance
 
     def get_docs(self) -> Iterator[NQDocInstance]:
         for doc in self.reader_doc:
             instance = NQDocInstance(id=doc['id'], text=doc['text'], title=doc['title'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[NQQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[NQQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(NQQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/quora_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/quora_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return instance
 
     def get_docs(self) -> Iterator[QuoraDocInstance]:
         for doc in self.reader_doc:
             instance = QuoraDocInstance(id=doc['id'], text=doc['text'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[QuoraQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[QuoraQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(QuoraQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/robust04_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/robust04_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return instance
 
     def get_docs(self) -> Iterator[Robust04DocInstance]:
         for doc in self.reader_doc:
             instance = Robust04DocInstance(id=doc['id'], text=doc['text'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[Robust04QrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[Robust04QrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(Robust04QrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/scidocs_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/scidocs_data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return instance
 
     def get_docs(self) -> Iterator[SciDocsDocInstance]:
         for doc in self.reader_doc:
             instance = SciDocsDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], year=doc['year'], authors=doc['authors'], cited_by=doc['cited_by'], references=doc['references'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[SciDocsQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[SciDocsQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(SciDocsQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/scifact_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/scifact_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return instance
 
     def get_docs(self) -> Iterator[SciFactDocInstance]:
         for doc in self.reader_doc:
             instance = SciFactDocInstance(id=doc['id'], text=doc['text'], title=doc['title'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[SciFactQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[SciFactQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(SciFactQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/signal1m_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/signal1m_data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return instance
 
     def get_docs(self) -> Iterator[Signal1MDocInstance]:
         for doc in self.reader_doc:
             instance = Signal1MDocInstance(id=doc['id'], text=doc['text'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[Signal1MQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[Signal1MQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(Signal1MQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/touche_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/touche_data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return instance
 
     def get_docs(self) -> Iterator[ToucheDocInstance]:
         for doc in self.reader_doc:
             instance = ToucheDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], stance=doc['stance'], url=doc['url'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[ToucheQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[ToucheQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(ToucheQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/touche_v2_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/touche_v2_data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return instance
 
     def get_docs(self) -> Iterator[Touchev2DocInstance]:
         for doc in self.reader_doc:
             instance = Touchev2DocInstance(id=doc['id'], text=doc['text'], title=doc['title'], stance=doc['stance'], url=doc['url'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[Touchev2QrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[Touchev2QrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(Touchev2QrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/trec_covid_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/trec_covid_data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return instance
 
     def get_docs(self) -> Iterator[TrecCovidDocInstance]:
         for doc in self.reader_doc:
             instance = TrecCovidDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], url=doc['url'], pubmed_id=doc['pubmed_id'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[TrecCovidQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[TrecCovidQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(TrecCovidQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/dataset/trec_news_data_loader.py` & `hamu-tool-0.0.8/hamu_tool/dataset/trec_news_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return instance
 
     def get_docs(self) -> Iterator[TrecNewsDocInstance]:
         for doc in self.reader_doc:
             instance = TrecNewsDocInstance(id=doc['id'], text=doc['text'], title=doc['title'], url=doc['url'], author=doc['author'], type=doc['type'], source=doc['source'], published_date=doc['published_date'])
             yield instance
 
-    def get_qrel(self, qid : str, mode : str) -> list[TrecNewsQrelInstance]:
+    def get_qrel(self, mode : str, qid : str) -> list[TrecNewsQrelInstance]:
         if qid not in self.qrel[mode]:
             raise KeyError(f'Qrel for query [{qid}] not found')
         instances = []
         for did, score in self.qrel[mode][qid]:
             instances.append(TrecNewsQrelInstance(qid=qid, did=did, score=score))
         return instances
```

### Comparing `hamu-tool-0.0.7/hamu_tool/utils/bib_extractor.py` & `hamu-tool-0.0.8/hamu_tool/utils/bib_extractor.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/hamu_tool/utils/corpus_reader.py` & `hamu-tool-0.0.8/hamu_tool/utils/corpus_reader.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/hamu_tool/utils/pprint.py` & `hamu-tool-0.0.8/hamu_tool/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/hamu_tool.egg-info/SOURCES.txt` & `hamu-tool-0.0.8/hamu_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.7/setup.py` & `hamu-tool-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hamu-tool',
-    version='0.0.7',
+    version='0.0.8',
     description='Many useful tools for computer scientists!',
     license='MIT',
     author='DoHyeon Lee',
     author_email='waylight3@snu.ac.kr',
     url='https://github.com/waylight3/hamu-tool',
     keywords=['hamu', 'tool', 'computer', 'science', 'useful', 'toolkit', 'library', 'python', 'package', 'module', 'utility', 'function', 'class', 'method'],
     install_requires=['unidecode >= 1.2.0'],
```

