# Comparing `tmp/qiskit_scaleway-0.1.7.tar.gz` & `tmp/qiskit_scaleway-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_scaleway-0.1.7.tar", last modified: Thu May  2 16:16:30 2024, max compression
+gzip compressed data, was "qiskit_scaleway-0.1.8.tar", last modified: Mon May  6 11:54:01 2024, max compression
```

## Comparing `qiskit_scaleway-0.1.7.tar` & `qiskit_scaleway-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.443006 qiskit_scaleway-0.1.7/
--rw-r--r--   0 bonnie     (501) staff       (20)    11357 2024-03-25 15:53:04.000000 qiskit_scaleway-0.1.7/LICENSE
--rw-r--r--   0 bonnie     (501) staff       (20)     3195 2024-05-02 16:16:30.442267 qiskit_scaleway-0.1.7/PKG-INFO
--rw-r--r--   0 bonnie     (501) staff       (20)     2805 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.7/README.md
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.431379 qiskit_scaleway-0.1.7/qiskit_scaleway/
--rw-r--r--   0 bonnie     (501) staff       (20)       39 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/__init__.py
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.438493 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/
--rw-r--r--   0 bonnie     (501) staff       (20)      178 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/__init__.py
--rw-r--r--   0 bonnie     (501) staff       (20)     5149 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/aer_backend.py
--rw-r--r--   0 bonnie     (501) staff       (20)     3504 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/aer_job.py
--rw-r--r--   0 bonnie     (501) staff       (20)     3076 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/qsim_backend.py
--rw-r--r--   0 bonnie     (501) staff       (20)     9781 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/qsim_job.py
--rw-r--r--   0 bonnie     (501) staff       (20)     2118 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/scaleway_backend.py
--rw-r--r--   0 bonnie     (501) staff       (20)     2041 2024-05-02 12:16:45.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/backends/scaleway_job.py
--rw-r--r--   0 bonnie     (501) staff       (20)     5135 2024-05-02 16:15:00.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/provider.py
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.439916 qiskit_scaleway-0.1.7/qiskit_scaleway/utils/
--rw-r--r--   0 bonnie     (501) staff       (20)       31 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/utils/__init__.py
--rw-r--r--   0 bonnie     (501) staff       (20)     4021 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.7/qiskit_scaleway/utils/client.py
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.433467 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/
--rw-r--r--   0 bonnie     (501) staff       (20)     3195 2024-05-02 16:16:30.000000 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/PKG-INFO
--rw-r--r--   0 bonnie     (501) staff       (20)      632 2024-05-02 16:16:30.000000 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/SOURCES.txt
--rw-r--r--   0 bonnie     (501) staff       (20)        1 2024-05-02 16:16:30.000000 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/dependency_links.txt
--rw-r--r--   0 bonnie     (501) staff       (20)      148 2024-05-02 16:16:30.000000 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/requires.txt
--rw-r--r--   0 bonnie     (501) staff       (20)       16 2024-05-02 16:16:30.000000 qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/top_level.txt
--rw-r--r--   0 bonnie     (501) staff       (20)       38 2024-05-02 16:16:30.443155 qiskit_scaleway-0.1.7/setup.cfg
--rw-r--r--   0 bonnie     (501) staff       (20)      545 2024-05-02 16:16:04.000000 qiskit_scaleway-0.1.7/setup.py
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:16:30.440926 qiskit_scaleway-0.1.7/test/
--rw-r--r--   0 bonnie     (501) staff       (20)     1041 2024-05-02 16:12:52.000000 qiskit_scaleway-0.1.7/test/test.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.8/LICENSE
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3000 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2805 2024-05-03 08:18:12.000000 qiskit_scaleway-0.1.8/README.md
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/__init__.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     5150 2024-05-06 11:30:47.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3077 2024-05-06 11:30:33.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2038 2024-05-06 11:32:05.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     5244 2024-05-06 11:30:00.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/provider.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     4019 2024-05-06 11:30:00.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/client.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3000 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      619 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      148 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/requires.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/top_level.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/setup.cfg
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      546 2024-05-06 11:53:18.000000 qiskit_scaleway-0.1.8/setup.py
```

### Comparing `qiskit_scaleway-0.1.7/LICENSE` & `qiskit_scaleway-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.7/PKG-INFO` & `qiskit_scaleway-0.1.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: qiskit_scaleway
-Version: 0.1.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: qiskit==1.0.2
-Requires-Dist: qiskit-aer==0.14.0.1
-Requires-Dist: randomname==0.2.1
-Requires-Dist: httpx==0.27.0
-Requires-Dist: dataclasses-json==0.6.4
-Requires-Dist: dataclasses==0.6
-Requires-Dist: pytimeparse==1.1.8
-Requires-Dist: python-dotenv==1.0.1
-
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
 To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
 
 More info on the [Quantum service web page](https://labs.scaleway.com/en/qaas/).
```

### Comparing `qiskit_scaleway-0.1.7/README.md` & `qiskit_scaleway-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: qiskit_scaleway
+Version: 0.1.8
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
 To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
 
 More info on the [Quantum service web page](https://labs.scaleway.com/en/qaas/).
@@ -85,7 +95,9 @@
 This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Reach us
 We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
+
+
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/aer_backend.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self._properties = None
         self._target = convert_to_target(
             self._configuration, self._properties, None, NAME_MAPPING
         )
         self._target.num_qubits = num_qubits
 
         # Set option validators
-        self.options.set_validator("shots", (1, 10000000))
+        self.options.set_validator("shots", (1, 100000000))
         self.options.set_validator("memory", bool)
 
     def __repr__(self) -> str:
         return f"<AerBackend(name={self.name},num_qubits={self.num_qubits},platform_id={self.id})>"
 
     @property
     def target(self):
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/aer_job.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/qsim_backend.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             availability=availability,
             version=version,
         )
 
         self._options = self._default_options()
 
         # Set option validators
-        self.options.set_validator("shots", (1, 10000000))
+        self.options.set_validator("shots", (1, 100000000))
 
         self._max_qubits = num_qubits
 
     def __repr__(self) -> str:
         return f"<QsimBackend(name={self.name},num_qubits={self.num_qubits},platform_id={self.id})>"
 
     @property
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/qsim_job.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/scaleway_backend.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,14 @@
     def id(self):
         return self._backend_id
 
     @property
     def availability(self):
         return self._availability
 
-    @property
-    def num_qubits(self) -> int:
-        return self._max_qubits
-
     def start_session(
         self,
         name: str = None,
         deduplication_id: str = None,
         max_duration: Union[int, str] = None,
         max_idle_duration: Union[int, str] = None,
     ) -> str:
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/backends/scaleway_job.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/provider.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 
     :param url: optional value, endpoint URL of the API, if the provided ``url`` is None, the value is loaded from the SCALEWAY_API_URL variables in the dotenv file or the QISKIT_SCALEWAY_API_URL environment variables, if no url is found, then ``_ENDPOINT_URL`` is used.
     """
 
     def __init__(
         self, project_id: str = None, secret_key: str = None, url: str = None
     ) -> None:
-        env_token = (
-            dotenv_values().get("QISKIT_SCALEWAY_API_TOKEN") or os.getenv("QISKIT_SCALEWAY_API_TOKEN")
+        env_token = dotenv_values().get("QISKIT_SCALEWAY_API_TOKEN") or os.getenv(
+            "QISKIT_SCALEWAY_API_TOKEN"
         )
-        env_project_id = (
-            dotenv_values().get("QISKIT_SCALEWAY_PROJECT_ID") or os.getenv("QISKIT_SCALEWAY_PROJECT_ID")
+        env_project_id = dotenv_values().get("QISKIT_SCALEWAY_PROJECT_ID") or os.getenv(
+            "QISKIT_SCALEWAY_PROJECT_ID"
         )
-        env_api_url = (
-            dotenv_values().get("QISKIT_SCALEWAY_API_URL") or os.getenv("QISKIT_SCALEWAY_API_URL")
+        env_api_url = dotenv_values().get("QISKIT_SCALEWAY_API_URL") or os.getenv(
+            "QISKIT_SCALEWAY_API_URL"
         )
 
         token = secret_key or env_token
         if token is None:
             raise Exception("secret_key is missing")
 
-
         project_id = project_id or env_project_id
         if project_id is None:
             raise Exception("project_id is missing")
 
         api_url = url or env_api_url or _ENDPOINT_URL
 
         self.__client = QaaSClient(url=api_url, token=token, project_id=project_id)
@@ -57,20 +56,19 @@
             list[ScalewayBackend]: a list of Backends that match the filtering
                 criteria.
         """
 
         scaleway_backends = []
         filters = {}
 
-        if (kwargs.get('operational') is not None):
-            filters["operational"] = kwargs.pop('operational', None)
-
-        if (kwargs.get('min_num_qubits') is not None):
-            filters["min_num_qubits"] = kwargs.pop('min_num_qubits', None)
+        if kwargs.get("operational") is not None:
+            filters["operational"] = kwargs.pop("operational", None)
 
+        if kwargs.get("min_num_qubits") is not None:
+            filters["min_num_qubits"] = kwargs.pop("min_num_qubits", None)
 
         json_resp = self.__client.list_platforms(name)
 
         for platform_dict in json_resp["platforms"]:
             name = platform_dict.get("name")
 
             backend = None
@@ -110,28 +108,34 @@
             scaleway_backends.append(backend)
 
         if filters is not None:
             scaleway_backends = self.filters(scaleway_backends, filters)
 
         return filter_backends(scaleway_backends, **kwargs)
 
-
     def _filter_availability(self, operational, availability):
-        availabilities = ['ailability_unknown','available', 'scarce'] if operational else ['shortage']
+        availabilities = (
+            ["ailability_unknown", "available", "scarce"]
+            if operational
+            else ["shortage"]
+        )
 
         return availability in availabilities
 
-    def filters(self, backends: list[ScalewayBackend], filters: dict) -> list[ScalewayBackend]:
+    def filters(
+        self, backends: list[ScalewayBackend], filters: dict
+    ) -> list[ScalewayBackend]:
         filtered_backends = []
-        operational = filters.get('operational')
-        min_num_qubits = filters.get('min_num_qubits')
-
+        operational = filters.get("operational")
+        min_num_qubits = filters.get("min_num_qubits")
 
         if operational is not None:
-            backends = [b for b in backends if self._filter_availability(operational, b.availability)]
-
+            backends = [
+                b
+                for b in backends
+                if self._filter_availability(operational, b.availability)
+            ]
 
         if min_num_qubits is not None:
             backends = [b for b in backends if b.num_qubits >= min_num_qubits]
 
-
         return backends
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway/utils/client.py` & `qiskit_scaleway-0.1.8/qiskit_scaleway/utils/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return {"X-Auth-Token": self.__token}
 
     def _build_endpoint(self, endpoint: str) -> str:
         return f"{self.__url}{endpoint}"
 
     def list_platforms(self, name: str) -> dict:
         filter_by_name = ""
-        if (name):
+        if name:
             filter_by_name = f"?name={name}"
 
         http_client = self._http_client()
         endpoint = f"{self._build_endpoint(_ENDPOINT_PLATFORM)}{filter_by_name}"
 
         resp = http_client.get(endpoint)
         resp.raise_for_status()
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/PKG-INFO` & `qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: qiskit-scaleway
-Version: 0.1.7
+Version: 0.1.8
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: qiskit==1.0.2
-Requires-Dist: qiskit-aer==0.14.0.1
-Requires-Dist: randomname==0.2.1
-Requires-Dist: httpx==0.27.0
-Requires-Dist: dataclasses-json==0.6.4
-Requires-Dist: dataclasses==0.6
-Requires-Dist: pytimeparse==1.1.8
-Requires-Dist: python-dotenv==1.0.1
 
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
 To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
 
@@ -99,7 +95,9 @@
 This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Reach us
 We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
+
+
```

### Comparing `qiskit_scaleway-0.1.7/qiskit_scaleway.egg-info/SOURCES.txt` & `qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 qiskit_scaleway/backends/aer_backend.py
 qiskit_scaleway/backends/aer_job.py
 qiskit_scaleway/backends/qsim_backend.py
 qiskit_scaleway/backends/qsim_job.py
 qiskit_scaleway/backends/scaleway_backend.py
 qiskit_scaleway/backends/scaleway_job.py
 qiskit_scaleway/utils/__init__.py
-qiskit_scaleway/utils/client.py
-test/test.py
+qiskit_scaleway/utils/client.py
```

### Comparing `qiskit_scaleway-0.1.7/setup.py` & `qiskit_scaleway-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="qiskit_scaleway",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
         "qiskit==1.0.2",
         "qiskit-aer==0.14.0.1",
         "randomname==0.2.1",
         "httpx==0.27.0",
         "dataclasses-json==0.6.4",
         "dataclasses==0.6",
         "pytimeparse==1.1.8",
-        "python-dotenv==1.0.1"
+        "python-dotenv==1.0.1",
     ],
     long_description=description,
     long_description_content_type="text/markdown",
 )
```

