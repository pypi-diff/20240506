# Comparing `tmp/release_by_changelog-0.2.1.tar.gz` & `tmp/release_by_changelog-0.2.2.tar.gz`

## Comparing `release_by_changelog-0.2.1.tar` & `release_by_changelog-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/release-by-changelog.iml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0    31905 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/requirements/dev.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/requirements/prod.txt
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/requirements/quality.txt
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/requirements/test.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/app.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/logging.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/typings_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/cmds/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/cmds/_release.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/cmds/release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/services/__init__.py
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/src/release_by_changelog/services/release.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/tests/CHANGELOG.md
--rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/tests/test_main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/.gitignore
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/AUTHORS.rst
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/LICENCE
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/README.md
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 release_by_changelog-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/.gitignore
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/misc.xml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/modules.xml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/release-by-changelog.iml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    31905 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/requirements/dev.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/requirements/prod.txt
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/requirements/quality.txt
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/requirements/test.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/app.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/logging.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/typings_.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/cmds/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/cmds/_release.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/cmds/release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/services/__init__.py
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/src/release_by_changelog/services/release.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/tests/CHANGELOG.md
+-rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/tests/test_main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/.gitignore
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/LICENCE
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/README.md
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 release_by_changelog-0.2.2/PKG-INFO
```

### Comparing `release_by_changelog-0.2.1/.gitlab-ci.yml` & `release_by_changelog-0.2.2/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 include:
     # https://r2devops.io/marketplace/gitlab/swepy/cicd-templates/ruff/ruff
     -   remote: 'https://gitlab.com/swepy/cicd-templates/ruff/-/raw/ruff@1.0.2/ruff.yml'
     # https://r2devops.io/marketplace/gitlab/dorianturba-templates/r2devops_catalog/r2_metadata/pytest
     -   remote: 'https://gitlab.com/dorianturba-templates/r2devops_catalog/-/raw/main/templates/python/testing/pytest/pytest.yml'
     # https://r2devops.io/marketplace/gitlab/swepy/cicd-templates/release-by-changelog/release-by-changelog
-    -   remote: 'https://gitlab.com/swepy/cicd-templates/release-by-changelog/-/raw/release-by-changelog@0.2.2/release-by-changelog.yml'
+    -   remote: 'https://gitlab.com/swepy/cicd-templates/release-by-changelog/-/raw/release-by-changelog@0.2.3/release-by-changelog.yml'
 
 variables:
     PACKAGE_NAME: "release_by_changelog"
 
 pytest:
     variables:
         PYTHON_SETUP: "pip install .[test]"
```

### Comparing `release_by_changelog-0.2.1/CHANGELOG.md` & `release_by_changelog-0.2.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 [![Pipeline](https://lab.frogg.it/swepy/release-by-changelog/badges/trunk/pipeline.svg)](https://lab.frogg.it/swepy/release-by-changelog/-/pipelines?ref=trunk)
 
+## [0.2.2] - 2024-05-06
+
+[![Pipeline](https://lab.frogg.it/swepy/release-by-changelog/badges/0.2.2/pipeline.svg)](https://lab.frogg.it/swepy/release-by-changelog/-/pipelines?ref=0.2.2)
+
 ## [0.2.1] - 2024-05-06
 
 [![Pipeline](https://lab.frogg.it/swepy/release-by-changelog/badges/0.2.1/pipeline.svg)](https://lab.frogg.it/swepy/release-by-changelog/-/pipelines?ref=0.2.1)
 
 ### Planned
 
 #### Changed
```

### Comparing `release_by_changelog-0.2.1/CONTRIBUTING.md` & `release_by_changelog-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/.idea/workspace.xml` & `release_by_changelog-0.2.2/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `release_by_changelog-0.2.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/requirements/dev.txt` & `release_by_changelog-0.2.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/requirements/prod.txt` & `release_by_changelog-0.2.2/requirements/prod.txt`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/requirements/quality.txt` & `release_by_changelog-0.2.2/requirements/quality.txt`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/requirements/test.txt` & `release_by_changelog-0.2.2/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/src/release_by_changelog/logging.py` & `release_by_changelog-0.2.2/src/release_by_changelog/logging.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/src/release_by_changelog/cmds/_release.py` & `release_by_changelog-0.2.2/src/release_by_changelog/cmds/_release.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/src/release_by_changelog/cmds/release.py` & `release_by_changelog-0.2.2/src/release_by_changelog/cmds/release.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/src/release_by_changelog/services/release.py` & `release_by_changelog-0.2.2/src/release_by_changelog/services/release.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/tests/conftest.py` & `release_by_changelog-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/tests/test_main.py` & `release_by_changelog-0.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/.gitignore` & `release_by_changelog-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/LICENCE` & `release_by_changelog-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/README.md` & `release_by_changelog-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `release_by_changelog-0.2.1/pyproject.toml` & `release_by_changelog-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "release_by_changelog"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {email = "releasebychangelog.rjsts@simplelogin.com", name = "Dorian Turba"},
 ]
 description = "Release a new version of a software based on CHANGELOG.md file."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -58,15 +58,15 @@
     "integration",
 ]
 
 [tool.bumpversion]
 allow-dirty = true
 commit = true
 config-file = "pyproject.toml"
-current_version = "0.2.1"
+current_version = "0.2.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 replace = "{new_version}"
 search = "{current_version}"
 serialize = [
     "{major}.{minor}.{patch}",
 ]
 tag = false
```

### Comparing `release_by_changelog-0.2.1/PKG-INFO` & `release_by_changelog-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: release_by_changelog
-Version: 0.2.1
+Version: 0.2.2
 Summary: Release a new version of a software based on CHANGELOG.md file.
 Project-URL: Bug Tracker, https://lab.frogg.it/swepy/release-by-changelog/-/issues
 Project-URL: Homepage, https://lab.frogg.it/swepy/release-by-changelog
 Author-email: Dorian Turba <releasebychangelog.rjsts@simplelogin.com>
 License-File: AUTHORS.rst
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
```

