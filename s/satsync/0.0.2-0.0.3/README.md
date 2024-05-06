# Comparing `tmp/satsync-0.0.2.tar.gz` & `tmp/satsync-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsync-0.0.2.tar", max compression
+gzip compressed data, was "satsync-0.0.3.tar", max compression
```

## Comparing `satsync-0.0.2.tar` & `satsync-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.2/LICENSE
--rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.2/README.md
--rw-r--r--   0        0        0     1962 2024-05-06 08:26:23.189437 satsync-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.2/satsync/__init__.py
--rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.2/satsync/ecc.py
--rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.2/satsync/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.2/satsync/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.2/satsync/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.2/satsync/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.2/satsync/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.2/satsync/lightglue/viz2d.py
--rw-r--r--   0        0        0    14302 2024-05-06 08:18:46.478456 satsync-0.0.2/satsync/main.py
--rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.2/satsync/pcc.py
--rw-r--r--   0        0        0    13287 2024-05-06 08:25:49.514397 satsync-0.0.2/satsync/utils.py
--rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 satsync-0.0.2/setup.py
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 satsync-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.3/README.md
+-rw-r--r--   0        0        0     1987 2024-05-06 08:39:16.207269 satsync-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.3/satsync/__init__.py
+-rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.3/satsync/ecc.py
+-rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.3/satsync/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.3/satsync/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.3/satsync/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.3/satsync/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.3/satsync/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.3/satsync/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.3/satsync/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.3/satsync/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.3/satsync/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.3/satsync/lightglue/viz2d.py
+-rw-r--r--   0        0        0    14302 2024-05-06 08:18:46.478456 satsync-0.0.3/satsync/main.py
+-rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.3/satsync/pcc.py
+-rw-r--r--   0        0        0    13287 2024-05-06 08:25:49.514397 satsync-0.0.3/satsync/utils.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 satsync-0.0.3/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 satsync-0.0.3/PKG-INFO
```

### Comparing `satsync-0.0.2/LICENSE` & `satsync-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/README.md` & `satsync-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/pyproject.toml` & `satsync-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "satsync"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python package to align satellite images."
 authors = ["Cesar Aybar <fcesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satsync"
 documentation = "https://csaybar.github.io/satsync/"
 readme = "README.md"
 packages = [
   {include = "satsync"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-numpy = "^1.26.4"
-xarray = "^2024.3.0"
-rasterio = "^1.3.10"
-scikit-image = "^0.23.2"
-opencv-python = "^4.9.0.80"
-pandas = "^2.2.2"
-kornia = "^0.7.2"
+numpy = ">=1.25.2"
+xarray = ">=2023.7.0"
+rasterio = ">=1.3.10"
+scikit-image = ">=0.19.3"
+opencv-python = ">=4.8.0.76"
+pandas = ">=2.0.3"
+kornia = ">=0.7.2"
+torch = ">=2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `satsync-0.0.2/satsync/ecc.py` & `satsync-0.0.3/satsync/ecc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lgm.py` & `satsync-0.0.3/satsync/lgm.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/aliked.py` & `satsync-0.0.3/satsync/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/disk.py` & `satsync-0.0.3/satsync/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/dog_hardnet.py` & `satsync-0.0.3/satsync/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/lightglue.py` & `satsync-0.0.3/satsync/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/sift.py` & `satsync-0.0.3/satsync/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/superpoint.py` & `satsync-0.0.3/satsync/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/utils.py` & `satsync-0.0.3/satsync/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/lightglue/viz2d.py` & `satsync-0.0.3/satsync/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/main.py` & `satsync-0.0.3/satsync/main.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/pcc.py` & `satsync-0.0.3/satsync/pcc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/satsync/utils.py` & `satsync-0.0.3/satsync/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.2/setup.py` & `satsync-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 packages = \
 ['satsync', 'satsync.lightglue']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kornia>=0.7.2,<0.8.0',
- 'numpy>=1.26.4,<2.0.0',
- 'opencv-python>=4.9.0.80,<5.0.0.0',
- 'pandas>=2.2.2,<3.0.0',
- 'rasterio>=1.3.10,<2.0.0',
- 'scikit-image>=0.23.2,<0.24.0',
- 'xarray>=2024.3.0,<2025.0.0']
+['kornia>=0.7.2',
+ 'numpy>=1.25.2',
+ 'opencv-python>=4.8.0.76',
+ 'pandas>=2.0.3',
+ 'rasterio>=1.3.10',
+ 'scikit-image>=0.19.3',
+ 'torch>=2.2.0',
+ 'xarray>=2023.7.0']
 
 setup_kwargs = {
     'name': 'satsync',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'A python package to align satellite images.',
     'long_description': '# satsync\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satsync)](https://img.shields.io/github/v/release/csaybar/satsync)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satsync/main.yml?branch=main)](https://github.com/csaybar/satsync/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satsync/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satsync)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satsync)](https://img.shields.io/github/commit-activity/m/csaybar/satsync)\n[![License](https://img.shields.io/github/license/csaybar/satsync)](https://img.shields.io/github/license/csaybar/satsync)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satsync/>\n- **Documentation** <https://csaybar.github.io/satsync/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satsync.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satsync/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satsync/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'fcesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satsync',
```

### Comparing `satsync-0.0.2/PKG-INFO` & `satsync-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: satsync
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to align satellite images.
 Home-page: https://github.com/csaybar/satsync
 Author: Cesar Aybar
 Author-email: fcesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: kornia (>=0.7.2,<0.8.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: rasterio (>=1.3.10,<2.0.0)
-Requires-Dist: scikit-image (>=0.23.2,<0.24.0)
-Requires-Dist: xarray (>=2024.3.0,<2025.0.0)
+Requires-Dist: kornia (>=0.7.2)
+Requires-Dist: numpy (>=1.25.2)
+Requires-Dist: opencv-python (>=4.8.0.76)
+Requires-Dist: pandas (>=2.0.3)
+Requires-Dist: rasterio (>=1.3.10)
+Requires-Dist: scikit-image (>=0.19.3)
+Requires-Dist: torch (>=2.2.0)
+Requires-Dist: xarray (>=2023.7.0)
 Project-URL: Documentation, https://csaybar.github.io/satsync/
 Project-URL: Repository, https://github.com/csaybar/satsync
 Description-Content-Type: text/markdown
 
 # satsync
 
 [![Release](https://img.shields.io/github/v/release/csaybar/satsync)](https://img.shields.io/github/v/release/csaybar/satsync)
```

