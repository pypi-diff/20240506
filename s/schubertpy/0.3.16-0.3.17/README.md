# Comparing `tmp/schubertpy-0.3.16.tar.gz` & `tmp/schubertpy-0.3.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubertpy-0.3.16.tar", last modified: Fri Apr 26 15:44:28 2024, max compression
+gzip compressed data, was "schubertpy-0.3.17.tar", last modified: Mon May  6 06:41:06 2024, max compression
```

## Comparing `schubertpy-0.3.16.tar` & `schubertpy-0.3.17.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:44:28.713137 schubertpy-0.3.16/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     1073 2023-09-25 07:57:01.000000 schubertpy-0.3.16/LICENSE
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6052 2024-04-26 15:44:28.713039 schubertpy-0.3.16/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)     5511 2024-02-14 05:48:03.000000 schubertpy-0.3.16/README.md
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:44:28.710505 schubertpy-0.3.16/schubertpy/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.16/schubertpy/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.16/schubertpy/abstract_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-02-10 16:43:47.000000 schubertpy-0.3.16/schubertpy/const.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.16/schubertpy/csv_bijection.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.16/schubertpy/grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.16/schubertpy/isotropic_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     5378 2024-02-13 13:41:03.000000 schubertpy-0.3.16/schubertpy/lc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.16/schubertpy/orthogonal_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.16/schubertpy/partition.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-02-13 13:42:24.000000 schubertpy-0.3.16/schubertpy/qcalc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3049 2024-02-13 13:41:35.000000 schubertpy-0.3.16/schubertpy/schur.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.16/schubertpy/util.py
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:44:28.712603 schubertpy-0.3.16/schubertpy.egg-info/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6052 2024-04-26 15:44:28.000000 schubertpy-0.3.16/schubertpy.egg-info/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-04-26 15:44:28.000000 schubertpy-0.3.16/schubertpy.egg-info/SOURCES.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-04-26 15:44:28.000000 schubertpy-0.3.16/schubertpy.egg-info/dependency_links.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-04-26 15:44:28.000000 schubertpy-0.3.16/schubertpy.egg-info/requires.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-04-26 15:44:28.000000 schubertpy-0.3.16/schubertpy.egg-info/top_level.txt
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-04-26 15:44:28.712165 schubertpy-0.3.16/schubertsage/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.16/schubertsage/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.16/schubertsage/conversion.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-04-26 15:44:28.713519 schubertpy-0.3.16/setup.cfg
--rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-04-26 15:44:28.000000 schubertpy-0.3.16/setup.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-06 06:41:06.774565 schubertpy-0.3.17/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    35147 2024-04-29 08:09:23.000000 schubertpy-0.3.17/LICENSE
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6722 2024-05-06 06:41:06.774429 schubertpy-0.3.17/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6180 2024-04-29 08:16:59.000000 schubertpy-0.3.17/README.md
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-06 06:41:06.772070 schubertpy-0.3.17/schubertpy/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.17/schubertpy/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.17/schubertpy/abstract_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-05-06 06:28:22.000000 schubertpy-0.3.17/schubertpy/const.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.17/schubertpy/csv_bijection.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.17/schubertpy/grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.17/schubertpy/isotropic_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     9203 2024-05-06 06:40:12.000000 schubertpy-0.3.17/schubertpy/lc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.17/schubertpy/orthogonal_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.17/schubertpy/partition.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-04-27 02:11:49.000000 schubertpy-0.3.17/schubertpy/qcalc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3239 2024-05-06 06:20:18.000000 schubertpy-0.3.17/schubertpy/schur.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.17/schubertpy/util.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-06 06:41:06.773960 schubertpy-0.3.17/schubertpy.egg-info/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6722 2024-05-06 06:41:06.000000 schubertpy-0.3.17/schubertpy.egg-info/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-05-06 06:41:06.000000 schubertpy-0.3.17/schubertpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-05-06 06:41:06.000000 schubertpy-0.3.17/schubertpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-05-06 06:41:06.000000 schubertpy-0.3.17/schubertpy.egg-info/requires.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-05-06 06:41:06.000000 schubertpy-0.3.17/schubertpy.egg-info/top_level.txt
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-06 06:41:06.773535 schubertpy-0.3.17/schubertsage/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.17/schubertsage/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.17/schubertsage/conversion.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-05-06 06:41:06.775010 schubertpy-0.3.17/setup.cfg
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      966 2024-05-06 06:41:06.000000 schubertpy-0.3.17/setup.py
```

### Comparing `schubertpy-0.3.16/PKG-INFO` & `schubertpy-0.3.17/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: schubertpy
-Version: 0.3.16
-Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
-Home-page: https://github.com/tranduythanh/schubertpy
-Author: Trần Duy Thanh
-Author-email: fbtranduythanh@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.24.3
-Requires-Dist: sympy>=1.11.1
-
 # schubertpy
 
 ## Overview
 
 `schubertpy` is a powerful Python package designed for performing advanced mathematical operations on the Grassmannian, a key concept in algebraic geometry and representation theory. This module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, and the manipulation of Schubert classes. It is a Python implementation based on the comprehensive maple library available at [https://sites.math.rutgers.edu/~asbuch/qcalc/](https://sites.math.rutgers.edu/~asbuch/qcalc/).
 
 References:
@@ -136,14 +123,30 @@
 
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
+## Authors
+- **Đặng Tuấn Hiệp**
+  - Email: hiepdt@dlu.edu.vn
+- **Trần Duy Thanh**
+  - Email: coachtranduythanh@gmail.com
+  - Email: 2015830@dlu.edu.vn
+- **Nguyễn Minh Đức**
+  - Email: 2113423@dlu.edu.vn
+- **Nguyễn Trương Thiên Ân**
+  - Email: 2113421@dlu.edu.vn
+
 ## Contributing
 
-Contributions to `schubertpy` are highly encouraged, whether they involve extending functionality, enhancing performance, or fixing bugs. Please feel free to submit issues or pull requests on GitHub to suggest changes or improvements.
+We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
+
+- **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
+- **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
+
+Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
-`schubertpy` is made available under the MIT License. For more details, see the LICENSE file included with the source code.
+`schubertpy` is open source software (under the GNU General Public License).
```

### Comparing `schubertpy-0.3.16/README.md` & `schubertpy-0.3.17/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: schubertpy
+Version: 0.3.17
+Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
+Home-page: https://github.com/tranduythanh/schubertpy
+Author: Trần Duy Thanh
+Author-email: fbtranduythanh@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: sympy>=1.11.1
+
 # schubertpy
 
 ## Overview
 
 `schubertpy` is a powerful Python package designed for performing advanced mathematical operations on the Grassmannian, a key concept in algebraic geometry and representation theory. This module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, and the manipulation of Schubert classes. It is a Python implementation based on the comprehensive maple library available at [https://sites.math.rutgers.edu/~asbuch/qcalc/](https://sites.math.rutgers.edu/~asbuch/qcalc/).
 
 References:
@@ -123,14 +136,30 @@
 
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
+## Authors
+- **Đặng Tuấn Hiệp**
+  - Email: hiepdt@dlu.edu.vn
+- **Trần Duy Thanh**
+  - Email: coachtranduythanh@gmail.com
+  - Email: 2015830@dlu.edu.vn
+- **Nguyễn Minh Đức**
+  - Email: 2113423@dlu.edu.vn
+- **Nguyễn Trương Thiên Ân**
+  - Email: 2113421@dlu.edu.vn
+
 ## Contributing
 
-Contributions to `schubertpy` are highly encouraged, whether they involve extending functionality, enhancing performance, or fixing bugs. Please feel free to submit issues or pull requests on GitHub to suggest changes or improvements.
+We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
+
+- **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
+- **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
+
+Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
-`schubertpy` is made available under the MIT License. For more details, see the LICENSE file included with the source code.
+`schubertpy` is open source software (under the GNU General Public License).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `schubertpy-0.3.16/schubertpy/abstract_grassmannian.py` & `schubertpy-0.3.17/schubertpy/abstract_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/csv_bijection.py` & `schubertpy-0.3.17/schubertpy/csv_bijection.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/grassmannian.py` & `schubertpy-0.3.17/schubertpy/grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/isotropic_grassmannian.py` & `schubertpy-0.3.17/schubertpy/isotropic_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/orthogonal_grassmannian.py` & `schubertpy-0.3.17/schubertpy/orthogonal_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/partition.py` & `schubertpy-0.3.17/schubertpy/partition.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/qcalc.py` & `schubertpy-0.3.17/schubertpy/qcalc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertpy/schur.py` & `schubertpy-0.3.17/schubertpy/schur.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 from typing import *
 import sympy as sp
 from .const import *
 import ast
 
 class Schur(object):
-    def __init__(self, p: List[int]):
+    def __init__(self, p: Union[List[int], sp.Expr, str]):
         # Set self.p to p or [] if p is None
-        self.p = p if p is not None else []
+        if isinstance(p, (list, tuple)):
+            self.p = p if p is not None else []
+            return
+        p = toSchur(p)
+        self.p = p.p
 
     def __str__(self):
         return f"S{self.p}".replace(' ', '')
 
     def __repr__(self):
         return self.__str__()
     
@@ -62,14 +66,17 @@
         if other.expr and isinstance(other.expr, sp.Expr):
             return self.symbol() ** other.expr
         raise ValueError(f"Invalid type for addition: {type(other)}")
 
     def symbol(self) -> sp.Symbol:
         return sp.parse_expr(self.__str__().translate(ftable))
 
+    def partition(self) -> List[int]:
+        return self.p
+
 
 def unique_schur_list(schur_list: List[Schur]):
     return  sorted(list(set(schur_list)))
 
 
 
 def isSchur(expr: sp.Expr) -> bool:
```

### Comparing `schubertpy-0.3.16/schubertpy.egg-info/PKG-INFO` & `schubertpy-0.3.17/schubertpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.16
+Version: 0.3.17
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -136,14 +136,30 @@
 
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
+## Authors
+- **Đặng Tuấn Hiệp**
+  - Email: hiepdt@dlu.edu.vn
+- **Trần Duy Thanh**
+  - Email: coachtranduythanh@gmail.com
+  - Email: 2015830@dlu.edu.vn
+- **Nguyễn Minh Đức**
+  - Email: 2113423@dlu.edu.vn
+- **Nguyễn Trương Thiên Ân**
+  - Email: 2113421@dlu.edu.vn
+
 ## Contributing
 
-Contributions to `schubertpy` are highly encouraged, whether they involve extending functionality, enhancing performance, or fixing bugs. Please feel free to submit issues or pull requests on GitHub to suggest changes or improvements.
+We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
+
+- **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
+- **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
+
+Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
-`schubertpy` is made available under the MIT License. For more details, see the LICENSE file included with the source code.
+`schubertpy` is open source software (under the GNU General Public License).
```

### Comparing `schubertpy-0.3.16/schubertpy.egg-info/SOURCES.txt` & `schubertpy-0.3.17/schubertpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/schubertsage/conversion.py` & `schubertpy-0.3.17/schubertsage/conversion.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.16/setup.py` & `schubertpy-0.3.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='schubertpy',
-    version='0.3.16',
+    version='0.3.17',
     packages=find_packages(),
     description='This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     author='Trần Duy Thanh',
     author_email='fbtranduythanh@gmail.com',
```

