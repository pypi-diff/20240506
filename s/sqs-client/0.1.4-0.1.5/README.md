# Comparing `tmp/sqs-client-0.1.4.tar.gz` & `tmp/sqs_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqs-client-0.1.4.tar", last modified: Thu Mar 21 11:08:01 2024, max compression
+gzip compressed data, was "sqs_client-0.1.5.tar", last modified: Mon May  6 08:50:22 2024, max compression
```

## Comparing `sqs-client-0.1.4.tar` & `sqs_client-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:08:01.560735 sqs-client-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-21 11:07:43.000000 sqs-client-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-21 11:08:01.560735 sqs-client-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-21 11:07:43.000000 sqs-client-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-21 11:07:43.000000 sqs-client-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-21 11:08:01.560735 sqs-client-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:08:01.556735 sqs-client-0.1.4/sqs_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 11:07:43.000000 sqs-client-0.1.4/sqs_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-03-21 11:07:43.000000 sqs-client-0.1.4/sqs_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-21 11:07:43.000000 sqs-client-0.1.4/sqs_client/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-03-21 11:07:43.000000 sqs-client-0.1.4/sqs_client/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:08:01.560735 sqs-client-0.1.4/sqs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-21 11:08:01.000000 sqs-client-0.1.4/sqs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-21 11:08:01.000000 sqs-client-0.1.4/sqs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 11:08:01.000000 sqs-client-0.1.4/sqs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 11:08:01.000000 sqs-client-0.1.4/sqs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.767235 sqs_client-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 08:50:08.000000 sqs_client-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-06 08:50:22.767235 sqs_client-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-06 08:50:08.000000 sqs_client-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 08:50:08.000000 sqs_client-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 08:50:22.767235 sqs_client-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.763235 sqs_client-0.1.5/sqs_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.767235 sqs_client-0.1.5/sqs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/top_level.txt
```

### Comparing `sqs-client-0.1.4/LICENSE` & `sqs_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqs-client-0.1.4/PKG-INFO` & `sqs_client-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqs-client-0.1.4/README.md` & `sqs_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sqs-client-0.1.4/pyproject.toml` & `sqs_client-0.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqs-client"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Digital Fortress", email="hai.huynh@digitalfortress.dev" },
 ]
 description = "SQS client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqs-client-0.1.4/sqs_client/client.py` & `sqs_client-0.1.5/sqs_client/client.py`

 * *Files identical despite different names*

### Comparing `sqs-client-0.1.4/sqs_client/publisher.py` & `sqs_client-0.1.5/sqs_client/publisher.py`

 * *Files identical despite different names*

### Comparing `sqs-client-0.1.4/sqs_client/task.py` & `sqs_client-0.1.5/sqs_client/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         """
         This function retrieves the ID of task
         Returns:
             The ID of task.
         """
         return self._id
 
+    def get_queue_name(self):
+        """
+        This function retrieves the queue name of task
+        Returns:
+            The queue name of task.
+        """
+        return self._queue_name
+
     def _get_message_processing(self):
         """
         This function retrieves the message processing for the task
         Returns:
             (function) The message processing for the task.
         """
         if self._lazy:
```

### Comparing `sqs-client-0.1.4/sqs_client.egg-info/PKG-INFO` & `sqs_client-0.1.5/sqs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

