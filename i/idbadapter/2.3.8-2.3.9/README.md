# Comparing `tmp/idbadapter-2.3.8.tar.gz` & `tmp/idbadapter-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-2.3.8.tar", last modified: Tue Dec 12 12:49:36 2023, max compression
+gzip compressed data, was "idbadapter-2.3.9.tar", last modified: Tue Dec 12 13:33:08 2023, max compression
```

## Comparing `idbadapter-2.3.8.tar` & `idbadapter-2.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-12-12 12:49:36.963725 idbadapter-2.3.8/
--rw-rw-rw-   0        0        0    11357 2023-09-29 08:13:42.000000 idbadapter-2.3.8/LICENSE
--rw-rw-rw-   0        0        0      673 2023-12-12 12:49:36.963725 idbadapter-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-09-29 08:13:42.000000 idbadapter-2.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-12 12:49:36.943724 idbadapter-2.3.8/idbadapter/
--rw-rw-rw-   0        0        0       81 2023-12-04 16:44:35.000000 idbadapter-2.3.8/idbadapter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-12 12:49:36.962726 idbadapter-2.3.8/idbadapter/field_dev/
--rw-rw-rw-   0        0        0       65 2023-11-28 16:05:58.000000 idbadapter-2.3.8/idbadapter/field_dev/__init__.py
--rw-rw-rw-   0        0        0      600 2023-11-28 16:05:58.000000 idbadapter-2.3.8/idbadapter/field_dev/history.py
--rw-rw-rw-   0        0        0     1601 2023-12-05 10:04:29.000000 idbadapter-2.3.8/idbadapter/models.py
--rw-rw-rw-   0        0        0     8808 2023-12-12 12:32:57.000000 idbadapter-2.3.8/idbadapter/mschm.py
--rw-rw-rw-   0        0        0     8983 2023-11-23 14:12:36.000000 idbadapter-2.3.8/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-12-12 12:49:36.955724 idbadapter-2.3.8/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      673 2023-12-12 12:49:36.000000 idbadapter-2.3.8/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-12-12 12:49:36.000000 idbadapter-2.3.8/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-12 12:49:36.000000 idbadapter-2.3.8/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-12-12 12:49:36.000000 idbadapter-2.3.8/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-12-12 12:49:36.000000 idbadapter-2.3.8/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-12 12:49:36.964724 idbadapter-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-12-12 12:49:19.000000 idbadapter-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-12 13:33:08.860121 idbadapter-2.3.9/
+-rw-rw-rw-   0        0        0    11357 2023-09-29 08:13:42.000000 idbadapter-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0      673 2023-12-12 13:33:08.860121 idbadapter-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-09-29 08:13:42.000000 idbadapter-2.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-12 13:33:08.838122 idbadapter-2.3.9/idbadapter/
+-rw-rw-rw-   0        0        0       81 2023-12-04 16:44:35.000000 idbadapter-2.3.9/idbadapter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-12 13:33:08.850122 idbadapter-2.3.9/idbadapter/field_dev/
+-rw-rw-rw-   0        0        0       65 2023-11-28 16:05:58.000000 idbadapter-2.3.9/idbadapter/field_dev/__init__.py
+-rw-rw-rw-   0        0        0      600 2023-11-28 16:05:58.000000 idbadapter-2.3.9/idbadapter/field_dev/history.py
+-rw-rw-rw-   0        0        0     1601 2023-12-05 10:04:29.000000 idbadapter-2.3.9/idbadapter/models.py
+-rw-rw-rw-   0        0        0     8820 2023-12-12 13:32:53.000000 idbadapter-2.3.9/idbadapter/mschm.py
+-rw-rw-rw-   0        0        0     8983 2023-11-23 14:12:36.000000 idbadapter-2.3.9/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-12-12 13:33:08.849121 idbadapter-2.3.9/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      673 2023-12-12 13:33:08.000000 idbadapter-2.3.9/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-12-12 13:33:08.000000 idbadapter-2.3.9/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-12 13:33:08.000000 idbadapter-2.3.9/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-12-12 13:33:08.000000 idbadapter-2.3.9/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-12-12 13:33:08.000000 idbadapter-2.3.9/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-12 13:33:08.861122 idbadapter-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-12-12 13:33:06.000000 idbadapter-2.3.9/setup.py
```

### Comparing `idbadapter-2.3.8/LICENSE` & `idbadapter-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-2.3.8/PKG-INFO` & `idbadapter-2.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 2.3.8
+Version: 2.3.9
 Summary: Adapter for database access
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-2.3.8/idbadapter/field_dev/history.py` & `idbadapter-2.3.9/idbadapter/field_dev/history.py`

 * *Files identical despite different names*

### Comparing `idbadapter-2.3.8/idbadapter/models.py` & `idbadapter-2.3.9/idbadapter/models.py`

 * *Files identical despite different names*

### Comparing `idbadapter-2.3.8/idbadapter/mschm.py` & `idbadapter-2.3.9/idbadapter/mschm.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     @lru_cache
     def get_model(self, name):
         if name in self.mschm_models:
             return self.mschm_models[name]
         elif len(self.mschm_models) == 0:
             result: list[MSModel] = self.__execute_query(
                 select(MSModel))
-            self.mschm_models = {k.name: k.data for k in result}
+            self.mschm_models = {k.name: json.loads(k.data) for k in result}
             return self.mschm_models[name]
         else:
             print(f"model with name {name} not found!")
             return
 
     def save_s7_model(self, model):
         models_to_write = []
```

### Comparing `idbadapter-2.3.8/idbadapter/schedule_loader.py` & `idbadapter-2.3.9/idbadapter/schedule_loader.py`

 * *Files identical despite different names*

### Comparing `idbadapter-2.3.8/idbadapter.egg-info/PKG-INFO` & `idbadapter-2.3.9/idbadapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 2.3.8
+Version: 2.3.9
 Summary: Adapter for database access
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-2.3.8/setup.py` & `idbadapter-2.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '2.3.8'
+version = '2.3.9'
 
 long_description = "Adapter for database access"
 
 setup(name='idbadapter',
-      version='2.3.8',
+      version='2.3.9',
       description='Adapter for database access',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter', 'idbadapter/field_dev'],
```

