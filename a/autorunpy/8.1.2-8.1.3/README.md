# Comparing `tmp/autorunpy-8.1.2.tar.gz` & `tmp/autorunpy-8.1.3.tar.gz`

## Comparing `autorunpy-8.1.2.tar` & `autorunpy-8.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.1.2/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 autorunpy-8.1.2/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.1.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.1.2/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.1.2/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.1.2/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.1.3/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 autorunpy-8.1.3/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.1.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.1.3/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.1.3/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.1.3/PKG-INFO
```

### Comparing `autorunpy-8.1.2/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.1.3/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-8.1.2/src/autorunpy/make_venv.py` & `autorunpy-8.1.3/src/autorunpy/make_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     py_ver = j[c.py_ver]
 
     _cmds = ['pyenv' , 'install' , '--skip-existing' , py_ver]
     subprocess.run(_cmds)
 
     _cmds = ['pyenv' , 'virtualenv' , py_ver , conf_stem]
-    # _cmds += ['&> /dev/null']
+    _cmds += ['&> /dev/null']
     subprocess.run(_cmds)
 
     print(conf_stem)
 
 if __name__ == '__main__' :
     arg = sys.argv[1]
     make_venv(arg)
```

### Comparing `autorunpy-8.1.2/.gitignore` & `autorunpy-8.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-8.1.2/LICENSE` & `autorunpy-8.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-8.1.2/PKG-INFO` & `autorunpy-8.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 8.1.2
+Version: 8.1.3
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

