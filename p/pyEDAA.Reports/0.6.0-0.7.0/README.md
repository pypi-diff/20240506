# Comparing `tmp/pyedaa_reports-0.6.0.tar.gz` & `tmp/pyedaa_reports-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedaa_reports-0.6.0.tar", last modified: Sun May  5 18:18:47 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.7.0.tar", last modified: Sun May  5 21:21:53 2024, max compression
```

## Comparing `pyedaa_reports-0.6.0.tar` & `pyedaa_reports-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.252588 pyedaa_reports-0.6.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/Unittesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.115482 pyedaa_reports-0.7.0/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/
+-rw-r--r--   0 runner    (1001) docker     (127)    34218 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/JUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/Unittesting.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/setup.py
```

### Comparing `pyedaa_reports-0.6.0/LICENSE.md` & `pyedaa_reports-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/PKG-INFO` & `pyedaa_reports-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.6.0
+Version: 0.7.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -19,60 +19,60 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: lxml~=5.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
 Provides-Extra: all
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
 Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.6.0/README.md` & `pyedaa_reports-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/Unittesting.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/Unittesting.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from pathlib import Path
 from typing import List
 
 from pyTooling.Attributes.ArgParse import CommandHandler
 from pyTooling.Attributes.ArgParse.ValuedFlag import LongValuedFlag
 from pyTooling.MetaClasses import ExtendedType
 
-from pyEDAA.Reports.Unittesting       import Document, MergedTestsuiteSummary
+from pyEDAA.Reports.Unittesting       import Document, MergedTestsuiteSummary, TestsuiteKind
 from pyEDAA.Reports.Unittesting.JUnit import Document, JUnitReaderMode, UnittestException
 
 
 class UnittestingHandlers(metaclass=ExtendedType, mixin=True):
 	@CommandHandler("merge-unittest", help="Merge unit testing results.", description="Merge unit testing results.")
 	@LongValuedFlag("--junit", dest="junit", metaName='JUnitFile', help="Unit testing summary file (XML).")
+	@LongValuedFlag("--pytest", dest="pytest", metaName='Package', help="Remove pytest overhead.")
 	def HandleMergeUnittest(self, args: Namespace) -> None:
 		"""Handle program calls with command ``merge-unittest``."""
 		self._PrintHeadline()
 
 		returnCode = 0
 		if args.junit is None:
 			self.WriteError(f"Option '--junit <JUnitFile' is missing.")
@@ -43,14 +44,31 @@
 
 		self.WriteNormal(f"Aggregating unit test metrics ...")
 		merged.Aggregate()
 
 		self.WriteNormal(f"Flattening data structures to a single dimension ...")
 		result = merged.ToTestsuiteSummary()
 
+		if args.pytest is not None:
+			self.WriteNormal(f"Remove overhead from pytest ...")
+			suite = result
+
+			for element in args.pytest.split("."):
+				suite = suite._testsuites[element]
+
+			for ts in suite._testsuites.values():
+				ts._parent = None
+				ts._kind = TestsuiteKind.Logical
+				result.AddTestsuite(ts)
+
+			while suite is not result:
+				name = suite._name
+				suite = suite._parent
+				del suite._testsuites[name]
+
 		self.WriteNormal(f"Writing merged unit test summaries to file ...")
 		mergedFile = Path.cwd() / Path("Unittesting.xml")
 		self.WriteVerbose(f"  Common Data Model -> OUT (JUnit):      {mergedFile}")
 		junitDocument = Document.FromTestsuiteSummary(mergedFile, result)
 		try:
 			junitDocument.Write(regenerate=True, overwrite=True)
 		except UnittestException as ex:
```

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/Python.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/JUnit.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/JUnit.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,18 +160,18 @@
 
 	def __init__(
 		self,
 		name: str,
 		duration:  Nullable[timedelta] = None,
 		status: TestcaseStatus = TestcaseStatus.Unknown,
 		assertionCount: Nullable[int] = None,
-		parent: Nullable["TestClass"] = None
+		parent: Nullable["Testclass"] = None
 	):
 		if parent is not None:
-			if not isinstance(parent, TestClass):
+			if not isinstance(parent, Testclass):
 				raise TypeError(f"Parameter 'parent' is not of type 'Class'.")
 
 			parent._testcases[name] = self
 
 		super().__init__(name, duration, assertionCount, parent)
 
 		self._status = status
@@ -328,15 +328,15 @@
 
 	@mustoverride
 	def Iterate(self, scheme: IterationScheme = IterationScheme.Default) -> Generator[Union[TestsuiteType, Testcase], None, None]:
 		pass
 
 
 @export
-class TestClass(Base):
+class Testclass(Base):
 	_testcases: Dict[str, "Testcase"]
 
 	def __init__(
 		self,
 		classname: str,
 		testcases: Nullable[Iterable["Testcase"]] = None,
 		parent: Nullable["Testsuite"] = None
@@ -414,24 +414,24 @@
 
 		return node
 
 
 @export
 class Testsuite(TestsuiteBase):
 	_hostname:    str
-	_testclasses: Dict[str, "TestClass"]
+	_testclasses: Dict[str, "Testclass"]
 
 	def __init__(
 		self,
 		name: str,
 		hostname: Nullable[str] = None,
 		startTime: Nullable[datetime] = None,
 		duration:  Nullable[timedelta] = None,
 		status: TestsuiteStatus = TestsuiteStatus.Unknown,
-		testclasses: Nullable[Iterable["TestClass"]] = None,
+		testclasses: Nullable[Iterable["Testclass"]] = None,
 		parent: Nullable["TestsuiteSummary"] = None
 	):
 		if parent is not None:
 			if not isinstance(parent, TestsuiteSummary):
 				raise TypeError(f"Parameter 'parent' is not of type 'TestsuiteSummary'.")
 
 			parent._testsuites[name] = self
@@ -453,15 +453,15 @@
 				self._testclasses[testclass._name] = testclass
 
 	@readonly
 	def Hostname(self) -> Nullable[str]:
 		return self._hostname
 
 	@readonly
-	def Testclasses(self) -> Dict[str, "TestClass"]:
+	def Testclasses(self) -> Dict[str, "Testclass"]:
 		return self._testclasses
 
 	@readonly
 	def TestclassCount(self) -> int:
 		return len(self._testclasses)
 
 	# @readonly
@@ -472,25 +472,25 @@
 	def TestcaseCount(self) -> int:
 		return sum(cls.TestcaseCount for cls in self._testclasses.values())
 
 	@readonly
 	def AssertionCount(self) -> int:
 		return sum(cls.AssertionCount for cls in self._testclasses.values())
 
-	def AddTestclass(self, testclass: "TestClass") -> None:
+	def AddTestclass(self, testclass: "Testclass") -> None:
 		if testclass._parent is not None:
 			raise ValueError(f"Class '{testclass._name}' is already part of a testsuite hierarchy.")
 
 		if testclass._name in self._testclasses:
 			raise DuplicateTestcaseException(f"Testsuite already contains a class with same name '{testclass._name}'.")
 
 		testclass._parent = self
 		self._testclasses[testclass._name] = testclass
 
-	def AddTestclasses(self, testclasses: Iterable["TestClass"]) -> None:
+	def AddTestclasses(self, testclasses: Iterable["Testclass"]) -> None:
 		for testcase in testclasses:
 			self.AddTestclass(testcase)
 
 	# def IterateTestsuites(self, scheme: IterationScheme = IterationScheme.TestsuiteDefault) -> Generator[TestsuiteType, None, None]:
 	# 	return self.Iterate(scheme)
 
 	def IterateTestcases(self, scheme: IterationScheme = IterationScheme.TestcaseDefault) -> Generator[Testcase, None, None]:
@@ -590,37 +590,53 @@
 		for tc in testsuite.IterateTestcases():
 			ts = tc._parent
 			if ts is None:
 				raise UnittestException(f"Testcase '{tc._name}' is not part of a hierarchy.")
 
 			classname = ts._name
 			ts = ts._parent
-			while ts is not None and ts.Kind > TestsuiteKind.Logical:
+			while ts is not None and ts._kind > TestsuiteKind.Logical:
 				classname = f"{ts._name}.{classname}"
 				ts = ts._parent
 
 			if classname in juTestsuite._testclasses:
 				juClass = juTestsuite._testclasses[classname]
 			else:
-				juClass = TestClass(classname, parent=juTestsuite)
+				juClass = Testclass(classname, parent=juTestsuite)
 
 			juClass.AddTestcase(Testcase.FromTestcase(tc))
 
 		return juTestsuite
 
 	def ToTestsuite(self) -> ut_Testsuite:
-		return ut_Testsuite(
+		testsuite = ut_Testsuite(
 			self._name,
 			TestsuiteKind.Logical,
 			startTime=self._startTime,
 			totalDuration=self._duration,
 			status=self._status,
-			testsuites=(cls.ToTestsuite() for cls in self._testclasses.values())
 		)
 
+		for testclass in self._testclasses.values():
+			suite = testsuite
+			classpath = testclass._name.split(".")
+			for element in classpath:
+				if element in suite._testsuites:
+					suite = suite._testsuites[element]
+				else:
+					suite = ut_Testsuite(element, kind=TestsuiteKind.Package, parent=suite)
+
+			suite._kind = TestsuiteKind.Class
+			if suite._parent is not testsuite:
+				suite._parent._kind = TestsuiteKind.Module
+
+			suite.AddTestcases(tc.ToTestcase() for tc in testclass._testcases.values())
+
+		return testsuite
+
 	def ToTree(self) -> Node:
 		node = Node(
 			value=self._name,
 			children=(cls.ToTree() for cls in self._testclasses.values())
 		)
 		node["startTime"] = self._startTime
 		node["duration"] = self._duration
@@ -913,15 +929,15 @@
 		# 	except KeyError:
 		# 		currentTestsuite._testsuites[testsuiteName] = new = Testsuite(testsuiteName)
 		# 		currentTestsuite = new
 
 		if className in parent._testclasses:
 			testclass = parent._testclasses[className]
 		else:
-			testclass = TestClass(className, parent=parent)
+			testclass = Testclass(className, parent=parent)
 
 		testcase = Testcase(name, duration=timedelta(seconds=time), parent=testclass)
 
 		for node in testsuiteNode.iterchildren():   # type: _Element
 			if isinstance(node, _Comment):
 				pass
 			elif isinstance(node, _Element):
@@ -985,17 +1001,17 @@
 
 		for testclass in testsuite._testclasses.values():
 			for tc in testclass._testcases.values():
 				self._GenerateTestcase(tc, testsuiteElement)
 
 	def _GenerateTestcase(self, testcase: Testcase, parentElement: _Element):
 		testcaseElement = SubElement(parentElement, "testcase")
-		testcaseElement.attrib["name"] = testcase._name
 		if testcase.Classname is not None:
 			testcaseElement.attrib["classname"] = testcase.Classname
+		testcaseElement.attrib["name"] = testcase._name
 		if testcase._duration is not None:
 			testcaseElement.attrib["time"] = f"{testcase._duration.total_seconds():.6f}"
 		if testcase._assertionCount is not None:
 			testcaseElement.attrib["assertions"] = f"{testcase._assertionCount}"
 
 		if testcase._status is TestcaseStatus.Passed:
 			pass
```

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -466,14 +466,18 @@
 		self._skipped =      0
 		self._errored =      0
 		self._weak =         0
 		self._failed =       0
 		self._passed =       0
 
 	@readonly
+	def Kind(self) -> TestsuiteKind:
+		return self._kind
+
+	@readonly
 	def Status(self) -> TestsuiteStatus:
 		return self._status
 
 	@readonly
 	def Testsuites(self) -> Dict[str, TestsuiteType]:
 		return self._testsuites
 
@@ -667,18 +671,14 @@
 				if testcase._name in self._testcases:
 					raise DuplicateTestcaseException(f"Testsuite already contains a testcase with same name '{testcase._name}'.")
 
 				testcase._parent = self
 				self._testcases[testcase._name] = testcase
 
 	@readonly
-	def Kind(self) -> TestsuiteKind:
-		return self._kind
-
-	@readonly
 	def Testcases(self) -> Dict[str, "Testcase"]:
 		return self._testcases
 
 	@readonly
 	def TestcaseCount(self) -> int:
 		return super().TestcaseCount + len(self._testcases)
```

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.7.0/pyEDAA/Reports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.6.0"
+__version__ =   "0.7.0"
 __keywords__ =  ["Reports", "Abstract Model", "Data Model", "Unit Testing", "Testcase", "Testsuite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
 from importlib.resources  import files
 from pathlib              import Path
 from sys                  import version_info
 from types                import ModuleType
```

### Comparing `pyedaa_reports-0.6.0/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.7.0/pyEDAA/Reports/resources/Unittesting.xsd`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.6.0
+Version: 0.7.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -19,60 +19,60 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: lxml~=5.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
 Provides-Extra: all
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
 Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/SOURCES.txt` & `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/requires.txt` & `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 lxml~=5.1
-ruamel.yaml~=0.18.6
 pyTooling~=6.1
+ruamel.yaml~=0.18.6
 
 [all]
 sphinx-copybutton>=0.5.2
-Coverage~=7.5
-sphinx_reports~=0.6
-autoapi>=2.0.1
-lxml~=5.1
-ruamel.yaml~=0.18.6
+sphinx_design>=0.5.0
+pyTooling~=6.1
 sphinxcontrib-mermaid>=0.9.2
 colorama>=0.4.6
-sphinx_design>=0.5.0
 mypy~=1.10
+sphinx_autodoc_typehints~=2.1
+setuptools~=69.5
 typing_extensions~=4.11
-pyTooling~=6.1
-sphinx~=7.3
-pytest~=8.2
 pytest-cov~=5.0
+sphinx~=7.3
+sphinx_reports~=0.6
 docutils~=0.18.1
+lxml~=5.1
+autoapi>=2.0.1
+pytest~=8.2
+Coverage~=7.5
 sphinx_rtd_theme~=2.0.0
-setuptools~=69.5
-sphinx_autodoc_typehints~=2.1
+ruamel.yaml~=0.18.6
 
 [doc]
-ruamel.yaml~=0.18.6
 sphinx-copybutton>=0.5.2
-sphinxcontrib-mermaid>=0.9.2
-docutils~=0.18.1
-colorama>=0.4.6
+setuptools~=69.5
+sphinx~=7.3
 sphinx_rtd_theme~=2.0.0
 sphinx_design>=0.5.0
-sphinx_reports~=0.6
-pyTooling~=6.1
+docutils~=0.18.1
 lxml~=5.1
-setuptools~=69.5
+pyTooling~=6.1
+sphinxcontrib-mermaid>=0.9.2
+sphinx_reports~=0.6
+ruamel.yaml~=0.18.6
+colorama>=0.4.6
 autoapi>=2.0.1
-sphinx~=7.3
 sphinx_autodoc_typehints~=2.1
 
 [test]
-ruamel.yaml~=0.18.6
-pytest-cov~=5.0
-Coverage~=7.5
-mypy~=1.10
 typing_extensions~=4.11
-pyTooling~=6.1
 lxml~=5.1
+pyTooling~=6.1
+pytest-cov~=5.0
+ruamel.yaml~=0.18.6
+mypy~=1.10
 pytest~=8.2
+Coverage~=7.5
```

### Comparing `pyedaa_reports-0.6.0/pyproject.toml` & `pyedaa_reports-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.6.0/setup.py` & `pyedaa_reports-0.7.0/setup.py`

 * *Files identical despite different names*

