# Comparing `tmp/pyedaa_reports-0.7.0.tar.gz` & `tmp/pyedaa_reports-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedaa_reports-0.7.0.tar", last modified: Sun May  5 21:21:53 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.7.1.tar", last modified: Sun May  5 22:14:23 2024, max compression
```

## Comparing `pyedaa_reports-0.7.0.tar` & `pyedaa_reports-0.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.115482 pyedaa_reports-0.7.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/Unittesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    34218 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:21:53.119482 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 21:21:53.000000 pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:21:53.127482 pyedaa_reports-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-05 21:21:49.000000 pyedaa_reports-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.496789 pyedaa_reports-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 22:14:23.496789 pyedaa_reports-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.484789 pyedaa_reports-0.7.1/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.488789 pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/
+-rw-r--r--   0 runner    (1001) docker     (127)    34218 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/JUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.492789 pyedaa_reports-0.7.1/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/resources/Unittesting.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:23.492789 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 22:14:23.000000 pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:14:23.496789 pyedaa_reports-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-05 22:14:19.000000 pyedaa_reports-0.7.1/setup.py
```

### Comparing `pyedaa_reports-0.7.0/LICENSE.md` & `pyedaa_reports-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/PKG-INFO` & `pyedaa_reports-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.7.0
+Version: 0.7.1
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
 Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: typing_extensions~=4.11; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: Coverage~=7.5; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: pytest-cov~=5.0; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.7.0/README.md` & `pyedaa_reports-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/Unittesting.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/CLI/Unittesting.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,29 +45,50 @@
 		self.WriteNormal(f"Aggregating unit test metrics ...")
 		merged.Aggregate()
 
 		self.WriteNormal(f"Flattening data structures to a single dimension ...")
 		result = merged.ToTestsuiteSummary()
 
 		if args.pytest is not None:
-			self.WriteNormal(f"Remove overhead from pytest ...")
-			suite = result
+			self.WriteNormal(f"Simplifying unit testing reports created by pytest ...")
 
-			for element in args.pytest.split("."):
-				suite = suite._testsuites[element]
-
-			for ts in suite._testsuites.values():
-				ts._parent = None
-				ts._kind = TestsuiteKind.Logical
-				result.AddTestsuite(ts)
-
-			while suite is not result:
-				name = suite._name
-				suite = suite._parent
-				del suite._testsuites[name]
+			cleanups = []
+			for path in args.pytest.split(";"):
+				suite = result
+				message = f"  Walking: {suite._name}"
+				for element in path.split("."):
+					if element in suite._testsuites:
+						suite = suite._testsuites[element]
+						message += f" -> {suite._name}"
+					else:
+						self.WriteVerbose(f"  Skipping: {path}")
+						suite = None
+						break
+
+				if suite is None:
+					continue
+
+				self.WriteVerbose(message)
+				cleanups.append(suite)
+
+				self.WriteVerbose(f"  Moving testsuites ...")
+				for ts in suite._testsuites.values():
+					self.WriteDebug(f"    {ts._name} -> {result._name}")
+					ts._parent = None
+					ts._kind = TestsuiteKind.Logical
+					result.AddTestsuite(ts)
+
+			self.WriteVerbose(f"  Deleting empty testsuites ...")
+			for clean in cleanups:
+				suite = clean
+				while suite is not result:
+					name = suite._name
+					suite = suite._parent
+					self.WriteDebug(f"    {name}")
+					del suite._testsuites[name]
 
 		self.WriteNormal(f"Writing merged unit test summaries to file ...")
 		mergedFile = Path.cwd() / Path("Unittesting.xml")
 		self.WriteVerbose(f"  Common Data Model -> OUT (JUnit):      {mergedFile}")
 		junitDocument = Document.FromTestsuiteSummary(mergedFile, result)
 		try:
 			junitDocument.Write(regenerate=True, overwrite=True)
```

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/CLI/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Dependency/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/Python.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Requirement/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Requirement/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/JUnit.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/JUnit.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/Unittesting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.7.1/pyEDAA/Reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.7.0"
+__version__ =   "0.7.1"
 __keywords__ =  ["Reports", "Abstract Model", "Data Model", "Unit Testing", "Testcase", "Testsuite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
 from importlib.resources  import files
 from pathlib              import Path
 from sys                  import version_info
 from types                import ModuleType
```

### Comparing `pyedaa_reports-0.7.0/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.7.1/pyEDAA/Reports/resources/Unittesting.xsd`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.7.0
+Version: 0.7.1
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
 Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: typing_extensions~=4.11; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: Coverage~=7.5; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: pytest-cov~=5.0; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/SOURCES.txt` & `pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/pyEDAA.Reports.egg-info/requires.txt` & `pyedaa_reports-0.7.1/pyEDAA.Reports.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+ruamel.yaml~=0.18.6
 lxml~=5.1
 pyTooling~=6.1
-ruamel.yaml~=0.18.6
 
 [all]
-sphinx-copybutton>=0.5.2
 sphinx_design>=0.5.0
-pyTooling~=6.1
-sphinxcontrib-mermaid>=0.9.2
-colorama>=0.4.6
-mypy~=1.10
+sphinx_rtd_theme~=2.0.0
+sphinx~=7.3
 sphinx_autodoc_typehints~=2.1
-setuptools~=69.5
+ruamel.yaml~=0.18.6
+Coverage~=7.5
+docutils~=0.18.1
+mypy~=1.10
+pytest~=8.2
+colorama>=0.4.6
+pyTooling~=6.1
+sphinx-copybutton>=0.5.2
 typing_extensions~=4.11
-pytest-cov~=5.0
-sphinx~=7.3
+autoapi>=2.0.1
 sphinx_reports~=0.6
-docutils~=0.18.1
 lxml~=5.1
-autoapi>=2.0.1
-pytest~=8.2
-Coverage~=7.5
-sphinx_rtd_theme~=2.0.0
-ruamel.yaml~=0.18.6
+pytest-cov~=5.0
+setuptools~=69.5
+sphinxcontrib-mermaid>=0.9.2
 
 [doc]
-sphinx-copybutton>=0.5.2
-setuptools~=69.5
-sphinx~=7.3
-sphinx_rtd_theme~=2.0.0
+colorama>=0.4.6
+lxml~=5.1
 sphinx_design>=0.5.0
+sphinx_rtd_theme~=2.0.0
 docutils~=0.18.1
-lxml~=5.1
+sphinx~=7.3
+autoapi>=2.0.1
 pyTooling~=6.1
+sphinx-copybutton>=0.5.2
+sphinx_autodoc_typehints~=2.1
+setuptools~=69.5
+ruamel.yaml~=0.18.6
 sphinxcontrib-mermaid>=0.9.2
 sphinx_reports~=0.6
-ruamel.yaml~=0.18.6
-colorama>=0.4.6
-autoapi>=2.0.1
-sphinx_autodoc_typehints~=2.1
 
 [test]
-typing_extensions~=4.11
+Coverage~=7.5
 lxml~=5.1
-pyTooling~=6.1
 pytest-cov~=5.0
-ruamel.yaml~=0.18.6
+pyTooling~=6.1
+typing_extensions~=4.11
 mypy~=1.10
+ruamel.yaml~=0.18.6
 pytest~=8.2
-Coverage~=7.5
```

### Comparing `pyedaa_reports-0.7.0/pyproject.toml` & `pyedaa_reports-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.7.0/setup.py` & `pyedaa_reports-0.7.1/setup.py`

 * *Files identical despite different names*

