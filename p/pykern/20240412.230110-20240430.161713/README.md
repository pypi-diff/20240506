# Comparing `tmp/pykern-20240412.230110.tar.gz` & `tmp/pykern-20240430.161713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykern-20240412.230110.tar", last modified: Tue Apr 16 16:23:09 2024, max compression
+gzip compressed data, was "pykern-20240430.161713.tar", last modified: Tue Apr 30 16:58:26 2024, max compression
```

## Comparing `pykern-20240412.230110.tar` & `pykern-20240430.161713.tar`

### file list

```diff
@@ -1,463 +1,463 @@
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.350607 pykern-20240412.230110/
--rw-r-----   0 root         (0) root         (0)    11324 2018-02-06 22:51:04.000000 pykern-20240412.230110/LICENSE
--rw-r-----   0 root         (0) root         (0)      182 2024-03-19 18:50:32.000000 pykern-20240412.230110/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-16 16:23:09.350607 pykern-20240412.230110/PKG-INFO
--rw-r-----   0 root         (0) root         (0)      264 2024-03-20 14:13:19.000000 pykern-20240412.230110/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.273606 pykern-20240412.230110/docs/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240412.230110/docs/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.274606 pykern-20240412.230110/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/docs/_static/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.274606 pykern-20240412.230110/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/docs/_templates/.gitignore
--rw-r-----   0 root         (0) root         (0)      365 2018-02-06 22:51:04.000000 pykern-20240412.230110/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.281606 pykern-20240412.230110/pykern/
--rw-r-----   0 root         (0) root         (0)      354 2024-03-20 14:13:19.000000 pykern-20240412.230110/pykern/__init__.py
--rw-r-----   0 root         (0) root         (0)    17824 2023-10-20 20:51:58.000000 pykern-20240412.230110/pykern/fconf.py
--rw-r-----   0 root         (0) root         (0)     1029 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/mpi.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.283606 pykern-20240412.230110/pykern/package_data/
--rw-r-----   0 root         (0) root         (0)     9727 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/docs-conf.py.format
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.284606 pykern-20240412.230110/pykern/package_data/projex/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.250606 pykern-20240412.230110/pykern/package_data/projex/.github/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.286606 pykern-20240412.230110/pykern/package_data/projex/.github/workflows/
--rw-r-----   0 root         (0) root         (0)      281 2022-07-20 23:21:19.000000 pykern-20240412.230110/pykern/package_data/projex/.github/workflows/python-ci.yml.jinja
--rw-r-----   0 root         (0) root         (0)      221 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/README.md.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.286606 pykern-20240412.230110/pykern/package_data/projex/docs/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.287606 pykern-20240412.230110/pykern/package_data/projex/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/docs/_static/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.287606 pykern-20240412.230110/pykern/package_data/projex/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/docs/_templates/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/docs/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)      207 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/docs/index.rst.jinja
--rw-r-----   0 root         (0) root         (0)      772 2022-02-12 15:07:54.000000 pykern-20240412.230110/pykern/package_data/projex/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.287606 pykern-20240412.230110/pykern/package_data/projex/projex/
--rw-r-----   0 root         (0) root         (0)      296 2022-10-24 20:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/projex/__init__.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.288607 pykern-20240412.230110/pykern/package_data/projex/projex/package_data/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/projex/package_data/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.288607 pykern-20240412.230110/pykern/package_data/projex/projex/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/projex/pkcli/__init__.py.jinja
--rw-r-----   0 root         (0) root         (0)      298 2022-10-24 20:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/projex/projex_console.py.jinja
--rw-r-----   0 root         (0) root         (0)      578 2022-10-24 20:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/setup.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.288607 pykern-20240412.230110/pykern/package_data/projex/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/tests/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)      228 2022-10-24 20:51:04.000000 pykern-20240412.230110/pykern/package_data/projex/tests/import_test.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.286606 pykern-20240412.230110/pykern/package_data/projex-licenses/
--rw-r-----   0 root         (0) root         (0)    34520 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/agpl-3.0.txt
--rw-r-----   0 root         (0) root         (0)    11358 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/apache2.jinja
--rw-r-----   0 root         (0) root         (0)    18092 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/gpl2.jinja
--rw-r-----   0 root         (0) root         (0)    35147 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/gpl3.jinja
--rw-r-----   0 root         (0) root         (0)    25383 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/lgpl2.jinja
--rw-r-----   0 root         (0) root         (0)     7651 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/lgpl3.jinja
--rw-r-----   0 root         (0) root         (0)     1085 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/mit.jinja
--rw-r-----   0 root         (0) root         (0)      191 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/projex-licenses/proprietary.jinja
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/pykern/package_data/test.yml
--rw-r-----   0 root         (0) root         (0)     1169 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkarray.py
--rw-r-----   0 root         (0) root         (0)     2845 2024-03-15 14:11:15.000000 pykern-20240412.230110/pykern/pkasyncio.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.291607 pykern-20240412.230110/pykern/pkcli/
--rw-r-----   0 root         (0) root         (0)    10485 2024-03-15 14:11:15.000000 pykern-20240412.230110/pykern/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)     4170 2024-03-20 14:13:19.000000 pykern-20240412.230110/pykern/pkcli/ci.py
--rw-r-----   0 root         (0) root         (0)     1763 2022-12-28 15:07:11.000000 pykern-20240412.230110/pykern/pkcli/fmt.py
--rw-r-----   0 root         (0) root         (0)    20449 2024-03-15 14:11:15.000000 pykern-20240412.230110/pykern/pkcli/github.py
--rw-r-----   0 root         (0) root         (0)    12793 2022-10-31 19:53:53.000000 pykern-20240412.230110/pykern/pkcli/github_orgmode.py
--rw-r-----   0 root         (0) root         (0)     2849 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkcli/pkexample.py
--rw-r-----   0 root         (0) root         (0)     4773 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkcli/projex.py
--rw-r-----   0 root         (0) root         (0)     2962 2024-04-13 14:11:29.000000 pykern-20240412.230110/pykern/pkcli/rsmanifest.py
--rw-r-----   0 root         (0) root         (0)     6686 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkcli/sim.py
--rw-r-----   0 root         (0) root         (0)     7427 2024-04-06 14:13:17.000000 pykern-20240412.230110/pykern/pkcli/test.py
--rw-r-----   0 root         (0) root         (0)    12808 2024-04-13 14:11:29.000000 pykern-20240412.230110/pykern/pkcollections.py
--rw-r-----   0 root         (0) root         (0)     3686 2023-09-13 14:10:24.000000 pykern-20240412.230110/pykern/pkcompat.py
--rw-r-----   0 root         (0) root         (0)    24232 2023-10-20 20:51:58.000000 pykern-20240412.230110/pykern/pkconfig.py
--rw-r-----   0 root         (0) root         (0)     1221 2024-03-28 17:40:02.000000 pykern-20240412.230110/pykern/pkconst.py
--rw-r-----   0 root         (0) root         (0)    22756 2024-01-19 15:11:21.000000 pykern-20240412.230110/pykern/pkdebug.py
--rw-r-----   0 root         (0) root         (0)     4591 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkexample.py
--rw-r-----   0 root         (0) root         (0)     8826 2024-01-19 15:11:21.000000 pykern-20240412.230110/pykern/pkinspect.py
--rw-r-----   0 root         (0) root         (0)    10253 2024-02-01 15:11:17.000000 pykern-20240412.230110/pykern/pkio.py
--rw-r-----   0 root         (0) root         (0)     1857 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkjinja.py
--rw-r-----   0 root         (0) root         (0)     3152 2024-04-13 14:11:29.000000 pykern-20240412.230110/pykern/pkjson.py
--rw-r-----   0 root         (0) root         (0)     1427 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkplatform.py
--rw-r-----   0 root         (0) root         (0)     3214 2024-03-28 17:40:02.000000 pykern-20240412.230110/pykern/pkresource.py
--rw-r-----   0 root         (0) root         (0)      774 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pkrunpy.py
--rw-r-----   0 root         (0) root         (0)    22115 2024-03-28 17:40:02.000000 pykern-20240412.230110/pykern/pksetup.py
--rw-r-----   0 root         (0) root         (0)     4287 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pksubprocess.py
--rw-r-----   0 root         (0) root         (0)    25421 2024-03-20 14:13:19.000000 pykern-20240412.230110/pykern/pkunit.py
--rw-r-----   0 root         (0) root         (0)     2578 2022-07-12 14:07:33.000000 pykern-20240412.230110/pykern/pkyaml.py
--rw-r-----   0 root         (0) root         (0)      421 2022-06-24 14:08:21.000000 pykern-20240412.230110/pykern/pykern_console.py
--rw-r-----   0 root         (0) root         (0)      180 2024-03-20 14:13:19.000000 pykern-20240412.230110/pykern/pytest_plugin.py
--rw-r-----   0 root         (0) root         (0)      404 2022-09-26 20:14:13.000000 pykern-20240412.230110/pykern/quest.py
--rw-r-----   0 root         (0) root         (0)     3756 2024-03-15 14:11:15.000000 pykern-20240412.230110/pykern/util.py
--rw-r-----   0 root         (0) root         (0)    23884 2023-09-25 14:09:48.000000 pykern-20240412.230110/pykern/xlsx.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.349607 pykern-20240412.230110/pykern.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/PKG-INFO
--rw-r-----   0 root         (0) root         (0)    11319 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/SOURCES.txt
--rw-r-----   0 root         (0) root         (0)        1 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/dependency_links.txt
--rw-r-----   0 root         (0) root         (0)       54 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/entry_points.txt
--rw-r-----   0 root         (0) root         (0)      376 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/requires.txt
--rw-r-----   0 root         (0) root         (0)        7 2024-04-16 16:23:09.000000 pykern-20240412.230110/pykern.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)     1455 2024-04-02 19:05:05.000000 pykern-20240412.230110/pyproject.toml
--rw-r-----   0 root         (0) root         (0)       38 2024-04-16 16:23:09.350607 pykern-20240412.230110/setup.cfg
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.300607 pykern-20240412.230110/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)      554 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/conftest.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.253606 pykern-20240412.230110/tests/fconf_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.301607 pykern-20240412.230110/tests/fconf_data/1.in/
--rw-r-----   0 root         (0) root         (0)      450 2022-07-18 15:54:21.000000 pykern-20240412.230110/tests/fconf_data/1.in/0.py
--rw-r-----   0 root         (0) root         (0)      883 2022-07-18 15:54:21.000000 pykern-20240412.230110/tests/fconf_data/1.in/1.yml
--rw-r-----   0 root         (0) root         (0)       57 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/1.in/2.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.301607 pykern-20240412.230110/tests/fconf_data/1.out/
--rw-r-----   0 root         (0) root         (0)     1647 2022-07-18 15:54:21.000000 pykern-20240412.230110/tests/fconf_data/1.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.301607 pykern-20240412.230110/tests/fconf_data/2.in/
--rw-r-----   0 root         (0) root         (0)      139 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/2.in/1.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.302606 pykern-20240412.230110/tests/fconf_data/2.out/
--rw-r-----   0 root         (0) root         (0)      374 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/2.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.302606 pykern-20240412.230110/tests/fconf_data/3.in/
--rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/3.in/0.py
--rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/3.in/1.py
--rw-r-----   0 root         (0) root         (0)       11 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/3.in/2.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.303607 pykern-20240412.230110/tests/fconf_data/3.out/
--rw-r-----   0 root         (0) root         (0)      118 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_data/3.out/res.json
--rw-r-----   0 root         (0) root         (0)      602 2022-07-07 14:08:03.000000 pykern-20240412.230110/tests/fconf_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.303607 pykern-20240412.230110/tests/mpi_data/
--rw-r-----   0 root         (0) root         (0)      925 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/mpi_data/p1.py
--rw-r-----   0 root         (0) root         (0)     1307 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/mpi_test.py
--rw-r-----   0 root         (0) root         (0)      885 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkarray_test.py
--rw-r-----   0 root         (0) root         (0)     2633 2024-01-19 15:11:21.000000 pykern-20240412.230110/tests/pkasyncio_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.306607 pykern-20240412.230110/tests/pkcli/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.254606 pykern-20240412.230110/tests/pkcli/ci1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.306607 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.306607 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/.x/
--rw-r-----   0 root         (0) root         (0)       61 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/.x/x.py
--rw-r-----   0 root         (0) root         (0)       34 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.307607 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/somepkg/
--rw-r-----   0 root         (0) root         (0)        8 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/somepkg/has_print.py
--rw-r-----   0 root         (0) root         (0)       14 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/somepkg/ok.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.307607 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/somepkg/package_data/
--rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/somepkg/package_data/not_checked.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.254606 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/tests/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.307607 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/tests/test_data/
--rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.in/tests/test_data/not_checked.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.307607 pykern-20240412.230110/tests/pkcli/ci1_data/1.out/
--rw-r-----   0 root         (0) root         (0)       45 2022-10-22 14:07:30.000000 pykern-20240412.230110/tests/pkcli/ci1_data/1.out/pkexcept
--rw-r-----   0 root         (0) root         (0)      428 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkcli/ci1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.257606 pykern-20240412.230110/tests/pkcli/ci_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.308606 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-1.in/
--rw-r-----   0 root         (0) root         (0)       36 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.308606 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-1.out/
--rw-r-----   0 root         (0) root         (0)       24 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.308606 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-2.in/
--rw-r-----   0 root         (0) root         (0)       45 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.308606 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_eof_newline-2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.309607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.309607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.in/run/
--rw-r-----   0 root         (0) root         (0)       27 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.in/run/ignored.py
--rw-r-----   0 root         (0) root         (0)      191 2022-11-17 18:34:08.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.309607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.out/
--rw-r-----   0 root         (0) root         (0)      148 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.309607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-2.in/
--rw-r-----   0 root         (0) root         (0)      208 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.310607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.310607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-3.in/
--rw-r-----   0 root         (0) root         (0)       87 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-3.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.310607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-3.out/
--rw-r-----   0 root         (0) root         (0)       82 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-3.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.310607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-4.in/
--rw-r-----   0 root         (0) root         (0)       10 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-4.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.311607 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-4.out/
--rw-r-----   0 root         (0) root         (0)       31 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/check_prints-4.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.311607 pykern-20240412.230110/tests/pkcli/ci_data/run-1.in/
--rw-r-----   0 root         (0) root         (0)       20 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/run-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.311607 pykern-20240412.230110/tests/pkcli/ci_data/run-1.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/run-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.311607 pykern-20240412.230110/tests/pkcli/ci_data/run-2.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.312606 pykern-20240412.230110/tests/pkcli/ci_data/run-2.in/tests/
--rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/run-2.in/tests/x_test.py
--rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/run-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.312606 pykern-20240412.230110/tests/pkcli/ci_data/run-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_data/run-2.out/pkexcept
--rw-r-----   0 root         (0) root         (0)      400 2022-11-17 18:34:09.000000 pykern-20240412.230110/tests/pkcli/ci_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.259606 pykern-20240412.230110/tests/pkcli/fmt_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.312606 pykern-20240412.230110/tests/pkcli/fmt_data/check1.in/
--rw-r-----   0 root         (0) root         (0)       44 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/check1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.312606 pykern-20240412.230110/tests/pkcli/fmt_data/check1.out/
--rw-r-----   0 root         (0) root         (0)       39 2022-12-28 15:07:11.000000 pykern-20240412.230110/tests/pkcli/fmt_data/check1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.312606 pykern-20240412.230110/tests/pkcli/fmt_data/check2.in/
--rw-r-----   0 root         (0) root         (0)       56 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/check2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.313607 pykern-20240412.230110/tests/pkcli/fmt_data/check2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240412.230110/tests/pkcli/fmt_data/check2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.313607 pykern-20240412.230110/tests/pkcli/fmt_data/diff.in/
--rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/diff.in/file1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.313607 pykern-20240412.230110/tests/pkcli/fmt_data/diff.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240412.230110/tests/pkcli/fmt_data/diff.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.313607 pykern-20240412.230110/tests/pkcli/fmt_data/diff2.in/
--rw-r-----   0 root         (0) root         (0)      368 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/diff2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.314607 pykern-20240412.230110/tests/pkcli/fmt_data/diff2.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-06-18 14:08:41.000000 pykern-20240412.230110/tests/pkcli/fmt_data/diff2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.314607 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.in/
--rw-r-----   0 root         (0) root         (0)      170 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.in/file1.py
--rw-r-----   0 root         (0) root         (0)      483 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.in/y.py
--rw-r-----   0 root         (0) root         (0)      244 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.in/z.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.315606 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.out/
--rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.out/file1.py
--rw-r-----   0 root         (0) root         (0)      584 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.out/y.py
--rw-r-----   0 root         (0) root         (0)      324 2022-06-14 14:07:59.000000 pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.out/z.py
--rw-r-----   0 root         (0) root         (0)      798 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkcli/fmt_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.260606 pykern-20240412.230110/tests/pkcli/github_orgmode_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.315606 pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.in/
--rw-r-----   0 root         (0) root         (0)    20455 2022-10-11 14:09:00.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.316607 pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.out/
--rw-r-----   0 root         (0) root         (0)     1301 2022-10-15 14:08:58.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.316607 pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.in/
--rw-r-----   0 root         (0) root         (0)    21657 2022-10-11 14:09:00.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.316607 pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.out/
--rw-r-----   0 root         (0) root         (0)     1056 2022-10-15 14:08:58.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.317607 pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.in/
--rw-r-----   0 root         (0) root         (0)     2922 2022-10-11 14:09:00.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json
--rw-r-----   0 root         (0) root         (0)     1264 2022-10-11 14:09:00.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.317607 pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.out/
--rw-r-----   0 root         (0) root         (0)      933 2022-10-11 14:09:00.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json
--rw-r-----   0 root         (0) root         (0)     2312 2022-10-31 19:53:53.000000 pykern-20240412.230110/tests/pkcli/github_orgmode_test.py
--rw-r-----   0 root         (0) root         (0)     4988 2024-03-15 14:11:15.000000 pykern-20240412.230110/tests/pkcli/github_test.py
--rw-r-----   0 root         (0) root         (0)     2923 2023-08-16 14:09:51.000000 pykern-20240412.230110/tests/pkcli/projex_test.py
--rw-r-----   0 root         (0) root         (0)     1995 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkcli/rsmanifest_test.py
--rw-r-----   0 root         (0) root         (0)     1816 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkcli/sim_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.260606 pykern-20240412.230110/tests/pkcli/test1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.317607 pykern-20240412.230110/tests/pkcli/test1_data/tests/
--rw-r-----   0 root         (0) root         (0)      293 2023-04-05 14:10:34.000000 pykern-20240412.230110/tests/pkcli/test1_data/tests/always_test.py
--rw-r-----   0 root         (0) root         (0)      461 2023-04-05 14:10:34.000000 pykern-20240412.230110/tests/pkcli/test1_data/tests/twice_test.py
--rw-r-----   0 root         (0) root         (0)      653 2023-04-05 14:10:34.000000 pykern-20240412.230110/tests/pkcli/test1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.261606 pykern-20240412.230110/tests/pkcli/test2_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.317607 pykern-20240412.230110/tests/pkcli/test2_data/1.in/
--rw-r-----   0 root         (0) root         (0)      338 2023-10-16 19:47:54.000000 pykern-20240412.230110/tests/pkcli/test2_data/1.in/coroutine_test.py
--rw-r-----   0 root         (0) root         (0)      685 2024-04-06 14:13:17.000000 pykern-20240412.230110/tests/pkcli/test2_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.261606 pykern-20240412.230110/tests/pkcli/test_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.318606 pykern-20240412.230110/tests/pkcli/test_data/tests/
--rw-r-----   0 root         (0) root         (0)      277 2019-12-04 23:50:51.000000 pykern-20240412.230110/tests/pkcli/test_data/tests/1_test.py
--rw-r-----   0 root         (0) root         (0)      282 2019-12-04 23:50:51.000000 pykern-20240412.230110/tests/pkcli/test_data/tests/2_test.py
--rw-r-----   0 root         (0) root         (0)      327 2024-02-13 15:11:30.000000 pykern-20240412.230110/tests/pkcli/test_data/tests/3_test.py
--rw-r-----   0 root         (0) root         (0)     2463 2024-02-13 15:11:30.000000 pykern-20240412.230110/tests/pkcli/test_test.py
--rw-r-----   0 root         (0) root         (0)      597 2022-06-30 14:07:51.000000 pykern-20240412.230110/tests/pkcli1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.262606 pykern-20240412.230110/tests/pkcli_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.318606 pykern-20240412.230110/tests/pkcli_data/arghparsing/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/arghparsing/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.319607 pykern-20240412.230110/tests/pkcli_data/arghparsing/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/arghparsing/pkcli/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.319607 pykern-20240412.230110/tests/pkcli_data/command_info.in/
--rw-r-----   0 root         (0) root         (0)      140 2022-10-04 14:08:26.000000 pykern-20240412.230110/tests/pkcli_data/command_info.in/example_pkcli_module.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.319607 pykern-20240412.230110/tests/pkcli_data/command_info.out/
--rw-r-----   0 root         (0) root         (0)       17 2022-10-04 14:08:26.000000 pykern-20240412.230110/tests/pkcli_data/command_info.out/example_stderr.out
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.319607 pykern-20240412.230110/tests/pkcli_data/package1/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.320607 pykern-20240412.230110/tests/pkcli_data/package1/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package1/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      366 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package1/pkcli/conf1.py
--rw-r-----   0 root         (0) root         (0)      178 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package1/pkcli/conf2.py
--rw-r-----   0 root         (0) root         (0)      219 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package1/pkcli/conf3.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.321606 pykern-20240412.230110/tests/pkcli_data/package2/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package2/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.321606 pykern-20240412.230110/tests/pkcli_data/package2/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package2/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      310 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package2/pkcli/argh_test.py
--rw-r-----   0 root         (0) root         (0)      195 2023-12-07 23:37:10.000000 pykern-20240412.230110/tests/pkcli_data/package2/pkcli/some_mod.py
--rw-r-----   0 root         (0) root         (0)     4879 2024-03-15 14:11:15.000000 pykern-20240412.230110/tests/pkcli_test.py
--rw-r-----   0 root         (0) root         (0)     6806 2024-04-13 14:11:29.000000 pykern-20240412.230110/tests/pkcollections_test.py
--rw-r-----   0 root         (0) root         (0)     2276 2023-09-13 14:10:24.000000 pykern-20240412.230110/tests/pkcompat_test.py
--rw-r-----   0 root         (0) root         (0)     1862 2023-03-14 17:59:06.000000 pykern-20240412.230110/tests/pkconfig1_test.py
--rw-r-----   0 root         (0) root         (0)     1175 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkconfig2_test.py
--rw-r-----   0 root         (0) root         (0)      868 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkconfig3_test.py
--rw-r-----   0 root         (0) root         (0)      754 2023-04-14 17:14:13.000000 pykern-20240412.230110/tests/pkconfig4_test.py
--rw-r-----   0 root         (0) root         (0)     1588 2023-04-14 17:14:13.000000 pykern-20240412.230110/tests/pkconfig5_test.py
--rw-r-----   0 root         (0) root         (0)      623 2023-04-14 17:14:13.000000 pykern-20240412.230110/tests/pkconfig6_test.py
--rw-r-----   0 root         (0) root         (0)      617 2023-04-14 17:14:13.000000 pykern-20240412.230110/tests/pkconfig7_test.py
--rw-r-----   0 root         (0) root         (0)      350 2023-04-23 14:08:30.000000 pykern-20240412.230110/tests/pkconfig8_test.py
--rw-r-----   0 root         (0) root         (0)      421 2023-10-20 20:51:58.000000 pykern-20240412.230110/tests/pkconfig9_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.263606 pykern-20240412.230110/tests/pkconfig_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.322607 pykern-20240412.230110/tests/pkconfig_data/p1/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkconfig_data/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      214 2023-10-20 20:51:58.000000 pykern-20240412.230110/tests/pkconfig_data/p1/append_error.py
--rw-r-----   0 root         (0) root         (0)      469 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkconfig_data/p1/base_pkconfig.py
--rw-r-----   0 root         (0) root         (0)     1984 2020-01-08 19:20:36.000000 pykern-20240412.230110/tests/pkconfig_data/p1/m1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.323607 pykern-20240412.230110/tests/pkconfig_data/p1/s1/
--rw-r-----   0 root         (0) root         (0)        2 2019-11-17 13:40:26.000000 pykern-20240412.230110/tests/pkconfig_data/p1/s1/__init__.py
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkconfig_data/p1/s1/m11.py
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkconfig_data/p1/s1/m12.py
--rw-r-----   0 root         (0) root         (0)    10382 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkdebug1_test.py
--rw-r-----   0 root         (0) root         (0)     1870 2023-08-16 14:09:51.000000 pykern-20240412.230110/tests/pkdebug2_test.py
--rw-r-----   0 root         (0) root         (0)     1737 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkexample_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.263606 pykern-20240412.230110/tests/pkinspect_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.323607 pykern-20240412.230110/tests/pkinspect_data/p1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkinspect_data/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      326 2021-02-16 00:17:58.000000 pykern-20240412.230110/tests/pkinspect_data/p1/m1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.324607 pykern-20240412.230110/tests/pkinspect_data/p1/p2/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkinspect_data/p1/p2/__init__.py
--rw-r-----   0 root         (0) root         (0)       35 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkinspect_data/p1/p2/m2.py
--rw-r-----   0 root         (0) root         (0)     3979 2024-01-19 15:11:21.000000 pykern-20240412.230110/tests/pkinspect_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.325607 pykern-20240412.230110/tests/pkio_data/
--rw-r-----   0 root         (0) root         (0)   239616 2024-02-01 15:11:17.000000 pykern-20240412.230110/tests/pkio_data/binary.dat
--rw-r-----   0 root         (0) root         (0)       18 2024-02-01 15:11:17.000000 pykern-20240412.230110/tests/pkio_data/text.dat
--rw-r-----   0 root         (0) root         (0)     7132 2024-03-15 14:11:15.000000 pykern-20240412.230110/tests/pkio_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.325607 pykern-20240412.230110/tests/pkjinja_data/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkjinja_data/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.325607 pykern-20240412.230110/tests/pkjinja_data/package_data/
--rw-r-----   0 root         (0) root         (0)       12 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkjinja_data/package_data/t1.jinja
--rw-r-----   0 root         (0) root         (0)      211 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkjinja_data/t1.py
--rw-r-----   0 root         (0) root         (0)      997 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkjinja_test.py
--rw-r-----   0 root         (0) root         (0)     1965 2024-04-13 14:11:29.000000 pykern-20240412.230110/tests/pkjson_test.py
--rw-r-----   0 root         (0) root         (0)     1415 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkplatform_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.326607 pykern-20240412.230110/tests/pkresource_data/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkresource_data/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.326607 pykern-20240412.230110/tests/pkresource_data/package_data/
--rw-r-----   0 root         (0) root         (0)       14 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkresource_data/package_data/somefile
--rw-r-----   0 root         (0) root         (0)      189 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkresource_data/t1.py
--rw-r-----   0 root         (0) root         (0)     1309 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkresource_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.326607 pykern-20240412.230110/tests/pkrunpy_data/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkrunpy_data/f1.py
--rw-r-----   0 root         (0) root         (0)      533 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pkrunpy_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.266606 pykern-20240412.230110/tests/pksetup_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.327607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/
--rw-r-----   0 root         (0) root         (0)      738 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/.gitignore
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/LICENSE
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.328607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/docs/
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.328607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/examples/
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/examples/example1.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.329607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/__init__.py
--rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/base_pkconfig.py
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/mod1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.329607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/
--rw-r-----   0 root         (0) root         (0)       10 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/data1
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.329607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/__init__.py
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/mod2.py
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/requirements.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.330607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/scripts/
--rw-r-----   0 root         (0) root         (0)       25 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/scripts/script1
--rw-r-----   0 root         (0) root         (0)      295 2019-05-06 20:05:16.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.330607 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)       99 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/tests/mod1_test.py
--rw-r-----   0 root         (0) root         (0)      181 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit1/tests/mod2_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.332607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/
--rw-r-----   0 root         (0) root         (0)      756 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/.gitignore
--rw-r-----   0 root         (0) root         (0)      134 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/.travis.yml
--rw-r-----   0 root         (0) root         (0)    22102 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/LICENSE
--rw-r-----   0 root         (0) root         (0)      302 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.332607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.333607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/_static/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.333607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/_templates/.gitignore
--rw-r-----   0 root         (0) root         (0)      227 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.334607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/__init__.py
--rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/base_pkconfig.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.334607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.334607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      466 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/pksetupunit2/pksetupunit2_console.py
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/requirements.txt
--rw-r-----   0 root         (0) root         (0)     1051 2019-05-06 20:05:16.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.334607 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)      321 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pksetup_data/pksetupunit2/tests/simple_test.py
--rw-r-----   0 root         (0) root         (0)     5098 2023-04-04 14:10:19.000000 pykern-20240412.230110/tests/pksetup_test.py
--rw-r-----   0 root         (0) root         (0)     3892 2022-06-24 14:08:21.000000 pykern-20240412.230110/tests/pksubprocess_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.268606 pykern-20240412.230110/tests/pkunit1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.335607 pykern-20240412.230110/tests/pkunit1_data/bytes-1.in/
--rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240412.230110/tests/pkunit1_data/bytes-1.in/dot.gif
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.335607 pykern-20240412.230110/tests/pkunit1_data/bytes-1.out/
--rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240412.230110/tests/pkunit1_data/bytes-1.out/dot.gif
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.335607 pykern-20240412.230110/tests/pkunit1_data/conformance-1.in/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-1.in/in.txt
--rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-1.in/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.336607 pykern-20240412.230110/tests/pkunit1_data/conformance-1.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-1.out/in.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-1.out/out.txt
--rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-1.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.337607 pykern-20240412.230110/tests/pkunit1_data/conformance-2.in/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-2.in/in.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-2.in/out.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.337607 pykern-20240412.230110/tests/pkunit1_data/conformance-2.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/conformance-2.out/in.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.337607 pykern-20240412.230110/tests/pkunit1_data/curly_brackets.in/
--rw-r-----   0 root         (0) root         (0)       13 2022-09-20 14:07:49.000000 pykern-20240412.230110/tests/pkunit1_data/curly_brackets.in/sample.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.337607 pykern-20240412.230110/tests/pkunit1_data/curly_brackets.out/
--rw-r-----   0 root         (0) root         (0)        9 2022-09-20 14:07:49.000000 pykern-20240412.230110/tests/pkunit1_data/curly_brackets.out/sample.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.338607 pykern-20240412.230110/tests/pkunit1_data/deviance-1.in/
--rw-r-----   0 root         (0) root         (0)        0 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/deviance-1.in/not-used.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.338607 pykern-20240412.230110/tests/pkunit1_data/deviance-1.out/
--rw-r-----   0 root         (0) root         (0)        9 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/pkunit1_data/deviance-1.out/out.txt
--rw-r-----   0 root         (0) root         (0)     1449 2023-04-14 14:08:36.000000 pykern-20240412.230110/tests/pkunit1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.344607 pykern-20240412.230110/tests/pkunit_data/
--rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/actual_abs_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240412.230110/tests/pkunit_data/actual_conformance_2.ndiff
--rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/actual_default_conformance.ndiff
--rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/actual_default_conformance_1.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/actual_rel_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/actual_rel_ok_2.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkunit_data/assert1.json
--rw-r-----   0 root         (0) root         (0)       88 2022-08-23 22:15:42.000000 pykern-20240412.230110/tests/pkunit_data/different.bin
--rw-r-----   0 root         (0) root         (0)      543 2022-05-16 23:38:16.000000 pykern-20240412.230110/tests/pkunit_data/example.csv
--rw-r-----   0 root         (0) root         (0)     5425 2022-05-16 23:38:16.000000 pykern-20240412.230110/tests/pkunit_data/example.xlsx
--rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/expect_abs_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240412.230110/tests/pkunit_data/expect_conformance_2.ndiff
--rw-r-----   0 root         (0) root         (0)       52 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/expect_default_conformance.ndiff
--rw-r-----   0 root         (0) root         (0)       51 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/expect_default_conformance_1.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/expect_rel_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240412.230110/tests/pkunit_data/expect_rel_ok_2.ndiff
--rw-r-----   0 root         (0) root         (0)       20 2022-04-08 21:30:14.000000 pykern-20240412.230110/tests/pkunit_data/file_eq1.json
--rw-r-----   0 root         (0) root         (0)        0 2022-04-08 21:30:14.000000 pykern-20240412.230110/tests/pkunit_data/file_eq2.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-04-08 21:30:14.000000 pykern-20240412.230110/tests/pkunit_data/file_eq3.txt
--rw-r-----   0 root         (0) root         (0)       67 2022-08-25 16:28:29.000000 pykern-20240412.230110/tests/pkunit_data/ignore_lines.in
--rw-r-----   0 root         (0) root         (0)       68 2022-08-25 16:28:29.000000 pykern-20240412.230110/tests/pkunit_data/ignore_lines.out
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.269606 pykern-20240412.230110/tests/pkunit_data/import1/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.344607 pykern-20240412.230110/tests/pkunit_data/import1/p1/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkunit_data/import1/p1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.269606 pykern-20240412.230110/tests/pkunit_data/import2/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.344607 pykern-20240412.230110/tests/pkunit_data/import2/p1/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkunit_data/import2/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240412.230110/tests/pkunit_data/in.bin
--rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240412.230110/tests/pkunit_data/out.bin
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkunit_data/t1.yml
--rw-r-----   0 root         (0) root         (0)     8413 2023-10-30 22:15:18.000000 pykern-20240412.230110/tests/pkunit_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.344607 pykern-20240412.230110/tests/pkyaml_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.345607 pykern-20240412.230110/tests/pkyaml_data/1.in/
--rw-r-----   0 root         (0) root         (0)       65 2022-07-12 14:07:33.000000 pykern-20240412.230110/tests/pkyaml_data/1.in/in.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.345607 pykern-20240412.230110/tests/pkyaml_data/1.out/
--rw-r-----   0 root         (0) root         (0)       62 2022-07-12 14:07:33.000000 pykern-20240412.230110/tests/pkyaml_data/1.out/out.yml
--rw-r-----   0 root         (0) root         (0)       27 2020-09-03 15:51:30.000000 pykern-20240412.230110/tests/pkyaml_data/dump1.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.345607 pykern-20240412.230110/tests/pkyaml_data/p1/
--rw-r-----   0 root         (0) root         (0)       61 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkyaml_data/p1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.345607 pykern-20240412.230110/tests/pkyaml_data/p1/package_data/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240412.230110/tests/pkyaml_data/p1/package_data/conf2.yml
--rw-r-----   0 root         (0) root         (0)     1275 2022-07-12 14:07:33.000000 pykern-20240412.230110/tests/pkyaml_test.py
--rw-r-----   0 root         (0) root         (0)     1163 2024-02-01 15:11:17.000000 pykern-20240412.230110/tests/util_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.272606 pykern-20240412.230110/tests/xlsx_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.346607 pykern-20240412.230110/tests/xlsx_data/1.in/
--rw-r-----   0 root         (0) root         (0)      903 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/1.in/case.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.346607 pykern-20240412.230110/tests/xlsx_data/1.out/
--rw-r-----   0 root         (0) root         (0)       58 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/1.out/case1.csv
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.346607 pykern-20240412.230110/tests/xlsx_data/1.out/xl/
--rw-r-----   0 root         (0) root         (0)      281 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/1.out/xl/sharedStrings.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.346607 pykern-20240412.230110/tests/xlsx_data/1.out/xl/worksheets/
--rw-r-----   0 root         (0) root         (0)     1250 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.347607 pykern-20240412.230110/tests/xlsx_data/2.in/
--rw-r-----   0 root         (0) root         (0)     1057 2022-08-10 14:07:21.000000 pykern-20240412.230110/tests/xlsx_data/2.in/case.py
--rw-r-----   0 root         (0) root         (0)     6288 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/2.in/case2.xlsx
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.347607 pykern-20240412.230110/tests/xlsx_data/2.out/
--rw-r-----   0 root         (0) root         (0)       90 2022-08-10 14:07:21.000000 pykern-20240412.230110/tests/xlsx_data/2.out/case2#0.csv
--rw-r-----   0 root         (0) root         (0)        9 2022-06-03 23:08:48.000000 pykern-20240412.230110/tests/xlsx_data/2.out/case2#1.csv
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.348607 pykern-20240412.230110/tests/xlsx_data/2.out/xl/
--rw-r-----   0 root         (0) root         (0)      338 2022-08-10 14:07:21.000000 pykern-20240412.230110/tests/xlsx_data/2.out/xl/sharedStrings.xml
--rw-r-----   0 root         (0) root         (0)     1656 2023-03-14 17:59:06.000000 pykern-20240412.230110/tests/xlsx_data/2.out/xl/styles.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.348607 pykern-20240412.230110/tests/xlsx_data/2.out/xl/worksheets/
--rw-r-----   0 root         (0) root         (0)     1830 2023-01-16 15:07:03.000000 pykern-20240412.230110/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml
--rw-r-----   0 root         (0) root         (0)      795 2022-06-03 23:08:48.000000 pykern-20240412.230110/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.349607 pykern-20240412.230110/tests/xlsx_data/3.in/
--rw-r-----   0 root         (0) root         (0)      484 2022-08-02 14:08:07.000000 pykern-20240412.230110/tests/xlsx_data/3.in/case.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-16 16:23:09.349607 pykern-20240412.230110/tests/xlsx_data/3.out/
--rw-r-----   0 root         (0) root         (0)       38 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/xlsx_data/3.out/pkexcept
--rw-r-----   0 root         (0) root         (0)     1114 2022-08-06 14:07:18.000000 pykern-20240412.230110/tests/xlsx_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.946969 pykern-20240430.161713/
+-rw-r-----   0 root         (0) root         (0)    11324 2018-02-06 22:51:04.000000 pykern-20240430.161713/LICENSE
+-rw-r-----   0 root         (0) root         (0)      182 2024-03-19 18:50:32.000000 pykern-20240430.161713/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-30 16:58:26.945969 pykern-20240430.161713/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)      264 2024-03-20 14:13:19.000000 pykern-20240430.161713/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.809968 pykern-20240430.161713/docs/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240430.161713/docs/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.810968 pykern-20240430.161713/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/docs/_static/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.810968 pykern-20240430.161713/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/docs/_templates/.gitignore
+-rw-r-----   0 root         (0) root         (0)      365 2018-02-06 22:51:04.000000 pykern-20240430.161713/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.822968 pykern-20240430.161713/pykern/
+-rw-r-----   0 root         (0) root         (0)      354 2024-03-20 14:13:19.000000 pykern-20240430.161713/pykern/__init__.py
+-rw-r-----   0 root         (0) root         (0)    18196 2024-04-29 20:21:08.000000 pykern-20240430.161713/pykern/fconf.py
+-rw-r-----   0 root         (0) root         (0)     1029 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/mpi.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.825968 pykern-20240430.161713/pykern/package_data/
+-rw-r-----   0 root         (0) root         (0)     9727 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/docs-conf.py.format
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.826968 pykern-20240430.161713/pykern/package_data/projex/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.786968 pykern-20240430.161713/pykern/package_data/projex/.github/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.831968 pykern-20240430.161713/pykern/package_data/projex/.github/workflows/
+-rw-r-----   0 root         (0) root         (0)      281 2022-07-20 23:21:19.000000 pykern-20240430.161713/pykern/package_data/projex/.github/workflows/python-ci.yml.jinja
+-rw-r-----   0 root         (0) root         (0)      221 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/README.md.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.832968 pykern-20240430.161713/pykern/package_data/projex/docs/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.833968 pykern-20240430.161713/pykern/package_data/projex/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/docs/_static/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.833968 pykern-20240430.161713/pykern/package_data/projex/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/docs/_templates/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/docs/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)      207 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/docs/index.rst.jinja
+-rw-r-----   0 root         (0) root         (0)      772 2022-02-12 15:07:54.000000 pykern-20240430.161713/pykern/package_data/projex/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.834968 pykern-20240430.161713/pykern/package_data/projex/projex/
+-rw-r-----   0 root         (0) root         (0)      296 2022-10-24 20:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/projex/__init__.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.834968 pykern-20240430.161713/pykern/package_data/projex/projex/package_data/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/projex/package_data/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.835968 pykern-20240430.161713/pykern/package_data/projex/projex/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/projex/pkcli/__init__.py.jinja
+-rw-r-----   0 root         (0) root         (0)      298 2022-10-24 20:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/projex/projex_console.py.jinja
+-rw-r-----   0 root         (0) root         (0)      578 2022-10-24 20:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/setup.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.835968 pykern-20240430.161713/pykern/package_data/projex/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/tests/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)      228 2022-10-24 20:51:04.000000 pykern-20240430.161713/pykern/package_data/projex/tests/import_test.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.831968 pykern-20240430.161713/pykern/package_data/projex-licenses/
+-rw-r-----   0 root         (0) root         (0)    34520 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/agpl-3.0.txt
+-rw-r-----   0 root         (0) root         (0)    11358 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/apache2.jinja
+-rw-r-----   0 root         (0) root         (0)    18092 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/gpl2.jinja
+-rw-r-----   0 root         (0) root         (0)    35147 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/gpl3.jinja
+-rw-r-----   0 root         (0) root         (0)    25383 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/lgpl2.jinja
+-rw-r-----   0 root         (0) root         (0)     7651 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/lgpl3.jinja
+-rw-r-----   0 root         (0) root         (0)     1085 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/mit.jinja
+-rw-r-----   0 root         (0) root         (0)      191 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/projex-licenses/proprietary.jinja
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/pykern/package_data/test.yml
+-rw-r-----   0 root         (0) root         (0)     1169 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkarray.py
+-rw-r-----   0 root         (0) root         (0)     2845 2024-03-15 14:11:15.000000 pykern-20240430.161713/pykern/pkasyncio.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.840968 pykern-20240430.161713/pykern/pkcli/
+-rw-r-----   0 root         (0) root         (0)    10485 2024-03-15 14:11:15.000000 pykern-20240430.161713/pykern/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4170 2024-03-20 14:13:19.000000 pykern-20240430.161713/pykern/pkcli/ci.py
+-rw-r-----   0 root         (0) root         (0)     1763 2022-12-28 15:07:11.000000 pykern-20240430.161713/pykern/pkcli/fmt.py
+-rw-r-----   0 root         (0) root         (0)    20449 2024-03-15 14:11:15.000000 pykern-20240430.161713/pykern/pkcli/github.py
+-rw-r-----   0 root         (0) root         (0)    12793 2022-10-31 19:53:53.000000 pykern-20240430.161713/pykern/pkcli/github_orgmode.py
+-rw-r-----   0 root         (0) root         (0)     2849 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkcli/pkexample.py
+-rw-r-----   0 root         (0) root         (0)     4773 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkcli/projex.py
+-rw-r-----   0 root         (0) root         (0)     2962 2024-04-13 14:11:29.000000 pykern-20240430.161713/pykern/pkcli/rsmanifest.py
+-rw-r-----   0 root         (0) root         (0)     6686 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkcli/sim.py
+-rw-r-----   0 root         (0) root         (0)     7427 2024-04-06 14:13:17.000000 pykern-20240430.161713/pykern/pkcli/test.py
+-rw-r-----   0 root         (0) root         (0)    12808 2024-04-13 14:11:29.000000 pykern-20240430.161713/pykern/pkcollections.py
+-rw-r-----   0 root         (0) root         (0)     3686 2023-09-13 14:10:24.000000 pykern-20240430.161713/pykern/pkcompat.py
+-rw-r-----   0 root         (0) root         (0)    24232 2023-10-20 20:51:58.000000 pykern-20240430.161713/pykern/pkconfig.py
+-rw-r-----   0 root         (0) root         (0)     1221 2024-03-28 17:40:02.000000 pykern-20240430.161713/pykern/pkconst.py
+-rw-r-----   0 root         (0) root         (0)    22756 2024-01-19 15:11:21.000000 pykern-20240430.161713/pykern/pkdebug.py
+-rw-r-----   0 root         (0) root         (0)     4591 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkexample.py
+-rw-r-----   0 root         (0) root         (0)     8826 2024-01-19 15:11:21.000000 pykern-20240430.161713/pykern/pkinspect.py
+-rw-r-----   0 root         (0) root         (0)    10253 2024-02-01 15:11:17.000000 pykern-20240430.161713/pykern/pkio.py
+-rw-r-----   0 root         (0) root         (0)     1857 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkjinja.py
+-rw-r-----   0 root         (0) root         (0)     3152 2024-04-13 14:11:29.000000 pykern-20240430.161713/pykern/pkjson.py
+-rw-r-----   0 root         (0) root         (0)     1427 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkplatform.py
+-rw-r-----   0 root         (0) root         (0)     3214 2024-03-28 17:40:02.000000 pykern-20240430.161713/pykern/pkresource.py
+-rw-r-----   0 root         (0) root         (0)      774 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pkrunpy.py
+-rw-r-----   0 root         (0) root         (0)    22115 2024-03-28 17:40:02.000000 pykern-20240430.161713/pykern/pksetup.py
+-rw-r-----   0 root         (0) root         (0)     4287 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pksubprocess.py
+-rw-r-----   0 root         (0) root         (0)    25421 2024-03-20 14:13:19.000000 pykern-20240430.161713/pykern/pkunit.py
+-rw-r-----   0 root         (0) root         (0)     2791 2024-04-30 16:56:28.000000 pykern-20240430.161713/pykern/pkyaml.py
+-rw-r-----   0 root         (0) root         (0)      421 2022-06-24 14:08:21.000000 pykern-20240430.161713/pykern/pykern_console.py
+-rw-r-----   0 root         (0) root         (0)      180 2024-03-20 14:13:19.000000 pykern-20240430.161713/pykern/pytest_plugin.py
+-rw-r-----   0 root         (0) root         (0)      404 2022-09-26 20:14:13.000000 pykern-20240430.161713/pykern/quest.py
+-rw-r-----   0 root         (0) root         (0)     3756 2024-03-15 14:11:15.000000 pykern-20240430.161713/pykern/util.py
+-rw-r-----   0 root         (0) root         (0)    23884 2023-09-25 14:09:48.000000 pykern-20240430.161713/pykern/xlsx.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.945969 pykern-20240430.161713/pykern.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)    11319 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/SOURCES.txt
+-rw-r-----   0 root         (0) root         (0)        1 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/dependency_links.txt
+-rw-r-----   0 root         (0) root         (0)       54 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/entry_points.txt
+-rw-r-----   0 root         (0) root         (0)      376 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/requires.txt
+-rw-r-----   0 root         (0) root         (0)        7 2024-04-30 16:58:26.000000 pykern-20240430.161713/pykern.egg-info/top_level.txt
+-rw-r-----   0 root         (0) root         (0)     1455 2024-04-02 19:05:05.000000 pykern-20240430.161713/pyproject.toml
+-rw-r-----   0 root         (0) root         (0)       38 2024-04-30 16:58:26.946969 pykern-20240430.161713/setup.cfg
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.855968 pykern-20240430.161713/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)      554 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/conftest.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.788968 pykern-20240430.161713/tests/fconf_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.857968 pykern-20240430.161713/tests/fconf_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      450 2022-07-18 15:54:21.000000 pykern-20240430.161713/tests/fconf_data/1.in/0.py
+-rw-r-----   0 root         (0) root         (0)      921 2024-04-27 14:14:09.000000 pykern-20240430.161713/tests/fconf_data/1.in/1.yml
+-rw-r-----   0 root         (0) root         (0)       57 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/1.in/2.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.857968 pykern-20240430.161713/tests/fconf_data/1.out/
+-rw-r-----   0 root         (0) root         (0)     1728 2024-04-27 14:14:09.000000 pykern-20240430.161713/tests/fconf_data/1.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.857968 pykern-20240430.161713/tests/fconf_data/2.in/
+-rw-r-----   0 root         (0) root         (0)      139 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/2.in/1.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.858968 pykern-20240430.161713/tests/fconf_data/2.out/
+-rw-r-----   0 root         (0) root         (0)      374 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/2.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.859968 pykern-20240430.161713/tests/fconf_data/3.in/
+-rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/3.in/0.py
+-rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/3.in/1.py
+-rw-r-----   0 root         (0) root         (0)       11 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/3.in/2.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.859968 pykern-20240430.161713/tests/fconf_data/3.out/
+-rw-r-----   0 root         (0) root         (0)      118 2022-07-07 14:08:03.000000 pykern-20240430.161713/tests/fconf_data/3.out/res.json
+-rw-r-----   0 root         (0) root         (0)      748 2024-04-27 14:14:09.000000 pykern-20240430.161713/tests/fconf_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.860968 pykern-20240430.161713/tests/mpi_data/
+-rw-r-----   0 root         (0) root         (0)      925 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/mpi_data/p1.py
+-rw-r-----   0 root         (0) root         (0)     1307 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/mpi_test.py
+-rw-r-----   0 root         (0) root         (0)      885 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkarray_test.py
+-rw-r-----   0 root         (0) root         (0)     2633 2024-01-19 15:11:21.000000 pykern-20240430.161713/tests/pkasyncio_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.865968 pykern-20240430.161713/tests/pkcli/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.790968 pykern-20240430.161713/tests/pkcli/ci1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.865968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.866968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/.x/
+-rw-r-----   0 root         (0) root         (0)       61 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/.x/x.py
+-rw-r-----   0 root         (0) root         (0)       34 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.867968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/somepkg/
+-rw-r-----   0 root         (0) root         (0)        8 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/somepkg/has_print.py
+-rw-r-----   0 root         (0) root         (0)       14 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/somepkg/ok.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.867968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/somepkg/package_data/
+-rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/somepkg/package_data/not_checked.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.790968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/tests/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.868968 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/tests/test_data/
+-rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.in/tests/test_data/not_checked.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.868968 pykern-20240430.161713/tests/pkcli/ci1_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       45 2022-10-22 14:07:30.000000 pykern-20240430.161713/tests/pkcli/ci1_data/1.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)      428 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkcli/ci1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.793968 pykern-20240430.161713/tests/pkcli/ci_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.868968 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-1.in/
+-rw-r-----   0 root         (0) root         (0)       36 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.869968 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-1.out/
+-rw-r-----   0 root         (0) root         (0)       24 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.869968 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-2.in/
+-rw-r-----   0 root         (0) root         (0)       45 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.870968 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_eof_newline-2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.870968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.871968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.in/run/
+-rw-r-----   0 root         (0) root         (0)       27 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.in/run/ignored.py
+-rw-r-----   0 root         (0) root         (0)      191 2022-11-17 18:34:08.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.871968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.out/
+-rw-r-----   0 root         (0) root         (0)      148 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.872968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-2.in/
+-rw-r-----   0 root         (0) root         (0)      208 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.872968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.872968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-3.in/
+-rw-r-----   0 root         (0) root         (0)       87 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-3.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.873968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-3.out/
+-rw-r-----   0 root         (0) root         (0)       82 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-3.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.873968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-4.in/
+-rw-r-----   0 root         (0) root         (0)       10 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-4.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.874968 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-4.out/
+-rw-r-----   0 root         (0) root         (0)       31 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/check_prints-4.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.874968 pykern-20240430.161713/tests/pkcli/ci_data/run-1.in/
+-rw-r-----   0 root         (0) root         (0)       20 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/run-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.875968 pykern-20240430.161713/tests/pkcli/ci_data/run-1.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/run-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.875968 pykern-20240430.161713/tests/pkcli/ci_data/run-2.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.876968 pykern-20240430.161713/tests/pkcli/ci_data/run-2.in/tests/
+-rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/run-2.in/tests/x_test.py
+-rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/run-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.876968 pykern-20240430.161713/tests/pkcli/ci_data/run-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_data/run-2.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)      400 2022-11-17 18:34:09.000000 pykern-20240430.161713/tests/pkcli/ci_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.794968 pykern-20240430.161713/tests/pkcli/fmt_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.876968 pykern-20240430.161713/tests/pkcli/fmt_data/check1.in/
+-rw-r-----   0 root         (0) root         (0)       44 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/check1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.877968 pykern-20240430.161713/tests/pkcli/fmt_data/check1.out/
+-rw-r-----   0 root         (0) root         (0)       39 2022-12-28 15:07:11.000000 pykern-20240430.161713/tests/pkcli/fmt_data/check1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.877968 pykern-20240430.161713/tests/pkcli/fmt_data/check2.in/
+-rw-r-----   0 root         (0) root         (0)       56 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/check2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.878968 pykern-20240430.161713/tests/pkcli/fmt_data/check2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240430.161713/tests/pkcli/fmt_data/check2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.878968 pykern-20240430.161713/tests/pkcli/fmt_data/diff.in/
+-rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/diff.in/file1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.879969 pykern-20240430.161713/tests/pkcli/fmt_data/diff.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240430.161713/tests/pkcli/fmt_data/diff.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.879969 pykern-20240430.161713/tests/pkcli/fmt_data/diff2.in/
+-rw-r-----   0 root         (0) root         (0)      368 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/diff2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.879969 pykern-20240430.161713/tests/pkcli/fmt_data/diff2.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-06-18 14:08:41.000000 pykern-20240430.161713/tests/pkcli/fmt_data/diff2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.881968 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.in/
+-rw-r-----   0 root         (0) root         (0)      170 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.in/file1.py
+-rw-r-----   0 root         (0) root         (0)      483 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.in/y.py
+-rw-r-----   0 root         (0) root         (0)      244 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.in/z.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.882969 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.out/
+-rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.out/file1.py
+-rw-r-----   0 root         (0) root         (0)      584 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.out/y.py
+-rw-r-----   0 root         (0) root         (0)      324 2022-06-14 14:07:59.000000 pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.out/z.py
+-rw-r-----   0 root         (0) root         (0)      798 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkcli/fmt_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.796968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.883968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)    20455 2022-10-11 14:09:00.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.883968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)     1301 2022-10-15 14:08:58.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.884968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)    21657 2022-10-11 14:09:00.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.884968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)     1056 2022-10-15 14:08:58.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.885969 pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)     2922 2022-10-11 14:09:00.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json
+-rw-r-----   0 root         (0) root         (0)     1264 2022-10-11 14:09:00.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.886968 pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)      933 2022-10-11 14:09:00.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json
+-rw-r-----   0 root         (0) root         (0)     2312 2022-10-31 19:53:53.000000 pykern-20240430.161713/tests/pkcli/github_orgmode_test.py
+-rw-r-----   0 root         (0) root         (0)     4988 2024-03-15 14:11:15.000000 pykern-20240430.161713/tests/pkcli/github_test.py
+-rw-r-----   0 root         (0) root         (0)     2923 2023-08-16 14:09:51.000000 pykern-20240430.161713/tests/pkcli/projex_test.py
+-rw-r-----   0 root         (0) root         (0)     1995 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkcli/rsmanifest_test.py
+-rw-r-----   0 root         (0) root         (0)     1816 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkcli/sim_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.796968 pykern-20240430.161713/tests/pkcli/test1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.886968 pykern-20240430.161713/tests/pkcli/test1_data/tests/
+-rw-r-----   0 root         (0) root         (0)      293 2023-04-05 14:10:34.000000 pykern-20240430.161713/tests/pkcli/test1_data/tests/always_test.py
+-rw-r-----   0 root         (0) root         (0)      461 2023-04-05 14:10:34.000000 pykern-20240430.161713/tests/pkcli/test1_data/tests/twice_test.py
+-rw-r-----   0 root         (0) root         (0)      653 2023-04-05 14:10:34.000000 pykern-20240430.161713/tests/pkcli/test1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.796968 pykern-20240430.161713/tests/pkcli/test2_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.887968 pykern-20240430.161713/tests/pkcli/test2_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      338 2023-10-16 19:47:54.000000 pykern-20240430.161713/tests/pkcli/test2_data/1.in/coroutine_test.py
+-rw-r-----   0 root         (0) root         (0)      685 2024-04-06 14:13:17.000000 pykern-20240430.161713/tests/pkcli/test2_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.796968 pykern-20240430.161713/tests/pkcli/test_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.888969 pykern-20240430.161713/tests/pkcli/test_data/tests/
+-rw-r-----   0 root         (0) root         (0)      277 2019-12-04 23:50:51.000000 pykern-20240430.161713/tests/pkcli/test_data/tests/1_test.py
+-rw-r-----   0 root         (0) root         (0)      282 2019-12-04 23:50:51.000000 pykern-20240430.161713/tests/pkcli/test_data/tests/2_test.py
+-rw-r-----   0 root         (0) root         (0)      327 2024-02-13 15:11:30.000000 pykern-20240430.161713/tests/pkcli/test_data/tests/3_test.py
+-rw-r-----   0 root         (0) root         (0)     2463 2024-02-13 15:11:30.000000 pykern-20240430.161713/tests/pkcli/test_test.py
+-rw-r-----   0 root         (0) root         (0)      597 2022-06-30 14:07:51.000000 pykern-20240430.161713/tests/pkcli1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.798968 pykern-20240430.161713/tests/pkcli_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.889968 pykern-20240430.161713/tests/pkcli_data/arghparsing/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/arghparsing/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.889968 pykern-20240430.161713/tests/pkcli_data/arghparsing/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/arghparsing/pkcli/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.889968 pykern-20240430.161713/tests/pkcli_data/command_info.in/
+-rw-r-----   0 root         (0) root         (0)      140 2022-10-04 14:08:26.000000 pykern-20240430.161713/tests/pkcli_data/command_info.in/example_pkcli_module.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.890968 pykern-20240430.161713/tests/pkcli_data/command_info.out/
+-rw-r-----   0 root         (0) root         (0)       17 2022-10-04 14:08:26.000000 pykern-20240430.161713/tests/pkcli_data/command_info.out/example_stderr.out
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.890968 pykern-20240430.161713/tests/pkcli_data/package1/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.892969 pykern-20240430.161713/tests/pkcli_data/package1/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package1/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      366 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package1/pkcli/conf1.py
+-rw-r-----   0 root         (0) root         (0)      178 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package1/pkcli/conf2.py
+-rw-r-----   0 root         (0) root         (0)      219 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package1/pkcli/conf3.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.893968 pykern-20240430.161713/tests/pkcli_data/package2/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package2/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.894968 pykern-20240430.161713/tests/pkcli_data/package2/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package2/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      310 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package2/pkcli/argh_test.py
+-rw-r-----   0 root         (0) root         (0)      195 2023-12-07 23:37:10.000000 pykern-20240430.161713/tests/pkcli_data/package2/pkcli/some_mod.py
+-rw-r-----   0 root         (0) root         (0)     4879 2024-03-15 14:11:15.000000 pykern-20240430.161713/tests/pkcli_test.py
+-rw-r-----   0 root         (0) root         (0)     6806 2024-04-13 14:11:29.000000 pykern-20240430.161713/tests/pkcollections_test.py
+-rw-r-----   0 root         (0) root         (0)     2276 2023-09-13 14:10:24.000000 pykern-20240430.161713/tests/pkcompat_test.py
+-rw-r-----   0 root         (0) root         (0)     1862 2023-03-14 17:59:06.000000 pykern-20240430.161713/tests/pkconfig1_test.py
+-rw-r-----   0 root         (0) root         (0)     1175 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkconfig2_test.py
+-rw-r-----   0 root         (0) root         (0)      868 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkconfig3_test.py
+-rw-r-----   0 root         (0) root         (0)      754 2023-04-14 17:14:13.000000 pykern-20240430.161713/tests/pkconfig4_test.py
+-rw-r-----   0 root         (0) root         (0)     1588 2023-04-14 17:14:13.000000 pykern-20240430.161713/tests/pkconfig5_test.py
+-rw-r-----   0 root         (0) root         (0)      623 2023-04-14 17:14:13.000000 pykern-20240430.161713/tests/pkconfig6_test.py
+-rw-r-----   0 root         (0) root         (0)      617 2023-04-14 17:14:13.000000 pykern-20240430.161713/tests/pkconfig7_test.py
+-rw-r-----   0 root         (0) root         (0)      350 2023-04-23 14:08:30.000000 pykern-20240430.161713/tests/pkconfig8_test.py
+-rw-r-----   0 root         (0) root         (0)      421 2023-10-20 20:51:58.000000 pykern-20240430.161713/tests/pkconfig9_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.798968 pykern-20240430.161713/tests/pkconfig_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.896968 pykern-20240430.161713/tests/pkconfig_data/p1/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkconfig_data/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      214 2023-10-20 20:51:58.000000 pykern-20240430.161713/tests/pkconfig_data/p1/append_error.py
+-rw-r-----   0 root         (0) root         (0)      469 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkconfig_data/p1/base_pkconfig.py
+-rw-r-----   0 root         (0) root         (0)     1984 2020-01-08 19:20:36.000000 pykern-20240430.161713/tests/pkconfig_data/p1/m1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.897968 pykern-20240430.161713/tests/pkconfig_data/p1/s1/
+-rw-r-----   0 root         (0) root         (0)        2 2019-11-17 13:40:26.000000 pykern-20240430.161713/tests/pkconfig_data/p1/s1/__init__.py
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkconfig_data/p1/s1/m11.py
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkconfig_data/p1/s1/m12.py
+-rw-r-----   0 root         (0) root         (0)    10382 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkdebug1_test.py
+-rw-r-----   0 root         (0) root         (0)     1870 2023-08-16 14:09:51.000000 pykern-20240430.161713/tests/pkdebug2_test.py
+-rw-r-----   0 root         (0) root         (0)     1737 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkexample_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.799968 pykern-20240430.161713/tests/pkinspect_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.898969 pykern-20240430.161713/tests/pkinspect_data/p1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkinspect_data/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      326 2021-02-16 00:17:58.000000 pykern-20240430.161713/tests/pkinspect_data/p1/m1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.898969 pykern-20240430.161713/tests/pkinspect_data/p1/p2/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkinspect_data/p1/p2/__init__.py
+-rw-r-----   0 root         (0) root         (0)       35 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkinspect_data/p1/p2/m2.py
+-rw-r-----   0 root         (0) root         (0)     3979 2024-01-19 15:11:21.000000 pykern-20240430.161713/tests/pkinspect_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.901969 pykern-20240430.161713/tests/pkio_data/
+-rw-r-----   0 root         (0) root         (0)   239616 2024-02-01 15:11:17.000000 pykern-20240430.161713/tests/pkio_data/binary.dat
+-rw-r-----   0 root         (0) root         (0)       18 2024-02-01 15:11:17.000000 pykern-20240430.161713/tests/pkio_data/text.dat
+-rw-r-----   0 root         (0) root         (0)     7132 2024-03-15 14:11:15.000000 pykern-20240430.161713/tests/pkio_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.901969 pykern-20240430.161713/tests/pkjinja_data/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkjinja_data/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.902969 pykern-20240430.161713/tests/pkjinja_data/package_data/
+-rw-r-----   0 root         (0) root         (0)       12 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkjinja_data/package_data/t1.jinja
+-rw-r-----   0 root         (0) root         (0)      211 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkjinja_data/t1.py
+-rw-r-----   0 root         (0) root         (0)      997 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkjinja_test.py
+-rw-r-----   0 root         (0) root         (0)     1965 2024-04-13 14:11:29.000000 pykern-20240430.161713/tests/pkjson_test.py
+-rw-r-----   0 root         (0) root         (0)     1415 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkplatform_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.903968 pykern-20240430.161713/tests/pkresource_data/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkresource_data/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.903968 pykern-20240430.161713/tests/pkresource_data/package_data/
+-rw-r-----   0 root         (0) root         (0)       14 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkresource_data/package_data/somefile
+-rw-r-----   0 root         (0) root         (0)      189 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkresource_data/t1.py
+-rw-r-----   0 root         (0) root         (0)     1309 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkresource_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.904969 pykern-20240430.161713/tests/pkrunpy_data/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkrunpy_data/f1.py
+-rw-r-----   0 root         (0) root         (0)      533 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pkrunpy_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.801968 pykern-20240430.161713/tests/pksetup_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.906968 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/
+-rw-r-----   0 root         (0) root         (0)      738 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/.gitignore
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/LICENSE
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.906968 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/docs/
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.907969 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/examples/
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/examples/example1.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.908969 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/base_pkconfig.py
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/mod1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.908969 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/
+-rw-r-----   0 root         (0) root         (0)       10 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/data1
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.909968 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/__init__.py
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/mod2.py
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/requirements.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.909968 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/scripts/
+-rw-r-----   0 root         (0) root         (0)       25 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/scripts/script1
+-rw-r-----   0 root         (0) root         (0)      295 2019-05-06 20:05:16.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.911969 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)       99 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/tests/mod1_test.py
+-rw-r-----   0 root         (0) root         (0)      181 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit1/tests/mod2_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.914969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/
+-rw-r-----   0 root         (0) root         (0)      756 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/.gitignore
+-rw-r-----   0 root         (0) root         (0)      134 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/.travis.yml
+-rw-r-----   0 root         (0) root         (0)    22102 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/LICENSE
+-rw-r-----   0 root         (0) root         (0)      302 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.914969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.915969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/_static/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.915969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/_templates/.gitignore
+-rw-r-----   0 root         (0) root         (0)      227 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.917969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/__init__.py
+-rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/base_pkconfig.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.917969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.917969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      466 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/pksetupunit2/pksetupunit2_console.py
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/requirements.txt
+-rw-r-----   0 root         (0) root         (0)     1051 2019-05-06 20:05:16.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.918969 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)      321 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pksetup_data/pksetupunit2/tests/simple_test.py
+-rw-r-----   0 root         (0) root         (0)     5098 2023-04-04 14:10:19.000000 pykern-20240430.161713/tests/pksetup_test.py
+-rw-r-----   0 root         (0) root         (0)     3892 2022-06-24 14:08:21.000000 pykern-20240430.161713/tests/pksubprocess_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.804968 pykern-20240430.161713/tests/pkunit1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.919969 pykern-20240430.161713/tests/pkunit1_data/bytes-1.in/
+-rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240430.161713/tests/pkunit1_data/bytes-1.in/dot.gif
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.919969 pykern-20240430.161713/tests/pkunit1_data/bytes-1.out/
+-rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240430.161713/tests/pkunit1_data/bytes-1.out/dot.gif
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.920969 pykern-20240430.161713/tests/pkunit1_data/conformance-1.in/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-1.in/in.txt
+-rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-1.in/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.921969 pykern-20240430.161713/tests/pkunit1_data/conformance-1.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-1.out/in.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-1.out/out.txt
+-rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-1.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.922969 pykern-20240430.161713/tests/pkunit1_data/conformance-2.in/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-2.in/in.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-2.in/out.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.923969 pykern-20240430.161713/tests/pkunit1_data/conformance-2.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/conformance-2.out/in.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.923969 pykern-20240430.161713/tests/pkunit1_data/curly_brackets.in/
+-rw-r-----   0 root         (0) root         (0)       13 2022-09-20 14:07:49.000000 pykern-20240430.161713/tests/pkunit1_data/curly_brackets.in/sample.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.924969 pykern-20240430.161713/tests/pkunit1_data/curly_brackets.out/
+-rw-r-----   0 root         (0) root         (0)        9 2022-09-20 14:07:49.000000 pykern-20240430.161713/tests/pkunit1_data/curly_brackets.out/sample.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.924969 pykern-20240430.161713/tests/pkunit1_data/deviance-1.in/
+-rw-r-----   0 root         (0) root         (0)        0 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/deviance-1.in/not-used.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.924969 pykern-20240430.161713/tests/pkunit1_data/deviance-1.out/
+-rw-r-----   0 root         (0) root         (0)        9 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/pkunit1_data/deviance-1.out/out.txt
+-rw-r-----   0 root         (0) root         (0)     1449 2023-04-14 14:08:36.000000 pykern-20240430.161713/tests/pkunit1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.935969 pykern-20240430.161713/tests/pkunit_data/
+-rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/actual_abs_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240430.161713/tests/pkunit_data/actual_conformance_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/actual_default_conformance.ndiff
+-rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/actual_default_conformance_1.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/actual_rel_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/actual_rel_ok_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkunit_data/assert1.json
+-rw-r-----   0 root         (0) root         (0)       88 2022-08-23 22:15:42.000000 pykern-20240430.161713/tests/pkunit_data/different.bin
+-rw-r-----   0 root         (0) root         (0)      543 2022-05-16 23:38:16.000000 pykern-20240430.161713/tests/pkunit_data/example.csv
+-rw-r-----   0 root         (0) root         (0)     5425 2022-05-16 23:38:16.000000 pykern-20240430.161713/tests/pkunit_data/example.xlsx
+-rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/expect_abs_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240430.161713/tests/pkunit_data/expect_conformance_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       52 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/expect_default_conformance.ndiff
+-rw-r-----   0 root         (0) root         (0)       51 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/expect_default_conformance_1.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/expect_rel_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240430.161713/tests/pkunit_data/expect_rel_ok_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       20 2022-04-08 21:30:14.000000 pykern-20240430.161713/tests/pkunit_data/file_eq1.json
+-rw-r-----   0 root         (0) root         (0)        0 2022-04-08 21:30:14.000000 pykern-20240430.161713/tests/pkunit_data/file_eq2.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-04-08 21:30:14.000000 pykern-20240430.161713/tests/pkunit_data/file_eq3.txt
+-rw-r-----   0 root         (0) root         (0)       67 2022-08-25 16:28:29.000000 pykern-20240430.161713/tests/pkunit_data/ignore_lines.in
+-rw-r-----   0 root         (0) root         (0)       68 2022-08-25 16:28:29.000000 pykern-20240430.161713/tests/pkunit_data/ignore_lines.out
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.805968 pykern-20240430.161713/tests/pkunit_data/import1/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.935969 pykern-20240430.161713/tests/pkunit_data/import1/p1/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkunit_data/import1/p1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.805968 pykern-20240430.161713/tests/pkunit_data/import2/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.936969 pykern-20240430.161713/tests/pkunit_data/import2/p1/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkunit_data/import2/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240430.161713/tests/pkunit_data/in.bin
+-rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240430.161713/tests/pkunit_data/out.bin
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkunit_data/t1.yml
+-rw-r-----   0 root         (0) root         (0)     8413 2023-10-30 22:15:18.000000 pykern-20240430.161713/tests/pkunit_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.936969 pykern-20240430.161713/tests/pkyaml_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.937969 pykern-20240430.161713/tests/pkyaml_data/1.in/
+-rw-r-----   0 root         (0) root         (0)       65 2022-07-12 14:07:33.000000 pykern-20240430.161713/tests/pkyaml_data/1.in/in.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.937969 pykern-20240430.161713/tests/pkyaml_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       62 2022-07-12 14:07:33.000000 pykern-20240430.161713/tests/pkyaml_data/1.out/out.yml
+-rw-r-----   0 root         (0) root         (0)       27 2020-09-03 15:51:30.000000 pykern-20240430.161713/tests/pkyaml_data/dump1.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.937969 pykern-20240430.161713/tests/pkyaml_data/p1/
+-rw-r-----   0 root         (0) root         (0)       61 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkyaml_data/p1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.938969 pykern-20240430.161713/tests/pkyaml_data/p1/package_data/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240430.161713/tests/pkyaml_data/p1/package_data/conf2.yml
+-rw-r-----   0 root         (0) root         (0)     1237 2024-04-30 16:56:28.000000 pykern-20240430.161713/tests/pkyaml_test.py
+-rw-r-----   0 root         (0) root         (0)     1163 2024-02-01 15:11:17.000000 pykern-20240430.161713/tests/util_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.807968 pykern-20240430.161713/tests/xlsx_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.938969 pykern-20240430.161713/tests/xlsx_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      903 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/1.in/case.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.939969 pykern-20240430.161713/tests/xlsx_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       58 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/1.out/case1.csv
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.939969 pykern-20240430.161713/tests/xlsx_data/1.out/xl/
+-rw-r-----   0 root         (0) root         (0)      281 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/1.out/xl/sharedStrings.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.940969 pykern-20240430.161713/tests/xlsx_data/1.out/xl/worksheets/
+-rw-r-----   0 root         (0) root         (0)     1250 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.941969 pykern-20240430.161713/tests/xlsx_data/2.in/
+-rw-r-----   0 root         (0) root         (0)     1057 2022-08-10 14:07:21.000000 pykern-20240430.161713/tests/xlsx_data/2.in/case.py
+-rw-r-----   0 root         (0) root         (0)     6288 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/2.in/case2.xlsx
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.942969 pykern-20240430.161713/tests/xlsx_data/2.out/
+-rw-r-----   0 root         (0) root         (0)       90 2022-08-10 14:07:21.000000 pykern-20240430.161713/tests/xlsx_data/2.out/case2#0.csv
+-rw-r-----   0 root         (0) root         (0)        9 2022-06-03 23:08:48.000000 pykern-20240430.161713/tests/xlsx_data/2.out/case2#1.csv
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.942969 pykern-20240430.161713/tests/xlsx_data/2.out/xl/
+-rw-r-----   0 root         (0) root         (0)      338 2022-08-10 14:07:21.000000 pykern-20240430.161713/tests/xlsx_data/2.out/xl/sharedStrings.xml
+-rw-r-----   0 root         (0) root         (0)     1656 2023-03-14 17:59:06.000000 pykern-20240430.161713/tests/xlsx_data/2.out/xl/styles.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.943969 pykern-20240430.161713/tests/xlsx_data/2.out/xl/worksheets/
+-rw-r-----   0 root         (0) root         (0)     1830 2023-01-16 15:07:03.000000 pykern-20240430.161713/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml
+-rw-r-----   0 root         (0) root         (0)      795 2022-06-03 23:08:48.000000 pykern-20240430.161713/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.944969 pykern-20240430.161713/tests/xlsx_data/3.in/
+-rw-r-----   0 root         (0) root         (0)      484 2022-08-02 14:08:07.000000 pykern-20240430.161713/tests/xlsx_data/3.in/case.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-30 16:58:26.944969 pykern-20240430.161713/tests/xlsx_data/3.out/
+-rw-r-----   0 root         (0) root         (0)       38 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/xlsx_data/3.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)     1114 2022-08-06 14:07:18.000000 pykern-20240430.161713/tests/xlsx_test.py
```

### Comparing `pykern-20240412.230110/LICENSE` & `pykern-20240430.161713/LICENSE`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/PKG-INFO` & `pykern-20240430.161713/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykern
-Version: 20240412.230110
+Version: 20240430.161713
 Summary: Python application support library
 Author-email: RadiaSoft LLC <pip@pykern.org>
 Project-URL: Homepage, http://pykern.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pykern-20240412.230110/pykern/fconf.py` & `pykern-20240430.161713/pykern/fconf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Python and YAML configuration file parser.
 
 FConf reads Python and YAML files and produces a single, merged
 PKDict. FConf is not a replacement for `pykern.pkconfig`. Rather it is
 for complex configuration input files to programs that often require
 programmatic generation. FConf was written for
 RSConf <https://git.radiasoft.org/rsconf>.
@@ -152,17 +151,19 @@
 
   a: 'c({"d": "e"})'
 
 :copyright: Copyright (c) 2022 RadiaSoft LLC.  All Rights Reserved.
 :license: http://www.apache.org/licenses/LICENSE-2.0.html
 
 """
+
 from pykern.pkcollections import PKDict
 from pykern.pkdebug import pkdc, pkdlog, pkdp
 import contextlib
+import copy
 import inspect
 import pykern.pkrunpy
 import re
 import pykern.pkyaml
 import pykern.pkcollections
 import pykern.pkinspect
 import pykern.pkio
@@ -189,27 +190,32 @@
 
 _NO_PARAM = object()
 
 _BUILTINS_EXT = "builtins"
 
 
 class Parser(PKDict):
-    def __init__(self, files):
+    def __init__(self, files, base_vars=None):
         self.pkupdate(
             files=PKDict(),
             macros=PKDict(),
         )
         self._add_file(pykern.pkio.py_path(f"fconf.{_BUILTINS_EXT}"))
         for f in files:
             try:
                 self._add_file(f)
             except Exception as e:
                 pykern.pkinspect.append_exception_reason(e, f"fconf.Parser.file={f}")
                 raise
-        e = _Evaluator(parser=self)
+        if "yml" not in self.files:
+            raise ValueError("must supply at least one '.yml' file")
+        e = _Evaluator(
+            global_fvars=PKDict() if base_vars is None else copy.deepcopy(base_vars),
+            parser=self,
+        )
         for f in self.files.yml:
             e.start(source=f)
         self.result = e.global_fvars
 
     def _add_file(self, path):
         e = path.ext[1:].lower()
         f = _File(
@@ -289,27 +295,30 @@
             if inspect.isfunction(o) and (
                 not co_filename or co_filename == o.__code__.co_filename
             ):
                 m[n] = o
         return m
 
 
-def parse_all(path):
+def parse_all(path, base_vars=None):
     """Parse all the Python and YAML files in `directory`
 
     Files are read in sorted order with all Python files first and
     YAML files next. YAML file evaluation happens in that same order.
 
     Args:
         path (py.path): directory that *.py and *.yml files
-
+        base_vars (PKDict): initial variable state. May be hierarchical. [None]
+    Returns:
+        PKDict: evaluated and merged files plus base_vars
     """
     return Parser(
         pykern.pkio.sorted_glob(path.join("*.py"))
         + pykern.pkio.sorted_glob(path.join("*.yml")),
+        base_vars=None,
     ).result
 
 
 class _Builtins:
     @staticmethod
     def fconf_var(namespace, name):
         return namespace._evaluator.fconf_var(name)
@@ -318,15 +327,14 @@
 class _Evaluator(PKDict):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # By NOT passing __builtins__=PKDict(), builtins are implicitly added.
         # Python builtins are useful
         self.global_ns = PKDict()
         self.local_ns = _Namespace(self)
-        self.global_fvars = PKDict()
         self.local_fvars = PKDict()
 
     def fconf_var(self, name):
         try:
             return self.global_fvars.pknested_get(name)
         except KeyError:
             # Do not cascade the exception.
```

### Comparing `pykern-20240412.230110/pykern/mpi.py` & `pykern-20240430.161713/pykern/mpi.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/docs-conf.py.format` & `pykern-20240430.161713/pykern/package_data/docs-conf.py.format`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex/dot-gitignore.jinja` & `pykern-20240430.161713/pykern/package_data/projex/dot-gitignore.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex/setup.py.jinja` & `pykern-20240430.161713/pykern/package_data/projex/setup.py.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/agpl-3.0.txt` & `pykern-20240430.161713/pykern/package_data/projex-licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/apache2.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/apache2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/gpl2.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/gpl2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/gpl3.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/gpl3.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/lgpl2.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/lgpl2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/lgpl3.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/lgpl3.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/package_data/projex-licenses/mit.jinja` & `pykern-20240430.161713/pykern/package_data/projex-licenses/mit.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkarray.py` & `pykern-20240430.161713/pykern/pkarray.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkasyncio.py` & `pykern-20240430.161713/pykern/pkasyncio.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/__init__.py` & `pykern-20240430.161713/pykern/pkcli/__init__.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/ci.py` & `pykern-20240430.161713/pykern/pkcli/ci.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/fmt.py` & `pykern-20240430.161713/pykern/pkcli/fmt.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/github.py` & `pykern-20240430.161713/pykern/pkcli/github.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/github_orgmode.py` & `pykern-20240430.161713/pykern/pkcli/github_orgmode.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/pkexample.py` & `pykern-20240430.161713/pykern/pkcli/pkexample.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/projex.py` & `pykern-20240430.161713/pykern/pkcli/projex.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/rsmanifest.py` & `pykern-20240430.161713/pykern/pkcli/rsmanifest.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/sim.py` & `pykern-20240430.161713/pykern/pkcli/sim.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcli/test.py` & `pykern-20240430.161713/pykern/pkcli/test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcollections.py` & `pykern-20240430.161713/pykern/pkcollections.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkcompat.py` & `pykern-20240430.161713/pykern/pkcompat.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkconfig.py` & `pykern-20240430.161713/pykern/pkconfig.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkconst.py` & `pykern-20240430.161713/pykern/pkconst.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkdebug.py` & `pykern-20240430.161713/pykern/pkdebug.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkexample.py` & `pykern-20240430.161713/pykern/pkexample.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkinspect.py` & `pykern-20240430.161713/pykern/pkinspect.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkio.py` & `pykern-20240430.161713/pykern/pkio.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkjinja.py` & `pykern-20240430.161713/pykern/pkjinja.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkjson.py` & `pykern-20240430.161713/pykern/pkjson.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkplatform.py` & `pykern-20240430.161713/pykern/pkplatform.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkresource.py` & `pykern-20240430.161713/pykern/pkresource.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkrunpy.py` & `pykern-20240430.161713/pykern/pkrunpy.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pksetup.py` & `pykern-20240430.161713/pykern/pksetup.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pksubprocess.py` & `pykern-20240430.161713/pykern/pksubprocess.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkunit.py` & `pykern-20240430.161713/pykern/pkunit.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/pkyaml.py` & `pykern-20240430.161713/pykern/pkyaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# -*- coding: utf-8 -*-
 """Wrapper for :mod:`yaml`
 
 :copyright: Copyright (c) 2015-2022 RadiaSoft LLC.  All Rights Reserved.
 :license: http://www.apache.org/licenses/LICENSE-2.0.html
 """
+
 from pykern.pkcollections import PKDict
 from pykern.pkdebug import pkdp, pkdlog
 from pykern import pkcompat
 from pykern import pkinspect
 from pykern import pkio
 from pykern import pkresource
 import ruamel.yaml
@@ -27,30 +27,40 @@
 
     Args:
         obj (object): any Python object
         filename (str or py.path): where to write
         pretty (bool): pretty print [True]
         kwargs (object): other arguments to `ruamel.yaml.dump`
     """
-    y = ruamel.yaml.YAML()
-    if pretty:
-        y.indent(mapping=2, sequence=4, offset=2)
-    y.dump(_fixup_dump(obj), stream=pkio.open_text(filename, mode="wt"), **kwargs)
+    try:
+        y = ruamel.yaml.YAML()
+        if pretty:
+            y.indent(mapping=2, sequence=4, offset=2)
+            y.dump(
+                _fixup_dump(obj), stream=pkio.open_text(filename, mode="wt"), **kwargs
+            )
+    except Exception:
+        pkdlog("error writing file={}", filename)
+        raise
 
 
 def load_file(filename):
     """Read a file, making sure all keys and values are locale.
 
     Args:
         filename (str or py.path): file to read (Note: ``.yml`` will not be appended)
 
     Returns:
         object: `PKDict` or list
     """
-    return load_str(pkio.read_text(filename))
+    try:
+        return load_str(pkio.read_text(filename))
+    except Exception:
+        pkdlog("error file={}", filename)
+        raise
 
 
 def load_resource(basename):
     """Read a resource, making sure all keys and values are locale
 
     Args:
         basename (str): file to read without yml suffix
```

### Comparing `pykern-20240412.230110/pykern/util.py` & `pykern-20240430.161713/pykern/util.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern/xlsx.py` & `pykern-20240430.161713/pykern/xlsx.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pykern.egg-info/PKG-INFO` & `pykern-20240430.161713/pykern.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykern
-Version: 20240412.230110
+Version: 20240430.161713
 Summary: Python application support library
 Author-email: RadiaSoft LLC <pip@pykern.org>
 Project-URL: Homepage, http://pykern.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pykern-20240412.230110/pykern.egg-info/SOURCES.txt` & `pykern-20240430.161713/pykern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/pyproject.toml` & `pykern-20240430.161713/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/conftest.py` & `pykern-20240430.161713/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/fconf_data/1.in/1.yml` & `pykern-20240430.161713/tests/fconf_data/1.in/1.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   must_be_pkdict({}): test canonicalization
   # without the quotes gets the error:
   # ruamel.yaml.parser.ParserError: while parsing a flow sequence
   #  in "<unicode string>"
   # did not find expected ',' or ']'
   #  in "<unicode string>"
   inline_array: [ "${top.pi}" ]
+  fconf_test_var1: ${fconf_test.var1}
 
 next:
   apple: 1
   pear: 2
   best_food: ${top.pi}
   score_plus_3: add_score(3)
   complex_data: nop(${top})
```

### Comparing `pykern-20240412.230110/tests/fconf_data/1.out/res.json` & `pykern-20240430.161713/tests/fconf_data/1.out/res.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8511904761904762%*

 * *Differences: {"'fconf_test'": "OrderedDict([('var1', 1234)])", "'one'": "{'fconf_test_var1': 1234}"}*

```diff
@@ -1,8 +1,11 @@
 {
+    "fconf_test": {
+        "var1": 1234
+    },
     "macros": [
         "fconf_var(namespace,name)",
         "add_score(self,num)",
         "four(self)",
         "must_be_pkdict(self,arg)",
         "mymap(self,func,args,res,a)",
         "nop(self,arg)",
@@ -36,14 +39,15 @@
         "blue": [
             "before here after",
             {
                 "this": "that"
             }
         ],
         "empty": null,
+        "fconf_test_var1": 1234,
         "inline_array": [
             3.14
         ],
         "item1": "ein",
         "item2": "zwei",
         "item3": [
             "un",
```

### Comparing `pykern-20240412.230110/tests/mpi_data/p1.py` & `pykern-20240430.161713/tests/mpi_data/p1.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/mpi_test.py` & `pykern-20240430.161713/tests/mpi_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkarray_test.py` & `pykern-20240430.161713/tests/pkarray_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkasyncio_test.py` & `pykern-20240430.161713/tests/pkasyncio_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/fmt_data/fmt_dir.out/y.py` & `pykern-20240430.161713/tests/pkcli/fmt_data/fmt_dir.out/y.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/fmt_test.py` & `pykern-20240430.161713/tests/pkcli/fmt_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json` & `pykern-20240430.161713/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_orgmode_test.py` & `pykern-20240430.161713/tests/pkcli/github_orgmode_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/github_test.py` & `pykern-20240430.161713/tests/pkcli/github_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/projex_test.py` & `pykern-20240430.161713/tests/pkcli/projex_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/rsmanifest_test.py` & `pykern-20240430.161713/tests/pkcli/rsmanifest_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/sim_test.py` & `pykern-20240430.161713/tests/pkcli/sim_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/test1_test.py` & `pykern-20240430.161713/tests/pkcli/test1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/test2_test.py` & `pykern-20240430.161713/tests/pkcli/test2_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli/test_test.py` & `pykern-20240430.161713/tests/pkcli/test_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli1_test.py` & `pykern-20240430.161713/tests/pkcli1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcli_test.py` & `pykern-20240430.161713/tests/pkcli_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcollections_test.py` & `pykern-20240430.161713/tests/pkcollections_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkcompat_test.py` & `pykern-20240430.161713/tests/pkcompat_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig1_test.py` & `pykern-20240430.161713/tests/pkconfig1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig2_test.py` & `pykern-20240430.161713/tests/pkconfig2_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig3_test.py` & `pykern-20240430.161713/tests/pkconfig3_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig4_test.py` & `pykern-20240430.161713/tests/pkconfig4_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig5_test.py` & `pykern-20240430.161713/tests/pkconfig5_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig6_test.py` & `pykern-20240430.161713/tests/pkconfig6_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig7_test.py` & `pykern-20240430.161713/tests/pkconfig7_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkconfig_data/p1/m1.py` & `pykern-20240430.161713/tests/pkconfig_data/p1/m1.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkdebug1_test.py` & `pykern-20240430.161713/tests/pkdebug1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkdebug2_test.py` & `pykern-20240430.161713/tests/pkdebug2_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkexample_test.py` & `pykern-20240430.161713/tests/pkexample_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkinspect_test.py` & `pykern-20240430.161713/tests/pkinspect_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkio_data/binary.dat` & `pykern-20240430.161713/tests/pkio_data/binary.dat`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkio_test.py` & `pykern-20240430.161713/tests/pkio_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkjinja_test.py` & `pykern-20240430.161713/tests/pkjinja_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkjson_test.py` & `pykern-20240430.161713/tests/pkjson_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkplatform_test.py` & `pykern-20240430.161713/tests/pkplatform_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkresource_test.py` & `pykern-20240430.161713/tests/pkresource_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkrunpy_test.py` & `pykern-20240430.161713/tests/pkrunpy_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksetup_data/pksetupunit1/.gitignore` & `pykern-20240430.161713/tests/pksetup_data/pksetupunit1/.gitignore`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksetup_data/pksetupunit2/.gitignore` & `pykern-20240430.161713/tests/pksetup_data/pksetupunit2/.gitignore`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksetup_data/pksetupunit2/LICENSE` & `pykern-20240430.161713/tests/pksetup_data/pksetupunit2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksetup_data/pksetupunit2/setup.py` & `pykern-20240430.161713/tests/pksetup_data/pksetupunit2/setup.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksetup_test.py` & `pykern-20240430.161713/tests/pksetup_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pksubprocess_test.py` & `pykern-20240430.161713/tests/pksubprocess_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkunit1_test.py` & `pykern-20240430.161713/tests/pkunit1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkunit_data/example.csv` & `pykern-20240430.161713/tests/pkunit_data/example.csv`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkunit_data/example.xlsx` & `pykern-20240430.161713/tests/pkunit_data/example.xlsx`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkunit_test.py` & `pykern-20240430.161713/tests/pkunit_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/pkyaml_test.py` & `pykern-20240430.161713/tests/pkyaml_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
 """PyTest for :mod:`pykern.pkyaml`
 
 :copyright: Copyright (c) 2015-2022 RadiaSoft LLC.  All Rights Reserved.
 :license: http://www.apache.org/licenses/LICENSE-2.0.html
 """
-import pytest
 
 
 def test_load_dump():
     """Test values are unicode"""
     from pykern import pkunit
     from pykern import pkyaml
```

### Comparing `pykern-20240412.230110/tests/util_test.py` & `pykern-20240430.161713/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/1.in/case.py` & `pykern-20240430.161713/tests/xlsx_data/1.in/case.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml` & `pykern-20240430.161713/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/2.in/case.py` & `pykern-20240430.161713/tests/xlsx_data/2.in/case.py`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/2.in/case2.xlsx` & `pykern-20240430.161713/tests/xlsx_data/2.in/case2.xlsx`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/2.out/xl/styles.xml` & `pykern-20240430.161713/tests/xlsx_data/2.out/xl/styles.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml` & `pykern-20240430.161713/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml` & `pykern-20240430.161713/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240412.230110/tests/xlsx_test.py` & `pykern-20240430.161713/tests/xlsx_test.py`

 * *Files identical despite different names*

