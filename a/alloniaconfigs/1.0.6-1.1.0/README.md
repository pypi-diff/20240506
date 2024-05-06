# Comparing `tmp/alloniaconfigs-1.0.6.tar.gz` & `tmp/alloniaconfigs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alloniaconfigs-1.0.6.tar", max compression
+gzip compressed data, was "alloniaconfigs-1.1.0.tar", max compression
```

## Comparing `alloniaconfigs-1.0.6.tar` & `alloniaconfigs-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1480 2024-04-17 08:55:10.686691 alloniaconfigs-1.0.6/README.md
--rw-r--r--   0        0        0       52 2024-04-17 08:55:10.686691 alloniaconfigs-1.0.6/alloniaconfigs/__init__.py
--rw-r--r--   0        0        0     3514 2024-04-17 08:55:10.686691 alloniaconfigs-1.0.6/alloniaconfigs/configs.py
--rw-r--r--   0        0        0     3415 2024-04-17 08:56:13.119226 alloniaconfigs-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 alloniaconfigs-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2047 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/README.md
+-rw-r--r--   0        0        0       52 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/alloniaconfigs/__init__.py
+-rw-r--r--   0        0        0     3514 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/alloniaconfigs/configs.py
+-rw-r--r--   0        0        0     3441 2024-05-06 12:33:16.468552 alloniaconfigs-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 alloniaconfigs-1.1.0/PKG-INFO
```

### Comparing `alloniaconfigs-1.0.6/README.md` & `alloniaconfigs-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,79 @@
 # Public Project AllOnIAConfigs
 
 This project contains the :obj:`~alloniaconfigs.configs.Configs` class that allows the user to
 easily handle configurations.
 
-You can find the user documentation [here](https://aleia-team.gitlab.io/public/alloniaconfigs)
+You can find the user documentation [this URL](https://aleia-team.gitlab.io/public/alloniaconfigs)
 
 This is a public project. Everyone is welcome to contribute to it.
 
 ## Installation
 
 ```bash
 pip install alloniaconfigs
 ````
 
-## Develope this project locally:
+## Contributing
+
+This is an open-source project. Everyone is welcome to contribute to it. To do
+so, fork the repository, add your features/fixes on your forked repository,
+then open a merge request to the original repository.
+
+### Install dependencies using poetry
 
 This project uses [Poetry](https://python-poetry.org/) to manage its
 working environment. Install it before coding in project.
 
-### Install dependencies using poetry:
+Then, run 
 
-```bash
-./init.sh
+ ```bash 
+poetry env use python3.12
+poetry install
+poetry run pre-commit install
 ```
 
-### Testing:
+### Testing
 
 ```bash
 poetry run pytest tests # Parallelized
 poetry run pytest tests -n 0 # Sequential
 
 # Sequential with logs (logs can't work with parallelized tests)
 poetry run pytest tests -n 0 -s # -s is the equivalent of --capture=no
 ```
 
-### Lint:
+#### Coverage
+
+We use `pytest-cov` to display the coverage, so, after run
+tests you can check the reports (term, html, xml are enabled), if you want to
+improve your coverage, the better thing to do is to check the html report in
+your browser:
+
+```bash
+open htmlcov/index.html
+```
+
+### Lint
 
 To run the linters used by this project, you can run:
 ```bash
 poetry run pre-commit run # Run lint only on staged files
 
 # Manually check conventional commits format:
 poetry run pre-commit run gitlint --hook-stage commit-msg --commit-msg-filename .git/COMMIT_EDITMSG
 ```
 
-### User documentation:
+### User documentation
 
-The documentation source files are located in _docs/source/_. If you add
-new features, please add them to the documentation.
+The documentation source files are located in [here](docs/source/). If you add
+new features, please add them to the documentation as well.
 
 You can buid the documentation locally by doing
 
 ```bash
 cd docs
 make html
 ```
 
 The produced documentation should then be readable by opening the file in
-docs/build/index.html in a web browser.
+docs/build/html/index.html in a web browser.
```

### Comparing `alloniaconfigs-1.0.6/alloniaconfigs/configs.py` & `alloniaconfigs-1.1.0/alloniaconfigs/configs.py`

 * *Files identical despite different names*

### Comparing `alloniaconfigs-1.0.6/pyproject.toml` & `alloniaconfigs-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "alloniaconfigs"
-version = "1.0.6"
+version = "1.1.0"
 description = "Class to handle configurations"
 authors = ["ALEIA"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 pydantic = "^2.7.0"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.1.0"
@@ -22,21 +22,22 @@
 sphinxcontrib-mermaid = "^0.9.2"
 sphinx_mdinclude = "0.5.3"
 sphinx_copybutton = "0.5.2"
 pydata_sphinx_theme = "0.15.2"
 pre-commit = "^3.3.3"
 ruff = "0.3.4"
 bandit = "1.7.8"
+eval_type_backport = "0.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-pythonpath = "src"
+pythonpath = "."
 cache_dir = ".cache/pytest_cache"
 testpaths = ['tests']
 addopts = [
     "--cov=alloniaconfigs",
     "--cov-report=term",
     "--cov-report=html",
     "--cov-report=xml",
```

### Comparing `alloniaconfigs-1.0.6/PKG-INFO` & `alloniaconfigs-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,95 @@
 Metadata-Version: 2.1
 Name: alloniaconfigs
-Version: 1.0.6
+Version: 1.1.0
 Summary: Class to handle configurations
 Author: ALEIA
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Public Project AllOnIAConfigs
 
 This project contains the :obj:`~alloniaconfigs.configs.Configs` class that allows the user to
 easily handle configurations.
 
-You can find the user documentation [here](https://aleia-team.gitlab.io/public/alloniaconfigs)
+You can find the user documentation [this URL](https://aleia-team.gitlab.io/public/alloniaconfigs)
 
 This is a public project. Everyone is welcome to contribute to it.
 
 ## Installation
 
 ```bash
 pip install alloniaconfigs
 ````
 
-## Develope this project locally:
+## Contributing
+
+This is an open-source project. Everyone is welcome to contribute to it. To do
+so, fork the repository, add your features/fixes on your forked repository,
+then open a merge request to the original repository.
+
+### Install dependencies using poetry
 
 This project uses [Poetry](https://python-poetry.org/) to manage its
 working environment. Install it before coding in project.
 
-### Install dependencies using poetry:
+Then, run 
 
-```bash
-./init.sh
+ ```bash 
+poetry env use python3.12
+poetry install
+poetry run pre-commit install
 ```
 
-### Testing:
+### Testing
 
 ```bash
 poetry run pytest tests # Parallelized
 poetry run pytest tests -n 0 # Sequential
 
 # Sequential with logs (logs can't work with parallelized tests)
 poetry run pytest tests -n 0 -s # -s is the equivalent of --capture=no
 ```
 
-### Lint:
+#### Coverage
+
+We use `pytest-cov` to display the coverage, so, after run
+tests you can check the reports (term, html, xml are enabled), if you want to
+improve your coverage, the better thing to do is to check the html report in
+your browser:
+
+```bash
+open htmlcov/index.html
+```
+
+### Lint
 
 To run the linters used by this project, you can run:
 ```bash
 poetry run pre-commit run # Run lint only on staged files
 
 # Manually check conventional commits format:
 poetry run pre-commit run gitlint --hook-stage commit-msg --commit-msg-filename .git/COMMIT_EDITMSG
 ```
 
-### User documentation:
+### User documentation
 
-The documentation source files are located in _docs/source/_. If you add
-new features, please add them to the documentation.
+The documentation source files are located in [here](docs/source/). If you add
+new features, please add them to the documentation as well.
 
 You can buid the documentation locally by doing
 
 ```bash
 cd docs
 make html
 ```
 
 The produced documentation should then be readable by opening the file in
-docs/build/index.html in a web browser.
+docs/build/html/index.html in a web browser.
```

