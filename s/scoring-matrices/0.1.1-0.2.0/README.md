# Comparing `tmp/scoring-matrices-0.1.1.tar.gz` & `tmp/scoring-matrices-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoring-matrices-0.1.1.tar", last modified: Fri May  3 13:38:36 2024, max compression
+gzip compressed data, was "scoring-matrices-0.2.0.tar", last modified: Mon May  6 11:07:15 2024, max compression
```

## Comparing `scoring-matrices-0.1.1.tar` & `scoring-matrices-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:38:36.810581 scoring-matrices-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-03 13:38:36.810581 scoring-matrices-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:38:36.806581 scoring-matrices-0.1.1/scoring_matrices/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/lib.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/lib.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   254460 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices/matrices.h
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/matrices.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:38:36.806581 scoring-matrices-0.1.1/scoring_matrices/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/scoring_matrices/tests/test_scoring_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:38:36.806581 scoring-matrices-0.1.1/scoring_matrices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 13:38:36.000000 scoring-matrices-0.1.1/scoring_matrices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-03 13:38:36.810581 scoring-matrices-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-03 13:38:31.000000 scoring-matrices-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:07:15.320841 scoring-matrices-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-06 11:07:15.320841 scoring-matrices-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:07:15.320841 scoring-matrices-0.2.0/scoring_matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/lib.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16781 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/lib.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   297451 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices/matrices.h
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/matrices.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:07:15.320841 scoring-matrices-0.2.0/scoring_matrices/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/scoring_matrices/tests/test_scoring_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:07:15.320841 scoring-matrices-0.2.0/scoring_matrices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 11:07:15.000000 scoring-matrices-0.2.0/scoring_matrices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-06 11:07:15.324842 scoring-matrices-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-06 11:07:10.000000 scoring-matrices-0.2.0/setup.py
```

### Comparing `scoring-matrices-0.1.1/COPYING` & `scoring-matrices-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `scoring-matrices-0.1.1/PKG-INFO` & `scoring-matrices-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scoring-matrices
-Version: 0.1.1
+Version: 0.2.0
 Summary: Dependency free, Cython-compatible scoring matrices to use with biological sequences.
 Home-page: https://github.com/althonos/score-matrices
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
-License: GPLv3+
+License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/scoring-matrices/issues
 Project-URL: Changelog, https://github.com/althonos/scoring-matrices/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/scoring-matrices/
 Project-URL: Builds, https://github.com/althonos/scoring-matrices/actions
 Keywords: bioinformatics,sequence,substitution,matrix,score
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -44,28 +44,27 @@
 [![PyPI](https://img.shields.io/pypi/v/scoring-matrices.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/scoring-matrices)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/scoring-matrices?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/scoring-matrices)
 [![AUR](https://img.shields.io/aur/version/python-scoring-matrices?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-scoring-matrices)
 [![Wheel](https://img.shields.io/pypi/wheel/scoring-matrices.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scoring-matrices.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/scoring-matrices.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/scoring-matrices/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/)
-[![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/scoring-matrices/)
 [![Issues](https://img.shields.io/github/issues/althonos/scoring-matrices.svg?style=flat-square&maxAge=600)](https://github.com/althonos/scoring-matrices/issues)
 [![Docs](https://img.shields.io/readthedocs/scoring-matrices/latest?style=flat-square&maxAge=600)](https://scoring-matrices.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/blob/main/CHANGELOG.md)
 [![Downloads](https://img.shields.io/pypi/dm/scoring-matrices?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/scoring-matrices)
 
 ## 🗺️ Overview
 
 *Scoring Matrices* are matrices used to score the matches and mismatches between
 two characters are the same position in a sequence alignment. Some of these
 matrices are derived from *substitution matrices*, which uses evolutionary 
 modeling.
 
-The `scoring-matrices` packages is a dependency-free, batteries included library
+The `scoring-matrices` package is a dependency-free, batteries included library
 to handle and distribute common substitution matrices:
 
 - **no external dependencies**: The matrices are distributed as-is: you don't 
   need the whole [Biopython](https://biopython.org) ecosystem, or even 
   [NumPy](https://numpy.org/).
 - **Cython compatibility**: The `ScoringMatrix` is a Cython class that can be
   inherited, and the matrix data can be accessed as either a raw pointer, or
```

### Comparing `scoring-matrices-0.1.1/README.md` & `scoring-matrices-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 [![PyPI](https://img.shields.io/pypi/v/scoring-matrices.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/scoring-matrices)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/scoring-matrices?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/scoring-matrices)
 [![AUR](https://img.shields.io/aur/version/python-scoring-matrices?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-scoring-matrices)
 [![Wheel](https://img.shields.io/pypi/wheel/scoring-matrices.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scoring-matrices.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/scoring-matrices.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/scoring-matrices/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/)
-[![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/scoring-matrices/)
 [![Issues](https://img.shields.io/github/issues/althonos/scoring-matrices.svg?style=flat-square&maxAge=600)](https://github.com/althonos/scoring-matrices/issues)
 [![Docs](https://img.shields.io/readthedocs/scoring-matrices/latest?style=flat-square&maxAge=600)](https://scoring-matrices.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/blob/main/CHANGELOG.md)
 [![Downloads](https://img.shields.io/pypi/dm/scoring-matrices?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/scoring-matrices)
 
 ## 🗺️ Overview
 
 *Scoring Matrices* are matrices used to score the matches and mismatches between
 two characters are the same position in a sequence alignment. Some of these
 matrices are derived from *substitution matrices*, which uses evolutionary 
 modeling.
 
-The `scoring-matrices` packages is a dependency-free, batteries included library
+The `scoring-matrices` package is a dependency-free, batteries included library
 to handle and distribute common substitution matrices:
 
 - **no external dependencies**: The matrices are distributed as-is: you don't 
   need the whole [Biopython](https://biopython.org) ecosystem, or even 
   [NumPy](https://numpy.org/).
 - **Cython compatibility**: The `ScoringMatrix` is a Cython class that can be
   inherited, and the matrix data can be accessed as either a raw pointer, or
```

### Comparing `scoring-matrices-0.1.1/scoring_matrices/lib.pxd` & `scoring-matrices-0.2.0/scoring_matrices/lib.pxd`

 * *Files 15% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 
     cdef size_t        _size
     cdef size_t        _nitems
     cdef Py_ssize_t[2] _shape
 
     cdef float*  _data
     cdef float** _matrix
+    cdef char*   _alphabet
 
     cdef int _allocate(self, size_t length) except 1 nogil
 
-    cdef const float* data(self) except NULL nogil
-    cdef const float** matrix(self) except NULL nogil    
+    cdef const float* data_ptr(self) except NULL nogil
+    cdef const float** matrix_ptr(self) except NULL nogil    
+    cdef const char* alphabet_ptr(self) except NULL nogil
+    cdef size_t size(self) noexcept nogil
 
     cpdef bint is_integer(self)
+    cpdef bint is_symmetric(self)
     cpdef float min(self)
     cpdef float max(self)
     cpdef ScoringMatrix copy(self)
     cpdef ScoringMatrix shuffle(self, str alphabet)
```

### Comparing `scoring-matrices-0.1.1/scoring_matrices/lib.pyi` & `scoring-matrices-0.2.0/scoring_matrices/lib.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 import typing
 from typing import TypeVar, Type, Optional, TextIO, Sequence, ClassVar, Tuple, List
 
 S = TypeVar("S")
 
-
 class ScoringMatrix:
     DEFAULT_ALPHABET: ClassVar[str]
     @classmethod
     def from_name(cls: Type[S], name: str = "BLOSUM62") -> S: ...
     @classmethod
     def from_file(cls: Type[S], file: TextIO, name: Optional[str] = None) -> S: ...
     @classmethod
     def from_str(cls: Type[S], text: str, name: Optional[str] = None) -> S: ...
+    @classmethod
+    def from_diagonal(
+        cls: Type[S],
+        diagonal: Iterable[float],
+        mismatch_score: float = 0.0,
+        alphabet: str = DEFAULT_ALPHABET,
+        name: Optional[str] = None,
+    ) -> S: ...
+    @classmethod
+    def from_match_mismatch(
+        cls: Type[S],
+        match_score: float = 1.0,
+        mismatch_score: float = -0.0,
+        alphabet: str = DEFAULT_ALPHABET,
+        name: Optional[str] = None,
+    ) -> S: ...
     def __init__(
         self,
         matrix: Sequence[Sequence[float]],
         alphabet: str = DEFAULT_ALPHABET,
         name: Optional[str] = None,
     ): ...
     def __copy__(self: S) -> S: ...
@@ -29,10 +44,11 @@
     def __getitem__(self, item: str) -> List[float]: ...
     @typing.overload
     def __getitem__(self, item: Tuple[int, int]) -> float: ...
     @typing.overload
     def __getitem__(self, item: Tuple[str, str]) -> float: ...
     def copy(self: S) -> S: ...
     def is_integer(self) -> bool: ...
+    def is_symmetric(self) -> bool: ...
     def min(self) -> float: ...
     def max(self) -> float: ...
-    def shuffle(self: S, alphabet: str) -> S: ...
+    def shuffle(self: S, alphabet: str) -> S: ...
```

### Comparing `scoring-matrices-0.1.1/scoring_matrices/lib.pyx` & `scoring-matrices-0.2.0/scoring_matrices/lib.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # distutils: language = c
 # cython: language_level=3, linetrace=True, binding=True
+"""Dependency free, Cython-compatible scoring matrices for bioinformatics.
+"""
 
 cimport cython
 from cpython.memoryview cimport PyMemoryView_FromMemory
 from cpython.buffer cimport PyBUF_FORMAT, PyBUF_READ, PyBUF_WRITE
 
 from libc.math cimport INFINITY, lrintf
 from libc.stdlib cimport realloc, free
-from libc.string cimport memcpy
+from libc.string cimport memcpy, memset
 
 from .matrices cimport _NAMES, _ALPHABETS, _SIZES, _MATRICES
 
 import io
 import pickle
 
 
@@ -95,14 +97,77 @@
 
     @classmethod
     def from_str(cls, str text, str name = None):
         """Load a scoring matrix from a string.
         """
         return cls.from_file(io.StringIO(text))
 
+    @classmethod
+    def from_diagonal(
+        cls, 
+        object diagonal, 
+        float mismatch_score=0.0, 
+        str alphabet not None = DEFAULT_ALPHABET, 
+        str name = None
+    ):
+        """Create a scoring matrix from a diagonal vector.
+
+        Arguments:
+            diagonal (sequence of `float`): The diagonal of the scoring
+                matrix, used to score character matches.
+            mismatch_score (`float`): The mismatch score to use for 
+                every mismatches.
+            alphabet (`str`): The alphabet to use with the scoring matrix.
+            name (`str` or `None`): A name for the scoring matrix, if any.
+
+        Example:
+            >>> matrix = ScoringMatrix.from_diagonal(
+            ...     diagonal=[2, 2, 3, 3],
+            ...     mismatch_score=-3.0,
+            ...     alphabet="ATGC",
+            ... )
+            >>> for row in matrix:
+            ...     print(row)
+            [2.0, -3.0, -3.0, -3.0]
+            [-3.0, 2.0, -3.0, -3.0]
+            [-3.0, -3.0, 3.0, -3.0]
+            [-3.0, -3.0, -3.0, 3.0]
+
+        .. versionadded:: 0.2.0
+
+        """
+        cdef list   matrix = []
+        cdef size_t length = len(alphabet)
+
+        for i, x in enumerate(diagonal):
+            row = [ x if j == i else mismatch_score for j in range(length) ]
+            matrix.append(row)
+        return cls(matrix, alphabet=alphabet, name=name)
+
+    @classmethod
+    def from_match_mismatch(
+        cls,
+        float match_score = 1.0, 
+        float mismatch_score = -1.0,
+        str alphabet not None = DEFAULT_ALPHABET,
+        str name = None,
+    ):
+        """Create a scoring matrix from two match/mismatch scores.
+
+        .. versionadded:: 0.2.0
+
+        """
+        cdef list   matrix = []
+        cdef size_t length = len(alphabet)
+
+        for i in range(length):
+            row = [ match_score if j == i else mismatch_score for j in range(length) ]
+            matrix.append(row)
+        return cls(matrix, alphabet=alphabet, name=name)
+
     # --- Magic methods --------------------------------------------------------
 
     def __cinit__(self):
         self._data = NULL
         self._matrix = NULL
         self._size = 0
         self._shape[0] = self._shape[1] = 0
@@ -110,14 +175,39 @@
     def __init__(
         self,
         object matrix not None,
         str alphabet not None = DEFAULT_ALPHABET,
         str name = None,
     ):
         """Create a new scoring matrix.
+
+        Arguments:
+            matrix (array-like of `float`): A square matrix with dimensions
+                equal to the ``alphabet`` length, storing the scores for each
+                pair of characters.
+            alphabet (`str`): The alphabet used to index the rows and columns
+                of the scoring matrix.
+            name (`str` or `None`): The name of the scoring matrix, if any.
+
+        Example:
+            >>> matrix = ScoringMatrix(
+            ...     [[91, -114,  -31, -123],
+            ...      [-114, 100, -125, -31],
+            ...      [-31, -125,  100, -114],
+            ...      [-123, -31, -114,  91]],
+            ...     alphabet="ACGT",
+            ...     name="HOXD70",
+            ... )
+
+        Raises:
+            `ValueError`: When the matrix is not a valid matrix or does not
+                match the given alphabet.
+            `MemoryError`: When memory for storing the scores could not be
+                allocated successfully.
+
         """
         cdef ssize_t i
         cdef ssize_t j
         cdef float   x
         cdef size_t  size = len(alphabet)
 
         if len(alphabet) != len(set(alphabet)):
@@ -127,16 +217,16 @@
 
         self.alphabet = alphabet
         self.name = name
 
         with nogil:
             self._allocate(size)
 
-        assert self._data != NULL
-        assert self._matrix != NULL
+        for i, c in enumerate(self.alphabet):
+            self._alphabet[i] = ord(c)
         for i, row in enumerate(matrix):
             if len(row) != size:
                 raise ValueError("Matrix must contain one column per alphabet letter")
             for j, x in enumerate(row):
                 self._matrix[i][j] = x
 
     def __copy__(self):
@@ -244,39 +334,51 @@
 
     # --- Private methods ------------------------------------------------------
     
     cdef int _allocate(self, size_t size) except 1 nogil:
         cdef size_t i
 
         self._data = <float*> realloc(self._data, sizeof(float) * size * size)
-        if self._data is NULL:
-            raise MemoryError("Failed to allocate matrix")
-
         self._matrix = <float**> realloc(self._matrix, sizeof(float*) * size)
-        if self._matrix is NULL:
+        self._alphabet = <char*> realloc(self._alphabet, sizeof(char) * (size + 1))
+        if self._data is NULL or self._matrix is NULL or self._alphabet is NULL:
             raise MemoryError("Failed to allocate matrix")
 
         self._size = self._shape[0] = self._shape[1] = size
         self._nitems = self._size * self._size
         for i in range(size):
             self._matrix[i] = &self._data[i * self._size]
+        memset(self._alphabet, 0, sizeof(char) * (size + 1))
 
         return 0
 
     # --- Public methods -------------------------------------------------------
 
-    cdef const float* data(self) except NULL nogil:
+    cdef size_t size(self) noexcept nogil:
+        """Get the size of the scoring matrix.
+        """
+        return self._size
+
+    cdef const char* alphabet_ptr(self) except NULL nogil:
+        """Get the alphabet of the scoring matrix as a C-string.
+        """
+        if self._alphabet == NULL:
+            with gil:
+                raise RuntimeError("uninitialized scoring matrix")
+        return <const char*> self._alphabet
+
+    cdef const float* data_ptr(self) except NULL nogil:
         """Get the matrix scores as a dense array.
         """
         if self._data == NULL:
             with gil:
                 raise RuntimeError("uninitialized scoring matrix")
         return <const float*> self._data
 
-    cdef const float** matrix(self) except NULL nogil:
+    cdef const float** matrix_ptr(self) except NULL nogil:
         """Get the matrix scores as an array of pointers.
         """
         if self._matrix == NULL:
             with gil:
                 raise RuntimeError("uninitialized scoring matrix")
         return <const float**> self._matrix
 
@@ -284,37 +386,61 @@
         """Get a copy of the matrix.
         """
         return type(self)(self, alphabet=self.alphabet, name=self.name)
 
     cpdef bint is_integer(self):
         """Test whether the scoring matrix is an integer matrix.
 
+        Returns:
+            `bool`: `True` if the matrix only contains integer scores.
+
         Example:
             >>> blosum62 = ScoringMatrix.from_name("BLOSUM62")
             >>> blosum62.is_integer()
             True
             >>> benner6 = ScoringMatrix.from_name("BENNER6")
             >>> benner6.is_integer()
             False
 
         """
-        assert self._data != NULL
-
-        cdef size_t i
-        cdef float  x
-        cdef bint   integer = True
+        cdef size_t       i
+        cdef float        x
+        cdef bint         integer = True
+        cdef const float* _data   = self.data_ptr()
 
         with nogil:
             for i in range(self._nitems):
-                x = self._data[i]
+                x = _data[i]
                 if lrintf(x) != x:
                     integer = False
                     break
         return integer
 
+    cpdef bint is_symmetric(self):
+        """Test whether the scoring matrix is symmetric.
+
+        Returns:
+            `bool`: `True` if the matrix is a symmetric matrix.
+
+        .. versionadded:: 0.2.0
+
+        """
+        cdef size_t        i
+        cdef size_t        j
+        cdef bint          symmetric = True
+        cdef const float** _matrix   = self.matrix_ptr()
+
+        with nogil:
+            for i in range(self._nitems):
+                for j in range(i + 1, self._nitems):
+                    if _matrix[i][j] != _matrix[j][i]:
+                        symmetric = False
+                        break
+        return symmetric
+
     cpdef float min(self):
         """Get the minimum score of the scoring matrix.
 
         Example:
             >>> blosum62 = ScoringMatrix.from_name("BLOSUM62")
             >>> blosum62.min()
             -4.0
@@ -385,12 +511,12 @@
         for x in alphabet:
             try:
                 indices.append(self.alphabet.index(x))
             except ValueError:
                 raise KeyError(f"new alphabet contains unknown letter: {x!r}") from None
 
         for letter in alphabet:
-            row = self[letter]
+            row = self[<str> letter]
             matrix.append([row[j] for j in indices])
 
         name = self.name if len(alphabet) == len(self.alphabet) else None
         return type(self)(matrix, alphabet=alphabet, name=name)
```

### Comparing `scoring-matrices-0.1.1/scoring_matrices/tests/test_doctest.py` & `scoring-matrices-0.2.0/scoring_matrices/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `scoring-matrices-0.1.1/scoring_matrices.egg-info/PKG-INFO` & `scoring-matrices-0.2.0/scoring_matrices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scoring-matrices
-Version: 0.1.1
+Version: 0.2.0
 Summary: Dependency free, Cython-compatible scoring matrices to use with biological sequences.
 Home-page: https://github.com/althonos/score-matrices
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
-License: GPLv3+
+License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/scoring-matrices/issues
 Project-URL: Changelog, https://github.com/althonos/scoring-matrices/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/scoring-matrices/
 Project-URL: Builds, https://github.com/althonos/scoring-matrices/actions
 Keywords: bioinformatics,sequence,substitution,matrix,score
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -44,28 +44,27 @@
 [![PyPI](https://img.shields.io/pypi/v/scoring-matrices.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/scoring-matrices)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/scoring-matrices?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/scoring-matrices)
 [![AUR](https://img.shields.io/aur/version/python-scoring-matrices?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-scoring-matrices)
 [![Wheel](https://img.shields.io/pypi/wheel/scoring-matrices.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scoring-matrices.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/scoring-matrices/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/scoring-matrices.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/scoring-matrices/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/)
-[![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/scoring-matrices/)
 [![Issues](https://img.shields.io/github/issues/althonos/scoring-matrices.svg?style=flat-square&maxAge=600)](https://github.com/althonos/scoring-matrices/issues)
 [![Docs](https://img.shields.io/readthedocs/scoring-matrices/latest?style=flat-square&maxAge=600)](https://scoring-matrices.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/scoring-matrices/blob/main/CHANGELOG.md)
 [![Downloads](https://img.shields.io/pypi/dm/scoring-matrices?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/scoring-matrices)
 
 ## 🗺️ Overview
 
 *Scoring Matrices* are matrices used to score the matches and mismatches between
 two characters are the same position in a sequence alignment. Some of these
 matrices are derived from *substitution matrices*, which uses evolutionary 
 modeling.
 
-The `scoring-matrices` packages is a dependency-free, batteries included library
+The `scoring-matrices` package is a dependency-free, batteries included library
 to handle and distribute common substitution matrices:
 
 - **no external dependencies**: The matrices are distributed as-is: you don't 
   need the whole [Biopython](https://biopython.org) ecosystem, or even 
   [NumPy](https://numpy.org/).
 - **Cython compatibility**: The `ScoringMatrix` is a Cython class that can be
   inherited, and the matrix data can be accessed as either a raw pointer, or
```

### Comparing `scoring-matrices-0.1.1/scoring_matrices.egg-info/SOURCES.txt` & `scoring-matrices-0.2.0/scoring_matrices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scoring-matrices-0.1.1/setup.cfg` & `scoring-matrices-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = attr: scoring_matrices.__version__
 author = Martin Larralde
 author_email = martin.larralde@embl.de
 url = https://github.com/althonos/score-matrices
 description = Dependency free, Cython-compatible scoring matrices to use with biological sequences.
 long_description = file: README.md
 long_description_content_type = text/markdown
-license = GPLv3+
+license = MIT
 platform = any
 keywords = bioinformatics, sequence, substitution, matrix, score
 classifier = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
```

### Comparing `scoring-matrices-0.1.1/setup.py` & `scoring-matrices-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,20 @@
                 alphabet, _ = matrices[name]
                 dst.write(f'{len(alphabet)}, ')
             dst.write("-1 };\n")
 
             for i, (name, id_) in enumerate(zip(names, ids)):
                 alphabet, matrix = matrices[name]
                 nitems = len(matrix) * len(matrix)
-                dst.write(f"float _MATRIX_{id_}[{nitems}] = {{ { ', '.join(map(repr, itertools.chain.from_iterable(matrix))) } }};\n")
+                dst.write(f"float _MATRIX_{id_}[{nitems}] = {{")
+                for i, item in enumerate(itertools.chain.from_iterable(matrix)):
+                    if i != 0:
+                        dst.write(", ")
+                    dst.write(f"{item!r}F")
+                dst.write("};\n")
 
             dst.write(f"const float* _MATRICES[{len(names) + 1}] = {{")
             for id_ in ids:
                 dst.write(f'_MATRIX_{id_}, ')
             dst.write("NULL };\n")
```

