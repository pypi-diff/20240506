# Comparing `tmp/coffe_analyzer-0.1.1.tar.gz` & `tmp/coffe_analyzer-0.1.2.tar.gz`

## Comparing `coffe_analyzer-0.1.1.tar` & `coffe_analyzer-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/src/coffe_analyzer/__init__.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/src/coffe_analyzer/coffeanalyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/tests/test_arp4761_q411.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/tests/test_example.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/tests/test_files/example.csv
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/tests/test_files/table_Q-4-6.csv
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/LICENSE
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/README.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    47036 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/src/coffe_analyzer/__init__.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/src/coffe_analyzer/coffeanalyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/tests/test_arp4761_q411.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/tests/test_example.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/tests/test_files/example.csv
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/tests/test_files/table_Q-4-6.csv
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/README.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    47038 2020-02-02 00:00:00.000000 coffe_analyzer-0.1.2/PKG-INFO
```

### Comparing `coffe_analyzer-0.1.1/src/coffe_analyzer/coffeanalyzer.py` & `coffe_analyzer-0.1.2/src/coffe_analyzer/coffeanalyzer.py`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/tests/test_arp4761_q411.py` & `coffe_analyzer-0.1.2/tests/test_arp4761_q411.py`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/tests/test_example.py` & `coffe_analyzer-0.1.2/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/tests/test_files/table_Q-4-6.csv` & `coffe_analyzer-0.1.2/tests/test_files/table_Q-4-6.csv`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/.gitignore` & `coffe_analyzer-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/LICENSE` & `coffe_analyzer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/README.md` & `coffe_analyzer-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 ## Acknowledgments
 * [SymPy](https://github.com/sympy/sympy)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[pypi-shield]: https://img.shields.io/pypi/v/coffeanalyzer.svg?style=for-the-badge
-[pypi-url]: https://pypi.python.org/pypi/coffeanalyzer
+[pypi-shield]: https://img.shields.io/pypi/v/coffe-analyzer.svg?style=for-the-badge
+[pypi-url]: https://pypi.python.org/pypi/coffe-analyzer
 [contributors-shield]: https://img.shields.io/github/contributors/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [contributors-url]: https://github.com/samuelglorente/coffe_analyzer/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [forks-url]: https://github.com/samuelglorente/coffe_analyzer/network/members
 [stars-shield]: https://img.shields.io/github/stars/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [stars-url]: https://github.com/samuelglorente/coffe_analyzer/stargazers
 [issues-shield]: https://img.shields.io/github/issues/samuelglorente/coffe_analyzer.svg?style=for-the-badge
```

#### html2text {}

```diff
@@ -54,16 +54,16 @@
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Samuel GarcÃ­a Lorente [LinkedIn](linkedin-url) â [email]
 (samuelglorente@gmail.com) - [GitHub](linkedin-url)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments * [SymPy](https://github.com/sympy/sympy)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-[pypi-shield]: https://img.shields.io/pypi/v/coffeanalyzer.svg?style=for-the-
-badge [pypi-url]: https://pypi.python.org/pypi/coffeanalyzer [contributors-
+[pypi-shield]: https://img.shields.io/pypi/v/coffe-analyzer.svg?style=for-the-
+badge [pypi-url]: https://pypi.python.org/pypi/coffe-analyzer [contributors-
 shield]: https://img.shields.io/github/contributors/samuelglorente/
 coffe_analyzer.svg?style=for-the-badge [contributors-url]: https://github.com/
 samuelglorente/coffe_analyzer/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/samuelglorente/coffe_analyzer.svg?style=for-the-
 badge [forks-url]: https://github.com/samuelglorente/coffe_analyzer/network/
 members [stars-shield]: https://img.shields.io/github/stars/samuelglorente/
 coffe_analyzer.svg?style=for-the-badge [stars-url]: https://github.com/
```

### Comparing `coffe_analyzer-0.1.1/pyproject.toml` & `coffe_analyzer-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coffe_analyzer-0.1.1/PKG-INFO` & `coffe_analyzer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coffe-analyzer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Supports the CoFFE analysis presented in ARP4761A/ED-135.
 Project-URL: Repository, https://github.com/samuelglorente/coffe_analyzer.git
 Project-URL: Issues, https://github.com/samuelglorente/coffe_analyzer/issues
 Author-email: Samuel Garcia Lorente <samuelglorente@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -794,16 +794,16 @@
 ## Acknowledgments
 * [SymPy](https://github.com/sympy/sympy)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[pypi-shield]: https://img.shields.io/pypi/v/coffeanalyzer.svg?style=for-the-badge
-[pypi-url]: https://pypi.python.org/pypi/coffeanalyzer
+[pypi-shield]: https://img.shields.io/pypi/v/coffe-analyzer.svg?style=for-the-badge
+[pypi-url]: https://pypi.python.org/pypi/coffe-analyzer
 [contributors-shield]: https://img.shields.io/github/contributors/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [contributors-url]: https://github.com/samuelglorente/coffe_analyzer/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [forks-url]: https://github.com/samuelglorente/coffe_analyzer/network/members
 [stars-shield]: https://img.shields.io/github/stars/samuelglorente/coffe_analyzer.svg?style=for-the-badge
 [stars-url]: https://github.com/samuelglorente/coffe_analyzer/stargazers
 [issues-shield]: https://img.shields.io/github/issues/samuelglorente/coffe_analyzer.svg?style=for-the-badge
```

