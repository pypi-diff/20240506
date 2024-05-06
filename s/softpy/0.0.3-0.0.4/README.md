# Comparing `tmp/softpy-0.0.3.tar.gz` & `tmp/softpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softpy-0.0.3.tar", last modified: Thu May  2 10:43:02 2024, max compression
+gzip compressed data, was "softpy-0.0.4.tar", last modified: Mon May  6 06:30:41 2024, max compression
```

## Comparing `softpy-0.0.3.tar` & `softpy-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.355692 softpy-0.0.3/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.3/LICENSE
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-02 10:43:02.356693 softpy-0.0.3/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.3/README.md
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-05-02 10:43:02.362820 softpy-0.0.3/setup.cfg
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-05-02 10:41:23.000000 softpy-0.0.3/setup.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:01.936905 softpy-0.0.3/softpy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.3/softpy/__init__.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.160914 softpy-0.0.3/softpy/evolutionary/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      708 2024-05-02 10:40:30.000000 softpy-0.0.3/softpy/evolutionary/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    12572 2023-06-21 10:17:14.000000 softpy-0.0.3/softpy/evolutionary/candidate.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7558 2024-03-08 14:08:59.000000 softpy-0.0.3/softpy/evolutionary/genetic.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.3/softpy/evolutionary/selection.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3238 2023-06-21 10:16:53.000000 softpy-0.0.3/softpy/evolutionary/singlestate.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.336680 softpy-0.0.3/softpy/fuzzy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.3/softpy/fuzzy/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3254 2024-03-08 14:08:45.000000 softpy-0.0.3/softpy/fuzzy/clustering.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9634 2024-03-08 14:08:37.000000 softpy-0.0.3/softpy/fuzzy/control.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    20235 2024-03-22 11:48:08.000000 softpy-0.0.3/softpy/fuzzy/fuzzyset.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14578 2024-03-22 11:52:40.000000 softpy-0.0.3/softpy/fuzzy/operations.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.036371 softpy-0.0.3/softpy.egg-info/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/requires.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/top_level.txt
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:41.294910 softpy-0.0.4/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.4/LICENSE
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-06 06:30:41.296915 softpy-0.0.4/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.4/README.md
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-05-06 06:30:41.307911 softpy-0.0.4/setup.cfg
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-05-06 06:29:53.000000 softpy-0.0.4/setup.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.415643 softpy-0.0.4/softpy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.4/softpy/__init__.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.962380 softpy-0.0.4/softpy/evolutionary/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      708 2024-05-02 10:40:30.000000 softpy-0.0.4/softpy/evolutionary/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    12572 2023-06-21 10:17:14.000000 softpy-0.0.4/softpy/evolutionary/candidate.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7558 2024-03-08 14:08:59.000000 softpy-0.0.4/softpy/evolutionary/genetic.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.4/softpy/evolutionary/selection.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3245 2024-05-06 06:29:19.000000 softpy-0.0.4/softpy/evolutionary/singlestate.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:41.253556 softpy-0.0.4/softpy/fuzzy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.4/softpy/fuzzy/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3254 2024-03-08 14:08:45.000000 softpy-0.0.4/softpy/fuzzy/clustering.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9634 2024-03-08 14:08:37.000000 softpy-0.0.4/softpy/fuzzy/control.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    20235 2024-03-22 11:48:08.000000 softpy-0.0.4/softpy/fuzzy/fuzzyset.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14578 2024-03-22 11:52:40.000000 softpy-0.0.4/softpy/fuzzy/operations.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-06 06:30:40.632445 softpy-0.0.4/softpy.egg-info/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-05-06 06:30:40.000000 softpy-0.0.4/softpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/requires.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-05-06 06:30:39.000000 softpy-0.0.4/softpy.egg-info/top_level.txt
```

### Comparing `softpy-0.0.3/PKG-INFO` & `softpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `softpy-0.0.3/README.md` & `softpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/setup.py` & `softpy-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='softpy',
-   version='0.0.3',
+   version='0.0.4',
    author='Andrea Campagner',
    python_requires=">3.8.0",
    author_email='onyris93@gmail.com',
    packages=find_packages(include=['softpy', 'softpy.*']),
    url='https://pypi.org/project/scikit-weak/',
    license='LICENSE.txt',
    description='A package for soft computing in Python.',
```

### Comparing `softpy-0.0.3/softpy/evolutionary/__init__.py` & `softpy-0.0.4/softpy/evolutionary/__init__.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/evolutionary/candidate.py` & `softpy-0.0.4/softpy/evolutionary/candidate.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/evolutionary/genetic.py` & `softpy-0.0.4/softpy/evolutionary/genetic.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/evolutionary/selection.py` & `softpy-0.0.4/softpy/evolutionary/selection.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/evolutionary/singlestate.py` & `softpy-0.0.4/softpy/evolutionary/singlestate.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         if keep_history:
             self.best_h = np.empty(n_iters, dtype=self.candidate_type)
             self.fitness_h = np.zeros(n_iters)
             self.fitness_h[:] = np.NINF
 
 
-        for it in n_iters:
+        for it in range(n_iters):
             population = np.array([self.candidate_type.generate(**self.kwargs) for i in range(self.pop_size)])
             fitness = np.vectorize(self.fitness_func)(population)
             v = np.max(fitness)
             self.best = population[np.argmax(fitness)] if v > self.fitness_best else self.best
             self.fitness_best = v if v > self.fitness_best else self.fitness_best
 
             if keep_history:
```

### Comparing `softpy-0.0.3/softpy/fuzzy/__init__.py` & `softpy-0.0.4/softpy/fuzzy/__init__.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/fuzzy/clustering.py` & `softpy-0.0.4/softpy/fuzzy/clustering.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/fuzzy/control.py` & `softpy-0.0.4/softpy/fuzzy/control.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/fuzzy/fuzzyset.py` & `softpy-0.0.4/softpy/fuzzy/fuzzyset.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy/fuzzy/operations.py` & `softpy-0.0.4/softpy/fuzzy/operations.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.3/softpy.egg-info/PKG-INFO` & `softpy-0.0.4/softpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

