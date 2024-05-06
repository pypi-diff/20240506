# Comparing `tmp/pkg_inspect-0.1.5.tar.gz` & `tmp/pkg_inspect-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.1.5.tar", last modified: Mon May  6 01:09:03 2024, max compression
+gzip compressed data, was "pkg_inspect-0.1.6.tar", last modified: Mon May  6 01:31:39 2024, max compression
```

## Comparing `pkg_inspect-0.1.5.tar` & `pkg_inspect-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.772885 pkg_inspect-0.1.5/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.5/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.5/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:09:03.772595 pkg_inspect-0.1.5/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.5/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-06 01:09:03.773862 pkg_inspect-0.1.5/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.5/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.762380 pkg_inspect-0.1.5/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      193 2024-05-06 01:06:55.000000 pkg_inspect-0.1.5/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.762718 pkg_inspect-0.1.5/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      104 2024-05-05 20:43:34.000000 pkg_inspect-0.1.5/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.765812 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-05 19:21:33.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13168 2024-05-06 00:56:09.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.767835 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47522 2024-05-05 20:43:35.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-05 18:27:31.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47426 2024-05-05 20:43:35.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.770755 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-05-05 19:26:25.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5393 2024-05-06 01:05:02.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/cli.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49212 2024-05-06 00:55:19.000000 pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.764759 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      735 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-06 01:09:03.000000 pkg_inspect-0.1.5/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:09:03.771751 pkg_inspect-0.1.5/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.5/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.1.5/tests/test_pkg_inspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.709761 pkg_inspect-0.1.6/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.6/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.6/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:31:39.709469 pkg_inspect-0.1.6/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.6/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-06 01:31:39.710611 pkg_inspect-0.1.6/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.6/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.699264 pkg_inspect-0.1.6/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      193 2024-05-06 01:29:53.000000 pkg_inspect-0.1.6/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.699779 pkg_inspect-0.1.6/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      104 2024-05-05 20:43:34.000000 pkg_inspect-0.1.6/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.702774 pkg_inspect-0.1.6/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-05 19:21:33.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13168 2024-05-06 00:56:09.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.704790 pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47582 2024-05-06 01:28:42.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-05 18:27:31.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47426 2024-05-05 20:43:35.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.707555 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-05-05 19:26:25.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5393 2024-05-06 01:05:02.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/cli.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49212 2024-05-06 00:55:19.000000 pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.701918 pkg_inspect-0.1.6/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-06 01:31:39.000000 pkg_inspect-0.1.6/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      735 2024-05-06 01:31:39.000000 pkg_inspect-0.1.6/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-06 01:31:39.000000 pkg_inspect-0.1.6/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-06 01:31:39.000000 pkg_inspect-0.1.6/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-06 01:31:39.708643 pkg_inspect-0.1.6/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.6/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.1.6/tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.1.5/LICENSE.md` & `pkg_inspect-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/PKG-INFO` & `pkg_inspect-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.1.5
+Version: 0.1.6
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.5/README.md` & `pkg_inspect-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/setup.cfg` & `pkg_inspect-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.1.5
+version = 0.1.6
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A comprehensive tools to inspect Python packages and Python installations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_functions/functions.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     @staticmethod
     def _vparser(v) -> PackageVersion:
         return PkgV.parse_version(v)
 
     @staticmethod
     def _fix_pkgname(pkg_name: str = None) -> str:
         if pkg_name:
-            return stranslate(pkg_name, "_", "-")
+            return stranslate(pkg_name, "-", "_")
 
     @classmethod
     @exception_handler("site-path version number", exceptions=StopIteration)
     def _get_version_num(
         cls,
         site_path: Union[Path, str],
         dist_ver: bool = False,
@@ -249,15 +249,17 @@
             - `str`: The package name for the specified Python version.
 
         #### Raises:
             - `PkgException`: If the package is not found in the specified Python version.
 
         """
         py_version: PackageVersion = self._check_version(py_version)
+        # print(package_name)
         package_name: str = self._fix_pkgname(package_name)
+        # print(package_name)
         try:
             # Check if the package is found in the specified Python version
             return next(
                 pkg
                 for pkg in self._get_package_names(
                     py_version=py_version, return_as_paths=False
                 )
```

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/cli.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/cli.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.1.6/src/pkg_inspect/pkg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.1.6/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.1.5
+Version: 0.1.6
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.5/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.1.6/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.5/tests/test_pkg_inspect.py` & `pkg_inspect-0.1.6/tests/test_pkg_inspect.py`

 * *Files identical despite different names*

