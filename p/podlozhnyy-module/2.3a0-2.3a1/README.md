# Comparing `tmp/podlozhnyy_module-2.3a0.tar.gz` & `tmp/podlozhnyy_module-2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podlozhnyy_module-2.3a0.tar", last modified: Fri May  3 08:48:12 2024, max compression
+gzip compressed data, was "dist\podlozhnyy_module-2.3a1.tar", last modified: Mon May  6 09:37:33 2024, max compression
```

## Comparing `podlozhnyy_module-2.3a0.tar` & `podlozhnyy_module-2.3a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/
--rw-rw-rw-   0        0        0     2671 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     1605 2024-05-02 11:23:34.000000 podlozhnyy_module-2.3a0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/
--rw-rw-rw-   0        0        0      729 2023-05-19 18:40:24.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-05-18 20:56:40.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/bootstrap.py
--rw-rw-rw-   0        0        0     2956 2023-08-28 00:07:56.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/charts.py
--rw-rw-rw-   0        0        0     5255 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/collocation.py
--rw-rw-rw-   0        0        0     4899 2024-04-22 21:45:42.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/correlation.py
--rw-rw-rw-   0        0        0     4315 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/pareto.py
--rw-rw-rw-   0        0        0     4103 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/permutation.py
--rw-rw-rw-   0        0        0    31680 2024-05-02 12:30:35.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/regression.py
--rw-rw-rw-   0        0        0    15398 2023-05-19 18:31:11.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/timeseries.py
--rw-rw-rw-   0        0        0     5598 2023-05-19 18:31:11.000000 podlozhnyy_module-2.3a0/podlozhnyy_module/timetest.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/
--rw-rw-rw-   0        0        0     2671 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 08:48:12.000000 podlozhnyy_module-2.3a0/setup.cfg
--rw-rw-rw-   0        0        0     1118 2024-05-02 12:22:20.000000 podlozhnyy_module-2.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/
+-rw-rw-rw-   0        0        0     2671 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1605 2024-05-02 11:23:34.000000 podlozhnyy_module-2.3a1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/
+-rw-rw-rw-   0        0        0      729 2023-05-19 18:40:24.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-05-18 20:56:40.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/bootstrap.py
+-rw-rw-rw-   0        0        0     2956 2023-08-28 00:07:56.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/charts.py
+-rw-rw-rw-   0        0        0     5255 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/collocation.py
+-rw-rw-rw-   0        0        0     4899 2024-04-22 21:45:42.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/correlation.py
+-rw-rw-rw-   0        0        0     4315 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/pareto.py
+-rw-rw-rw-   0        0        0     4103 2023-05-19 18:39:18.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/permutation.py
+-rw-rw-rw-   0        0        0    31685 2024-05-06 09:36:50.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/regression.py
+-rw-rw-rw-   0        0        0    15398 2023-05-19 18:31:11.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/timeseries.py
+-rw-rw-rw-   0        0        0     5598 2023-05-19 18:31:11.000000 podlozhnyy_module-2.3a1/podlozhnyy_module/timetest.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/
+-rw-rw-rw-   0        0        0     2671 2024-05-06 09:37:32.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:37:32.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-05-06 09:37:32.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 09:37:32.000000 podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:37:33.000000 podlozhnyy_module-2.3a1/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2024-05-06 09:35:50.000000 podlozhnyy_module-2.3a1/setup.py
```

### Comparing `podlozhnyy_module-2.3a0/PKG-INFO` & `podlozhnyy_module-2.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podlozhnyy_module
-Version: 2.3a0
+Version: 2.3a1
 Summary: One place for the most useful methods for work
 Home-page: https://github.com/NPodlozhniy/podlozhnyy-module
 Author: Nikita Podlozhnyy
 Author-email: podlozhnyy.ne@phystech.edu
 License: MIT
 Description: # podlozhnyy-module
```

### Comparing `podlozhnyy_module-2.3a0/README.md` & `podlozhnyy_module-2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/__init__.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/__init__.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/bootstrap.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/bootstrap.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/charts.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/charts.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/collocation.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/collocation.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/correlation.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/correlation.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/pareto.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/pareto.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/permutation.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/permutation.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/regression.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,15 +747,15 @@
     val_dict = {}
     for name, value in zip(names, values):
         val_dict[name] = round(value, 3)
     if verbose:
         coef_list = list(val_dict.items())
         coef_list.sort(key=lambda i: i[1], reverse=True)
         for i in coef_list:
-            if i[1] >= thr:
+            if abs(i[1]) >= thr:
                 print(i[0], ":", round(i[1], 5))
     return val_dict
 
 
 @_set_options
 def plot_confusion_matrix(
     cm, classes, normalize=False, title="Confusion matrix", cmap=plt.cm.Blues
```

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/timeseries.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/timeseries.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module/timetest.py` & `podlozhnyy_module-2.3a1/podlozhnyy_module/timetest.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/PKG-INFO` & `podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podlozhnyy-module
-Version: 2.3a0
+Version: 2.3a1
 Summary: One place for the most useful methods for work
 Home-page: https://github.com/NPodlozhniy/podlozhnyy-module
 Author: Nikita Podlozhnyy
 Author-email: podlozhnyy.ne@phystech.edu
 License: MIT
 Description: # podlozhnyy-module
```

### Comparing `podlozhnyy_module-2.3a0/podlozhnyy_module.egg-info/SOURCES.txt` & `podlozhnyy_module-2.3a1/podlozhnyy_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.3a0/setup.py` & `podlozhnyy_module-2.3a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt", "r") as req_file:
     requirements = req_file.read().split("\n")
 
 setup(
     name="podlozhnyy_module",
-    version="2.3-alpha",
+    version="2.3-alpha.1",
     description="One place for the most useful methods for work",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Nikita Podlozhnyy",
     author_email="podlozhnyy.ne@phystech.edu",
     python_requires=">=3.7.0",
     url="https://github.com/NPodlozhniy/podlozhnyy-module",
```

