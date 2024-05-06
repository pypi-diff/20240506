# Comparing `tmp/autorunpy-7.4.0.tar.gz` & `tmp/autorunpy-8.0.0.tar.gz`

## Comparing `autorunpy-7.4.0.tar` & `autorunpy-8.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-7.4.0/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 autorunpy-7.4.0/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-7.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-7.4.0/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-7.4.0/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-7.4.0/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.0/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 autorunpy-8.0.0/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.0/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.0/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.0/PKG-INFO
```

### Comparing `autorunpy-7.4.0/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.0.0/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-7.4.0/src/autorunpy/make_venv.py` & `autorunpy-8.0.0/src/autorunpy/make_venv.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 def make_venv(fp) :
     j = read_json(fp)
 
     py_ver = j[c.py_ver]
 
     venv_name = Path(fp).stem
 
-    subprocess.run(['pyenv' , 'install' , '--skip-existing' , py_ver])
+    _cmds = ['pyenv' , 'install' , '--skip-existing' , py_ver]
+    subprocess.run(_cmds)
 
-    cmds = ['pyenv' , 'virtualenv' , py_ver , venv_name , '&> /dev/null']
-    subprocess.run(cmds)
+    _cmds = ['pyenv' , 'virtualenv' , py_ver , venv_name , '&> /dev/null']
+    subprocess.run(_cmds)
 
     print(venv_name)
 
 if __name__ == '__main__' :
     conf_fn = sys.argv[1]
     make_venv(conf_fn)
```

### Comparing `autorunpy-7.4.0/.gitignore` & `autorunpy-8.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-7.4.0/LICENSE` & `autorunpy-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-7.4.0/PKG-INFO` & `autorunpy-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 7.4.0
+Version: 8.0.0
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

