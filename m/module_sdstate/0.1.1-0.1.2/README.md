# Comparing `tmp/module_sdstate-0.1.1.tar.gz` & `tmp/module_sdstate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module_sdstate-0.1.1.tar", max compression
+gzip compressed data, was "module_sdstate-0.1.2.tar", max compression
```

## Comparing `module_sdstate-0.1.1.tar` & `module_sdstate-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.1/LICENSE
--rw-r--r--   0        0        0      680 2024-03-05 20:20:24.518070 module_sdstate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.1/README.md
--rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.1/src/module_sdstate/__init__.py
--rw-r--r--   0        0        0     6634 2024-03-05 20:21:28.613246 module_sdstate-0.1.1/src/module_sdstate/lanczos_utils.py
--rw-r--r--   0        0        0    10149 2024-02-26 20:19:06.196762 module_sdstate-0.1.1/src/module_sdstate/sdstate_utils.py
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.2/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-06 20:46:09.395470 module_sdstate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.2/README.md
+-rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.2/src/module_sdstate/__init__.py
+-rw-r--r--   0        0        0     6603 2024-05-06 20:37:26.351098 module_sdstate-0.1.2/src/module_sdstate/lanczos_utils.py
+-rw-r--r--   0        0        0    10149 2024-02-26 20:19:06.196762 module_sdstate-0.1.2/src/module_sdstate/sdstate_utils.py
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.2/PKG-INFO
```

### Comparing `module_sdstate-0.1.1/LICENSE` & `module_sdstate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.1/pyproject.toml` & `module_sdstate-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "module_sdstate"
-version = "0.1.1"
+version = "0.1.2"
 description = "Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range."
 authors = ["Linjun Wang"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `module_sdstate-0.1.1/README.md` & `module_sdstate-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.1/src/module_sdstate/lanczos_utils.py` & `module_sdstate-0.1.2/src/module_sdstate/lanczos_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,19 @@
     lstate = sdstate(((1 << ne) - 1) << (n-ne), n_qubit = n)
     E_low = lstate.exp(Hf)
     #  <high|H|high>
     hstate = sdstate((1 << ne) - 1, n_qubit = n)
     E_high = hstate.exp(Hf)
     return E_high, E_low
 
-def HF_spectrum_range(Hf, multiprocessing = True):
+def HF_spectrum_range(Hf, n, multiprocessing = True):
     """Compute the naive Hartree-Fock energy range of the Hamiltonian 2e tensor Hf for all number of electrons.
     Multiprocessing parameter is set to parallelize computations for the states with different number of electrons. 
     Warning: This is not the actual Hartree-Fock energy range, which takes exponential time to compute
     """
-    n = of.utils.count_qubits(Hf)
     if multiprocessing:
         num_processes = os.cpu_count()
         with Pool(processes=num_processes) as pool:
             res = pool.starmap(HF_energy, [(Hf, n, ne) for ne in range(n)])
         low = 1e10
         low_state = ""
         high = -1e10
```

### Comparing `module_sdstate-0.1.1/src/module_sdstate/sdstate_utils.py` & `module_sdstate-0.1.2/src/module_sdstate/sdstate_utils.py`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.1/PKG-INFO` & `module_sdstate-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_sdstate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range.
 License: MIT
 Author: Linjun Wang
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

