# Comparing `tmp/homematicip-1.1.0.post1.dev16.tar.gz` & `tmp/homematicip-1.1.0.post1.dev21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homematicip-1.1.0.post1.dev16.tar", last modified: Sat May  4 22:36:10 2024, max compression
+gzip compressed data, was "homematicip-1.1.0.post1.dev21.tar", last modified: Mon May  6 16:15:01 2024, max compression
```

## Comparing `homematicip-1.1.0.post1.dev16.tar` & `homematicip-1.1.0.post1.dev21.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.545278 homematicip-1.1.0.post1.dev16/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.529278 homematicip-1.1.0.post1.dev16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/test-on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.529278 homematicip-1.1.0.post1.dev16/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/api_introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.aio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/sample_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/sample_data/json_data/
--rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/security_journal.json
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/unknown_types.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:36:10.545278 homematicip-1.1.0.post1.dev16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/src/homematicip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/action_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/functional_channel_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/group_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli_debug_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/log_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_token_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/rest_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/config_not_found_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/src/homematicip/model/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/anoymizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    52256 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/functional_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/hmip_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_action_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_functional_channel_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_group_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/connection/test_client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/connection/test_rest_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/events/test_hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/model/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/test_functional_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.503858 homematicip-1.1.0.post1.dev21/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.507858 homematicip-1.1.0.post1.dev21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.github/workflows/test-on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.507858 homematicip-1.1.0.post1.dev21/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.511858 homematicip-1.1.0.post1.dev21/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.511858 homematicip-1.1.0.post1.dev21/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/api_introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/homematicip.aio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/homematicip.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/homematicip.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.503858 homematicip-1.1.0.post1.dev21/sample_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.511858 homematicip-1.1.0.post1.dev21/sample_data/json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/sample_data/json_data/home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/sample_data/json_data/security_journal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/sample_data/json_data/unknown_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.503858 homematicip-1.1.0.post1.dev21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.511858 homematicip-1.1.0.post1.dev21/src/homematicip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/action/action_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/action/functional_channel_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/action/group_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/cli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44297 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/cli/hmip.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/cli/hmip_cli_debug_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/configuration/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/configuration/config_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/configuration/log_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/connection/client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/connection/client_token_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/connection/rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/events/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/events/hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.515858 homematicip-1.1.0.post1.dev21/src/homematicip/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/exceptions/config_not_found_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/src/homematicip/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/anoymizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52256 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/functional_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/hmip_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/src/homematicip/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 16:15:01.000000 homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/actions/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/actions/test_action_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/actions/test_functional_channel_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/actions/test_group_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/cli/test_hmip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/connection/test_client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/connection/test_rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/events/test_hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:15:01.519858 homematicip-1.1.0.post1.dev21/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/model/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/model/test_functional_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-06 16:14:54.000000 homematicip-1.1.0.post1.dev21/tests/test_runner.py
```

### Comparing `homematicip-1.1.0.post1.dev16/.github/workflows/build-docs.yml` & `homematicip-1.1.0.post1.dev21/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/.github/workflows/codeql-analysis.yml` & `homematicip-1.1.0.post1.dev21/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/.github/workflows/publish.yml` & `homematicip-1.1.0.post1.dev21/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/.github/workflows/test-on-push.yml` & `homematicip-1.1.0.post1.dev21/.github/workflows/test-on-push.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/.gitignore` & `homematicip-1.1.0.post1.dev21/.gitignore`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/CHANGELOG.md` & `homematicip-1.1.0.post1.dev21/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/CODE_OF_CONDUCT.md` & `homematicip-1.1.0.post1.dev21/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/LICENSE.txt` & `homematicip-1.1.0.post1.dev21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/PKG-INFO` & `homematicip-1.1.0.post1.dev21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.1.0.post1.dev16
+Version: 1.1.0.post1.dev21
 Summary: An API for the homematicip cloud
 Author-email: Thomas Hahn <homematicip-rest-api@outlook.com>
 Project-URL: Homepage, https://github.com/hahn-th/homematicip-rest-api
 Project-URL: Repository, https://github.com/hahn-th/homematicip-rest-api.git
 Project-URL: Issues, https://github.com/hahn-th/homematicip-rest-api/issues
 Project-URL: Changelog, https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md
 Keywords: homematicip cloud,homematicip
```

### Comparing `homematicip-1.1.0.post1.dev16/README.md` & `homematicip-1.1.0.post1.dev21/README.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/Makefile` & `homematicip-1.1.0.post1.dev21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/make.bat` & `homematicip-1.1.0.post1.dev21/docs/make.bat`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/api_introduction.rst` & `homematicip-1.1.0.post1.dev21/docs/source/api_introduction.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/conf.py` & `homematicip-1.1.0.post1.dev21/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/gettingstarted.rst` & `homematicip-1.1.0.post1.dev21/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/homematicip.aio.rst` & `homematicip-1.1.0.post1.dev21/docs/source/homematicip.aio.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/homematicip.base.rst` & `homematicip-1.1.0.post1.dev21/docs/source/homematicip.base.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/homematicip.rst` & `homematicip-1.1.0.post1.dev21/docs/source/homematicip.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/docs/source/index.rst` & `homematicip-1.1.0.post1.dev21/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/pyproject.toml` & `homematicip-1.1.0.post1.dev21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 [tool.setuptools_scm]
 version_file = "src/homematicip/_version.py"
 version_scheme = "no-guess-dev"
 local_scheme = "no-local-version"
 
 
 [project.scripts]
-hmip = "homematicip.cli.hmip_cli:cli"
+hmip = "homematicip.cli.hmip:cli"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 #addopts = "--cov=src --cov-report term-missing"
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `homematicip-1.1.0.post1.dev16/sample_data/json_data/home.json` & `homematicip-1.1.0.post1.dev21/sample_data/json_data/home.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/sample_data/json_data/security_journal.json` & `homematicip-1.1.0.post1.dev21/sample_data/json_data/security_journal.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/sample_data/json_data/unknown_types.json` & `homematicip-1.1.0.post1.dev21/sample_data/json_data/unknown_types.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/action/action.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/action/action.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/action/action_registry.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/action/action_registry.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/auth.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/cli/helper.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/cli/helper.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/cli/hmip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
 import datetime
 import json
 import logging
 import os
+import sys
 import time
 from logging.handlers import TimedRotatingFileHandler
-
+from importlib.metadata import version as metadata_version
 import click
 import httpx
 from alive_progress import alive_bar
 from click import ClickException
 
 from homematicip.action.functional_channel_actions import action_set_slats_level, action_set_shutter_level, \
     action_set_switch_state, action_set_dim_level, action_start_impulse
 from homematicip.action.group_actions import action_set_boost, action_set_point_temperature, action_set_boost_duration, \
-    action_set_active_profile, action_set_control_mode
+    action_set_active_profile, action_set_control_mode, action_set_shutter_level_group, action_set_slats_level_group
 from homematicip.auth import Auth
 from homematicip.cli.helper import get_channel_by_index_of_first
 from homematicip.cli.helper import get_rssi_bar_string
 from homematicip.configuration.config import Config, PersistentConfig
 from homematicip.configuration.config_io import ConfigIO
 from homematicip.configuration.log_helper import get_logger_filename
 from homematicip.connection.rest_connection import ConnectionContext, RestResult
+from homematicip.events.event_types import ModelUpdateEvent
 from homematicip.model.anoymizer import handle_config
 from homematicip.model.enums import ClimateControlMode
 from homematicip.runner import Runner
 
 
 async def get_initialized_runner(including_model: bool = True) -> Runner:
     config = get_config()
@@ -65,14 +67,15 @@
     if should_roll_over:
         handler.doRollover()
 
     logging.basicConfig(level=log_level, handlers=[handler],
                         format='%(asctime)s %(name)-12s %(levelname)-8s %(message)s')
     logging.getLogger("httpx").setLevel(logging.CRITICAL)
     logging.getLogger("httpcore").setLevel(logging.CRITICAL)
+    logging.getLogger("websockets.client").setLevel(logging.CRITICAL)
 
 
 def setup_logger(
         log_level: int, log_file: str
 ) -> logging.Logger:
     """Initialize logger. If log_file is set, log to file, otherwise to stdout. The log level """
     setup_basic_logging(log_level, log_file)
@@ -157,15 +160,15 @@
                     break
                 last_request = datetime.datetime.now()
 
             bar()
 
     logger.debug("Getting auth token and client-id")
     auth_token = asyncio.run(auth.request_auth_token())
-    client_id = asyncio.run(auth.confirm_auth_token(auth_token))
+    asyncio.run(auth.confirm_auth_token(auth_token))
 
     logger.debug("Got auth-token and client-id. Persist config.")
 
     config = PersistentConfig(accesspoint_id=access_point_id, auth_token=auth_token)
     config_path = ConfigIO.to_file(config)
 
     click.echo("")
@@ -310,86 +313,116 @@
 
 @cli.group
 def run():
     """Run actions on devices, groups, home or functional channels."""
     pass
 
 
-@run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("channel_index", type=int, nargs=1)
-@click.argument("slats_level", type=float, nargs=1)
-@click.argument("shutter_level", type=float, nargs=1, required=False)
-def set_slats_level(id: str, channel_index: int, slats_level: float, shutter_level: float = None):
-    """Set the slats level for a device. specify FunctionalChannel-Index."""
+async def _model_update_event_handler(event: ModelUpdateEvent, args) -> None:
+    click.echo(f"ModelUpdateEvent: {event}; {args}")
+
+
+# @cli.command
+# def listen():
+#     """Listen to events. If filename is specified, events are written to the file. If not, they are written to
+#     console."""
+#     runner = asyncio.run(get_initialized_runner())
+#     runner.event_manager.subscribe(ModelUpdateEvent.ITEM_CREATED, _model_update_event_handler)
+#     runner.event_manager.subscribe(ModelUpdateEvent.ITEM_UPDATED, _model_update_event_handler)
+#     runner.event_manager.subscribe(ModelUpdateEvent.ITEM_REMOVED, _model_update_event_handler)
+#
+#     loop = asyncio.new_event_loop()
+#     task = loop.create_task(runner.async_listening_for_updates())
+#
+#     try:
+#         click.echo("Waiting for events... press CTRL+C to stop listening.")
+#         loop.run_until_complete(task)
+#     except asyncio.CancelledError:
+#         pass
+#     except KeyboardInterrupt:
+#         task.cancel()
+#         loop.stop()
+#         click.echo("Stopping listener...")
+
+
+@cli.command
+def version():
+    """Print the version of the homematicip-rest-api."""
+    click.echo(f"HomematicIP-Rest-Api: {metadata_version("homematicip")}")
+    click.echo(f"Python: {sys.version}")
+
+
+@run.command()
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
+def turn_on(id: str, channel: int = None):
+    """Turn a device on. Specify a FunctionalChannel-Index."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.devices:
         click.echo(f"Device with id {id} not found.", err=True, color=True)
         return
 
     device = runner.model.devices[id]
-    if str(channel_index) not in device.functionalChannels:
-        click.echo(f"Channel with index {channel_index} not found.", err=True, color=True)
-        return
+    fc = get_channel_by_index_of_first(device, channel)
 
-    result = asyncio.run(
-        action_set_slats_level(runner, device.functionalChannels[str(channel_index)], channel_index, slats_level,
-                               shutter_level))
+    result = asyncio.run(action_set_switch_state(runner, fc, True))
 
     click.echo(
-        f"Run set_slats_level for device {device.label or device.id} with result: {result.status_text} ({result.status})")
+        f"Run turn_on for device {device.label or device.id} with result: {result.status_text} ({result.status})")
 
 
-@run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("channel_index", type=int, nargs=1)
-@click.argument("shutter_level", type=float, nargs=1)
-def set_shutter_level(id: str, channel_index: int, shutter_level: float):
+@run.command()
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
+def turn_off(id: str, channel: int = None):
+    """Turn a device off. Specify a FunctionalChannel-Index.
+
+    ID is the ID of the device.\n
+    CHANNEL_INDEX is the index of the channel. If the device has only one channel (excl. BaseChannel 0) this can be omitted."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.devices:
         click.echo(f"Device with id {id} not found.", err=True, color=True)
         return
 
     device = runner.model.devices[id]
-    if str(channel_index) not in device.functionalChannels:
-        click.echo(f"Channel with index {channel_index} not found.", err=True, color=True)
-        return
+    fc = get_channel_by_index_of_first(device, channel)
 
-    result = asyncio.run(
-        action_set_shutter_level(runner, device.functionalChannels[str(channel_index)], shutter_level))
+    result = asyncio.run(action_set_switch_state(runner, fc, False))
 
     click.echo(
-        f"Run set_shutter_level for device {device.label or device.id} with result: {result.status_text} ({result.status})")
+        f"Run turn_off for device {device.label or device.id} with result: {result.status_text} ({result.status})")
 
 
 @run.command()
-@click.argument("id", type=str, nargs=1)
-@click.argument("channel_index", type=int, nargs=1)
-@click.argument("state", type=bool, nargs=1)
-def set_switch_state(id: str, channel_index: int, state: bool):
-    """Set the switch state for a device. specify FunctionalChannel-Index.
-
-    ID is the Id of the device. Use 'list devices' to get desired Id.
-    CHANNEL_INDEX is the index of the channel.
-    STATE is the target state."""
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
+@click.option("--state", type=bool, required=True, help="The target state. True or False")
+def set_switch_state(id: str, channel: int, state: bool):
+    """Set the switch state for a device. specify FunctionalChannel-Index."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.devices:
         click.echo(f"Device with id {id} not found.", err=True, color=True)
         return
 
     device = runner.model.devices[id]
-    if str(channel_index) not in device.functionalChannels:
-        click.echo(f"Channel with index {channel_index} not found.", err=True, color=True)
+    if str(channel) not in device.functionalChannels:
+        click.echo(f"Channel with index {channel} not found.", err=True, color=True)
         return
 
     result = asyncio.run(
-        action_set_switch_state(runner, device.functionalChannels[str(channel_index)], state))
+        action_set_switch_state(runner, device.functionalChannels[str(channel)], state))
 
     click.echo(
         f"Run set_switch_state for device {device.label or device.id} with result: {result.status_text} ({result.status})")
 
 
 @run.command()
 @click.argument("filename", type=click.File('w'))
@@ -409,56 +442,48 @@
     filename.close()
 
     click.echo(f"Successfully dumped config to file {filename.name}")
     return
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
 def set_boost(id: str):
-    """Set Boost on Group.
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id."""
+    """Set Boost on Group."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
     result = asyncio.run(action_set_boost(runner, runner.model.groups[id], True))
     click.echo(f"Run set_boost with result: {result.status_text}")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
 def set_boost_stop(id: str):
-    """Stop Boost on Group.
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id."""
+    """Stop Boost on Group."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
     result = asyncio.run(action_set_boost(runner, runner.model.groups[id], False))
     click.echo(
         f"Run set_boost for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("temperature", type=float, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-t", "--temperature", type=float, help="Target Temperature", required=True)
 def set_point_temperature(id: str, temperature: float):
-    """Set point temperature for a group.
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id.
-    TEMPERATURE is the target temperature.
-    """
+    """Set point temperature for a group."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
     result = asyncio.run(action_set_point_temperature(runner, runner.model.groups[id], temperature))
@@ -468,78 +493,72 @@
 
     click.echo(
         f"Run set_point_temperature for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("minutes", type=int, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-m", "--minutes", type=int, nargs=1, help="Duration of boost in Minutes", required=True)
 def set_boost_duration(id: str, minutes: int):
-    """Sets the boost duration for a group in minutes
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id.
-    MINUTES is the duration in minutes.
-    """
+    """Sets the boost duration for a group in minutes"""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
     result = asyncio.run(action_set_boost_duration(runner, runner.model.groups[id], minutes))
     click.echo(
         f"Run set_boost_duration for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("profile_index", type=str, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-p", "--profile_index", type=str, required=True,
+              help="index of the profile. Usually this is PROFILE_x. Use 'hmip list profiles <group-id>' to get a "
+                   "list of available profiles for a group.")
 def set_active_profile(id: str, profile_index: str):
-    """Set the active profile for a group.
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id.
-    PROFILE_INDEX is the index of the profile. Usally this is PROFILE_x. List Profiles to get an overview."""
+    """Set the active profile for a group."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
     result = asyncio.run(action_set_active_profile(runner, runner.model.groups[id], profile_index))
     click.echo(
         f"Run set_active_profile for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("control_mode", type=ClimateControlMode, nargs=1)
-def set_control_mode(id: str, control_mode: ClimateControlMode):
-    """Set the control mode for a group.
-
-    ID is the Id of a Group. Use 'list groups' to get desired Id.
-    CONTROL_MODE is the control mode."""
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("--mode", type=ClimateControlMode, help="the control mode. [ECO|AUTOMATIC|MANUAL]")
+def set_control_mode(id: str, mode: ClimateControlMode):
+    """Set the control mode for a group."""
     runner = asyncio.run(get_initialized_runner())
 
     if id not in runner.model.groups:
         click.echo(f"Group with id {id} not found.", err=True, color=True)
         return
 
-    result = asyncio.run(action_set_control_mode(runner, runner.model.groups[id], control_mode))
+    result = asyncio.run(action_set_control_mode(runner, runner.model.groups[id], mode))
     click.echo(
         f"Run set_control_mode for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
 
 @run.command
-@click.argument("id", type=str, nargs=1)
-@click.argument("dim_level", type=click.FloatRange(0.0, 1.0), nargs=1)
-@click.argument("channel", type=int, nargs=1)
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-d", "--dim_level", type=click.FloatRange(0.0, 1.0), help="Target Dim Level", required=True)
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
 def set_dim_level(id: str, dim_level: float, channel: int = None):
     """Set the dim level for a device.
 
     ID is the Id of the device. Use 'list devices' to get desired Id.\n
     DIM_LEVEL is the target dim level. Must be between 0.0 and 1.0.\n
     CHANNEL is the channel index of the device. If the device has only one channel (excl. BaseChannel 0) this can be omitted.
     """
@@ -558,14 +577,74 @@
         return
     result = asyncio.run(action_set_dim_level(runner, fc, dim_level))
     click.echo(
         f"Run set_dim_level for device {device.label or device.id} and channel {fc.index} with result: {result.status_text} ({result.status})")
 
 
 @run.command
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
+@click.option("-s", "--shutter_level", type=click.FloatRange(0.0, 1.0), required=True, help="Target shutter level.")
+def set_shutter_level(id: str, shutter_level: float, channel: int):
+    runner = asyncio.run(get_initialized_runner())
+
+    if id in runner.model.devices:
+        device = runner.model.devices[id]
+        fc = get_channel_by_index_of_first(device, channel)
+        result = asyncio.run(action_set_shutter_level(runner, fc, shutter_level))
+        click.echo(
+            f"Run set_shutter_level for device {device.label or device.id} with result: {result.status_text} ({result.status})")
+        return
+
+    if id in runner.model.groups:
+        group = runner.model.groups[id]
+        result = asyncio.run(action_set_shutter_level_group(runner, group, shutter_level))
+        click.echo(
+            f"Run set_shutter_level for group {group.label or group.id} with result: {result.status_text} ({result.status})")
+        return
+
+    click.echo(f"Id is neither a device nor a group.", err=True, color=True)
+
+
+@run.command
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
+@click.option("-sl", "--slats-level", type=click.FloatRange(0.0, 1.0), nargs=1, required=True, help="Slats Level.")
+@click.option("-sh", "--shutter-level", type=click.FloatRange(0.0, 1.0), nargs=1, required=False, default=None,
+              help="Shutter Level.")
+def set_slats_level(id: str, slats_level: float, shutter_level: float = None, channel: int = None):
+    runner = asyncio.run(get_initialized_runner())
+
+    if id in runner.model.devices:
+        device = runner.model.devices[id]
+        fc = get_channel_by_index_of_first(device, channel)
+        result = asyncio.run(action_set_slats_level(runner, fc, slats_level, shutter_level))
+        click.echo(
+            f"Run set_slats_level for device {device.label or device.id} with result: {result.status_text} ({result.status})")
+        return
+
+    if id in runner.model.groups:
+        group = runner.model.groups[id]
+        result = asyncio.run(action_set_slats_level_group(runner, group, slats_level, shutter_level))
+        click.echo(
+            f"Run set_slats_level for group {group.label or group.id} with result: {result.status_text} ({result.status})")
+        return
+
+    click.echo(f"Specified Id '{id}' is neither a device nor a group.", err=True, color=True)
+
+
+@run.command
+@click.option("--id", type=str, required=True, help="ID of the device or group, which the run command is applied to.")
+@click.option("-c", "--channel", type=int, required=False, default=None,
+              help="Index of the Channel. Only necessary, if you have more than one channel on the device. Not "
+                   "needed, if you want to control a group.")
 def toggle_garage_door(id: str, channel: int = None):
     """Toggle the garage door.
 
     ID is the Id of the device. Use 'list devices' to get desired Id."""
     runner = asyncio.run(get_initialized_runner())
     model = runner.model
 
@@ -672,23 +751,15 @@
 #     #                     "set_lock_state",
 #     #                     targetLockState,
 #     #                     pin,
 #     #                 )
 #     #             command_entered = True
 #     #
 #     #
-#     #         if args.device_shutter_level is not None:
-#     #             _execute_action_for_device(
-#     #                 device,
-#     #                 args,
-#     #                 CliActions.SET_SHUTTER_LEVEL,
-#     #                 "set_shutter_level",
-#     #                 args.device_shutter_level,
-#     #             )
-#     #             command_entered = True
+#     #
 #     #
 #     #         if args.device_slats_level is not None:
 #     #             slats_level = args.device_slats_level[0]
 #     #             shutter_level = (
 #     #                 args.device_slats_level[1]
 #     #                 if len(args.device_slats_level) > 1
 #     #                 else None
@@ -854,22 +925,15 @@
 #     #         command_entered = True
 #     #         group.set_shutter_level(args.group_shutter_level)
 #     #
 #     #     if args.group_shutter_stop:
 #     #         command_entered = True
 #     #         group.set_shutter_stop()
 #     #
-#     #     if args.group_slats_level:
-#     #         slats_level = args.group_slats_level[0]
-#     #         shutter_level = (
-#     #             args.group_slats_level[1] if len(args.group_slats_level) > 1 else None
-#     #         )
-#     #
-#     #         command_entered = True
-#     #         group.set_slats_level(slats_level, shutter_level)
+
 #     #
 #     #     if args.group_set_point_temperature:
 #     #         command_entered = True
 #     #         if isinstance(group, HeatingGroup):
 #     #             group.set_point_temperature(args.group_set_point_temperature)
 #     #         else:
 #     #             logger.error("Group %s isn't a HEATING group", g.id)
@@ -945,25 +1009,14 @@
 #     #             time.sleep(1)
 #     #     except KeyboardInterrupt:
 #     #         return
 #
 #     return command_entered
 #
 #
-# def register_events(event_manager: EventManager):
-#     """Register events for the event manager."""
-#     event_manager.subscribe(ModelUpdateEvent.ITEM_CREATED, print_event)
-#     event_manager.subscribe(ModelUpdateEvent.ITEM_UPDATED, print_event)
-#     event_manager.subscribe(ModelUpdateEvent.ITEM_REMOVED, print_event)
-#
-#
-# def print_event(event):
-#     """Print the event."""
-#     pprint(event)
-#
 #
 # #
 # # def _get_target_channel_indices(device: BaseDevice, channels: list = None) -> list:
 # #     """Get list with adressed channel indices. Is the channels list None, than the channel 1 is used."""
 # #     target_channels_indices = []
 # #     if channels:
 # #         target_channels_indices = [*channels]
@@ -1034,21 +1087,7 @@
 # #     """Check, if a channel could execute the given function"""
 # #     return (
 # #         channel.functionalChannelType in FUNCTIONALCHANNEL_CLI_MAP
 # #         and action in FUNCTIONALCHANNEL_CLI_MAP[channel.functionalChannelType]
 # #     )
 # #
 # #
-# # def printEvents(eventList):
-# #     for event in eventList:
-# #         print("EventType: {} Data: {}".format(event["eventType"], event["data"]))
-# #
-#
-#
-#
-# def fake_download_configuration():
-#     """Use a json file as configuration source for the server."""
-#     global server_config
-#     if server_config:
-#         with open(server_config) as file:
-#             return json.load(file)
-#     return None
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/configuration/config.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config_io.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/configuration/config_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Get the well known locations for the configuration file."""
         config_filename = "config.json"
         search_locations = [os.path.join("./", config_filename)]
 
         os_name = platform.system()
 
         if os_name == "Windows":
-            appdata = os.getenv("appdata")
+            appdata = os.getenv("localappdata")
             programdata = os.getenv("programdata")
             search_locations.append(
                 os.path.join(appdata, "homematicip-rest-api", config_filename)
             )
             search_locations.append(
                 os.path.join(programdata, "homematicip-rest-api", config_filename)
             )
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/log_helper.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/configuration/log_helper.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_characteristics_builder.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/connection/client_characteristics_builder.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/connection/rest_connection.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/connection/rest_connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/events/event_manager.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/events/event_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,11 @@
             self._subscriptions[event_type].append(callback)
 
     def unsubscribe(self, event_type, callback):
         if event_type in self._subscriptions:
             if callback in self._subscriptions[event_type]:
                 self._subscriptions[event_type].remove(callback)
 
-    def publish(self, event_type, event_args):
+    async def publish(self, event_type: ModelUpdateEvent, event_args):
         if event_type in self._subscriptions:
             for callback in self._subscriptions[event_type]:
-                callback(event_args)
+                await callback(event_type, event_args)
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/events/hmip_event_handler.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/events/hmip_event_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,79 +14,79 @@
 class HmipEventHandler:
     """Take an incoming event from homematicip-cloud websocket and update model."""
 
     def __init__(self, event_manager: EventManager, model: Model):
         self._model = model
         self._event_manager = event_manager
 
-    def process_event(self, event_json):
+    async def process_event_async(self, event_json):
         for event in event_json["events"].values():
 
             LOGGER.info(f"Processing event {event['pushEventType']}")
 
             event_type = EventType[event['pushEventType']]
             if event_type == EventType.CLIENT_ADDED:
                 data = event['client']
                 client_id = data['id']
                 client = Client.model_validate_json(data, strict=False)
                 self._model.clients[client_id] = client
-                self._event_manager.publish(ModelUpdateEvent.ITEM_CREATED, client)
+                await self._event_manager.publish(ModelUpdateEvent.ITEM_CREATED, client)
 
             elif event_type == EventType.CLIENT_CHANGED:
                 data = event['client']
                 if data['id'] in self._model.clients:
                     client: BaseModel = self._model.clients[data['id']]
                     self._model.clients[data['id']] = client.model_copy(update={**data})
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, client)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, client)
 
             elif event_type == EventType.CLIENT_REMOVED:
                 data = event['client']
 
                 client = self._model.clients.pop(data['id'], None)
                 if client is not None:
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, client)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, client)
 
             elif event_type == EventType.DEVICE_ADDED:
                 data = event['device']
                 if data['id'] not in self._model.devices:
                     device = Device.model_validate_json(data, strict=False)
                     self._model.devices[data['id']] = device
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_CREATED, device)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_CREATED, device)
 
             elif event_type == EventType.DEVICE_CHANGED:
                 data = event['device']
                 if data['id'] in self._model.devices:
                     device: BaseModel = self._model.devices[data['id']]
                     self._model.devices[data['id']] = device.model_copy(update={**data})
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, device)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, device)
 
             elif event_type == EventType.DEVICE_REMOVED:
                 data = event['device']
 
                 device = self._model.devices.pop(data['id'], None)
                 if device is not None:
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, device)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, device)
 
             elif event_type == EventType.GROUP_ADDED:
                 pass
             elif event_type == EventType.GROUP_CHANGED:
                 pass
             elif event_type == EventType.GROUP_REMOVED:
                 data = event['group']
 
                 group = self._model.groups.pop(data['id'], None)
                 if group is not None:
-                    self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, group)
+                    await self._event_manager.publish(ModelUpdateEvent.ITEM_REMOVED, group)
 
             elif event_type == EventType.HOME_CHANGED:
                 data = event['home']
 
                 home = self._model.home.model_copy(update={**data})
                 self._model.home = home
-                self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, home)
+                await self._event_manager.publish(ModelUpdateEvent.ITEM_UPDATED, home)
 
             elif event_type == EventType.SECURITY_JOURNAL_CHANGED:
                 pass
 
     def _get_device_from_model(self, model: Model, id: str):
         if id in model.clients:
             return model.clients[id]
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/model/anoymizer.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/model/anoymizer.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/model/devices.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/model/devices.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/model/enums.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/model/enums.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/model/functional_channels.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/model/functional_channels.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/model/home.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/model/home.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip/runner.py` & `homematicip-1.1.0.post1.dev21/src/homematicip/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return result.json
 
     async def _async_start_listening_for_updates(self, context: ConnectionContext):
         handler = WebSocketHandler()
         hmip_event_handler = HmipEventHandler(event_manager=self.event_manager, model=self.model)
         async for message in handler.listen(context, False):
             try:
-                hmip_event_handler.process_event(json.loads(message))
+                await hmip_event_handler.process_event_async(json.loads(message))
 
             except Exception as e:
                 LOGGER.error(f"Error while handling incoming event. Message: {message}", exc_info=e)
 
     @property
     def rest_connection(self):
         return self._rest_connection
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/PKG-INFO` & `homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.1.0.post1.dev16
+Version: 1.1.0.post1.dev21
 Summary: An API for the homematicip cloud
 Author-email: Thomas Hahn <homematicip-rest-api@outlook.com>
 Project-URL: Homepage, https://github.com/hahn-th/homematicip-rest-api
 Project-URL: Repository, https://github.com/hahn-th/homematicip-rest-api.git
 Project-URL: Issues, https://github.com/hahn-th/homematicip-rest-api/issues
 Project-URL: Changelog, https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md
 Keywords: homematicip cloud,homematicip
```

### Comparing `homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/SOURCES.txt` & `homematicip-1.1.0.post1.dev21/src/homematicip.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 src/homematicip/action/__init__.py
 src/homematicip/action/action.py
 src/homematicip/action/action_registry.py
 src/homematicip/action/functional_channel_actions.py
 src/homematicip/action/group_actions.py
 src/homematicip/cli/__init__.py
 src/homematicip/cli/helper.py
-src/homematicip/cli/hmip_cli.py
+src/homematicip/cli/hmip.py
 src/homematicip/cli/hmip_cli_debug_wrapper.py
 src/homematicip/configuration/__init__.py
 src/homematicip/configuration/config.py
 src/homematicip/configuration/config_io.py
 src/homematicip/configuration/log_helper.py
 src/homematicip/connection/__init__.py
 src/homematicip/connection/client_characteristics_builder.py
@@ -77,13 +77,14 @@
 tests/conftest.py
 tests/test_auth.py
 tests/test_runner.py
 tests/actions/conftest.py
 tests/actions/test_action_decorator.py
 tests/actions/test_functional_channel_actions.py
 tests/actions/test_group_actions.py
+tests/cli/test_hmip.py
 tests/connection/test_client_characteristics_builder.py
 tests/connection/test_rest_connection.py
 tests/events/test_hmip_event_handler.py
 tests/model/conftest.py
 tests/model/test_functional_channel.py
 tests/model/test_model.py
```

### Comparing `homematicip-1.1.0.post1.dev16/tests/actions/test_action_decorator.py` & `homematicip-1.1.0.post1.dev21/tests/actions/test_action_decorator.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/actions/test_functional_channel_actions.py` & `homematicip-1.1.0.post1.dev21/tests/actions/test_functional_channel_actions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import pytest
 
 from homematicip.action.functional_channel_actions import action_start_impulse, action_set_switch_state, \
     action_set_slats_level, action_set_shutter_level, action_set_dim_level, set_acceleration_sensor_mode_action, \
     set_acceleration_sensor_neutral_position, set_acceleration_sensor_sensitivity, \
     set_acceleration_sensor_trigger_angle, set_acceleration_sensor_event_filter_period, set_notification_sound_type, \
-    set_minimum_floor_heating_valve_position, set_operation_lock
+    set_minimum_floor_heating_valve_position, set_operation_lock, action_send_door_command, action_set_door_state, \
+    action_set_rgb_dim_level, action_set_rgb_dim_level_with_time, action_set_primary_shading_level, \
+    action_set_secondary_shading_level, action_reset_energy_counter, action_set_display, \
+    action_set_acoustic_alarm_signal, action_set_acoustic_alarm_timing, action_set_acoustic_water_alarm_trigger, \
+    action_set_inapp_water_alarm_trigger, action_set_siren_water_alarm_trigger
 from homematicip.connection.rest_connection import RestResult, RestConnection
 from homematicip.model.enums import AccelerationSensorMode, AccelerationSensorNeutralPosition, \
-    AccelerationSensorSensitivity, NotificationSoundType
+    AccelerationSensorSensitivity, NotificationSoundType, DoorCommand, LockState, RGBColorState, ClimateControlDisplay, \
+    AcousticAlarmSignal, AcousticAlarmTiming, WaterAlarmTrigger
 from homematicip.model.functional_channels import FunctionalChannel
 from homematicip.runner import Runner
 
 
 @pytest.fixture
 def runner(mocker, filled_model):
     conn = mocker.Mock(spec=RestConnection)
@@ -176,7 +181,164 @@
     sample_functional_channel.functionalChannelType = "DEVICE_OPERATIONLOCK"
     result = await set_operation_lock(runner, sample_functional_channel, True)
     assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setOperationLock"
     assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
     assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
     assert runner.rest_connection.async_post.call_args[0][1]["operationLock"] is True
     assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_send_door_command(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "DOOR_CHANNEL"
+    result = await action_send_door_command(runner, sample_functional_channel, DoorCommand.OPEN)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/sendDoorCommand"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["doorCommand"] == str(DoorCommand.OPEN)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_door_state(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "DOOR_LOCK_CHANNEL"
+    result = await action_set_door_state(runner, sample_functional_channel, LockState.OPEN, "1234")
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/setLockState"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["authorizationPin"] == "1234"
+    assert runner.rest_connection.async_post.call_args[0][1]["targetLockState"] == str(LockState.OPEN)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_rgb_dim_level(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "NOTIFICATION_LIGHT_CHANNEL"
+    result = await action_set_rgb_dim_level(runner, sample_functional_channel, RGBColorState.BLUE, 0.5)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/setSimpleRGBColorDimLevel"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["dimLevel"] == 0.5
+    assert runner.rest_connection.async_post.call_args[0][1]["simpleRGBColorState"] == str(RGBColorState.BLUE)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_rgb_dim_level_with_time(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "NOTIFICATION_LIGHT_CHANNEL"
+    result = await action_set_rgb_dim_level_with_time(runner, sample_functional_channel, RGBColorState.BLUE, 0.5, 10.5,
+                                                      20.5)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/setSimpleRGBColorDimLevelWithTime"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["dimLevel"] == 0.5
+    assert runner.rest_connection.async_post.call_args[0][1]["onTime"] == 10.5
+    assert runner.rest_connection.async_post.call_args[0][1]["rampTime"] == 20.5
+    assert runner.rest_connection.async_post.call_args[0][1]["simpleRGBColorState"] == str(RGBColorState.BLUE)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_primary_shading_level(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "SHADING_CHANNEL"
+    result = await action_set_primary_shading_level(runner, sample_functional_channel, 0.5)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/setPrimaryShadingLevel"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["primaryShadingLevel"] == 0.5
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_secondary_shading_level(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "SHADING_CHANNEL"
+    result = await action_set_secondary_shading_level(runner, sample_functional_channel, 0.5, 0.8)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/setSecondaryShadingLevel"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["primaryShadingLevel"] == 0.5
+    assert runner.rest_connection.async_post.call_args[0][1]["secondaryShadingLevel"] == 0.8
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_reset_energy_counter(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "SWITCH_MEASURING_CHANNEL"
+    result = await action_reset_energy_counter(runner, sample_functional_channel)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/control/resetEnergyCounter"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_display(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WALL_MOUNTED_THERMOSTAT_PRO_CHANNEL"
+    result = await action_set_display(runner, sample_functional_channel, ClimateControlDisplay.ACTUAL)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setClimateControlDisplay"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["display"] == str(ClimateControlDisplay.ACTUAL)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_acoustic_alarm_signal(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WATER_SENSOR_CHANNEL"
+    result = await action_set_acoustic_alarm_signal(runner, sample_functional_channel,
+                                                    AcousticAlarmSignal.DISABLE_ACOUSTIC_SIGNAL)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setAcousticAlarmSignal"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["acousticAlarmSignal"] == str(
+        AcousticAlarmSignal.DISABLE_ACOUSTIC_SIGNAL)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_acoustic_alarm_timing(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WATER_SENSOR_CHANNEL"
+    result = await action_set_acoustic_alarm_timing(runner, sample_functional_channel,
+                                                    AcousticAlarmTiming.PERMANENT)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setAcousticAlarmTiming"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["acousticAlarmTiming"] == str(
+        AcousticAlarmTiming.PERMANENT)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_set_acoustic_water_alarm_trigger(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WATER_SENSOR_CHANNEL"
+    result = await action_set_acoustic_water_alarm_trigger(runner, sample_functional_channel,
+                                                           WaterAlarmTrigger.WATER_DETECTION)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setAcousticWaterAlarmTrigger"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["acousticWaterAlarmTrigger"] == str(
+        WaterAlarmTrigger.WATER_DETECTION)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_action_set_inapp_water_alarm_trigger(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WATER_SENSOR_CHANNEL"
+    result = await action_set_inapp_water_alarm_trigger(runner, sample_functional_channel,
+                                                        WaterAlarmTrigger.WATER_DETECTION)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setInAppWaterAlarmTrigger"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["inAppWaterAlarmTrigger"] == str(
+        WaterAlarmTrigger.WATER_DETECTION)
+    assert result.status == 200
+
+
+@pytest.mark.asyncio
+async def test_action_set_siren_water_alarm_trigger(runner, sample_functional_channel):
+    sample_functional_channel.functionalChannelType = "WATER_SENSOR_CHANNEL"
+    result = await action_set_siren_water_alarm_trigger(runner, sample_functional_channel, WaterAlarmTrigger.WATER_DETECTION)
+    assert runner.rest_connection.async_post.call_args[0][0] == "device/configuration/setSirenWaterAlarmTrigger"
+    assert runner.rest_connection.async_post.call_args[0][1]["deviceId"] == "00000000-0000-0000-0000-000000000001"
+    assert runner.rest_connection.async_post.call_args[0][1]["channelIndex"] == 1
+    assert runner.rest_connection.async_post.call_args[0][1]["sirenWaterAlarmTrigger"] == str(WaterAlarmTrigger.WATER_DETECTION)
+    assert result.status == 200
```

### Comparing `homematicip-1.1.0.post1.dev16/tests/actions/test_group_actions.py` & `homematicip-1.1.0.post1.dev21/tests/actions/test_group_actions.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/conftest.py` & `homematicip-1.1.0.post1.dev21/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/connection/test_rest_connection.py` & `homematicip-1.1.0.post1.dev21/tests/connection/test_rest_connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/events/test_hmip_event_handler.py` & `homematicip-1.1.0.post1.dev21/tests/events/test_hmip_event_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import json
+
+import pytest
+
 from homematicip.model import build_model_from_json
 from homematicip.events.event_manager import EventManager
 from homematicip.events.hmip_event_handler import HmipEventHandler
 
 
 def test_device_removed(sample_data_complete):
     assert True
 
 
 def test_device_added(sample_data_complete):
     assert True
 
 
-def test_device_updated(sample_data_complete):
+@pytest.mark.asyncio
+async def test_device_updated(sample_data_complete):
     event_manager = EventManager()
     model = build_model_from_json(sample_data_complete)
     device_id = "3014F7110000RAIN_SENSOR"
     device_before = model.devices[device_id]
     change_event_b = b'{"events":{"0":{"pushEventType":"DEVICE_CHANGED","device":{"availableFirmwareVersion":"1.0.18","connectionType":"HMIP_RF","firmwareVersion":"1.0.18","firmwareVersionInteger":65554,"functionalChannels":{"0":{"busConfigMismatch":null,"coProFaulty":false,"coProRestartNeeded":false,"coProUpdateFailure":false,"configPending":false,"deviceId":"3014F7110000RAIN_SENSOR","deviceOverheated":false,"deviceOverloaded":false,"devicePowerFailureDetected":false,"deviceUndervoltage":false,"dutyCycle":false,"functionalChannelType":"DEVICE_BASE","groupIndex":0,"groups":["00000000-0000-0000-0000-000000000042"],"index":0,"label":"","lowBat":null,"multicastRoutingEnabled":false,"powerShortCircuit":null,"routerModuleEnabled":false,"routerModuleSupported":false,"rssiDeviceValue":-91,"rssiPeerValue":null,"shortCircuitDataLine":null,"supportedOptionalFeatures":{"IFeatureBusConfigMismatch":false,"IFeatureDeviceCoProError":false,"IFeatureDeviceCoProRestart":false,"IFeatureDeviceCoProUpdate":false,"IFeatureDeviceIdentify":false,"IFeatureDeviceOverheated":false,"IFeatureDeviceOverloaded":false,"IFeatureDevicePowerFailure":false,"IFeatureDeviceTemperatureOutOfRange":false,"IFeatureDeviceUndervoltage":false,"IFeatureMulticastRouter":false,"IFeaturePowerShortCircuit":false,"IFeatureRssiValue":true,"IFeatureShortCircuitDataLine":false,"IOptionalFeatureDutyCycle":true,"IOptionalFeatureLowBat":false},"temperatureOutOfRange":false,"unreach":false},"1":{"deviceId":"3014F7110000RAIN_SENSOR","functionalChannelType":"RAIN_DETECTION_CHANNEL","groupIndex":1,"groups":["00000000-0000-0000-0000-000000000043"],"index":1,"label":"","rainSensorSensitivity":80.0,"raining":true}},"homeId":"00000000-0000-0000-0000-000000000001","id":"3014F7110000RAIN_SENSOR","label":"Regensensor","lastStatusUpdate":1610893558747,"liveUpdateState":"LIVE_UPDATE_NOT_SUPPORTED","manufacturerCode":1,"modelId":412,"modelType":"HmIP-SRD","oem":"eQ-3","permanentlyReachable":true,"serializedGlobalTradeItemNumber":"3014F7110000RAIN_SENSOR","type":"RAIN_SENSOR","updateState":"UP_TO_DATE"}}}}'
     change_event = json.loads(change_event_b)
 
     hmip_event_handler = HmipEventHandler(event_manager=event_manager, model=model)
-    hmip_event_handler.process_event(change_event)
+    await hmip_event_handler.process_event_async(change_event)
 
     assert model.devices[device_id].lastStatusUpdate != device_before.lastStatusUpdate
 
 
 def test_client_removed(sample_data_complete):
     assert True
```

### Comparing `homematicip-1.1.0.post1.dev16/tests/model/test_model.py` & `homematicip-1.1.0.post1.dev21/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/test_auth.py` & `homematicip-1.1.0.post1.dev21/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev16/tests/test_runner.py` & `homematicip-1.1.0.post1.dev21/tests/test_runner.py`

 * *Files identical despite different names*

