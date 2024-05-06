# Comparing `tmp/nutshell-0.3.1.tar.gz` & `tmp/nutshell-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutshell-0.3.1.tar", max compression
+gzip compressed data, was "nutshell-0.3.2.tar", max compression
```

## Comparing `nutshell-0.3.1.tar` & `nutshell-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2141 2024-04-04 20:56:58.332838 nutshell-0.3.1/README.md
--rw-r--r--   0        0        0       38 2024-04-04 20:06:34.504541 nutshell-0.3.1/nutshell/__init__.py
--rw-r--r--   0        0        0     4637 2024-04-04 20:01:06.368939 nutshell-0.3.1/nutshell/entities.py
--rw-r--r--   0        0        0     4810 2024-04-04 20:08:29.054520 nutshell-0.3.1/nutshell/methods.py
--rw-r--r--   0        0        0     3149 2024-04-04 20:46:07.813266 nutshell-0.3.1/nutshell/nutshell_api.py
--rw-r--r--   0        0        0      784 2024-04-04 20:08:12.391554 nutshell-0.3.1/nutshell/responses.py
--rw-r--r--   0        0        0      624 2024-04-04 20:58:45.972490 nutshell-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 nutshell-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2141 2024-04-04 20:56:58.332838 nutshell-0.3.2/README.md
+-rw-r--r--   0        0        0      683 2024-05-06 20:44:05.980361 nutshell-0.3.2/nutshell/__init__.py
+-rw-r--r--   0        0        0    10171 2024-05-06 20:44:06.048075 nutshell-0.3.2/nutshell/entities.py
+-rw-r--r--   0        0        0     5465 2024-05-06 20:25:57.425124 nutshell-0.3.2/nutshell/methods.py
+-rw-r--r--   0        0        0     3149 2024-04-04 20:46:07.813266 nutshell-0.3.2/nutshell/nutshell_api.py
+-rw-r--r--   0        0        0      784 2024-04-04 20:08:12.391554 nutshell-0.3.2/nutshell/responses.py
+-rw-r--r--   0        0        0      624 2024-05-06 20:44:23.806559 nutshell-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 nutshell-0.3.2/PKG-INFO
```

### Comparing `nutshell-0.3.1/README.md` & `nutshell-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nutshell-0.3.1/nutshell/methods.py` & `nutshell-0.3.2/nutshell/methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,50 @@
 
 from pydantic import BaseModel, computed_field
 
 from nutshell.entities import AnalyticsReportType, FindLeadsQuery, ActivityType, User, Team
 
 
 class _APIMethod(BaseModel):
-    """Base class for all method calls to the Nutshell API."""
+    """
+    Base class for all method calls to the Nutshell API.
+
+    This class should not be used directly, but should be subclassed for each API method.
+    """
     api_method: str
 
     @computed_field
     @property
     def params(self) -> dict:
         return {}
 
 
 class FindUsers(_APIMethod):
-    """findUsers method for Nutshell API."""
+    """
+    This method is used to retrieve a list of users from the Nutshell API.
+
+    Attributes
+    ----------
+    query : Optional[dict]
+        A dictionary of query parameters to filter the results.
+    order_by : str
+        The field to order the results by.
+    order_direction : str
+        The direction to order the results by.
+    limit : int
+        The maximum number of results to return.
+    page : int
+        The page of results to return.
+
+    Computed Attributes
+    -------------------
+    params : dict
+        A dictionary of the parameters to be passed to the API.
+
+    """
     query: Optional[dict] = None
     order_by: str = "last_name"
     order_direction: str = "ASC"
     limit: int = 50
     page: int = 1
     api_method: str = "findUsers"
```

### Comparing `nutshell-0.3.1/nutshell/nutshell_api.py` & `nutshell-0.3.2/nutshell/nutshell_api.py`

 * *Files identical despite different names*

### Comparing `nutshell-0.3.1/nutshell/responses.py` & `nutshell-0.3.2/nutshell/responses.py`

 * *Files identical despite different names*

### Comparing `nutshell-0.3.1/pyproject.toml` & `nutshell-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutshell"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python wrapper on the Nutshell CRM JSON RPC API"
 authors = ["Mark Nyberg <bigusdeveloper@gmail.com>"]
 license = "\"MIT\""
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nutshell-0.3.1/PKG-INFO` & `nutshell-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutshell
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python wrapper on the Nutshell CRM JSON RPC API
 License: "MIT"
 Author: Mark Nyberg
 Author-email: bigusdeveloper@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
```

