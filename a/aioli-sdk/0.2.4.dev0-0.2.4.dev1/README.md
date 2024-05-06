# Comparing `tmp/aioli_sdk-0.2.4.dev0.tar.gz` & `tmp/aioli_sdk-0.2.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4.dev0.tar", last modified: Tue Apr 30 21:11:09 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4.dev1.tar", last modified: Mon May  6 16:26:18 2024, max compression
```

## Comparing `aioli_sdk-0.2.4.dev0.tar` & `aioli_sdk-0.2.4.dev1.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.601179 aioli_sdk-0.2.4.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-04-30 21:11:09.601179 aioli_sdk-0.2.4.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14908 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28285 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.601179 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2447 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-30 21:11:07.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-30 21:11:09.000000 aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.597179 aioli_sdk-0.2.4.dev0/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.601179 aioli_sdk-0.2.4.dev0/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54371 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:09.601179 aioli_sdk-0.2.4.dev0/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4884 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6065 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5499 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-04-30 21:11:05.000000 aioli_sdk-0.2.4.dev0/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-30 21:11:09.605179 aioli_sdk-0.2.4.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-04-30 21:04:57.000000 aioli_sdk-0.2.4.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.948191 aioli_sdk-0.2.4.dev1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-06 16:26:18.948191 aioli_sdk-0.2.4.dev1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.940191 aioli_sdk-0.2.4.dev1/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.940191 aioli_sdk-0.2.4.dev1/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.940191 aioli_sdk-0.2.4.dev1/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29032 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.940191 aioli_sdk-0.2.4.dev1/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.940191 aioli_sdk-0.2.4.dev1/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.948191 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 16:26:15.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-06 16:26:18.000000 aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.944191 aioli_sdk-0.2.4.dev1/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.944191 aioli_sdk-0.2.4.dev1/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64597 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:18.948191 aioli_sdk-0.2.4.dev1/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4884 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6065 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5499 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-06 16:26:13.000000 aioli_sdk-0.2.4.dev1/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-06 16:26:18.948191 aioli_sdk-0.2.4.dev1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-06 16:19:06.000000 aioli_sdk-0.2.4.dev1/setup.py
```

### Comparing `aioli_sdk-0.2.4.dev0/PKG-INFO` & `aioli_sdk-0.2.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev0
+Version: 0.2.4.dev1
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/_util.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/cli.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/deployment.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/errors.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/model.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # © Copyright 2023-2024 Hewlett Packard Enterprise Development LP
+import re
 from argparse import Namespace
 from typing import Any, List
 
 from pydantic import StrictInt
 
 import aiolirest
 from aioli import cli
@@ -113,39 +114,37 @@
         if r.name == name:
             model = r
             model_count += 1
 
     if model_count == 1:
         return model  # Found a single version of the specified model
     if model_count > 1 and not args.version:
-        raise_version_required(name)
+        raise_version_required(name, model_count)
 
     if model_count == 0:
         # The specified model does not exist; extract the version suffix if any
-        split_on = ".v"
-        split = name.lower().rsplit(split_on, 1)
-
-        if len(split) != 1:
-            version = split[1]  # without the ".v"
-            # Extract name as everything to the left of the last ".v"
-            name = name[0 : len(name) - len(version) - len(split_on)]
+        regexp = re.compile(r"^(.+)\.[Vv](\d+)$")
+        m = regexp.match(name)
+        if m is None:
+            raise NotFoundException(
+                f"model {name} not found. Model versions may optionally be specified "
+                "using the suffix '.v#', for example, '.v1', '.v100'"
+            )
+        name = m.group(1)
+        version = m.group(2)
 
     # if there is an explicit version specified, then use that
     if args.version:
         version = args.version
-    if version is None:
-        raise_version_required(name)
 
     return lookup_model_and_version(name, version, models)
 
 
-def raise_version_required(name: str) -> None:
-    raise VersionRequiredException(
-        f"please specify model version as {name} matches more than one model"
-    )
+def raise_version_required(name: str, count: int) -> None:
+    raise VersionRequiredException(f"specify a version as model {name} exists in {count} versions")
 
 
 def lookup_model_and_version(name: str, version: str, models: List[PackagedModel]) -> PackagedModel:
     # The version may optionally be expressed with a prefix of 'v'
     version_no_prefix: str = version.lstrip("vV")
     for r in models:
         if r.name == name and r.version == StrictInt(version_no_prefix):
```

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/registry.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/render.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/role.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/sso.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,14 +353,28 @@
             "                                      | bento-registry1"
         )
         actual = subprocess.check_output(["aioli", "model", "list"]).decode("utf-8")
 
         assert (actual.find(expected)) > 0
         assert os.system("aioli model delete openllm 1") == 0
 
+    def test_model_update_bad_model_name(self, setup_login: None) -> None:
+        # Attempt to update model specifying the version incorrectly. Here we specify
+        # a suffix of ".1", and not ".v1" which would specify the name & version.
+        # assert (os.system("aioli model update iris-tf-keras.1") == 0)
+        try:
+            subprocess.check_output(
+                ["aioli", "model", "update", "iris-tf-keras.1"], stderr=subprocess.STDOUT
+            )
+        except subprocess.CalledProcessError as e:
+            assert e.returncode == 1
+            expected = "Failed to modify a packaged model: model iris-tf-keras.1 not found"
+            actual: str = e.output.decode("utf-8")
+            assert actual.find(expected) == 0
+
     def test_model_update(self, setup_login: None) -> None:
         # Update existing model entry and test for expected values
         assert (
             os.system(
                 "aioli model update iris-tf-keras --name iris-tf-keras1 "
                 "--registry bento-registry1 "
                 "--url s3://demo-bento-registry/iris-tf-keras_updated "
```

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/user.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/cli/version.py` & `aioli_sdk-0.2.4.dev1/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4.dev1/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/api/certs.py` & `aioli_sdk-0.2.4.dev1/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/api/errors.py` & `aioli_sdk-0.2.4.dev1/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/api/request.py` & `aioli_sdk-0.2.4.dev1/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/check.py` & `aioli_sdk-0.2.4.dev1/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/constants.py` & `aioli_sdk-0.2.4.dev1/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4.dev1/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/requests.py` & `aioli_sdk-0.2.4.dev1/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/common/util.py` & `aioli_sdk-0.2.4.dev1/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli/util.py` & `aioli_sdk-0.2.4.dev1/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev0
+Version: 0.2.4.dev1
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev0/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4.dev1/aioli_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 aiolirest/models/deployment_state.py
 aiolirest/models/error_response.py
 aiolirest/models/event_info.py
 aiolirest/models/failure_info.py
 aiolirest/models/login_request.py
 aiolirest/models/login_response.py
 aiolirest/models/model_auth_token.py
+aiolirest/models/model_response.py
 aiolirest/models/observability.py
 aiolirest/models/packaged_model.py
 aiolirest/models/packaged_model_request.py
 aiolirest/models/resource_profile.py
 aiolirest/models/resources_template.py
 aiolirest/models/role.py
 aiolirest/models/role_assignment.py
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/__init__.py` & `aioli_sdk-0.2.4.dev1/aiolirest/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -48,14 +48,15 @@
 from aiolirest.models.deployment_state import DeploymentState
 from aiolirest.models.error_response import ErrorResponse
 from aiolirest.models.event_info import EventInfo
 from aiolirest.models.failure_info import FailureInfo
 from aiolirest.models.login_request import LoginRequest
 from aiolirest.models.login_response import LoginResponse
 from aiolirest.models.model_auth_token import ModelAuthToken
+from aiolirest.models.model_response import ModelResponse
 from aiolirest.models.observability import Observability
 from aiolirest.models.packaged_model import PackagedModel
 from aiolirest.models.packaged_model_request import PackagedModelRequest
 from aiolirest.models.resource_profile import ResourceProfile
 from aiolirest.models.resources_template import ResourcesTemplate
 from aiolirest.models.role import Role
 from aiolirest.models.role_assignment import RoleAssignment
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/registries_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,14 +26,15 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
 from typing import List
 
+from aiolirest.models.model_response import ModelResponse
 from aiolirest.models.success_response import SuccessResponse
 from aiolirest.models.trained_model_registry import TrainedModelRegistry
 from aiolirest.models.trained_model_registry_request import TrainedModelRegistryRequest
 
 from aiolirest.api_client import ApiClient
 from aiolirest.api_response import ApiResponse
 from aiolirest.rest import RESTResponseType
@@ -826,14 +827,282 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def registries_id_models_get(
+        self,
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[ModelResponse]:
+        """Get all available models from a registry
+
+        Returns an array of all available models from a registry
+
+        :param id: Model Registry ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._registries_id_models_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[ModelResponse]",
+            '404': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def registries_id_models_get_with_http_info(
+        self,
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[ModelResponse]]:
+        """Get all available models from a registry
+
+        Returns an array of all available models from a registry
+
+        :param id: Model Registry ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._registries_id_models_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[ModelResponse]",
+            '404': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def registries_id_models_get_without_preload_content(
+        self,
+        id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Get all available models from a registry
+
+        Returns an array of all available models from a registry
+
+        :param id: Model Registry ID (required)
+        :type id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._registries_id_models_get_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[ModelResponse]",
+            '404': "ErrorResponse",
+            '500': "ErrorResponse"
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _registries_id_models_get_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/registries/{id}/models',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api_client.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/api_response.py` & `aioli_sdk-0.2.4.dev1/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/configuration.py` & `aioli_sdk-0.2.4.dev1/aiolirest/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-dev0\n"\
+               "Version of the API: 0.2.4-dev1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/exceptions.py` & `aioli_sdk-0.2.4.dev1/aiolirest/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,14 +24,15 @@
 from aiolirest.models.deployment_state import DeploymentState
 from aiolirest.models.error_response import ErrorResponse
 from aiolirest.models.event_info import EventInfo
 from aiolirest.models.failure_info import FailureInfo
 from aiolirest.models.login_request import LoginRequest
 from aiolirest.models.login_response import LoginResponse
 from aiolirest.models.model_auth_token import ModelAuthToken
+from aiolirest.models.model_response import ModelResponse
 from aiolirest.models.observability import Observability
 from aiolirest.models.packaged_model import PackagedModel
 from aiolirest.models.packaged_model_request import PackagedModelRequest
 from aiolirest.models.resource_profile import ResourceProfile
 from aiolirest.models.resources_template import ResourcesTemplate
 from aiolirest.models.role import Role
 from aiolirest.models.role_assignment import RoleAssignment
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/autoscaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/configuration_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/deployment_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/event_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/failure_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/login_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/model_auth_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/observability.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/observability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/packaged_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/packaged_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/resource_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/resources_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/role.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/security.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/success_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/trained_model_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/trained_model_registry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/user.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/user_patch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4.dev1/aiolirest/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/aiolirest/rest.py` & `aioli_sdk-0.2.4.dev1/aiolirest/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev0
+    The version of the OpenAPI document: 0.2.4-dev1
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev0/setup.py` & `aioli_sdk-0.2.4.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-dev0",
+    version="0.2.4-dev1",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

