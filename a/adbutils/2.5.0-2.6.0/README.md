# Comparing `tmp/adbutils-2.5.0.tar.gz` & `tmp/adbutils-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.5.0.tar", last modified: Sun Apr 28 11:05:58 2024, max compression
+gzip compressed data, was "adbutils-2.6.0.tar", last modified: Mon May  6 07:05:42 2024, max compression
```

## Comparing `adbutils-2.5.0.tar` & `adbutils-2.6.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-28 11:05:51.000000 adbutils-2.5.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-28 11:05:51.000000 adbutils-2.5.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 11:05:58.000000 adbutils-2.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-28 11:05:58.000000 adbutils-2.5.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 11:05:51.000000 adbutils-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-28 11:05:58.076576 adbutils-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-28 11:05:51.000000 adbutils-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-28 11:05:51.000000 adbutils-2.5.0/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-28 11:05:51.000000 adbutils-2.5.0/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-28 11:05:51.000000 adbutils-2.5.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 11:05:51.000000 adbutils-2.5.0/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 11:05:51.000000 adbutils-2.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 11:05:51.000000 adbutils-2.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-28 11:05:58.076576 adbutils-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-28 11:05:51.000000 adbutils-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/test_adb_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 07:05:34.000000 adbutils-2.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 07:05:34.000000 adbutils-2.6.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 07:05:42.000000 adbutils-2.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 07:05:42.000000 adbutils-2.6.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 07:05:34.000000 adbutils-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 07:05:42.330343 adbutils-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-06 07:05:34.000000 adbutils-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.322343 adbutils-2.6.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-06 07:05:34.000000 adbutils-2.6.0/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-06 07:05:34.000000 adbutils-2.6.0/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 07:05:34.000000 adbutils-2.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 07:05:34.000000 adbutils-2.6.0/docs/PROTOCOL.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-06 07:05:34.000000 adbutils-2.6.0/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:05:34.000000 adbutils-2.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 07:05:34.000000 adbutils-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 07:05:42.330343 adbutils-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 07:05:34.000000 adbutils-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/test_adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/test_adb_shell.py
```

### Comparing `adbutils-2.5.0/.coveragerc` & `adbutils-2.6.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/.github/workflows/main.yml` & `adbutils-2.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/.github/workflows/publish-to-pypi.yml` & `adbutils-2.6.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/.travis.yml` & `adbutils-2.6.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/LICENSE` & `adbutils-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/PKG-INFO` & `adbutils-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.5.0
+Version: 2.6.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.5.0/README.md` & `adbutils-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,17 @@
 d.is_screen_on() # 返回屏幕是否亮屏 True or False
 
 # adb root
 d.root()
 
 # adb tcpip <port>
 d.tcpip(5555)
+
+print(d.battery())
+BatteryInfo(ac_powered=False, usb_powered=False, wireless_powered=False, dock_powered=False, max_charging_current=0, max_charging_voltage=0, charge_counter=10000, status=4, health=2, present=True, level=100, scale=100, voltage=5000, temperature=25.0, technology='Li-ion')
 ```
 
 Screenrecord (mp4)
 
 ```python
 d.start_recording("video.mp4")
 time.sleep(5)
```

### Comparing `adbutils-2.5.0/adbutils/__init__.py` & `adbutils-2.6.0/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/__main__.py` & `adbutils-2.6.0/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/_adb.py` & `adbutils-2.6.0/adbutils/_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/_deprecated.py` & `adbutils-2.6.0/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/_device.py` & `adbutils-2.6.0/adbutils/_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pathlib
 import re
 import socket
 import subprocess
 import threading
 import typing
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from PIL import Image, UnidentifiedImageError
 
 from adbutils._deprecated import DeprecatedExtension
 from adbutils.install import InstallExtension
 from adbutils.screenrecord import ScreenrecordExtension
 from adbutils.screenshot import ScreenshotExtesion
@@ -69,30 +69,32 @@
         c = self._client.make_connection()
         if timeout:
             c.conn.settimeout(timeout)
 
         if command:
             if self._transport_id:
                 c.send_command(f"host-transport-id:{self._transport_id}:{command}")
+                c.check_okay()
             elif self._serial:
                 c.send_command(f"host-serial:{self._serial}:{command}")
+                c.check_okay()
             else:
                 raise RuntimeError("should not reach here")
-            c.check_okay()
         else:
             if self._transport_id:
                 c.send_command(f"host:transport-id:{self._transport_id}")
+                c.check_okay()
             elif self._serial:
                 # host:tport:serial:xxx is also fine, but receive 12 bytes
                 # recv: 4f 4b 41 59 14 00 00 00 00 00 00 00              OKAY........
-                # so here use host:transport
-                c.send_command(f"host:transport:{self._serial}")
+                c.send_command(f"host:tport:serial:{self._serial}")
+                c.check_okay()
+                c.read(8)  # skip 8 bytes
             else:
                 raise RuntimeError("should not reach here")
-            c.check_okay()
         return c
 
     def _get_with_command(self, cmd: str) -> str:
         c = self.open_transport(cmd)
         return c.read_string_block()
 
     def get_state(self) -> str:
@@ -230,19 +232,25 @@
         returncoode = int(output[rindex + len(MAGIC) :])
         output = output[:rindex]
         if rstrip and encoding:
             output = output.rstrip()
         return ShellReturn(command=cmdargs, returncode=returncoode, output=output)
 
     def forward(self, local: str, remote: str, norebind: bool = False):
-        args = ["forward"]
+        c = self.open_transport()
+        args = ["host:forward"]
         if norebind:
             args.append("norebind")
         args.append(local + ";" + remote)
-        self.open_transport(":".join(args))
+        c.send_command(":".join(args))
+        c.check_okay() # this OKAY means message was received
+        c.check_okay() # check reponse
+        # when successfully forwarded, port string will response, eg: "00041237"
+        # here we just read it and ignore
+        c.read_until_close()
 
     def forward_port(self, remote: Union[int, str]) -> int:
         """forward remote port to local random port"""
         if isinstance(remote, int):
             remote = "tcp:" + str(remote)
         for f in self.forward_list():
             if (
@@ -251,22 +259,24 @@
                 and f.local.startswith("tcp:")
             ):  # yapf: disable
                 return int(f.local[len("tcp:") :])
         local_port = get_free_port()
         self.forward("tcp:" + str(local_port), remote)
         return local_port
 
-    def forward_list(self) -> typing.Iterator[ForwardItem]:
+    def forward_list(self) -> List[ForwardItem]:
         c = self.open_transport("list-forward")
         content = c.read_string_block()
+        items = []
         for line in content.splitlines():
             parts = line.split()
             if len(parts) != 3:
                 continue
-            yield ForwardItem(*parts)
+            items.append(ForwardItem(*parts))
+        return items
 
     def reverse(self, remote: str, local: str, norebind: bool = False):
         """
         Args:
             serial (str): device serial
             remote, local (str):
                 - tcp:<port>
@@ -274,33 +284,38 @@
                 - localreserved:<unix domain socket name>
                 - localfilesystem:<unix domain socket name>
             norebind (bool): fail if already reversed when set to true
 
         Raises:
             AdbError
         """
-        args = ["forward"]
+        c = self.open_transport()
+        args = ["reverse:forward"]
         if norebind:
             args.append("norebind")
-        args.append(local + ";" + remote)
-        self.open_transport(":".join(args))
+        args.append(remote + ";" + local)
+        c.send_command(":".join(args))
+        c.check_okay() # this OKAY means message was received
+        c.check_okay() # check reponse
 
-    def reverse_list(self):
+    def reverse_list(self) -> List[ReverseItem]:
         c = self.open_transport()
         c.send_command("reverse:list-forward")
         c.check_okay()
         content = c.read_string_block()
+        items = []
         for line in content.splitlines():
             parts = line.split()
             if len(parts) != 3:
                 continue
-            yield ReverseItem(*parts[1:])
+            items.append(ReverseItem(*parts[1:]))
+        return items
     
     def framebuffer(self) -> Image.Image:
-        """Capture device screen and return PIL.Image object
+        """Capture device screen and return PIL.Image object (Not very stable)
 
         Raises:
             NotImplementedError
         """
         # Ref: https://android.googlesource.com/platform/system/core/+/android-cts-7.0_r18/adb/framebuffer_service.cpp
         # Ref: https://github.com/DeviceFarmer/adbkit/blob/c16081384ca34addbdab318bda3c76434b7538af/src/adb/command/host-transport/framebuffer.ts
         c = self.open_transport()
```

### Comparing `adbutils-2.5.0/adbutils/_proto.py` & `adbutils-2.6.0/adbutils/_proto.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Network", "DeviceEvent", "ForwardItem", "ReverseItem", "FileInfo",
     "WindowSize", "RunningAppInfo", "ShellReturn", "AdbDeviceInfo", "AppInfo"
 ]
 
 import enum
 import datetime
 import pathlib
-import typing
+from typing import List, NamedTuple, Optional, Union
 from dataclasses import dataclass
 
 
 class Network(str, enum.Enum):
     TCP = "tcp"
     UNIX = "unix"
 
@@ -54,25 +54,44 @@
     mtime: datetime.datetime
     path: str
 
 
 @dataclass
 class AppInfo:
     package_name: str
-    version_name: typing.Optional[str]
-    version_code: typing.Optional[int]
-    flags: str
+    version_name: Optional[str]
+    version_code: Optional[int]
+    flags: Union[str, list]
     first_install_time: datetime.datetime
     last_update_time: datetime.datetime
     signature: str
     path: str
-    sub_apk_paths: typing.List[str]
+    sub_apk_paths: List[str]
 
 
-class WindowSize(typing.NamedTuple):
+@dataclass
+class BatteryInfo:
+    ac_powered: bool
+    usb_powered: bool
+    wireless_powered: Optional[bool]
+    dock_powered: Optional[bool]
+    max_charging_current: Optional[int]
+    max_charging_voltage: Optional[int]
+    charge_counter: Optional[int]
+    status: Optional[int]
+    health: Optional[int]
+    present: Optional[bool]
+    level: Optional[int]
+    scale: Optional[int]
+    voltage: Optional[int] # mV
+    temperature: Optional[float] # e.g. 25.0
+    technology: Optional[str]
+
+
+class WindowSize(NamedTuple):
     width: int
     height: int
 
 
 @dataclass
 class RunningAppInfo:
     package: str
@@ -95,8 +114,8 @@
 
 @dataclass
 class AdbDeviceInfo:
     serial: str
     state: str
 
 
-StrOrPathLike = typing.Union[str, pathlib.Path]
+StrOrPathLike = Union[str, pathlib.Path]
```

### Comparing `adbutils-2.5.0/adbutils/_utils.py` & `adbutils-2.6.0/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/errors.py` & `adbutils-2.6.0/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/install.py` & `adbutils-2.6.0/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/pidcat.py` & `adbutils-2.6.0/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/screenrecord.py` & `adbutils-2.6.0/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/screenshot.py` & `adbutils-2.6.0/adbutils/screenshot.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils/shell.py` & `adbutils-2.6.0/adbutils/shell.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Created on Sun Apr 07 2024 18:44:52 by codeskyblue
 """
 
-
 import abc
 import datetime
 import json
 import re
 import time
 from typing import List, Optional, Union
-from adbutils._proto import WindowSize, AppInfo, RunningAppInfo
+from adbutils._proto import WindowSize, AppInfo, RunningAppInfo, BatteryInfo
 from adbutils.errors import AdbError, AdbInstallError
 from adbutils._utils import escape_special_characters
 from retry import retry
 
 from adbutils.sync import Sync
 
-
 _DISPLAY_RE = re.compile(
     r".*DisplayViewport{.*?valid=true, .*?orientation=(?P<orientation>\d+), .*?deviceWidth=(?P<width>\d+), deviceHeight=(?P<height>\d+).*"
 )
 
 
 def is_percent(v):
     return isinstance(v, float) and v <= 1.0
@@ -214,15 +212,15 @@
             return int(o)
 
         output = self.shell(
             "LD_LIBRARY_PATH=/data/local/tmp /data/local/tmp/minicap -i"
         )
         try:
             if output.startswith("INFO:"):
-                output = output[output.index("{") :]
+                output = output[output.index("{"):]
             data = json.loads(output)
             return data["rotation"] / 90
         except ValueError:
             pass
 
         raise AdbError("rotation get failed")
 
@@ -260,15 +258,15 @@
 
         Args:
             pkg_name (str): package name
         """
         return self.shell(["pm", "uninstall", pkg_name])
 
     def install_remote(
-        self, remote_path: str, clean: bool = False, flags: list = ["-r", "-t"]
+            self, remote_path: str, clean: bool = False, flags: list = ["-r", "-t"]
     ):
         """
         Args:
             remote_path: remote package path
             clean(bool): remove when installed, default(False)
             flags (list): default ["-r", "-t"]
 
@@ -300,15 +298,15 @@
 
     def app_stop(self, package_name: str):
         """stop app with "am force-stop" """
         self.shell(["am", "force-stop", package_name])
 
     def app_clear(self, package_name: str):
         self.shell(["pm", "clear", package_name])
-    
+
     def app_info(self, package_name: str) -> Optional[AppInfo]:
         """
         Get app info
 
         Returns:
             None or AppInfo
         """
@@ -438,8 +436,78 @@
         buf = b''
         for chunk in self.sync.iter_content(target):
             buf += chunk
         xml_data = buf.decode("utf-8")
         if not xml_data.startswith('<?xml'):
             raise AdbError("dump output is not xml", xml_data)
         return xml_data
-    
+
+    def battery(self) -> BatteryInfo:
+        """
+        Get battery info
+
+        Returns:
+            BatteryInfo
+        
+        Details:
+            AC powered - Indicates that the device is currently not powered by AC power. If true, it indicates that the device is connected to an AC power adapter.
+            USB powered - Indicates that the device is currently being powered or charged through the USB interface.
+            Wireless powered - Indicates that the device is not powered through wireless charging. If wireless charging is supported and currently in use, this will be true.
+            Max charging current - The maximum charging current supported by the device, usually in microamperes（ μ A).
+            Max charging voltage - The maximum charging voltage supported by the device may be in millivolts (mV).
+            Charge counter - The cumulative charge count of a battery, usually measured in milliampere hours (mAh)
+            Status - Battery status code.
+            Health - Battery health status code.
+            Present  - indicates that the battery is currently detected and installed in the device.
+            Level - The percentage of current battery level.
+            Scale - The full scale of the percentage of battery charge, indicating that the battery level is measured using 100 as the standard for full charge.
+            Voltage - The current voltage of the battery, usually measured in millivolts (mV).
+            Temperature - Battery temperature, usually measured in degrees Celsius (° C)
+            Technology - Battery type, like (Li-ion) battery
+        """
+        def to_bool(v: str) -> bool:
+            return v == "true"
+        
+        output = self.shell(["dumpsys", "battery"])
+        shell_kvs = {}
+        for line in output.splitlines():
+            key, val = line.strip().split(':', 1)
+            shell_kvs[key.strip()] = val.strip()
+        
+        def get_key(k: str, map_function):
+            v = shell_kvs.get(k)
+            if v is not None:
+                return map_function(v)
+            return None
+        
+        ac_powered = get_key("AC powered", to_bool)
+        usb_powered = get_key("USB powered", to_bool)
+        wireless_powered = get_key("Wireless powered", to_bool)
+        dock_powered = get_key("Dock powered", to_bool)
+        max_charging_current = get_key("Max charging current", int)
+        max_charging_voltage = get_key("Max charging voltage", int)
+        charge_counter = get_key("Charge counter", int)
+        status = get_key("status", int)
+        health = get_key("health", int)
+        present = get_key("present", to_bool)
+        level = get_key("level", int)
+        scale = get_key("scale", int)
+        voltage = get_key("voltage", int)
+        temperature = get_key("temperature", lambda x: int(x) / 10)
+        technology = shell_kvs.get("technology", str)
+        return BatteryInfo(
+            ac_powered=ac_powered,
+            usb_powered=usb_powered,
+            wireless_powered=wireless_powered,
+            dock_powered=dock_powered,
+            max_charging_current=max_charging_current,
+            max_charging_voltage=max_charging_voltage,
+            charge_counter=charge_counter,
+            status=status,
+            health=health,
+            present=present,
+            level=level,
+            scale=scale,
+            voltage=voltage,
+            temperature=temperature,
+            technology=technology,
+        )
```

### Comparing `adbutils-2.5.0/adbutils/sync.py` & `adbutils-2.6.0/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/adbutils.egg-info/PKG-INFO` & `adbutils-2.6.0/adbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.5.0
+Version: 2.6.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.5.0/adbutils.egg-info/SOURCES.txt` & `adbutils-2.6.0/adbutils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,21 @@
 adbutils.egg-info/not-zip-safe
 adbutils.egg-info/pbr.json
 adbutils.egg-info/requires.txt
 adbutils.egg-info/top_level.txt
 adbutils/binaries/README.md
 adbutils/binaries/__init__.py
 assets/images/pidcat.png
+docs/PROTOCOL.md
 examples/reset-offline.py
 test_real_device/conftest.py
 test_real_device/test_adb.py
 test_real_device/test_deprecated.py
 test_real_device/test_device.py
 test_real_device/test_forward_reverse.py
 test_real_device/test_import.py
 test_real_device/test_record.py
 test_real_device/test_utils.py
 tests/adb_server.py
 tests/conftest.py
-tests/test_adb_server.py
+tests/test_adb_server.py
+tests/test_adb_shell.py
```

### Comparing `adbutils-2.5.0/assets/images/pidcat.png` & `adbutils-2.6.0/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/build_wheel.py` & `adbutils-2.6.0/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/examples/reset-offline.py` & `adbutils-2.6.0/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/setup.cfg` & `adbutils-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/test_real_device/test_adb.py` & `adbutils-2.6.0/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/test_real_device/test_deprecated.py` & `adbutils-2.6.0/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/test_real_device/test_device.py` & `adbutils-2.6.0/test_real_device/test_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,33 +35,39 @@
 
 
 def test_shell_stream(device: AdbDevice):
     c = device.shell(["echo", "-n", "hello world"], stream=True)
     output = c.read_until_close()
     assert output == "hello world"
 
+
 def test_adb_shell_raise_timeout(device: AdbDevice):
     with pytest.raises(adbutils.AdbTimeout):
         device.shell("sleep 10", timeout=1.0)
 
+
 def test_shell2(device: AdbDevice):
     cmd = "echo -n 'hello'; false"
     res = device.shell2(cmd)
     assert res.output == "hello"
     assert res.returncode == 1
     assert res.command == cmd
-    
+
 
 def test_get_xxx(device: AdbDevice):
     assert device.get_serialno()
     assert device.get_state() == "device"
     # adb connect device devpath is "unknown"
     # assert device.get_devpath().startswith("usb:")
 
 
+def test_battery(device: AdbDevice):
+    print(device.battery().level)
+
+
 def test_keyevent(device: AdbDevice):
     # make sure no error raised
     device.keyevent(4)
     device.volume_up(2)
     device.volume_down(3)
     device.volume_mute()
 
@@ -122,38 +128,39 @@
     device.sync.push(b"Hello 12", device_tmp_path)
     assert "Hello 12" == device.sync.read_text(device_tmp_path)
 
     target_path = tmp_path / "hi.txt"
     target_path.write_text("Hello Android")
     dst_path = tmp_path / "dst.txt"
     dst_path.unlink(missing_ok=True)
-    
+
     device.sync.push(target_path, device_tmp_path)
     assert "Hello Android" == device.sync.read_text(device_tmp_path)
     device.sync.pull(device_tmp_path, dst_path)
     assert "Hello Android" == dst_path.read_text(encoding="utf-8")
 
     data = b""
     for chunk in device.sync.iter_content(device_tmp_path):
         data += chunk
     assert b"Hello Android" == data
 
+
 def test_sync_pull_file_push(device: AdbDevice, device_tmp_path, tmp_path: pathlib.Path):
     src = io.BytesIO(b"Hello 1")
     device.sync.push(src, device_tmp_path)
     assert b"Hello 1" == device.sync.read_bytes(device_tmp_path)
 
     device.sync.push(b"Hello 12", device_tmp_path)
     assert "Hello 12" == device.sync.read_text(device_tmp_path)
 
     target_path = tmp_path / "hi.txt"
     target_path.write_text("Hello Android")
     dst_path = tmp_path / "dst.txt"
     dst_path.unlink(missing_ok=True)
-    
+
     device.sync.push(target_path, device_tmp_path)
     assert "Hello Android" == device.sync.read_text(device_tmp_path)
     device.sync.pull_file(device_tmp_path, dst_path)
     assert "Hello Android" == dst_path.read_text(encoding="utf-8")
 
     data = b""
     for chunk in device.sync.iter_content(device_tmp_path):
@@ -216,22 +223,23 @@
     device.shell(["log", "-p", "i", "-t", "TAG", "hello"])
     time.sleep(.1)
     logcat.stop()
     assert logcat_path.exists()
     assert re.compile(r"I/TAG.*hello").search(logcat_path.read_text(encoding="utf-8"))
 
 
+
+
 # todo: make independent of already present stuff on the phone
 def test_pull_push_dirs(
-        device: AdbDevice, 
-        device_tmp_dir_path:str, 
-        local_src_in_dir:pathlib.Path, 
-        tmp_path:pathlib.Path, 
-    ):
-
+        device: AdbDevice,
+        device_tmp_dir_path: str,
+        local_src_in_dir: pathlib.Path,
+        tmp_path: pathlib.Path,
+):
     def are_dir_trees_equal(dir1, dir2):
         """
         Compare two directories recursively. Files in each directory are
         assumed to be equal if their names and contents are equal.
 
         NB: retreived from: https://stackoverflow.com/a/6681395
 
@@ -240,45 +248,39 @@
 
         @return: True if the directory trees are the same and 
             there were no errors while accessing the directories or files, 
             False otherwise.
         """
 
         dirs_cmp = filecmp.dircmp(dir1, dir2)
-        if len(dirs_cmp.left_only)>0 or len(dirs_cmp.right_only)>0 or \
-            len(dirs_cmp.funny_files)>0:
+        if len(dirs_cmp.left_only) > 0 or len(dirs_cmp.right_only) > 0 or \
+                len(dirs_cmp.funny_files) > 0:
             return False
-        (_, mismatch, errors) =  filecmp.cmpfiles(
+        (_, mismatch, errors) = filecmp.cmpfiles(
             dir1, dir2, dirs_cmp.common_files, shallow=False)
-        if len(mismatch)>0 or len(errors)>0:
+        if len(mismatch) > 0 or len(errors) > 0:
             return False
         for common_dir in dirs_cmp.common_dirs:
             new_dir1 = os.path.join(dir1, common_dir)
             new_dir2 = os.path.join(dir2, common_dir)
             if not are_dir_trees_equal(new_dir1, new_dir2):
                 return False
         return True
-    
+
     local_src_out_dir1 = tmp_path / 'dir1'
     local_src_out_dir2 = tmp_path / 'dir2'
 
     device.push(local_src_in_dir, device_tmp_dir_path)
 
     device.sync.pull_dir(device_tmp_dir_path, local_src_out_dir1)
 
     assert local_src_out_dir1.exists()
     assert local_src_out_dir1.is_dir()
 
     are_dir_trees_equal(local_src_in_dir, local_src_out_dir1)
-    
 
     device.sync.pull(device_tmp_dir_path, local_src_out_dir2)
 
     assert local_src_out_dir2.exists()
     assert local_src_out_dir2.is_dir()
 
     are_dir_trees_equal(local_src_in_dir, local_src_out_dir2)
-
-
-
-
-
```

### Comparing `adbutils-2.5.0/test_real_device/test_forward_reverse.py` & `adbutils-2.6.0/test_real_device/test_forward_reverse.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             exists = True
     assert exists
 
     lport = device.forward_port("tcp:7912")
     assert isinstance(lport, int)
 
 
-@pytest.mark.skip("skip since it always failed")
 def test_reverse(device: AdbDevice):
     """
     Test commands:
     
         adb reverse --list
         adb -s xxxxx reverse --list
     """
```

### Comparing `adbutils-2.5.0/test_real_device/test_utils.py` & `adbutils-2.6.0/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.5.0/tests/conftest.py` & `adbutils-2.6.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 #
 
 import logging
 import threading
+from unittest import mock
 import adbutils
 import pytest
 import time
 import socket
 from adb_server import run_adb_server
 
 
@@ -24,15 +25,14 @@
     start_time = time.time()
     while True:
         if time.time() - start_time > timeout:
             raise TimeoutError(f"Port {port} is not being listened to within {timeout} seconds")
         if check_port(port) == ready:
             return
         time.sleep(0.1)
-        
 
 
 @pytest.fixture(scope='function')
 def adb_server_fixture():
     th = threading.Thread(target=run_adb_server, name='mock-adb-server')
     th.daemon = True
     th.start()
```

