# Comparing `tmp/ARS_Test_Runner-0.1.9.tar.gz` & `tmp/ARS_Test_Runner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARS_Test_Runner-0.1.9.tar", last modified: Mon Apr 15 20:18:51 2024, max compression
+gzip compressed data, was "ARS_Test_Runner-0.2.0.tar", last modified: Mon May  6 16:25:42 2024, max compression
```

## Comparing `ARS_Test_Runner-0.1.9.tar` & `ARS_Test_Runner-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 20:18:51.134811 ARS_Test_Runner-0.1.9/
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 20:18:51.128840 ARS_Test_Runner-0.1.9/ARS_Test_Runner/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/__init__.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/cli.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22753 2024-04-15 20:05:42.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/semantic_test.py
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 20:18:51.133477 ARS_Test_Runner-0.1.9/ARS_Test_Runner/templates/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/templates/affects_creative.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/templates/treats.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner/templates/treats_creative.json
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 20:18:51.133956 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/SOURCES.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/dependency_links.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/entry_points.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/requires.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-15 20:18:50.000000 ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/top_level.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.9/LICENSE.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-15 20:18:51.134533 ARS_Test_Runner-0.1.9/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.9/README.md
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-15 20:18:51.135472 ARS_Test_Runner-0.1.9/setup.cfg
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-15 20:04:04.000000 ARS_Test_Runner-0.1.9/setup.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.363081 ARS_Test_Runner-0.2.0/
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.355103 ARS_Test_Runner-0.2.0/ARS_Test_Runner/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/__init__.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/cli.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22749 2024-05-06 13:56:31.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/semantic_test.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.360930 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/affects_creative.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/treats.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/treats_creative.json
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-05-06 16:25:42.361897 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-05-06 16:25:42.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/SOURCES.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/dependency_links.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/entry_points.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/requires.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-05-06 16:25:41.000000 ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/top_level.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.2.0/LICENSE.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-05-06 16:25:42.362730 ARS_Test_Runner-0.2.0/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.2.0/README.md
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-05-06 16:25:42.364063 ARS_Test_Runner-0.2.0/setup.cfg
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-05-06 16:23:19.000000 ARS_Test_Runner-0.2.0/setup.py
```

### Comparing `ARS_Test_Runner-0.1.9/ARS_Test_Runner/cli.py` & `ARS_Test_Runner-0.2.0/ARS_Test_Runner/cli.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.9/ARS_Test_Runner/semantic_test.py` & `ARS_Test_Runner-0.2.0/ARS_Test_Runner/semantic_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 parser = argparse.ArgumentParser(description='Semantic Smoke Test')
 parser.add_argument('--env', help='environment to run the analysis on', default='ci')
 parser.add_argument('--predicate',help='predicate',default='treats', type=str)
 parser.add_argument('--runner_setting', help='creative mode indicator',nargs="*", type=str )
 parser.add_argument('--expected_output', help="[TopAnswer'|'Acceptable'|'BadButForgivable'|'NeverShow']",nargs="*", type=str)
 parser.add_argument('--biolink_object_aspect_qualifier', help='activity_or_abundance', type=str, default='')
 parser.add_argument('--biolink_object_direction_qualifier', help='increased/decreased', type=str,default='')
-parser.add_argument('--input_category', help='Gene/Chemical', type=str, default='biolink:Disease')
+parser.add_argument('--input_category', help='Gene/ChemicalEntity', type=str, default='biolink:Disease')
 parser.add_argument('--input_curie', help='Input Curie', type=str)
 parser.add_argument('--output_curie', help='output Curie', nargs="*", type=str)
 
 env_spec = {
     'dev': 'ars-dev',
     'ci': 'ars.ci',
     'test': 'ars.test',
@@ -193,15 +193,15 @@
             report_card['results'].append(report)
     return report_card
 
 async def pass_fail_analysis(report: Dict[str,any], agent: str, results: List[Dict[str,any]], out_curie: str, expect_output: str):
     """" function to run pass fail analysis on individual results"""
     #get the top_n result's ids
     try:
-        res_sort = sorted(results, key=lambda x: x['normalized_score'], reverse=True)
+        res_sort = sorted(results, key=lambda x: x['sugeno'], reverse=True)
         all_ids=[]
         for res in res_sort:
             for res_node, res_value in res["node_bindings"].items():
                 for val in res_value:
                     ids = str(val["id"])
                     if ids not in all_ids:
                         all_ids.append(ids)
```

### Comparing `ARS_Test_Runner-0.1.9/ARS_Test_Runner/templates/affects_creative.json` & `ARS_Test_Runner-0.2.0/ARS_Test_Runner/templates/affects_creative.json`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.9/ARS_Test_Runner.egg-info/PKG-INFO` & `ARS_Test_Runner-0.2.0/ARS_Test_Runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS-Test-Runner
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.9/LICENSE.txt` & `ARS_Test_Runner-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.9/PKG-INFO` & `ARS_Test_Runner-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS_Test_Runner
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.9/README.md` & `ARS_Test_Runner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.9/setup.py` & `ARS_Test_Runner-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from semantic_release import setup_hook
     setup_hook(sys.argv)
 except ImportError:
     pass
 
-__version__='0.1.9'
+__version__='0.2.0'
 setup(
     name="ARS_Test_Runner",
     version= __version__,
     description="Python package for ARS pass/fail test",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Shervin Abdollahi, Mark Williams",
```

