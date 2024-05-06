# Comparing `tmp/python-documentcloud-4.1.0.tar.gz` & `tmp/python-documentcloud-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-documentcloud-4.1.0.tar", last modified: Wed Mar  6 19:58:17 2024, max compression
+gzip compressed data, was "python-documentcloud-4.1.1.tar", last modified: Mon May  6 20:22:24 2024, max compression
```

## Comparing `python-documentcloud-4.1.0.tar` & `python-documentcloud-4.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2024-03-06 19:58:17.197266 python-documentcloud-4.1.0/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1151 2020-06-11 15:56:14.000000 python-documentcloud-4.1.0/LICENSE
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2076 2024-03-06 19:58:17.197266 python-documentcloud-4.1.0/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1156 2023-11-14 19:13:06.000000 python-documentcloud-4.1.0/README.md
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2024-03-06 19:58:17.193266 python-documentcloud-4.1.0/documentcloud/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      220 2020-06-13 15:35:49.000000 python-documentcloud-4.1.0/documentcloud/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    11754 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/addon.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2538 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/annotations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     6543 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/base.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5843 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/client.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1333 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/constants.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    19563 2024-03-06 19:54:29.000000 python-documentcloud-4.1.0/documentcloud/documents.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1161 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/exceptions.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      392 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/organizations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5328 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/projects.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      924 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/sections.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1835 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/toolbox.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      354 2023-12-20 15:20:46.000000 python-documentcloud-4.1.0/documentcloud/users.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2024-03-06 19:58:17.197266 python-documentcloud-4.1.0/python_documentcloud.egg-info/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2076 2024-03-06 19:58:17.000000 python-documentcloud-4.1.0/python_documentcloud.egg-info/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      592 2024-03-06 19:58:17.000000 python-documentcloud-4.1.0/python_documentcloud.egg-info/SOURCES.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2024-03-06 19:58:17.000000 python-documentcloud-4.1.0/python_documentcloud.egg-info/dependency_links.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      188 2024-03-06 19:58:17.000000 python-documentcloud-4.1.0/python_documentcloud.egg-info/requires.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       14 2024-03-06 19:58:17.000000 python-documentcloud-4.1.0/python_documentcloud.egg-info/top_level.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2024-03-06 19:58:17.197266 python-documentcloud-4.1.0/setup.cfg
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1631 2024-03-06 19:58:00.000000 python-documentcloud-4.1.0/setup.py
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1151 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/LICENSE
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/PKG-INFO
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1156 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/README.md
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.684792 python-documentcloud-4.1.1/documentcloud/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      220 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/__init__.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)    11754 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/addon.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2538 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/annotations.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     6543 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/base.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     5906 2024-05-06 20:08:46.000000 python-documentcloud-4.1.1/documentcloud/client.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1333 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/constants.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)    19563 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/documents.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1161 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/exceptions.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      392 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/organizations.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     5328 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/projects.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      924 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/sections.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1835 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/toolbox.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      354 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/users.py
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/python_documentcloud.egg-info/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      592 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)        1 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      188 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/requires.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)       14 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/top_level.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      102 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/setup.cfg
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1631 2024-05-06 20:19:36.000000 python-documentcloud-4.1.1/setup.py
```

### Comparing `python-documentcloud-4.1.0/LICENSE` & `python-documentcloud-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/PKG-INFO` & `python-documentcloud-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 4.1.0
+Version: 4.1.1
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-4.1.0/README.md` & `python-documentcloud-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/addon.py` & `python-documentcloud-4.1.1/documentcloud/addon.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/annotations.py` & `python-documentcloud-4.1.1/documentcloud/annotations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/base.py` & `python-documentcloud-4.1.1/documentcloud/base.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/client.py` & `python-documentcloud-4.1.1/documentcloud/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,18 @@
             # check to avoid double setting version
             kwargs.setdefault("params", {}).update({"version": "2.0"})
 
         response = requests_retry_session(session=self.session).request(
             method, url, timeout=self.timeout, **kwargs
         )
         logger.debug("response: %s - %s", response.status_code, response.content)
-        if response.status_code == requests.codes.FORBIDDEN and set_tokens:
+        if (
+            response.status_code in [requests.codes.FORBIDDEN, requests.codes.TOO_MANY]
+            and set_tokens
+        ):
             self._set_tokens()
             # track set_tokens to not enter an infinite loop
             kwargs["set_tokens"] = False
             return self._request(method, url, full_url=True, **kwargs)
 
         if raise_error:
             self.raise_for_status(response)
```

### Comparing `python-documentcloud-4.1.0/documentcloud/constants.py` & `python-documentcloud-4.1.1/documentcloud/constants.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/documents.py` & `python-documentcloud-4.1.1/documentcloud/documents.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/exceptions.py` & `python-documentcloud-4.1.1/documentcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/projects.py` & `python-documentcloud-4.1.1/documentcloud/projects.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/sections.py` & `python-documentcloud-4.1.1/documentcloud/sections.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/documentcloud/toolbox.py` & `python-documentcloud-4.1.1/documentcloud/toolbox.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/python_documentcloud.egg-info/PKG-INFO` & `python-documentcloud-4.1.1/python_documentcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 4.1.0
+Version: 4.1.1
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-4.1.0/python_documentcloud.egg-info/SOURCES.txt` & `python-documentcloud-4.1.1/python_documentcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.0/setup.py` & `python-documentcloud-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="python-documentcloud",
-    version="4.1.0",
+    version="4.1.1",
     description="A simple Python wrapper for the DocumentCloud API",
     author="Mitchell Kotler",
     author_email="mitch@muckrock.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muckrock/python-documentcloud",
     license="MIT",
```

