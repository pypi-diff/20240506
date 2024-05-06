# Comparing `tmp/autorunpy-8.0.7.tar.gz` & `tmp/autorunpy-8.1.0.tar.gz`

## Comparing `autorunpy-8.0.7.tar` & `autorunpy-8.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.7/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 autorunpy-8.0.7/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.7/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.7/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.7/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.7/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.1.0/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 autorunpy-8.1.0/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.1.0/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.1.0/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.1.0/PKG-INFO
```

### Comparing `autorunpy-8.0.7/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.1.0/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.7/src/autorunpy/make_venv.py` & `autorunpy-8.1.0/src/autorunpy/make_venv.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 
     _cmds = ['pyenv' , 'virtualenv' , py_ver , conf_stem , '&> /dev/null']
     subprocess.run(_cmds)
 
     print(conf_stem)
 
 if __name__ == '__main__' :
-    conf_stem = sys.argv[1]
-    make_venv(conf_stem)
+    arg = sys.argv[1]
+    make_venv(arg)
```

### Comparing `autorunpy-8.0.7/.gitignore` & `autorunpy-8.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.7/LICENSE` & `autorunpy-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.7/PKG-INFO` & `autorunpy-8.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 8.0.7
+Version: 8.1.0
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

