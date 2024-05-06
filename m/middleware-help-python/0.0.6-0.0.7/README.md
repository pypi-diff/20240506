# Comparing `tmp/middleware-help-python-0.0.6.tar.gz` & `tmp/middleware-help-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.6.tar", last modified: Mon Apr 29 08:51:19 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.7.tar", last modified: Mon May  6 15:19:58 2024, max compression
```

## Comparing `middleware-help-python-0.0.6.tar` & `middleware-help-python-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:51:19.353317 middleware-help-python-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      543 2024-04-29 08:51:19.351348 middleware-help-python-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:51:19.350340 middleware-help-python-0.0.6/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      543 2024-04-29 08:51:19.000000 middleware-help-python-0.0.6/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-29 08:51:19.000000 middleware-help-python-0.0.6/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:51:19.000000 middleware-help-python-0.0.6/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-29 08:51:19.000000 middleware-help-python-0.0.6/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 08:51:19.000000 middleware-help-python-0.0.6/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 08:51:19.348358 middleware-help-python-0.0.6/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.6/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0     3819 2024-04-29 08:33:44.000000 middleware-help-python-0.0.6/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.6/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.6/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-04-29 08:51:19.353317 middleware-help-python-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-04-29 08:51:14.000000 middleware-help-python-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.692155 middleware-help-python-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      543 2024-05-06 15:19:58.691158 middleware-help-python-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.689164 middleware-help-python-0.0.7/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.686196 middleware-help-python-0.0.7/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.7/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2024-05-06 15:13:25.000000 middleware-help-python-0.0.7/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.7/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.7/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:19:58.692155 middleware-help-python-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-06 15:12:36.000000 middleware-help-python-0.0.7/setup.py
```

### Comparing `middleware-help-python-0.0.6/LICENSE` & `middleware-help-python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.6/PKG-INFO` & `middleware-help-python-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.6/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.7/middleware_help_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.6/middleware_helper/mysql.py` & `middleware-help-python-0.0.7/middleware_helper/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,16 @@
             print("当前连接不正常.")
         return results
 
     @classmethod
     def convert_key_value_str(cls, **kwargs) -> tuple:
         field_list, value_list = list(), list()
         for key, value in kwargs.items():
+            if value is None:
+                value = ''
             field_list.append("`{}`".format(key))
             if isinstance(value, str):
                 value = "'{}'".format(value)
             else:
                 value = str(value)
             value_list.append(value)
         field_str = "(" + ", ".join(field_list) + ")"
```

### Comparing `middleware-help-python-0.0.6/middleware_helper/network.py` & `middleware-help-python-0.0.7/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.6/middleware_helper/redis.py` & `middleware-help-python-0.0.7/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.6/setup.py` & `middleware-help-python-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.6',
+    version='0.0.7',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

