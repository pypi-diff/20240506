# Comparing `tmp/autorunpy-8.0.2.tar.gz` & `tmp/autorunpy-8.0.3.tar.gz`

## Comparing `autorunpy-8.0.2.tar` & `autorunpy-8.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.2/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 autorunpy-8.0.2/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.2/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.2/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.2/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.3/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autorunpy-8.0.3/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.3/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.3/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.3/PKG-INFO
```

### Comparing `autorunpy-8.0.2/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.0.3/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.2/src/autorunpy/make_venv.py` & `autorunpy-8.0.3/src/autorunpy/make_venv.py`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.2/src/autorunpy/util.py` & `autorunpy-8.0.3/src/autorunpy/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class Const :
     rc = Path(environ['HOME']) / 'auto_run_configs'
 
 c = Const()
 
 def read_json(fp) :
-    print("config path:" , fp)
     fp = Path(fp)
 
     # if fp is not entered with .json extension, add .json to it
     fp = fp.with_suffix('.json')
 
     fp = c.rc / fp
```

### Comparing `autorunpy-8.0.2/.gitignore` & `autorunpy-8.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.2/LICENSE` & `autorunpy-8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.2/PKG-INFO` & `autorunpy-8.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 8.0.2
+Version: 8.0.3
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

