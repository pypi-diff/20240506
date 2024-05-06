# Comparing `tmp/fasts2-0.0.2.tar.gz` & `tmp/fasts2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasts2-0.0.2.tar", max compression
+gzip compressed data, was "fasts2-0.0.3.tar", max compression
```

## Comparing `fasts2-0.0.2.tar` & `fasts2-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2024-05-03 10:52:22.901032 fasts2-0.0.2/LICENSE
--rw-r--r--   0        0        0     2462 2024-05-03 10:53:11.467399 fasts2-0.0.2/README.md
--rw-r--r--   0        0        0      114 2024-05-03 14:30:14.673075 fasts2-0.0.2/fasts2/__init__.py
--rw-r--r--   0        0        0     4024 2024-05-03 14:30:14.669075 fasts2-0.0.2/fasts2/main.py
--rw-r--r--   0        0        0     3676 2024-05-03 14:30:14.677075 fasts2-0.0.2/fasts2/task1.py
--rw-r--r--   0        0        0     9016 2024-05-03 14:30:23.344804 fasts2-0.0.2/fasts2/task2.py
--rw-r--r--   0        0        0     3275 2024-05-03 14:30:14.673075 fasts2-0.0.2/fasts2/utils.py
--rw-r--r--   0        0        0     1967 2024-05-03 14:31:49.290130 fasts2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 fasts2-0.0.2/setup.py
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 fasts2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 10:52:22.901032 fasts2-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2462 2024-05-03 10:53:11.467399 fasts2-0.0.3/README.md
+-rw-r--r--   0        0        0      114 2024-05-03 14:30:14.673075 fasts2-0.0.3/fasts2/__init__.py
+-rw-r--r--   0        0        0     4023 2024-05-05 19:08:05.630881 fasts2-0.0.3/fasts2/main.py
+-rw-r--r--   0        0        0     3672 2024-05-03 14:32:01.201759 fasts2-0.0.3/fasts2/task1.py
+-rw-r--r--   0        0        0     9016 2024-05-03 14:30:23.344804 fasts2-0.0.3/fasts2/task2.py
+-rw-r--r--   0        0        0     3275 2024-05-03 14:30:14.673075 fasts2-0.0.3/fasts2/utils.py
+-rw-r--r--   0        0        0     1974 2024-05-06 08:42:23.969884 fasts2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 fasts2-0.0.3/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 fasts2-0.0.3/PKG-INFO
```

### Comparing `fasts2-0.0.2/LICENSE` & `fasts2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fasts2-0.0.2/README.md` & `fasts2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fasts2-0.0.2/fasts2/main.py` & `fasts2-0.0.3/fasts2/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pathlib
 from typing import Any, List, Literal, Optional, Union
 
 import pydantic
 import torch
-
 from fasts2.task1 import t1_worker
 from fasts2.task2 import t2_cleaner, t2_worker
 from fasts2.utils import fix_coordinates, load_cloud_model
 
 
 class S2GoogleTask(pydantic.BaseModel):
     """Create a new download task for retrieve
```

### Comparing `fasts2-0.0.2/fasts2/task1.py` & `fasts2-0.0.3/fasts2/task1.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,9 +105,10 @@
         # If there is an exception, raise it
         for future in concurrent.futures.as_completed(futures):
             if future.exception() is not None:
                 raise future.exception()
 
 
 # send package to the pypi
-# python setup.py sdist bdist_wheel
+# poetry build
+# poetry publish
 # twine upload dist/*
```

### Comparing `fasts2-0.0.2/fasts2/task2.py` & `fasts2-0.0.3/fasts2/task2.py`

 * *Files identical despite different names*

### Comparing `fasts2-0.0.2/fasts2/utils.py` & `fasts2-0.0.3/fasts2/utils.py`

 * *Files identical despite different names*

### Comparing `fasts2-0.0.2/pyproject.toml` & `fasts2-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "fasts2"
-version = "0.0.2"
-description = "🏎💨vroom vroom S2 imagery downloader"
+version = "0.0.3"
+description = "🏎💨vroom vroom - S2 imagery downloader"
 authors = ["Cesar Aybar <fcesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/fastS2"
 documentation = "https://csaybar.github.io/fastS2/"
 readme = "README.md"
 packages = [
   {include = "fasts2"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pydantic = ">=2.0.0"
-planetary-computer = "^1.0.0"
-pystac-client = "^0.7.7"
-stackstac = "^0.5.0"
-torch = ">=2.0.0"
-earthengine-api = "^0.1.401"
-shapely = "^2.0.4"
+planetary-computer = ">=1.0.0"
+pystac-client = ">=0.7.7"
+stackstac = ">=0.5.0"
+torch = ">=2.2.0"
+earthengine-api = ">=0.1.400"
+shapely = ">=2.0.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `fasts2-0.0.2/setup.py` & `fasts2-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['fasts2']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['earthengine-api>=0.1.401,<0.2.0',
- 'planetary-computer>=1.0.0,<2.0.0',
+['earthengine-api>=0.1.400',
+ 'planetary-computer>=1.0.0',
  'pydantic>=2.0.0',
- 'pystac-client>=0.7.7,<0.8.0',
- 'shapely>=2.0.4,<3.0.0',
- 'stackstac>=0.5.0,<0.6.0',
- 'torch>=2.0.0']
+ 'pystac-client>=0.7.7',
+ 'shapely>=2.0.4',
+ 'stackstac>=0.5.0',
+ 'torch>=2.2.0']
 
 setup_kwargs = {
     'name': 'fasts2',
-    'version': '0.0.2',
-    'description': '🏎💨vroom vroom S2 imagery downloader',
+    'version': '0.0.3',
+    'description': '🏎💨vroom vroom - S2 imagery downloader',
     'long_description': '# fastS2\n\n[![Release](https://img.shields.io/github/v/release/csaybar/fastS2)](https://img.shields.io/github/v/release/csaybar/fastS2)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/fastS2/main.yml?branch=main)](https://github.com/csaybar/fastS2/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/fastS2/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/fastS2)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/fastS2)](https://img.shields.io/github/commit-activity/m/csaybar/fastS2)\n[![License](https://img.shields.io/github/license/csaybar/fastS2)](https://img.shields.io/github/license/csaybar/fastS2)\n\n🏎💨 vroom vroom S2 imagery\n\n- **Github repository**: <https://github.com/csaybar/fastS2/>\n- **Documentation** <https://csaybar.github.io/fastS2/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/fastS2.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/fastS2/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/fastS2/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'fcesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/fastS2',
     'packages': packages,
```

### Comparing `fasts2-0.0.2/PKG-INFO` & `fasts2-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fasts2
-Version: 0.0.2
-Summary: 🏎💨vroom vroom S2 imagery downloader
+Version: 0.0.3
+Summary: 🏎💨vroom vroom - S2 imagery downloader
 Home-page: https://github.com/csaybar/fastS2
 Author: Cesar Aybar
 Author-email: fcesar.aybar@uv.es
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: earthengine-api (>=0.1.401,<0.2.0)
-Requires-Dist: planetary-computer (>=1.0.0,<2.0.0)
+Requires-Dist: earthengine-api (>=0.1.400)
+Requires-Dist: planetary-computer (>=1.0.0)
 Requires-Dist: pydantic (>=2.0.0)
-Requires-Dist: pystac-client (>=0.7.7,<0.8.0)
-Requires-Dist: shapely (>=2.0.4,<3.0.0)
-Requires-Dist: stackstac (>=0.5.0,<0.6.0)
-Requires-Dist: torch (>=2.0.0)
+Requires-Dist: pystac-client (>=0.7.7)
+Requires-Dist: shapely (>=2.0.4)
+Requires-Dist: stackstac (>=0.5.0)
+Requires-Dist: torch (>=2.2.0)
 Project-URL: Documentation, https://csaybar.github.io/fastS2/
 Project-URL: Repository, https://github.com/csaybar/fastS2
 Description-Content-Type: text/markdown
 
 # fastS2
 
 [![Release](https://img.shields.io/github/v/release/csaybar/fastS2)](https://img.shields.io/github/v/release/csaybar/fastS2)
```

