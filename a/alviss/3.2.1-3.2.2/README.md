# Comparing `tmp/alviss-3.2.1.tar.gz` & `tmp/alviss-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alviss-3.2.1.tar", last modified: Tue Apr 30 10:09:22 2024, max compression
+gzip compressed data, was "alviss-3.2.2.tar", last modified: Mon May  6 13:44:24 2024, max compression
```

## Comparing `alviss-3.2.1.tar` & `alviss-3.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 10:09:12.000000 alviss-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-30 10:09:22.769177 alviss-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-30 10:09:12.000000 alviss-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/render/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/stubber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/stubber/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/autoloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17478 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/jsonfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/yamlfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/quickloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/renderers/static/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/cfgstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/singletonconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss/stubber/stubmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/utils/kwfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 10:09:12.000000 alviss-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:09:22.769177 alviss-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 10:09:12.000000 alviss-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.147643 alviss-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 13:44:08.000000 alviss-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-06 13:44:24.147643 alviss-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-06 13:44:08.000000 alviss-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/stubber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/stubber/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/autoloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17478 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/jsonfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/yamlfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/quickloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/renderers/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/cfgstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/singletonconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/stubber/stubmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/utils/kwfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 13:44:08.000000 alviss-3.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:44:24.147643 alviss-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 13:44:08.000000 alviss-3.2.2/setup.py
```

### Comparing `alviss-3.2.1/LICENSE` & `alviss-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/PKG-INFO` & `alviss-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.1
+Version: 3.2.2
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.1/README.md` & `alviss-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/cli/render/main.py` & `alviss-3.2.2/alviss/cli/render/main.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/cli/stubber/main.py` & `alviss-3.2.2/alviss/cli/stubber/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,33 @@
     if args.verbose:
         import logging
         logging.basicConfig(level=logging.DEBUG)
 
     if not args.silent:
         print(f'Reading and stubbing file: {args.file}...')
 
+    cls_name = 'AlvissConfigStub' if args.class_name is None else args.class_name
+    if cls_name.lower().strip() == 'none':
+        cls_name = ''
+
     try:
         if args.output:
             if not args.silent:
                 print(f'Writing output to: {args.output}...')
 
             stubber.SimpleStubMaker().render_stub_classes_to_file(input_file=args.file,
                                                                   output_file=args.output,
                                                                   overwrite_existing=args.force_overwrite,
-                                                                  is_private=not args.export_all)
+                                                                  is_private=not args.export_all,
+                                                                  class_name=cls_name)
         else:
             if not args.silent:
                 print(f'Printing results:')
                 print(f'==================================================')
-            cls_name = 'AlvissConfigStub' if args.class_name is None else args.class_name
-            if cls_name.lower().strip() == 'none':
-                cls_name = ''
+
             print(stubber.SimpleStubMaker().render_stub_classes_from_descriptor_file(args.file, class_name=cls_name, is_private=not args.export_all))
 
             if not args.silent:
                 print(f'==================================================')
 
         if not args.silent:
             print(f'Done!')
```

### Comparing `alviss-3.2.1/alviss/loaders/autoloader.py` & `alviss-3.2.2/alviss/loaders/autoloader.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/loaders/base.py` & `alviss-3.2.2/alviss/loaders/base.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/loaders/interface.py` & `alviss-3.2.2/alviss/loaders/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/loaders/jsonfile.py` & `alviss-3.2.2/alviss/loaders/jsonfile.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/loaders/yamlfile.py` & `alviss-3.2.2/alviss/loaders/yamlfile.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/renderers/static/_simple.py` & `alviss-3.2.2/alviss/renderers/static/_simple.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/renderers/static/interface.py` & `alviss-3.2.2/alviss/renderers/static/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/structs/baseconfig.py` & `alviss-3.2.2/alviss/structs/baseconfig.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/structs/errors.py` & `alviss-3.2.2/alviss/structs/errors.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/stubber/stubmaker/_simple.py` & `alviss-3.2.2/alviss/stubber/stubmaker/_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
 from alviss.structs import Empty
 from alviss.structs.cfgstub import _BaseCfgStub
 from alviss.structs import BaseConfig
 
 
 {class_str}{root_cls}"""
 
-    def render_stub_classes_to_file(self, input_file: str, output_file: str, overwrite_existing: bool = False, is_private: bool = True):
+    def render_stub_classes_to_file(self, input_file: str, output_file: str, overwrite_existing: bool = False, is_private: bool = True, class_name: str = 'AlvissConfigStub'):
         out = pathlib.Path(output_file).absolute()
         if out.exists() and not overwrite_existing:
             raise AlvissFileAlreadyExistsError('Output file already exists', file_name=output_file)
 
-        results = self.render_stub_classes_from_descriptor_file(input_file, is_private=is_private)
+        results = self.render_stub_classes_from_descriptor_file(input_file, is_private=is_private, class_name=class_name)
 
         if not out.parent.exists():
             log.debug(f'Creating output path: {out.parent}')
             os.makedirs(out.parent, exist_ok=True)
 
         with open(output_file, 'w') as fin:
             fin.write(results)
```

### Comparing `alviss-3.2.1/alviss/stubber/stubmaker/_structs.py` & `alviss-3.2.2/alviss/stubber/stubmaker/_structs.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss/stubber/stubmaker/interface.py` & `alviss-3.2.2/alviss/stubber/stubmaker/interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,12 +11,13 @@
         """Renders a Python module file with type hinting stub classes from the
         Alviss config type descriptor file.
         """
         pass
 
     @abc.abstractmethod
     def render_stub_classes_to_file(self, input_file: str, output_file: str,
-                                    overwrite_existing: bool = False, is_private: bool = True):
+                                    overwrite_existing: bool = False, is_private: bool = True,
+                                    class_name: str = 'AlvissConfigStub'):
         """Writer the results of the `render_stub_classes_from_descriptor_file`
         call to the given output file.
         """
         pass
```

### Comparing `alviss-3.2.1/alviss/utils/kwfields.py` & `alviss-3.2.2/alviss/utils/kwfields.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/alviss.egg-info/PKG-INFO` & `alviss-3.2.2/alviss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.1
+Version: 3.2.2
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.1/alviss.egg-info/SOURCES.txt` & `alviss-3.2.2/alviss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alviss-3.2.1/pyproject.toml` & `alviss-3.2.2/pyproject.toml`

 * *Files identical despite different names*

