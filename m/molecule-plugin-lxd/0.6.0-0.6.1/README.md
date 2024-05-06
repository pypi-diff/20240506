# Comparing `tmp/molecule-plugin-lxd-0.6.0.tar.gz` & `tmp/molecule_plugin_lxd-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-plugin-lxd-0.6.0.tar", last modified: Fri Sep 15 08:43:32 2023, max compression
+gzip compressed data, was "molecule_plugin_lxd-0.6.1.tar", last modified: Mon May  6 08:58:46 2024, max compression
```

## Comparing `molecule-plugin-lxd-0.6.0.tar` & `molecule_plugin_lxd-0.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.397151 molecule-plugin-lxd-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.ansible-lint-ignore
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.389151 molecule-plugin-lxd-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-09-15 08:43:32.397151 molecule-plugin-lxd-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.389151 molecule-plugin-lxd-0.6.0/doc/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/doc/ec2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/doc/ec2/platforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.389151 molecule-plugin-lxd-0.6.0/doc/vagrant/
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/doc/vagrant/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.389151 molecule-plugin-lxd-0.6.0/molecule/test-podman/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/molecule/test-podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/molecule/test-podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/molecule/test-podman/verify.yml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 08:43:32.397151 molecule-plugin-lxd-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.389151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-15 08:43:32.000000 molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.385151 molecule-plugin-lxd-0.6.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/test/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/test/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/test/lxd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/test/lxd/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/test/lxd/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 08:43:32.393151 molecule-plugin-lxd-0.6.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tools/Vagrantfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      514 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tools/create_testbox.sh
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tools/extract_plugin_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tools/generate-templates.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6414 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tools/test-setup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2023-09-15 08:43:11.000000 molecule-plugin-lxd-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.366743 molecule_plugin_lxd-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.ansible-lint-ignore
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.350743 molecule_plugin_lxd-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-06 08:58:46.366743 molecule_plugin_lxd-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.350743 molecule_plugin_lxd-0.6.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/doc/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/doc/ec2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/doc/ec2/platforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/doc/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/doc/vagrant/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.354743 molecule_plugin_lxd-0.6.1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/molecule/test-podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/molecule/test-podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/molecule/test-podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/molecule/test-podman/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:58:46.366743 molecule_plugin_lxd-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.354743 molecule_plugin_lxd-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.354743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.358743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.362743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.362743 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 08:58:46.000000 molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.354743 molecule_plugin_lxd-0.6.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.362743 molecule_plugin_lxd-0.6.1/test/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/test/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/test/lxd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/test/lxd/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/test/lxd/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:58:46.362743 molecule_plugin_lxd-0.6.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tools/Vagrantfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      514 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tools/create_testbox.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tools/extract_plugin_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tools/generate-templates.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6414 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tools/test-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-06 08:58:33.000000 molecule_plugin_lxd-0.6.1/tox.ini
```

### Comparing `molecule-plugin-lxd-0.6.0/.ansible-lint-ignore` & `molecule_plugin_lxd-0.6.1/.ansible-lint-ignore`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/.github/workflows/release.yml` & `molecule_plugin_lxd-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/.github/workflows/tox.yml` & `molecule_plugin_lxd-0.6.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/.gitignore` & `molecule_plugin_lxd-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/.pre-commit-config.yaml` & `molecule_plugin_lxd-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/LICENSE` & `molecule_plugin_lxd-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/PKG-INFO` & `molecule_plugin_lxd-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugin-lxd
-Version: 0.6.0
+Version: 0.6.1
 Summary: Molecule LXD Plugin
 Author-email: Philipp Dittert <philipp.dittert@gmail.com>
 Maintainer-email: Philipp Dittert <philipp.dittert@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/phlpdtrt/molecule-plugin-lxd
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/phlpdtrt/molecule-plugin-lxd
```

### Comparing `molecule-plugin-lxd-0.6.0/README.md` & `molecule_plugin_lxd-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/bindep.txt` & `molecule_plugin_lxd-0.6.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/conftest.py` & `molecule_plugin_lxd-0.6.1/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/doc/ec2/README.rst` & `molecule_plugin_lxd-0.6.1/doc/ec2/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/doc/ec2/platforms.rst` & `molecule_plugin_lxd-0.6.1/doc/ec2/platforms.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/doc/vagrant/README.rst` & `molecule_plugin_lxd-0.6.1/doc/vagrant/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/pyproject.toml` & `molecule_plugin_lxd-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/driver.py` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/create.yml` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
 
   vars:
     default_source:
       type: image
       mode: pull
-      server: https://images.linuxcontainers.org
+      server: https://images.lxd.canonical.com
       alias: ubuntu/jammy
       protocol: simplestreams
     default_config:
       "security.nesting": "true"
 
   tasks:
     - name: Create molecule instance(s)
```

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/destroy.yml` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd/lxd/playbooks/prepare.yml` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd/lxd/playbooks/prepare.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/PKG-INFO` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugin-lxd
-Version: 0.6.0
+Version: 0.6.1
 Summary: Molecule LXD Plugin
 Author-email: Philipp Dittert <philipp.dittert@gmail.com>
 Maintainer-email: Philipp Dittert <philipp.dittert@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/phlpdtrt/molecule-plugin-lxd
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/phlpdtrt/molecule-plugin-lxd
```

### Comparing `molecule-plugin-lxd-0.6.0/src/molecule_plugin_lxd.egg-info/SOURCES.txt` & `molecule_plugin_lxd-0.6.1/src/molecule_plugin_lxd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/test/lxd/conftest.py` & `molecule_plugin_lxd-0.6.1/test/lxd/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/test/lxd/test_func.py` & `molecule_plugin_lxd-0.6.1/test/lxd/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/tools/create_testbox.sh` & `molecule_plugin_lxd-0.6.1/tools/create_testbox.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/tools/generate-templates.sh` & `molecule_plugin_lxd-0.6.1/tools/generate-templates.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/tools/test-setup.sh` & `molecule_plugin_lxd-0.6.1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugin-lxd-0.6.0/tox.ini` & `molecule_plugin_lxd-0.6.1/tox.ini`

 * *Files identical despite different names*

