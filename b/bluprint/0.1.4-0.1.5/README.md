# Comparing `tmp/bluprint-0.1.4.tar.gz` & `tmp/bluprint-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluprint-0.1.4.tar", last modified: Sun Apr 28 04:38:22 2024, max compression
+gzip compressed data, was "bluprint-0.1.5.tar", last modified: Mon May  6 04:52:13 2024, max compression
```

## Comparing `bluprint-0.1.4.tar` & `bluprint-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/
--rw-r--r--   0 igor      (1000) igor      (1000)     1068 2023-11-24 16:08:59.000000 bluprint-0.1.4/LICENSE
--rw-r--r--   0 igor      (1000) igor      (1000)       28 2023-12-26 11:35:41.000000 bluprint-0.1.4/MANIFEST.in
--rw-r--r--   0 igor      (1000) igor      (1000)     4918 2024-04-28 04:38:22.950477 bluprint-0.1.4/PKG-INFO
--rw-r--r--   0 igor      (1000) igor      (1000)     4564 2024-02-22 16:05:17.000000 bluprint-0.1.4/README.rst
--rw-r--r--   0 igor      (1000) igor      (1000)     3243 2024-04-28 04:02:59.000000 bluprint-0.1.4/pyproject.toml
--rw-r--r--   0 igor      (1000) igor      (1000)       38 2024-04-28 04:38:22.950477 bluprint-0.1.4/setup.cfg
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/
--rw-r--r--   0 igor      (1000) igor      (1000)        0 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/__init__.py
--rw-r--r--   0 igor      (1000) igor      (1000)     1972 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/binary.py
--rw-r--r--   0 igor      (1000) igor      (1000)     7654 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/cli.py
--rw-r--r--   0 igor      (1000) igor      (1000)     1480 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/colors.py
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/create/
--rw-r--r--   0 igor      (1000) igor      (1000)        0 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/create/__init__.py
--rw-r--r--   0 igor      (1000) igor      (1000)      818 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/errors.py
--rw-r--r--   0 igor      (1000) igor      (1000)     3077 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/py_project.py
--rw-r--r--   0 igor      (1000) igor      (1000)      773 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/r_project.py
--rw-r--r--   0 igor      (1000) igor      (1000)      860 2024-01-18 06:34:23.000000 bluprint-0.1.4/src/bluprint/errors.py
--rw-r--r--   0 igor      (1000) igor      (1000)     1812 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/index.py
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/notebook/
--rw-r--r--   0 igor      (1000) igor      (1000)     2242 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/jupyter.py
--rw-r--r--   0 igor      (1000) igor      (1000)      677 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/progress.py
--rw-r--r--   0 igor      (1000) igor      (1000)       57 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/notebook/quarto.py
--rw-r--r--   0 igor      (1000) igor      (1000)     1573 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/rmarkdown.py
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/
--rw-r--r--   0 igor      (1000) igor      (1000)     3190 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/.gitignore
--rw-r--r--   0 igor      (1000) igor      (1000)       17 2024-01-24 05:11:11.000000 bluprint-0.1.4/src/bluprint/template/.pdm-python
--rw-r--r--   0 igor      (1000) igor      (1000)      516 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/README.md
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/conf/
--rw-r--r--   0 igor      (1000) igor      (1000)       22 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/conf/config.yaml
--rw-r--r--   0 igor      (1000) igor      (1000)       28 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/conf/data.yaml
--rw-r--r--   0 igor      (1000) igor      (1000)       43 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/conf/workflows.yaml
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/data/
--rw-r--r--   0 igor      (1000) igor      (1000)       23 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/data/example_data.csv
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint/template/notebooks/
--rw-r--r--   0 igor      (1000) igor      (1000)     1596 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_jupyternb.ipynb
--rw-r--r--   0 igor      (1000) igor      (1000)      515 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_quarto.qmd
--rw-r--r--   0 igor      (1000) igor      (1000)      423 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_rmarkdown.Rmd
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint/template/placeholder_name/
--rw-r--r--   0 igor      (1000) igor      (1000)        0 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name/__init__.py
--rw-r--r--   0 igor      (1000) igor      (1000)       73 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name/example.py
--rw-r--r--   0 igor      (1000) igor      (1000)      195 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name.Rproj
--rw-r--r--   0 igor      (1000) igor      (1000)      350 2024-04-28 04:02:44.000000 bluprint-0.1.4/src/bluprint/template/pyproject.toml
--rw-r--r--   0 igor      (1000) igor      (1000)     1069 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template.py
--rw-r--r--   0 igor      (1000) igor      (1000)     2756 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/workflow.py
-drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint.egg-info/
--rw-r--r--   0 igor      (1000) igor      (1000)     4918 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/PKG-INFO
--rw-r--r--   0 igor      (1000) igor      (1000)     1317 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/SOURCES.txt
--rw-r--r--   0 igor      (1000) igor      (1000)        1 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/dependency_links.txt
--rw-r--r--   0 igor      (1000) igor      (1000)       47 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/entry_points.txt
--rw-r--r--   0 igor      (1000) igor      (1000)       97 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/requires.txt
--rw-r--r--   0 igor      (1000) igor      (1000)        9 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/top_level.txt
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.604600 bluprint-0.1.5/
+-rw-r--r--   0 igor       (501) staff       (20)     1068 2023-12-10 22:02:31.000000 bluprint-0.1.5/LICENSE
+-rw-r--r--   0 igor       (501) staff       (20)       28 2023-12-24 01:45:36.000000 bluprint-0.1.5/MANIFEST.in
+-rw-r--r--   0 igor       (501) staff       (20)     4918 2024-05-06 04:52:13.604253 bluprint-0.1.5/PKG-INFO
+-rw-r--r--   0 igor       (501) staff       (20)     4564 2024-05-06 00:38:43.000000 bluprint-0.1.5/README.rst
+-rw-r--r--   0 igor       (501) staff       (20)     3264 2024-05-06 04:51:44.000000 bluprint-0.1.5/pyproject.toml
+-rw-r--r--   0 igor       (501) staff       (20)       38 2024-05-06 04:52:13.604732 bluprint-0.1.5/setup.cfg
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.588802 bluprint-0.1.5/src/
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.594129 bluprint-0.1.5/src/bluprint/
+-rw-r--r--   0 igor       (501) staff       (20)        0 2023-12-12 09:33:52.000000 bluprint-0.1.5/src/bluprint/__init__.py
+-rw-r--r--   0 igor       (501) staff       (20)     1972 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/binary.py
+-rw-r--r--   0 igor       (501) staff       (20)     8099 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/cli.py
+-rw-r--r--   0 igor       (501) staff       (20)     1480 2023-12-12 09:33:52.000000 bluprint-0.1.5/src/bluprint/colors.py
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.597236 bluprint-0.1.5/src/bluprint/create/
+-rw-r--r--   0 igor       (501) staff       (20)        0 2023-12-12 09:33:52.000000 bluprint-0.1.5/src/bluprint/create/__init__.py
+-rw-r--r--   0 igor       (501) staff       (20)      932 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/create/errors.py
+-rw-r--r--   0 igor       (501) staff       (20)     3565 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/create/py_project.py
+-rw-r--r--   0 igor       (501) staff       (20)      773 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/create/r_project.py
+-rw-r--r--   0 igor       (501) staff       (20)      860 2024-05-06 01:12:36.000000 bluprint-0.1.5/src/bluprint/errors.py
+-rw-r--r--   0 igor       (501) staff       (20)     1812 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/index.py
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.598483 bluprint-0.1.5/src/bluprint/notebook/
+-rw-r--r--   0 igor       (501) staff       (20)     2242 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/notebook/jupyter.py
+-rw-r--r--   0 igor       (501) staff       (20)      677 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/notebook/progress.py
+-rw-r--r--   0 igor       (501) staff       (20)       57 2023-12-12 09:33:52.000000 bluprint-0.1.5/src/bluprint/notebook/quarto.py
+-rw-r--r--   0 igor       (501) staff       (20)     1601 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/notebook/rmarkdown.py
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.600401 bluprint-0.1.5/src/bluprint/template/
+-rw-r--r--   0 igor       (501) staff       (20)     6148 2023-12-18 22:56:35.000000 bluprint-0.1.5/src/bluprint/template/.DS_Store
+-rw-r--r--   0 igor       (501) staff       (20)     3190 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template/.gitignore
+-rw-r--r--   0 igor       (501) staff       (20)       17 2023-12-24 01:45:36.000000 bluprint-0.1.5/src/bluprint/template/.pdm-python
+-rw-r--r--   0 igor       (501) staff       (20)      517 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/template/README.md
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.601517 bluprint-0.1.5/src/bluprint/template/conf/
+-rw-r--r--   0 igor       (501) staff       (20)       22 2023-12-24 01:45:36.000000 bluprint-0.1.5/src/bluprint/template/conf/config.yaml
+-rw-r--r--   0 igor       (501) staff       (20)       28 2023-12-22 11:50:44.000000 bluprint-0.1.5/src/bluprint/template/conf/data.yaml
+-rw-r--r--   0 igor       (501) staff       (20)       43 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template/conf/workflows.yaml
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.601840 bluprint-0.1.5/src/bluprint/template/data/
+-rw-r--r--   0 igor       (501) staff       (20)       23 2023-12-22 11:50:44.000000 bluprint-0.1.5/src/bluprint/template/data/example_data.csv
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.602841 bluprint-0.1.5/src/bluprint/template/notebooks/
+-rw-r--r--   0 igor       (501) staff       (20)     1596 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template/notebooks/example_jupyternb.ipynb
+-rw-r--r--   0 igor       (501) staff       (20)      515 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template/notebooks/example_quarto.qmd
+-rw-r--r--   0 igor       (501) staff       (20)      424 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/template/notebooks/example_rmarkdown.Rmd
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.603326 bluprint-0.1.5/src/bluprint/template/placeholder_name/
+-rw-r--r--   0 igor       (501) staff       (20)        0 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template/placeholder_name/__init__.py
+-rw-r--r--   0 igor       (501) staff       (20)       73 2023-12-24 01:45:36.000000 bluprint-0.1.5/src/bluprint/template/placeholder_name/example.py
+-rw-r--r--   0 igor       (501) staff       (20)      195 2023-12-24 01:45:36.000000 bluprint-0.1.5/src/bluprint/template/placeholder_name.Rproj
+-rw-r--r--   0 igor       (501) staff       (20)      350 2024-05-06 04:51:44.000000 bluprint-0.1.5/src/bluprint/template/pyproject.toml
+-rw-r--r--   0 igor       (501) staff       (20)     1069 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/template.py
+-rw-r--r--   0 igor       (501) staff       (20)     2756 2024-02-06 06:01:22.000000 bluprint-0.1.5/src/bluprint/workflow.py
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-05-06 04:52:13.603682 bluprint-0.1.5/src/bluprint.egg-info/
+-rw-r--r--   0 igor       (501) staff       (20)     4918 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/PKG-INFO
+-rw-r--r--   0 igor       (501) staff       (20)     1349 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/SOURCES.txt
+-rw-r--r--   0 igor       (501) staff       (20)        1 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/dependency_links.txt
+-rw-r--r--   0 igor       (501) staff       (20)       47 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/entry_points.txt
+-rw-r--r--   0 igor       (501) staff       (20)       97 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/requires.txt
+-rw-r--r--   0 igor       (501) staff       (20)        9 2024-05-06 04:52:13.000000 bluprint-0.1.5/src/bluprint.egg-info/top_level.txt
```

### Comparing `bluprint-0.1.4/LICENSE` & `bluprint-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/PKG-INFO` & `bluprint-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluprint
-Version: 0.1.4
+Version: 0.1.5
 Author: igor-sb
 License: MIT
 Requires-Python: ==3.11.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: notebook>=7.0.6
 Requires-Dist: fire>=0.5.0
```

### Comparing `bluprint-0.1.4/README.rst` & `bluprint-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/pyproject.toml` & `bluprint-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bluprint"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = [
 	{name = "igor-sb"},
 ]
 readme = "README.rst"
 license = { text = "MIT" }
 requires-python = "==3.11.*"
@@ -48,19 +48,20 @@
 # Fire library throws this warning
 filterwarnings = [
 	"ignore:.*pipes.* is deprecated and slated for removal:DeprecationWarning",
 ]
 
 [tool.isort]
 profile = "wemake"
-line_length = 79
+line_length = 80
 
 [tool.flake8]
 max-module-members = 8
 max-arguments = 6
+max-line-length = 80
 ignore = [
 	'D101',  # D101 Missing docstring in public class
 	'D102',  # D102 Missing docstring in public method
 	'D103',  # D103 Missing docstring in public function
 	'D104',  # Missing docstring in public package
 	'D107',  # D107 Missing docstring in __init__
 	'D412',  # No blank lines allowed between a section header and its content
```

### Comparing `bluprint-0.1.4/src/bluprint/binary.py` & `bluprint-0.1.5/src/bluprint/binary.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/cli.py` & `bluprint-0.1.5/src/bluprint/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from pathlib import Path
 
 import fire
 from bluprint_conf import load_config_yaml
 
 from bluprint.binary import check_if_executable_is_installed
 from bluprint.colors import styled_print
-from bluprint.create.py_project import create_project, initialize_project
+from bluprint.create.py_project import (
+    check_python_version,
+    create_project,
+    initialize_project,
+)
 from bluprint.create.r_project import (
     check_if_r_package_is_installed,
     initialize_r_project,
 )
 from bluprint.errors import ProjectExistsError
 from bluprint.index import index_dir_to_config_yaml
 from bluprint.workflow import run_notebook, run_workflow
@@ -50,16 +54,17 @@
 
         Args:
 
         project_name (str): Name of the project, also the name of the main
             project directory.
 
         python_version (str | None, optional): Python version to be used. If
-            not specified, uses the latest stable version from
-            `pyenv install -l`.
+            not specified, uses either the latest stable version from
+            `pyenv install -l` or 3.11 (whichever is greater). Bluprint requires
+            Python >= 3.11.
 
         parent_dir (str | None, optional): Parent directory to create a
             PROJECT_NAME directory in. If not specific PARENT_DIR is a current
             directory.
 
         template_dir (str | None, optional): Path to a directory with a
             Bluprint or PDM template. If not specified (default), uses Bluprint
@@ -73,14 +78,15 @@
             'creating Python{with_r} project {project_name}... '.format(
                 project_name=project_name,
                 with_r='/R' if r_proj else '',
             ),
             endline='',
         )
         check_if_project_can_be_created(project_name, parent_dir, r_proj)
+        check_python_version(python_version)
         create_project(project_name, python_version, parent_dir, template_dir)
         if r_proj:
             initialize_r_project(project_name, parent_dir)
         styled_print('Ok', print_bluprint=False)
 
     def init(
         self,
@@ -91,43 +97,47 @@
         r_proj: bool = False,
     ) -> None:
         """Initialize a bluprint project in existing directory.
 
         Args:
 
         project_name (str): Name of the project.
-        python_version (str | None, optional): Python version to be used.
-            If not specified, uses `python --version`.
+
+        python_version (str | None, optional): Python version to be used. If
+            not specified, uses either the latest stable version from
+            `pyenv install -l` or 3.11 (whichever is greater). Bluprint requires
+            Python >= 3.11.
+
         project_dir (str | None, optional): Project directory where to
             initialize a new bluprint project. By default uses current working
             directory.
+
         template_dir (str | None, optional): Path to a directory with a
             Bluprint or PDM template. If not specified (default), uses Bluprint
             default built-in template.
+
         r_proj (bool): Setup R library using renv to support package
             isolation in RMarkdown notebooks.
 
         Raises:
-            ProjectExistsError: Raised if pyproject.toml exists in the
-            `project_dir`.
+
+            ProjectExistsError: Raised if pyproject.toml exists in
+                the `project_dir`.
         """
         if not project_dir:
             project_dir = getcwd()
         styled_print(
             'initializing Python{with_r} project {project_name}... '.format(
                 project_name=project_name,
                 with_r='/R' if r_proj else '',
             ),
             endline='',
         )
-        if (Path(project_dir) / 'pyproject.toml').exists():
-            raise ProjectExistsError(
-                f'pyproject.toml already exists in {project_dir}: '
-                + 'cannot initialize new bluprint project',
-            )
+        check_if_pyproject_toml_exists(project_dir)
+        check_python_version(python_version)
         initialize_project(
             project_name,
             python_version,
             Path(project_dir),
             template_dir,
         )
         if r_proj:
@@ -221,13 +231,21 @@
 def check_if_project_exists(project_name: str, parent_dir: str | None) -> None:
     if not parent_dir:
         parent_dir = '.'
     if (Path(parent_dir) / project_name).is_dir():
         raise ProjectExistsError(f'{project_name} directory exists.')
 
 
+def check_if_pyproject_toml_exists(project_dir: str) -> None:
+    if (Path(project_dir) / 'pyproject.toml').exists():
+        raise ProjectExistsError(
+            f'pyproject.toml already exists in {project_dir}: '
+            + 'cannot initialize new bluprint project',
+        )
+
+
 def main():
     fire.Fire(Bluprint)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `bluprint-0.1.4/src/bluprint/colors.py` & `bluprint-0.1.5/src/bluprint/colors.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/create/errors.py` & `bluprint-0.1.5/src/bluprint/create/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from bluprint.errors import StyledError
 
 
 class PythonVersionError(StyledError):
     """Raises exception if python --version fails."""
 
 
+class LowPythonVersionError(StyledError):
+    """Raises exception if user-provided Python version is < 3.11."""
+
+
 class PdmAddError(StyledError):
     """Raises exception if PDM add fails."""
 
 
 class PdmInitError(StyledError):
     """Raises exception if PDM init fails."""
```

### Comparing `bluprint-0.1.4/src/bluprint/create/py_project.py` & `bluprint-0.1.5/src/bluprint/create/py_project.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """Create a bluprint project."""
 
 import re
 from pathlib import Path
 
 import nbformat
 from importlib_resources import files
+from packaging.version import Version
 
 from bluprint.binary import pdm_add, pdm_init, run
-from bluprint.create.errors import GitError, PythonVersionError
+from bluprint.create.errors import (
+    GitError,
+    LowPythonVersionError,
+    PythonVersionError,
+)
+
+MIN_PYTHON_VERSION = '3.11'
 
 
 def create_project(
     project_name: str,
     python_version: str | None = None,
     parent_dir: str | None = None,
     template_dir: str | None = None,
@@ -86,10 +93,21 @@
             readme_content,
         )
 
     with open(readme_file, 'w') as readme_w:
         readme_w.write(readme_content)
 
 
-def default_python_version() -> str:
+def default_python_version(min_version: str = MIN_PYTHON_VERSION) -> str:
     python_out = run(['python', '--version'], PythonVersionError)
-    return python_out.strip().replace('Python ', '')
+    py_version = python_out.strip().replace('Python ', '')
+    if Version(py_version) >= Version(min_version):
+        return py_version
+    return min_version
+
+
+def check_python_version(
+    python_version: str | None,
+) -> None:
+    if python_version:
+        if Version(python_version) < Version(MIN_PYTHON_VERSION):
+            raise LowPythonVersionError('Bluprint requires Python >= 3.11.')
```

### Comparing `bluprint-0.1.4/src/bluprint/create/r_project.py` & `bluprint-0.1.5/src/bluprint/create/r_project.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/errors.py` & `bluprint-0.1.5/src/bluprint/errors.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/index.py` & `bluprint-0.1.5/src/bluprint/index.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/notebook/jupyter.py` & `bluprint-0.1.5/src/bluprint/notebook/jupyter.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/notebook/progress.py` & `bluprint-0.1.5/src/bluprint/notebook/progress.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/notebook/rmarkdown.py` & `bluprint-0.1.5/src/bluprint/notebook/rmarkdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             ['Rscript', '-e', f'rmarkdown::render("{notebook_file}")'],
             bufsize=1,
             universal_newlines=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         last_percent = 0
+        current_percent = 0
         for line in rmd_out.stdout:  # type: ignore
             if progress_bar_pct.match(line):
                 current_percent = int(progress_bar_pct.sub(r'\1', line))
             elif progress_bar_frac.match(line):
                 current_cell = int(progress_bar_frac.sub(r'\1', line))
                 total_cells = int(progress_bar_frac.sub(r'\2', line))
                 current_percent = 100 * current_cell // total_cells
```

### Comparing `bluprint-0.1.4/src/bluprint/template/.gitignore` & `bluprint-0.1.5/src/bluprint/template/.gitignore`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/template/README.md` & `bluprint-0.1.5/src/bluprint/template/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 ```
 
 ## Running notebooks
 
 Open and run a notebook in your IDE of choice (VSCode, Jupyter, ...). Make sure
 to select the correct kernel, which should point to the `.venv` virtual
 environment inside this directory. In VSCode it will show as `.venv/bin/python`
-and should be marked as "Recommended".
+and should be marked as "Recommended".
```

### Comparing `bluprint-0.1.4/src/bluprint/template/notebooks/example_jupyternb.ipynb` & `bluprint-0.1.5/src/bluprint/template/notebooks/example_jupyternb.ipynb`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/template/notebooks/example_quarto.qmd` & `bluprint-0.1.5/src/bluprint/template/notebooks/example_quarto.qmd`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/template.py` & `bluprint-0.1.5/src/bluprint/template.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint/workflow.py` & `bluprint-0.1.5/src/bluprint/workflow.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.4/src/bluprint.egg-info/PKG-INFO` & `bluprint-0.1.5/src/bluprint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluprint
-Version: 0.1.4
+Version: 0.1.5
 Author: igor-sb
 License: MIT
 Requires-Python: ==3.11.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: notebook>=7.0.6
 Requires-Dist: fire>=0.5.0
```

### Comparing `bluprint-0.1.4/src/bluprint.egg-info/SOURCES.txt` & `bluprint-0.1.5/src/bluprint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/bluprint/create/errors.py
 src/bluprint/create/py_project.py
 src/bluprint/create/r_project.py
 src/bluprint/notebook/jupyter.py
 src/bluprint/notebook/progress.py
 src/bluprint/notebook/quarto.py
 src/bluprint/notebook/rmarkdown.py
+src/bluprint/template/.DS_Store
 src/bluprint/template/.gitignore
 src/bluprint/template/.pdm-python
 src/bluprint/template/README.md
 src/bluprint/template/placeholder_name.Rproj
 src/bluprint/template/pyproject.toml
 src/bluprint/template/conf/config.yaml
 src/bluprint/template/conf/data.yaml
```

