# Comparing `tmp/zeus_utility-0.0.9.tar.gz` & `tmp/zeus_utility-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus_utility-0.0.9.tar", last modified: Tue Mar 19 17:26:04 2024, max compression
+gzip compressed data, was "zeus_utility-0.1.0.tar", last modified: Mon May  6 03:35:53 2024, max compression
```

## Comparing `zeus_utility-0.0.9.tar` & `zeus_utility-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.105517 zeus_utility-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 zeus_utility-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1189 2024-03-19 17:26:04.095991 zeus_utility-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-01-15 10:14:05.000000 zeus_utility-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 17:26:04.105517 zeus_utility-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3310 2024-03-19 17:12:17.000000 zeus_utility-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.089470 zeus_utility-0.0.9/zeus_utility/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 zeus_utility-0.0.9/zeus_utility/__init__.py
--rw-rw-rw-   0        0        0      671 2024-03-15 10:32:04.000000 zeus_utility-0.0.9/zeus_utility/io.py
--rw-rw-rw-   0        0        0     3301 2024-03-19 17:09:06.000000 zeus_utility-0.0.9/zeus_utility/parallel_executor.py
-drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.095002 zeus_utility-0.0.9/zeus_utility.egg-info/
--rw-rw-rw-   0        0        0     1189 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 03:35:53.746766 zeus_utility-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 zeus_utility-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1204 2024-05-06 03:35:53.745772 zeus_utility-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-01-15 10:14:05.000000 zeus_utility-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:35:53.746766 zeus_utility-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3318 2024-05-06 03:32:31.000000 zeus_utility-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:35:53.731513 zeus_utility-0.1.0/zeus_utility/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 zeus_utility-0.1.0/zeus_utility/__init__.py
+-rw-rw-rw-   0        0        0     4717 2024-04-29 09:45:22.000000 zeus_utility-0.1.0/zeus_utility/embeddings.py
+-rw-rw-rw-   0        0        0      671 2024-03-15 10:32:04.000000 zeus_utility-0.1.0/zeus_utility/io.py
+-rw-rw-rw-   0        0        0     3341 2024-03-25 10:24:08.000000 zeus_utility-0.1.0/zeus_utility/parallel_executor.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:35:53.744779 zeus_utility-0.1.0/zeus_utility.egg-info/
+-rw-rw-rw-   0        0        0     1204 2024-05-06 03:35:53.000000 zeus_utility-0.1.0/zeus_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-06 03:35:53.000000 zeus_utility-0.1.0/zeus_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:35:53.000000 zeus_utility-0.1.0/zeus_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-06 03:35:53.000000 zeus_utility-0.1.0/zeus_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 03:35:53.000000 zeus_utility-0.1.0/zeus_utility.egg-info/top_level.txt
```

### Comparing `zeus_utility-0.0.9/LICENSE` & `zeus_utility-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus_utility-0.0.9/PKG-INFO` & `zeus_utility-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: zeus_utility
-Version: 0.0.9
+Version: 0.1.0
 Summary: Just some useful utilities Zeus will use in almost every projects.
 Home-page: https://github.com/zeuscsc/zeus_utility.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pypdf
-Requires-Dist: tqdm
+Requires-Dist: pypdf==4.2.0
+Requires-Dist: tqdm==4.66.4
 
 
 # Zeus's Utility
 
 ## Features
 - [x] Parallel Execute
```

### Comparing `zeus_utility-0.0.9/setup.py` & `zeus_utility-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 NAME = 'zeus_utility'
 DESCRIPTION = 'Just some useful utilities Zeus will use in almost every projects.'
 URL = 'https://github.com/zeuscsc/zeus_utility.git'
 EMAIL = 'zeuscsc@gmail.com'
 AUTHOR = 'Zeus Chiu'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
-with open('requirements.txt') as f:
+with open('requirements_version.txt') as f:
     required_packages = f.readlines()
     required_packages = [pkg.strip() for pkg in required_packages]
 
 EXTRAS = {
 }
 
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `zeus_utility-0.0.9/zeus_utility/io.py` & `zeus_utility-0.1.0/zeus_utility/io.py`

 * *Files identical despite different names*

### Comparing `zeus_utility-0.0.9/zeus_utility/parallel_executor.py` & `zeus_utility-0.1.0/zeus_utility/parallel_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def add_task(self,task:Callable,**kwargs):
         super().append((task,kwargs))
 
     def execute(self,progress_bar=None):
         if self.threads_count==1:
             for task in self:
                 task[0](**task[1])
+                progress_bar.update(1)
         elif self.threads_count>1:
             execute_queue(self,threads_count=self.threads_count,slience=self.slience,waiting_time=self.waiting_time,use_try_catch=self.use_try_catch,progress_bar=progress_bar)
     pass
 def execute_queue(iterator:Iterator,threads_count:int=10,slience=True,waiting_time=0,use_try_catch=False,progress_bar:tqdm=None):
     def run_task(task:Callable,*args, **kwargs):
         if not use_try_catch:
             task(*args, **kwargs)
```

### Comparing `zeus_utility-0.0.9/zeus_utility.egg-info/PKG-INFO` & `zeus_utility-0.1.0/zeus_utility.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
-Name: zeus_utility
-Version: 0.0.9
+Name: zeus-utility
+Version: 0.1.0
 Summary: Just some useful utilities Zeus will use in almost every projects.
 Home-page: https://github.com/zeuscsc/zeus_utility.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pypdf
-Requires-Dist: tqdm
+Requires-Dist: pypdf==4.2.0
+Requires-Dist: tqdm==4.66.4
 
 
 # Zeus's Utility
 
 ## Features
 - [x] Parallel Execute
```

