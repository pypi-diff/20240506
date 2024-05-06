# Comparing `tmp/polyharmonics-0.1.0.tar.gz` & `tmp/polyharmonics-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyharmonics-0.1.0.tar", max compression
+gzip compressed data, was "polyharmonics-0.2.0.tar", max compression
```

## Comparing `polyharmonics-0.1.0.tar` & `polyharmonics-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,16 @@
--rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     6272 2024-05-01 17:53:48.000000 polyharmonics-0.1.0/README.md
--rwxr-xr-x   0        0        0      466 2024-05-01 18:06:30.000000 polyharmonics-0.1.0/polyharmonics/__init__.py
--rwxr-xr-x   0        0        0     7681 2024-05-01 18:09:26.000000 polyharmonics-0.1.0/polyharmonics/__main__.py
--rwxr-xr-x   0        0        0     6679 2024-05-01 18:08:21.000000 polyharmonics-0.1.0/polyharmonics/associated_legendre_functions.py
--rwxr-xr-x   0        0        0     5068 2024-05-01 18:08:29.000000 polyharmonics-0.1.0/polyharmonics/legendre_polynomials.py
--rwxr-xr-x   0        0        0     3438 2024-04-27 09:22:00.000000 polyharmonics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 polyharmonics-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     6137 2024-05-01 19:57:18.000000 polyharmonics-0.2.0/README.md
+-rwxr-xr-x   0        0        0      459 2024-05-04 15:40:05.000000 polyharmonics-0.2.0/polyharmonics/__init__.py
+-rwxr-xr-x   0        0        0     1075 2024-05-06 13:28:42.421280 polyharmonics-0.2.0/polyharmonics/__main__.py
+-rwxr-xr-x   0        0        0     7241 2024-05-06 13:42:35.576924 polyharmonics-0.2.0/polyharmonics/associated_legendre_functions.py
+-rwxr-xr-x   0        0        0      209 2024-05-06 13:28:42.418277 polyharmonics-0.2.0/polyharmonics/cli/__init__.py
+-rwxr-xr-x   0        0        0     5707 2024-05-06 13:28:42.427725 polyharmonics-0.2.0/polyharmonics/cli/associated_legendre_cmd.py
+-rwxr-xr-x   0        0        0      190 2024-05-06 13:28:42.418225 polyharmonics-0.2.0/polyharmonics/cli/benchmark/__init__.py
+-rwxr-xr-x   0        0        0    13006 2024-05-06 13:41:16.581886 polyharmonics-0.2.0/polyharmonics/cli/benchmark/associated_legendre_bench.py
+-rwxr-xr-x   0        0        0     5553 2024-05-06 13:41:16.580068 polyharmonics-0.2.0/polyharmonics/cli/benchmark/legendre_bench.py
+-rwxr-xr-x   0        0        0      650 2024-05-06 13:28:42.421780 polyharmonics-0.2.0/polyharmonics/cli/benchmark_cmd.py
+-rwxr-xr-x   0        0        0      183 2024-05-04 16:25:21.000000 polyharmonics-0.2.0/polyharmonics/cli/colors.py
+-rwxr-xr-x   0        0        0     3456 2024-05-06 13:28:42.423962 polyharmonics-0.2.0/polyharmonics/cli/legendre_cmd.py
+-rwxr-xr-x   0        0        0     4957 2024-05-06 13:37:17.743809 polyharmonics-0.2.0/polyharmonics/legendre_polynomials.py
+-rwxr-xr-x   0        0        0     3462 2024-05-06 13:37:39.200763 polyharmonics-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7667 1970-01-01 00:00:00.000000 polyharmonics-0.2.0/PKG-INFO
```

### Comparing `polyharmonics-0.1.0/LICENSE` & `polyharmonics-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.1.0/README.md` & `polyharmonics-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Polyharmonics
 
 <div align="center">
 
-[![Build status](https://github.com/ComicIvans/polyharmonics/workflows/build/badge.svg?branch=main&event=push)](https://github.com/ComicIvans/polyharmonics/actions?query=workflow%3Abuild)
+![PyPI](https://img.shields.io/pypi/v/polyharmonics)
 [![Python Version](https://img.shields.io/pypi/pyversions/polyharmonics.svg)](https://pypi.org/project/polyharmonics/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ComicIvans/polyharmonics/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: ruff](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/astral-sh/ruff)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ComicIvans/polyharmonics/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ComicIvans/polyharmonics/releases)
```

### Comparing `polyharmonics-0.1.0/polyharmonics/legendre_polynomials.py` & `polyharmonics-0.2.0/polyharmonics/legendre_polynomials.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-from typing import List, Union
+from typing import List
 
 from sympy import Expr, Rational, diff, expand, factorial, symbols
 
 x, t = symbols("x t")
-
 gen_Legendre: Expr = (1 - 2 * x * t + t**2) ** Rational(-1, 2)
 
-# Where the differentiation of the generating function is stored when using legendre_def
-LEGENDRE_DEF_STORE: List[Expr] = [
-    (1 - 2 * x * t + t**2) ** Rational(-1, 2),
-    -(1 / 2) * (2 * t - 2 * x) * (1 - 2 * x * t + t**2) ** Rational(-3, 2),
-]
 
-# Where the Legendre polynomials are stored when using legendre_rec
-LEGENDRE_REC_STORE: List[Expr] = [x**0, x**1]
+class LegendreStore:
+    def __init__(self):
+        self.reset()
+
+    def reset(self, definition=True, recursion=True):
+        # Stores differentiation of the generating function when using def
+        if definition:
+            self.definition: List[Expr] = [
+                (1 - 2 * x * t + t**2) ** Rational(-1, 2),
+                -Rational(1, 2)
+                * (2 * t - 2 * x)
+                * (1 - 2 * x * t + t**2) ** Rational(-3, 2),
+            ]
+
+        # Stores the Legendre polynomials when using recursion
+        if recursion:
+            self.recursion: List[Expr] = [x**0, x**1]
+
+
+legendre_store = LegendreStore()
 
 
 def legendre_def(n: int, store: bool = True, callback: bool = False):
     if n == 0:
         return x**0
     elif n == 1:
         return x**1
     else:
         if store:
             # If the previous polynomials are not stored, calculate and store them
-            if len(LEGENDRE_DEF_STORE) <= n:
-                if len(LEGENDRE_DEF_STORE) < n:
+            if len(legendre_store.definition) <= n:
+                if len(legendre_store.definition) < n:
                     legendre_def(n - 1, store=True, callback=True)
-                LEGENDRE_DEF_STORE.append(diff(LEGENDRE_DEF_STORE[n - 1], t, 1))
+                legendre_store.definition.append(
+                    diff(legendre_store.definition[n - 1], t, 1)
+                )
             # If the function is called by itself to store
             # the previous polynomials, don't return them
             if callback:
                 return None
             else:
-                # The fractions are converted to floats
-                # subs is the problem but don't know why
                 return expand(
-                    (1 / factorial(n)) * LEGENDRE_DEF_STORE[n].subs(t, 0),
+                    (1 / factorial(n)) * legendre_store.definition[n].subs(t, 0),
                     deep=True,
                     mul=True,
                     multinomial=False,
                     power_exp=False,
                     power_base=False,
                     log=False,
                 )
@@ -62,33 +74,33 @@
     elif n == 1:
         if callback:
             return x**1, x**0
         else:
             return x**1
     else:
         if store:
-            if len(LEGENDRE_REC_STORE) <= n:
-                if len(LEGENDRE_REC_STORE) < n:
+            if len(legendre_store.recursion) <= n:
+                if len(legendre_store.recursion) < n:
                     legendre_rec(n - 1, store=store)
-                LEGENDRE_REC_STORE.append(
+                legendre_store.recursion.append(
                     expand(
                         (
-                            (2 * n - 1) * x * LEGENDRE_REC_STORE[n - 1]
-                            - (n - 1) * LEGENDRE_REC_STORE[n - 2]
+                            (2 * n - 1) * x * legendre_store.recursion[n - 1]
+                            - (n - 1) * legendre_store.recursion[n - 2]
                         )
                         / n,
                         deep=True,
                         mul=True,
                         multinomial=False,
                         power_exp=False,
                         power_base=False,
                         log=False,
                     ),
                 )
-            return LEGENDRE_REC_STORE[n]
+            return legendre_store.recursion[n]
         else:
             curr_pol, prev_pol = legendre_rec(n - 1, store=store, callback=True)
             if callback:
                 return (
                     expand(
                         ((2 * n - 1) * x * curr_pol - (n - 1) * prev_pol) / n,
                         deep=True,
@@ -108,37 +120,32 @@
                     multinomial=False,
                     power_exp=False,
                     power_base=False,
                     log=False,
                 )
 
 
-def legendre(n: Union[int, List[int]]) -> Union[Expr, List[Expr]]:
+def legendre(n: int) -> Expr:
     """
-    Calculate the analytical expression of the Legendre polynomials
+    Calculate the analytical expression of the Legendre polynomial
 
     Args:
-        n (Union[int, List[int]]): The degree of the Legendre polynomial(s).
-        Must be an integer or a list of integers greater than or equal to 0.
+        n (int): The degree of the Legendre polynomial.
+        Must be an integer greater than or equal to 0.
 
     Returns:
-        Union[Expr, List[Expr]]: The Legendre polynomial(s) of the given degree(s).
+        Expr: The Legendre polynomial of the given degree.
 
     Examples:
         .. code:: python
 
+            >>> legendre(0)
+            1
             >>> legendre(1)
             x
-            >>> legendre([0, 1])
-            [1, x]
     """  # noqa: E501
     if isinstance(n, int):
         if n < 0:
-            raise ValueError("Degree n must be greater than or equal to 0")
-        return legendre_rec(n, store=False)
-    elif isinstance(n, list):
-        if any(i < 0 for i in n):
-            raise ValueError("All degrees n must be greater than or equal to 0")
-        store: bool = len(n) > 1
-        return [legendre_rec(i, store=store) for i in n]
+            raise ValueError("n must be greater than or equal to 0")
+        return legendre_rec(n, store=True)
     else:
-        raise TypeError("n must be an integer or a list of integers")
+        raise TypeError("n must be an integer")
```

### Comparing `polyharmonics-0.1.0/pyproject.toml` & `polyharmonics-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polyharmonics"
-version = "0.1.0"
+version = "0.2.0"
 description = "Ortogonal polynomials in the unit sphere"
 readme = "README.md"
 authors = [
   "Iván Salido Cobo <isalidocobo@gmail.com>",
 ]
 license = "BSD-3-Clause"
 repository = "https://github.com/ComicIvans/polyharmonics"
@@ -51,14 +51,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 matplotlib = "^3.8.4"
 sympy = "^1.12"
 rich = "^13.7.1"
 typer = "^0.12.3"
 numpy = "^1.26.4"
+prettytable = "^3.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 pytest-html = "^4.1.1"
 pytest-cov = "^5.0.0"
 bandit = "^1.7.1"
 ruff = "^0.4.1"
@@ -67,15 +68,15 @@
 coverage-badge = "^1.1.0"
 
 
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/settings/
 # https://docs.astral.sh/ruff/configuration/
-line-length = 88
+line-length = 92
 
 # https://beta.ruff.rs/docs/rules/
 lint.select = ["E", "W", "F", "I"]
 lint.extend-select = ["I"]
 lint.ignore = ["F401"]
 
 # Exclude a variety of commonly ignored directories.
```

### Comparing `polyharmonics-0.1.0/PKG-INFO` & `polyharmonics-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyharmonics
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ortogonal polynomials in the unit sphere
 Home-page: https://github.com/ComicIvans/polyharmonics
 License: BSD-3-Clause
 Keywords: python,polynomials,unit sphere,orthogonal polynomials,mathematics,math,legendre polynomials,associated legendre functions,spherical harmonics
 Author: Iván Salido Cobo
 Author-email: isalidocobo@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -20,25 +20,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: prettytable (>=3.10.0,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sympy (>=1.12,<2.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/ComicIvans/polyharmonics
 Description-Content-Type: text/markdown
 
 # Polyharmonics
 
 <div align="center">
 
-[![Build status](https://github.com/ComicIvans/polyharmonics/workflows/build/badge.svg?branch=main&event=push)](https://github.com/ComicIvans/polyharmonics/actions?query=workflow%3Abuild)
+![PyPI](https://img.shields.io/pypi/v/polyharmonics)
 [![Python Version](https://img.shields.io/pypi/pyversions/polyharmonics.svg)](https://pypi.org/project/polyharmonics/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ComicIvans/polyharmonics/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: ruff](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/astral-sh/ruff)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ComicIvans/polyharmonics/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ComicIvans/polyharmonics/releases)
```

