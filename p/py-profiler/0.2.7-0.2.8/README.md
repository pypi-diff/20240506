# Comparing `tmp/py_profiler-0.2.7.tar.gz` & `tmp/py_profiler-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_profiler-0.2.7.tar", last modified: Thu May  2 10:59:53 2024, max compression
+gzip compressed data, was "py_profiler-0.2.8.tar", last modified: Mon May  6 07:19:19 2024, max compression
```

## Comparing `py_profiler-0.2.7.tar` & `py_profiler-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.651219 py_profiler-0.2.7/
--rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.2.7/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.2.7/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-02 10:59:53.650935 py_profiler-0.2.7/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.2.7/README.md
--rw-r--r--   0 andy       (501) staff       (20)      126 2023-02-02 15:54:28.000000 py_profiler-0.2.7/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-02 10:59:53.651274 py_profiler-0.2.7/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)      911 2024-05-02 05:32:12.000000 py_profiler-0.2.7/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.645250 py_profiler-0.2.7/src/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.649043 py_profiler-0.2.7/src/py_profiler/
--rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1026 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/decorator.py
--rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.2.7/src/py_profiler/fastapi_profiler_controller.py
--rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/long_adder.py
--rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.2.7/src/py_profiler/measure_service.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.2.7/src/py_profiler/profiler_controller.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.650158 py_profiler-0.2.7/src/py_profiler/templates/
--rw-r--r--   0 andy       (501) staff       (20)     3308 2024-03-14 09:35:36.000000 py_profiler-0.2.7/src/py_profiler/templates/profiler.html
--rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.650624 py_profiler-0.2.7/src/py_profiler.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      520 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       22 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       12 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-06 07:19:19.318706 py_profiler-0.2.8/
+-rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.2.8/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.2.8/MANIFEST.in
+-rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-06 07:19:19.318385 py_profiler-0.2.8/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.2.8/README.md
+-rw-r--r--   0 andy       (501) staff       (20)      126 2023-02-02 15:54:28.000000 py_profiler-0.2.8/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-06 07:19:19.318765 py_profiler-0.2.8/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)      911 2024-05-06 07:18:00.000000 py_profiler-0.2.8/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-06 07:19:19.313740 py_profiler-0.2.8/src/
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-06 07:19:19.316696 py_profiler-0.2.8/src/py_profiler/
+-rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.2.8/src/py_profiler/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1026 2023-02-02 15:54:28.000000 py_profiler-0.2.8/src/py_profiler/decorator.py
+-rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.2.8/src/py_profiler/fastapi_profiler_controller.py
+-rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.2.8/src/py_profiler/long_adder.py
+-rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.2.8/src/py_profiler/measure_service.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.2.8/src/py_profiler/profiler_controller.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-06 07:19:19.317621 py_profiler-0.2.8/src/py_profiler/templates/
+-rw-r--r--   0 andy       (501) staff       (20)     3337 2024-05-06 07:17:48.000000 py_profiler-0.2.8/src/py_profiler/templates/profiler.html
+-rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.2.8/src/py_profiler/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-06 07:19:19.317953 py_profiler-0.2.8/src/py_profiler.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-06 07:19:19.000000 py_profiler-0.2.8/src/py_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      520 2024-05-06 07:19:19.000000 py_profiler-0.2.8/src/py_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-06 07:19:19.000000 py_profiler-0.2.8/src/py_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       22 2024-05-06 07:19:19.000000 py_profiler-0.2.8/src/py_profiler.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       12 2024-05-06 07:19:19.000000 py_profiler-0.2.8/src/py_profiler.egg-info/top_level.txt
```

### Comparing `py_profiler-0.2.7/LICENSE` & `py_profiler-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/PKG-INFO` & `py_profiler-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.7/README.md` & `py_profiler-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/setup.py` & `py_profiler-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_profiler",
-    version="0.2.7",
+    version="0.2.8",
     author="Andy Le",
     author_email="tauit.dnmd@gmail.com",
     description="A library to measure your method, function execution time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andy1xx8/py-profiler",
     project_urls={
```

### Comparing `py_profiler-0.2.7/src/py_profiler/decorator.py` & `py_profiler-0.2.8/src/py_profiler/decorator.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/src/py_profiler/long_adder.py` & `py_profiler-0.2.8/src/py_profiler/long_adder.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/src/py_profiler/measure_service.py` & `py_profiler-0.2.8/src/py_profiler/measure_service.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/src/py_profiler/templates/profiler.html` & `py_profiler-0.2.8/src/py_profiler/templates/profiler.html`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 <table style="width:100%">
     <thead>
     <tr style="background-color: paleturquoise">
         <th>No</th>
         <th>Name</th>
         <th>Total Req</th>
         <th>Pending Req</th>
+        <th>Failure Req</th>
         <th>Total Exec Time
             <br>(millis)
         </th>
         <th>Last Exec Time
             <br>(millis)
         </th>
         <th>Highest Exec Time
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-NNoo         NNaammee             TToottaall RReeqq                   PPeennddiinngg RReeqq                           TToottaall EExxeecc TTiimmee                     LLaasstt EExxeecc TTiimmee              HHiigghheesstt EExxeecc TTiimmee          RReeqquueesstt RRaattee                  AAvvgg TTiimmee//RReeqquueesstt
-                                                                                              ((mmiilllliiss))                            ((mmiilllliiss))                    ((mmiilllliiss))                   ((rreeqq//sseecc))                     ((mmiilllliiss//rreeqq))
+NNoo         NNaammee             TToottaall RReeqq                   PPeennddiinngg RReeqq                           FFaaiilluurree RReeqq                         TToottaall EExxeecc TTiimmee             LLaasstt EExxeecc TTiimmee             HHiigghheesstt EExxeecc TTiimmee             RReeqquueesstt RRaattee            AAvvgg TTiimmee//RReeqquueesstt
+                                                                                                                                  ((mmiilllliiss))                    ((mmiilllliiss))                   ((mmiilllliiss))                      ((rreeqq//sseecc))               ((mmiilllliiss//rreeqq))
 {          {                {                           {                                     {                                   {                           {                          {                             {                       {
 {          {                {                           {                                     {                                   {                           {                          {                             {                       {
 loop.index report.func_name report.total_hits.get_value report.current_pending_hits.get_value report.current_error_hits.get_value report.total_duration_as_ms report.last_duration_as_ms report.highest_duration_as_ms report.get_request_rate report.get_avg_time_per_request
 }}         }}               () }}                       () }}                                 () }}                               () }}                       () }}                      () }}                         () }}                   () }}
 UUpp TTiimmee    {{ uptime }}
 SSttaarrtt AAtt   {{ start_at }}
```

### Comparing `py_profiler-0.2.7/src/py_profiler/utils.py` & `py_profiler-0.2.8/src/py_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.7/src/py_profiler.egg-info/PKG-INFO` & `py_profiler-0.2.8/src/py_profiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.7/src/py_profiler.egg-info/SOURCES.txt` & `py_profiler-0.2.8/src/py_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

