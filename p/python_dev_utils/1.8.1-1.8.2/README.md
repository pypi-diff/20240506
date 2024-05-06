# Comparing `tmp/python_dev_utils-1.8.1.tar.gz` & `tmp/python_dev_utils-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.8.1.tar", last modified: Fri May  3 14:03:52 2024, max compression
+gzip compressed data, was "python_dev_utils-1.8.2.tar", last modified: Mon May  6 07:01:55 2024, max compression
```

## Comparing `python_dev_utils-1.8.1.tar` & `python_dev_utils-1.8.2.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.8.1/LICENCE
--rw-r--r--   0        0        0     5202 2024-05-03 14:00:43.373038 python_dev_utils-1.8.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.8.1/dev_utils/__init__.py
--rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-1.8.1/dev_utils/alembic/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-1.8.1/dev_utils/alembic/ignore_table.py
--rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.8.1/dev_utils/alembic/migration_numbering.py
--rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-1.8.1/dev_utils/alembic/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 13:16:34.515756 python_dev_utils-1.8.1/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.8.1/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.8.1/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.8.1/dev_utils/core/results.py
--rw-r--r--   0        0        0      662 2024-05-01 13:15:58.588972 python_dev_utils-1.8.1/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.8.1/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-1.8.1/dev_utils/core/utils/envs.py
--rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-1.8.1/dev_utils/core/utils/humanize.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.8.1/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-1.8.1/dev_utils/core/utils/strings.py
--rw-r--r--   0        0        0      328 2024-05-03 13:54:07.264813 python_dev_utils-1.8.1/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.8.1/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.8.1/dev_utils/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.8.1/dev_utils/fastapi/openapi/exporter.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.8.1/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.8.1/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     4138 2024-05-02 07:47:31.057832 python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1261 2024-04-30 19:40:08.223220 python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     8096 2024-05-02 07:17:04.053247 python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0     1229 2024-04-30 19:48:16.754203 python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.8.1/dev_utils/sqlalchemy/naming_conventions.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.8.1/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-01 11:31:16.251129 python_dev_utils-1.8.1/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0     3348 2024-05-02 06:36:14.437004 python_dev_utils-1.8.1/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.8.1/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0      863 2024-05-03 13:55:40.190397 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0     3474 2024-05-03 13:51:00.856651 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/constants.py
--rw-r--r--   0        0        0    12313 2024-05-03 13:51:58.674390 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0      231 2024-05-03 13:54:58.674583 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/__init__.py
--rw-r--r--   0        0        0     3685 2024-05-03 13:58:54.208527 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/handlers.py
--rw-r--r--   0        0        0     2176 2024-05-03 13:49:22.085103 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/openapi_override.py
--rw-r--r--   0        0        0     1257 2024-05-03 13:49:14.900136 python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/utils.py
--rw-r--r--   0        0        0     3250 2024-05-03 14:03:52.180192 python_dev_utils-1.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.8.1/tests/alembic/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-1.8.1/tests/alembic/test_ignore_table.py
--rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.8.1/tests/alembic/test_migration_numbering.py
--rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-1.8.1/tests/alembic/test_utils.py
--rw-r--r--   0        0        0     9331 2024-05-02 06:38:31.027987 python_dev_utils-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.8.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/core/test_abstract.py
--rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-1.8.1/tests/core/test_datetime_utils.py
--rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-1.8.1/tests/core/test_env_utils.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.8.1/tests/core/test_guards.py
--rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-1.8.1/tests/core/test_humanize_utils.py
--rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-1.8.1/tests/core/test_inspect_utils.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/core/test_results.py
--rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-1.8.1/tests/core/test_strings_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.8.1/tests/fastapi/__init__.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.8.1/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.8.1/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.8.1/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     8627 2024-05-02 07:18:33.212683 python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.8.1/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.8.1/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.8.1/tests/sqlalchemy/test_naming_conventions.py
--rw-r--r--   0        0        0     4407 2024-05-02 06:53:17.265549 python_dev_utils-1.8.1/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.8.1/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.8.1/tests/types.py
--rw-r--r--   0        0        0     8004 2024-05-02 06:53:23.154533 python_dev_utils-1.8.1/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-03 13:53:03.076101 python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/__init__.py
--rw-r--r--   0        0        0     1463 2024-05-03 13:53:44.760914 python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/conftest.py
--rw-r--r--   0        0        0     6060 2024-05-03 13:56:41.003124 python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py
--rw-r--r--   0        0        0     1601 2024-05-03 13:56:07.243276 python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py
--rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 python_dev_utils-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.8.2/LICENCE
+-rw-r--r--   0        0        0     5202 2024-05-03 14:00:43.373038 python_dev_utils-1.8.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.8.2/dev_utils/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-1.8.2/dev_utils/alembic/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-1.8.2/dev_utils/alembic/ignore_table.py
+-rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.8.2/dev_utils/alembic/migration_numbering.py
+-rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-1.8.2/dev_utils/alembic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 13:16:34.515756 python_dev_utils-1.8.2/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.8.2/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.8.2/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.8.2/dev_utils/core/results.py
+-rw-r--r--   0        0        0      662 2024-05-01 13:15:58.588972 python_dev_utils-1.8.2/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.8.2/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-1.8.2/dev_utils/core/utils/envs.py
+-rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-1.8.2/dev_utils/core/utils/humanize.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.8.2/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-1.8.2/dev_utils/core/utils/strings.py
+-rw-r--r--   0        0        0      328 2024-05-03 13:54:07.264813 python_dev_utils-1.8.2/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.8.2/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.8.2/dev_utils/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.8.2/dev_utils/fastapi/openapi/exporter.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.8.2/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.8.2/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     4138 2024-05-02 07:47:31.057832 python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1261 2024-04-30 19:40:08.223220 python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     8096 2024-05-02 07:17:04.053247 python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0     1229 2024-04-30 19:48:16.754203 python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.8.2/dev_utils/sqlalchemy/naming_conventions.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.8.2/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-01 11:31:16.251129 python_dev_utils-1.8.2/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0     3348 2024-05-02 06:36:14.437004 python_dev_utils-1.8.2/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.8.2/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0      863 2024-05-03 13:55:40.190397 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0     3474 2024-05-03 13:51:00.856651 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/constants.py
+-rw-r--r--   0        0        0    12313 2024-05-03 13:51:58.674390 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0      309 2024-05-06 06:55:08.545628 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/__init__.py
+-rw-r--r--   0        0        0     3685 2024-05-03 13:58:54.208527 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/handlers.py
+-rw-r--r--   0        0        0     2176 2024-05-03 13:49:22.085103 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/openapi_override.py
+-rw-r--r--   0        0        0     2536 2024-05-06 06:57:09.609863 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/schemas.py
+-rw-r--r--   0        0        0     1257 2024-05-03 13:49:14.900136 python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/utils.py
+-rw-r--r--   0        0        0     3250 2024-05-06 07:01:55.173632 python_dev_utils-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.8.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.8.2/tests/alembic/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-1.8.2/tests/alembic/test_ignore_table.py
+-rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.8.2/tests/alembic/test_migration_numbering.py
+-rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-1.8.2/tests/alembic/test_utils.py
+-rw-r--r--   0        0        0     9331 2024-05-02 06:38:31.027987 python_dev_utils-1.8.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.8.2/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-1.8.2/tests/core/test_datetime_utils.py
+-rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-1.8.2/tests/core/test_env_utils.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.8.2/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-1.8.2/tests/core/test_humanize_utils.py
+-rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-1.8.2/tests/core/test_inspect_utils.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/core/test_results.py
+-rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-1.8.2/tests/core/test_strings_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.8.2/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.8.2/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.8.2/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.8.2/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     8627 2024-05-02 07:18:33.212683 python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.8.2/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.8.2/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.8.2/tests/sqlalchemy/test_naming_conventions.py
+-rw-r--r--   0        0        0     4407 2024-05-02 06:53:17.265549 python_dev_utils-1.8.2/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.8.2/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.8.2/tests/types.py
+-rw-r--r--   0        0        0     8004 2024-05-02 06:53:23.154533 python_dev_utils-1.8.2/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:53:03.076101 python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-03 13:53:44.760914 python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/conftest.py
+-rw-r--r--   0        0        0     6060 2024-05-03 13:56:41.003124 python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py
+-rw-r--r--   0        0        0     1601 2024-05-03 13:56:07.243276 python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py
+-rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 python_dev_utils-1.8.2/PKG-INFO
```

### Comparing `python_dev_utils-1.8.1/LICENCE` & `python_dev_utils-1.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/README.md` & `python_dev_utils-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/alembic/ignore_table.py` & `python_dev_utils-1.8.2/dev_utils/alembic/ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/alembic/migration_numbering.py` & `python_dev_utils-1.8.2/dev_utils/alembic/migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/alembic/utils.py` & `python_dev_utils-1.8.2/dev_utils/alembic/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/abstract.py` & `python_dev_utils-1.8.2/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/exc.py` & `python_dev_utils-1.8.2/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/guards.py` & `python_dev_utils-1.8.2/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/logging.py` & `python_dev_utils-1.8.2/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/results.py` & `python_dev_utils-1.8.2/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/utils/__init__.py` & `python_dev_utils-1.8.2/dev_utils/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/utils/envs.py` & `python_dev_utils-1.8.2/dev_utils/core/utils/envs.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/utils/humanize.py` & `python_dev_utils-1.8.2/dev_utils/core/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/utils/inspect.py` & `python_dev_utils-1.8.2/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/core/utils/strings.py` & `python_dev_utils-1.8.2/dev_utils/core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.8.2/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/fastapi/openapi/exporter.py` & `python_dev_utils-1.8.2/dev_utils/fastapi/openapi/exporter.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/naming_conventions.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/types/pydantic.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/types/pydantic.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.8.2/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/constants.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/exc.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/handlers.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/openapi_override.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/openapi_override.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/dev_utils/verbose_http_exceptions/fastapi/utils.py` & `python_dev_utils-1.8.2/dev_utils/verbose_http_exceptions/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/pyproject.toml` & `python_dev_utils-1.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
     "pytest-mock>=3.14.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.8.1"
+version = "1.8.2"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-1.8.1/tests/alembic/test_ignore_table.py` & `python_dev_utils-1.8.2/tests/alembic/test_ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/alembic/test_migration_numbering.py` & `python_dev_utils-1.8.2/tests/alembic/test_migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/alembic/test_utils.py` & `python_dev_utils-1.8.2/tests/alembic/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/conftest.py` & `python_dev_utils-1.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_abstract.py` & `python_dev_utils-1.8.2/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_env_utils.py` & `python_dev_utils-1.8.2/tests/core/test_env_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_guards.py` & `python_dev_utils-1.8.2/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_humanize_utils.py` & `python_dev_utils-1.8.2/tests/core/test_humanize_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_results.py` & `python_dev_utils-1.8.2/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/core/test_strings_utils.py` & `python_dev_utils-1.8.2/tests/core/test_strings_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.8.2/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/types.py` & `python_dev_utils-1.8.2/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/utils.py` & `python_dev_utils-1.8.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/conftest.py` & `python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py` & `python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py` & `python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py` & `python_dev_utils-1.8.2/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.8.1/PKG-INFO` & `python_dev_utils-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.8.1
+Version: 1.8.2
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
 Provides-Extra: extract-openapi
```

