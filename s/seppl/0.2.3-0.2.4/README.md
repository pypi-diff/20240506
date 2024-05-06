# Comparing `tmp/seppl-0.2.3.tar.gz` & `tmp/seppl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppl-0.2.3.tar", last modified: Fri May  3 02:24:41 2024, max compression
+gzip compressed data, was "seppl-0.2.4.tar", last modified: Mon May  6 01:33:37 2024, max compression
```

## Comparing `seppl-0.2.3.tar` & `seppl-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.015680 seppl-0.2.3/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4636 2024-05-03 02:23:46.000000 seppl-0.2.3/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.2.3/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.2.3/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6997 2024-05-03 02:24:41.015680 seppl-0.2.3/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3741 2024-05-01 21:38:44.000000 seppl-0.2.3/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-03 02:24:41.015680 seppl-0.2.3/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-05-03 02:23:46.000000 seppl-0.2.3/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.011680 seppl-0.2.3/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.011680 seppl-0.2.3/src/seppl/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-04-30 23:53:36.000000 seppl-0.2.3/src/seppl/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.2.3/src/seppl/_args.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    16741 2024-05-03 02:00:38.000000 seppl-0.2.3/src/seppl/_class_registry.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.2.3/src/seppl/_entry_points.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.2.3/src/seppl/_help.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.2.3/src/seppl/_metadata.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.2.3/src/seppl/_plugin.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15743 2024-04-30 23:41:51.000000 seppl-0.2.3/src/seppl/_registry.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.2.3/src/seppl/_session.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.2.3/src/seppl/_types.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.015680 seppl-0.2.3/src/seppl/io/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.2.3/src/seppl/io/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5459 2024-05-03 02:05:32.000000 seppl-0.2.3/src/seppl/io/_execution.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.2.3/src/seppl/io/_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.2.3/src/seppl/io/_reader.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.2.3/src/seppl/io/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.2.3/src/seppl/io/_utils.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.2.3/src/seppl/io/_writer.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.015680 seppl-0.2.3/src/seppl/tool/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.2.3/src/seppl/tool/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.2.3/src/seppl/tool/escape.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.2.3/src/seppl/tool/unescape.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:24:41.015680 seppl-0.2.3/src/seppl.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6997 2024-05-03 02:24:40.000000 seppl-0.2.3/src/seppl.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      700 2024-05-03 02:24:40.000000 seppl-0.2.3/src/seppl.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-03 02:24:40.000000 seppl-0.2.3/src/seppl.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-05-03 02:24:40.000000 seppl-0.2.3/src/seppl.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-05-03 02:24:40.000000 seppl-0.2.3/src/seppl.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.701107 seppl-0.2.4/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4710 2024-05-06 01:32:31.000000 seppl-0.2.4/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      568 2023-11-09 01:56:09.000000 seppl-0.2.4/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 seppl-0.2.4/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7119 2024-05-06 01:33:37.701107 seppl-0.2.4/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3741 2024-05-01 21:38:44.000000 seppl-0.2.4/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-06 01:33:37.701107 seppl-0.2.4/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1130 2024-05-06 01:32:31.000000 seppl-0.2.4/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.697107 seppl-0.2.4/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.701107 seppl-0.2.4/src/seppl/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      765 2024-04-30 23:53:36.000000 seppl-0.2.4/src/seppl/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5702 2024-02-21 21:20:08.000000 seppl-0.2.4/src/seppl/_args.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    17165 2024-05-06 01:31:34.000000 seppl-0.2.4/src/seppl/_class_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1719 2023-10-04 19:59:54.000000 seppl-0.2.4/src/seppl/_entry_points.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2876 2023-10-04 20:28:17.000000 seppl-0.2.4/src/seppl/_help.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1942 2024-02-04 21:21:35.000000 seppl-0.2.4/src/seppl/_metadata.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8347 2024-02-28 19:32:25.000000 seppl-0.2.4/src/seppl/_plugin.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15743 2024-04-30 23:41:51.000000 seppl-0.2.4/src/seppl/_registry.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1679 2024-02-04 21:33:05.000000 seppl-0.2.4/src/seppl/_session.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2623 2024-02-28 19:32:25.000000 seppl-0.2.4/src/seppl/_types.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.701107 seppl-0.2.4/src/seppl/io/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      282 2024-02-05 00:23:10.000000 seppl-0.2.4/src/seppl/io/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5459 2024-05-03 02:05:32.000000 seppl-0.2.4/src/seppl/io/_execution.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6560 2024-02-04 23:34:50.000000 seppl-0.2.4/src/seppl/io/_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1555 2024-02-04 23:40:54.000000 seppl-0.2.4/src/seppl/io/_reader.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3147 2024-02-07 03:48:04.000000 seppl-0.2.4/src/seppl/io/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2444 2024-02-05 00:23:10.000000 seppl-0.2.4/src/seppl/io/_utils.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3319 2024-02-04 23:40:54.000000 seppl-0.2.4/src/seppl/io/_writer.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.701107 seppl-0.2.4/src/seppl/tool/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-21 20:25:44.000000 seppl-0.2.4/src/seppl/tool/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      772 2024-02-21 20:32:02.000000 seppl-0.2.4/src/seppl/tool/escape.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      780 2024-02-21 20:32:02.000000 seppl-0.2.4/src/seppl/tool/unescape.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-06 01:33:37.701107 seppl-0.2.4/src/seppl.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7119 2024-05-06 01:33:37.000000 seppl-0.2.4/src/seppl.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      700 2024-05-06 01:33:37.000000 seppl-0.2.4/src/seppl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-06 01:33:37.000000 seppl-0.2.4/src/seppl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      107 2024-05-06 01:33:37.000000 seppl-0.2.4/src/seppl.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2024-05-06 01:33:37.000000 seppl-0.2.4/src/seppl.egg-info/top_level.txt
```

### Comparing `seppl-0.2.3/CHANGES.rst` & `seppl-0.2.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
-0.2.3 (2024-05-3)
+0.2.4 (2024-05-06)
+------------------
+
+- reworked excluding of classes
+
+
+0.2.3 (2024-05-03)
 ------------------
 
 - `_determine_from_entry_points` method of `ClassListerRegistry` class now checks whether
   there the attributes tuple has any elements (i.e., whether the optional `:function_name`
   was provided)
 - message `X records processed in total` now only output at the end
```

### Comparing `seppl-0.2.3/DESCRIPTION.rst` & `seppl-0.2.4/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/PKG-INFO` & `seppl-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,15 +18,21 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
-        0.2.3 (2024-05-3)
+        0.2.4 (2024-05-06)
+        ------------------
+        
+        - reworked excluding of classes
+        
+        
+        0.2.3 (2024-05-03)
         ------------------
         
         - `_determine_from_entry_points` method of `ClassListerRegistry` class now checks whether
           there the attributes tuple has any elements (i.e., whether the optional `:function_name`
           was provided)
         - message `X records processed in total` now only output at the end
```

### Comparing `seppl-0.2.3/README.md` & `seppl-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/setup.py` & `seppl-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'Programming Language :: Python :: 3',
     ],
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=find_namespace_packages(where='src'),
-    version="0.2.3",
+    version="0.2.4",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
             "seppl-escape=seppl.tool.escape:sys_main",
             "seppl-unescape=seppl.tool.unescape:sys_main",
         ],
```

### Comparing `seppl-0.2.3/src/seppl/__init__.py` & `seppl-0.2.4/src/seppl/__init__.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_args.py` & `seppl-0.2.4/src/seppl/_args.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_class_registry.py` & `seppl-0.2.4/src/seppl/_class_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,22 +319,28 @@
         :type class_listers: list
         :return: the determined list of subclasses
         :rtype: list
         """
         result = []
 
         if len(class_listers) > 0:
-            try:
-                cls = get_class(c)
-            except:
-                print("Failed to instantiate class: %s" % c, file=sys.stderr)
-                traceback.print_exc()
-                return result
+            cls = None
 
             for class_lister in class_listers:
+                if class_lister == "":
+                    continue
+
+                if cls is None:
+                    try:
+                        cls = get_class(c)
+                    except:
+                        print("Failed to instantiate class: %s" % c, file=sys.stderr)
+                        traceback.print_exc()
+                        return result
+
                 try:
                     func = get_class_lister(class_lister)
                 except:
                     print("Problem encountered with class lister: %s" % class_lister, file=sys.stderr)
                     traceback.print_exc()
                     continue
 
@@ -381,15 +387,16 @@
         :type c: str
         :return: the determined list of subclasses
         :rtype: list
         """
         result = []
 
         if os.getenv(self.env_class_listers) is not None:
-            # format: "module:function,module:function,...",
+            # format: "classlister1,classlister2,..."
+            # classlister format: "module_name:function_name" or "module_name" if "list_classes" as method
             class_listers = os.getenv(self.env_class_listers).split(",")
             result = self._determine_from_class_listers(c, class_listers)
 
         return result
 
     def _initialize(self, c: str):
         """
@@ -406,19 +413,23 @@
         entry_point_classes = self._determine_from_entry_points(c)
         if entry_point_classes is not None:
             all_classes.update(entry_point_classes)
 
         # register from class listers as well?
         if (len(all_classes) == 0) or ((self._custom_class_listers is not None) and (len(self._custom_class_listers) > 0)) or self.has_env_class_listers():
             actual = self.actual_fallback_class_listers()
-            for excl in self.actual_excluded_class_listers():
-                if excl in actual:
-                    actual.remove(excl)
             all_classes.update(self._determine_from_class_listers(c, actual))
 
+        # excluded classes?
+        excluded_listers = self.actual_excluded_class_listers()
+        excluded_classes = self._determine_from_class_listers(c, excluded_listers)
+        for cls in excluded_classes:
+            if cls in all_classes:
+                all_classes.remove(cls)
+
         self._classes[c] = sorted(list(all_classes))
 
     def plugins(self, c: Union[str, Type], fail_if_empty: bool = True) -> Dict[str, Plugin]:
         """
         Returns the classes for the specified superclass.
 
         :param c: the super class to get the derived classes for (classname or type)
```

### Comparing `seppl-0.2.3/src/seppl/_entry_points.py` & `seppl-0.2.4/src/seppl/_entry_points.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_help.py` & `seppl-0.2.4/src/seppl/_help.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_metadata.py` & `seppl-0.2.4/src/seppl/_metadata.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_plugin.py` & `seppl-0.2.4/src/seppl/_plugin.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_registry.py` & `seppl-0.2.4/src/seppl/_registry.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_session.py` & `seppl-0.2.4/src/seppl/_session.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/_types.py` & `seppl-0.2.4/src/seppl/_types.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_execution.py` & `seppl-0.2.4/src/seppl/io/_execution.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_filter.py` & `seppl-0.2.4/src/seppl/io/_filter.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_reader.py` & `seppl-0.2.4/src/seppl/io/_reader.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_split.py` & `seppl-0.2.4/src/seppl/io/_split.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_utils.py` & `seppl-0.2.4/src/seppl/io/_utils.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/io/_writer.py` & `seppl-0.2.4/src/seppl/io/_writer.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/tool/escape.py` & `seppl-0.2.4/src/seppl/tool/escape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl/tool/unescape.py` & `seppl-0.2.4/src/seppl/tool/unescape.py`

 * *Files identical despite different names*

### Comparing `seppl-0.2.3/src/seppl.egg-info/PKG-INFO` & `seppl-0.2.4/src/seppl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: seppl
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python3 library for parsing pipeline components with their own options.
 Home-page: https://github.com/waikato-datamining/seppl
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Simple Entry Point PipeLines (seppl). Python library for parsing pipeline components with their own options. 
         
@@ -18,15 +18,21 @@
         
         `https://github.com/waikato-datamining/seppl <https://github.com/waikato-datamining/seppl>`__
         
         
         Changelog
         =========
         
-        0.2.3 (2024-05-3)
+        0.2.4 (2024-05-06)
+        ------------------
+        
+        - reworked excluding of classes
+        
+        
+        0.2.3 (2024-05-03)
         ------------------
         
         - `_determine_from_entry_points` method of `ClassListerRegistry` class now checks whether
           there the attributes tuple has any elements (i.e., whether the optional `:function_name`
           was provided)
         - message `X records processed in total` now only output at the end
```

### Comparing `seppl-0.2.3/src/seppl.egg-info/SOURCES.txt` & `seppl-0.2.4/src/seppl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

