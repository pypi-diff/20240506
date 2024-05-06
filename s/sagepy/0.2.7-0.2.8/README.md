# Comparing `tmp/sagepy-0.2.7.tar.gz` & `tmp/sagepy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagepy-0.2.7.tar", max compression
+gzip compressed data, was "sagepy-0.2.8.tar", max compression
```

## Comparing `sagepy-0.2.7.tar` & `sagepy-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     7031 2024-02-05 09:33:27.682607 sagepy-0.2.7/README.md
--rw-r--r--   0        0        0      348 2024-02-05 09:33:27.682607 sagepy-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-05 09:33:27.682607 sagepy-0.2.7/sagepy/__init__.py
--rw-r--r--   0        0        0      372 2024-02-05 09:33:27.682607 sagepy-0.2.7/sagepy/core/__init__.py
--rw-r--r--   0        0        0    18115 2024-02-05 09:33:27.682607 sagepy-0.2.7/sagepy/core/database.py
--rw-r--r--   0        0        0     6904 2024-02-05 09:33:27.682607 sagepy-0.2.7/sagepy/core/enzyme.py
--rw-r--r--   0        0        0      894 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/fasta.py
--rw-r--r--   0        0        0     1607 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/fdr.py
--rw-r--r--   0        0        0     2744 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/ion_series.py
--rw-r--r--   0        0        0     8964 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/lfq.py
--rw-r--r--   0        0        0     3438 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/mass.py
--rw-r--r--   0        0        0        0 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/ml/__init__.py
--rw-r--r--   0        0        0     2275 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/modification.py
--rw-r--r--   0        0        0     4251 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/peptide.py
--rw-r--r--   0        0        0    18268 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/scoring.py
--rw-r--r--   0        0        0    13472 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/spectrum.py
--rw-r--r--   0        0        0     4178 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/core/tmt.py
--rw-r--r--   0        0        0      636 2024-02-05 09:33:27.686607 sagepy-0.2.7/sagepy/utility.py
--rw-r--r--   0        0        0     7534 1970-01-01 00:00:00.000000 sagepy-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     7031 2024-05-06 13:07:33.029336 sagepy-0.2.8/README.md
+-rw-r--r--   0        0        0      348 2024-05-06 13:07:33.029336 sagepy-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/__init__.py
+-rw-r--r--   0        0        0    18115 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/database.py
+-rw-r--r--   0        0        0     6904 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/enzyme.py
+-rw-r--r--   0        0        0      894 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/fasta.py
+-rw-r--r--   0        0        0     1607 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/fdr.py
+-rw-r--r--   0        0        0     3103 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/ion_series.py
+-rw-r--r--   0        0        0     8954 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/lfq.py
+-rw-r--r--   0        0        0     3438 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/mass.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/ml/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/modification.py
+-rw-r--r--   0        0        0     4251 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/peptide.py
+-rw-r--r--   0        0        0    28587 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/scoring.py
+-rw-r--r--   0        0        0    14105 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/spectrum.py
+-rw-r--r--   0        0        0     4178 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/tmt.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/qfdr/__init__.py
+-rw-r--r--   0        0        0     2128 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/qfdr/tdc.py
+-rw-r--r--   0        0        0     1676 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/utility.py
+-rw-r--r--   0        0        0     7534 1970-01-01 00:00:00.000000 sagepy-0.2.8/PKG-INFO
```

### Comparing `sagepy-0.2.7/README.md` & `sagepy-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/database.py` & `sagepy-0.2.8/sagepy/core/database.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/enzyme.py` & `sagepy-0.2.8/sagepy/core/enzyme.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/fasta.py` & `sagepy-0.2.8/sagepy/core/fasta.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/fdr.py` & `sagepy-0.2.8/sagepy/core/fdr.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/ion_series.py` & `sagepy-0.2.8/sagepy/core/ion_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,28 @@
     @classmethod
     def b(cls):
         return cls.from_py_kind(psc.PyKind('b'))
 
     def __repr__(self):
         return f"IonType({self.__ion_type_ptr.kind_as_string()})"
 
+    def __hash__(self):
+        return hash(self.__ion_type_ptr.kind_as_string())
+
+    def __eq__(self, other):
+        if not isinstance(other, IonType):
+            return False
+        return self.__ion_type_ptr.kind_as_string() == other.__ion_type_ptr.kind_as_string()
+
     def get_py_ptr(self):
         return self.__ion_type_ptr
 
+    def to_string(self) -> str:
+        return self.__ion_type_ptr.kind_as_string()
+
 
 class Ion:
     """Ion class
 
     Args:
         ion_type (IonType): The ion type, e.g. b, y
         mass (float): The mass of the ion
```

### Comparing `sagepy-0.2.7/sagepy/core/lfq.py` & `sagepy-0.2.8/sagepy/core/lfq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List
+from typing import List
 from sagepy.core.database import PeptideIx
 import sagepy_connector
 psc = sagepy_connector.py_lfq
 
 
 class PeakScoringStrategy:
     """PeakScoringStrategy class
```

### Comparing `sagepy-0.2.7/sagepy/core/mass.py` & `sagepy-0.2.8/sagepy/core/mass.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/modification.py` & `sagepy-0.2.8/sagepy/core/modification.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/peptide.py` & `sagepy-0.2.8/sagepy/core/peptide.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/sagepy/core/spectrum.py` & `sagepy-0.2.8/sagepy/core/spectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from typing import List
+from typing import List, Optional
 
 import sagepy_connector
 from numpy.typing import NDArray
 
 from sagepy.core.mass import Tolerance
 psc = sagepy_connector.py_spectrum
 
@@ -79,30 +79,33 @@
 
     def __repr__(self):
         return f"Deisotoped(mz: {self.mz}, intensity: {self.intensity}, charge: {self.charge}, envelope: {self.envelope})"
 
 
 class Precursor:
     def __init__(self, mz: float, intensity: float = None, charge: int = None,
-                 spectrum_ref: str = None, isolation_window: Tolerance = None, inverse_ion_mobility: float = None):
+                 spectrum_ref: str = None, isolation_window: Tolerance = None,
+                 inverse_ion_mobility: float = None, collision_energy: Optional[float] = None):
         """Precursor class
 
         Args:
             mz (float): The mz of the precursor
             intensity (float, optional): The intensity of the precursor. Defaults to None.
             charge (int, optional): The charge of the precursor. Defaults to None.
             spectrum_ref (str, optional): The spectrum reference of the precursor. Defaults to None.
             isolation_window (Tolerance, optional): The isolation window of the precursor. Defaults to None.
             inverse_ion_mobility (float, optional): The inverse ion mobility of the precursor. Defaults to None.
         """
         if isolation_window is not None:
             self.__precursor_ptr = psc.PyPrecursor(mz, intensity, charge,
-                                                   spectrum_ref, isolation_window.get_py_ptr(), inverse_ion_mobility)
+                                                   spectrum_ref, isolation_window.get_py_ptr(), inverse_ion_mobility,
+                                                   collision_energy)
         else:
-            self.__precursor_ptr = psc.PyPrecursor(mz, intensity, charge, spectrum_ref, None, inverse_ion_mobility)
+            self.__precursor_ptr = psc.PyPrecursor(mz, intensity, charge, spectrum_ref, None, inverse_ion_mobility,
+                                                   collision_energy)
 
     @classmethod
     def from_py_precursor(cls, precursor: psc.PyPrecursor):
         instance = cls.__new__(cls)
         instance.__precursor_ptr = precursor
         return instance
 
@@ -130,23 +133,29 @@
         else:
             return None
 
     @property
     def inverse_ion_mobility(self):
         return self.__precursor_ptr.inverse_ion_mobility
 
+    @property
+    def collision_energy(self):
+        return self.__precursor_ptr.collision_energy
+
     def get_py_ptr(self):
         return self.__precursor_ptr
 
     def __repr__(self):
         return (f"Precursor(mz: {np.round(self.mz, 2)}, "
                 f"intensity: {self.intensity}, "
                 f"charge: {self.charge}, "
                 f"spectrum_ref: {self.spectrum_ref}, "
-                f"isolation_window: {self.isolation_window})")
+                f"isolation_window: {self.isolation_window}), "
+                f"inverse_ion_mobility: {np.round(self.inverse_ion_mobility, 2)}, "
+                f"collision_energy: {np.round(self.collision_energy, 2)})")
 
 
 class Representation:
     def __init__(self, representation: str = 'centroid'):
         """Representation class
 
         Args:
@@ -338,25 +347,28 @@
 
 
 class SpectrumProcessor:
     def __init__(
             self, take_top_n: int = 150,
             min_fragment_mz: float = 150,
             max_fragment_mz: float = 2000,
+            min_deisotope_mz: float = 0.0,
             deisotope: bool = False,
     ):
         """SpectrumProcessor class
 
         Args:
             take_top_n (int, optional): The number of peaks to take. Defaults to 150.
             min_fragment_mz (float, optional): The minimum fragment mz. Defaults to 150.
             max_fragment_mz (float, optional): The maximum fragment mz. Defaults to 2000.
+            min_deisotope_mz (float, optional): The minimum deisotope mz. Defaults to 0.0.
             deisotope (bool, optional): Whether to deisotope the spectrum. Defaults to False.
         """
-        self.__spectrum_processor_ptr = psc.PySpectrumProcessor(take_top_n, max_fragment_mz, min_fragment_mz, deisotope)
+        self.__spectrum_processor_ptr = psc.PySpectrumProcessor(
+            take_top_n, max_fragment_mz, min_fragment_mz, min_deisotope_mz, deisotope)
 
     @classmethod
     def from_py_spectrum_processor(cls, spectrum_processor: psc.PySpectrumProcessor):
         instance = cls.__new__(cls)
         instance.__spectrum_processor_ptr = spectrum_processor
         return instance
```

### Comparing `sagepy-0.2.7/sagepy/core/tmt.py` & `sagepy-0.2.8/sagepy/core/tmt.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.7/PKG-INFO` & `sagepy-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sagepy
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: theGreatHerrLebert
 Author-email: davidteschner@googlemail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: pandas (>=1.3.3)
-Requires-Dist: sagepy-connector (>=0.2.7)
+Requires-Dist: sagepy-connector (>=0.2.8)
 Description-Content-Type: text/markdown
 
 # SAGEpy
 A python interface to the core [SAGE](https://github.com/lazear/sage) search engine for mass spectrometry proteomics
 
 <p align="center">
   <img src="sagepy_logo.png" alt="logo" width="250"/>
```

