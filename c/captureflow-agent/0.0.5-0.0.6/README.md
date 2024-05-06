# Comparing `tmp/captureflow_agent-0.0.5.tar.gz` & `tmp/captureflow_agent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captureflow_agent-0.0.5.tar", last modified: Mon May  6 08:30:37 2024, max compression
+gzip compressed data, was "captureflow_agent-0.0.6.tar", last modified: Mon May  6 08:52:12 2024, max compression
```

## Comparing `captureflow_agent-0.0.5.tar` & `captureflow_agent-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:30:37.247399 captureflow_agent-0.0.5/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:30:37.246863 captureflow_agent-0.0.5/PKG-INFO
--rw-r--r--   0 nikitakutc   (501) staff       (20)     2528 2024-04-02 15:22:49.000000 captureflow_agent-0.0.5/README.md
--rw-r--r--   0 nikitakutc   (501) staff       (20)      768 2024-05-06 08:29:48.000000 captureflow_agent-0.0.5/pyproject.toml
--rw-r--r--   0 nikitakutc   (501) staff       (20)       38 2024-05-06 08:30:37.247545 captureflow_agent-0.0.5/setup.cfg
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:30:37.241760 captureflow_agent-0.0.5/src/
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:30:37.243364 captureflow_agent-0.0.5/src/captureflow/
--rw-r--r--   0 nikitakutc   (501) staff       (20)        0 2024-03-22 22:30:50.000000 captureflow_agent-0.0.5/src/captureflow/__init__.py
--rw-r--r--   0 nikitakutc   (501) staff       (20)     6967 2024-05-06 08:24:49.000000 captureflow_agent-0.0.5/src/captureflow/tracer.py
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:30:37.246434 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:30:37.000000 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/PKG-INFO
--rw-r--r--   0 nikitakutc   (501) staff       (20)      331 2024-05-06 08:30:37.000000 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/SOURCES.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)        1 2024-05-06 08:30:37.000000 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/dependency_links.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)       86 2024-05-06 08:30:37.000000 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/requires.txt
--rw-r--r--   0 nikitakutc   (501) staff       (20)       12 2024-05-06 08:30:37.000000 captureflow_agent-0.0.5/src/captureflow_agent.egg-info/top_level.txt
-drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:30:37.245491 captureflow_agent-0.0.5/tests/
--rw-r--r--   0 nikitakutc   (501) staff       (20)     3007 2024-05-01 13:37:39.000000 captureflow_agent-0.0.5/tests/test_fastapi_tracer.py
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.605311 captureflow_agent-0.0.6/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:52:12.604901 captureflow_agent-0.0.6/PKG-INFO
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     2528 2024-04-02 15:22:49.000000 captureflow_agent-0.0.6/README.md
+-rw-r--r--   0 nikitakutc   (501) staff       (20)      768 2024-05-06 08:52:07.000000 captureflow_agent-0.0.6/pyproject.toml
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       38 2024-05-06 08:52:12.605398 captureflow_agent-0.0.6/setup.cfg
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.598816 captureflow_agent-0.0.6/src/
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.600169 captureflow_agent-0.0.6/src/captureflow/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)        0 2024-03-22 22:30:50.000000 captureflow_agent-0.0.6/src/captureflow/__init__.py
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     7258 2024-05-06 08:50:51.000000 captureflow_agent-0.0.6/src/captureflow/tracer.py
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.604447 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3053 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/PKG-INFO
+-rw-r--r--   0 nikitakutc   (501) staff       (20)      331 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)        1 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       86 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/requires.txt
+-rw-r--r--   0 nikitakutc   (501) staff       (20)       12 2024-05-06 08:52:12.000000 captureflow_agent-0.0.6/src/captureflow_agent.egg-info/top_level.txt
+drwxr-xr-x   0 nikitakutc   (501) staff       (20)        0 2024-05-06 08:52:12.604043 captureflow_agent-0.0.6/tests/
+-rw-r--r--   0 nikitakutc   (501) staff       (20)     3007 2024-05-01 13:37:39.000000 captureflow_agent-0.0.6/tests/test_fastapi_tracer.py
```

### Comparing `captureflow_agent-0.0.5/PKG-INFO` & `captureflow_agent-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captureflow-agent
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data collector to unleash LLM power
 Author-email: Nikita Kuts <me@nikitakuts.com>
 Project-URL: homepage, https://captureflow.dev/
 Project-URL: repository, https://github.com/CaptureFlow/captureflow-py
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
```

### Comparing `captureflow_agent-0.0.5/README.md` & `captureflow_agent-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `captureflow_agent-0.0.5/pyproject.toml` & `captureflow_agent-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = { find = { where = ["src"], exclude = ["tests", "examples"] } }
 
 [project]
 name = "captureflow-agent"
-version = "0.0.5"
+version = "0.0.6"
 description = "Data collector to unleash LLM power"
 authors = [
     {name = "Nikita Kuts", email = "me@nikitakuts.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `captureflow_agent-0.0.5/src/captureflow/tracer.py` & `captureflow_agent-0.0.6/src/captureflow/tracer.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,20 @@
     def _trace_function_calls(self, frame, event, arg, context: Dict[str, Any]) -> Callable:
         """Trace function calls and capture relevant data."""
         code = frame.f_code
         func_name, file_name, line_no = code.co_name, code.co_filename, frame.f_lineno
 
         tag = self._get_file_tag(file_name)
 
-        if tag == "STDLIB" or tag == "LIBRARY":
+        # Skip STDLIB, LIBRARY, and everything that does not start with '/' (like /usr/app/src etc)
+        if tag == "STDLIB" or tag == "LIBRARY" or not file_name.startswith('/'):
+            return lambda frame, event, arg: self._trace_function_calls(frame, event, arg, context)
+
+        # Skip lines for now
+        if event == "line":
             return lambda frame, event, arg: self._trace_function_calls(frame, event, arg, context)
 
         caller_id = context["call_stack"][-1]["id"] if context["call_stack"] else None
 
         call_id = str(uuid.uuid4())
         trace_event = {
             "id": call_id,
```

### Comparing `captureflow_agent-0.0.5/src/captureflow_agent.egg-info/PKG-INFO` & `captureflow_agent-0.0.6/src/captureflow_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captureflow-agent
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data collector to unleash LLM power
 Author-email: Nikita Kuts <me@nikitakuts.com>
 Project-URL: homepage, https://captureflow.dev/
 Project-URL: repository, https://github.com/CaptureFlow/captureflow-py
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
```

### Comparing `captureflow_agent-0.0.5/tests/test_fastapi_tracer.py` & `captureflow_agent-0.0.6/tests/test_fastapi_tracer.py`

 * *Files identical despite different names*

