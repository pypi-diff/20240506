# Comparing `tmp/coffe_analyzer-0.1.3.tar.gz` & `tmp/coffe_analyzer-0.1.4.tar.gz`

## Comparing `coffe_analyzer-0.1.3.tar` & `coffe_analyzer-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/src/__init__.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/src/coffeanalyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/tests/test_arp4761_q411.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/tests/test_example.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/tests/test_files/example.csv
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/tests/test_files/table_Q-4-6.csv
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/LICENSE
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/README.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    47038 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/requirements-dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/src/__init__.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/src/coffeanalyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/tests/test_arp4761_q411.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/tests/test_example.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/tests/test_files/example.csv
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/tests/test_files/table_Q-4-6.csv
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/README.md
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    47038 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.4/PKG-INFO
```

### Comparing `coffe_analyzer-0.1.3/src/coffeanalyzer.py` & `coffe_analyzer-0.1.4/src/coffeanalyzer.py`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.3/tests/test_arp4761_q411.py` & `coffe_analyzer-0.1.4/tests/test_arp4761_q411.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 
 pkg_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if pkg_path not in sys.path:
     sys.path.append(pkg_path)
 
-from coffeanalyzer import CoffeInstance
+from src.coffeanalyzer import CoffeInstance
 
 
 def test_highspeed_overrun():
     path_csv = 'tests/test_files/table_Q-4-6.csv'
 
     overrun_coffe = CoffeInstance(
         ignored_states=['O'],
```

### Comparing `coffe_analyzer-0.1.3/tests/test_example.py` & `coffe_analyzer-0.1.4/tests/test_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 
 pkg_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if pkg_path not in sys.path:
     sys.path.append(pkg_path)
     
-from coffeanalyzer import CoffeInstance
+from src.coffeanalyzer import CoffeInstance
 
 def main():
     path_csv = 'tests/test_files/example.csv'
 
     loss_coffe = CoffeInstance(
         ignored_states=['O'], 
         ignored_results=['No Loss']
```

### Comparing `coffe_analyzer-0.1.3/tests/test_files/table_Q-4-6.csv` & `coffe_analyzer-0.1.4/tests/test_files/table_Q-4-6.csv`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.3/.gitignore` & `coffe_analyzer-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.3/LICENSE` & `coffe_analyzer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.3/README.md` & `coffe_analyzer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.3/pyproject.toml` & `coffe_analyzer-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 Repository = "https://github.com/samuelglorente/coffe_analyzer.git"
 Issues = "https://github.com/samuelglorente/coffe_analyzer/issues"
 
 [tool.hatch.version]
 path = "src/__init__.py"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/coffeanalyzer"]
+packages = ["src"]
```

### Comparing `coffe_analyzer-0.1.3/PKG-INFO` & `coffe_analyzer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coffe-analyzer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Supports the CoFFE analysis presented in ARP4761A/ED-135.
 Project-URL: Repository, https://github.com/samuelglorente/coffe_analyzer.git
 Project-URL: Issues, https://github.com/samuelglorente/coffe_analyzer/issues
 Author-email: Samuel Garcia Lorente <samuelglorente@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

