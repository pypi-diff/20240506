# Comparing `tmp/autorunpy-8.0.0.tar.gz` & `tmp/autorunpy-8.0.1.tar.gz`

## Comparing `autorunpy-8.0.0.tar` & `autorunpy-8.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.0/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.0/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.0/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.1/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autorunpy-8.0.1/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.1/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.1/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.1/PKG-INFO
```

### Comparing `autorunpy-8.0.0/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.0.1/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.0/src/autorunpy/make_venv.py` & `autorunpy-8.0.1/src/autorunpy/make_venv.py`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.0/src/autorunpy/util.py` & `autorunpy-8.0.1/src/autorunpy/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 class Const :
     rc = Path(environ['HOME']) / 'auto_run_configs'
 
 c = Const()
 
 def read_json(fp) :
+    fp = Path(fp)
+
     # if fp is not entered with .json extension, add .json to it
     fp = fp.with_suffix('.json')
 
     fp = c.rc / fp
 
     with open(fp , 'r') as f :
         return json.load(f)
```

### Comparing `autorunpy-8.0.0/.gitignore` & `autorunpy-8.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.0/LICENSE` & `autorunpy-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.0/PKG-INFO` & `autorunpy-8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 8.0.0
+Version: 8.0.1
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

