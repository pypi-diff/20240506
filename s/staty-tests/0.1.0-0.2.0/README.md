# Comparing `tmp/staty_tests-0.1.0.tar.gz` & `tmp/staty_tests-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staty_tests-0.1.0.tar", last modified: Sat May  4 09:15:05 2024, max compression
+gzip compressed data, was "staty_tests-0.2.0.tar", last modified: Mon May  6 11:11:02 2024, max compression
```

## Comparing `staty_tests-0.1.0.tar` & `staty_tests-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-04 09:15:05.471823 staty_tests-0.1.0/
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1076 2024-05-04 07:20:41.000000 staty_tests-0.1.0/LICENSE
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1420 2024-05-04 09:15:05.471628 staty_tests-0.1.0/PKG-INFO
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      619 2024-05-04 07:23:27.000000 staty_tests-0.1.0/README.md
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       38 2024-05-04 09:15:05.471866 staty_tests-0.1.0/setup.cfg
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      972 2024-05-04 09:14:09.000000 staty_tests-0.1.0/setup.py
-drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-04 09:15:05.470456 staty_tests-0.1.0/statistical_tests/
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-04 07:22:39.000000 staty_tests-0.1.0/statistical_tests/__init__.py
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     2650 2024-05-04 08:32:02.000000 staty_tests-0.1.0/statistical_tests/tests.py
-drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-04 09:15:05.471415 staty_tests-0.1.0/staty_tests.egg-info/
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1420 2024-05-04 09:15:05.000000 staty_tests-0.1.0/staty_tests.egg-info/PKG-INFO
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      257 2024-05-04 09:15:05.000000 staty_tests-0.1.0/staty_tests.egg-info/SOURCES.txt
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)        1 2024-05-04 09:15:05.000000 staty_tests-0.1.0/staty_tests.egg-info/dependency_links.txt
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       22 2024-05-04 09:15:05.000000 staty_tests-0.1.0/staty_tests.egg-info/requires.txt
--rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       18 2024-05-04 09:15:05.000000 staty_tests-0.1.0/staty_tests.egg-info/top_level.txt
+drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-06 11:11:02.794368 staty_tests-0.2.0/
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1076 2024-05-04 07:20:41.000000 staty_tests-0.2.0/LICENSE
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1420 2024-05-06 11:11:02.794147 staty_tests-0.2.0/PKG-INFO
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      619 2024-05-04 07:23:27.000000 staty_tests-0.2.0/README.md
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       38 2024-05-06 11:11:02.794418 staty_tests-0.2.0/setup.cfg
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      972 2024-05-06 11:09:52.000000 staty_tests-0.2.0/setup.py
+drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-06 11:11:02.792094 staty_tests-0.2.0/statistical_tests/
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-04 07:22:39.000000 staty_tests-0.2.0/statistical_tests/__init__.py
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     2602 2024-05-06 11:09:42.000000 staty_tests-0.2.0/statistical_tests/tests.py
+drwxr-xr-x   0 rtv-lpt-127   (501) staff       (20)        0 2024-05-06 11:11:02.793906 staty_tests-0.2.0/staty_tests.egg-info/
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)     1420 2024-05-06 11:11:02.000000 staty_tests-0.2.0/staty_tests.egg-info/PKG-INFO
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)      257 2024-05-06 11:11:02.000000 staty_tests-0.2.0/staty_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)        1 2024-05-06 11:11:02.000000 staty_tests-0.2.0/staty_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       22 2024-05-06 11:11:02.000000 staty_tests-0.2.0/staty_tests.egg-info/requires.txt
+-rw-r--r--   0 rtv-lpt-127   (501) staff       (20)       18 2024-05-06 11:11:02.000000 staty_tests-0.2.0/staty_tests.egg-info/top_level.txt
```

### Comparing `staty_tests-0.1.0/LICENSE` & `staty_tests-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `staty_tests-0.1.0/PKG-INFO` & `staty_tests-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staty-tests
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for performing statistical tests like ANOVA and chi-square.
 Home-page: https://github.com/solab5/statistical-tests
 Author: Twinomugisha Morris
 Author-email: morristwinomugisha2000@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `staty_tests-0.1.0/README.md` & `staty_tests-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `staty_tests-0.1.0/setup.py` & `staty_tests-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='staty-tests',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     author='Twinomugisha Morris',
     author_email='morristwinomugisha2000@gmail.com',
     description='A Python library for performing statistical tests like ANOVA and chi-square.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/solab5/statistical-tests',
```

### Comparing `staty_tests-0.1.0/statistical_tests/tests.py` & `staty_tests-0.2.0/statistical_tests/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,21 @@
             grouped_data = [data[data[group_var] == group][dependent_variable] for group in unique_groups]
             f_statistic, p_value = f_oneway(*grouped_data)
                 
             # Calculate proportions of each group
             group_sizes = [len(group) for group in grouped_data]
             total_size = sum(group_sizes)
             group_labels = [f"{group_var}={group}" for group in unique_groups]  # Labels for each group
-            group_proportions = [(size / total_size, label) for size, label in zip(group_sizes, group_labels)]
+            # group_proportions = [(size / total_size, label) for size, label in zip(group_sizes, group_labels)]
                 
             results.append({
                 'Dependent Variable': dependent_variable,
                 'Group Variable': group_var,
                 'F-Statistic': f_statistic,
-                'P-value': p_value,
-                'Proportions': group_proportions
+                'P-value': p_value
             })
         
         # Print results in a table
         if results:
             result_table = pd.DataFrame(results)
             print("One-Way ANOVA Results:")
             print(tabulate(result_table, headers='keys', tablefmt='pretty', showindex=False))
```

### Comparing `staty_tests-0.1.0/staty_tests.egg-info/PKG-INFO` & `staty_tests-0.2.0/staty_tests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staty-tests
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for performing statistical tests like ANOVA and chi-square.
 Home-page: https://github.com/solab5/statistical-tests
 Author: Twinomugisha Morris
 Author-email: morristwinomugisha2000@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

