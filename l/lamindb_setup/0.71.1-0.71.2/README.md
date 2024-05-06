# Comparing `tmp/lamindb_setup-0.71.1.tar.gz` & `tmp/lamindb_setup-0.71.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.71.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.71.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.71.1.tar` & `lamindb_setup-0.71.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     8451 2024-04-30 14:26:00.291346 lamindb_setup-0.71.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.1/.gitignore
--rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.1/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.1/README.md
--rw-r--r--   0        0        0    99802 2024-05-03 15:45:25.498159 lamindb_setup-0.71.1/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.1/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.1/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0    10279 2024-05-03 10:05:44.384789 lamindb_setup-0.71.1/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.1/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3191 2024-05-03 13:28:51.894897 lamindb_setup-0.71.1/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3886 2024-05-03 13:28:51.895365 lamindb_setup-0.71.1/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.1/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.1/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.1/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.1/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.1/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.1/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.1/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.1/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.1/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.1/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.1/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.1/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.1/docs/index.md
--rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.1/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.1/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-03 15:45:16.228444 lamindb_setup-0.71.1/lamindb_setup/__init__.py
--rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.1/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.1/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.1/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.1/lamindb_setup/_close.py
--rw-r--r--   0        0        0    12616 2024-05-03 15:45:08.370116 lamindb_setup-0.71.1/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     7232 2024-05-03 15:45:13.866583 lamindb_setup-0.71.1/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.1/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.1/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.1/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11921 2024-05-03 10:05:44.386303 lamindb_setup-0.71.1/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.1/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.1/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.1/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1268 2024-05-03 10:05:44.386575 lamindb_setup-0.71.1/lamindb_setup/_set_managed_storage.py
--rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.1/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.1/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.1/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.1/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.1/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.1/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.1/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    15970 2024-05-03 10:05:44.386959 lamindb_setup-0.71.1/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4859 2024-05-03 10:05:44.387393 lamindb_setup-0.71.1/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.1/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.1/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.1/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3922 2024-05-03 10:05:44.387683 lamindb_setup-0.71.1/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2704 2024-05-03 10:05:44.387946 lamindb_setup-0.71.1/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    12382 2024-05-03 10:05:44.388316 lamindb_setup-0.71.1/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2084 2024-05-03 10:05:44.388614 lamindb_setup-0.71.1/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-04-25 16:11:02.480798 lamindb_setup-0.71.1/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.1/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.1/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3450 2024-04-30 14:26:00.296696 lamindb_setup-0.71.1/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.1/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.1/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.1/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    28286 2024-05-03 15:45:13.867035 lamindb_setup-0.71.1/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.1/noxfile.py
--rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.1/pyproject.toml
--rw-r--r--   0        0        0     5410 2024-04-27 13:43:14.996364 lamindb_setup-0.71.1/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      270 2024-05-03 10:05:44.388882 lamindb_setup-0.71.1/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5716 2024-05-03 10:05:44.389145 lamindb_setup-0.71.1/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.1/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.1/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      482 2024-05-03 10:05:44.389367 lamindb_setup-0.71.1/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      582 2024-04-25 16:11:02.484159 lamindb_setup-0.71.1/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11218 2024-04-30 14:26:00.298556 lamindb_setup-0.71.1/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.1/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.1/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.1/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.1/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.1/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.1/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.1/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      891 2024-05-03 15:45:13.867354 lamindb_setup-0.71.1/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.1/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.1/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.1/PKG-INFO
+-rw-r--r--   0        0        0     8571 2024-05-06 09:10:47.882123 lamindb_setup-0.71.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.2/.gitignore
+-rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.2/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.2/README.md
+-rw-r--r--   0        0        0   100264 2024-05-06 18:56:39.644805 lamindb_setup-0.71.2/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.2/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.2/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10279 2024-05-03 10:05:44.384789 lamindb_setup-0.71.2/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.2/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3191 2024-05-03 13:28:51.894897 lamindb_setup-0.71.2/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3886 2024-05-03 13:28:51.895365 lamindb_setup-0.71.2/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.2/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.2/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.2/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.2/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.2/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.2/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.2/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.2/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.2/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.2/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.2/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.2/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.2/docs/index.md
+-rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.2/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.2/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-06 18:56:19.192283 lamindb_setup-0.71.2/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.2/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.2/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.2/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.2/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12600 2024-05-06 16:12:29.980099 lamindb_setup-0.71.2/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     7232 2024-05-03 15:45:13.866583 lamindb_setup-0.71.2/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.2/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.2/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.2/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11924 2024-05-06 10:09:29.480733 lamindb_setup-0.71.2/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.2/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.2/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.2/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1268 2024-05-03 10:05:44.386575 lamindb_setup-0.71.2/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.2/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.2/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.2/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.2/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.2/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.2/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.2/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    15971 2024-05-06 14:14:11.656183 lamindb_setup-0.71.2/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-03 10:05:44.387393 lamindb_setup-0.71.2/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.2/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.2/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.2/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-03 10:05:44.387683 lamindb_setup-0.71.2/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-03 10:05:44.387946 lamindb_setup-0.71.2/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    12382 2024-05-03 10:05:44.388316 lamindb_setup-0.71.2/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-03 10:05:44.388614 lamindb_setup-0.71.2/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1563 2024-05-06 09:00:23.405007 lamindb_setup-0.71.2/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.2/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.2/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3450 2024-04-30 14:26:00.296696 lamindb_setup-0.71.2/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.2/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.2/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.2/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    28342 2024-05-06 11:31:20.317968 lamindb_setup-0.71.2/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.2/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.2/pyproject.toml
+-rw-r--r--   0        0        0     5410 2024-04-27 13:43:14.996364 lamindb_setup-0.71.2/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-03 10:05:44.388882 lamindb_setup-0.71.2/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-03 10:05:44.389145 lamindb_setup-0.71.2/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.2/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.2/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-03 10:05:44.389367 lamindb_setup-0.71.2/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      582 2024-04-25 16:11:02.484159 lamindb_setup-0.71.2/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11218 2024-04-30 14:26:00.298556 lamindb_setup-0.71.2/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.2/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.2/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.2/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.2/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.2/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.2/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.2/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-03 15:45:13.867354 lamindb_setup-0.71.2/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.2/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.2/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.2/PKG-INFO
```

### Comparing `lamindb_setup-0.71.1/.github/workflows/build.yml` & `lamindb_setup-0.71.2/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   repository_dispatch:
     types: [build]
 
 jobs:
   # tests only on production hub
   hub-prod:
     runs-on: ubuntu-latest
+    timeout-minutes: 10
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.9" # consciously run one job on Python 3.9
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml"
@@ -56,15 +57,15 @@
           cache-dependency-path: ".github/workflows/build.yml"
       - name: checkout laminhub
         uses: actions/checkout@v4
         with:
           repository: laminlabs/laminapp-ui
           token: ${{ secrets.GH_TOKEN_DEPLOY_LAMINAPP }}
           path: laminhub
-          ref: main
+          ref: 11b0e5065d6f1a05484e1ef8ab8413f3c65bfa5a
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - id: cache-postgres
         uses: actions/cache@v3
         with:
@@ -87,14 +88,15 @@
         with:
           name: coverage--hub-cloud
           path: .coverage
 
   # test user access to storage
   storage:
     runs-on: ubuntu-latest
+    timeout-minutes: 10
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10" # consciously run one job on Python 3.10
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml"
@@ -110,29 +112,29 @@
         with:
           name: coverage--storage
           path: .coverage
 
   # test low-level hub functionality
   hub-local:
     runs-on: ubuntu-latest
-    timeout-minutes: 15
+    timeout-minutes: 10
     steps:
       - uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       - uses: actions/checkout@v4
       - name: checkout laminhub
         uses: actions/checkout@v4
         with:
           repository: laminlabs/laminapp-ui
           token: ${{ secrets.GH_TOKEN_DEPLOY_LAMINAPP }}
           path: laminhub
-          ref: main
+          ref: 11b0e5065d6f1a05484e1ef8ab8413f3c65bfa5a
       - name: Set env file for local test of edge functions
         run: |
           touch .env.local
           echo "AWS_ACCESS_KEY_ID_HOSTED_S3=${{ secrets.AWS_ACCESS_KEY_ID }}" >> .env.local
           echo "AWS_SECRET_ACCESS_KEY_HOSTED_S3=${{ secrets.AWS_SECRET_ACCESS_KEY }}" >> .env.local
         working-directory: laminhub/rest-hub/supabase
       - uses: actions/setup-python@v4
```

### Comparing `lamindb_setup-0.71.1/.github/workflows/latest-changes.yml` & `lamindb_setup-0.71.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/.gitignore` & `lamindb_setup-0.71.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/.pre-commit-config.yaml` & `lamindb_setup-0.71.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/LICENSE` & `lamindb_setup-0.71.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/changelog.md` & `lamindb_setup-0.71.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Actually use local db | [751](https://github.com/laminlabs/lamindb-setup/pull/751) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 | 0.71.2
+✏️ Restore view_tree py3.9 compatibility | [750](https://github.com/laminlabs/lamindb-setup/pull/750) | [sunnyosun](https://github.com/sunnyosun) | 2024-05-06 |
+💚 Pin laminapp-ui | [749](https://github.com/laminlabs/lamindb-setup/pull/749) | [falexwolf](https://github.com/falexwolf) | 2024-05-06 |
 ♻️ Extend valid suffixes to composite suffixes | [746](https://github.com/laminlabs/lamindb-setup/pull/746) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 | 0.71.1
 🐛 Fix test failures | [745](https://github.com/laminlabs/lamindb-setup/pull/745) | [Koncopd](https://github.com/Koncopd) | 2024-05-03 |
 ♻️ Persist keep-artifacts-local in settings.env | [743](https://github.com/laminlabs/lamindb-setup/pull/743) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 |
 ✅ Expand tests to multi users for managed storage | [742](https://github.com/laminlabs/lamindb-setup/pull/742) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 |
 🐛 Fix delete function | [741](https://github.com/laminlabs/lamindb-setup/pull/741) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 | 0.71.0
 ✨ Manage multiple storage locations with integrity | [738](https://github.com/laminlabs/lamindb-setup/pull/738) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 |
 ✨ Proper progress bars for upload and download | [739](https://github.com/laminlabs/lamindb-setup/pull/739) | [Koncopd](https://github.com/Koncopd) | 2024-04-28 |
```

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.71.2/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.71.2/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/docs/notebooks.md` & `lamindb_setup-0.71.2/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/__init__.py` & `lamindb_setup-0.71.2/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.71.1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.71.2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_cache.py` & `lamindb_setup-0.71.2/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_check_setup.py` & `lamindb_setup-0.71.2/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_close.py` & `lamindb_setup-0.71.2/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.71.2/lamindb_setup/_connect_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 @unlock_cloud_sqlite_upon_exception(ignore_prev_locker=True)
 def connect(
     slug: str,
     *,
     db: str | None = None,
     storage: UPathStr | None = None,
-    _raise_not_reachable_error: bool = True,
+    _raise_not_found_error: bool = True,
     _test: bool = False,
 ) -> str | tuple | None:
     """Connect to instance.
 
     Args:
         slug: The instance slug `account_handle/instance_name` or URL.
             If the instance is owned by you, it suffices to pass the instance name.
@@ -177,20 +177,20 @@
             else:
                 message = INSTANCE_NOT_FOUND_MESSAGE.format(
                     owner=owner, name=name, hub_result=hub_result
                 )
                 if settings_file.exists():
                     isettings = load_instance_settings(settings_file)
                     if isettings.is_remote:
-                        if _raise_not_reachable_error:
+                        if _raise_not_found_error:
                             raise InstanceNotFoundError(message)
                         return "instance-not-found"
 
                 else:
-                    if _raise_not_reachable_error:
+                    if _raise_not_found_error:
                         raise InstanceNotFoundError(message)
                     return "instance-not-found"
 
         if storage is not None:
             update_isettings_with_storage(isettings, storage)
         isettings._persist()
         if _test:
@@ -205,15 +205,15 @@
             )
             if local_db:
                 logger.warning(
                     "SQLite file does not exist in the cloud, but exists locally:"
                     f" {isettings._sqlite_file_local}\nTo push the file to the cloud,"
                     " call: lamin close"
                 )
-            elif _raise_not_reachable_error:
+            elif _raise_not_found_error:
                 raise SystemExit(msg)
             else:
                 logger.warning(
                     f"instance exists with id {isettings._id.hex}, but database is not"
                     " loadable: re-initializing"
                 )
                 return "instance-corrupted-or-deleted", instance_result
```

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_delete.py` & `lamindb_setup-0.71.2/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_django.py` & `lamindb_setup-0.71.2/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_exportdb.py` & `lamindb_setup-0.71.2/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_importdb.py` & `lamindb_setup-0.71.2/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_init_instance.py` & `lamindb_setup-0.71.2/lamindb_setup/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         validate_schema_arg,
     )
 
     # should be called as the first thing
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # test whether instance exists by trying to load it
     instance_slug = f"{settings.user.handle}/{name_str}"
-    response = connect(instance_slug, _raise_not_reachable_error=False, _test=_test)
+    response = connect(instance_slug, db=db, _raise_not_found_error=False, _test=_test)
     instance_state: Literal[
         "connected",
         "instance-corrupted-or-deleted",
         "account-not-exists",
         "instance-not-found",
     ] = "connected"
     instance_id = None
```

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_migrate.py` & `lamindb_setup-0.71.2/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_register_instance.py` & `lamindb_setup-0.71.2/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_schema.py` & `lamindb_setup-0.71.2/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_set_managed_storage.py` & `lamindb_setup-0.71.2/lamindb_setup/_set_managed_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_setup_user.py` & `lamindb_setup-0.71.2/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.71.2/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_hub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         client.table("instance").insert(fields, returning="minimal").execute()
     except APIError as e:
         logger.warning("instance likely already exists")
         raise e
     client.table("storage").update(
         {"instance_id": isettings._id.hex, "is_default": True}
     ).eq("id", isettings.storage._uuid.hex).execute()  # type: ignore
-    logger.save(f"browse to: https://lamin.ai/{isettings.owner}/{isettings.name}")
+    logger.important(f"go to: https://lamin.ai/{isettings.owner}/{isettings.name}")
 
 
 def connect_instance(
     *,
     owner: str,  # account_handle
     name: str,  # instance_name
 ) -> tuple[dict, dict] | str:
```

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.71.2/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.71.2/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/django.py` & `lamindb_setup-0.71.2/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/hashing.py` & `lamindb_setup-0.71.2/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/types.py` & `lamindb_setup-0.71.2/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/lamindb_setup/core/upath.py` & `lamindb_setup-0.71.2/lamindb_setup/core/upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,16 @@
             for i in dir_path.iterdir()
             if i.as_posix().rstrip("/") != stripped_dir_path
         ]
         if only_dirs:
             contents = [d for d in contents if d.is_dir()]
         pointers = [tee] * (len(contents) - 1) + [last]
         n_files_per_dir_and_type = defaultdict(lambda: 0)  # type: ignore
-        for pointer, child_path in zip(pointers, contents, strict=False):  # type: ignore
+        # TODO: pass strict=False to zip with python > 3.9
+        for pointer, child_path in zip(pointers, contents):  # type: ignore
             if child_path.is_dir():
                 if include_dirs and child_path not in include_dirs:
                     continue
                 yield prefix + pointer + child_path.name
                 n_directories += 1
                 n_files_per_dir_and_type = defaultdict(lambda: 0)
                 extension = branch if pointer == tee else space
@@ -500,16 +501,16 @@
         folder_tree += f"\n{line}"
     if next(iterator, None):
         folder_tree += f"\n... only showing {n_max_files} out of {n_objects} files"
     directory_info = "directory" if n_directories == 1 else "directories"
     display_suffixes = ", ".join([f"{suffix!r}" for suffix in suffixes])
     suffix_message = f" with suffixes {display_suffixes}" if n_objects > 0 else ""
     message = (
-        f"{path.name} ({n_directories} sub-{directory_info} &"
-        f" {n_objects} files{suffix_message}): {folder_tree}"
+        f"{n_directories} sub-{directory_info} &"
+        f" {n_objects} files{suffix_message}\n{path.resolve()}{folder_tree}"
     )
     return message, n_objects
 
 
 # adapted from: https://stackoverflow.com/questions/9727673
 def view_tree(
     path: Path,
@@ -806,20 +807,20 @@
     n_objects = len(objects)
     n_diff = n_objects - n_offset_objects
     ask_for_deletion = (
         "delete them prior to deleting the instance"
         if raise_error
         else "consider deleting them"
     )
-    hint = "'./lamindb/_is_initialized' "
+    hint = "'_is_initialized'"
     if n_offset_objects == 2:
-        hint += "& SQLite file"
+        hint += " & SQLite file"
     hint += " ignored"
     message = (
-        f"Storage {directory_string} contains {n_objects} objects "
+        f"Storage {directory_string} contains {n_objects - n_offset_objects} objects "
         f"({hint}) - {ask_for_deletion}\n{objects}"
     )
     if n_diff > 0:
         if raise_error:
             raise InstanceNotEmpty(message)
         else:
             logger.warning(message)
```

### Comparing `lamindb_setup-0.71.1/noxfile.py` & `lamindb_setup-0.71.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/pyproject.toml` & `lamindb_setup-0.71.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.71.2/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.71.2/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-cloud/test_login.py` & `lamindb_setup-0.71.2/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-local/conftest.py` & `lamindb_setup-0.71.2/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-local/test_all.py` & `lamindb_setup-0.71.2/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-prod/conftest.py` & `lamindb_setup-0.71.2/tests/hub-prod/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.71.2/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/hub-prod/test_upath.py` & `lamindb_setup-0.71.2/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/storage/test_hashing.py` & `lamindb_setup-0.71.2/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/storage/test_storage_access.py` & `lamindb_setup-0.71.2/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/storage/test_storage_basis.py` & `lamindb_setup-0.71.2/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/storage/test_storage_stats.py` & `lamindb_setup-0.71.2/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/tests/storage/test_to_url.py` & `lamindb_setup-0.71.2/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.1/PKG-INFO` & `lamindb_setup-0.71.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.71.1
+Version: 0.71.2
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

