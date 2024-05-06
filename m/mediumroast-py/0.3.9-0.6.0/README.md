# Comparing `tmp/mediumroast_py-0.3.9.tar.gz` & `tmp/mediumroast_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediumroast_py-0.3.9.tar", max compression
+gzip compressed data, was "mediumroast_py-0.6.0.tar", max compression
```

## Comparing `mediumroast_py-0.3.9.tar` & `mediumroast_py-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/LICENSE
--rw-r--r--   0        0        0     2993 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/README.md
--rw-r--r--   0        0        0      624 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/.mediumroast/config.ini
--rw-r--r--   0        0        0     4349 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/example_data/companies.json
--rw-r--r--   0        0        0     1006 2022-08-19 01:03:11.632587 mediumroast_py-0.3.9/examples/example_data/interactions.json
--rw-r--r--   0        0        0     3576 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/example_data/studies.json
--rw-r--r--   0        0        0      317 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/example_data/users.json
--rwxr-xr-x   0        0        0     1215 2022-08-19 00:58:59.446883 mediumroast_py-0.3.9/examples/interaction.py
--rw-r--r--   0        0        0       19 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/rewrite_rules/README.md
--rw-r--r--   0        0        0    13104 2022-07-31 02:39:32.788886 mediumroast_py-0.3.9/examples/rewrite_rules/company.ini
--rw-r--r--   0        0        0     6815 2022-07-31 02:45:13.103211 mediumroast_py-0.3.9/examples/rewrite_rules/interaction.ini
--rw-r--r--   0        0        0    31100 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/examples/rewrite_rules/study.ini
--rwxr-xr-x   0        0        0        0 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/__init__.py
--rwxr-xr-x   0        0        0        0 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/api/__init__.py
--rw-r--r--   0        0        0     2933 2022-08-18 23:47:25.617957 mediumroast_py-0.3.9/mediumroast_py/api/mr_server.py
--rw-r--r--   0        0        0     4473 2022-08-18 23:49:39.290868 mediumroast_py-0.3.9/mediumroast_py/api/scaffold.py
--rwxr-xr-x   0        0        0        0 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/extractors/__init__.py
--rw-r--r--   0        0        0     3709 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/extractors/file.py
--rw-r--r--   0        0        0     1669 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/extractors/filesystem.py
--rw-r--r--   0        0        0     6786 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/extractors/folder.py
--rw-r--r--   0        0        0     2815 2022-07-31 02:39:32.792886 mediumroast_py-0.3.9/mediumroast_py/extractors/s3bucket.py
--rw-r--r--   0        0        0    15040 2022-07-31 02:44:25.506884 mediumroast_py-0.3.9/mediumroast_py/helpers.py
--rwxr-xr-x   0        0        0        0 2022-07-31 02:39:32.796886 mediumroast_py-0.3.9/mediumroast_py/transformers/__init__.py
--rw-r--r--   0        0        0     9834 2022-08-18 23:54:09.332687 mediumroast_py-0.3.9/mediumroast_py/transformers/company.py
--rw-r--r--   0        0        0    19083 2022-07-31 02:39:32.796886 mediumroast_py-0.3.9/mediumroast_py/transformers/helpers.py
--rw-r--r--   0        0        0    10588 2022-08-19 04:11:21.117378 mediumroast_py-0.3.9/mediumroast_py/transformers/interaction.py
--rw-r--r--   0        0        0     7503 2022-08-19 00:44:00.788620 mediumroast_py-0.3.9/mediumroast_py/transformers/study.py
--rw-r--r--   0        0        0      969 2022-08-19 15:19:39.306933 mediumroast_py-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     4080 2022-08-19 15:19:53.475352 mediumroast_py-0.3.9/setup.py
--rw-r--r--   0        0        0     4257 2022-08-19 15:19:53.475653 mediumroast_py-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-26 03:31:36.080868 mediumroast_py-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2458 2024-05-05 21:42:42.608247 mediumroast_py-0.6.0/README.md
+-rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083900 mediumroast_py-0.6.0/mediumroast_py/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083981 mediumroast_py-0.6.0/mediumroast_py/api/__init__.py
+-rw-r--r--   0        0        0     6987 2024-05-05 17:08:08.184732 mediumroast_py-0.6.0/mediumroast_py/api/authorize.py
+-rw-r--r--   0        0        0    27467 2024-05-05 15:48:58.458760 mediumroast_py-0.6.0/mediumroast_py/api/github.py
+-rw-r--r--   0        0        0    21789 2024-05-05 20:34:39.399858 mediumroast_py-0.6.0/mediumroast_py/api/github_server.py
+-rw-r--r--   0        0        0      956 2024-05-05 21:43:48.423938 mediumroast_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 mediumroast_py-0.6.0/setup.py
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mediumroast_py-0.6.0/PKG-INFO
```

### Comparing `mediumroast_py-0.3.9/LICENSE` & `mediumroast_py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediumroast_py-0.3.9/pyproject.toml` & `mediumroast_py-0.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "mediumroast_py"
-version = "0.3.9"
-description = "A package to perform ETL (Extract, Transform and Load) and  interact with the mediumroast.io application."
+version = "0.6.0"
+description = "This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of."
 authors = ["Michael Hay <michael.hay@mediumroast.io>"]
 license = "Apache-2.0"
 repository = "https://github.com/mediumroast/mediumroast_py"
 readme = "README.md"
 keywords = ["Product Management", "Competitive Insights", "Customer Insights", "Partner Insights", "Empowered Teams"]
-include = ["examples/interaction.py", "examples/*/*", "examples/.*/*"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
-pyfiglet = "^0.8.post1"
-spacy = "^3.3.1"
-boto3 = "^1.24.24"
-python-magic = "^0.4.27"
-pdfx = "^1.4.1"
-PyDocX = "^0.9.10"
-python-pptx = "^0.6.21"
-geopy = "^2.2.0"
+pyjwt = "^2.8.0"
+cryptography = "^42.0.6"
+pygithub = "^2.3.0"
+python-dotenv = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.scripts]
+test = "run_tests:main"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mediumroast/mediumroast_py/issues"
```

### Comparing `mediumroast_py-0.3.9/setup.py` & `mediumroast_py-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mediumroast-py
+Version: 0.6.0
+Summary: This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of.
+Home-page: https://github.com/mediumroast/mediumroast_py
+License: Apache-2.0
+Keywords: Product Management,Competitive Insights,Customer Insights,Partner Insights,Empowered Teams
+Author: Michael Hay
+Author-email: michael.hay@mediumroast.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=42.0.6,<43.0.0)
+Requires-Dist: pygithub (>=2.3.0,<3.0.0)
+Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/mediumroast/mediumroast_py/issues
+Project-URL: Repository, https://github.com/mediumroast/mediumroast_py
+Description-Content-Type: text/markdown
+
+# mediumroast_py
+
+## Introduction
+
+This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of.
+
+### Notice
+The SDK is in active development and is subject to change. The SDK is not yet stable and should not be used in production environments. 
+
+## Installation
+
+To install the package, you can use pip:
+
+```bash
+pip install mediumroast_py
+```
+
+## Usage
+To use the package, you will need to import the `mediumroast_py` modules and classes. The package provides three main classes for interacting with objects: `Companies`, `Interactions`, and `Users`.
+
+### Authentication
+To use the package, you will need to authenticate with the Mediumroast API using the `GitHubAuth` class. Here is an example of how to authenticate with the Mediumroast API using a GitHub App installation and a private key file. You will need to set the `MR_CLIENT_ID`, `MR_APP_ID`, and `YOUR_INSTALLATION_ID` environment variables to the appropriate values for your GitHub App installation. You will also need to set the `YOUR_PEM_FILE` environment variable to the path of your private key file. Here is an example of how to authenticate with the Mediumroast API using a GitHub App installation and a private key file.
+
+```python
+from mediumroast_py.api import Companies, Interactions, Users
+from mediumroast_py.api.authorize import GitHubAuth
+
+auth = GitHubAuth(env={'clientId': os.getenv('MR_CLIENT_ID')})
+token = auth.get_access_token_pem(
+      os.getenv('YOUR_PEM_FILE'), 
+      os.getenv('MR_APP_ID'), 
+      os.getenv('YOUR_INSTALLATION_ID')
+)
+```
+
+### Companies
+The `Companies` class provides methods for interacting with companies in Mediumroast. You can use the `get_all` method to get information about all companies.
+
+```python
+company_ctl = Companies(token_info['token'], os.getenv('YOUR_ORG') , process_name)
+companies = company_ctl.get_all()
+```
+
+### Interactions
+The `Interactions` class provides methods for interacting with interactions in Mediumroast. You can use the `get_all` method to get information about all interactions.
+
+```python
+interaction_ctl = Interactions(token_info['token'], os.getenv('YOUR_ORG') , process_name)
+interactions = interaction_ctl.get_all()
+```
 
-packages = \
-['mediumroast_py',
- 'mediumroast_py.api',
- 'mediumroast_py.extractors',
- 'mediumroast_py.transformers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyDocX>=0.9.10,<0.10.0',
- 'boto3>=1.24.24,<2.0.0',
- 'geopy>=2.2.0,<3.0.0',
- 'pdfx>=1.4.1,<2.0.0',
- 'pyfiglet>=0.8.post1,<0.9',
- 'python-magic>=0.4.27,<0.5.0',
- 'python-pptx>=0.6.21,<0.7.0',
- 'requests>=2.28.1,<3.0.0',
- 'spacy>=3.3.1,<4.0.0']
-
-setup_kwargs = {
-    'name': 'mediumroast-py',
-    'version': '0.3.9',
-    'description': 'A package to perform ETL (Extract, Transform and Load) and  interact with the mediumroast.io application.',
-    'long_description': "# Introduction\nThis is the Python Software Development Kit (SDK) for the mediumroast.io.  Internal tooling from Mediumroast, Inc. uses this SDK, so it will always be a first class citizen. Specifically, we build tools requiring ETL (Extract, Transform and Load), Machine Learning and Natural Language Processing (NLP) with this SDK. As appropriate examples illustrating various capabilities of the SDK can be found in the `examples/` directory of this package.  \n\n# Installation and Configuration Steps for Developers\nThe following steps are important if you are developing or extending the Python SDK.  If you're not a developer these steps aren't as important to you and you should pay attention to section entitled *Installation for Early Adopters and Testers*.\n\n## Cloning the repository for Developers\nAssuming `git` is installed and your credentials are set up to talk to the mediumroast.io set of repositories it should be possible to do the following as a user on the system:\n1. `mkdir ~/dev;cd ~/dev`\n2. `git clone git@github.com:mediumroast/mediumroast_py.git`\nThis will create an `mediumroast_py` directory in `~/dev/` and allow you to proceed to the following steps for installation.\n\n## Installation\nFor developers of the package the `setup.py` file is available to enable a local software distribution that can be improved upon.  As inspired by [this article](https://python-packaging-tutorial.readthedocs.io/en/latest/setup_py.html) the best current way to perform the installation of a developer version after cloning is to assuming you've cloned into `~/dev`:\n1. `cd ~/dev/mr_sdk/python`\n2. `sudo pip install -e ./`\nWith this accomplished tools that you've written which depend upon this package should operate.  If there are issues encountered then please open an [issue](https://github.com/mediumroast/mr_python/issues).\n\n## Structure of the repository\nThe following structure is available for the Python SDK, as new SDK implementations are created additional top level directories will be created.\n```\nmr_python/\n      examples/\n      mediumroast_py/\n            api/\n            extractors/\n            transformers/\n            helpers.py\n      project.toml\n      README.md\n      LICENSE\n```\n\n# The Examples\nTo illustrate how to interact programmatically with the mediumroast.io application several examples have been created to make it easier for developers to interact with the system.  The scope of the examples, over time, will include all aspects of the SDK to speed up 3rd party development processes.  This means that over time examples for all apsects of the SDK will be produced and made available under the Apache Software License.  As with anything in the SDK if you run into problems please make sure that you raise an [issue](https://github.com/mediumroast/mediumroast_py/issues) in the repository.  More detail on the examples can be found within the [examples directory](https://github.com/mediumroast/mediumroast_py/tree/main/examples) of this repository.",
-    'author': 'Michael Hay',
-    'author_email': 'michael.hay@mediumroast.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mediumroast/mediumroast_py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Issues
+If you encounter any issues with the SDK, please report them on the [mediumroast_py issues](https://github.com/mediumroast/mediumroast_py/issues) page.
 
-
-setup(**setup_kwargs)
```

