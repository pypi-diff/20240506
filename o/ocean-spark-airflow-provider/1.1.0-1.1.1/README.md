# Comparing `tmp/ocean_spark_airflow_provider-1.1.0.tar.gz` & `tmp/ocean_spark_airflow_provider-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean_spark_airflow_provider-1.1.0.tar", max compression
+gzip compressed data, was "ocean_spark_airflow_provider-1.1.1.tar", max compression
```

## Comparing `ocean_spark_airflow_provider-1.1.0.tar` & `ocean_spark_airflow_provider-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      578 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/LICENSE
--rw-r--r--   0        0        0     3483 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/README.md
--rw-r--r--   0        0        0     1553 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/__init__.py
--rw-r--r--   0        0        0      665 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/application_state.py
--rw-r--r--   0        0        0        0 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/__init__.py
--rw-r--r--   0        0        0     3179 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/hook.py
--rw-r--r--   0        0        0     4601 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/inverse_websockify.py
--rw-r--r--   0        0        0     2690 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/operator.py
--rw-r--r--   0        0        0      805 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/extra_links.py
--rw-r--r--   0        0        0     6679 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/hooks.py
--rw-r--r--   0        0        0     6316 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/operators.py
--rw-r--r--   0        0        0     1150 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/plugins.py
--rw-r--r--   0        0        0      487 2024-01-29 13:50:04.549337 ocean_spark_airflow_provider-1.1.0/ocean_spark/response.py
--rw-r--r--   0        0        0     1455 2024-01-29 13:50:11.561390 ocean_spark_airflow_provider-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 ocean_spark_airflow_provider-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3483 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/README.md
+-rw-r--r--   0        0        0     1553 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/application_state.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/__init__.py
+-rw-r--r--   0        0        0     3179 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/hook.py
+-rw-r--r--   0        0        0     4601 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/inverse_websockify.py
+-rw-r--r--   0        0        0     2690 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/operator.py
+-rw-r--r--   0        0        0      805 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/extra_links.py
+-rw-r--r--   0        0        0     7447 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/hooks.py
+-rw-r--r--   0        0        0     6420 2024-05-06 17:10:22.274313 ocean_spark_airflow_provider-1.1.1/ocean_spark/operators.py
+-rw-r--r--   0        0        0     1150 2024-05-06 17:10:22.278313 ocean_spark_airflow_provider-1.1.1/ocean_spark/plugins.py
+-rw-r--r--   0        0        0      487 2024-05-06 17:10:22.278313 ocean_spark_airflow_provider-1.1.1/ocean_spark/response.py
+-rw-r--r--   0        0        0     1455 2024-05-06 17:10:30.266353 ocean_spark_airflow_provider-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 ocean_spark_airflow_provider-1.1.1/PKG-INFO
```

### Comparing `ocean_spark_airflow_provider-1.1.0/LICENSE` & `ocean_spark_airflow_provider-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/README.md` & `ocean_spark_airflow_provider-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/__init__.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/application_state.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/application_state.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/hook.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/hook.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/inverse_websockify.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/inverse_websockify.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/connect/operator.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/connect/operator.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/extra_links.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/extra_links.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/hooks.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from datetime import timedelta
-from typing import Callable, Dict, Any
+from typing import Callable, Dict, Any, Tuple
 
 
 from airflow.hooks.base import BaseHook
 
 from airflow import __version__
 from airflow.exceptions import AirflowException
 
@@ -15,14 +15,19 @@
 from requests import exceptions as requests_exceptions
 
 from ocean_spark.response import ApiResponse
 
 API_HOST = "https://api.spotinst.io/ocean/spark/"
 FE_HOST = "https://console.spotinst.com/ocean/spark/"
 
+GET_CLUSTER_ENDPOINT = (
+    requests.get,
+    urljoin(API_HOST, "cluster/{cluster_id}"),
+)
+
 SUBMIT_APP_ENDPOINT = (
     requests.post,
     urljoin(API_HOST, "cluster/{cluster_id}/app"),
 )
 GET_APP_ENDPOINT = (
     requests.get,
     urljoin(API_HOST, "cluster/{cluster_id}/app/{app_id}"),
@@ -77,16 +82,14 @@
             this function returns the response in JSON. Otherwise,
             we throw an AirflowException.
         :rtype: dict
         """
 
         if payload is None:
             payload = {}
-        if payload is None:
-            payload = {}
         headers = {**USER_AGENT_HEADER, "Authorization": f"Bearer {self.token}"}
 
         attempt_num = 1
         while True:
             try:
                 response = method(
                     endpoint,
@@ -173,14 +176,36 @@
 
     def get_app_page_url(self, app_id: str) -> str:
         return urljoin(
             FE_HOST,
             f"apps/clusters/{self.cluster_id}/apps/{app_id}/overview&accountId={self.account_id}",
         )
 
+    def test_connection(self) -> Tuple[bool, str]:
+        method, path = GET_CLUSTER_ENDPOINT
+        try:
+            response = self._do_api_call(
+                method,
+                path.format(
+                    cluster_id=self.cluster_id,
+                ),
+                {},
+            )
+            if response["response"]["items"][0]["state"] not in [
+                "AVAILABLE",
+                "PROGRESSING",
+            ]:
+                return (
+                    False,
+                    f"Cluster state is {response['response']['items'][0]['state']}",
+                )
+            return True, "Connection successful"
+        except AirflowException as e:
+            return False, str(e)
+
     @staticmethod
     def get_ui_field_behaviour() -> Dict:
         return {
             "hidden_fields": ["port", "extra", "schema"],
             "relabeling": {
                 "password": "API token",
                 "host": "Cluster id",
```

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/operators.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,21 @@
             self.payload["appId"] = self._payload_app_id
         if self.config_template_id is not None:
             self.payload["configTemplateId"] = self.config_template_id
 
         # templated config overrides dict pulled from xcom is a json str
         if self.config_overrides is not None:
             if isinstance(self.config_overrides, str):
-                # json standard requires double quotes
-                self.config_overrides = json.loads(
-                    self.config_overrides.replace("'", '"')
-                )
+                try:
+                    self.config_overrides = json.loads(self.config_overrides)
+                except json.JSONDecodeError as e:
+                    raise AirflowException(
+                        f"Failed to parse config_overrides as JSON: {e}"
+                    )
+
             self.payload["configOverrides"] = self.config_overrides
 
     def execute(self, context: "Context") -> None:
         self._build_payload()
         hook = self._get_hook()
         self.app_id = hook.submit_app(self.payload)
         if self.on_spark_submit_callback:
```

### Comparing `ocean_spark_airflow_provider-1.1.0/ocean_spark/plugins.py` & `ocean_spark_airflow_provider-1.1.1/ocean_spark/plugins.py`

 * *Files identical despite different names*

### Comparing `ocean_spark_airflow_provider-1.1.0/pyproject.toml` & `ocean_spark_airflow_provider-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocean-spark-airflow-provider"
-version = "1.1.0"
+version = "1.1.1"
 description = "Apache Airflow connector for Ocean for Apache Spark"
 authors = ["Ocean for Apache Spark authors <clement.rezvoy@netapp.com>" ]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://spot.io/products/ocean-apache-spark/"
 repository = "https://github.com/spotinst/ocean-spark-airflow-provider"
 keywords = ["airflow", "provider", "spark", "ocean"]
```

### Comparing `ocean_spark_airflow_provider-1.1.0/PKG-INFO` & `ocean_spark_airflow_provider-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-spark-airflow-provider
-Version: 1.1.0
+Version: 1.1.1
 Summary: Apache Airflow connector for Ocean for Apache Spark
 Home-page: https://spot.io/products/ocean-apache-spark/
 License: Apache-2.0
 Keywords: airflow,provider,spark,ocean
 Author: Ocean for Apache Spark authors
 Author-email: clement.rezvoy@netapp.com
 Requires-Python: >=3.7,<4.0
```

