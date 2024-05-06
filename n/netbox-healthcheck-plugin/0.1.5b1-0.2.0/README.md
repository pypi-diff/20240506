# Comparing `tmp/netbox-healthcheck-plugin-0.1.5b1.tar.gz` & `tmp/netbox_healthcheck_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-healthcheck-plugin-0.1.5b1.tar", last modified: Mon Apr  8 18:58:43 2024, max compression
+gzip compressed data, was "netbox_healthcheck_plugin-0.2.0.tar", last modified: Mon May  6 19:39:40 2024, max compression
```

## Comparing `netbox-healthcheck-plugin-0.1.5b1.tar` & `netbox_healthcheck_plugin-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 18:58:43.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/tests/test_netbox_healthcheck_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.774828 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.774828 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-06 19:39:40.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 19:39:40.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:39:40.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 19:39:40.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 19:39:40.000000 netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:39:40.778828 netbox_healthcheck_plugin-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 19:39:37.000000 netbox_healthcheck_plugin-0.2.0/tests/test_netbox_healthcheck_plugin.py
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/CONTRIBUTING.md` & `netbox_healthcheck_plugin-0.2.0/CONTRIBUTING.md`

 * *Files 15% similar despite different names*

```diff
@@ -65,35 +65,36 @@
 1. Fork the `netbox-healthcheck-plugin` repo on GitHub.
 2. Clone your fork locally
 
     ```
     $ git clone git@github.com:your_name_here/netbox-healthcheck-plugin.git
     ```
 
-3. Install dependencies and start your virtualenv:
+3. Activate the NetBox virtual environment (see the NetBox documentation under [Setting up a Development Environment](https://docs.netbox.dev/en/stable/development/getting-started/)):
 
     ```
-    $ poetry install -E test -E doc -E dev
+    $ source ~/.venv/netbox/bin/activate
     ```
 
-4. Create a branch for local development:
+4. Add the plugin to NetBox virtual environment in Develop mode (see [Plugins Development](https://docs.netbox.dev/en/stable/plugins/development/)):
+
+    To ease development, it is recommended to go ahead and install the plugin at this point using setuptools' develop mode. This will create symbolic links within your Python environment to the plugin development directory. Call setup.py from the plugin's root directory with the develop argument (instead of install):
 
     ```
-    $ git checkout -b name-of-your-bugfix-or-feature
+    $ python setup.py develop
     ```
 
-    Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass the
-   tests, including testing other Python versions, with tox:
+5. Create a branch for local development:
 
     ```
-    $ poetry run tox
+    $ git checkout -b name-of-your-bugfix-or-feature
     ```
 
+    Now you can make your changes locally.
+
 6. Commit your changes and push your branch to GitHub:
 
     ```
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
     ```
@@ -104,25 +105,17 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.md.
-3. The pull request should work for Python 3.6, 3.7, 3.8 and 3.9. Check
+3. The pull request should work for Python 3.10, 3.11 and 3.12. Check
    https://github.com/netbox-community/netbox-healthcheck-plugin/actions
    and make sure that the tests pass for all supported Python versions.
 
 
 ## Deploying
 
 A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in CHANGELOG.md).
-Then run:
-
-```
-$ poetry run bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-```
-
-GitHub Actions will then deploy to PyPI if tests pass.
+Make sure all your changes are committed (including an entry in CHANGELOG.md) and that all tests pass.
+Then in the github project go to `Releases` and create a new release with a new tag.  This will automatically upload the release to pypi:
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/LICENSE` & `netbox_healthcheck_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.5b1/PKG-INFO` & `netbox_healthcheck_plugin-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.5b1
+Version: 0.2.0
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django-health-check<4,>=3
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
@@ -45,14 +44,15 @@
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
 |   3.4 - 3.7    |      0.1.3     |
+|   4.0.         |      0.2.0     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/README.md` & `netbox_healthcheck_plugin-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
 |   3.4 - 3.7    |      0.1.3     |
+|   4.0.         |      0.2.0     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/__init__.py` & `netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for NetBox HealthCheck Plugin."""
 
 __author__ = """Arthur Hanson"""
 __email__ = 'ahanson@netboxlabs.com'
-__version__ = '0.1.5b1'
+__version__ = '0.2.0'
 
 
 from netbox.plugins import PluginConfig
 
 
 class HealthCheckConfig(PluginConfig):
     name = 'netbox_healthcheck_plugin'
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/PKG-INFO` & `netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.5b1
+Version: 0.2.0
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django-health-check<4,>=3
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
@@ -45,14 +44,15 @@
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
 |   3.4 - 3.7    |      0.1.3     |
+|   4.0.         |      0.2.0     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/SOURCES.txt` & `netbox_healthcheck_plugin-0.2.0/netbox_healthcheck_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.5b1/pyproject.toml` & `netbox_healthcheck_plugin-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-healthcheck-plugin"
-version = "0.1.5b1"
+version = "0.2.0"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for HealthCheck."
 readme = "README.md"
 
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     "Programming Language :: Python :: 3 :: Only",
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
-requires-python = ">=3.8.1"
+requires-python = ">=3.10.0"
 
 dependencies = [
     'django-health-check >= 3,<4'
 ]
 
 [project.optional-dependencies]
 test = [
@@ -44,11 +43,11 @@
 [project.urls]
 Documentation = "https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md"
 Source = "https://github.com/netbox-community/netbox-healthcheck-plugin"
 Tracker = "https://github.com/netbox-community/netbox-healthcheck-plugin/issues"
 
 [tool.black]
 line-length = 120
-target_version = ['py39', 'py310', 'py311', 'py312']
+target_version = ['py310', 'py311', 'py312']
 
 [tool.setuptools.package-data]
 netbox_healthcheck_plugin = ["templates/**"]
```

