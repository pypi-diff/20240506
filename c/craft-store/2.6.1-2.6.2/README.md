# Comparing `tmp/craft-store-2.6.1.tar.gz` & `tmp/craft-store-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-store-2.6.1.tar", last modified: Tue Mar 26 17:26:04 2024, max compression
+gzip compressed data, was "craft-store-2.6.2.tar", last modified: Mon May  6 19:16:47 2024, max compression
```

## Comparing `craft-store-2.6.1.tar` & `craft-store-2.6.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.321117 craft-store-2.6.1/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      192 2024-03-26 17:22:41.000000 craft-store-2.6.1/.bumpversion.cfg
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2024-03-26 15:09:22.000000 craft-store-2.6.1/.editorconfig
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.311117 craft-store-2.6.1/.github/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      512 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.311117 craft-store-2.6.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1386 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      389 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      788 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      506 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/release-drafter.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3685 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/renovate.json5
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.311117 craft-store-2.6.1/.github/workflows/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1297 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/automatic-doc-checks.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/cla-check.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      854 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/docs.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      347 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1601 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/release-publish.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3595 2024-03-26 15:09:22.000000 craft-store-2.6.1/.github/workflows/tests.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2108 2024-03-26 15:09:22.000000 craft-store-2.6.1/.gitignore
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      147 2024-03-26 15:09:22.000000 craft-store-2.6.1/.gitmodules
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2024-03-26 15:09:22.000000 craft-store-2.6.1/.pre-commit-config.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      740 2024-03-26 15:09:22.000000 craft-store-2.6.1/.readthedocs.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      188 2024-03-26 15:09:22.000000 craft-store-2.6.1/.yamllint.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2024-03-26 15:09:22.000000 craft-store-2.6.1/LICENSE
--rw-r--r--   0 lengau    (1000) lengau    (1000)     3298 2024-03-26 17:26:04.321117 craft-store-2.6.1/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2387 2024-03-26 15:09:22.000000 craft-store-2.6.1/README.md
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.312116 craft-store-2.6.1/craft_store/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1207 2024-03-26 17:22:41.000000 craft-store-2.6.1/craft_store/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      411 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store/_version.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2558 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/attenuations.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    10627 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/auth.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    17715 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/base_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6796 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/creds.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7359 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/endpoints.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6469 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5737 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/http_client.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/craft_store/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2122 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2040 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/_base_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1304 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/_charm_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1886 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/_common_list_releases_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1121 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/_snap_models.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1075 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/account_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1727 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/charm_list_releases_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      877 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/error_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1886 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/registered_name_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1420 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/release_request_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2397 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/resource_revision_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2676 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/revisions_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1442 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/snap_list_releases_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1049 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/track_guardrail_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1070 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/models/track_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/py.typed
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5065 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/store_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5448 2024-03-26 15:09:22.000000 craft-store-2.6.1/craft_store/ubuntu_one_store_client.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.318117 craft-store-2.6.1/craft_store.egg-info/
--rw-r--r--   0 lengau    (1000) lengau    (1000)     3298 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store.egg-info/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3895 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store.egg-info/SOURCES.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store.egg-info/dependency_links.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      895 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store.egg-info/requires.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       12 2024-03-26 17:26:04.000000 craft-store-2.6.1/craft_store.egg-info/top_level.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/docs/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      185 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/.custom_wordlist.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/docs/.sphinx/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      336 2024-03-26 15:55:47.000000 craft-store-2.6.1/docs/.sphinx/requirements.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3414 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/Makefile
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.309116 craft-store-2.6.1/docs/_static/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/docs/_static/css/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      481 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/_static/css/custom.css
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4897 2024-03-26 17:22:41.000000 craft-store-2.6.1/docs/changelog.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4107 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/conf.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5617 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/custom_conf.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/docs/explanation/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       72 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/explanation/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.314117 craft-store-2.6.1/docs/howto/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.309116 craft-store-2.6.1/docs/howto/code/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.315117 craft-store-2.6.1/docs/howto/code/craft-cli-upload-progress/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1061 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/craft-cli-upload-progress/craft_cli_upload.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      537 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/craft-cli-upload-progress/task.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.315117 craft-store-2.6.1/docs/howto/code/upload-package-with-resources/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/upload-package-with-resources/empty-file
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      595 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/upload-package-with-resources/task.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    11207 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/upload-package-with-resources/test.charm
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3693 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/code/upload-package-with-resources/upload_package.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      636 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/craft-cli-upload-progress.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1955 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/environment-credentials.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      160 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/index.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3205 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/howto/upload-package-with-resources.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      429 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.315117 craft-store-2.6.1/docs/reference/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      129 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/reference/auto-generated.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      208 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/reference/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.315117 craft-store-2.6.1/docs/reuse/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/reuse/links.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.316116 craft-store-2.6.1/docs/tutorials/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      343 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/tutorials/index.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1005 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/tutorials/snap-store-account-info.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2409 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/tutorials/snap-store-login-ubuntu-one.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1015 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/tutorials/snap-store-login.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2811 2024-03-26 15:09:22.000000 craft-store-2.6.1/docs/tutorials/snap-store-upload-snap.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    10770 2024-03-26 15:55:47.000000 craft-store-2.6.1/pyproject.toml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2024-03-26 17:26:04.321117 craft-store-2.6.1/setup.cfg
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2375 2024-03-26 15:09:22.000000 craft-store-2.6.1/spread.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.316116 craft-store-2.6.1/tests/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/__init__.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.316116 craft-store-2.6.1/tests/integration/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/__init__.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.317116 craft-store-2.6.1/tests/integration/charmhub/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/charmhub/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     8868 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/charmhub/test_charmhub_workflow.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4780 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/conftest.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1997 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_auth.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4797 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_get_list_releases.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2311 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_list_resource_revisions.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1993 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_list_revisions.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3198 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_push_resource.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1909 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_register_unregister.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1182 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_release.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2411 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_update_resource_revisions.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1515 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/integration/test_upload.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.317116 craft-store-2.6.1/tests/unit/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3454 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-03-26 17:26:04.318117 craft-store-2.6.1/tests/unit/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1929 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_account_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5550 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_charm_list_releases_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4379 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_registered_name_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2097 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_request_release_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1637 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_resource_revision_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1396 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_revisions.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5579 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_snap_list_releases_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1804 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_track_guardrail_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2550 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/models/test_track_model.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    10217 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_auth.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    15349 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_base_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3774 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_creds.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5948 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_endpoints.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5809 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     8148 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_http_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    18616 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_store_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    17243 2024-03-26 15:09:22.000000 craft-store-2.6.1/tests/unit/test_ubuntu_one_store_client.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5388 2024-03-26 15:09:22.000000 craft-store-2.6.1/tox.ini
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.754452 craft-store-2.6.2/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      192 2024-05-06 17:33:51.000000 craft-store-2.6.2/.bumpversion.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      723 2024-05-06 09:33:23.000000 craft-store-2.6.2/.editorconfig
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.745452 craft-store-2.6.2/.github/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      512 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.745452 craft-store-2.6.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1386 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      389 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      788 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      179 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      506 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/release-drafter.yml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3685 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/renovate.json5
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.746452 craft-store-2.6.2/.github/workflows/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1297 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/automatic-doc-checks.yml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      179 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      854 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/docs.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      347 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1601 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/release-publish.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3595 2024-05-06 09:33:23.000000 craft-store-2.6.2/.github/workflows/tests.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2108 2024-05-06 09:33:23.000000 craft-store-2.6.2/.gitignore
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      147 2024-05-06 09:33:23.000000 craft-store-2.6.2/.gitmodules
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      921 2024-05-06 09:33:23.000000 craft-store-2.6.2/.pre-commit-config.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      740 2024-05-06 09:33:23.000000 craft-store-2.6.2/.readthedocs.yml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      188 2024-05-06 09:33:23.000000 craft-store-2.6.2/.yamllint.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2023-02-13 18:27:34.000000 craft-store-2.6.2/LICENSE
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     3298 2024-05-06 19:16:47.754452 craft-store-2.6.2/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2387 2024-05-06 09:33:23.000000 craft-store-2.6.2/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.747452 craft-store-2.6.2/craft_store/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1207 2024-05-06 17:33:51.000000 craft-store-2.6.2/craft_store/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      411 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store/_version.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2558 2023-02-13 18:27:34.000000 craft-store-2.6.2/craft_store/attenuations.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10750 2024-05-06 16:57:02.000000 craft-store-2.6.2/craft_store/auth.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    17715 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/base_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6796 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/creds.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7359 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/endpoints.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6469 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5737 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/http_client.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.748452 craft-store-2.6.2/craft_store/models/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2122 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2040 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/_base_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1304 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/_charm_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1886 2023-02-13 18:27:34.000000 craft-store-2.6.2/craft_store/models/_common_list_releases_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1121 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/_snap_models.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1075 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/account_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1727 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/charm_list_releases_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      877 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/error_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1886 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/registered_name_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1420 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/release_request_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2397 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/resource_revision_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2676 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/revisions_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1442 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/snap_list_releases_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1049 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/track_guardrail_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1070 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/models/track_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2023-02-13 18:27:34.000000 craft-store-2.6.2/craft_store/py.typed
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5065 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/store_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5448 2024-05-06 09:33:23.000000 craft-store-2.6.2/craft_store/ubuntu_one_store_client.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.752452 craft-store-2.6.2/craft_store.egg-info/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     3298 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3895 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      895 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       12 2024-05-06 19:16:47.000000 craft-store-2.6.2/craft_store.egg-info/top_level.txt
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.748452 craft-store-2.6.2/docs/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      192 2024-05-06 17:33:51.000000 craft-store-2.6.2/docs/.custom_wordlist.txt
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.748452 craft-store-2.6.2/docs/.sphinx/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      336 2024-05-06 16:47:13.000000 craft-store-2.6.2/docs/.sphinx/requirements.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3414 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/Makefile
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.743452 craft-store-2.6.2/docs/_static/
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.748452 craft-store-2.6.2/docs/_static/css/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      481 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/_static/css/custom.css
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5051 2024-05-06 17:33:51.000000 craft-store-2.6.2/docs/changelog.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4107 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/conf.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5617 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/custom_conf.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/explanation/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       72 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/explanation/index.rst
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/howto/
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.744452 craft-store-2.6.2/docs/howto/code/
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/howto/code/craft-cli-upload-progress/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1061 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/craft-cli-upload-progress/craft_cli_upload.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      537 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/craft-cli-upload-progress/task.yaml
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/howto/code/upload-package-with-resources/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/upload-package-with-resources/empty-file
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      595 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/upload-package-with-resources/task.yaml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    11207 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/upload-package-with-resources/test.charm
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3693 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/code/upload-package-with-resources/upload_package.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      636 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/craft-cli-upload-progress.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1955 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/environment-credentials.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      160 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/index.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3205 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/howto/upload-package-with-resources.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      429 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/index.rst
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/reference/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      129 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/reference/auto-generated.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      208 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/reference/index.rst
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.749452 craft-store-2.6.2/docs/reuse/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/reuse/links.txt
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.750452 craft-store-2.6.2/docs/tutorials/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      343 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/tutorials/index.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1005 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/tutorials/snap-store-account-info.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2409 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/tutorials/snap-store-login-ubuntu-one.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1015 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/tutorials/snap-store-login.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2811 2024-05-06 09:33:23.000000 craft-store-2.6.2/docs/tutorials/snap-store-upload-snap.rst
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10770 2024-05-06 16:47:13.000000 craft-store-2.6.2/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       38 2024-05-06 19:16:47.754452 craft-store-2.6.2/setup.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2375 2024-05-06 09:33:23.000000 craft-store-2.6.2/spread.yaml
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.750452 craft-store-2.6.2/tests/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.750452 craft-store-2.6.2/tests/integration/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2023-02-13 18:27:34.000000 craft-store-2.6.2/tests/integration/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.751452 craft-store-2.6.2/tests/integration/charmhub/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/charmhub/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8868 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/charmhub/test_charmhub_workflow.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4780 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/conftest.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1997 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_auth.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4797 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_get_list_releases.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2311 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_list_resource_revisions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1993 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_list_revisions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3198 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_push_resource.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1909 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_register_unregister.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1182 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_release.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2411 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_update_resource_revisions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1515 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/integration/test_upload.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.751452 craft-store-2.6.2/tests/unit/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2023-02-13 18:27:34.000000 craft-store-2.6.2/tests/unit/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3454 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/conftest.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-05-06 19:16:47.752452 craft-store-2.6.2/tests/unit/models/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1929 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_account_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5550 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_charm_list_releases_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4379 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_registered_name_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2097 2023-02-13 18:27:34.000000 craft-store-2.6.2/tests/unit/models/test_request_release_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1637 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_resource_revision_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1396 2023-02-13 18:27:34.000000 craft-store-2.6.2/tests/unit/models/test_revisions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5579 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_snap_list_releases_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1804 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_track_guardrail_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2550 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/models/test_track_model.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10217 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_auth.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    15349 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_base_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3774 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_creds.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5948 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_endpoints.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5809 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8148 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_http_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    18616 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_store_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    17243 2024-05-06 09:33:23.000000 craft-store-2.6.2/tests/unit/test_ubuntu_one_store_client.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5388 2024-05-06 09:33:23.000000 craft-store-2.6.2/tox.ini
```

### Comparing `craft-store-2.6.1/.editorconfig` & `craft-store-2.6.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/.jira_sync_config.yaml` & `craft-store-2.6.2/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/ISSUE_TEMPLATE/bug.yaml` & `craft-store-2.6.2/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/ISSUE_TEMPLATE/task.yaml` & `craft-store-2.6.2/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/renovate.json5` & `craft-store-2.6.2/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/workflows/automatic-doc-checks.yml` & `craft-store-2.6.2/.github/workflows/automatic-doc-checks.yml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/workflows/docs.yaml` & `craft-store-2.6.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/workflows/release-publish.yaml` & `craft-store-2.6.2/.github/workflows/release-publish.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.github/workflows/tests.yaml` & `craft-store-2.6.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.gitignore` & `craft-store-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.pre-commit-config.yaml` & `craft-store-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/.readthedocs.yml` & `craft-store-2.6.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/LICENSE` & `craft-store-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/PKG-INFO` & `craft-store-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-store
-Version: 2.6.1
+Version: 2.6.2
 Summary: Store bindings for Snaps and Charms
 Author-email: "Canonical Ltd." <snapcraft@lists.snapcraft.io>
 Project-URL: Documentation, https://craft-store.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-store
 Project-URL: Issues, https://github.com/canonical/craft-store/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `craft-store-2.6.1/README.md` & `craft-store-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/__init__.py` & `craft-store-2.6.2/craft_store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Interact with Canonical services such as Charmhub and the Snap Store."""
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 
 
 from . import creds, endpoints, errors, models
 from .auth import Auth
 from .base_client import BaseClient
 from .http_client import HTTPClient
 from .store_client import StoreClient
```

### Comparing `craft-store-2.6.1/craft_store/attenuations.py` & `craft-store-2.6.2/craft_store/attenuations.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/auth.py` & `craft-store-2.6.2/craft_store/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,22 @@
 from typing import Dict, Optional, Tuple, Union, cast
 
 import keyring
 import keyring.backend
 import keyring.backends.fail
 import keyring.errors
 from keyring._compat import properties
-from keyring.backends import SecretService
 from xdg import BaseDirectory  # type: ignore[import]
 
 from . import errors
 
+# workaround to prevent legacy provider loading in focal
+os.environ["CRYPTOGRAPHY_OPENSSL_NO_LEGACY"] = "1"
+from keyring.backends import SecretService  # noqa: E402
+
 logger = logging.getLogger(__name__)
 
 
 if sys.platform == "linux":
     from secretstorage.exceptions import SecretServiceNotAvailableException
 
     KEYRING_EXCEPTIONS = (keyring.errors.InitError, SecretServiceNotAvailableException)
```

### Comparing `craft-store-2.6.1/craft_store/base_client.py` & `craft-store-2.6.2/craft_store/base_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/creds.py` & `craft-store-2.6.2/craft_store/creds.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/endpoints.py` & `craft-store-2.6.2/craft_store/endpoints.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/errors.py` & `craft-store-2.6.2/craft_store/errors.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/http_client.py` & `craft-store-2.6.2/craft_store/http_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/__init__.py` & `craft-store-2.6.2/craft_store/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/_base_model.py` & `craft-store-2.6.2/craft_store/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/_charm_model.py` & `craft-store-2.6.2/craft_store/models/_charm_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/_common_list_releases_model.py` & `craft-store-2.6.2/craft_store/models/_common_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/_snap_models.py` & `craft-store-2.6.2/craft_store/models/_snap_models.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/account_model.py` & `craft-store-2.6.2/craft_store/models/account_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/charm_list_releases_model.py` & `craft-store-2.6.2/craft_store/models/charm_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/error_model.py` & `craft-store-2.6.2/craft_store/models/error_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/registered_name_model.py` & `craft-store-2.6.2/craft_store/models/registered_name_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/release_request_model.py` & `craft-store-2.6.2/craft_store/models/release_request_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/resource_revision_model.py` & `craft-store-2.6.2/craft_store/models/resource_revision_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/revisions_model.py` & `craft-store-2.6.2/craft_store/models/revisions_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/snap_list_releases_model.py` & `craft-store-2.6.2/craft_store/models/snap_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/track_guardrail_model.py` & `craft-store-2.6.2/craft_store/models/track_guardrail_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/models/track_model.py` & `craft-store-2.6.2/craft_store/models/track_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/store_client.py` & `craft-store-2.6.2/craft_store/store_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store/ubuntu_one_store_client.py` & `craft-store-2.6.2/craft_store/ubuntu_one_store_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store.egg-info/PKG-INFO` & `craft-store-2.6.2/craft_store.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-store
-Version: 2.6.1
+Version: 2.6.2
 Summary: Store bindings for Snaps and Charms
 Author-email: "Canonical Ltd." <snapcraft@lists.snapcraft.io>
 Project-URL: Documentation, https://craft-store.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-store
 Project-URL: Issues, https://github.com/canonical/craft-store/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `craft-store-2.6.1/craft_store.egg-info/SOURCES.txt` & `craft-store-2.6.2/craft_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/craft_store.egg-info/requires.txt` & `craft-store-2.6.2/craft_store.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/Makefile` & `craft-store-2.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/changelog.rst` & `craft-store-2.6.2/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 *********
 Changelog
 *********
+
+2.6.2 (2024-05-06)
+------------------
+
+- Disable legacy libssl providers. This is a workaround to prevent a crash
+  when loading cryptography in focal.
+
 2.6.1 (2024-03-26)
 ------------------
 
 - Remove dependency on ``protobuf``
 - Explicitly note incompatibility with ``keyring`` v25.0
 
 2.6.0 (2024-01-02)
```

### Comparing `craft-store-2.6.1/docs/conf.py` & `craft-store-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/custom_conf.py` & `craft-store-2.6.2/docs/custom_conf.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/code/craft-cli-upload-progress/craft_cli_upload.py` & `craft-store-2.6.2/docs/howto/code/craft-cli-upload-progress/craft_cli_upload.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/code/craft-cli-upload-progress/task.yaml` & `craft-store-2.6.2/docs/howto/code/craft-cli-upload-progress/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/code/upload-package-with-resources/task.yaml` & `craft-store-2.6.2/docs/howto/code/upload-package-with-resources/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/code/upload-package-with-resources/test.charm` & `craft-store-2.6.2/docs/howto/code/upload-package-with-resources/test.charm`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/code/upload-package-with-resources/upload_package.py` & `craft-store-2.6.2/docs/howto/code/upload-package-with-resources/upload_package.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/craft-cli-upload-progress.rst` & `craft-store-2.6.2/docs/howto/craft-cli-upload-progress.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/environment-credentials.rst` & `craft-store-2.6.2/docs/howto/environment-credentials.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/howto/upload-package-with-resources.rst` & `craft-store-2.6.2/docs/howto/upload-package-with-resources.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/tutorials/snap-store-account-info.rst` & `craft-store-2.6.2/docs/tutorials/snap-store-account-info.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/tutorials/snap-store-login-ubuntu-one.rst` & `craft-store-2.6.2/docs/tutorials/snap-store-login-ubuntu-one.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/tutorials/snap-store-login.rst` & `craft-store-2.6.2/docs/tutorials/snap-store-login.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/docs/tutorials/snap-store-upload-snap.rst` & `craft-store-2.6.2/docs/tutorials/snap-store-upload-snap.rst`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/pyproject.toml` & `craft-store-2.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/spread.yaml` & `craft-store-2.6.2/spread.yaml`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/charmhub/test_charmhub_workflow.py` & `craft-store-2.6.2/tests/integration/charmhub/test_charmhub_workflow.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/conftest.py` & `craft-store-2.6.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_auth.py` & `craft-store-2.6.2/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_get_list_releases.py` & `craft-store-2.6.2/tests/integration/test_get_list_releases.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_list_resource_revisions.py` & `craft-store-2.6.2/tests/integration/test_list_resource_revisions.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_list_revisions.py` & `craft-store-2.6.2/tests/integration/test_list_revisions.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_push_resource.py` & `craft-store-2.6.2/tests/integration/test_push_resource.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_register_unregister.py` & `craft-store-2.6.2/tests/integration/test_register_unregister.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_release.py` & `craft-store-2.6.2/tests/integration/test_release.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_update_resource_revisions.py` & `craft-store-2.6.2/tests/integration/test_update_resource_revisions.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/integration/test_upload.py` & `craft-store-2.6.2/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/conftest.py` & `craft-store-2.6.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_account_model.py` & `craft-store-2.6.2/tests/unit/models/test_account_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_charm_list_releases_model.py` & `craft-store-2.6.2/tests/unit/models/test_charm_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_registered_name_model.py` & `craft-store-2.6.2/tests/unit/models/test_registered_name_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_request_release_model.py` & `craft-store-2.6.2/tests/unit/models/test_request_release_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_resource_revision_model.py` & `craft-store-2.6.2/tests/unit/models/test_resource_revision_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_revisions.py` & `craft-store-2.6.2/tests/unit/models/test_revisions.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_snap_list_releases_model.py` & `craft-store-2.6.2/tests/unit/models/test_snap_list_releases_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_track_guardrail_model.py` & `craft-store-2.6.2/tests/unit/models/test_track_guardrail_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/models/test_track_model.py` & `craft-store-2.6.2/tests/unit/models/test_track_model.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_auth.py` & `craft-store-2.6.2/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_base_client.py` & `craft-store-2.6.2/tests/unit/test_base_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_creds.py` & `craft-store-2.6.2/tests/unit/test_creds.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_endpoints.py` & `craft-store-2.6.2/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_errors.py` & `craft-store-2.6.2/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_http_client.py` & `craft-store-2.6.2/tests/unit/test_http_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_store_client.py` & `craft-store-2.6.2/tests/unit/test_store_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tests/unit/test_ubuntu_one_store_client.py` & `craft-store-2.6.2/tests/unit/test_ubuntu_one_store_client.py`

 * *Files identical despite different names*

### Comparing `craft-store-2.6.1/tox.ini` & `craft-store-2.6.2/tox.ini`

 * *Files identical despite different names*

