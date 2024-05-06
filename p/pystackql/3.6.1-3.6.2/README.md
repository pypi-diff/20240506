# Comparing `tmp/pystackql-3.6.1.tar.gz` & `tmp/pystackql-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.6.1.tar", last modified: Wed Apr 17 22:49:02 2024, max compression
+gzip compressed data, was "pystackql-3.6.2.tar", last modified: Mon May  6 03:06:40 2024, max compression
```

## Comparing `pystackql-3.6.1.tar` & `pystackql-3.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 22:49:02.416126 pystackql-3.6.1/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.6.1/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 22:49:02.397527 pystackql-3.6.1/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5198 2024-04-17 21:43:36.000000 pystackql-3.6.1/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 22:49:02.049591 pystackql-3.6.1/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.6.1/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.6.1/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.6.1/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.6.1/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.6.1/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    27161 2024-04-17 22:22:26.000000 pystackql-3.6.1/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 22:49:02.368879 pystackql-3.6.1/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 22:49:01.000000 pystackql-3.6.1/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 22:49:01.000000 pystackql-3.6.1/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 22:49:01.000000 pystackql-3.6.1/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 22:49:01.000000 pystackql-3.6.1/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 22:49:01.000000 pystackql-3.6.1/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 22:49:02.419138 pystackql-3.6.1/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 22:24:06.000000 pystackql-3.6.1/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 22:49:02.314582 pystackql-3.6.1/tests/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.6.1/tests/test_params.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-06 03:06:40.418200 pystackql-3.6.2/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.6.2/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-05-06 03:06:40.399609 pystackql-3.6.2/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5198 2024-05-06 01:28:47.000000 pystackql-3.6.2/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-06 03:06:40.060374 pystackql-3.6.2/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.6.2/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.6.2/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.6.2/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.6.2/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.6.2/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    27337 2024-05-06 01:27:13.000000 pystackql-3.6.2/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-06 03:06:40.371990 pystackql-3.6.2/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-05-06 03:06:39.000000 pystackql-3.6.2/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-05-06 03:06:39.000000 pystackql-3.6.2/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-05-06 03:06:39.000000 pystackql-3.6.2/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-05-06 03:06:39.000000 pystackql-3.6.2/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-05-06 03:06:39.000000 pystackql-3.6.2/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-05-06 03:06:40.420207 pystackql-3.6.2/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-05-06 01:28:47.000000 pystackql-3.6.2/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-06 03:06:40.314745 pystackql-3.6.2/tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2299 2024-05-06 02:34:06.000000 pystackql-3.6.2/tests/test_params.py
```

### Comparing `pystackql-3.6.1/LICENSE` & `pystackql-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.6.1/PKG-INFO` & `pystackql-3.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.6.1
+Version: 3.6.2
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.2.tar.gz
```

### Comparing `pystackql-3.6.1/README.rst` & `pystackql-3.6.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -190,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.2.tar.gz
```

### Comparing `pystackql-3.6.1/pystackql/_util.py` & `pystackql-3.6.2/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.6.1/pystackql/base_stackql_magic.py` & `pystackql-3.6.2/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.6.1/pystackql/magic.py` & `pystackql-3.6.2/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.6.1/pystackql/magics.py` & `pystackql-3.6.2/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.6.1/pystackql/stackql.py` & `pystackql-3.6.2/pystackql/stackql.py`

 * *Files 2% similar despite different names*

```diff
@@ -510,15 +510,19 @@
 			message = result["error"]
 
 			if self.output == 'pandas':
 				return pd.DataFrame({'message': [message]}) if message else pd.DataFrame({'message': []})
 			elif self.output == 'csv':
 				return message
 			else:
-				return {'message': message}			
+				# count number of rows in the message
+				try:
+					return {'message': message, 'rowsaffected': message.count('\n')}
+				except Exception as e:
+					return {'message': message, 'rowsaffected': 0}							
 	
 	def execute(self, query, suppress_errors=True):
 		"""
 		Executes a StackQL query and returns the output based on the specified output format.
 
 		This method supports execution both in server mode and locally using subprocess. In server mode,
 		the query is sent to a StackQL server, while in local mode, it runs the query using a local binary.
```

### Comparing `pystackql-3.6.1/pystackql.egg-info/PKG-INFO` & `pystackql-3.6.2/pystackql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.6.1
+Version: 3.6.2
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload --config-file .pypirc dist/pystackql-3.6.0.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.6.2.tar.gz
```

### Comparing `pystackql-3.6.1/setup.py` & `pystackql-3.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.6.1',
+    version='3.6.2',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

### Comparing `pystackql-3.6.1/tests/test_params.py` & `pystackql-3.6.2/tests/test_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         'darwin': '/tmp',
         'linux': '/tmp'
     }
     return custom_download_dirs.get(platform_name, '/tmp')
 
 registry_pull_google_query = "REGISTRY PULL google"
 registry_pull_aws_query = "REGISTRY PULL aws"
-registry_pull_awscc_query = "REGISTRY PULL awscc"
 registry_pull_okta_query = "REGISTRY PULL okta"
 registry_pull_github_query = "REGISTRY PULL github"
 
 def registry_pull_resp_pattern(provider):
     return r"%s provider, version 'v\d+\.\d+\.\d+' successfully installed\s*" % provider
 
 google_query = f"""
@@ -40,25 +39,25 @@
 WHERE project = '{os.environ['GCP_PROJECT']}' 
 AND zone = '{os.environ['GCP_ZONE']}'
 GROUP BY status
 """
 
 aws_query = f"""
 SELECT 
-SPLIT_PART(CreationDate, '-', 1) as year, count(*) as num_buckets FROM aws.s3.buckets
+SPLIT_PART(CreationDate, '-', 1) as year, count(*) as num_buckets FROM aws.s3_api.buckets
 WHERE region = 'us-east-1'
 GROUP BY year
 """
 
 regions = os.environ.get('AWS_REGIONS').split(',')
 
 async_queries = [
     f"""
     SELECT region, COUNT(*) as num_functions
-    FROM awscc.lambda.functions
+    FROM aws.lambda.functions
     WHERE region = '{region}'
     """
     for region in regions
 ]
 
 def print_test_result(test_name, condition=True, server_mode=False, is_ipython=False):
     status_header = colored("[PASSED] ", 'green') if condition else colored("[FAILED] ", 'red')
```

