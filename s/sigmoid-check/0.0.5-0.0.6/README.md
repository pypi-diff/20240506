# Comparing `tmp/sigmoid_check-0.0.5.tar.gz` & `tmp/sigmoid_check-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoid_check-0.0.5.tar", last modified: Tue Apr 30 12:27:42 2024, max compression
+gzip compressed data, was "sigmoid_check-0.0.6.tar", last modified: Mon May  6 17:31:52 2024, max compression
```

## Comparing `sigmoid_check-0.0.5.tar` & `sigmoid_check-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.309676 sigmoid_check-0.0.5/
--rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2756 2024-04-30 12:27:42.308674 sigmoid_check-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2024-04-30 12:27:42.316201 sigmoid_check-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1104 2024-04-29 12:54:57.000000 sigmoid_check-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.277739 sigmoid_check-0.0.5/sigmoid_check/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.5/sigmoid_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.294368 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/
--rw-rw-rw-   0        0        0       84 2024-04-24 19:44:04.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.298630 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/__init__.py
--rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.300658 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/__init__.py
--rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.303653 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/
--rw-rw-rw-   0        0        0        0 2024-04-29 12:54:48.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/__init__.py
--rw-rw-rw-   0        0        0    21468 2024-04-30 12:20:28.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/lesson_13.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.306170 sigmoid_check-0.0.5/sigmoid_check.egg-info/
--rw-rw-rw-   0        0        0     2756 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.387037 sigmoid_check-0.0.6/
+-rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2756 2024-05-06 17:31:52.385264 sigmoid_check-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 17:31:52.388312 sigmoid_check-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-05-06 17:30:25.000000 sigmoid_check-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.341917 sigmoid_check-0.0.6/sigmoid_check/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.6/sigmoid_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.362411 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/
+-rw-rw-rw-   0        0        0      170 2024-05-05 08:15:26.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.367203 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_10/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_10/__init__.py
+-rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.371213 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_11/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_11/__init__.py
+-rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.376212 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_13/
+-rw-rw-rw-   0        0        0        0 2024-04-29 12:54:48.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_13/__init__.py
+-rw-rw-rw-   0        0        0    21468 2024-04-30 12:20:28.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_13/lesson_13.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.380252 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_14/
+-rw-rw-rw-   0        0        0        0 2024-05-05 08:14:58.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_14/__init__.py
+-rw-rw-rw-   0        0        0    13394 2024-05-06 17:28:23.000000 sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_14/lesson_14.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:31:52.382252 sigmoid_check-0.0.6/sigmoid_check.egg-info/
+-rw-rw-rw-   0        0        0     2756 2024-05-06 17:31:52.000000 sigmoid_check-0.0.6/sigmoid_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2024-05-06 17:31:52.000000 sigmoid_check-0.0.6/sigmoid_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:31:52.000000 sigmoid_check-0.0.6/sigmoid_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-06 17:31:52.000000 sigmoid_check-0.0.6/sigmoid_check.egg-info/top_level.txt
```

### Comparing `sigmoid_check-0.0.5/LICENSE` & `sigmoid_check-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.5/PKG-INFO` & `sigmoid_check-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.5/README.md` & `sigmoid_check-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.5/setup.py` & `sigmoid_check-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="sigmoid_check",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     description="A package for checking the implementation of tasks in Sigmoid Courses",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SigmoidAI - Balamatiuc Eduard",
     author_email="balamatiuc2@gmail.com",
     keywords=["tasks", "check", "sigmoid", "sigmoidai", "sigmoid_check"],
```

### Comparing `sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/lesson_10.py` & `sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_10/lesson_10.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/lesson_11.py` & `sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_11/lesson_11.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/lesson_13.py` & `sigmoid_check-0.0.6/sigmoid_check/python_odyssey/lesson_13/lesson_13.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.5/sigmoid_check.egg-info/PKG-INFO` & `sigmoid_check-0.0.6/sigmoid_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.5/sigmoid_check.egg-info/SOURCES.txt` & `sigmoid_check-0.0.6/sigmoid_check.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 sigmoid_check.egg-info/top_level.txt
 sigmoid_check/python_odyssey/__init__.py
 sigmoid_check/python_odyssey/lesson_10/__init__.py
 sigmoid_check/python_odyssey/lesson_10/lesson_10.py
 sigmoid_check/python_odyssey/lesson_11/__init__.py
 sigmoid_check/python_odyssey/lesson_11/lesson_11.py
 sigmoid_check/python_odyssey/lesson_13/__init__.py
-sigmoid_check/python_odyssey/lesson_13/lesson_13.py
+sigmoid_check/python_odyssey/lesson_13/lesson_13.py
+sigmoid_check/python_odyssey/lesson_14/__init__.py
+sigmoid_check/python_odyssey/lesson_14/lesson_14.py
```

