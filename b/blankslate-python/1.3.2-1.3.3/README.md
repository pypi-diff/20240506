# Comparing `tmp/blankslate_python-1.3.2.tar.gz` & `tmp/blankslate_python-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.3.2.tar", max compression
+gzip compressed data, was "blankslate_python-1.3.3.tar", max compression
```

## Comparing `blankslate_python-1.3.2.tar` & `blankslate_python-1.3.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.3.2/LICENSE
--rw-r--r--   0        0        0     2866 2024-05-05 17:15:28.213424 blankslate_python-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2292 2024-05-05 16:49:57.766569 blankslate_python-1.3.2/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.3.2/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.2/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.3.2/source/blankslate/config/constants.py
--rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.3.2/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.2/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.3.2/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7458 2024-05-05 16:50:23.878225 blankslate_python-1.3.2/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.3.2/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.3.2/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0        0 2024-05-05 16:50:31.130211 blankslate_python-1.3.2/source/blankslate/generation/templates/.nojekyll.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.3.2/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.3.2/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.3.2/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.3.2/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.3.2/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.3.2/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.3.2/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.3.2/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.3.2/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.3.2/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.3.2/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.3.2/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.3.2/source/blankslate/generation/templates/make.bat.j2
--rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.3.2/source/blankslate/generation/templates/Makefile.j2
--rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.3.2/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.3.2/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2913 2024-05-05 17:14:45.200718 blankslate_python-1.3.2/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1016 2024-05-05 14:35:17.971966 blankslate_python-1.3.2/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.3.2/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.3.2/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       13 2024-05-05 14:38:29.079891 blankslate_python-1.3.2/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.3.2/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      448 2024-05-05 16:17:52.211617 blankslate_python-1.3.2/source/blankslate/generation/templates/test_main.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.3.2/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.3.2/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.3.2/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.2/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.3.2/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.2/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.3.2/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.3.2/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.3.2/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-05 17:15:30.408695 blankslate_python-1.3.2/source/blankslate/VERSION
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2866 2024-05-06 12:58:05.559973 blankslate_python-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2292 2024-05-05 16:49:57.766569 blankslate_python-1.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.3.3/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.3/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.3.3/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0     1370 2024-05-04 22:07:28.201885 blankslate_python-1.3.3/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.3/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-04 21:50:23.783020 blankslate_python-1.3.3/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7496 2024-05-06 12:45:12.741783 blankslate_python-1.3.3/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1927 2024-05-05 12:20:11.191034 blankslate_python-1.3.3/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.3.3/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0        0 2024-05-05 16:50:31.130211 blankslate_python-1.3.3/source/blankslate/generation/templates/.nojekyll.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.3.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.3.3/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.3.3/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.3.3/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.3.3/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.3.3/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3393 2024-05-05 13:27:07.390679 blankslate_python-1.3.3/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.3.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.3.3/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.3.3/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.3.3/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      538 2024-05-04 22:16:16.909317 blankslate_python-1.3.3/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      804 2024-05-05 13:29:20.897846 blankslate_python-1.3.3/source/blankslate/generation/templates/make.bat.j2
+-rw-r--r--   0        0        0      658 2024-05-05 13:29:36.112070 blankslate_python-1.3.3/source/blankslate/generation/templates/Makefile.j2
+-rw-r--r--   0        0        0     1450 2024-05-04 22:08:31.773848 blankslate_python-1.3.3/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.3.3/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2913 2024-05-05 17:14:45.200718 blankslate_python-1.3.3/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1016 2024-05-05 14:35:17.971966 blankslate_python-1.3.3/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.3.3/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.3.3/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       13 2024-05-05 14:38:29.079891 blankslate_python-1.3.3/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.3.3/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      448 2024-05-05 16:17:52.211617 blankslate_python-1.3.3/source/blankslate/generation/templates/test_main.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.3.3/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2810 2024-05-05 13:26:45.432480 blankslate_python-1.3.3/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.3.3/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.3/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3786 2024-05-06 12:47:52.524798 blankslate_python-1.3.3/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.3.3/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.3.3/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      790 2024-05-06 12:55:56.003162 blankslate_python-1.3.3/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.3.3/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-06 12:58:09.100284 blankslate_python-1.3.3/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 blankslate_python-1.3.3/PKG-INFO
```

### Comparing `blankslate_python-1.3.2/LICENSE` & `blankslate_python-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/pyproject.toml` & `blankslate_python-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.3.2"
+version = "1.3.3"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
```

### Comparing `blankslate_python-1.3.2/README.md` & `blankslate_python-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/config/constants.py` & `blankslate_python-1.3.3/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/config/paths.py` & `blankslate_python-1.3.3/source/blankslate/config/paths.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.3.3/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/project_generation.py` & `blankslate_python-1.3.3/source/blankslate/generation/project_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
                     "__init__.py": None,
                     "command_line.py": None,
                 },
                 "logs": {
                     "__init__.py": None,
                     "setup_logging.py": None,
                 },
+                "__init__.py": None,
                 "main.py": None,
                 "py.typed": None,
                 "VERSION": None,
             },
         },
         "tests": {"__init__.py": None, "test_main.py": None},
         ".gitignore": None,
```

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.3.3/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/make.bat.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/make.bat.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/Makefile.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/Makefile.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.3.3/source/blankslate/generation/templates/tox.ini.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/interface/command_line.py` & `blankslate_python-1.3.3/source/blankslate/interface/command_line.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     """
     detail_spaced = detail.replace("_", " ", 1)
     detail_lower = detail_spaced.lower()
     detail_bracketed = detail_lower.replace("_", " (", 1)
     detail_formatted = (
         detail_spaced if detail_spaced == detail_bracketed else detail_bracketed + ")"
     )
+    detail_formatted = detail_formatted.replace("-", "_")  # TODO: Improve handling of hyphens
 
     return detail_formatted
 
 
 def input_project_details() -> dict[str, str]:
     """
     Input project details.
```

### Comparing `blankslate_python-1.3.2/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.3.3/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.3.2/source/blankslate/main.py` & `blankslate_python-1.3.3/source/blankslate/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Notes
     -----
     This function is the entry point for the application.
     """
     try:
         main_logger.info("Application started.")
         project_details = input_project_details()
-        generate_project(project_details)
+        generate_project(project_details)  # TODO: add auto GitHub repo publish
     except KeyboardInterrupt:
         print("\n")
         main_logger.info("Exiting application due to user interrupt...")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `blankslate_python-1.3.2/PKG-INFO` & `blankslate_python-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.3.2
+Version: 1.3.3
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

