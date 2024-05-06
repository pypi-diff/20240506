# Comparing `tmp/setuptools-scm-8.0.3.tar.gz` & `tmp/setuptools-scm-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-scm-8.0.3.tar", last modified: Fri Sep 22 08:29:11 2023, max compression
+gzip compressed data, was "setuptools-scm-8.0.4.tar", last modified: Mon Oct  2 15:09:14 2023, max compression
```

## Comparing `setuptools-scm-8.0.3.tar` & `setuptools-scm-8.0.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.479638 setuptools-scm-8.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.471638 setuptools-scm-8.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.471638 setuptools-scm-8.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2023-09-22 08:29:11.479638 setuptools-scm-8.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/_own_version_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.475638 setuptools-scm-8.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/customizing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.471638 setuptools-scm-8.0.3/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.475638 setuptools-scm-8.0.3/docs/examples/version_scheme_code/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/examples/version_scheme_code/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/examples/version_scheme_code/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/extending.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/overrides.md
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/hatch.toml
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 08:29:11.479638 setuptools-scm-8.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.471638 setuptools-scm-8.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.475638 setuptools-scm-8.0.3/src/setuptools_scm/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.475638 setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/hg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_get_version_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.479638 setuptools-scm-8.0.3/src/setuptools_scm/_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_integration/dump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_integration/pyproject_reading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_integration/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_modify_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/_version_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/fallbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/hg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/hg_git.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/scm_workdir.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/src/setuptools_scm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.475638 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-22 08:29:11.000000 setuptools-scm-8.0.3/src/setuptools_scm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 08:29:11.479638 setuptools-scm-8.0.3/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/Dockerfile.busted-buster
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/Dockerfile.rawhide-git
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      577 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/play_out_381.bash
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_basic_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18308 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_hg_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_internal_log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_mercurial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/testing/wd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-09-22 08:28:49.000000 setuptools-scm-8.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.650890 setuptools-scm-8.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.642890 setuptools-scm-8.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.642890 setuptools-scm-8.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-10-02 15:09:14.650890 setuptools-scm-8.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/_own_version_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.642890 setuptools-scm-8.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/customizing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.638890 setuptools-scm-8.0.4/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.642890 setuptools-scm-8.0.4/docs/examples/version_scheme_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/examples/version_scheme_code/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/examples/version_scheme_code/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/extending.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/overrides.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/hatch.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-02 15:09:14.650890 setuptools-scm-8.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.638890 setuptools-scm-8.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.646890 setuptools-scm-8.0.4/src/setuptools_scm/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.646890 setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_get_version_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.646890 setuptools-scm-8.0.4/src/setuptools_scm/_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_integration/dump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_integration/pyproject_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_integration/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_integration/toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_modify_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/_version_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/fallbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/hg_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/scm_workdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/src/setuptools_scm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.646890 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-02 15:09:14.000000 setuptools-scm-8.0.4/src/setuptools_scm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 15:09:14.646890 setuptools-scm-8.0.4/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/Dockerfile.busted-buster
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/Dockerfile.rawhide-git
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      577 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/play_out_381.bash
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_basic_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18382 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_hg_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_internal_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/testing/wd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-10-02 15:08:52.000000 setuptools-scm-8.0.4/tox.ini
```

### Comparing `setuptools-scm-8.0.3/.github/workflows/python-tests.yml` & `setuptools-scm-8.0.4/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/.gitignore` & `setuptools-scm-8.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/LICENSE` & `setuptools-scm-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/PKG-INFO` & `setuptools-scm-8.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-scm
-Version: 8.0.3
+Version: 8.0.4
 Summary: the blessed package to manage your versions by scm tags
 Author-email: Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -17,14 +17,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
+Project-URL: documentation, https://setuptools-scm.readthedocs.io/
 Project-URL: repository, https://github.com/pypa/setuptools_scm/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -37,32 +38,34 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging>=20
 Requires-Dist: setuptools
 Requires-Dist: tomli>=1; python_version < "3.11"
-Requires-Dist: typing-extensions; python_version < "3.11"
+Requires-Dist: typing-extensions
 Provides-Extra: docs
 Requires-Dist: entangled_cli[rich]; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-entangled-plugin; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: pygments; extra == "docs"
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
+Requires-Dist: build; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: rich; extra == "test"
-Requires-Dist: virtualenv>20; extra == "test"
+Requires-Dist: wheel; extra == "test"
 Provides-Extra: toml
 
 # setuptools_scm
 [![github ci](https://github.com/pypa/setuptools_scm/workflows/python%20tests+artifacts+release/badge.svg)](https://github.com/pypa/setuptools_scm/actions)
+[![Documentation Status](https://readthedocs.org/projects/setuptools-scm/badge/?version=latest)](https://setuptools-scm.readthedocs.io/en/latest/?badge=latest)
 [![tidelift](https://tidelift.com/badges/package/pypi/setuptools-scm) ](https://tidelift.com/subscription/pkg/pypi-setuptools-scm?utm_source=pypi-setuptools-scm&utm_medium=readme)
 
 ## about
 
 [setuptools-scm] extracts Python package versions from `git` or
 `hg` metadata instead of declaring them as the version argument
 or in an SCM managed file.
@@ -115,22 +118,24 @@
 ```
 
 Where `pkg` is the name of your package.
 
 If you need to confirm which version string is being generated or debug the configuration,
 you can install [setuptools-scm] directly in your working environment and run:
 
-[setuptools-scm]: https://github.com/pypa/setuptools_scm
-
 ```console
 $ python -m setuptools_scm
 # To explore other options, try:
 $ python -m setuptools_scm --help
 ```
 
+For further configuration see the [documentation].
+
+[setuptools-scm]: https://github.com/pypa/setuptools_scm
+[documentation]: https://setuptools-scm.readthedocs.io/
 
 
 ## Interaction with Enterprise Distributions
 
 Some enterprise distributions like RHEL7
 ship rather old setuptools versions.
```

### Comparing `setuptools-scm-8.0.3/README.md` & `setuptools-scm-8.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # setuptools_scm
 [![github ci](https://github.com/pypa/setuptools_scm/workflows/python%20tests+artifacts+release/badge.svg)](https://github.com/pypa/setuptools_scm/actions)
+[![Documentation Status](https://readthedocs.org/projects/setuptools-scm/badge/?version=latest)](https://setuptools-scm.readthedocs.io/en/latest/?badge=latest)
 [![tidelift](https://tidelift.com/badges/package/pypi/setuptools-scm) ](https://tidelift.com/subscription/pkg/pypi-setuptools-scm?utm_source=pypi-setuptools-scm&utm_medium=readme)
 
 ## about
 
 [setuptools-scm] extracts Python package versions from `git` or
 `hg` metadata instead of declaring them as the version argument
 or in an SCM managed file.
@@ -56,22 +57,24 @@
 ```
 
 Where `pkg` is the name of your package.
 
 If you need to confirm which version string is being generated or debug the configuration,
 you can install [setuptools-scm] directly in your working environment and run:
 
-[setuptools-scm]: https://github.com/pypa/setuptools_scm
-
 ```console
 $ python -m setuptools_scm
 # To explore other options, try:
 $ python -m setuptools_scm --help
 ```
 
+For further configuration see the [documentation].
+
+[setuptools-scm]: https://github.com/pypa/setuptools_scm
+[documentation]: https://setuptools-scm.readthedocs.io/
 
 
 ## Interaction with Enterprise Distributions
 
 Some enterprise distributions like RHEL7
 ship rather old setuptools versions.
```

### Comparing `setuptools-scm-8.0.3/_own_version_helper.py` & `setuptools-scm-8.0.4/_own_version_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pyproject.toml is respected
 """
 from __future__ import annotations
 
 import logging
 from typing import Callable
 
-from setuptools.build_meta import *  # noqa
+from setuptools import build_meta as build_meta  # noqa
 
 from setuptools_scm import _types as _t
 from setuptools_scm import Configuration
 from setuptools_scm import get_version
 from setuptools_scm import git
 from setuptools_scm import hg
 from setuptools_scm.fallbacks import parse_pkginfo
```

### Comparing `setuptools-scm-8.0.3/docs/config.md` & `setuptools-scm-8.0.4/docs/config.md`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/docs/customizing.md` & `setuptools-scm-8.0.4/docs/customizing.md`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/docs/extending.md` & `setuptools-scm-8.0.4/docs/extending.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 `guess-next-dev (default)`
 :   Automatically guesses the next development version (default).
     Guesses the upcoming release by incrementing the pre-release segment if present,
     otherwise by incrementing the micro segment. Then appends :code:`.devN`.
     In case the tag ends with `.dev0` the version is not bumped
     and custom `.devN` versions will trigger a error.
+
 `post-release (deprecated)`
 :   Generates post release versions (adds `.postN`)
     after review of the version number pep this is considered a bad idea
     as post releases are intended to be chosen not autogenerated.
 
     !!! warning "the recommended replacement is `no-guess-dev`"
 
@@ -75,14 +76,15 @@
 `release-branch-semver`
 :   Semantic versioning for projects with release branches.
     The same as `guess-next-dev` (incrementing the pre-release or micro segment)
     however when on a release branch: a branch whose name (ignoring namespace) parses as a version
     that matches the most recent tag up to the minor segment. Otherwise if on a
     non-release branch, increments the minor segment and sets the micro segment to
     zero, then appends `.devN`
+
 `no-guess-dev`
 : Does no next version guessing, just adds `.post1.devN`
 
 
 ### `setuptools_scm.local_scheme`
 Configures how the local part of a version is rendered given a
 [ScmVersion][setuptools_scm.version.ScmVersion] instance and should return a string
```

### Comparing `setuptools-scm-8.0.3/docs/index.md` & `setuptools-scm-8.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/docs/overrides.md` & `setuptools-scm-8.0.4/docs/overrides.md`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/docs/usage.md` & `setuptools-scm-8.0.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/mkdocs.yml` & `setuptools-scm-8.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/pyproject.toml` & `setuptools-scm-8.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 
 [build-system]
-build-backend = "_own_version_helper"
+build-backend = "_own_version_helper:build_meta"
 requires = [
-  "rich",
   "setuptools>=61",
   'tomli; python_version < "3.11"',
 ]
 backend-path = [
   ".",
   "src",
 ]
@@ -39,36 +38,38 @@
 dynamic = [
   "version",
 ]
 dependencies = [
   "packaging>=20",
   "setuptools",
   'tomli>=1; python_version < "3.11"',
-  'typing-extensions; python_version < "3.11"',
+  "typing-extensions",
 ]
 [project.optional-dependencies]
 docs = [
   "entangled_cli[rich]",
   "mkdocs",
   "mkdocs-entangled-plugin",
   "mkdocs-material",
   "mkdocstrings[python]",
   "pygments",
 ]
 rich = [
   "rich",
 ]
 test = [
+  "build",
   "pytest",
   "rich",
-  "virtualenv>20",
+  "wheel",
 ]
 toml = [
 ]
 [project.urls]
+documentation = "https://setuptools-scm.readthedocs.io/"
 repository = "https://github.com/pypa/setuptools_scm/"
 [project.entry-points."distutils.setup_keywords"]
 use_scm_version = "setuptools_scm._integration.setuptools:version_keyword"
 [project.entry-points."setuptools.file_finders"]
 setuptools_scm = "setuptools_scm._file_finders:find_files"
 [project.entry-points."setuptools.finalize_distribution_options"]
 setuptools_scm = "setuptools_scm._integration.setuptools:infer_version"
@@ -104,7 +105,30 @@
 where = ["src"]
 namespaces = false
 
 [tool.setuptools.dynamic]
 version = { attr = "_own_version_helper.version"}
 
 [tool.setuptools_scm]
+
+[tool.ruff]
+select = ["E", "F", "B", "U", "YTT", "C", "DTZ", "PYI", "PT"]
+ignore = ["B028"]
+
+[tool.pytest.ini_options]
+testpaths = ["testing"]
+filterwarnings = [
+  "error",
+  "ignore:.*tool\\.setuptools_scm.*",
+  "ignore:.*git archive did not support describe output.*:UserWarning",
+]
+log_level = "debug"
+log_cli_level = "info"
+# disable unraisable until investigated
+addopts = ["-p", "no:unraisableexception"]
+markers = [
+  "issue(id): reference to github issue",
+  "skip_commit: allows to skip committing in the helpers",
+]
+
+[tool.scriv]
+format = "md"
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/__init__.py` & `setuptools-scm-8.0.4/src/setuptools_scm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 :copyright: 2010-2023 by Ronny Pfannschmidt
 :license: MIT
 """
 from __future__ import annotations
 
 from ._config import Configuration
+from ._config import DEFAULT_LOCAL_SCHEME  # soft deprecated
+from ._config import DEFAULT_VERSION_SCHEME  # soft deprecated
 from ._get_version_impl import _get_version  # soft deprecated
 from ._get_version_impl import get_version  # soft deprecated
 from ._integration.dump_version import dump_version  # soft deprecated
 from ._version_cls import NonNormalizedVersion
 from ._version_cls import Version
 from .version import ScmVersion
 
 
 # Public API
 __all__ = [
-    "get_version",  # deprecated imported for backward compatibility
-    "_get_version",  # deprecated imported for backward compatibility
-    "dump_version",  # deprecated imported for backward compatibility
+    # soft deprecated imports, left for backward compatibility
+    "get_version",
+    "_get_version",
+    "dump_version",
+    "DEFAULT_VERSION_SCHEME",
+    "DEFAULT_LOCAL_SCHEME",
     "Configuration",
     "Version",
     "ScmVersion",
     "NonNormalizedVersion",
 ]
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_cli.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_config.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ configuration """
 from __future__ import annotations
 
 import dataclasses
 import os
 import re
 import warnings
+from pathlib import Path
 from typing import Any
-from typing import Callable
 from typing import Pattern
 from typing import Protocol
 
 from . import _log
 from . import _types as _t
 from ._integration.pyproject_reading import (
     get_args_for_pyproject as _get_args_for_pyproject,
@@ -61,16 +61,15 @@
     if relative_to:
         if (
             os.path.isabs(root)
             and os.path.isabs(relative_to)
             and not os.path.commonpath([root, relative_to]) == root
         ):
             warnings.warn(
-                "absolute root path '%s' overrides relative_to '%s'"
-                % (root, relative_to)
+                f"absolute root path '{root}' overrides relative_to '{relative_to}'"
             )
         if os.path.isdir(relative_to):
             warnings.warn(
                 "relative_to is expected to be a file,"
                 f" its the directory {relative_to}\n"
                 "assuming the parent directory was passed"
             )
@@ -111,29 +110,30 @@
         return _check_absolute_root(self.root, self.relative_to)
 
     @classmethod
     def from_file(
         cls,
         name: str | os.PathLike[str] = "pyproject.toml",
         dist_name: str | None = None,
-        _load_toml: Callable[[str], dict[str, Any]] | None = None,
+        _require_section: bool = True,
         **kwargs: Any,
     ) -> Configuration:
         """
         Read Configuration from pyproject.toml (or similar).
         Raises exceptions when file is not found or toml is
         not installed or the file has invalid format or does
         not contain the [tool.setuptools_scm] section.
         """
 
-        pyproject_data = _read_pyproject(name, _load_toml=_load_toml)
+        pyproject_data = _read_pyproject(Path(name), require_section=_require_section)
         args = _get_args_for_pyproject(pyproject_data, dist_name, kwargs)
 
         args.update(read_toml_overrides(args["dist_name"]))
-        return cls.from_data(relative_to=name, data=args)
+        relative_to = args.pop("relative_to", name)
+        return cls.from_data(relative_to=relative_to, data=args)
 
     @classmethod
     def from_data(
         cls, relative_to: str | os.PathLike[str], data: dict[str, Any]
     ) -> Configuration:
         """
         given configuration data
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_entrypoints.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_entrypoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from importlib.metadata import entry_points, EntryPoints
 
 
 log = _log.log.getChild("entrypoints")
 
 
 def version_from_entrypoint(
-    config: Configuration, entrypoint: str, root: _t.PathT
+    config: Configuration, *, entrypoint: str, root: _t.PathT
 ) -> version.ScmVersion | None:
     from .discover import iter_matching_entrypoints
 
     log.debug("version_from_ep %s in %s", entrypoint, root)
     for ep in iter_matching_entrypoints(root, entrypoint, config):
         fn: ParseFunction = ep.load()
         maybe_version: version.ScmVersion | None = fn(root, config=config)
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/__init__.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     realpath = os.path.normcase(os.path.realpath(path))
     seen: set[str] = set()
     res: list[str] = []
     for dirpath, dirnames, filenames in os.walk(realpath, followlinks=True):
         # dirpath with symlinks resolved
         realdirpath = os.path.normcase(os.path.realpath(dirpath))
 
-        def _link_not_in_scm(n: str) -> bool:
+        def _link_not_in_scm(n: str, realdirpath: str = realdirpath) -> bool:
             fn = os.path.join(realdirpath, os.path.normcase(n))
             return os.path.islink(fn) and fn not in scm_files
 
         if not force_all_files and realdirpath not in scm_dirs:
             # directory not in scm, don't walk it's content
             dirnames[:] = []
             continue
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/git.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/git.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_file_finders/hg.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_file_finders/hg.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def _hg_ls_files_and_dirs(toplevel: str) -> tuple[set[str], set[str]]:
     hg_files: set[str] = set()
     hg_dirs = {toplevel}
     res = _run(["hg", "files"], cwd=toplevel)
     if res.returncode:
-        (), ()
+        return set(), set()
     for name in res.stdout.splitlines():
         name = os.path.normcase(name).replace("/", os.path.sep)
         fullname = os.path.join(toplevel, name)
         hg_files.add(fullname)
         dirname = os.path.dirname(fullname)
         while len(dirname) > len(toplevel) and dirname not in hg_dirs:
             hg_dirs.add(dirname)
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_get_version_impl.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_get_version_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,26 +28,30 @@
             if parse_result is not None and not isinstance(parse_result, ScmVersion):
                 raise TypeError(
                     f"version parse result was {str!r}\n"
                     "please return a parsed version (ScmVersion)"
                 )
             return parse_result
         else:
-            entrypoint = "setuptools_scm.parse_scm"
-            root = config.absolute_root
-            return _entrypoints.version_from_entrypoint(config, entrypoint, root)
+            return _entrypoints.version_from_entrypoint(
+                config,
+                entrypoint="setuptools_scm.parse_scm",
+                root=config.absolute_root,
+            )
     except _run_cmd.CommandNotFoundError as e:
         _log.exception("command %s not found while parsing the scm, using fallbacks", e)
         return None
 
 
 def parse_fallback_version(config: Configuration) -> ScmVersion | None:
-    entrypoint = "setuptools_scm.parse_scm_fallback"
-    root = config.fallback_root
-    return _entrypoints.version_from_entrypoint(config, entrypoint, root)
+    return _entrypoints.version_from_entrypoint(
+        config,
+        entrypoint="setuptools_scm.parse_scm_fallback",
+        root=config.fallback_root,
+    )
 
 
 def parse_version(config: Configuration) -> ScmVersion | None:
     return (
         _read_pretended_version_for(config)
         or parse_scm_version(config)
         or parse_fallback_version(config)
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_integration/dump_version.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_integration/dump_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,36 +13,52 @@
 
 TEMPLATES = {
     ".py": """\
 # file generated by setuptools_scm
 # don't change, don't track in version control
 TYPE_CHECKING = False
 if TYPE_CHECKING:
-    from typing import Tuple
+    from typing import Tuple, Union
+    VERSION_TUPLE = Tuple[Union[int, str], ...]
+else:
+    VERSION_TUPLE = object
+
+version: str
+__version__: str
+__version_tuple__: VERSION_TUPLE
+version_tuple: VERSION_TUPLE
 
-__version__ = version = {version!r}  # type: str
-__version_tuple__ = version_tuple = {version_tuple!r}  # type: Tuple[int | str, ...]
+__version__ = version = {version!r}
+__version_tuple__ = version_tuple = {version_tuple!r}
 """,
     ".txt": "{version}",
 }
 
 
 def dump_version(
     root: _t.PathT,
     version: str,
     write_to: _t.PathT,
     template: str | None = None,
     scm_version: ScmVersion | None = None,
 ) -> None:
     assert isinstance(version, str)
-    # todo: assert write_to doesnt escape
+    root = Path(root)
     write_to = Path(write_to)
-
-    assert not write_to.is_absolute(), f"{write_to=}"
-    target = Path(root).joinpath(write_to)
+    if write_to.is_absolute():
+        # trigger warning on escape
+        write_to.relative_to(root)
+        warnings.warn(
+            f"{write_to=!s} is a absolute path,"
+            " please switch to using a relative version file",
+            DeprecationWarning,
+        )
+        target = write_to
+    else:
+        target = Path(root).joinpath(write_to)
     write_version_to_path(
         target, template=template, version=version, scm_version=scm_version
     )
 
 
 def _validate_template(target: Path, template: str | None) -> str:
     if template == "":
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_log.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_log.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_modify_version.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_modify_version.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_overrides.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_overrides.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import os
 import re
 from typing import Any
-from typing import cast
-from typing import TypedDict
 
 from . import _config
 from . import _log
 from . import version
-from ._integration.pyproject_reading import lazy_toml_load
+from ._integration.toml import load_toml_or_inline_map
 
 log = _log.log.getChild("overrides")
 
 PRETEND_KEY = "SETUPTOOLS_SCM_PRETEND_VERSION"
 PRETEND_KEY_NAMED = PRETEND_KEY + "_FOR_{name}"
 
 
@@ -47,27 +45,10 @@
         # we use meta here since the pretended version
         # must adhere to the pep to begin with
         return version.meta(tag=pretended, preformatted=True, config=config)
     else:
         return None
 
 
-class _CheatTomlData(TypedDict):
-    cheat: dict[str, Any]
-
-
-def load_toml_or_inline_map(data: str | None) -> dict[str, Any]:
-    """
-    load toml data - with a special hack if only a inline map is given
-    """
-    if not data:
-        return {}
-    elif data[0] == "{":
-        data = "cheat=" + data
-        loaded: _CheatTomlData = cast(_CheatTomlData, lazy_toml_load(data))
-        return loaded["cheat"]
-    return lazy_toml_load(data)
-
-
 def read_toml_overrides(dist_name: str | None) -> dict[str, Any]:
     data = read_named_env(name="OVERRIDES", dist_name=dist_name)
     return load_toml_or_inline_map(data)
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_run_cmd.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_run_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 import os
 import shlex
 import subprocess
 import textwrap
 import warnings
 from typing import Callable
+from typing import Final
 from typing import Mapping
 from typing import overload
 from typing import Sequence
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 from . import _log
 from . import _types as _t
 
 if TYPE_CHECKING:
     BaseCompletedProcess = subprocess.CompletedProcess[str]
 else:
     BaseCompletedProcess = subprocess.CompletedProcess
 
+# pick 40 seconds
+# unfortunately github CI for windows sometimes needs
+# up to 30 seconds to start a command
+
+BROKEN_TIMEOUT: Final[int] = 40
 
 log = _log.log.getChild("run_cmd")
 
 PARSE_RESULT = TypeVar("PARSE_RESULT")
 T = TypeVar("T")
 
 
@@ -122,15 +128,15 @@
 
 def run(
     cmd: _t.CMD_TYPE,
     cwd: _t.PathT,
     *,
     strip: bool = True,
     trace: bool = True,
-    timeout: int = 20,
+    timeout: int = BROKEN_TIMEOUT,
     check: bool = False,
 ) -> CompletedProcess:
     if isinstance(cmd, str):
         cmd = shlex.split(cmd)
     else:
         cmd = [os.fspath(x) for x in cmd]
     cmd_4_trace = " ".join(map(_unsafe_quote_for_display, cmd))
@@ -170,15 +176,15 @@
     return text if all(c not in text for c in " {[:") else f'"{text}"'
 
 
 def has_command(
     name: str, args: Sequence[str] = ["version"], warn: bool = True
 ) -> bool:
     try:
-        p = run([name, *args], cwd=".", timeout=5)
+        p = run([name, *args], cwd=".", timeout=BROKEN_TIMEOUT)
         if p.returncode != 0:
             log.error(f"Command '{name}' returned non-zero. This is stderr:")
             log.error(p.stderr)
     except OSError as e:
         log.warning("command %s missing: %s", name, e)
         res = False
     except subprocess.TimeoutExpired as e:
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_types.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_types.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/_version_cls.py` & `setuptools-scm-8.0.4/src/setuptools_scm/_version_cls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
-from logging import getLogger
 from typing import cast
 from typing import Type
 from typing import Union
 
 try:
     from packaging.version import InvalidVersion
     from packaging.version import Version as Version
 except ImportError:
     from setuptools.extern.packaging.version import InvalidVersion  # type: ignore
     from setuptools.extern.packaging.version import Version as Version  # type: ignore
+from . import _log
+
+log = _log.log.getChild("version_cls")
 
 
 class NonNormalizedVersion(Version):
     """A non-normalizing version handler.
 
     You can use this class to preserve version verification but skip normalization.
     For example you can use this to avoid git release candidate version tags
@@ -37,18 +39,16 @@
         # same pattern as parent
         return f"<NonNormalizedVersion({self._raw_version!r})>"
 
 
 def _version_as_tuple(version_str: str) -> tuple[int | str, ...]:
     try:
         parsed_version = Version(version_str)
-    except InvalidVersion:
-        log = getLogger(__name__).parent
-        assert log is not None
-        log.error("failed to parse version %s", version_str)
+    except InvalidVersion as e:
+        log.error("failed to parse version %s: %s", e, version_str)
         return (version_str,)
     else:
         version_fields: tuple[int | str, ...] = parsed_version.release
         if parsed_version.dev is not None:
             version_fields += (f"dev{parsed_version.dev}",)
         if parsed_version.local is not None:
             version_fields += (parsed_version.local,)
@@ -80,10 +80,12 @@
         # Use `version_cls` if provided, default to packaging or pkg_resources
         if version_cls is None:
             return Version
         elif isinstance(version_cls, str):
             try:
                 return cast(Type[_VersionT], import_name(version_cls))
             except:  # noqa
-                raise ValueError(f"Unable to import version_cls='{version_cls}'")
+                raise ValueError(
+                    f"Unable to import version_cls='{version_cls}'"
+                ) from None
         else:
             return version_cls
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/discover.py` & `setuptools-scm-8.0.4/src/setuptools_scm/discover.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/fallbacks.py` & `setuptools-scm-8.0.4/src/setuptools_scm/fallbacks.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/git.py` & `setuptools-scm-8.0.4/src/setuptools_scm/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 import re
 import shlex
 import warnings
 from datetime import date
 from datetime import datetime
+from datetime import timezone
 from os.path import samefile
 from pathlib import Path
 from typing import Callable
 from typing import Sequence
 from typing import TYPE_CHECKING
 
 from . import _types as _t
@@ -264,15 +265,15 @@
             distance = wd.count_all_nodes()
             node = "g" + node
             dirty = wd.is_dirty()
         version = meta(
             tag=tag, distance=distance, dirty=dirty, node=node, config=config
         )
     branch = wd.get_branch()
-    node_date = wd.get_head_date() or date.today()
+    node_date = wd.get_head_date() or datetime.now(timezone.utc).date()
     return dataclasses.replace(version, branch=branch, node_date=node_date)
 
 
 def _git_parse_describe(
     describe_output: str,
 ) -> tuple[str, int, str | None, bool]:
     # 'describe_output' looks e.g. like 'v1.5.0-0-g4060507' or
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/hg.py` & `setuptools-scm-8.0.4/src/setuptools_scm/hg.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/hg_git.py` & `setuptools-scm-8.0.4/src/setuptools_scm/hg_git.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/integration.py` & `setuptools-scm-8.0.4/src/setuptools_scm/integration.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm/version.py` & `setuptools-scm-8.0.4/src/setuptools_scm/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
 def guess_next_simple_semver(
     version: ScmVersion, retain: int, increment: bool = True
 ) -> str:
     try:
         parts = [int(i) for i in str(version.tag).split(".")[:retain]]
     except ValueError:
-        raise ValueError(f"{version} can't be parsed as numeric version")
+        raise ValueError(f"{version} can't be parsed as numeric version") from None
     while len(parts) < retain:
         parts.append(0)
     if increment:
         parts[-1] += 1
     while len(parts) < SEMVER_LEN:
         parts.append(0)
     return ".".join(str(i) for i in parts)
@@ -351,25 +351,28 @@
 
     today = version.time.date()
     head_date = node_date or today
     # compute patch
     if match is None:
         tag_date = today
     else:
-        tag_date = datetime.strptime(match.group("date"), date_fmt).date()
+        tag_date = (
+            datetime.strptime(match.group("date"), date_fmt)
+            .replace(tzinfo=timezone.utc)
+            .date()
+        )
     if tag_date == head_date:
         patch = "0" if match is None else (match.group("patch") or "0")
         patch = int(patch) + 1
     else:
         if tag_date > head_date and match is not None:
             # warn on future times
             warnings.warn(
-                "your previous tag  ({}) is ahead your node date ({})".format(
-                    tag_date, head_date
-                )
+                f"your previous tag  ({tag_date})"
+                f" is ahead your node date ({head_date})"
             )
         patch = 0
     next_version = "{node_date:{date_fmt}}.{patch}".format(
         node_date=head_date, date_fmt=date_fmt, patch=patch
     )
     # rely on the Version object to ensure consistency (e.g. remove leading 0s)
     if version_cls is None:
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm.egg-info/PKG-INFO` & `setuptools-scm-8.0.4/src/setuptools_scm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-scm
-Version: 8.0.3
+Version: 8.0.4
 Summary: the blessed package to manage your versions by scm tags
 Author-email: Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -17,14 +17,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
+Project-URL: documentation, https://setuptools-scm.readthedocs.io/
 Project-URL: repository, https://github.com/pypa/setuptools_scm/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -37,32 +38,34 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging>=20
 Requires-Dist: setuptools
 Requires-Dist: tomli>=1; python_version < "3.11"
-Requires-Dist: typing-extensions; python_version < "3.11"
+Requires-Dist: typing-extensions
 Provides-Extra: docs
 Requires-Dist: entangled_cli[rich]; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-entangled-plugin; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: pygments; extra == "docs"
 Provides-Extra: rich
 Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
+Requires-Dist: build; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: rich; extra == "test"
-Requires-Dist: virtualenv>20; extra == "test"
+Requires-Dist: wheel; extra == "test"
 Provides-Extra: toml
 
 # setuptools_scm
 [![github ci](https://github.com/pypa/setuptools_scm/workflows/python%20tests+artifacts+release/badge.svg)](https://github.com/pypa/setuptools_scm/actions)
+[![Documentation Status](https://readthedocs.org/projects/setuptools-scm/badge/?version=latest)](https://setuptools-scm.readthedocs.io/en/latest/?badge=latest)
 [![tidelift](https://tidelift.com/badges/package/pypi/setuptools-scm) ](https://tidelift.com/subscription/pkg/pypi-setuptools-scm?utm_source=pypi-setuptools-scm&utm_medium=readme)
 
 ## about
 
 [setuptools-scm] extracts Python package versions from `git` or
 `hg` metadata instead of declaring them as the version argument
 or in an SCM managed file.
@@ -115,22 +118,24 @@
 ```
 
 Where `pkg` is the name of your package.
 
 If you need to confirm which version string is being generated or debug the configuration,
 you can install [setuptools-scm] directly in your working environment and run:
 
-[setuptools-scm]: https://github.com/pypa/setuptools_scm
-
 ```console
 $ python -m setuptools_scm
 # To explore other options, try:
 $ python -m setuptools_scm --help
 ```
 
+For further configuration see the [documentation].
+
+[setuptools-scm]: https://github.com/pypa/setuptools_scm
+[documentation]: https://setuptools-scm.readthedocs.io/
 
 
 ## Interaction with Enterprise Distributions
 
 Some enterprise distributions like RHEL7
 ship rather old setuptools versions.
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm.egg-info/SOURCES.txt` & `setuptools-scm-8.0.4/src/setuptools_scm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .gitattributes
 .gitignore
-.readthedocs.yaml
-CHANGELOG.rst
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 _own_version_helper.py
 hatch.toml
 mkdocs.yml
 mypy.ini
@@ -52,14 +51,15 @@
 src/setuptools_scm/_file_finders/__init__.py
 src/setuptools_scm/_file_finders/git.py
 src/setuptools_scm/_file_finders/hg.py
 src/setuptools_scm/_integration/__init__.py
 src/setuptools_scm/_integration/dump_version.py
 src/setuptools_scm/_integration/pyproject_reading.py
 src/setuptools_scm/_integration/setuptools.py
+src/setuptools_scm/_integration/toml.py
 testing/Dockerfile.busted-buster
 testing/Dockerfile.rawhide-git
 testing/__init__.py
 testing/conftest.py
 testing/play_out_381.bash
 testing/test_basic_api.py
 testing/test_cli.py
```

### Comparing `setuptools-scm-8.0.3/src/setuptools_scm.egg-info/entry_points.txt` & `setuptools-scm-8.0.4/src/setuptools_scm.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/testing/conftest.py` & `setuptools-scm-8.0.4/testing/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import os
 from pathlib import Path
 from types import TracebackType
 from typing import Any
 from typing import Iterator
 
 import pytest
+from typing_extensions import Self
 
 from .wd_wrapper import WorkDir
 from setuptools_scm._run_cmd import run
 
 
 def pytest_configure() -> None:
     # 2009-02-13T23:31:30+00:00
     os.environ["SOURCE_DATE_EPOCH"] = "1234567890"
     os.environ["SETUPTOOLS_SCM_DEBUG"] = "1"
 
 
-VERSION_PKGS = ["setuptools", "setuptools_scm", "packaging"]
+VERSION_PKGS = ["setuptools", "setuptools_scm", "packaging", "build", "wheel"]
 
 
 def pytest_report_header() -> list[str]:
     from importlib.metadata import version
 
     res = []
     for pkg in VERSION_PKGS:
@@ -42,15 +43,15 @@
 
 class DebugMode(contextlib.AbstractContextManager):  # type: ignore[type-arg]
     from setuptools_scm import _log as __module
 
     def __init__(self) -> None:
         self.__stack = contextlib.ExitStack()
 
-    def __enter__(self) -> DebugMode:
+    def __enter__(self) -> Self:
         self.enable()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
@@ -67,22 +68,22 @@
 
 @pytest.fixture(autouse=True)
 def debug_mode() -> Iterator[DebugMode]:
     with DebugMode() as debug_mode:
         yield debug_mode
 
 
-@pytest.fixture
+@pytest.fixture()
 def wd(tmp_path: Path) -> WorkDir:
     target_wd = tmp_path.resolve() / "wd"
     target_wd.mkdir()
     return WorkDir(target_wd)
 
 
-@pytest.fixture
+@pytest.fixture()
 def repositories_hg_git(tmp_path: Path) -> tuple[WorkDir, WorkDir]:
     tmp_path = tmp_path.resolve()
     path_git = tmp_path / "repo_git"
     path_git.mkdir()
 
     wd = WorkDir(path_git)
     wd("git init")
```

### Comparing `setuptools-scm-8.0.3/testing/play_out_381.bash` & `setuptools-scm-8.0.4/testing/play_out_381.bash`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/testing/test_basic_api.py` & `setuptools-scm-8.0.4/testing/test_basic_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,17 +176,16 @@
     assert read("first.txt") == "1.0"
 
     version = "1.0.dev42"
     scm_version = meta("1.0", distance=42, config=c)
     dump_version(tmp_path, version, "first.py", scm_version=scm_version)
     lines = read("first.py").splitlines()
     assert lines[-2:] == [
-        "__version__ = version = '1.0.dev42'  # type: str",
-        "__version_tuple__ = version_tuple = (1, 0, 'dev42')"
-        "  # type: Tuple[int | str, ...]",
+        "__version__ = version = '1.0.dev42'",
+        "__version_tuple__ = version_tuple = (1, 0, 'dev42')",
     ]
 
     version = "1.0.1+g4ac9d2c"
     scm_version = meta("1.0.1", node="g4ac9d2c", config=c)
     dump_version(
         tmp_path, version, "second.py", scm_version=scm_version, template=template
     )
@@ -223,22 +222,26 @@
         setuptools_scm.get_version(parse=parse)
 
 
 def test_custom_version_cls() -> None:
     """Test that `normalize` and `version_cls` work as expected"""
 
     class MyVersion:
-        def __init__(self, tag_str: str):
+        def __init__(self, tag_str: str) -> None:
             self.version = tag_str
 
         def __repr__(self) -> str:
             return f"hello,{self.version}"
 
     # you can not use normalize=False and version_cls at the same time
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match="Providing a custom `version_cls`"
+        " is not permitted when `normalize=False`",
+    ):
         setuptools_scm.get_version(normalize=False, version_cls=MyVersion)
 
     # TODO unfortunately with PRETEND_KEY the preformatted flag becomes True
     #  which bypasses our class. which other mechanism would be ok to use here
     #  to create a test?
     # monkeypatch.setenv(setuptools_scm.PRETEND_KEY, "1.0.1")
     # assert setuptools_scm.get_version(version_cls=MyVersion) == "1"
```

### Comparing `setuptools-scm-8.0.3/testing/test_cli.py` & `setuptools-scm-8.0.4/testing/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/testing/test_config.py` & `setuptools-scm-8.0.4/testing/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 
 from setuptools_scm import Configuration
 
 
 @pytest.mark.parametrize(
-    "tag, expected_version",
+    ("tag", "expected_version"),
     [
         ("apache-arrow-0.9.0", "0.9.0"),
         ("arrow-0.9.0", "0.9.0"),
         ("arrow-0.9.0-rc", "0.9.0-rc"),
         ("arrow-1", "1"),
         ("arrow-1+", "1"),
         ("arrow-1+foo", "1"),
```

### Comparing `setuptools-scm-8.0.3/testing/test_file_finder.py` & `setuptools-scm-8.0.4/testing/test_file_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 import os
 import sys
-from typing import Generator
 from typing import Iterable
 
 import pytest
 
 from .wd_wrapper import WorkDir
 from setuptools_scm._file_finders import find_files
 
 
 @pytest.fixture(params=["git", "hg"])
 def inwd(
     request: pytest.FixtureRequest, wd: WorkDir, monkeypatch: pytest.MonkeyPatch
-) -> Generator[WorkDir, None, None]:
-    param: str = getattr(request, "param")  # todo: fix
+) -> WorkDir:
+    param: str = request.param  # type: ignore
     if param == "git":
         try:
             wd("git init")
         except OSError:
             pytest.skip("git executable not found")
         wd("git config user.email test@example.com")
         wd('git config user.name "a test"')
@@ -38,15 +37,15 @@
     (adir / "filea").touch()
     bdir = wd.cwd / "bdir"
     bdir.mkdir()
     (bdir / "fileb").touch()
     if request.node.get_closest_marker("skip_commit") is None:
         wd.add_and_commit()
     monkeypatch.chdir(wd.cwd)
-    yield wd
+    return wd
 
 
 def _sep(paths: Iterable[str]) -> set[str]:
     return {path.replace("/", os.path.sep) for path in paths}
 
 
 def test_basic(inwd: WorkDir) -> None:
@@ -194,29 +193,29 @@
             "bdir/fileb",
             "data/datafile",
         }
     )
 
 
 @pytest.mark.issue(587)
-@pytest.mark.skip_commit
+@pytest.mark.skip_commit()
 def test_not_commited(inwd: WorkDir) -> None:
     assert find_files() == []
 
 
 def test_unexpanded_git_archival(wd: WorkDir, monkeypatch: pytest.MonkeyPatch) -> None:
     # When substitutions in `.git_archival.txt` are not expanded, files should
     # not be automatically listed.
     monkeypatch.chdir(wd.cwd)
     (wd.cwd / ".git_archival.txt").write_text("node: $Format:%H$", encoding="utf-8")
     (wd.cwd / "file1.txt").touch()
     assert find_files() == []
 
 
-@pytest.mark.parametrize("archive_file", (".git_archival.txt", ".hg_archival.txt"))
+@pytest.mark.parametrize("archive_file", [".git_archival.txt", ".hg_archival.txt"])
 def test_archive(
     wd: WorkDir, monkeypatch: pytest.MonkeyPatch, archive_file: str
 ) -> None:
     # When substitutions in `.git_archival.txt` are not expanded, files should
     # not be automatically listed.
     monkeypatch.chdir(wd.cwd)
     sha = "a1bda3d984d1a40d7b00ae1d0869354d6d503001"
```

### Comparing `setuptools-scm-8.0.3/testing/test_functions.py` & `setuptools-scm-8.0.4/testing/test_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools_scm.version import meta
 from setuptools_scm.version import tag_to_version
 
 c = Configuration()
 
 
 @pytest.mark.parametrize(
-    "tag, expected",
+    ("tag", "expected"),
     [
         ("1.1", "1.2"),
         ("1.2.dev", "1.2"),
         ("1.1a2", "1.1a3"),
         pytest.param(
             "23.24.post2+deadbeef",
             "23.24.post3",
@@ -44,15 +44,15 @@
     "dirty": meta("1.1", distance=0, dirty=True, config=c),
     "distance-clean": meta("1.1", distance=3, dirty=False, config=c),
     "distance-dirty": meta("1.1", distance=3, dirty=True, config=c),
 }
 
 
 @pytest.mark.parametrize(
-    "version,version_scheme, local_scheme,expected",
+    ("version", "version_scheme", "local_scheme", "expected"),
     [
         ("exact", "guess-next-dev", "node-and-date", "1.1"),
         ("dirty", "guess-next-dev", "node-and-date", "1.2.dev0+d20090213"),
         ("dirty", "guess-next-dev", "no-local-version", "1.2.dev0"),
         ("distance-clean", "guess-next-dev", "node-and-date", "1.2.dev3"),
         ("distance-dirty", "guess-next-dev", "node-and-date", "1.2.dev3+d20090213"),
         ("exact", "post-release", "node-and-date", "1.1"),
@@ -168,15 +168,15 @@
     for record in caplog.records:
         if "returned non-zero. This is stderr" in record.message:
             found_it = True
     assert found_it, "Did not find expected log record for "
 
 
 @pytest.mark.parametrize(
-    "tag, expected_version",
+    ("tag", "expected_version"),
     [
         ("1.1", "1.1"),
         ("release-1.1", "1.1"),
         pytest.param("3.3.1-rc26", "3.3.1rc26", marks=pytest.mark.issue(266)),
     ],
 )
 def test_tag_to_version(tag: str, expected_version: str) -> None:
```

### Comparing `setuptools-scm-8.0.3/testing/test_git.py` & `setuptools-scm-8.0.4/testing/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     wd.add_command = "git add ."
     wd.commit_command = "git commit -m test-{reason}"
     debug_mode.enable()
     return wd
 
 
 @pytest.mark.parametrize(
-    "given, tag, number, node, dirty",
+    ("given", "tag", "number", "node", "dirty"),
     [
         ("3.3.1-rc26-0-g9df187b", "3.3.1-rc26", 0, "g9df187b", False),
         ("17.33.0-rc-17-g38c3047c0", "17.33.0-rc", 17, "g38c3047c0", False),
     ],
 )
 def test_parse_describe_output(
     given: str, tag: str, number: int, node: str, dirty: bool
@@ -154,15 +154,16 @@
         assert git.parse(str(wd.cwd), Configuration())
 
 
 def test_version_from_git(wd: WorkDir) -> None:
     assert wd.get_version() == "0.1.dev0+d20090213"
 
     parsed = git.parse(str(wd.cwd), Configuration(), git.DEFAULT_DESCRIBE)
-    assert parsed is not None and parsed.branch in ("master", "main")
+    assert parsed is not None
+    assert parsed.branch in ("master", "main")
 
     wd.commit_testfile()
     assert wd.get_version().startswith("0.1.dev1+g")
     assert not wd.get_version().endswith("1-")
 
     wd("git tag v0.1")
     assert wd.get_version() == "0.1"
@@ -281,30 +282,31 @@
     version = wd.get_version()
 
     if today:
         # the date on the tag is in UTC
         tag = datetime.now(timezone.utc).date().strftime(".d%Y%m%d")
     else:
         tag = ".d20090213"
-    assert version.startswith("0.1.dev1+g") and version.endswith(tag)
+    assert version.startswith("0.1.dev1+g")
+    assert version.endswith(tag)
 
 
 @pytest.mark.issue(193)
 @pytest.mark.xfail(reason="sometimes relative path results")
 def test_git_worktree_support(wd: WorkDir, tmp_path: Path) -> None:
     wd.commit_testfile()
     worktree = tmp_path / "work_tree"
     wd("git worktree add -b work-tree %s" % worktree)
 
     res = run([sys.executable, "-m", "setuptools_scm", "ls"], cwd=worktree)
     assert "test.txt" in res.stdout
     assert str(worktree) in res.stdout
 
 
-@pytest.fixture
+@pytest.fixture()
 def shallow_wd(wd: WorkDir, tmp_path: Path) -> Path:
     wd.commit_testfile()
     wd.commit_testfile()
     wd.commit_testfile()
     target = tmp_path / "wd_shallow"
     run(["git", "clone", f"file://{wd.cwd}", target, "--depth=1"], tmp_path, check=True)
     return target
@@ -457,15 +459,15 @@
     # git hooks set this and break subsequent setuptools_scm unless we clean
     monkeypatch.setenv("GIT_DIR", __file__)
     assert wd.get_version() == normal
 
 
 def test_git_getdate(wd: WorkDir) -> None:
     # TODO: case coverage for git wd parse
-    today = date.today()
+    today = datetime.now(timezone.utc).date()
 
     def parse_date() -> date:
         parsed = git.parse(os.fspath(wd.cwd), Configuration())
         assert parsed is not None
         assert parsed.node_date is not None
         return parsed.node_date
 
@@ -488,15 +490,15 @@
         git,
         "run_git",
         Mock(return_value=fake_date_result),
     ):
         assert git_wd.get_head_date() is None
 
 
-@pytest.fixture
+@pytest.fixture()
 def signed_commit_wd(monkeypatch: pytest.MonkeyPatch, wd: WorkDir) -> WorkDir:
     if not has_command("gpg", args=["--version"], warn=False):
         pytest.skip("gpg executable not found")
 
     wd.write(
         ".gpg_batch_params",
         """\
@@ -515,22 +517,22 @@
     wd("git config log.showSignature true")
     wd.signed_commit_command = "git commit -S -m test-{reason}"
     return wd
 
 
 @pytest.mark.issue("https://github.com/pypa/setuptools_scm/issues/548")
 def test_git_getdate_signed_commit(signed_commit_wd: WorkDir) -> None:
-    today = date.today()
+    today = datetime.now(timezone.utc).date()
     signed_commit_wd.commit_testfile(signed=True)
     git_wd = git.GitWorkdir(signed_commit_wd.cwd)
     assert git_wd.get_head_date() == today
 
 
 @pytest.mark.parametrize(
-    "expected, from_data",
+    ("expected", "from_data"),
     [
         (
             "1.0",
             {"describe-name": "1.0-0-g0000"},
         ),
         (
             "1.1.dev3+g0000",
```

### Comparing `setuptools-scm-8.0.3/testing/test_hg_git.py` & `setuptools-scm-8.0.4/testing/test_hg_git.py`

 * *Files identical despite different names*

### Comparing `setuptools-scm-8.0.3/testing/test_integration.py` & `setuptools-scm-8.0.4/testing/test_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 import importlib.metadata
+import os
+import subprocess
 import sys
 import textwrap
 from pathlib import Path
 
 import pytest
 
 import setuptools_scm._integration.setuptools
@@ -14,15 +16,15 @@
 from setuptools_scm._overrides import PRETEND_KEY
 from setuptools_scm._overrides import PRETEND_KEY_NAMED
 from setuptools_scm._run_cmd import run
 
 c = Configuration()
 
 
-@pytest.fixture
+@pytest.fixture()
 def wd(wd: WorkDir) -> WorkDir:
     wd("git init")
     wd("git config user.email test@example.com")
     wd('git config user.name "a test"')
     wd.add_command = "git add ."
     wd.commit_command = "git commit -m test-{reason}"
     return wd
@@ -95,14 +97,57 @@
     wd.write("pyproject.toml", PYPROJECT_FILES[metadata_in])
     wd.write("setup.py", SETUP_PY_FILES[metadata_in])
     wd.write("setup.cfg", SETUP_CFG_FILES[metadata_in])
     res = wd([sys.executable, "setup.py", "--version"])
     assert res.endswith("0.1.dev0+d20090213")
 
 
+@pytest.mark.parametrize("use_scm_version", ["True", "{}", "lambda: {}"])
+def test_pyproject_missing_setup_hook_works(wd: WorkDir, use_scm_version: str) -> None:
+    wd.write(
+        "setup.py",
+        f"""__import__('setuptools').setup(
+    name="example-scm-unique",
+    use_scm_version={use_scm_version},
+    )""",
+    )
+    wd.write(
+        "pyproject.toml",
+        textwrap.dedent(
+            """
+            [build-system]
+            requires=["setuptools", "setuptools_scm"]
+            build-backend = "setuptools.build_meta"
+            [tool]
+            """
+        ),
+    )
+
+    res = subprocess.run(
+        [sys.executable, "setup.py", "--version"],
+        cwd=wd.cwd,
+        check=True,
+        stdout=subprocess.PIPE,
+        encoding="utf-8",
+    )
+    stripped = res.stdout.strip()
+    assert stripped.endswith("0.1.dev0+d20090213")
+
+    res_build = subprocess.run(
+        [sys.executable, "-m", "build", "-nxw"],
+        env={k: v for k, v in os.environ.items() if k != "SETUPTOOLS_SCM_DEBUG"},
+        cwd=wd.cwd,
+    )
+    import pprint
+
+    pprint.pprint(res_build)
+    wheel: Path = next(wd.cwd.joinpath("dist").iterdir())
+    assert "0.1.dev0+d20090213" in str(wheel)
+
+
 def test_pretend_version(monkeypatch: pytest.MonkeyPatch, wd: WorkDir) -> None:
     monkeypatch.setenv(PRETEND_KEY, "1.0.0")
 
     assert wd.get_version() == "1.0.0"
     assert wd.get_version(dist_name="ignored") == "1.0.0"
```

### Comparing `setuptools-scm-8.0.3/testing/test_main.py` & `setuptools-scm-8.0.4/testing/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     )
     ns = {"__package__": "setuptools_scm"}
     with open(mainfile) as f:
         code = compile(f.read(), "__main__.py", "exec")
         exec(code, ns)
 
 
-@pytest.fixture
+@pytest.fixture()
 def repo(wd: WorkDir) -> WorkDir:
     wd("git init")
     wd("git config user.email user@host")
     wd("git config user.name user")
     wd.add_command = "git add ."
     wd.commit_command = "git commit -m test-{reason}"
```

### Comparing `setuptools-scm-8.0.3/testing/test_mercurial.py` & `setuptools-scm-8.0.4/testing/test_mercurial.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 pytestmark = pytest.mark.skipif(
     not has_command("hg", warn=False), reason="hg executable not found"
 )
 
 
-@pytest.fixture
+@pytest.fixture()
 def wd(wd: WorkDir) -> WorkDir:
     wd("hg init")
     wd.add_command = "hg add ."
     wd.commit_command = 'hg commit -m test-{reason} -u test -d "0 0"'
     return wd
 
 
@@ -37,15 +37,15 @@
     },
     "0.0": {"node": "0" * 20},
     "1.2.2": {"tag": "release-1.2.2"},
     "1.2.2.dev0": {"tag": "release-1.2.2.dev"},
 }
 
 
-@pytest.mark.parametrize("expected,data", sorted(archival_mapping.items()))
+@pytest.mark.parametrize(("expected", "data"), sorted(archival_mapping.items()))
 def test_archival_to_version(expected: str, data: dict[str, str]) -> None:
     config = Configuration(
         version_scheme="guess-next-dev", local_scheme="node-and-date"
     )
     version = archival_to_version(data, config=config)
     assert format_version(version) == expected
 
@@ -132,23 +132,23 @@
 @pytest.mark.issue(128)
 def test_parse_no_worktree(tmp_path: Path) -> None:
     config = Configuration()
     ret = parse(os.fspath(tmp_path), config)
     assert ret is None
 
 
-@pytest.fixture
+@pytest.fixture()
 def version_1_0(wd: WorkDir) -> WorkDir:
     wd("hg branch default")
     wd.commit_testfile()
     wd('hg tag 1.0.0 -u test -d "0 0"')
     return wd
 
 
-@pytest.fixture
+@pytest.fixture()
 def pre_merge_commit_after_tag(version_1_0: WorkDir) -> WorkDir:
     wd = version_1_0
     wd("hg branch testbranch")
     wd.write("branchfile", "branchtext")
     wd(wd.add_command)
     wd.commit()
     wd("hg update default")
```

### Comparing `setuptools-scm-8.0.3/testing/test_regressions.py` & `setuptools-scm-8.0.4/testing/test_regressions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import pprint
 import subprocess
 import sys
+from dataclasses import replace
 from importlib.metadata import distribution
 from importlib.metadata import EntryPoint
 from pathlib import Path
 
 import pytest
 
 from setuptools_scm import Configuration
 from setuptools_scm._run_cmd import run
 from setuptools_scm.git import parse
 from setuptools_scm.integration import data_from_mime
+from setuptools_scm.version import meta
 
 
 def test_data_from_mime_ignores_body() -> None:
     assert data_from_mime(
         "test",
         "version: 1.0\r\n\r\nversion: bad",
     ) == {"version": "1.0"}
@@ -100,7 +102,25 @@
     for ep in eps:
         try:
             ep.load()
         except Exception as e:
             failed.append((ep, e))
     if failed:
         pytest.fail(pprint.pformat(failed))
+
+
+def test_write_to_absolute_path_passes_when_subdir_of_root(tmp_path: Path) -> None:
+    c = Configuration(root=tmp_path, write_to=tmp_path / "VERSION.py")
+    v = meta("1.0", config=c)
+    from setuptools_scm._get_version_impl import write_version_files
+
+    with pytest.warns(DeprecationWarning, match=".*write_to=.* is a absolute.*"):
+        write_version_files(c, "1.0", v)
+    write_version_files(replace(c, write_to="VERSION.py"), "1.0", v)
+    subdir = tmp_path / "subdir"
+    subdir.mkdir()
+    with pytest.raises(
+        # todo: python version specific error list
+        ValueError,
+        match=".*VERSION.py' .* .*subdir.*",
+    ):
+        write_version_files(replace(c, root=subdir), "1.0", v)
```

### Comparing `setuptools-scm-8.0.3/testing/test_version.py` & `setuptools-scm-8.0.4/testing/test_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 c = Configuration()
 c_non_normalize = Configuration(version_cls=NonNormalizedVersion)
 
 
 @pytest.mark.parametrize(
-    "version, expected_next",
+    ("version", "expected_next"),
     [
         pytest.param(meta("1.0.0", config=c), "1.0.0", id="exact"),
         pytest.param(meta("1.0", config=c), "1.0.0", id="short_tag"),
         pytest.param(
             meta("1.0.0", distance=2, branch="default", config=c),
             "1.0.1.dev2",
             id="normal_branch",
@@ -66,15 +66,15 @@
     with pytest.raises(
         ValueError, match=r"1\.0\.0-foo.* can't be parsed as numeric version"
     ):
         simplified_semver_version(version)
 
 
 @pytest.mark.parametrize(
-    "version, expected_next",
+    ("version", "expected_next"),
     [
         pytest.param(meta("1.0.0", config=c), "1.0.0", id="exact"),
         pytest.param(
             meta("1.0.0", distance=2, branch="master", config=c),
             "1.1.0.dev2",
             id="development_branch",
         ),
@@ -111,15 +111,15 @@
 
 
 def m(tag: str, **kw: Any) -> ScmVersion:
     return meta(tag, **kw, config=c)
 
 
 @pytest.mark.parametrize(
-    "version, expected_next",
+    ("version", "expected_next"),
     [
         pytest.param(
             m("1.0.0", distance=2),
             "1.0.0.post1.dev2",
             id="dev_distance",
         ),
         pytest.param(
@@ -139,15 +139,15 @@
 )
 def test_no_guess_version(version: ScmVersion, expected_next: str) -> None:
     computed = no_guess_dev_version(version)
     assert computed == expected_next
 
 
 @pytest.mark.parametrize(
-    "version, match",
+    ("version", "match"),
     [
         ("1.0.dev1", "choosing custom numbers for the `.devX` distance"),
         ("1.0.post1", "already is a post release"),
     ],
 )
 def test_no_guess_version_bad(version: str, match: str) -> None:
     with pytest.raises(ValueError, match=match):
@@ -155,27 +155,27 @@
 
 
 def test_bump_dev_version_zero() -> None:
     assert guess_next_version(m("1.0.dev0")) == "1.0"
 
 
 def test_bump_dev_version_nonzero_raises() -> None:
-    with pytest.raises(ValueError) as excinfo:
-        guess_next_version(m("1.0.dev1"))
-
-    assert str(excinfo.value) == (
+    match = (
         "choosing custom numbers for the `.devX` distance "
         "is not supported.\n "
         "The 1.0.dev1 can't be bumped\n"
         "Please drop the tag or create a new supported one ending in .dev0"
     )
 
+    with pytest.raises(ValueError, match=match):
+        guess_next_version(m("1.0.dev1"))
+
 
 @pytest.mark.parametrize(
-    "tag, expected",
+    ("tag", "expected"),
     [
         ("v1.0.0", "1.0.0"),
         ("v1.0.0-rc.1", "1.0.0rc1"),
         ("v1.0.0-rc.1+-25259o4382757gjurh54", "1.0.0rc1"),
     ],
 )
 def test_tag_regex1(tag: str, expected: str) -> None:
@@ -190,15 +190,15 @@
 
 
 @pytest.mark.issue("https://github.com/pypa/setuptools_scm/issues/471")
 def test_version_bump_bad() -> None:
     class YikesVersion:
         val: str
 
-        def __init__(self, val: str):
+        def __init__(self, val: str) -> None:
             self.val = val
 
         def __str__(self) -> str:
             return self.val
 
     config = Configuration(version_cls=YikesVersion)  # type: ignore[arg-type]
     with pytest.raises(
@@ -250,15 +250,15 @@
     days_offset: int = 0,
     fmt: str = "%y.%m.%d",
 ) -> str:
     return format(date_offset(base_date, days_offset), fmt)
 
 
 @pytest.mark.parametrize(
-    "version, expected_next",
+    ("version", "expected_next"),
     [
         pytest.param(
             meta(date_to_str(days_offset=3), config=c_non_normalize),
             date_to_str(days_offset=3),
             id="exact",
         ),
         pytest.param(
@@ -342,15 +342,15 @@
 )
 def test_calver_by_date(version: ScmVersion, expected_next: str) -> None:
     computed = calver_by_date(version)
     assert computed == expected_next
 
 
 @pytest.mark.parametrize(
-    "version, expected_next",
+    ("version", "expected_next"),
     [
         pytest.param(meta("1.0.0", config=c), "1.0.0", id="SemVer exact stays"),
         pytest.param(
             meta("1.0.0", config=c_non_normalize, dirty=True),
             "09.02.13.1.dev0",
             id="SemVer dirty is replaced by date",
             marks=pytest.mark.filterwarnings("ignore:.*legacy version.*:UserWarning"),
@@ -366,15 +366,15 @@
     with pytest.warns(UserWarning, match="your previous tag*"):
         calver_by_date(
             meta(date_to_str(days_offset=-2), config=c_non_normalize, distance=2)
         )
 
 
 @pytest.mark.parametrize(
-    ["tag", "node_date", "expected"],
+    ("tag", "node_date", "expected"),
     [
         pytest.param("20.03.03", date(2020, 3, 4), "20.03.04.0", id="next day"),
         pytest.param("20.03.03", date(2020, 3, 3), "20.03.03.1", id="same day"),
         pytest.param(
             "20.03.03.2", date(2020, 3, 3), "20.03.03.3", id="same day with patch"
         ),
         pytest.param(
@@ -392,15 +392,15 @@
     assert next == expected
 
 
 def test_custom_version_cls() -> None:
     """Test that we can pass our own version class instead of pkg_resources"""
 
     class MyVersion:
-        def __init__(self, tag_str: str):
+        def __init__(self, tag_str: str) -> None:
             self.tag = tag_str
 
         def __str__(self) -> str:
             return "Custom %s" % self.tag
 
         def __repr__(self) -> str:
             return "MyVersion<Custom%s>" % self.tag
```

### Comparing `setuptools-scm-8.0.3/testing/wd_wrapper.py` & `setuptools-scm-8.0.4/testing/wd_wrapper.py`

 * *Files identical despite different names*

