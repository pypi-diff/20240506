# Comparing `tmp/katcp_codec-0.1.0.tar.gz` & `tmp/katcp_codec-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katcp_codec-0.1.0.tar", last modified: Mon May  6 09:25:26 2024, max compression
+gzip compressed data, was "katcp_codec-0.1.0b2.tar", last modified: Mon Apr 15 14:35:23 2024, max compression
```

## Comparing `katcp_codec-0.1.0.tar` & `katcp_codec-0.1.0b2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.717703 katcp_codec-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/.ci/
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.ci/before_all_linux.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    27667 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 09:25:26.717703 katcp_codec-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/benches/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/benches/bench_format.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/benches/bench_parse.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.705703 katcp_codec-0.1.0/crates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/crates/fsm/
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/crates/fsm/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/crates/fsm/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.709703 katcp_codec-0.1.0/crates/fsm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/crates/fsm/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.713703 katcp_codec-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/design.rst
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/katcp_codec.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/doc-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.705703 katcp_codec-0.1.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.713703 katcp_codec-0.1.0/python/katcp_codec/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/python/katcp_codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/python/katcp_codec/_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/python/katcp_codec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.713703 katcp_codec-0.1.0/python/katcp_codec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 09:25:26.000000 katcp_codec-0.1.0/python/katcp_codec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-06 09:25:26.000000 katcp_codec-0.1.0/python/katcp_codec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:25:26.000000 katcp_codec-0.1.0/python/katcp_codec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 09:25:26.000000 katcp_codec-0.1.0/python/katcp_codec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 09:25:26.000000 katcp_codec-0.1.0/python/katcp_codec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.713703 katcp_codec-0.1.0/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/python/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/python/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:25:26.717703 katcp_codec-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:25:26.713703 katcp_codec-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/binding.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/format.rs
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/message.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17037 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/parse.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/tables.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-06 09:25:20.000000 katcp_codec-0.1.0/src/test.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/.ci/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.ci/before_all_linux.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    30267 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/benches/bench_format.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/benches/bench_parse.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.627585 katcp_codec-0.1.0b2/crates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/crates/fsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/crates/fsm/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/crates/fsm/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/crates/fsm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/crates/fsm/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/design.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/katcp_codec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/doc-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.627585 katcp_codec-0.1.0b2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.631585 katcp_codec-0.1.0b2/python/katcp_codec/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/python/katcp_codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/python/katcp_codec/_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/python/katcp_codec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-15 14:35:23.000000 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 14:35:23.000000 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:35:23.000000 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 14:35:23.000000 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 14:35:23.000000 katcp_codec-0.1.0b2/python/katcp_codec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/python/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/python/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:35:23.635585 katcp_codec-0.1.0b2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/binding.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/format.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17037 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/parse.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/tables.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-15 14:35:17.000000 katcp_codec-0.1.0b2/src/test.rs
```

### Comparing `katcp_codec-0.1.0/.github/workflows/test.yml` & `katcp_codec-0.1.0b2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/.pre-commit-config.yaml` & `katcp_codec-0.1.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/.readthedocs.yml` & `katcp_codec-0.1.0b2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/Cargo.lock` & `katcp_codec-0.1.0b2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.7"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "autocfg"
-version = "1.3.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
 dependencies = [
@@ -42,23 +42,29 @@
 name = "bit-vec"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
 
 [[package]]
 name = "bitflags"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+
+[[package]]
+name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.16.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -185,17 +191,17 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "enum-map"
 version = "2.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6866f3bfdf8207509a033af1a75a7b08abda06bbaaeae6669323fd5a097df2e9"
 dependencies = [
@@ -221,46 +227,46 @@
 dependencies = [
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.1.0"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "half"
-version = "2.4.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "heck"
@@ -342,17 +348,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -360,48 +366,48 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.12"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.2"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
-version = "0.9.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.19"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
@@ -413,33 +419,33 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.10"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
@@ -476,46 +482,46 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31b476131c3c86cb68032fdc5cb6d5a1045e3e42d96b69fa599fd77701e1f5bf"
 dependencies = [
  "bit-set",
  "bit-vec",
- "bitflags",
+ "bitflags 2.5.0",
  "lazy_static",
  "num-traits",
  "rand",
  "rand_chacha",
  "rand_xorshift",
  "regex-syntax",
  "rusty-fork",
  "tempfile",
  "unarray",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
+checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -523,49 +529,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
+checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
+checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
+checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
+checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -574,17 +580,17 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.36"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -642,19 +648,19 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.5.1"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -674,23 +680,23 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.3"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "relative-path"
-version = "1.9.3"
+version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba39f3699c378cd8970968dcbff9c43159ea4cfbd88d43c00b22f2ef10a435d2"
+checksum = "e898588f33fdd5b9420719948f9f2a32c922a246964576f71ba7f24f80610fbc"
 
 [[package]]
 name = "rstest"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97eeab2f3c0a199bc4be135c36c924b6590b88c377d416494288c14f2db30199"
 dependencies = [
@@ -722,19 +728,19 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.34"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
@@ -774,54 +780,54 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -840,26 +846,26 @@
  "fastrand",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -982,87 +988,159 @@
 checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
 name = "winapi-util"
-version = "0.1.8"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
- "windows-sys",
+ "winapi",
 ]
 
 [[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.52.4",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.5"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_gnullvm",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.5"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
-name = "windows_i686_gnullvm"
-version = "0.52.5"
+name = "windows_i686_gnu"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.5"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.5"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.5"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
```

### Comparing `katcp_codec-0.1.0/Cargo.toml` & `katcp_codec-0.1.0b2/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 name = "_lib"
 crate-type = ["cdylib", "rlib"]  # rlib included just for testing
 
 [dependencies]
 enum-map = "2.7.3"
 itoa = "1.0.10"
 katcp-codec-fsm = { path = "crates/fsm", features = ["pyo3"] }
-pyo3 = { version = "0.21.0", features = ["extension-module"] }
+pyo3 = { version = "0.21.0-beta.0", features = ["extension-module"] }
 thiserror = "1.0.58"
 uninit = "0.6.2"
 
 [dev-dependencies]
 criterion = "0.5.1"
 proptest = "1.4.0"
 rstest = { version = "0.18.2", default-features = false }
```

### Comparing `katcp_codec-0.1.0/PKG-INFO` & `katcp_codec-0.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katcp-codec
-Version: 0.1.0
+Version: 0.1.0b2
 Summary: Fast encoding and decoding of katcp messages
 Author-email: Bruce Merry <bmerry@sarao.ac.za>
 Project-URL: Homepage, https://github.com/ska-sa/katcp-codec
 Keywords: katcp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
```

### Comparing `katcp_codec-0.1.0/benches/bench_format.rs` & `katcp_codec-0.1.0b2/benches/bench_format.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/benches/bench_parse.rs` & `katcp_codec-0.1.0b2/benches/bench_parse.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/build.rs` & `katcp_codec-0.1.0b2/build.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/crates/fsm/Cargo.lock` & `katcp_codec-0.1.0b2/crates/fsm/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.3.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
-version = "2.5.0"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -58,23 +58,23 @@
 dependencies = [
  "enum-map",
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
-version = "0.4.12"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -89,27 +89,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.10"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -118,26 +118,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
+checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -145,71 +145,71 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
+checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
+checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
+checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
+checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.36"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.5.1"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -220,17 +220,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -249,68 +249,61 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
- "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
-
-[[package]]
-name = "windows_i686_gnullvm"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.5"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
```

### Comparing `katcp_codec-0.1.0/crates/fsm/Cargo.toml` & `katcp_codec-0.1.0b2/crates/fsm/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 edition = "2021"
 
 [features]
 pyo3 = ["dep:pyo3"]
 
 [dependencies]
 enum-map = "2.7.3"
-pyo3 = { version = "0.21.0", features = ["extension-module"], optional = true }
+pyo3 = { version = "0.21.0-beta.0", features = ["extension-module"], optional = true }
```

### Comparing `katcp_codec-0.1.0/crates/fsm/src/lib.rs` & `katcp_codec-0.1.0b2/crates/fsm/src/lib.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/Makefile` & `katcp_codec-0.1.0b2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/conf.py` & `katcp_codec-0.1.0b2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/design.rst` & `katcp_codec-0.1.0b2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/index.rst` & `katcp_codec-0.1.0b2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/introduction.rst` & `katcp_codec-0.1.0b2/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc/usage.rst` & `katcp_codec-0.1.0b2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/doc-requirements.txt` & `katcp_codec-0.1.0b2/doc-requirements.txt`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/pyproject.toml` & `katcp_codec-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/python/katcp_codec/__init__.py` & `katcp_codec-0.1.0b2/python/katcp_codec/__init__.py`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/python/katcp_codec/_lib.pyi` & `katcp_codec-0.1.0b2/python/katcp_codec/_lib.pyi`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/python/katcp_codec.egg-info/PKG-INFO` & `katcp_codec-0.1.0b2/python/katcp_codec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katcp-codec
-Version: 0.1.0
+Version: 0.1.0b2
 Summary: Fast encoding and decoding of katcp messages
 Author-email: Bruce Merry <bmerry@sarao.ac.za>
 Project-URL: Homepage, https://github.com/ska-sa/katcp-codec
 Keywords: katcp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
```

### Comparing `katcp_codec-0.1.0/python/katcp_codec.egg-info/SOURCES.txt` & `katcp_codec-0.1.0b2/python/katcp_codec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/python/tests/test_format.py` & `katcp_codec-0.1.0b2/python/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/python/tests/test_parse.py` & `katcp_codec-0.1.0b2/python/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/requirements.txt` & `katcp_codec-0.1.0b2/requirements.txt`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/binding.rs` & `katcp_codec-0.1.0b2/src/binding.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/format.rs` & `katcp_codec-0.1.0b2/src/format.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/lib.rs` & `katcp_codec-0.1.0b2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/message.rs` & `katcp_codec-0.1.0b2/src/message.rs`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,14 @@
         name: Bound<'py, PyBytes>,
         mid: Option<u32>,
         arguments: Bound<'py, PyList>,
     ) -> Self {
         Self::new(mtype, name.unbind(), mid, arguments.unbind())
     }
 
-    // See https://pyo3.rs/v0.21.2/class/protocols#garbage-collector-integration
     fn __traverse__(&self, visit: PyVisit) -> Result<(), PyTraverseError> {
         if let Some(name) = &self.name {
             visit.call(name)?;
         }
         if let Some(arguments) = &self.arguments {
             visit.call(arguments)?;
         }
@@ -149,15 +148,15 @@
             .name
             .as_ref()
             .ok_or_else(|| PyValueError::new_err("name is None"))?;
         let name = name.bind(py);
         let arguments = self
             .arguments
             .as_ref()
-            .ok_or_else(|| PyValueError::new_err("arguments is None"))?;
+            .ok_or_else(|| PyValueError::new_err("name is None"))?;
         // TODO: this is creating a new vector to hold the arguments.
         // Can we use another trait to handle directly iterating the PyList?
         let arguments: Vec<PyBackedBytes> = arguments.bind(py).extract()?;
         let message = Message {
             mtype: self.mtype,
             name: name.as_bytes(),
             mid: self.mid,
```

### Comparing `katcp_codec-0.1.0/src/parse.rs` & `katcp_codec-0.1.0b2/src/parse.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/tables.rs` & `katcp_codec-0.1.0b2/src/tables.rs`

 * *Files identical despite different names*

### Comparing `katcp_codec-0.1.0/src/test.rs` & `katcp_codec-0.1.0b2/src/test.rs`

 * *Files identical despite different names*

