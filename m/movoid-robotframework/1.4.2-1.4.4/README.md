# Comparing `tmp/movoid_robotframework-1.4.2.tar.gz` & `tmp/movoid_robotframework-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.2.tar", last modified: Thu Apr 25 13:56:54 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.4.tar", last modified: Mon May  6 14:31:37 2024, max compression
```

## Comparing `movoid_robotframework-1.4.2.tar` & `movoid_robotframework-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:56:54.936854 movoid_robotframework-1.4.2/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-04-25 13:56:54.935857 movoid_robotframework-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 13:56:54.924400 movoid_robotframework-1.4.2/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:56:54.928391 movoid_robotframework-1.4.2/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     8305 2024-04-25 13:54:33.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     4476 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.2/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:56:54.934861 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-04-25 13:56:54.000000 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-25 13:56:54.000000 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:56:54.000000 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-25 13:56:54.000000 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-25 13:56:54.000000 movoid_robotframework-1.4.2/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 13:56:54.936854 movoid_robotframework-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-25 13:52:02.000000 movoid_robotframework-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.816159 movoid_robotframework-1.4.4/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-05-06 14:31:37.814176 movoid_robotframework-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.797222 movoid_robotframework-1.4.4/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.803203 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     8305 2024-04-25 13:54:33.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     6654 2024-05-06 14:28:24.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.813169 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:31:37.816159 movoid_robotframework-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-05-06 14:29:51.000000 movoid_robotframework-1.4.4/setup.py
```

### Comparing `movoid_robotframework-1.4.2/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.4/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.2/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.4/RobotFrameworkBasic/action/config.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.2/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.4/RobotFrameworkBasic/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # -*- coding: utf-8 -*-
 """
 # File          : common
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/2/13 12:04
 # Description   : 
 """
+import base64
 import json
+import traceback
+from typing import Union
 
 from robot.libraries.BuiltIn import BuiltIn
 
 from .decorator import robot_log_keyword
 from .error import RfError
 from .version import VERSION
 
@@ -122,7 +125,54 @@
         if suite:
             sc_list.append(self.get_robot_variable('SUITE NAME'))
         if case:
             temp = self.get_robot_variable('TEST NAME')
             if temp is not None:
                 sc_list.append(self.get_robot_variable('TEST NAME'))
         return join_str.join(sc_list)
+
+    @robot_log_keyword
+    def log_show_image(self, image_path: str):
+        with open(image_path, mode='rb') as f:
+            img_str = base64.b64encode(f.read()).decode()
+            self.print(f'<img src="data:image/png;base64,{img_str}">', html=True)
+
+    @robot_log_keyword
+    def robot_check_param(self, param_str: str, param_style: Union[str, type], default=None, error=False):
+        if type(param_style) is str:
+            param_style_str = param_style.lower()
+        elif type(param_style) is type:
+            param_style_str = param_style.__name__
+        else:
+            error_text = f'what is <{param_style}>({type(param_style).__name__}) which is not str or type?'
+            if error:
+                raise TypeError(error_text)
+            else:
+                return default
+        self.print(f'try to change <{param_str}> to {param_style}')
+        try:
+            if param_style_str in ('str',):
+                re_value = str(param_str)
+            elif param_style_str in ('int',):
+                re_value = int(param_str)
+            elif param_style_str in ('float',):
+                re_value = float(param_str)
+            elif param_style_str in ('bool',):
+                if param_str in ('true',):
+                    re_value = True
+                elif param_str in ('false',):
+                    re_value = False
+                else:
+                    self.print(f'{param_str} is not a traditional bool, we use forced conversion.')
+                    re_value = bool(param_str)
+            else:
+                re_value = eval(f'{param_style_str}({param_str})')
+        except Exception as err:
+            error_text = f'something wrong happened when we change <{param_str}> to <{param_style_str}>:\n{traceback.format_exc()}'
+            if error:
+                self.error(error_text)
+                raise err
+            else:
+                self.print(error_text)
+                self.print(f'we use default value:<{default}>({type(default).__name__})')
+                re_value = default
+        return re_value
```

### Comparing `movoid_robotframework-1.4.2/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.4/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.2/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.4/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.2/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.4/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.2/setup.py` & `movoid_robotframework-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.2',
+    version='1.4.4',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

