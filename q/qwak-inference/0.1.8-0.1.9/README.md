# Comparing `tmp/qwak_inference-0.1.8.tar.gz` & `tmp/qwak_inference-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.8.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.9.tar", max compression
```

## Comparing `qwak_inference-0.1.8.tar` & `qwak_inference-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10480 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/LICENSE
--rw-r--r--   0        0        0      267 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/README.md
--rw-r--r--   0        0        0     2192 2023-08-07 12:40:43.624905 qwak_inference-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      804 2023-08-07 12:40:43.624905 qwak_inference-0.1.8/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    26621 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0     1497 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/instance_validation.py
--rw-r--r--   0        0        0     1300 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4811 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     2346 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 qwak_inference-0.1.8/setup.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 qwak_inference-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-10-05 06:45:06.089196 qwak_inference-0.1.9/LICENSE
+-rw-r--r--   0        0        0      267 2023-10-05 06:45:06.089196 qwak_inference-0.1.9/README.md
+-rw-r--r--   0        0        0     2192 2023-10-05 06:45:58.197576 qwak_inference-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-10-05 06:45:58.197576 qwak_inference-0.1.9/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    26621 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0     1497 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/batch_client/instance_validation.py
+-rw-r--r--   0        0        0     1300 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4961 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     2346 2023-10-05 06:45:06.093196 qwak_inference-0.1.9/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 qwak_inference-0.1.9/setup.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 qwak_inference-0.1.9/PKG-INFO
```

### Comparing `qwak_inference-0.1.8/LICENSE` & `qwak_inference-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/pyproject.toml` & `qwak_inference-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.8"
+version = "0.1.9"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qwak_inference-0.1.8/qwak_inference/__init__.py` & `qwak_inference-0.1.9/qwak_inference/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `qwak_inference-0.1.8/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.9/qwak_inference/batch_client/batch_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.9/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/batch_client/instance_validation.py` & `qwak_inference-0.1.9/qwak_inference/batch_client/instance_validation.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.9/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/configuration/account.py` & `qwak_inference-0.1.9/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.9/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/configuration/session.py` & `qwak_inference-0.1.9/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/constants.py` & `qwak_inference-0.1.9/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/exceptions.py` & `qwak_inference-0.1.9/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/feedback_client.py` & `qwak_inference-0.1.9/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.9/qwak_inference/realtime_client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,28 +50,30 @@
         )
 
     def predict(
         self,
         feature_vectors,
         output_format=InferenceOutputFormat.DICTIONARY,
         metadata: dict = {},
+        orient: str = "split",
     ):
         """
         Perform a prediction request against a Qwak based model
 
         :param feature_vectors: A list of feature vectors to predict against. Each feature vector is modeled as a python
          dictionary, or a pandas Dataframe
         :param output_format: A list of feature vectors to predict against. Each feature vector is modeled as a python
          dictionary, or a pandas Dataframe
         :param metadata: metadata to split traffic based on
         :return: Prediction response from the model
+        :param orient: The format of the JSON string. Default is 'split'. See pandas.DataFrame.to_json for more details
         """
 
         if feature_vectors.__class__.__name__ == "DataFrame":
-            feature_vectors = feature_vectors.to_json(orient="split")
+            feature_vectors = feature_vectors.to_json(orient=orient)
 
         if isinstance(feature_vectors, dict) or isinstance(feature_vectors, list):
             feature_vectors = json.dumps(feature_vectors)
 
         try:
             rule_based_traffic = {}
             if metadata:
```

### Comparing `qwak_inference-0.1.8/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.9/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.8/setup.py` & `qwak_inference-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'feedback:python_version >= "3.10"': ['qwak-core>=0.0.147',
                                        'qwak-core>=0.0.147'],
  'feedback:python_version >= "3.8" and python_version < "3.12"': ['pandas>=1.4.0',
                                                                   'pandas>=1.4.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.1.8/PKG-INFO` & `qwak_inference-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.8
+Version: 0.1.9
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

