# Comparing `tmp/autorunpy-8.0.5.tar.gz` & `tmp/autorunpy-8.0.6.tar.gz`

## Comparing `autorunpy-8.0.5.tar` & `autorunpy-8.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.5/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/ret_module_2_run.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/ret_pkg_name.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/rm_venv.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 autorunpy-8.0.5/src/autorunpy/util.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.5/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.5/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.5/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.5/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-8.0.6/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 autorunpy-8.0.6/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 autorunpy-8.0.6/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-8.0.6/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-8.0.6/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-8.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-8.0.6/PKG-INFO
```

### Comparing `autorunpy-8.0.5/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-8.0.6/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.5/src/autorunpy/make_venv.py` & `autorunpy-8.0.6/src/autorunpy/make_venv.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,29 @@
     1. Installs the required python version, skips if already installed
     2. Creates a virtual environment with that python version
 
     """
 
 import subprocess
 import sys
-from pathlib import Path
 
 from .util import Conf
 from .util import read_json
 
 c = Conf()
 
 def make_venv(conf_stem) :
     fp , j = read_json(conf_stem)
 
     py_ver = j[c.py_ver]
 
-    venv_name = conf_stem
-
     _cmds = ['pyenv' , 'install' , '--skip-existing' , py_ver]
     subprocess.run(_cmds)
 
-    _cmds = ['pyenv' , 'virtualenv' , py_ver , venv_name , '&> /dev/null']
+    _cmds = ['pyenv' , 'virtualenv' , py_ver , conf_stem , '&> /dev/null']
     subprocess.run(_cmds)
 
-    print(venv_name)
+    print(conf_stem)
 
 if __name__ == '__main__' :
     conf_stem = sys.argv[1]
     make_venv(conf_stem)
```

### Comparing `autorunpy-8.0.5/.gitignore` & `autorunpy-8.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.5/LICENSE` & `autorunpy-8.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-8.0.5/PKG-INFO` & `autorunpy-8.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autorunpy
-Version: 8.0.5
+Version: 8.0.6
 Summary: Tools for auto running python scripts
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

