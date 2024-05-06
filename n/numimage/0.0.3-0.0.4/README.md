# Comparing `tmp/numimage-0.0.3.tar.gz` & `tmp/numimage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numimage-0.0.3.tar", last modified: Sun Apr 28 06:59:57 2024, max compression
+gzip compressed data, was "numimage-0.0.4.tar", last modified: Mon May  6 08:10:59 2024, max compression
```

## Comparing `numimage-0.0.3.tar` & `numimage-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:59:57.594489 numimage-0.0.3/
--rw-rw-rw-   0        0        0     1073 2020-03-05 23:01:44.000000 numimage-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3022 2024-04-28 06:59:57.594489 numimage-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2024-04-28 06:37:33.000000 numimage-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 06:59:57.586515 numimage-0.0.3/numimage/
--rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.3/numimage/__init__.py
--rw-rw-rw-   0        0        0     5546 2024-04-28 06:31:49.000000 numimage-0.0.3/numimage/geometry.py
--rw-rw-rw-   0        0        0      142 2024-04-26 09:14:23.000000 numimage-0.0.3/numimage/math_h.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:59:57.593492 numimage-0.0.3/numimage.egg-info/
--rw-rw-rw-   0        0        0     3022 2024-04-28 06:59:57.000000 numimage-0.0.3/numimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-28 06:59:57.000000 numimage-0.0.3/numimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:59:57.000000 numimage-0.0.3/numimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-28 06:59:57.000000 numimage-0.0.3/numimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 06:59:57.000000 numimage-0.0.3/numimage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:59:57.594489 numimage-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2064 2024-04-28 06:59:26.000000 numimage-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:59:57.593492 numimage-0.0.3/string_h/
--rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.3/string_h/__init__.py
--rw-rw-rw-   0        0        0       48 2020-03-05 23:01:44.000000 numimage-0.0.3/string_h/reverse.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:59.921440 numimage-0.0.4/
+-rw-rw-rw-   0        0        0     1073 2020-03-05 23:01:44.000000 numimage-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3022 2024-05-06 08:10:59.921440 numimage-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2024-04-28 06:37:33.000000 numimage-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:59.910551 numimage-0.0.4/configurations/
+-rw-rw-rw-   0        0        0       21 2024-02-22 07:43:10.000000 numimage-0.0.4/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-03-27 03:16:53.000000 numimage-0.0.4/configurations/config.py
+-rw-rw-rw-   0        0        0    65297 2024-04-28 03:32:01.000000 numimage-0.0.4/configurations/template_editor_config.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:59.914252 numimage-0.0.4/numimage/
+-rw-rw-rw-   0        0        0      183 2024-05-06 07:57:56.000000 numimage-0.0.4/numimage/__init__.py
+-rw-rw-rw-   0        0        0     1351 2024-05-06 02:19:16.000000 numimage-0.0.4/numimage/color_picker.py
+-rw-rw-rw-   0        0        0     5546 2024-04-28 06:31:49.000000 numimage-0.0.4/numimage/geometry.py
+-rw-rw-rw-   0        0        0     1881 2024-05-06 07:14:12.000000 numimage-0.0.4/numimage/getsvgrect.py
+-rw-rw-rw-   0        0        0     6100 2024-05-06 03:56:12.000000 numimage-0.0.4/numimage/outline.py
+-rw-rw-rw-   0        0        0     3504 2024-04-28 07:41:46.000000 numimage-0.0.4/numimage/potrace.py
+-rw-rw-rw-   0        0        0     3775 2024-04-28 07:41:49.000000 numimage-0.0.4/numimage/proc_bbox.py
+-rw-rw-rw-   0        0        0    19862 2024-05-06 03:40:01.000000 numimage-0.0.4/numimage/proc_color.py
+-rw-rw-rw-   0        0        0    28691 2024-04-28 07:42:14.000000 numimage-0.0.4/numimage/proc_image.py
+-rw-rw-rw-   0        0        0     1595 2024-04-28 07:42:17.000000 numimage-0.0.4/numimage/proc_points.py
+-rw-rw-rw-   0        0        0    40144 2024-04-28 08:01:12.000000 numimage-0.0.4/numimage/reverse_logo.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:59.921440 numimage-0.0.4/numimage.egg-info/
+-rw-rw-rw-   0        0        0     3022 2024-05-06 08:10:59.000000 numimage-0.0.4/numimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-06 08:10:59.000000 numimage-0.0.4/numimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:10:59.000000 numimage-0.0.4/numimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 08:10:59.000000 numimage-0.0.4/numimage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-05-06 08:10:59.000000 numimage-0.0.4/numimage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:10:59.921440 numimage-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2064 2024-05-06 08:10:48.000000 numimage-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:10:59.920443 numimage-0.0.4/string_h/
+-rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.4/string_h/__init__.py
+-rw-rw-rw-   0        0        0       48 2020-03-05 23:01:44.000000 numimage-0.0.4/string_h/reverse.py
```

### Comparing `numimage-0.0.3/LICENSE.txt` & `numimage-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numimage-0.0.3/PKG-INFO` & `numimage-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numimage
-Version: 0.0.3
+Version: 0.0.4
 Summary: 验证打包功能的测试包, 请勿下载
 Home-page: https://github.com/JackyFuHk/numimage
 Author: JackyFu
 Author-email: 343651570@qq.com
 License: MIT
 Keywords: jacky package demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `numimage-0.0.3/README.md` & `numimage-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `numimage-0.0.3/numimage/geometry.py` & `numimage-0.0.4/numimage/geometry.py`

 * *Files identical despite different names*

### Comparing `numimage-0.0.3/numimage.egg-info/PKG-INFO` & `numimage-0.0.4/numimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numimage
-Version: 0.0.3
+Version: 0.0.4
 Summary: 验证打包功能的测试包, 请勿下载
 Home-page: https://github.com/JackyFuHk/numimage
 Author: JackyFu
 Author-email: 343651570@qq.com
 License: MIT
 Keywords: jacky package demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `numimage-0.0.3/setup.py` & `numimage-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包名
     name="numimage",
     # 版本(也可以用日期表示 2020.3.1 这样每次提交不需要在改版本)
-    version="0.0.3",
+    version="0.0.4",
     # 作者
     author="JackyFu",
     # 作者邮箱
     author_email="343651570@qq.com",
     # 包的说明(这个要正规,会展示出来, 列表页灰色横幅可见)
     description="验证打包功能的测试包, 请勿下载",
     # 项目描述
```

