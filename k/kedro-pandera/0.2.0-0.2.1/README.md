# Comparing `tmp/kedro_pandera-0.2.0.tar.gz` & `tmp/kedro_pandera-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_pandera-0.2.0.tar", last modified: Sun Apr 21 19:01:54 2024, max compression
+gzip compressed data, was "kedro_pandera-0.2.1.tar", last modified: Mon May  6 21:15:49 2024, max compression
```

## Comparing `kedro_pandera-0.2.0.tar` & `kedro_pandera-0.2.1.tar`

### file list

```diff
@@ -1,123 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.889532 kedro_pandera-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.889532 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/check-links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/failed_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (127)    33287 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/log_failed_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/imgs/successful_validation_during_kedro_run.png
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/docs/source/01_tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/01_tutorials/01_getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/01_tutorials/02_dataframe_model.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/docs/source/migration_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/config/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/kedro_pandera/framework/hooks/pandera_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.893532 kedro_pandera-0.2.0/kedro_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 19:01:54.000000 kedro_pandera-0.2.0/kedro_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/mlc_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.885532 kedro_pandera-0.2.0/tests/_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/prompts.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.885532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.897532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/cli/test_cli_infer_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:54.901532 kedro_pandera-0.2.0/tests/framework/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-21 19:01:50.000000 kedro_pandera-0.2.0/tests/framework/config/test_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/workflows/check-links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/imgs/failed_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33287 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/imgs/log_failed_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/imgs/successful_validation_during_kedro_run.png
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/docs/source/01_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/source/01_tutorials/01_getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/source/01_tutorials/02_dataframe_model.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/docs/source/migration_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.663370 kedro_pandera-0.2.1/kedro_pandera/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/kedro_pandera/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/kedro_pandera/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/kedro_pandera/framework/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/config/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/kedro_pandera/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/kedro_pandera/framework/hooks/pandera_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/kedro_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 21:15:49.000000 kedro_pandera-0.2.1/kedro_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/mlc_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.659370 kedro_pandera-0.2.1/tests/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/prompts.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.659370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.667370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/data/iris_schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/cli/test_cli_infer_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/framework/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/config/test_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:49.671370 kedro_pandera-0.2.1/tests/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 21:15:45.000000 kedro_pandera-0.2.1/tests/framework/hooks/test_hook.py
```

### Comparing `kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kedro_pandera-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `kedro_pandera-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `kedro_pandera-0.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.github/workflows/prepare-release.yml` & `kedro_pandera-0.2.1/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.github/workflows/publish.yml` & `kedro_pandera-0.2.1/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -49,11 +49,11 @@
       uses: author/action-rollback@stable
       with:
         # Using a known release ID
         release_id: ${{ steps.create_release.outputs.id }}
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
-    - name: Publish package distributions to Test PyPI
+    - name: Publish package distributions to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         verbose: true  # trace if the upload fails
```

### Comparing `kedro_pandera-0.2.0/.github/workflows/test.yml` & `kedro_pandera-0.2.1/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,37 +10,50 @@
     branches: [main]
 
 jobs:
   lint_and_test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.8", "3.10"] # 3.10 is converted to 3.1 if not a string
+        python-version: ["3.8", "3.11"]
         os: [ubuntu-latest, macos-latest, windows-latest]
     env:
       OS: ${{ matrix.os }}
       PYTHON_VERSION: ${{ matrix.python-version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[test]
-    - name: Check code formatting and linting
-      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.8' # linting should occur only once in the loop
+    - name: Check code formatting with ruff
+      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.11' # linting should occur only once in the loop
       run: |
-        make lint
+        ruff format . --check
+    - name: Check import order and syntax with ruff
+      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.11' # linting should occur only once in the loop
+      #"F",  # Pyflakes
+      #"E",  # Pycodestyle
+      # "W",  # Pycodestyle
+      # "UP",  # pyupgrade
+      # "I",  # isort
+      # "PL", # Pylint
+      # PLR0913 lines-too-long managed by "ruff format"
+      run: |
+        ruff check . --select F,E,W,UP,I,PL --ignore E,PLR0913 --exclude "/template/"
+
     - name: Test with pytest and generate coverage report
       run: |
         pytest --cov=./ --cov-report=xml
     - name: Upload coverage report to Codecov
-      uses: codecov/codecov-action@v3
-      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.8' # upload should occur only once in the loop
+      uses: codecov/codecov-action@v4
+      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.11' # upload should occur only once in the loop
       with:
         token: ${{ secrets.CODECOV_TOKEN }}  # token is not mandatory but make access more stable
+        # use_oidc: true would better?
         file: ./coverage.xml
         env_vars: OS,PYTHON
         fail_ci_if_error: true
```

### Comparing `kedro_pandera-0.2.0/.gitignore` & `kedro_pandera-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.gitpod.yml` & `kedro_pandera-0.2.1/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.pre-commit-config.yaml` & `kedro_pandera-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/.readthedocs.yml` & `kedro_pandera-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/CHANGELOG.md` & `kedro_pandera-0.2.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.2.1] - 2024-05-06
+
+-   :bug: Fix dataset reference in hook for kedro >= 0.19.0
+
 ## [0.2.0] - 2024-04-19
 
 ### Changed
 
 -   :boom: :sparkles: :arrow_up: Drop support for `kedro==0.18.x` and add support for `kedro==0.19.x` ([#46](https://github.com/Galileo-Galilei/kedro-pandera/issues/46))
 
 ## [0.1.0] - 2023-09-02
@@ -15,12 +19,14 @@
 -   :sparkles: Add a CLI command to infer the schema of a dataset and persist it to a file ([#4](https://github.com/Galileo-Galilei/kedro-pandera/pull/4))
 -   :sparkles: Automatically register customer resolvers `pa.dict`, `pa.yaml` to make schema declaration easier in the catalog  ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
 -   :sparkles: Automatically register customer resolver `pa.python` to enable schema declaration in the catalog from a `DataframeModel` class ([#32](https://github.com/Galileo-Galilei/kedro-pandera/pull/32))
 -   :sparkles: Add runtime validation : before running each node, data is validated against the schema declared in the catalog ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
 -   :loud_sound: `kedro-pandera` logs defaults is set to `INFO` so it is visible by default in the kedro logs ([#13](https://github.com/Galileo-Galilei/kedro-pandera/pull/13))
 -   :memo: Add a tutorial for using `kedro-pandera` ([#5](https://github.com/Galileo-Galilei/kedro-pandera/pull/5))
 
-[Unreleased]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...HEAD
+[Unreleased]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.1...HEAD
+
+[0.2.1]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...0.2.1
 
 [0.2.0]: https://github.com/Galileo-Galilei/kedro-pandera/compare/0.1.0...0.2.0
 
 [0.1.0]: https://github.com/Galileo-Galilei/kedro-pandera/compare/dcba7c128e5187c1a9b26430cddb274064ac96a4...0.1.0
```

### Comparing `kedro_pandera-0.2.0/CODE_OF_CONDUCT.md` & `kedro_pandera-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/CONTRIBUTING.md` & `kedro_pandera-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/LICENSE` & `kedro_pandera-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/PKG-INFO` & `kedro_pandera-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro_pandera
-Version: 0.2.0
+Version: 0.2.1
 Summary: A kedro plugin to use pandera in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-pandera
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -34,15 +34,15 @@
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.1)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.1...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
```

### Comparing `kedro_pandera-0.2.0/README.md` & `kedro_pandera-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.1)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.1...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
```

### Comparing `kedro_pandera-0.2.0/docs/Makefile` & `kedro_pandera-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/conf.py` & `kedro_pandera-0.2.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # "sphinx.ext.ifconfig",
     # "sphinx_sitemap",
     # "nbsphinx",
     "sphinx_copybutton",
     "sphinx_markdown_tables",
     "myst_parser",
     "sphinxawesome_theme",
-    "sphinxawesome_theme.docsearch",
+    "sphinx_docsearch",  # before: "sphinxawesome_theme.docsearch",
     "sphinxawesome_theme.highlighting",
 ]
 
 # enable autosummary plugin (table of contents for modules/classes/class
 # methods)
 autosummary_generate = True
 autosummary_generate_overwrite = False
```

### Comparing `kedro_pandera-0.2.0/docs/imgs/failed_validation_during_kedro_run.png` & `kedro_pandera-0.2.1/docs/imgs/failed_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/imgs/log_failed_validation_during_kedro_run.png` & `kedro_pandera-0.2.1/docs/imgs/log_failed_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/imgs/successful_validation_during_kedro_run.png` & `kedro_pandera-0.2.1/docs/imgs/successful_validation_during_kedro_run.png`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/make.bat` & `kedro_pandera-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/source/01_tutorials/01_getting_started.md` & `kedro_pandera-0.2.1/docs/source/01_tutorials/01_getting_started.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/docs/source/01_tutorials/02_dataframe_model.md` & `kedro_pandera-0.2.1/docs/source/01_tutorials/02_dataframe_model.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/kedro_pandera/framework/cli/cli.py` & `kedro_pandera-0.2.1/kedro_pandera/framework/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/kedro_pandera/framework/config/resolvers.py` & `kedro_pandera-0.2.1/kedro_pandera/framework/config/resolvers.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/kedro_pandera/framework/hooks/pandera_hook.py` & `kedro_pandera-0.2.1/kedro_pandera/framework/hooks/pandera_hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,21 +47,19 @@
 
     @hook_impl
     def before_node_run(  # noqa : PLR0913
         self, node, catalog, inputs, is_async, session_id
     ):
         for name, data in inputs.items():
             if (
-                catalog._data_sets[name].metadata is not None
-                and "pandera" in catalog._data_sets[name].metadata
+                catalog._datasets[name].metadata is not None
+                and "pandera" in catalog._datasets[name].metadata
             ):
                 try:
-                    catalog._data_sets[name].metadata["pandera"]["schema"].validate(
-                        data
-                    )
+                    catalog._datasets[name].metadata["pandera"]["schema"].validate(data)
                 except SchemaError as err:
                     self._logger.error(
                         f"Dataset '{name}' pandera validation failed before running '{node.name}', see details in the error message. "
                     )
                     raise err
                 except Exception as err:
                     self._logger.error(
```

### Comparing `kedro_pandera-0.2.0/kedro_pandera.egg-info/PKG-INFO` & `kedro_pandera-0.2.1/kedro_pandera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-pandera
-Version: 0.2.0
+Version: 0.2.1
 Summary: A kedro plugin to use pandera in your kedro projects
 Home-page: https://github.com/Galileo-Galilei/kedro-pandera
 Author: Yolan Honoré-Rougé
 License: Apache Software License (Apache 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -34,15 +34,15 @@
 | Pypi                | [![PyPI version](https://badge.fury.io/py/kedro-pandera.svg)](https://pypi.org/project/kedro-pandera/) | [![Downloads](https://pepy.tech/badge/kedro-pandera)](https://pepy.tech/project/kedro-pandera) |
 
 **Code health**
 
 ----------------------------------------------------------
 | Branch                                | Tests                                                                                                                                                                                                                                    | Coverage                                                                                                                                                                                                                                                                                               | Links                                                                                                                                                                                                                                                                                                                                                 | Documentation                                                                                                                                                                 | Deployment                                                                                                                                                                                                                                                                                                                                      | Activity                                                                                                                                                                                                                                                                     |
 | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.0)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.0...main) |
+| `main` | [![test](https://github.com/Galileo-Galilei/kedro-pandera/workflows/test/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Atest+branch%3Amain) | [![codecov](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main/graph/badge.svg)](https://codecov.io/gh/Galileo-Galilei/kedro-pandera/branch/main) | [![links](https://github.com/Galileo-Galilei/kedro-pandera/workflows/check-links/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=workflow%3Acheck-links+branch%3Amain) | [![Documentation](https://readthedocs.org/projects/kedro-pandera/badge/?version=stable)](https://kedro-pandera.readthedocs.io/en/stable/) | [![publish](https://github.com/Galileo-Galilei/kedro-pandera/workflows/publish/badge.svg?branch=main)](https://github.com/Galileo-Galilei/kedro-pandera/actions?query=branch%3Amain+workflow%3Apublish) | [![commit](https://img.shields.io/github/commits-since/Galileo-Galilei/kedro-pandera/0.2.1)](https://github.com/Galileo-Galilei/kedro-pandera/compare/0.2.1...main) |
 
 # What is kedro-pandera?
 
 
 # How do I install kedro-pandera?
```

### Comparing `kedro_pandera-0.2.0/kedro_pandera.egg-info/SOURCES.txt` & `kedro_pandera-0.2.1/kedro_pandera.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -75,13 +75,17 @@
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
 tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+tests/data/iris.csv
+tests/data/iris_schema.yml
 tests/framework/__init__.py
 tests/framework/cli/__init__.py
 tests/framework/cli/test_cli.py
 tests/framework/cli/test_cli_infer_schema.py
 tests/framework/config/__init__.py
-tests/framework/config/test_resolvers.py
+tests/framework/config/test_resolvers.py
+tests/framework/hooks/__init__.py
+tests/framework/hooks/test_hook.py
```

### Comparing `kedro_pandera-0.2.0/setup.py` & `kedro_pandera-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,31 +21,32 @@
 # Get the long description from the README file
 with open((HERE / "README.md").as_posix(), encoding="utf-8") as file_handler:
     README = file_handler.read()
 
 
 setup(
     name=NAME,
-    version="0.2.0",  # this will be bumped automatically by bump2version
+    version="0.2.1",  # this will be bumped automatically by bump2version
     description="A kedro plugin to use pandera in your kedro projects",
     license="Apache Software License (Apache 2.0)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Galileo-Galilei/kedro-pandera",
     python_requires=">=3.8, <3.12",
     packages=find_packages(exclude=["docs*", "tests*"]),
     setup_requires=["setuptools_scm"],
     include_package_data=True,
     install_requires=base_requirements,
     extras_require={
         "doc": [
-            "sphinx>=4.5.0,<7.2.0",  # https://github.com/kai687/sphinxawesome-theme/issues/1464
+            "sphinx>=4.5.0,<7.3.0",  # https://github.com/kai687/sphinxawesome-theme/issues/1464
             "sphinxawesome-theme",
+            "sphinx-docsearch",
             "sphinx-markdown-tables~=0.0.15",
-            "sphinx-click>=3.1,<4.5",
+            "sphinx-click>=3.1,<6.0",
             "sphinx_copybutton~=0.5.0",
             # "sphinx-sitemap",
             "sphinx-design",
             "myst-parser>=0.17.2,<2.1.0",
         ],
         "test": [
             "ruff>=0.4.0, <0.5.0",
```

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/catalog.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/data/01_raw/iris.csv`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro_pandera-0.2.1/tests/_data/pandas-iris/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/conftest.py` & `kedro_pandera-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/framework/cli/test_cli.py` & `kedro_pandera-0.2.1/tests/framework/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/framework/cli/test_cli_infer_schema.py` & `kedro_pandera-0.2.1/tests/framework/cli/test_cli_infer_schema.py`

 * *Files identical despite different names*

### Comparing `kedro_pandera-0.2.0/tests/framework/config/test_resolvers.py` & `kedro_pandera-0.2.1/tests/framework/config/test_resolvers.py`

 * *Files identical despite different names*

