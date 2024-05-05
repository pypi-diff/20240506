# Comparing `tmp/Jinja2-3.1.3.tar.gz` & `tmp/jinja2-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jinja2-3.1.3.tar", last modified: Wed Jan 10 23:09:26 2024, max compression
+gzip compressed data, was "jinja2-3.1.4.tar", last modified: Sun May  5 23:37:30 2024, max compression
```

## Comparing `Jinja2-3.1.3.tar` & `jinja2-3.1.4.tar`

### file list

```diff
@@ -1,123 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.727756 Jinja2-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    39545 2024-01-10 23:09:17.000000 Jinja2-3.1.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-10 23:09:17.000000 Jinja2-3.1.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-10 23:09:17.000000 Jinja2-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-01-10 23:09:26.727756 Jinja2-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-01-10 23:09:17.000000 Jinja2-3.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.707756 Jinja2-3.1.3/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-01-10 23:09:17.000000 Jinja2-3.1.3/artwork/jinjalogo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.711756 Jinja2-3.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.711756 Jinja2-3.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/_static/jinja-logo-sidebar.png
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/_static/jinja-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    30941 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.711756 Jinja2-3.1.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/examples/cache_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/examples/inline_gettext_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/nativetypes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/sandbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/switching.rst
--rw-r--r--   0 runner    (1001) docker     (127)    62656 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-01-10 23:09:17.000000 Jinja2-3.1.3/docs/tricks.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.703756 Jinja2-3.1.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.711756 Jinja2-3.1.3/examples/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/inheritance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.711756 Jinja2-3.1.3/examples/basic/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/templates/broken.html
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/templates/subbroken.html
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/test_filter_and_linestatements.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/test_loop_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-10 23:09:17.000000 Jinja2-3.1.3/examples/basic/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.715756 Jinja2-3.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-10 23:09:17.000000 Jinja2-3.1.3/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-10 23:09:17.000000 Jinja2-3.1.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-10 23:09:17.000000 Jinja2-3.1.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-10 23:09:17.000000 Jinja2-3.1.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-10 23:09:17.000000 Jinja2-3.1.3/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-01-10 23:09:26.727756 Jinja2-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-10 23:09:17.000000 Jinja2-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.707756 Jinja2-3.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/src/Jinja2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-10 23:09:26.000000 Jinja2-3.1.3/src/Jinja2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.719756 Jinja2-3.1.3/src/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/bccache.py
--rw-r--r--   0 runner    (1001) docker     (127)    72199 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    61253 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31844 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    53862 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/idtracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    29726 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/nativetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    34550 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    39736 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33406 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    23933 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-01-10 23:09:17.000000 Jinja2-3.1.3/src/jinja2/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/tests/res/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/package.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/tests/res/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates/broken.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/tests/res/templates/foo/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates/foo/test.html
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates/mojibake.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates/syntaxerror.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates/test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:09:26.723756 Jinja2-3.1.3/tests/res/templates2/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/res/templates2/foo
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22225 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_async_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_bytecode_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    20316 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_core_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26315 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    32604 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_idtracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    35473 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_lexnparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_nativetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-10 23:09:17.000000 Jinja2-3.1.3/tox.ini
+-rw-r--r--   0        0        0     1475 2024-05-05 23:37:30.000000 jinja2-3.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1607 2024-05-05 23:37:30.000000 jinja2-3.1.4/README.md
+-rw-r--r--   0        0        0      581 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/Makefile
+-rw-r--r--   0        0        0    10484 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/_static/jinja-logo-sidebar.png
+-rw-r--r--   0        0        0    12854 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/_static/jinja-logo.png
+-rw-r--r--   0        0        0    30941 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/api.rst
+-rw-r--r--   0        0        0       45 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/changes.rst
+-rw-r--r--   0        0        0     1950 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/conf.py
+-rw-r--r--   0        0        0     2053 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/examples/cache_extension.py
+-rw-r--r--   0        0        0     2397 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/examples/inline_gettext_extension.py
+-rw-r--r--   0        0        0    12830 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/extensions.rst
+-rw-r--r--   0        0        0     3316 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/faq.rst
+-rw-r--r--   0        0        0      553 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/index.rst
+-rw-r--r--   0        0        0     2754 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/integration.rst
+-rw-r--r--   0        0        0     1976 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/intro.rst
+-rw-r--r--   0        0        0       98 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/license.rst
+-rw-r--r--   0        0        0      757 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/make.bat
+-rw-r--r--   0        0        0     1565 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/nativetypes.rst
+-rw-r--r--   0        0        0     4184 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/sandbox.rst
+-rw-r--r--   0        0        0     4413 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/switching.rst
+-rw-r--r--   0        0        0    62656 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/templates.rst
+-rw-r--r--   0        0        0     3168 2024-05-05 23:37:30.000000 jinja2-3.1.4/docs/tricks.rst
+-rw-r--r--   0        0        0     2126 2024-05-05 23:37:30.000000 jinja2-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/build.in
+-rw-r--r--   0        0        0      294 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/build.txt
+-rw-r--r--   0        0        0       69 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/dev.in
+-rw-r--r--   0        0        0     1181 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/dev.txt
+-rw-r--r--   0        0        0       69 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/docs.in
+-rw-r--r--   0        0        0     1281 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/docs.txt
+-rw-r--r--   0        0        0        7 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/tests.in
+-rw-r--r--   0        0        0      361 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/tests.txt
+-rw-r--r--   0        0        0        5 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/typing.in
+-rw-r--r--   0        0        0      299 2024-05-05 23:37:30.000000 jinja2-3.1.4/requirements/typing.txt
+-rw-r--r--   0        0        0     1928 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/__init__.py
+-rw-r--r--   0        0        0     1958 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/_identifier.py
+-rw-r--r--   0        0        0     2477 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/async_utils.py
+-rw-r--r--   0        0        0    14061 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/bccache.py
+-rw-r--r--   0        0        0    72271 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/compiler.py
+-rw-r--r--   0        0        0     1433 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/constants.py
+-rw-r--r--   0        0        0     6299 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/debug.py
+-rw-r--r--   0        0        0     1267 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/defaults.py
+-rw-r--r--   0        0        0    61538 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/environment.py
+-rw-r--r--   0        0        0     5071 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/exceptions.py
+-rw-r--r--   0        0        0    31877 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/ext.py
+-rw-r--r--   0        0        0    54611 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/filters.py
+-rw-r--r--   0        0        0    10704 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/idtracking.py
+-rw-r--r--   0        0        0    29754 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/lexer.py
+-rw-r--r--   0        0        0    23167 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/loaders.py
+-rw-r--r--   0        0        0     4397 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/meta.py
+-rw-r--r--   0        0        0     4210 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/nativetypes.py
+-rw-r--r--   0        0        0    34579 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/nodes.py
+-rw-r--r--   0        0        0     1651 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/optimizer.py
+-rw-r--r--   0        0        0    39890 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/parser.py
+-rw-r--r--   0        0        0        0 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/py.typed
+-rw-r--r--   0        0        0    33435 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/runtime.py
+-rw-r--r--   0        0        0    14616 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/sandbox.py
+-rw-r--r--   0        0        0     5926 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/tests.py
+-rw-r--r--   0        0        0    23952 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/utils.py
+-rw-r--r--   0        0        0     3557 2024-05-05 23:37:30.000000 jinja2-3.1.4/src/jinja2/visitor.py
+-rw-r--r--   0        0        0     1184 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/package.zip
+-rw-r--r--   0        0        0       26 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates/broken.html
+-rw-r--r--   0        0        0        4 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates/foo/test.html
+-rw-r--r--   0        0        0       13 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates/mojibake.txt
+-rw-r--r--   0        0        0       47 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates/syntaxerror.html
+-rw-r--r--   0        0        0        4 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates/test.html
+-rw-r--r--   0        0        0       99 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/res/templates2/foo
+-rw-r--r--   0        0        0    17046 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_api.py
+-rw-r--r--   0        0        0    22225 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_async.py
+-rw-r--r--   0        0        0     8001 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_async_filters.py
+-rw-r--r--   0        0        0     1984 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_bytecode_cache.py
+-rw-r--r--   0        0        0     1084 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_compile.py
+-rw-r--r--   0        0        0    20316 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_core_tags.py
+-rw-r--r--   0        0        0     3704 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_debug.py
+-rw-r--r--   0        0        0    26315 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_ext.py
+-rw-r--r--   0        0        0    32714 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_filters.py
+-rw-r--r--   0        0        0     8653 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_idtracking.py
+-rw-r--r--   0        0        0     7571 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_imports.py
+-rw-r--r--   0        0        0    13504 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_inheritance.py
+-rw-r--r--   0        0        0    35473 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_lexnparse.py
+-rw-r--r--   0        0        0    14883 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_loader.py
+-rw-r--r--   0        0        0     4275 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_nativetypes.py
+-rw-r--r--   0        0        0       86 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_nodes.py
+-rw-r--r--   0        0        0      148 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_pickle.py
+-rw-r--r--   0        0        0    22250 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_regression.py
+-rw-r--r--   0        0        0     2192 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_runtime.py
+-rw-r--r--   0        0        0     6176 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_security.py
+-rw-r--r--   0        0        0     7851 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_tests.py
+-rw-r--r--   0        0        0     5631 2024-05-05 23:37:30.000000 jinja2-3.1.4/tests/test_utils.py
+-rw-r--r--   0        0        0      890 2024-05-05 23:37:30.000000 jinja2-3.1.4/tox.ini
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 jinja2-3.1.4/PKG-INFO
```

### Comparing `Jinja2-3.1.3/LICENSE.rst` & `jinja2-3.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/README.rst` & `jinja2-3.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Jinja
-=====
+# Jinja
 
 Jinja is a fast, expressive, extensible templating engine. Special
 placeholders in the template allow writing code similar to Python
 syntax. Then the template is passed data to render the final document.
 
 It includes:
 
@@ -22,55 +21,30 @@
 -   Extensible filters, tests, functions, and even syntax.
 
 Jinja's philosophy is that while application logic belongs in Python if
 possible, it shouldn't make the template designer's job difficult by
 restricting functionality too much.
 
 
-Installing
-----------
-
-Install and update using `pip`_:
-
-.. code-block:: text
-
-    $ pip install -U Jinja2
-
-.. _pip: https://pip.pypa.io/en/stable/getting-started/
-
-
-In A Nutshell
--------------
+## In A Nutshell
 
 .. code-block:: jinja
 
     {% extends "base.html" %}
     {% block title %}Members{% endblock %}
     {% block content %}
       <ul>
       {% for user in users %}
         <li><a href="{{ user.url }}">{{ user.username }}</a></li>
       {% endfor %}
       </ul>
     {% endblock %}
 
 
-Donate
-------
+## Donate
 
 The Pallets organization develops and supports Jinja and other popular
 packages. In order to grow the community of contributors and users, and
-allow the maintainers to devote more time to the projects, `please
-donate today`_.
-
-.. _please donate today: https://palletsprojects.com/donate
-
-
-Links
------
+allow the maintainers to devote more time to the projects, [please
+donate today][].
 
--   Documentation: https://jinja.palletsprojects.com/
--   Changes: https://jinja.palletsprojects.com/changes/
--   PyPI Releases: https://pypi.org/project/Jinja2/
--   Source Code: https://github.com/pallets/jinja/
--   Issue Tracker: https://github.com/pallets/jinja/issues/
--   Chat: https://discord.gg/pallets
+[please donate today]: https://palletsprojects.com/donate
```

#### html2text {}

```diff
@@ -1,29 +1,22 @@
-Jinja ===== Jinja is a fast, expressive, extensible templating engine. Special
+# Jinja Jinja is a fast, expressive, extensible templating engine. Special
 placeholders in the template allow writing code similar to Python syntax. Then
 the template is passed data to render the final document. It includes: -
 Template inheritance and inclusion. - Define and import macros within
 templates. - HTML templates can use autoescaping to prevent XSS from untrusted
 user input. - A sandboxed environment can safely render untrusted templates. -
 AsyncIO support for generating templates and calling async functions. - I18N
 support with Babel. - Templates are compiled to optimized Python code just-in-
 time and cached, or can be compiled ahead-of-time. - Exceptions point to the
 correct line in templates to make debugging easier. - Extensible filters,
 tests, functions, and even syntax. Jinja's philosophy is that while application
 logic belongs in Python if possible, it shouldn't make the template designer's
-job difficult by restricting functionality too much. Installing ---------
-- Install and update using `pip`_: .. code-block:: text $ pip install -U Jinja2
-.. _pip: https://pip.pypa.io/en/stable/getting-started/ In A Nutshell ---------
----- .. code-block:: jinja {% extends "base.html" %} {% block title %}Members{%
-endblock %} {% block content %}
+job difficult by restricting functionality too much. ## In A Nutshell .. code-
+block:: jinja {% extends "base.html" %} {% block title %}Members{% endblock %}
+{% block content %}
     * {% for user in users %}
     * _{_{_ _u_s_e_r_._u_s_e_r_n_a_m_e_ _}_}
     * {% endfor %}
-{% endblock %} Donate ------ The Pallets organization develops and supports
-Jinja and other popular packages. In order to grow the community of
-contributors and users, and allow the maintainers to devote more time to the
-projects, `please donate today`_. .. _please donate today: https://
-palletsprojects.com/donate Links ----- - Documentation: https://
-jinja.palletsprojects.com/ - Changes: https://jinja.palletsprojects.com/
-changes/ - PyPI Releases: https://pypi.org/project/Jinja2/ - Source Code:
-https://github.com/pallets/jinja/ - Issue Tracker: https://github.com/pallets/
-jinja/issues/ - Chat: https://discord.gg/pallets
+{% endblock %} ## Donate The Pallets organization develops and supports Jinja
+and other popular packages. In order to grow the community of contributors and
+users, and allow the maintainers to devote more time to the projects, [please
+donate today][]. [please donate today]: https://palletsprojects.com/donate
```

### Comparing `Jinja2-3.1.3/docs/Makefile` & `jinja2-3.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/_static/jinja-logo-sidebar.png` & `jinja2-3.1.4/docs/_static/jinja-logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/_static/jinja-logo.png` & `jinja2-3.1.4/docs/_static/jinja-logo.png`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/api.rst` & `jinja2-3.1.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/conf.py` & `jinja2-3.1.4/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 project = "Jinja"
 copyright = "2007 Pallets"
 author = "Pallets"
 release, version = get_version("Jinja2")
 
 # General --------------------------------------------------------------
 
-master_doc = "index"
+default_role = "code"
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
-    "pallets_sphinx_themes",
     "sphinxcontrib.log_cabinet",
-    "sphinx_issues",
+    "pallets_sphinx_themes",
 ]
+autodoc_member_order = "bysource"
 autodoc_typehints = "description"
-intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
-issues_github_path = "pallets/jinja"
+autodoc_preserve_defaults = True
+extlinks = {
+    "issue": ("https://github.com/pallets/jinja/issues/%s", "#%s"),
+    "pr": ("https://github.com/pallets/jinja/pull/%s", "#%s"),
+    "ghsa": ("https://github.com/advisories/GHSA-%s", "GHSA-%s"),
+}
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3/", None),
+}
 
 # HTML -----------------------------------------------------------------
 
 html_theme = "jinja"
 html_theme_options = {"index_sidebar_logo": False}
 html_context = {
     "project_links": [
@@ -41,11 +49,7 @@
 }
 singlehtml_sidebars = {"index": ["project.html", "localtoc.html", "ethicalads.html"]}
 html_static_path = ["_static"]
 html_favicon = "_static/jinja-logo-sidebar.png"
 html_logo = "_static/jinja-logo-sidebar.png"
 html_title = f"Jinja Documentation ({version})"
 html_show_sourcelink = False
-
-# LaTeX ----------------------------------------------------------------
-
-latex_documents = [(master_doc, f"Jinja-{version}.tex", html_title, author, "manual")]
```

### Comparing `Jinja2-3.1.3/docs/examples/cache_extension.py` & `jinja2-3.1.4/docs/examples/cache_extension.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/examples/inline_gettext_extension.py` & `jinja2-3.1.4/docs/examples/inline_gettext_extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 
 from jinja2.exceptions import TemplateSyntaxError
 from jinja2.ext import Extension
 from jinja2.lexer import count_newlines
 from jinja2.lexer import Token
 
-
 _outside_re = re.compile(r"\\?(gettext|_)\(")
 _inside_re = re.compile(r"\\?[()]")
 
 
 class InlineGettext(Extension):
     """This extension implements support for inline gettext blocks::
```

### Comparing `Jinja2-3.1.3/docs/extensions.rst` & `jinja2-3.1.4/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/faq.rst` & `jinja2-3.1.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/index.rst` & `jinja2-3.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/integration.rst` & `jinja2-3.1.4/docs/integration.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/intro.rst` & `jinja2-3.1.4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/make.bat` & `jinja2-3.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/nativetypes.rst` & `jinja2-3.1.4/docs/nativetypes.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/sandbox.rst` & `jinja2-3.1.4/docs/sandbox.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/switching.rst` & `jinja2-3.1.4/docs/switching.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/templates.rst` & `jinja2-3.1.4/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/docs/tricks.rst` & `jinja2-3.1.4/docs/tricks.rst`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/requirements/dev.txt` & `jinja2-3.1.4/requirements/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     #   virtualenv
 pre-commit==3.3.3
     # via -r requirements/dev.in
 pyproject-api==1.5.2
     # via tox
 pyproject-hooks==1.0.0
     # via build
-pyyaml==6.0
+pyyaml==6.0.1
     # via pre-commit
 toposort==1.10
     # via pip-compile-multi
 tox==4.6.3
     # via -r requirements/dev.in
 virtualenv==20.23.1
     # via
```

### Comparing `Jinja2-3.1.3/requirements/docs.txt` & `jinja2-3.1.4/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/__init__.py` & `jinja2-3.1.4/src/jinja2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Jinja is a template engine written in pure Python. It provides a
 non-XML syntax that supports inline expressions and an optional
 sandboxed environment.
 """
+
 from .bccache import BytecodeCache as BytecodeCache
 from .bccache import FileSystemBytecodeCache as FileSystemBytecodeCache
 from .bccache import MemcachedBytecodeCache as MemcachedBytecodeCache
 from .environment import Environment as Environment
 from .environment import Template as Template
 from .exceptions import TemplateAssertionError as TemplateAssertionError
 from .exceptions import TemplateError as TemplateError
@@ -30,8 +31,8 @@
 from .utils import clear_caches as clear_caches
 from .utils import is_undefined as is_undefined
 from .utils import pass_context as pass_context
 from .utils import pass_environment as pass_environment
 from .utils import pass_eval_context as pass_eval_context
 from .utils import select_autoescape as select_autoescape
 
-__version__ = "3.1.3"
+__version__ = "3.1.4"
```

### Comparing `Jinja2-3.1.3/src/jinja2/_identifier.py` & `jinja2-3.1.4/src/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/async_utils.py` & `jinja2-3.1.4/src/jinja2/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 return async_func(*args, **kwargs)
 
             return normal_func(*args, **kwargs)
 
         if need_eval_context:
             wrapper = pass_eval_context(wrapper)
 
-        wrapper.jinja_async_variant = True
+        wrapper.jinja_async_variant = True  # type: ignore[attr-defined]
         return wrapper
 
     return decorator
 
 
 _common_primitives = {int, float, bool, str, list, dict, tuple, type(None)}
```

### Comparing `Jinja2-3.1.3/src/jinja2/bccache.py` & `jinja2-3.1.4/src/jinja2/bccache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """The optional bytecode cache system. This is useful if you have very
 complex template situations and the compilation of all those templates
 slows down your application too much.
 
 Situations where this is useful are often forking web applications that
 are initialized on the first request.
 """
+
 import errno
 import fnmatch
 import marshal
 import os
 import pickle
 import stat
 import sys
@@ -16,22 +17,23 @@
 import typing as t
 from hashlib import sha1
 from io import BytesIO
 from types import CodeType
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
 
     class _MemcachedClient(te.Protocol):
-        def get(self, key: str) -> bytes:
-            ...
+        def get(self, key: str) -> bytes: ...
 
-        def set(self, key: str, value: bytes, timeout: t.Optional[int] = None) -> None:
-            ...
+        def set(
+            self, key: str, value: bytes, timeout: t.Optional[int] = None
+        ) -> None: ...
 
 
 bc_version = 5
 # Magic bytes to identify Jinja bytecode cache files. Contains the
 # Python major and minor version to avoid loading incompatible bytecode
 # if a project upgrades its Python version.
 bc_magic = (
```

### Comparing `Jinja2-3.1.3/src/jinja2/compiler.py` & `jinja2-3.1.4/src/jinja2/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Compiles nodes from the parser into Python code."""
+
 import typing as t
 from contextlib import contextmanager
 from functools import update_wrapper
 from io import StringIO
 from itertools import chain
 from keyword import iskeyword as is_python_keyword
 
@@ -20,14 +21,15 @@
 from .optimizer import Optimizer
 from .utils import _PassArg
 from .utils import concat
 from .visitor import NodeVisitor
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
 
 F = t.TypeVar("F", bound=t.Callable[..., t.Any])
 
 operators = {
     "eq": "==",
     "ne": "!=",
@@ -56,16 +58,15 @@
     return update_wrapper(t.cast(F, new_func), f)
 
 
 def _make_binop(op: str) -> t.Callable[["CodeGenerator", nodes.BinExpr, "Frame"], None]:
     @optimizeconst
     def visitor(self: "CodeGenerator", node: nodes.BinExpr, frame: Frame) -> None:
         if (
-            self.environment.sandboxed
-            and op in self.environment.intercepted_binops  # type: ignore
+            self.environment.sandboxed and op in self.environment.intercepted_binops  # type: ignore
         ):
             self.write(f"environment.call_binop(context, {op!r}, ")
             self.visit(node.left, frame)
             self.write(", ")
             self.visit(node.right, frame)
         else:
             self.write("(")
@@ -80,16 +81,15 @@
 
 def _make_unop(
     op: str,
 ) -> t.Callable[["CodeGenerator", nodes.UnaryExpr, "Frame"], None]:
     @optimizeconst
     def visitor(self: "CodeGenerator", node: nodes.UnaryExpr, frame: Frame) -> None:
         if (
-            self.environment.sandboxed
-            and op in self.environment.intercepted_unops  # type: ignore
+            self.environment.sandboxed and op in self.environment.intercepted_unops  # type: ignore
         ):
             self.write(f"environment.call_unop(context, {op!r}, ")
             self.visit(node.node, frame)
         else:
             self.write("(" + op)
             self.visit(node.node, frame)
 
@@ -129,15 +129,15 @@
 
     if type(value) in {bool, int, float, complex, range, str, Markup}:
         return True
 
     if type(value) in {tuple, list, set, frozenset}:
         return all(has_safe_repr(v) for v in value)
 
-    if type(value) is dict:
+    if type(value) is dict:  # noqa E721
         return all(has_safe_repr(k) and has_safe_repr(v) for k, v in value.items())
 
     return False
 
 
 def find_undeclared(
     nodes: t.Iterable[nodes.Node], names: t.Iterable[str]
@@ -547,18 +547,21 @@
             runtime instead of compile time.
         """
         visitor = DependencyFinderVisitor()
 
         for node in nodes:
             visitor.visit(node)
 
-        for id_map, names, dependency in (self.filters, visitor.filters, "filters"), (
-            self.tests,
-            visitor.tests,
-            "tests",
+        for id_map, names, dependency in (
+            (self.filters, visitor.filters, "filters"),
+            (
+                self.tests,
+                visitor.tests,
+                "tests",
+            ),
         ):
             for name in sorted(names):
                 if name not in id_map:
                     id_map[name] = self.temporary_identifier()
 
                 # add check during runtime that dependencies used inside of executed
                 # blocks are defined, as this step may be skipped during compile time
@@ -825,15 +828,16 @@
 
     def visit_Template(
         self, node: nodes.Template, frame: t.Optional[Frame] = None
     ) -> None:
         assert frame is None, "no root frame allowed"
         eval_ctx = EvalContext(self.environment, self.name)
 
-        from .runtime import exported, async_exported
+        from .runtime import async_exported
+        from .runtime import exported
 
         if self.environment.is_async:
             exported_names = sorted(exported + async_exported)
         else:
             exported_names = sorted(exported)
 
         self.writeline("from jinja2.runtime import " + ", ".join(exported_names))
```

### Comparing `Jinja2-3.1.3/src/jinja2/constants.py` & `jinja2-3.1.4/src/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/debug.py` & `jinja2-3.1.4/src/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/defaults.py` & `jinja2-3.1.4/src/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/environment.py` & `jinja2-3.1.4/src/jinja2/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Classes for managing templates and their runtime and compile time
 options.
 """
+
 import os
 import typing
 import typing as t
 import weakref
 from collections import ChainMap
 from functools import lru_cache
 from functools import partial
@@ -16,18 +17,18 @@
 from . import nodes
 from .compiler import CodeGenerator
 from .compiler import generate
 from .defaults import BLOCK_END_STRING
 from .defaults import BLOCK_START_STRING
 from .defaults import COMMENT_END_STRING
 from .defaults import COMMENT_START_STRING
-from .defaults import DEFAULT_FILTERS
+from .defaults import DEFAULT_FILTERS  # type: ignore[attr-defined]
 from .defaults import DEFAULT_NAMESPACE
 from .defaults import DEFAULT_POLICIES
-from .defaults import DEFAULT_TESTS
+from .defaults import DEFAULT_TESTS  # type: ignore[attr-defined]
 from .defaults import KEEP_TRAILING_NEWLINE
 from .defaults import LINE_COMMENT_PREFIX
 from .defaults import LINE_STATEMENT_PREFIX
 from .defaults import LSTRIP_BLOCKS
 from .defaults import NEWLINE_SEQUENCE
 from .defaults import TRIM_BLOCKS
 from .defaults import VARIABLE_END_STRING
@@ -51,14 +52,15 @@
 from .utils import import_string
 from .utils import internalcode
 from .utils import LRUCache
 from .utils import missing
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .bccache import BytecodeCache
     from .ext import Extension
     from .loaders import BaseLoader
 
 _env_bound = t.TypeVar("_env_bound", bound="Environment")
 
 
@@ -75,33 +77,33 @@
     env = cls(*args)
     env.shared = True
     return env
 
 
 def create_cache(
     size: int,
-) -> t.Optional[t.MutableMapping[t.Tuple[weakref.ref, str], "Template"]]:
+) -> t.Optional[t.MutableMapping[t.Tuple["weakref.ref[t.Any]", str], "Template"]]:
     """Return the cache class for the given size."""
     if size == 0:
         return None
 
     if size < 0:
         return {}
 
     return LRUCache(size)  # type: ignore
 
 
 def copy_cache(
-    cache: t.Optional[t.MutableMapping],
-) -> t.Optional[t.MutableMapping[t.Tuple[weakref.ref, str], "Template"]]:
+    cache: t.Optional[t.MutableMapping[t.Any, t.Any]],
+) -> t.Optional[t.MutableMapping[t.Tuple["weakref.ref[t.Any]", str], "Template"]]:
     """Create an empty copy of the given cache."""
     if cache is None:
         return None
 
-    if type(cache) is dict:
+    if type(cache) is dict:  # noqa E721
         return {}
 
     return LRUCache(cache.capacity)  # type: ignore
 
 
 def load_extensions(
     environment: "Environment",
@@ -666,15 +668,15 @@
         source = self.preprocess(source, name, filename)
         stream = self.lexer.tokenize(source, name, filename, state)
 
         for ext in self.iter_extensions():
             stream = ext.filter_stream(stream)  # type: ignore
 
             if not isinstance(stream, TokenStream):
-                stream = TokenStream(stream, name, filename)  # type: ignore
+                stream = TokenStream(stream, name, filename)
 
         return stream
 
     def _generate(
         self,
         source: nodes.Template,
         name: t.Optional[str],
@@ -707,27 +709,25 @@
     def compile(  # type: ignore
         self,
         source: t.Union[str, nodes.Template],
         name: t.Optional[str] = None,
         filename: t.Optional[str] = None,
         raw: "te.Literal[False]" = False,
         defer_init: bool = False,
-    ) -> CodeType:
-        ...
+    ) -> CodeType: ...
 
     @typing.overload
     def compile(
         self,
         source: t.Union[str, nodes.Template],
         name: t.Optional[str] = None,
         filename: t.Optional[str] = None,
         raw: "te.Literal[True]" = ...,
         defer_init: bool = False,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     @internalcode
     def compile(
         self,
         source: t.Union[str, nodes.Template],
         name: t.Optional[str] = None,
         filename: t.Optional[str] = None,
@@ -810,15 +810,15 @@
 
         body = [nodes.Assign(nodes.Name("result", "store"), expr, lineno=1)]
         template = self.from_string(nodes.Template(body, lineno=1))
         return TemplateExpression(template, undefined_to_none)
 
     def compile_templates(
         self,
-        target: t.Union[str, os.PathLike],
+        target: t.Union[str, "os.PathLike[str]"],
         extensions: t.Optional[t.Collection[str]] = None,
         filter_func: t.Optional[t.Callable[[str], bool]] = None,
         zip: t.Optional[str] = "deflated",
         log_function: t.Optional[t.Callable[[str], None]] = None,
         ignore_errors: bool = True,
     ) -> None:
         """Finds all the templates the loader can find, compiles them
@@ -854,15 +854,18 @@
                 info.external_attr = 0o755 << 16
                 zip_file.writestr(info, data)
             else:
                 with open(os.path.join(target, filename), "wb") as f:
                     f.write(data.encode("utf8"))
 
         if zip is not None:
-            from zipfile import ZipFile, ZipInfo, ZIP_DEFLATED, ZIP_STORED
+            from zipfile import ZIP_DEFLATED
+            from zipfile import ZIP_STORED
+            from zipfile import ZipFile
+            from zipfile import ZipInfo
 
             zip_file = ZipFile(
                 target, "w", dict(deflated=ZIP_DEFLATED, stored=ZIP_STORED)[zip]
             )
             log_function(f"Compiling into Zip archive {target!r}")
         else:
             if not os.path.isdir(target):
@@ -1413,15 +1416,17 @@
         """As template module creation can invoke template code for
         asynchronous executions this method must be used instead of the
         normal :meth:`make_module` one.  Likewise the module attribute
         becomes unavailable in async mode.
         """
         ctx = self.new_context(vars, shared, locals)
         return TemplateModule(
-            self, ctx, [x async for x in self.root_render_func(ctx)]  # type: ignore
+            self,
+            ctx,
+            [x async for x in self.root_render_func(ctx)],  # type: ignore
         )
 
     @internalcode
     def _get_default_module(self, ctx: t.Optional[Context] = None) -> "TemplateModule":
         """If a context is passed in, this means that the template was
         imported. Imported templates have access to the current
         template's globals by default, but they can only be accessed via
@@ -1584,15 +1589,15 @@
 
     def __init__(self, gen: t.Iterator[str]) -> None:
         self._gen = gen
         self.disable_buffering()
 
     def dump(
         self,
-        fp: t.Union[str, t.IO],
+        fp: t.Union[str, t.IO[bytes]],
         encoding: t.Optional[str] = None,
         errors: t.Optional[str] = "strict",
     ) -> None:
         """Dump the complete stream into a file or file-like object.
         Per default strings are written, if you want to encode
         before writing specify an `encoding`.
 
@@ -1602,30 +1607,33 @@
         """
         close = False
 
         if isinstance(fp, str):
             if encoding is None:
                 encoding = "utf-8"
 
-            fp = open(fp, "wb")
+            real_fp: t.IO[bytes] = open(fp, "wb")
             close = True
+        else:
+            real_fp = fp
+
         try:
             if encoding is not None:
                 iterable = (x.encode(encoding, errors) for x in self)  # type: ignore
             else:
                 iterable = self  # type: ignore
 
-            if hasattr(fp, "writelines"):
-                fp.writelines(iterable)
+            if hasattr(real_fp, "writelines"):
+                real_fp.writelines(iterable)
             else:
                 for item in iterable:
-                    fp.write(item)
+                    real_fp.write(item)
         finally:
             if close:
-                fp.close()
+                real_fp.close()
 
     def disable_buffering(self) -> None:
         """Disable the output buffering."""
         self._next = partial(next, self._gen)
         self.buffered = False
 
     def _buffered_generator(self, size: int) -> t.Iterator[str]:
```

### Comparing `Jinja2-3.1.3/src/jinja2/exceptions.py` & `jinja2-3.1.4/src/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/ext.py` & `jinja2-3.1.4/src/jinja2/ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extension API for adding custom tags and behavior."""
+
 import pprint
 import re
 import typing as t
 
 from markupsafe import Markup
 
 from . import defaults
@@ -14,31 +15,31 @@
 from .runtime import Context
 from .runtime import Undefined
 from .utils import import_string
 from .utils import pass_context
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .lexer import Token
     from .lexer import TokenStream
     from .parser import Parser
 
     class _TranslationsBasic(te.Protocol):
-        def gettext(self, message: str) -> str:
-            ...
+        def gettext(self, message: str) -> str: ...
 
         def ngettext(self, singular: str, plural: str, n: int) -> str:
             pass
 
     class _TranslationsContext(_TranslationsBasic):
-        def pgettext(self, context: str, message: str) -> str:
-            ...
+        def pgettext(self, context: str, message: str) -> str: ...
 
-        def npgettext(self, context: str, singular: str, plural: str, n: int) -> str:
-            ...
+        def npgettext(
+            self, context: str, singular: str, plural: str, n: int
+        ) -> str: ...
 
     _SupportedTranslations = t.Union[_TranslationsBasic, _TranslationsContext]
 
 
 # I18N functions available in Jinja templates. If the I18N library
 # provides ugettext, it will be assigned to gettext.
 GETTEXT_FUNCTIONS: t.Tuple[str, ...] = (
@@ -214,15 +215,15 @@
         # Always treat as a format string, see gettext comment above.
         return rv % variables  # type: ignore
 
     return pgettext
 
 
 def _make_new_npgettext(
-    func: t.Callable[[str, str, str, int], str]
+    func: t.Callable[[str, str, str, int], str],
 ) -> t.Callable[..., str]:
     @pass_context
     def npgettext(
         __context: Context,
         __string_ctx: str,
         __singular: str,
         __plural: str,
@@ -290,22 +291,22 @@
         translations = gettext.NullTranslations()
 
         if hasattr(translations, "pgettext"):
             # Python < 3.8
             pgettext = translations.pgettext
         else:
 
-            def pgettext(c: str, s: str) -> str:
+            def pgettext(c: str, s: str) -> str:  # type: ignore[misc]
                 return s
 
         if hasattr(translations, "npgettext"):
             npgettext = translations.npgettext
         else:
 
-            def npgettext(c: str, s: str, p: str, n: int) -> str:
+            def npgettext(c: str, s: str, p: str, n: int) -> str:  # type: ignore[misc]
                 return s if n == 1 else p
 
         self._install_callables(
             gettext=translations.gettext,
             ngettext=translations.ngettext,
             newstyle=newstyle,
             pgettext=pgettext,
```

### Comparing `Jinja2-3.1.3/src/jinja2/filters.py` & `jinja2-3.1.4/src/jinja2/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built-in template filters used with the ``|`` operator."""
+
 import math
 import random
 import re
 import typing
 import typing as t
 from collections import abc
 from itertools import chain
@@ -24,14 +25,15 @@
 from .utils import pass_eval_context
 from .utils import pformat
 from .utils import url_quote
 from .utils import urlize
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
     from .nodes import EvalContext
     from .runtime import Context
     from .sandbox import SandboxedEnvironment  # noqa: F401
 
     class HasHTML(te.Protocol):
         def __html__(self) -> str:
@@ -118,15 +120,15 @@
 
         return items
 
     return attrgetter
 
 
 def _prepare_attribute_parts(
-    attr: t.Optional[t.Union[str, int]]
+    attr: t.Optional[t.Union[str, int]],
 ) -> t.List[t.Union[str, int]]:
     if attr is None:
         return []
 
     if isinstance(attr, str):
         return [int(x) if x.isdigit() else x for x in attr.split(".")]
 
@@ -138,15 +140,15 @@
     if hasattr(value, "__html__"):
         value = t.cast("HasHTML", value).__html__()
 
     return escape(str(value))
 
 
 def do_urlencode(
-    value: t.Union[str, t.Mapping[str, t.Any], t.Iterable[t.Tuple[str, t.Any]]]
+    value: t.Union[str, t.Mapping[str, t.Any], t.Iterable[t.Tuple[str, t.Any]]],
 ) -> str:
     """Quote data for use in a URL path or query using UTF-8.
 
     Basic wrapper around :func:`urllib.parse.quote` when given a
     string, or :func:`urllib.parse.urlencode` for a dict or iterable.
 
     :param value: Data to quote. A string will be quoted directly. A
@@ -244,25 +246,33 @@
 
     if not isinstance(value, abc.Mapping):
         raise TypeError("Can only get item pairs from a mapping.")
 
     yield from value.items()
 
 
-_space_re = re.compile(r"\s", flags=re.ASCII)
+# Check for characters that would move the parser state from key to value.
+# https://html.spec.whatwg.org/#attribute-name-state
+_attr_key_re = re.compile(r"[\s/>=]", flags=re.ASCII)
 
 
 @pass_eval_context
 def do_xmlattr(
     eval_ctx: "EvalContext", d: t.Mapping[str, t.Any], autospace: bool = True
 ) -> str:
     """Create an SGML/XML attribute string based on the items in a dict.
 
-    If any key contains a space, this fails with a ``ValueError``. Values that
-    are neither ``none`` nor ``undefined`` are automatically escaped.
+    **Values** that are neither ``none`` nor ``undefined`` are automatically
+    escaped, safely allowing untrusted user input.
+
+    User input should not be used as **keys** to this filter. If any key
+    contains a space, ``/`` solidus, ``>`` greater-than sign, or ``=`` equals
+    sign, this fails with a ``ValueError``. Regardless of this, user input
+    should never be used as keys to this filter, or must be separately validated
+    first.
 
     .. sourcecode:: html+jinja
 
         <ul{{ {'class': 'my_list', 'missing': none,
                 'id': 'list-%d'|format(variable)}|xmlattr }}>
         ...
         </ul>
@@ -274,25 +284,29 @@
         <ul class="my_list" id="list-42">
         ...
         </ul>
 
     As you can see it automatically prepends a space in front of the item
     if the filter returned something unless the second parameter is false.
 
+    .. versionchanged:: 3.1.4
+        Keys with ``/`` solidus, ``>`` greater-than sign, or ``=`` equals sign
+        are not allowed.
+
     .. versionchanged:: 3.1.3
         Keys with spaces are not allowed.
     """
     items = []
 
     for key, value in d.items():
         if value is None or isinstance(value, Undefined):
             continue
 
-        if _space_re.search(key) is not None:
-            raise ValueError(f"Spaces are not allowed in attributes: '{key}'")
+        if _attr_key_re.search(key) is not None:
+            raise ValueError(f"Invalid character in attribute name: {key!r}")
 
         items.append(f'{escape(key)}="{escape(value)}"')
 
     rv = " ".join(items)
 
     if autospace and rv:
         rv = " " + rv
@@ -548,15 +562,15 @@
 
     return value
 
 
 @pass_eval_context
 def sync_do_join(
     eval_ctx: "EvalContext",
-    value: t.Iterable,
+    value: t.Iterable[t.Any],
     d: str = "",
     attribute: t.Optional[t.Union[str, int]] = None,
 ) -> str:
     """Return a string which is the concatenation of the strings in the
     sequence. The separator between elements is an empty string per
     default, you can define it with the optional parameter:
 
@@ -606,15 +620,15 @@
     # no html involved, to normal joining
     return soft_str(d).join(map(soft_str, value))
 
 
 @async_variant(sync_do_join)  # type: ignore
 async def do_join(
     eval_ctx: "EvalContext",
-    value: t.Union[t.AsyncIterable, t.Iterable],
+    value: t.Union[t.AsyncIterable[t.Any], t.Iterable[t.Any]],
     d: str = "",
     attribute: t.Optional[t.Union[str, int]] = None,
 ) -> str:
     return sync_do_join(eval_ctx, await auto_to_list(value), d, attribute)
 
 
 def do_center(value: str, width: int = 80) -> str:
@@ -1156,15 +1170,15 @@
 
     func = getattr(math, method)
     return t.cast(float, func(value * (10**precision)) / (10**precision))
 
 
 class _GroupTuple(t.NamedTuple):
     grouper: t.Any
-    list: t.List
+    list: t.List[t.Any]
 
     # Use the regular tuple repr to hide this subclass if users print
     # out the value during debugging.
     def __repr__(self) -> str:
         return tuple.__repr__(self)
 
     def __str__(self) -> str:
@@ -1352,21 +1366,19 @@
 
 def do_mark_unsafe(value: str) -> str:
     """Mark a value as unsafe.  This is the reverse operation for :func:`safe`."""
     return str(value)
 
 
 @typing.overload
-def do_reverse(value: str) -> str:
-    ...
+def do_reverse(value: str) -> str: ...
 
 
 @typing.overload
-def do_reverse(value: "t.Iterable[V]") -> "t.Iterable[V]":
-    ...
+def do_reverse(value: "t.Iterable[V]") -> "t.Iterable[V]": ...
 
 
 def do_reverse(value: t.Union[str, t.Iterable[V]]) -> t.Union[str, t.Iterable[V]]:
     """Reverse the object or return an iterator that iterates over it the other
     way round.
     """
     if isinstance(value, str):
@@ -1412,34 +1424,36 @@
             return value
 
     return environment.undefined(obj=obj, name=name)
 
 
 @typing.overload
 def sync_do_map(
-    context: "Context", value: t.Iterable, name: str, *args: t.Any, **kwargs: t.Any
-) -> t.Iterable:
-    ...
+    context: "Context",
+    value: t.Iterable[t.Any],
+    name: str,
+    *args: t.Any,
+    **kwargs: t.Any,
+) -> t.Iterable[t.Any]: ...
 
 
 @typing.overload
 def sync_do_map(
     context: "Context",
-    value: t.Iterable,
+    value: t.Iterable[t.Any],
     *,
     attribute: str = ...,
     default: t.Optional[t.Any] = None,
-) -> t.Iterable:
-    ...
+) -> t.Iterable[t.Any]: ...
 
 
 @pass_context
 def sync_do_map(
-    context: "Context", value: t.Iterable, *args: t.Any, **kwargs: t.Any
-) -> t.Iterable:
+    context: "Context", value: t.Iterable[t.Any], *args: t.Any, **kwargs: t.Any
+) -> t.Iterable[t.Any]:
     """Applies a filter on a sequence of objects or looks up an attribute.
     This is useful when dealing with lists of objects but you are really
     only interested in a certain value of it.
 
     The basic usage is mapping on an attribute.  Imagine you have a list
     of users but you are only interested in a list of usernames:
 
@@ -1481,40 +1495,38 @@
         for item in value:
             yield func(item)
 
 
 @typing.overload
 def do_map(
     context: "Context",
-    value: t.Union[t.AsyncIterable, t.Iterable],
+    value: t.Union[t.AsyncIterable[t.Any], t.Iterable[t.Any]],
     name: str,
     *args: t.Any,
     **kwargs: t.Any,
-) -> t.Iterable:
-    ...
+) -> t.Iterable[t.Any]: ...
 
 
 @typing.overload
 def do_map(
     context: "Context",
-    value: t.Union[t.AsyncIterable, t.Iterable],
+    value: t.Union[t.AsyncIterable[t.Any], t.Iterable[t.Any]],
     *,
     attribute: str = ...,
     default: t.Optional[t.Any] = None,
-) -> t.Iterable:
-    ...
+) -> t.Iterable[t.Any]: ...
 
 
 @async_variant(sync_do_map)  # type: ignore
 async def do_map(
     context: "Context",
-    value: t.Union[t.AsyncIterable, t.Iterable],
+    value: t.Union[t.AsyncIterable[t.Any], t.Iterable[t.Any]],
     *args: t.Any,
     **kwargs: t.Any,
-) -> t.AsyncIterable:
+) -> t.AsyncIterable[t.Any]:
     if value:
         func = prepare_map(context, args, kwargs)
 
         async for item in auto_aiter(value):
             yield await auto_await(func(item))
 
 
@@ -1699,15 +1711,15 @@
         kwargs = kwargs.copy()
         kwargs["indent"] = indent
 
     return htmlsafe_json_dumps(value, dumps=dumps, **kwargs)
 
 
 def prepare_map(
-    context: "Context", args: t.Tuple, kwargs: t.Dict[str, t.Any]
+    context: "Context", args: t.Tuple[t.Any, ...], kwargs: t.Dict[str, t.Any]
 ) -> t.Callable[[t.Any], t.Any]:
     if not args and "attribute" in kwargs:
         attribute = kwargs.pop("attribute")
         default = kwargs.pop("default", None)
 
         if kwargs:
             raise FilterArgumentError(
@@ -1728,15 +1740,15 @@
             )
 
     return func
 
 
 def prepare_select_or_reject(
     context: "Context",
-    args: t.Tuple,
+    args: t.Tuple[t.Any, ...],
     kwargs: t.Dict[str, t.Any],
     modfunc: t.Callable[[t.Any], t.Any],
     lookup_attr: bool,
 ) -> t.Callable[[t.Any], t.Any]:
     if lookup_attr:
         try:
             attr = args[0]
@@ -1763,15 +1775,15 @@
 
     return lambda item: modfunc(func(transfunc(item)))
 
 
 def select_or_reject(
     context: "Context",
     value: "t.Iterable[V]",
-    args: t.Tuple,
+    args: t.Tuple[t.Any, ...],
     kwargs: t.Dict[str, t.Any],
     modfunc: t.Callable[[t.Any], t.Any],
     lookup_attr: bool,
 ) -> "t.Iterator[V]":
     if value:
         func = prepare_select_or_reject(context, args, kwargs, modfunc, lookup_attr)
 
@@ -1779,15 +1791,15 @@
             if func(item):
                 yield item
 
 
 async def async_select_or_reject(
     context: "Context",
     value: "t.Union[t.AsyncIterable[V], t.Iterable[V]]",
-    args: t.Tuple,
+    args: t.Tuple[t.Any, ...],
     kwargs: t.Dict[str, t.Any],
     modfunc: t.Callable[[t.Any], t.Any],
     lookup_attr: bool,
 ) -> "t.AsyncIterator[V]":
     if value:
         func = prepare_select_or_reject(context, args, kwargs, modfunc, lookup_attr)
```

### Comparing `Jinja2-3.1.3/src/jinja2/idtracking.py` & `jinja2-3.1.4/src/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/lexer.py` & `jinja2-3.1.4/src/jinja2/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Implements a Jinja / Python combination lexer. The ``Lexer`` class
 is used to do some preprocessing. It filters out invalid operators like
 the bitshift operators we don't allow in templates. It separates
 template code and python code in expressions.
 """
+
 import re
 import typing as t
 from ast import literal_eval
 from collections import deque
 from sys import intern
 
 from ._identifier import pattern as name_re
 from .exceptions import TemplateSyntaxError
 from .utils import LRUCache
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
 
 # cache for the lexers. Exists in order to be able to have multiple
 # environments with the same lexer
 _lexer_cache: t.MutableMapping[t.Tuple, "Lexer"] = LRUCache(50)  # type: ignore
 
 # static regular expressions
@@ -443,15 +445,15 @@
 
     if lexer is None:
         _lexer_cache[key] = lexer = Lexer(environment)
 
     return lexer
 
 
-class OptionalLStrip(tuple):
+class OptionalLStrip(tuple):  # type: ignore[type-arg]
     """A special tuple for marking a point in the state that can have
     lstrip applied.
     """
 
     __slots__ = ()
 
     # Even though it looks like a no-op, creating instances fails
```

### Comparing `Jinja2-3.1.3/src/jinja2/loaders.py` & `jinja2-3.1.4/src/jinja2/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """API and implementations for loading templates from different data
 sources.
 """
+
 import importlib.util
 import os
 import posixpath
 import sys
 import typing as t
 import weakref
 import zipimport
@@ -173,15 +174,17 @@
 
     .. versionchanged:: 2.8
         Added the ``followlinks`` parameter.
     """
 
     def __init__(
         self,
-        searchpath: t.Union[str, os.PathLike, t.Sequence[t.Union[str, os.PathLike]]],
+        searchpath: t.Union[
+            str, "os.PathLike[str]", t.Sequence[t.Union[str, "os.PathLike[str]"]]
+        ],
         encoding: str = "utf-8",
         followlinks: bool = False,
     ) -> None:
         if not isinstance(searchpath, abc.Iterable) or isinstance(searchpath, str):
             searchpath = [searchpath]
 
         self.searchpath = [os.fspath(p) for p in searchpath]
@@ -597,15 +600,18 @@
 
     Templates can be precompiled with :meth:`Environment.compile_templates`.
     """
 
     has_source_access = False
 
     def __init__(
-        self, path: t.Union[str, os.PathLike, t.Sequence[t.Union[str, os.PathLike]]]
+        self,
+        path: t.Union[
+            str, "os.PathLike[str]", t.Sequence[t.Union[str, "os.PathLike[str]"]]
+        ],
     ) -> None:
         package_name = f"_jinja2_module_templates_{id(self):x}"
 
         # create a fake module that looks for the templates in the
         # path given.
         mod = _TemplateModule(package_name)
```

### Comparing `Jinja2-3.1.3/src/jinja2/meta.py` & `jinja2-3.1.4/src/jinja2/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Functions that expose information about templates that might be
 interesting for introspection.
 """
+
 import typing as t
 
 from . import nodes
 from .compiler import CodeGenerator
 from .compiler import Frame
 
 if t.TYPE_CHECKING:
```

### Comparing `Jinja2-3.1.3/src/jinja2/nativetypes.py` & `jinja2-3.1.4/src/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/src/jinja2/nodes.py` & `jinja2-3.1.4/src/jinja2/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """AST nodes generated by the parser for the compiler. Also provides
 some node tree helper functions used by the parser and compiler in order
 to normalize nodes.
 """
+
 import inspect
 import operator
 import typing as t
 from collections import deque
 
 from markupsafe import Markup
 
 from .utils import _PassArg
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
 
 _NodeBound = t.TypeVar("_NodeBound", bound="Node")
 
 _binop_to_func: t.Dict[str, t.Callable[[t.Any, t.Any], t.Any]] = {
     "*": operator.mul,
     "/": operator.truediv,
@@ -52,15 +54,15 @@
 class NodeType(type):
     """A metaclass for nodes that handles the field and attribute
     inheritance.  fields and attributes from the parent class are
     automatically forwarded to the child."""
 
     def __new__(mcs, name, bases, d):  # type: ignore
         for attr in "fields", "attributes":
-            storage = []
+            storage: t.List[t.Tuple[str, ...]] = []
             storage.extend(getattr(bases[0] if bases else object, attr, ()))
             storage.extend(d.get(attr, ()))
             assert len(bases) <= 1, "multiple inheritance not allowed"
             assert len(storage) == len(set(storage)), "layout conflict"
             d[attr] = tuple(storage)
         d.setdefault("abstract", False)
         return type.__new__(mcs, name, bases, d)
```

### Comparing `Jinja2-3.1.3/src/jinja2/optimizer.py` & `jinja2-3.1.4/src/jinja2/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Because the AST does not contain all the scoping information and the
 compiler has to find that out, we cannot do all the optimizations we
 want. For example, loop unrolling doesn't work because unrolled loops
 would have a different scope. The solution would be a second syntax tree
 that stored the scoping rules.
 """
+
 import typing as t
 
 from . import nodes
 from .visitor import NodeTransformer
 
 if t.TYPE_CHECKING:
     from .environment import Environment
```

### Comparing `Jinja2-3.1.3/src/jinja2/parser.py` & `jinja2-3.1.4/src/jinja2/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Parse tokens from the lexer into nodes for the compiler."""
+
 import typing
 import typing as t
 
 from . import nodes
 from .exceptions import TemplateAssertionError
 from .exceptions import TemplateSyntaxError
 from .lexer import describe_token
 from .lexer import describe_token_expr
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
+
     from .environment import Environment
 
 _ImportInclude = t.TypeVar("_ImportInclude", nodes.Import, nodes.Include)
 _MacroCall = t.TypeVar("_MacroCall", nodes.Macro, nodes.CallBlock)
 
 _statement_keywords = frozenset(
     [
@@ -453,26 +455,24 @@
                 self.stream.expect("comma")
             node.nodes.append(self.parse_expression())
         return node
 
     @typing.overload
     def parse_assign_target(
         self, with_tuple: bool = ..., name_only: "te.Literal[True]" = ...
-    ) -> nodes.Name:
-        ...
+    ) -> nodes.Name: ...
 
     @typing.overload
     def parse_assign_target(
         self,
         with_tuple: bool = True,
         name_only: bool = False,
         extra_end_rules: t.Optional[t.Tuple[str, ...]] = None,
         with_namespace: bool = False,
-    ) -> t.Union[nodes.NSRef, nodes.Name, nodes.Tuple]:
-        ...
+    ) -> t.Union[nodes.NSRef, nodes.Name, nodes.Tuple]: ...
 
     def parse_assign_target(
         self,
         with_tuple: bool = True,
         name_only: bool = False,
         extra_end_rules: t.Optional[t.Tuple[str, ...]] = None,
         with_namespace: bool = False,
@@ -857,15 +857,22 @@
             else:
                 args.append(None)
         else:
             args.append(None)
 
         return nodes.Slice(lineno=lineno, *args)  # noqa: B026
 
-    def parse_call_args(self) -> t.Tuple:
+    def parse_call_args(
+        self,
+    ) -> t.Tuple[
+        t.List[nodes.Expr],
+        t.List[nodes.Keyword],
+        t.Optional[nodes.Expr],
+        t.Optional[nodes.Expr],
+    ]:
         token = self.stream.expect("lparen")
         args = []
         kwargs = []
         dyn_args = None
         dyn_kwargs = None
         require_comma = False
 
@@ -948,15 +955,15 @@
         else:
             negated = False
         name = self.stream.expect("name").value
         while self.stream.current.type == "dot":
             next(self.stream)
             name += "." + self.stream.expect("name").value
         dyn_args = dyn_kwargs = None
-        kwargs = []
+        kwargs: t.List[nodes.Keyword] = []
         if self.stream.current.type == "lparen":
             args, kwargs, dyn_args, dyn_kwargs = self.parse_call_args()
         elif self.stream.current.type in {
             "name",
             "string",
             "integer",
             "float",
```

### Comparing `Jinja2-3.1.3/src/jinja2/runtime.py` & `jinja2-3.1.4/src/jinja2/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The runtime functions and state used by compiled templates."""
+
 import functools
 import sys
 import typing as t
 from collections import abc
 from itertools import chain
 
 from markupsafe import escape  # noqa: F401
@@ -24,25 +25,26 @@
 from .utils import pass_eval_context
 
 V = t.TypeVar("V")
 F = t.TypeVar("F", bound=t.Callable[..., t.Any])
 
 if t.TYPE_CHECKING:
     import logging
+
     import typing_extensions as te
+
     from .environment import Environment
 
     class LoopRenderFunc(te.Protocol):
         def __call__(
             self,
             reciter: t.Iterable[V],
             loop_render_func: "LoopRenderFunc",
             depth: int = 0,
-        ) -> str:
-            ...
+        ) -> str: ...
 
 
 # these variables are exported to the template runtime
 exported = [
     "LoopContext",
     "TemplateReference",
     "Macro",
@@ -255,15 +257,18 @@
             return self.parent
         if not self.parent:
             return self.vars
         return dict(self.parent, **self.vars)
 
     @internalcode
     def call(
-        __self, __obj: t.Callable, *args: t.Any, **kwargs: t.Any  # noqa: B902
+        __self,
+        __obj: t.Callable[..., t.Any],
+        *args: t.Any,
+        **kwargs: t.Any,  # noqa: B902
     ) -> t.Union[t.Any, "Undefined"]:
         """Call the callable with the arguments and keyword arguments
         provided but inject the active context or environment as first
         argument if the callable has :func:`pass_context` or
         :func:`pass_environment`.
         """
         if __debug__:
@@ -582,15 +587,15 @@
 
 
 class AsyncLoopContext(LoopContext):
     _iterator: t.AsyncIterator[t.Any]  # type: ignore
 
     @staticmethod
     def _to_iterator(  # type: ignore
-        iterable: t.Union[t.Iterable[V], t.AsyncIterable[V]]
+        iterable: t.Union[t.Iterable[V], t.AsyncIterable[V]],
     ) -> t.AsyncIterator[V]:
         return auto_aiter(iterable)
 
     @property
     async def length(self) -> int:  # type: ignore
         if self._length is not None:
             return self._length
```

### Comparing `Jinja2-3.1.3/src/jinja2/sandbox.py` & `jinja2-3.1.4/src/jinja2/sandbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """A sandbox layer that ensures unsafe operations cannot be performed.
 Useful when the template itself comes from an untrusted source.
 """
+
 import operator
 import types
 import typing as t
-from _string import formatter_field_name_split  # type: ignore
 from collections import abc
 from collections import deque
 from string import Formatter
 
+from _string import formatter_field_name_split  # type: ignore
 from markupsafe import EscapeFormatter
 from markupsafe import Markup
 
 from .environment import Environment
 from .exceptions import SecurityError
 from .runtime import Context
 from .runtime import Undefined
@@ -33,15 +34,15 @@
 
 #: unsafe attributes on coroutines
 UNSAFE_COROUTINE_ATTRIBUTES = {"cr_frame", "cr_code"}
 
 #: unsafe attributes on async generators
 UNSAFE_ASYNC_GENERATOR_ATTRIBUTES = {"ag_code", "ag_frame"}
 
-_mutable_spec: t.Tuple[t.Tuple[t.Type, t.FrozenSet[str]], ...] = (
+_mutable_spec: t.Tuple[t.Tuple[t.Type[t.Any], t.FrozenSet[str]], ...] = (
     (
         abc.MutableSet,
         frozenset(
             [
                 "add",
                 "clear",
                 "difference_update",
@@ -76,15 +77,15 @@
                 "rotate",
             ]
         ),
     ),
 )
 
 
-def inspect_format_method(callable: t.Callable) -> t.Optional[str]:
+def inspect_format_method(callable: t.Callable[..., t.Any]) -> t.Optional[str]:
     if not isinstance(
         callable, (types.MethodType, types.BuiltinMethodType)
     ) or callable.__name__ not in ("format", "format_map"):
         return None
 
     obj = callable.__self__
 
@@ -346,15 +347,15 @@
         )
 
     def format_string(
         self,
         s: str,
         args: t.Tuple[t.Any, ...],
         kwargs: t.Dict[str, t.Any],
-        format_func: t.Optional[t.Callable] = None,
+        format_func: t.Optional[t.Callable[..., t.Any]] = None,
     ) -> str:
         """If a format call is detected, then this is routed through this
         method so that our safety sandbox can be used for it.
         """
         formatter: SandboxedFormatter
         if isinstance(s, Markup):
             formatter = SandboxedEscapeFormatter(self, escape=s.escape)
```

### Comparing `Jinja2-3.1.3/src/jinja2/tests.py` & `jinja2-3.1.4/src/jinja2/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built-in template tests used with the ``is`` operator."""
+
 import operator
 import typing as t
 from collections import abc
 from numbers import Number
 
 from .runtime import Undefined
 from .utils import pass_environment
@@ -165,15 +166,15 @@
 
 def test_sequence(value: t.Any) -> bool:
     """Return true if the variable is a sequence. Sequences are variables
     that are iterable.
     """
     try:
         len(value)
-        value.__getitem__
+        value.__getitem__  # noqa B018
     except Exception:
         return False
 
     return True
 
 
 def test_sameas(value: t.Any, other: t.Any) -> bool:
@@ -200,15 +201,15 @@
 
 
 def test_escaped(value: t.Any) -> bool:
     """Check if the value is escaped."""
     return hasattr(value, "__html__")
 
 
-def test_in(value: t.Any, seq: t.Container) -> bool:
+def test_in(value: t.Any, seq: t.Container[t.Any]) -> bool:
     """Check if value is in seq.
 
     .. versionadded:: 2.10
     """
     return value in seq
```

### Comparing `Jinja2-3.1.3/src/jinja2/utils.py` & `jinja2-3.1.4/src/jinja2/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             return __import__(import_name)
         return getattr(__import__(module, None, None, [obj]), obj)
     except (ImportError, AttributeError):
         if not silent:
             raise
 
 
-def open_if_exists(filename: str, mode: str = "rb") -> t.Optional[t.IO]:
+def open_if_exists(filename: str, mode: str = "rb") -> t.Optional[t.IO[t.Any]]:
     """Returns a file descriptor for the filename if that file exists,
     otherwise ``None``.
     """
     if not os.path.isfile(filename):
         return None
 
     return open(filename, mode)
@@ -446,15 +446,15 @@
             "_queue": self._queue,
         }
 
     def __setstate__(self, d: t.Mapping[str, t.Any]) -> None:
         self.__dict__.update(d)
         self._postinit()
 
-    def __getnewargs__(self) -> t.Tuple:
+    def __getnewargs__(self) -> t.Tuple[t.Any, ...]:
         return (self.capacity,)
 
     def copy(self) -> "LRUCache":
         """Return a shallow copy of the instance."""
         rv = self.__class__(self.capacity)
         rv._mapping.update(self._mapping)
         rv._queue.extend(self._queue)
```

### Comparing `Jinja2-3.1.3/src/jinja2/visitor.py` & `jinja2-3.1.4/src/jinja2/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """API for traversing the AST nodes. Implemented by the compiler and
 meta introspection.
 """
+
 import typing as t
 
 from .nodes import Node
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     class VisitCallable(te.Protocol):
-        def __call__(self, node: Node, *args: t.Any, **kwargs: t.Any) -> t.Any:
-            ...
+        def __call__(self, node: Node, *args: t.Any, **kwargs: t.Any) -> t.Any: ...
 
 
 class NodeVisitor:
     """Walks the abstract syntax tree and call visitor functions for every
     node found.  The visitor functions may return values which will be
     forwarded by the `visit` method.
```

### Comparing `Jinja2-3.1.3/tests/conftest.py` & `jinja2-3.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/res/package.zip` & `jinja2-3.1.4/tests/res/package.zip`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_api.py` & `jinja2-3.1.4/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,16 @@
         assert t.render(foo="<foo>") == "<foo>"
         t = env.get_template("test.html")
         assert t.render(foo="<foo>") == "&lt;foo&gt;"
         t = env.from_string("{{ foo }}")
         assert t.render(foo="<foo>") == "<foo>"
 
     def test_sandbox_max_range(self, env):
-        from jinja2.sandbox import SandboxedEnvironment, MAX_RANGE
+        from jinja2.sandbox import MAX_RANGE
+        from jinja2.sandbox import SandboxedEnvironment
 
         env = SandboxedEnvironment()
         t = env.from_string("{% for item in range(total) %}{{ item }}{% endfor %}")
 
         with pytest.raises(OverflowError):
             t.render(total=MAX_RANGE + 1)
 
@@ -260,15 +261,15 @@
         t = Template("A{{ test() }}B")
         assert t.render(test=test) == "AB"
         t = Template("A{{ test().missingattribute }}B")
         pytest.raises(UndefinedError, t.render, test=test)
 
     def test_undefined_and_special_attributes(self):
         with pytest.raises(AttributeError):
-            Undefined("Foo").__dict__
+            Undefined("Foo").__dict__  # noqa B018
 
     def test_undefined_attribute_error(self):
         # Django's LazyObject turns the __class__ attribute into a
         # property that resolves the wrapped function. If that wrapped
         # function raises an AttributeError, printing the repr of the
         # object in the undefined message would cause a RecursionError.
         class Error:
```

### Comparing `Jinja2-3.1.3/tests/test_async.py` & `jinja2-3.1.4/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_async_filters.py` & `jinja2-3.1.4/tests/test_async_filters.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_bytecode_cache.py` & `jinja2-3.1.4/tests/test_bytecode_cache.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_compile.py` & `jinja2-3.1.4/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_core_tags.py` & `jinja2-3.1.4/tests/test_core_tags.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_debug.py` & `jinja2-3.1.4/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_ext.py` & `jinja2-3.1.4/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_filters.py` & `jinja2-3.1.4/tests/test_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,19 +470,20 @@
         )
         out = tmpl.render().split()
         assert len(out) == 3
         assert 'foo="42"' in out
         assert 'bar="23"' in out
         assert 'blub:blub="&lt;?&gt;"' in out
 
-    def test_xmlattr_key_with_spaces(self, env):
-        with pytest.raises(ValueError, match="Spaces are not allowed"):
-            env.from_string(
-                "{{ {'src=1 onerror=alert(1)': 'my_class'}|xmlattr }}"
-            ).render()
+    @pytest.mark.parametrize("sep", ("\t", "\n", "\f", " ", "/", ">", "="))
+    def test_xmlattr_key_invalid(self, env: Environment, sep: str) -> None:
+        with pytest.raises(ValueError, match="Invalid character"):
+            env.from_string("{{ {key: 'my_class'}|xmlattr }}").render(
+                key=f"class{sep}onclick=alert(1)"
+            )
 
     def test_sort1(self, env):
         tmpl = env.from_string("{{ [2, 3, 1]|sort }}|{{ [2, 3, 1]|sort(true) }}")
         assert tmpl.render() == "[1, 2, 3]|[3, 2, 1]"
 
     def test_sort2(self, env):
         tmpl = env.from_string('{{ "".join(["c", "A", "b", "D"]|sort) }}')
```

### Comparing `Jinja2-3.1.3/tests/test_idtracking.py` & `jinja2-3.1.4/tests/test_idtracking.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_imports.py` & `jinja2-3.1.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_inheritance.py` & `jinja2-3.1.4/tests/test_inheritance.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,30 +361,29 @@
 
         with pytest.raises(TemplateSyntaxError):
             tmpl.render(default="default2", seq=list(range(3)))
 
 
 class TestBugFix:
     def test_fixed_macro_scoping_bug(self, env):
-        assert (
-            Environment(
-                loader=DictLoader(
-                    {
-                        "test.html": """\
+        assert Environment(
+            loader=DictLoader(
+                {
+                    "test.html": """\
         {% extends 'details.html' %}
 
         {% macro my_macro() %}
         my_macro
         {% endmacro %}
 
         {% block inner_box %}
             {{ my_macro() }}
         {% endblock %}
             """,
-                        "details.html": """\
+                    "details.html": """\
         {% extends 'standard.html' %}
 
         {% macro my_macro() %}
         my_macro
         {% endmacro %}
 
         {% block content %}
@@ -392,25 +391,20 @@
                 outer_box
                 {% block inner_box %}
                     inner_box
                 {% endblock %}
             {% endblock %}
         {% endblock %}
         """,
-                        "standard.html": """
+                    "standard.html": """
         {% block content %}&nbsp;{% endblock %}
         """,
-                    }
-                )
+                }
             )
-            .get_template("test.html")
-            .render()
-            .split()
-            == ["outer_box", "my_macro"]
-        )
+        ).get_template("test.html").render().split() == ["outer_box", "my_macro"]
 
     def test_double_extends(self, env):
         """Ensures that a template with more than 1 {% extends ... %} usage
         raises a ``TemplateError``.
         """
         with pytest.raises(TemplateRuntimeError, match="extended multiple times"):
             env.get_template("doublee").render()
```

### Comparing `Jinja2-3.1.3/tests/test_lexnparse.py` & `jinja2-3.1.4/tests/test_lexnparse.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_loader.py` & `jinja2-3.1.4/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_nativetypes.py` & `jinja2-3.1.4/tests/test_nativetypes.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_regression.py` & `jinja2-3.1.4/tests/test_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,14 +595,15 @@
         tmpl = env.from_string(
             "{%- for value in values recursive %}1{% else %}0{% endfor -%}"
         )
         assert tmpl.render(values=[]) == "0"
 
     def test_markup_and_chainable_undefined(self):
         from markupsafe import Markup
+
         from jinja2.runtime import ChainableUndefined
 
         assert str(Markup(ChainableUndefined())) == ""
 
     def test_scoped_block_loop_vars(self, env):
         tmpl = env.from_string(
             """\
```

### Comparing `Jinja2-3.1.3/tests/test_runtime.py` & `jinja2-3.1.4/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_security.py` & `jinja2-3.1.4/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_tests.py` & `jinja2-3.1.4/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tests/test_utils.py` & `jinja2-3.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Jinja2-3.1.3/tox.ini` & `jinja2-3.1.4/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -6,22 +6,38 @@
     typing
     docs
 skip_missing_interpreters = true
 
 [testenv]
 package = wheel
 wheel_build_env = .pkg
+constrain_package_deps = true
+use_frozen_constraints = true
 deps = -r requirements/tests.txt
 commands = pytest -v --tb=short --basetemp={envtmpdir} {posargs}
 
 [testenv:style]
 deps = pre-commit
 skip_install = true
 commands = pre-commit run --all-files
 
 [testenv:typing]
 deps = -r requirements/typing.txt
 commands = mypy
 
 [testenv:docs]
 deps = -r requirements/docs.txt
-commands = sphinx-build -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
+commands = sphinx-build -E -W -b dirhtml docs docs/_build/dirhtml
+
+[testenv:update-requirements]
+deps =
+    pip-tools
+    pre-commit
+skip_install = true
+change_dir = requirements
+commands =
+    pre-commit autoupdate -j4
+    pip-compile -U build.in
+    pip-compile -U docs.in
+    pip-compile -U tests.in
+    pip-compile -U typing.in
+    pip-compile -U dev.in
```

