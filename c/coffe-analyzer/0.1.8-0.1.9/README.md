# Comparing `tmp/coffe_analyzer-0.1.8.tar.gz` & `tmp/coffe_analyzer-0.1.9.tar.gz`

## Comparing `coffe_analyzer-0.1.8.tar` & `coffe_analyzer-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/requirements-dev.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/src/__init__.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/src/coffeanalyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/tests/test_arp4761_q411.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/tests/test_example.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/tests/test_files/example.csv
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/tests/test_files/table_Q-4-6.csv
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/LICENSE
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    47038 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/requirements-dev.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/src/coffe_analyzer/__init__.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/src/coffe_analyzer/coffeanalyzer.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/tests/test_arp4761_q411.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/tests/test_example.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/tests/test_files/example.csv
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/tests/test_files/table_Q-4-6.csv
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/README.md
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    47038 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.9/PKG-INFO
```

### Comparing `coffe_analyzer-0.1.8/src/coffeanalyzer.py` & `coffe_analyzer-0.1.9/src/coffe_analyzer/coffeanalyzer.py`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.8/tests/test_arp4761_q411.py` & `coffe_analyzer-0.1.9/tests/test_arp4761_q411.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import os
 import sys
 
 pkg_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if pkg_path not in sys.path:
     sys.path.append(pkg_path)
 
-from src.coffeanalyzer import CoffeInstance
-
+from src.coffe_analyzer.coffeanalyzer import CoffeInstance
 
 def test_highspeed_overrun():
     path_csv = 'tests/test_files/table_Q-4-6.csv'
 
     overrun_coffe = CoffeInstance(
         ignored_states=['O'], 
         ignored_results=['No overrun', 'Low-speed overrun'],
```

### Comparing `coffe_analyzer-0.1.8/tests/test_example.py` & `coffe_analyzer-0.1.9/tests/test_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 
 pkg_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if pkg_path not in sys.path:
     sys.path.append(pkg_path)
     
-from src.coffeanalyzer import CoffeInstance
+from src.coffe_analyzer.coffeanalyzer import CoffeInstance
 
 def main():
     path_csv = 'tests/test_files/example.csv'
 
     loss_coffe = CoffeInstance(
         ignored_states=['O'], 
         ignored_results=['No Loss']
```

### Comparing `coffe_analyzer-0.1.8/tests/test_files/table_Q-4-6.csv` & `coffe_analyzer-0.1.9/tests/test_files/table_Q-4-6.csv`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.8/.gitignore` & `coffe_analyzer-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.8/LICENSE` & `coffe_analyzer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.8/README.md` & `coffe_analyzer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.8/pyproject.toml` & `coffe_analyzer-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,11 +29,8 @@
 ]
 
 [project.urls]
 Repository = "https://github.com/samuelglorente/coffe_analyzer.git"
 Issues = "https://github.com/samuelglorente/coffe_analyzer/issues"
 
 [tool.hatch.version]
-path = "src/__init__.py"
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/coffeanalyzer.py"]
+path = "src/coffe_analyzer/__init__.py"
```

### Comparing `coffe_analyzer-0.1.8/PKG-INFO` & `coffe_analyzer-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coffe-analyzer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Supports the CoFFE analysis presented in ARP4761A/ED-135.
 Project-URL: Repository, https://github.com/samuelglorente/coffe_analyzer.git
 Project-URL: Issues, https://github.com/samuelglorente/coffe_analyzer/issues
 Author-email: Samuel Garcia Lorente <samuelglorente@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

