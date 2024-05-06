# Comparing `tmp/captureflow_agent-0.0.6.tar.gz` & `tmp/captureflow_agent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captureflow_agent-0.0.6.tar", last modified: Mon May  6 08:52:12 2024, max compression
+gzip compressed data, was "captureflow_agent-0.0.7.tar", last modified: Mon May  6 09:13:26 2024, max compression
```

## Comparing `captureflow_agent-0.0.6.tar` & `captureflow_agent-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.605311 captureflow_agent-0.0.6/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:52:12.604901 captureflow_agent-0.0.6/PKG-INFO
--rw-r--r--   0 nikitakutc   (501) staff       (20)     2528 2024-04-02 15:22:49.000000 captureflow_agent-0.0.6/README.md
--rw-r--r--   0 nikitakutc   (501) staff       (20)      768 2024-05-06 08:52:07.000000 captureflow_agent-0.0.6/pyproject.toml
--rw-r--r--   0 nikitakutc   (501) staff       (20)       38 2024-05-06 08:52:12.605398 captureflow_agent-0.0.6/setup.cfg
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.598816 captureflow_agent-0.0.6/src/
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.600169 captureflow_agent-0.0.6/src/captureflow/
--rw-r--r--   0 nikitakutc   (501) staff       (20)        0 2024-03-22 22:30:50.000000 captureflow_agent-0.0.6/src/captureflow/__init__.py
--rw-r--r--   0 nikitakutc   (501) staff       (20)     7258 2024-05-06 08:50:51.000000 captureflow_agent-0.0.6/src/captureflow/tracer.py
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.604447 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/PKG-INFO
--rw-r--r--   0 nikitakutc   (501) staff       (20)      331 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/SOURCES.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)        1 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/dependency_links.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)       86 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/requires.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)       12 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/top_level.txt
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.604043 captureflow_agent-0.0.6/tests/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3007 2024-05-01 13:37:39.000000 captureflow_agent-0.0.6/tests/test_fastapi_tracer.py
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 09:13:26.765944 captureflow_agent-0.0.7/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 09:13:26.765226 captureflow_agent-0.0.7/PKG-INFO
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     2528 2024-04-02 15:22:49.000000 captureflow_agent-0.0.7/README.md
+-rw-r--r--   0 nikitakutc   (501) staff       (20)      768 2024-05-06 09:13:12.000000 captureflow_agent-0.0.7/pyproject.toml
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       38 2024-05-06 09:13:26.766056 captureflow_agent-0.0.7/setup.cfg
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 09:13:26.759355 captureflow_agent-0.0.7/src/
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 09:13:26.761053 captureflow_agent-0.0.7/src/captureflow/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)        0 2024-03-22 22:30:50.000000 captureflow_agent-0.0.7/src/captureflow/__init__.py
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     7361 2024-05-06 09:13:03.000000 captureflow_agent-0.0.7/src/captureflow/tracer.py
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 09:13:26.764429 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 09:13:26.000000 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/PKG-INFO
+-rw-r--r--   0 nikitakutc   (501) staff       (20)      331 2024-05-06 09:13:26.000000 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)        1 2024-05-06 09:13:26.000000 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       86 2024-05-06 09:13:26.000000 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/requires.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       12 2024-05-06 09:13:26.000000 captureflow_agent-0.0.7/src/captureflow_agent.egg-info/top_level.txt
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 09:13:26.763931 captureflow_agent-0.0.7/tests/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3007 2024-05-01 13:37:39.000000 captureflow_agent-0.0.7/tests/test_fastapi_tracer.py
```

### Comparing `captureflow_agent-0.0.6/PKG-INFO` & `captureflow_agent-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captureflow-agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data collector to unleash LLM power
 Author-email: Nikita Kuts <me@nikitakuts.com>
 Project-URL: homepage, https://captureflow.dev/
 Project-URL: repository, https://github.com/CaptureFlow/captureflow-py
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
```

### Comparing `captureflow_agent-0.0.6/README.md` & `captureflow_agent-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `captureflow_agent-0.0.6/pyproject.toml` & `captureflow_agent-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = { find = { where = ["src"], exclude = ["tests", "examples"] } }
 
 [project]
 name = "captureflow-agent"
-version = "0.0.6"
+version = "0.0.7"
 description = "Data collector to unleash LLM power"
 authors = [
     {name = "Nikita Kuts", email = "me@nikitakuts.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `captureflow_agent-0.0.6/src/captureflow/tracer.py` & `captureflow_agent-0.0.7/src/captureflow/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,22 @@
     def _send_trace_log(self, context: Dict[str, Any]) -> None:
         if os.environ.get("CAPTUREFLOW_DEV_SERVER") == "true":
             log_filename = f"trace_{context['invocation_id']}.json"
             with open(log_filename, "w") as f:
                 json.dump(context, f, indent=4)
 
         try:
+            logger.error("WE ARE SENDING REQUEST YYEEE")
             response = requests.post(
                 self.trace_endpoint_url,
                 params={"repository-url": self.repo_url},  # TODO: move param to HTTP body
                 json=context,
                 headers={"Content-Type": "application/json"},
             )
+            logger.error("REQUEST FINISHED ")
             if response.status_code != 200:
                 logger.info(f"CaptureFlow server responded: {response.status_code}")
         except Exception as e:
             logger.info(f"Exception during logging: {e}")
 
     def _serialize_variable(self, value: Any) -> Dict[str, Any]:
         try:
```

### Comparing `captureflow_agent-0.0.6/src/captureflow_agent.egg-info/PKG-INFO` & `captureflow_agent-0.0.7/src/captureflow_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captureflow-agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: Data collector to unleash LLM power
 Author-email: Nikita Kuts <me@nikitakuts.com>
 Project-URL: homepage, https://captureflow.dev/
 Project-URL: repository, https://github.com/CaptureFlow/captureflow-py
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
```

### Comparing `captureflow_agent-0.0.6/tests/test_fastapi_tracer.py` & `captureflow_agent-0.0.7/tests/test_fastapi_tracer.py`

 * *Files identical despite different names*

