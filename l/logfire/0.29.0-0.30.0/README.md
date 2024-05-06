# Comparing `tmp/logfire-0.29.0.tar.gz` & `tmp/logfire-0.30.0.tar.gz`

## Comparing `logfire-0.29.0.tar` & `logfire-0.30.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.29.0/Makefile
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    54920 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    12882 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    53273 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/__init__.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_backfill.py
--rw-r--r--   0        0        0    44869 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_configure.py
--rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45507 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0    67482 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_loguru.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_no_production.py
--rw-r--r--   0        0        0    53664 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_structlog.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    40300 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    42320 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.29.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.29.0/LICENSE
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 logfire-0.29.0/README.md
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 logfire-0.29.0/pyproject.toml
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 logfire-0.29.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.30.0/Makefile
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    54139 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/openai.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/__init__.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    44869 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_configure.py
+-rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45555 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0    67482 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_loguru.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    53680 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    40300 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    43085 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.30.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.30.0/LICENSE
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 logfire-0.30.0/README.md
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 logfire-0.30.0/pyproject.toml
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 logfire-0.30.0/PKG-INFO
```

### Comparing `logfire-0.29.0/Makefile` & `logfire-0.30.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/__init__.py` & `logfire-0.30.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/propagate.py` & `logfire-0.30.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/testing.py` & `logfire-0.30.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/ast_utils.py` & `logfire-0.30.0/logfire/_internal/ast_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def logfire_method_arg_values(self, qualname: str, lineno: int) -> tuple[str, dict[str, otel_types.AttributeValue]]:
         stack_info: StackInfo = {
             **get_filepath_attribute(self.filename),
             'code.lineno': lineno,
             'code.function': qualname,
         }
-        attributes: dict[str, otel_types.AttributeValue] = {**stack_info}
+        attributes: dict[str, otel_types.AttributeValue] = {**stack_info}  # type: ignore
 
         logfire_args = self.logfire_args
         msg_template = logfire_args.msg_template or f'Calling {self.module_name}.{qualname}'
         attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] = msg_template
 
         span_name = logfire_args.span_name or msg_template
```

### Comparing `logfire-0.29.0/logfire/_internal/async_.py` & `logfire-0.30.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/auth.py` & `logfire-0.30.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/backfill.py` & `logfire-0.30.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/cli.py` & `logfire-0.30.0/logfire/_internal/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     'grpc',
     'httpx',
     'jinja2',
     'kafka_python',
     'mysql',
     'mysqlclient',
     'pika',
+    'psycopg',
     'psycopg2',
     'pymemcache',
     'pymongo',
     'pymysql',
     'pyramid',
     'remoulade',
     'requests',
@@ -217,15 +218,15 @@
 
     if packages:  # pragma: no branch
         otel_packages_to_install = ' '.join(
             f'opentelemetry-instrumentation-{pkg.replace(".", "-")}' for pkg in packages.values()
         )
         install_command = f'pip install {otel_packages_to_install}'
         console.print('\n[bold green]To install these packages, run:[/bold green]\n')
-        console.print(f'[bold]$[/bold] [cyan]{install_command}[/cyan]', justify='center')
+        console.print(f'[cyan]{install_command}[/cyan]', soft_wrap=True)
         console.print('\n[bold blue]For further information, visit[/bold blue]', end=' ')
         console.print(f'[link={INTEGRATIONS_DOCS_URL}]{INTEGRATIONS_DOCS_URL}[/link]')
 
 
 def parse_auth(args: argparse.Namespace) -> None:
     """Authenticate with Logfire.
 
@@ -395,16 +396,16 @@
 
     parser.add_argument('--version', action='store_true', help='show the version and exit')
     global_opts = parser.add_argument_group(title='global options')
     global_opts.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help=argparse.SUPPRESS)
     parser.set_defaults(func=lambda _: parser.print_help())  # type: ignore
     subparsers = parser.add_subparsers(title='commands', metavar='')
 
-    # Note(DavidM): Let's try to keep the commands listed in alphabetical order if we can
-    cmd_auth = subparsers.add_parser('auth', help=parse_auth.__doc__.split('\n', 1)[0], description=parse_auth.__doc__)
+    # NOTE(DavidM): Let's try to keep the commands listed in alphabetical order if we can
+    cmd_auth = subparsers.add_parser('auth', help=parse_auth.__doc__.split('\n', 1)[0], description=parse_auth.__doc__)  # type: ignore
     cmd_auth.set_defaults(func=parse_auth)
 
     cmd_backfill = subparsers.add_parser('backfill', help=parse_backfill.__doc__)
     cmd_backfill.set_defaults(func=parse_backfill)
     cmd_backfill.add_argument('--data-dir', default='.logfire')
     cmd_backfill.add_argument('--file', default='logfire_spans.bin')
```

### Comparing `logfire-0.29.0/logfire/_internal/config.py` & `logfire-0.30.0/logfire/_internal/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,15 +815,21 @@
 
     @classmethod
     def _get_user_token(cls, logfire_api_url: str) -> str:
         if DEFAULT_FILE.is_file():  # pragma: no branch
             data = cast(DefaultFile, read_toml_file(DEFAULT_FILE))
             if is_logged_in(data, logfire_api_url):  # pragma: no branch
                 return data['tokens'][logfire_api_url]['token']
-        raise LogfireConfigError('You are not authenticated. Please run `logfire auth` to authenticate.')
+        raise LogfireConfigError(
+            """You are not authenticated. Please run `logfire auth` to authenticate.
+
+If you are running in production, you can set the `LOGFIRE_TOKEN` environment variable.
+To create a write token, refer to https://docs.pydantic.dev/logfire/guides/advanced/creating_write_tokens/
+"""
+        )
 
     @classmethod
     def get_current_user(cls, session: requests.Session, logfire_api_url: str) -> dict[str, Any] | None:
         try:
             user_token = cls._get_user_token(logfire_api_url=logfire_api_url)
         except LogfireConfigError:
             return None
```

### Comparing `logfire-0.29.0/logfire/_internal/config_params.py` & `logfire-0.30.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/constants.py` & `logfire-0.30.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/formatter.py` & `logfire-0.30.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/instrument.py` & `logfire-0.30.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/json_encoder.py` & `logfire-0.30.0/logfire/_internal/json_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,16 +235,17 @@
         seen.add(id(o))
 
         if isinstance(o, (list, tuple)):
             # we do list & tuple before Mapping as it's > twice as fast and just as common
             return [to_json_value(item, seen) for item in o]  # type: ignore
         elif isinstance(o, Mapping):
             return {
-                key if isinstance(key, str) else safe_repr(key): to_json_value(value, seen) for key, value in o.items()
-            }  # type: ignore
+                key if isinstance(key, str) else safe_repr(key): to_json_value(value, seen)
+                for key, value in o.items()  # type: ignore
+            }
         elif is_sqlalchemy(o):
             return _get_sqlalchemy_data(o, seen)
         elif dataclasses.is_dataclass(o):
             return {f.name: to_json_value(getattr(o, f.name), seen) for f in dataclasses.fields(o)}
         elif is_attrs(o):
             return _get_attrs_data(o, seen)
```

### Comparing `logfire-0.29.0/logfire/_internal/json_formatter.py` & `logfire-0.30.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/json_schema.py` & `logfire-0.30.0/logfire/_internal/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .utils import JsonDict, dump_json, safe_repr
 
 __all__ = 'create_json_schema', 'attributes_json_schema_properties', 'attributes_json_schema', 'JsonSchemaProperties'
 
 
 @lru_cache
 def type_to_schema() -> dict[type[Any], JsonDict | Callable[[Any, set[int]], JsonDict]]:
-    lookup: dict[type[Any], JsonDict | Callable[[Any], JsonDict]] = {
+    lookup: dict[type[Any], JsonDict | Callable[[Any, set[int]], JsonDict]] = {
         bytes: _bytes_schema,
         bytearray: _bytearray_schema,
         Enum: _enum_schema,
         Decimal: {'type': 'string', 'format': 'decimal'},
         datetime.datetime: {'type': 'string', 'format': 'date-time'},
         datetime.date: {'type': 'string', 'format': 'date'},
         datetime.time: {'type': 'string', 'format': 'time'},
```

### Comparing `logfire-0.29.0/logfire/_internal/json_types.py` & `logfire-0.30.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/main.py` & `logfire-0.30.0/logfire/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import atexit
 import sys
 import traceback
 import typing
 import warnings
-from functools import cached_property
+from functools import cached_property, partial
 from time import time
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Callable, ContextManager, Iterable, Literal, Sequence, TypeVar, Union, cast
 
 import opentelemetry.context as context_api
 import opentelemetry.trace as trace_api
 from opentelemetry.metrics import CallbackT, Counter, Histogram, UpDownCounter
@@ -145,15 +146,15 @@
         merged_attributes[ATTRIBUTES_MESSAGE_KEY] = log_message
 
         otlp_attributes = user_attributes(merged_attributes)
 
         if json_schema_properties := attributes_json_schema_properties(attributes):
             otlp_attributes[ATTRIBUTES_JSON_SCHEMA_KEY] = attributes_json_schema(json_schema_properties)
 
-        tags = (self._tags or ()) + tuple(_tags or ())
+        tags = cast('tuple[str, ...]', (self._tags or ()) + tuple(_tags or ()))
         if tags:
             otlp_attributes[ATTRIBUTES_TAGS_KEY] = uniquify_sequence(tags)
 
         sample_rate = (
             self._sample_rate
             if self._sample_rate is not None
             else otlp_attributes.pop(ATTRIBUTES_SAMPLE_RATE_KEY, None)
@@ -213,17 +214,18 @@
         logfire.trace('This is a trace log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('trace', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def debug(
         self,
@@ -242,17 +244,18 @@
         logfire.debug('This is a debug log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('debug', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def info(
         self,
@@ -271,17 +274,18 @@
         logfire.info('This is an info log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('info', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def notice(
         self,
@@ -300,17 +304,18 @@
         logfire.notice('This is a notice log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('notice', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def warn(
         self,
@@ -329,17 +334,18 @@
         logfire.warn('This is a warning log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('warn', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def error(
         self,
@@ -358,17 +364,18 @@
         logfire.error('This is an error log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('error', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def fatal(
         self,
@@ -387,17 +394,18 @@
         logfire.fatal('This is a fatal log')
         ```
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('fatal', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def exception(
         self,
@@ -412,15 +420,15 @@
 
         This means that a traceback will be logged for any currently handled exception.
 
         Args:
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
-            _exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
         """
         if any(k.startswith('_') for k in attributes):  # pragma: no cover
             raise ValueError('Attribute keys cannot start with an underscore.')
         self.log('error', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
 
     def span(
@@ -445,15 +453,14 @@
 
         Args:
             msg_template: The template for the span message.
             _span_name: The span name. If not provided, the `msg_template` will be used.
             _tags: An optional sequence of tags to include in the span.
             _level: An optional log level name.
             _stack_offset: The stack level offset to use when collecting stack info, defaults to `3`.
-
             attributes: The arguments to include in the span and format the message template with.
                 Attributes starting with an underscore are not allowed.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         return self._span(
             msg_template,
@@ -514,24 +521,28 @@
         ```
 
         Args:
             level: The level of the log.
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             tags: An optional sequence of tags to include in the log.
-            exc_info: Set to an exception or a tuple as returned by `sys.exc_info()`
+            exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
-                Set to True to use the currently handled exception.
+
+                Set to `True` to use the currently handled exception.
             stack_offset: The stack level offset to use when collecting stack info, also affects the warning which
                 message formatting might emit, defaults to `0` which means the stack info will be collected from the
-                position where `logfire.log` was called.
+                position where [`logfire.log`][logfire.Logfire.log] was called.
             console_log: Whether to log to the console, defaults to `True`.
-            custom_scope_suffix: A custom suffix to append to `logfire.`, should only be used when you're using
-                logfire to instrument another library like structlog or loguru.
-                See `TraceProvider.get_tracer(instrumenting_module_name)` docstring for more info.
+            custom_scope_suffix: A custom suffix to append to `logfire.` e.g. `logfire.loguru`.
+
+                It should only be used when instrumenting another library with Logfire, such as structlog or loguru.
+
+                See the `instrumenting_module_name` parameter on
+                [TracerProvider.get_tracer][opentelemetry.sdk.trace.TracerProvider.get_tracer] for more info.
         """
         stack_offset = (self._stack_offset if stack_offset is None else stack_offset) + 2
         stack_info = get_caller_stack_info(stack_offset)
 
         attributes = attributes or {}
         merged_attributes = {**stack_info, **attributes}
         if (msg := attributes.pop(ATTRIBUTES_MESSAGE_KEY, None)) is None:
@@ -634,19 +645,22 @@
     ) -> Logfire:
         """A new Logfire instance which uses the given settings.
 
         Args:
             tags: Sequence of tags to include in the log.
             stack_offset: The stack level offset to use when collecting stack info, also affects the warning which
                 message formatting might emit, defaults to `0` which means the stack info will be collected from the
-                position where `logfire.log` was called.
+                position where [`logfire.log`][logfire.Logfire.log] was called.
             console_log: Whether to log to the console, defaults to `True`.
-            custom_scope_suffix: A custom suffix to append to `logfire.`, should only be used when you're using
-                logfire to instrument another library like structlog or loguru.
-                See `TraceProvider.get_tracer(instrumenting_module_name)` docstring for more info.
+            custom_scope_suffix: A custom suffix to append to `logfire.` e.g. `logfire.loguru`.
+
+                It should only be used when instrumenting another library with Logfire, such as structlog or loguru.
+
+                See the `instrumenting_module_name` parameter on
+                [TracerProvider.get_tracer][opentelemetry.sdk.trace.TracerProvider.get_tracer] for more info.
 
         Returns:
             A new Logfire instance with the given settings applied.
         """
         # TODO add sample_rate once it's more stable
         return Logfire(
             config=self._config,
@@ -1076,15 +1090,15 @@
         This will clean up any resources used by the tracers and meters and flush any remaining spans and metrics.
 
         Args:
             timeout_millis: The timeout in milliseconds.
             flush: Whether to flush remaining spans and metrics before shutting down.
 
         Returns:
-            False if the timeout was reached before the shutdown was completed, True otherwise.
+            `False` if the timeout was reached before the shutdown was completed, `True` otherwise.
         """
         start = time()
         if flush:  # pragma: no branch
             self._tracer_provider.force_flush(timeout_millis)
         remaining = max(0, timeout_millis - (time() - start))
         if not remaining:  # pragma: no cover
             return False
@@ -1101,24 +1115,27 @@
         self._meter_provider.shutdown(remaining)
         return (start - time()) < timeout_millis
 
 
 class FastLogfireSpan:
     """A simple version of `LogfireSpan` optimized for auto-tracing."""
 
-    __slots__ = ('_span', '_token')
+    __slots__ = ('_span', '_token', '_atexit')
 
     def __init__(self, span: trace_api.Span) -> None:
         self._span = span
         self._token = context_api.attach(trace_api.set_span_in_context(self._span))
+        self._atexit = partial(self.__exit__, None, None, None)
+        atexit.register(self._atexit)
 
     def __enter__(self) -> FastLogfireSpan:
         return self
 
     def __exit__(self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: Any) -> None:
+        atexit.unregister(self._atexit)
         context_api.detach(self._token)
         _exit_span(self._span, exc_value)
         self._span.end()
 
 
 # Changes to this class may need to be reflected in `FastLogfireSpan` as well.
 class LogfireSpan(ReadableSpan):
@@ -1135,14 +1152,15 @@
         self._json_schema_properties = json_schema_properties
 
         self._added_attributes = False
         self._end_on_exit: bool | None = None
         self._token: None | object = None
         self._span: None | trace_api.Span = None
         self.end_on_exit = True
+        self._atexit: Callable[[], None] | None = None
 
     if not TYPE_CHECKING:  # pragma: no branch
 
         def __getattr__(self, name: str) -> Any:
             return getattr(self._span, name)
 
     def __enter__(self) -> LogfireSpan:
@@ -1150,20 +1168,27 @@
         if self._span is None:
             self._span = self._tracer.start_span(
                 name=self._span_name,
                 attributes=self._otlp_attributes,
             )
         if self._token is None:  # pragma: no branch
             self._token = context_api.attach(trace_api.set_span_in_context(self._span))
+
+        self._atexit = partial(self.__exit__, None, None, None)
+        atexit.register(self._atexit)
+
         return self
 
     def __exit__(self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: Any) -> None:
         if self._token is None:  # pragma: no cover
             return
 
+        if self._atexit:  # pragma: no branch
+            atexit.unregister(self._atexit)
+
         context_api.detach(self._token)
         self._token = None
 
         assert self._span is not None
         _exit_span(self._span, exc_value)
 
         end_on_exit_ = self.end_on_exit
```

### Comparing `logfire-0.29.0/logfire/_internal/metrics.py` & `logfire-0.30.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/scrubbing.py` & `logfire-0.30.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/stack_info.py` & `logfire-0.30.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/tracer.py` & `logfire-0.30.0/logfire/_internal/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         return _MaybeDeterministicTimestampSpan(
             span,
             ns_timestamp_generator=self.provider.config.ns_timestamp_generator,
         )
 
     # This means that `with start_as_current_span(...):`
     # is roughly equivalent to `with use_span(start_span(...)):`
-    start_as_current_span = SDKTracer.start_as_current_span
+    start_as_current_span = SDKTracer.start_as_current_span  # type: ignore
 
 
 @dataclass
 class PendingSpanProcessor(SpanProcessor):
     """Span processor that emits an extra pending span for each span as it starts.
 
     The pending span is emitted by calling `on_end` on all other processors.
```

### Comparing `logfire-0.29.0/logfire/_internal/utils.py` & `logfire-0.30.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.30.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.30.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.30.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/auto_trace/types.py` & `logfire-0.30.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/console.py` & `logfire-0.30.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/fallback.py` & `logfire-0.30.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/file.py` & `logfire-0.30.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/otlp.py` & `logfire-0.30.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.30.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.30.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.30.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/integrations/executors.py` & `logfire-0.30.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.30.0/logfire/_internal/integrations/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import inspect
 from contextlib import contextmanager
 from functools import lru_cache
-from typing import Any, Callable, ContextManager, Iterable, Literal
+from typing import Any, Callable, ContextManager, Iterable, Literal, cast
 from weakref import WeakKeyDictionary
 
 import fastapi.routing
 from fastapi import BackgroundTasks, FastAPI, Response
 from fastapi.routing import APIRoute, APIWebSocketRoute
 from fastapi.security import SecurityScopes
 from opentelemetry.instrumentation.asgi import get_host_port_url_tuple  # type: ignore
@@ -130,15 +130,15 @@
         else:
             self.excluded_urls_list = parse_excluded_urls(excluded_urls)  # pragma: no cover
 
     async def solve_dependencies(
         self, request: Request | WebSocket, result: tuple[dict[str, Any], list[Any], Any, Any, Any]
     ):
         try:
-            url = get_host_port_url_tuple(request.scope)[2]
+            url = cast(str, get_host_port_url_tuple(request.scope)[2])
             if self.excluded_urls_list.url_disabled(url):
                 return result  # pragma: no cover
 
             attributes: dict[str, Any] | None = {
                 # Shallow copy these so that the user can safely modify them, but we don't tell them that.
                 # We do explicitly tell them that the contents should not be modified.
                 # Making a deep copy could be very expensive and maybe even impossible.
```

### Comparing `logfire-0.29.0/logfire/_internal/integrations/openai.py` & `logfire-0.30.0/logfire/_internal/integrations/openai.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from openai.types.chat.chat_completion import ChatCompletion
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.completion import Completion
 from openai.types.create_embedding_response import CreateEmbeddingResponse
 from openai.types.images_response import ImagesResponse
 from opentelemetry import context
 
+from ..constants import ONE_SECOND_IN_NANOSECONDS
+
 if TYPE_CHECKING:
     from openai._models import FinalRequestOptions
     from openai._streaming import AsyncStream, Stream
     from openai._types import ResponseT
     from typing_extensions import LiteralString, TypedDict, Unpack
 
     from ..main import Logfire, LogfireSpan
@@ -76,15 +78,15 @@
             client._request = client._original_request_method  # type: ignore
             del client._original_request_method  # type: ignore
             client._is_instrumented_by_logfire = False  # type: ignore
 
     return uninstrument_context()
 
 
-STEAMING_MSG_TEMPLATE: LiteralString = 'streaming response from {request_data[model]!r}'
+STEAMING_MSG_TEMPLATE: LiteralString = 'streaming response from {request_data[model]!r} took {duration:.2f}s'
 
 
 def instrument_openai_sync(logfire_openai: Logfire, openai_client: openai.OpenAI, suppress_otel: bool) -> None:
     # WARNING: this method is vey similar to `instrument_openai_async` below, any changes here should be reflected there
     openai_client._original_request_method = original_request_method = openai_client._request  # type: ignore
 
     def instrumented_openai_request(**kwargs: Unpack[OpenAIRequest[ResponseT, _StreamT]]) -> ResponseT | _StreamT:
@@ -103,26 +105,18 @@
 
         if stream and content_from_stream:
             stream_cls = kwargs['stream_cls']
             assert stream_cls is not None, 'Expected `stream_cls` when streaming'
 
             class LogfireInstrumentedStream(stream_cls):
                 def __stream__(self) -> Iterator[Any]:
-                    content: list[str] = []
-                    with logfire_openai.span(STEAMING_MSG_TEMPLATE, **span_data) as stream_span:
-                        with maybe_suppress_instrumentation(suppress_otel):
-                            for chunk in super().__stream__():
-                                chunk_content = content_from_stream(chunk)
-                                if chunk_content is not None:
-                                    content.append(chunk_content)
-                                yield chunk
-                            stream_span.set_attribute(
-                                'response_data',
-                                {'combined_chunk_content': ''.join(content), 'chunk_count': len(content)},
-                            )
+                    with record_streaming(logfire_openai, span_data, content_from_stream) as record_chunk:
+                        for chunk in super().__stream__():
+                            record_chunk(chunk)
+                            yield chunk
 
             kwargs['stream_cls'] = LogfireInstrumentedStream  # type: ignore
 
         with logfire_openai.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
                     return original_request_method(**kwargs)
@@ -155,26 +149,18 @@
 
         if stream and content_from_stream:
             stream_cls = kwargs['stream_cls']
             assert stream_cls is not None, 'Expected `stream_cls` when streaming'
 
             class LogfireInstrumentedStream(stream_cls):
                 async def __stream__(self) -> AsyncIterator[Any]:
-                    content: list[str] = []
-                    with logfire_openai.span(STEAMING_MSG_TEMPLATE, **span_data) as stream_span:
-                        with maybe_suppress_instrumentation(suppress_otel):
-                            async for chunk in super().__stream__():
-                                chunk_content = content_from_stream(chunk)
-                                if chunk_content is not None:
-                                    content.append(chunk_content)
-                                yield chunk
-                            stream_span.set_attribute(
-                                'response_data',
-                                {'combined_chunk_content': ''.join(content), 'chunk_count': len(content)},
-                            )
+                    with record_streaming(logfire_openai, span_data, content_from_stream) as record_chunk:
+                        async for chunk in super().__stream__():
+                            record_chunk(chunk)
+                            yield chunk
 
             kwargs['stream_cls'] = LogfireInstrumentedStream  # type: ignore
 
         with logfire_openai.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
                     return await original_request_method(**kwargs)
@@ -270,7 +256,34 @@
         token = context.attach(new_context)
         try:
             yield
         finally:
             context.detach(token)
     else:
         yield
+
+
+@contextmanager
+def record_streaming(
+    logfire_openai: Logfire,
+    span_data: dict[str, Any],
+    content_from_stream: Callable[[Any], str | None],
+):
+    content: list[str] = []
+
+    def record_chunk(chunk: Any) -> Any:
+        chunk_content = content_from_stream(chunk)
+        if chunk_content is not None:
+            content.append(chunk_content)
+
+    timer = logfire_openai._config.ns_timestamp_generator  # type: ignore
+    start = timer()
+    try:
+        yield record_chunk
+    finally:
+        duration = (timer() - start) / ONE_SECOND_IN_NANOSECONDS
+        logfire_openai.info(
+            STEAMING_MSG_TEMPLATE,
+            **span_data,
+            duration=duration,
+            response_data={'combined_chunk_content': ''.join(content), 'chunk_count': len(content)},
+        )
```

### Comparing `logfire-0.29.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.30.0/logfire/_internal/integrations/psycopg.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         mod = importlib.import_module(name)
         skip_dep_check = check_version(name, mod.__version__, instrumentor)
 
         if kwargs.get('enable_commenter') and name == 'psycopg':
             import psycopg.pq
 
             # OTEL looks for __libpq_version__ which only exists in psycopg2.
-            mod.__libpq_version__ = psycopg.pq.version()
+            mod.__libpq_version__ = psycopg.pq.version()  # type: ignore
 
         instrumentor.instrument(skip_dep_check=skip_dep_check, **kwargs)
     else:
         # instrument_connection doesn't have a skip_dep_check argument.
         instrumentor.instrument_connection(conn)
```

### Comparing `logfire-0.29.0/logfire/integrations/logging.py` & `logfire-0.30.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/integrations/loguru.py` & `logfire-0.30.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/logfire/integrations/pydantic.py` & `logfire-0.30.0/logfire/integrations/pydantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
         # Check that we're replacing the code that's known to be buggy.
         == """
     def __getattr__(self, name: str) -> Any:
         return getattr(self._schema_validator, name)
     """.strip()
     ):
 
-        def __getattr__(self, name: str) -> Any:
+        def __getattr__(self: Any, name: str) -> Any:
             # Add these two lines to the above.
             # The exact error or return value is not important, as long as the end result
             # is an AttributeError rather than infinite recursion.
             if name == '_schema_validator':
                 raise AttributeError(name)
 
             return getattr(self._schema_validator, name)
```

### Comparing `logfire-0.29.0/logfire/integrations/structlog.py` & `logfire-0.30.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/conftest.py` & `logfire-0.30.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_auto_trace.py` & `logfire-0.30.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_backfill.py` & `logfire-0.30.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_cli.py` & `logfire-0.30.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_collect_package_resources.py` & `logfire-0.30.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_configure.py` & `logfire-0.30.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_console_exporter.py` & `logfire-0.30.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_formatter.py` & `logfire-0.30.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_json_args.py` & `logfire-0.30.0/tests/test_json_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
             Path('/tmp/test.py'),
             '/tmp/test.py',
             '"/tmp/test.py"',
             {'type': 'string', 'format': 'path', 'x-python-datatype': 'PosixPath'},
             id='path',
         ),
         pytest.param(
-            FilePath(__file__),
+            FilePath(__file__),  # type: ignore
             __file__,
             f'"{__file__}"',
             {'type': 'string', 'format': 'path', 'x-python-datatype': 'PosixPath'},
             id='pydantic_file_path',
         ),
         pytest.param(
             re.compile('test'),
@@ -636,15 +636,15 @@
                 'x-column-count': 2,
             },
             id='dataframe',
         ),
         pytest.param(
             pandas.DataFrame(
                 data={f'col{i}': [i * j for j in range(1, 23)] for i in range(1, 13)},
-                index=[f'i{x}' for x in range(1, 23)],
+                index=[f'i{x}' for x in range(1, 23)],  # type: ignore
             ),
             '     col1  col2  col3  col4  col5  ...  col8  col9  col10  col'
             '...'
             '  ...   176   198    220    242    264\n\n[22 rows x 12 columns]',
             '[[1,2,3,4,5,8,9,10,11,12],'
             '[2,4,6,8,10,16,18,20,22,24],'
             '[3,6,9,12,15,24,27,30,33,36],'
@@ -1037,15 +1037,15 @@
     class Model(BaseModel):
         lst: list[Any]
 
     @dataclass
     class Dataclass:
         dct: dict[str, Any]
 
-    dct = {}
+    dct: dict[str, Any] = {}
     data = Dataclass(dct=dct)
     lst = [data]
     model = Model(lst=lst)
     dct['model'] = model
 
     logfire.info(
         'hi',
```

### Comparing `logfire-0.29.0/tests/test_json_args_formatting.py` & `logfire-0.30.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_logfire.py` & `logfire-0.30.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_loguru.py` & `logfire-0.30.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_metrics.py` & `logfire-0.30.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_no_production.py` & `logfire-0.30.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_pydantic_plugin.py` & `logfire-0.30.0/tests/test_pydantic_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1225,8 +1225,8 @@
 
 
 def test_cloudpickle():
     class MyModel(BaseModel):
         x: int
 
     m = MyModel(x=1)
-    assert cloudpickle.loads(cloudpickle.dumps(m)).model_dump() == m.model_dump() == {'x': 1}
+    assert cloudpickle.loads(cloudpickle.dumps(m)).model_dump() == m.model_dump() == {'x': 1}  # type: ignore
```

### Comparing `logfire-0.29.0/tests/test_sampling.py` & `logfire-0.30.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_secret_scrubbing.py` & `logfire-0.30.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_slow_async_callbacks.py` & `logfire-0.30.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_source_code_extraction.py` & `logfire-0.30.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_stdlib_logging.py` & `logfire-0.30.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_structlog.py` & `logfire-0.30.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_testing.py` & `logfire-0.30.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/test_utils.py` & `logfire-0.30.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/utils.py` & `logfire-0.30.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.30.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/exporters/test_file_exporter.py` & `logfire-0.30.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/exporters/test_otlp_session.py` & `logfire-0.30.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/exporters/test_remove_pending.py` & `logfire-0.30.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.30.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.30.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_asgi.py` & `logfire-0.30.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_django.py` & `logfire-0.30.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.30.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_flask.py` & `logfire-0.30.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_httpx.py` & `logfire-0.30.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_openai.py` & `logfire-0.30.0/tests/otel_integrations/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,30 +388,32 @@
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
                 },
             },
             {
-                'name': 'streaming response from {request_data[model]!r}',
+                'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'openai.py',
-                    'code.function': '__stream__',
+                    'logfire.level_num': 9,
+                    'code.function': 'record_streaming',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
-                    'logfire.msg_template': 'streaming response from {request_data[model]!r}',
-                    'logfire.msg': "streaming response from 'gpt-4'",
-                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
+                    'logfire.span_type': 'log',
+                    'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
-                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
+                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
 def test_sync_chat_empty_response_choices(instrumented_client: openai.Client, exporter: TestExporter) -> None:
@@ -440,30 +442,32 @@
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
                 },
             },
             {
-                'name': 'streaming response from {request_data[model]!r}',
+                'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'openai.py',
-                    'code.function': '__stream__',
+                    'logfire.level_num': 9,
+                    'code.function': 'record_streaming',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty choices in response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
-                    'logfire.msg_template': 'streaming response from {request_data[model]!r}',
-                    'logfire.msg': "streaming response from 'gpt-4'",
-                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
+                    'logfire.span_type': 'log',
+                    'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
-                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
+                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
 def test_sync_chat_completions_stream(instrumented_client: openai.Client, exporter: TestExporter) -> None:
@@ -494,30 +498,32 @@
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
                 },
             },
             {
-                'name': 'streaming response from {request_data[model]!r}',
+                'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'openai.py',
-                    'code.function': '__stream__',
+                    'logfire.level_num': 9,
+                    'code.function': 'record_streaming',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': False,
-                    'logfire.msg_template': 'streaming response from {request_data[model]!r}',
-                    'logfire.msg': "streaming response from 'gpt-4'",
-                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
+                    'logfire.span_type': 'log',
+                    'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
-                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
+                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
 async def test_async_chat_completions_stream(
@@ -551,30 +557,32 @@
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
                 },
             },
             {
-                'name': 'streaming response from {request_data[model]!r}',
+                'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'openai.py',
-                    'code.function': '__stream__',
+                    'logfire.level_num': 9,
+                    'code.function': 'record_streaming',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': True,
-                    'logfire.msg_template': 'streaming response from {request_data[model]!r}',
-                    'logfire.msg': "streaming response from 'gpt-4'",
-                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
+                    'logfire.span_type': 'log',
+                    'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
-                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
+                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
 def test_completions(instrumented_client: openai.Client, exporter: TestExporter) -> None:
@@ -633,30 +641,32 @@
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
                 },
             },
             {
-                'name': 'streaming response from {request_data[model]!r}',
+                'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
-                'start_time': 3000000000,
-                'end_time': 4000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'openai.py',
-                    'code.function': '__stream__',
+                    'logfire.level_num': 9,
+                    'code.function': 'record_streaming',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?","stream":true}',
                     'async': False,
-                    'logfire.msg_template': 'streaming response from {request_data[model]!r}',
-                    'logfire.msg': "streaming response from 'gpt-3.5-turbo-instruct'",
-                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'logfire.msg': "streaming response from 'gpt-3.5-turbo-instruct' took 1.00s",
+                    'logfire.span_type': 'log',
+                    'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":3}',
-                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
+                    'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
 
 def test_embeddings(instrumented_client: openai.Client, exporter: TestExporter) -> None:
```

### Comparing `logfire-0.29.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.30.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_requests.py` & `logfire-0.30.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.30.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,8 +185,8 @@
                 'db.statement': 'DELETE FROM auth_records WHERE auth_records.id = ?',
                 'db.system': 'sqlite',
                 'db.name': 'example.db',
             },
         },
     ]
 
-    SQLAlchemyInstrumentor().uninstrument()
+    SQLAlchemyInstrumentor().uninstrument()  # type: ignore[reportUnknownMemberType]
```

### Comparing `logfire-0.29.0/tests/otel_integrations/test_starlette.py` & `logfire-0.30.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.30.0/tests/otel_integrations/test_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logfire
 from logfire.testing import TestExporter
 
 
 def test_wsgi_middleware(exporter: TestExporter) -> None:
     app = Flask(__name__)
-    app.wsgi_app = OpenTelemetryMiddleware(app.wsgi_app)  # type: ignore
+    app.wsgi_app = OpenTelemetryMiddleware(app.wsgi_app)
 
     @app.route('/')
     def homepage():  # type: ignore
         logfire.info('inside request handler')
         return 'middleware test'
 
     client = Client(app)
```

### Comparing `logfire-0.29.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.30.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/LICENSE` & `logfire-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/README.md` & `logfire-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.29.0/pyproject.toml` & `logfire-0.30.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.29.0"
+version = "0.30.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
@@ -41,30 +41,30 @@
 ]
 dependencies = [
     "opentelemetry-sdk >= 1.21.0",
     "opentelemetry-exporter-otlp-proto-http >= 1.21.0",
     "opentelemetry-instrumentation >= 0.41b0",
     "rich >= 13.4.2",
     "protobuf >= 4.23.4",
-    "typing-extensions >= 4.0.0",
+    "typing-extensions >= 4.1.0",
     "tomli >= 2.0.1; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 system-metrics = ["opentelemetry-instrumentation-system-metrics >= 0.42b0"]
 aiohttp = ["opentelemetry-instrumentation-aiohttp-client >= 0.42b0"]
 celery = ["opentelemetry-instrumentation-celery >= 0.42b0"]
 django = ["opentelemetry-instrumentation-django >= 0.42b0"]
 fastapi = ["opentelemetry-instrumentation-fastapi >= 0.42b0"]
 flask = ["opentelemetry-instrumentation-flask >= 0.42b0"]
 httpx = ["opentelemetry-instrumentation-httpx >= 0.42b0"]
 starlette = ["opentelemetry-instrumentation-starlette >= 0.42b0"]
 sqlalchemy = ["opentelemetry-instrumentation-sqlalchemy >= 0.42b0"]
 asyncpg = ["opentelemetry-instrumentation-asyncpg >= 0.42b0"]
-psycopg = ["opentelemetry-instrumentation-psycopg2 >= 0.42b0", "packaging"]
+psycopg = ["opentelemetry-instrumentation-psycopg >= 0.42b0", "packaging"]
 psycopg2 = ["opentelemetry-instrumentation-psycopg2 >= 0.42b0", "packaging"]
 pymongo = ["opentelemetry-instrumentation-pymongo >= 0.42b0"]
 redis = ["opentelemetry-instrumentation-redis >= 0.42b0"]
 requests = ["opentelemetry-instrumentation-requests >= 0.42b0"]
 
 [project.scripts]
 logfire = "logfire.cli:main"
@@ -112,15 +112,15 @@
     "devtools",
     "eval-type-backport",
     "requests-mock",
     "inline-snapshot",
     "structlog",
     "loguru",
     "ruff",
-    "pyright",
+    "pyright>=1.1.360",
     "pre-commit>=3.7.0",
     "mkdocs>=1.5.0",
     "mkdocs-material>=9.5.17",
     "mkdocs-glightbox>=0.3.7",
     "mkdocstrings-python>=1.8.0",
     "coverage[toml]>=7.5.0",
     "psycopg[binary]",
@@ -180,15 +180,15 @@
 docstring-code-format = true
 quote-style = "single"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportUnnecessaryTypeIgnoreComment = true
 reportMissingTypeStubs = false
-exclude = ["docs/**/*.py", "site/**/*.py"]
+exclude = ["docs/**/*.py", "site/**/*.py", ".venv"]
 venvPath = ".venv"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 filterwarnings = [
     "error",
     # fastapi uses deprecated pydantic functions
```

### Comparing `logfire-0.29.0/PKG-INFO` & `logfire-0.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.29.0
+Version: 0.30.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
@@ -26,15 +26,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.21.0
 Requires-Dist: opentelemetry-instrumentation>=0.41b0
 Requires-Dist: opentelemetry-sdk>=1.21.0
 Requires-Dist: protobuf>=4.23.4
 Requires-Dist: rich>=13.4.2
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
-Requires-Dist: typing-extensions>=4.0.0
+Requires-Dist: typing-extensions>=4.1.0
 Provides-Extra: aiohttp
 Requires-Dist: opentelemetry-instrumentation-aiohttp-client>=0.42b0; extra == 'aiohttp'
 Provides-Extra: asyncpg
 Requires-Dist: opentelemetry-instrumentation-asyncpg>=0.42b0; extra == 'asyncpg'
 Provides-Extra: celery
 Requires-Dist: opentelemetry-instrumentation-celery>=0.42b0; extra == 'celery'
 Provides-Extra: django
@@ -42,15 +42,15 @@
 Provides-Extra: fastapi
 Requires-Dist: opentelemetry-instrumentation-fastapi>=0.42b0; extra == 'fastapi'
 Provides-Extra: flask
 Requires-Dist: opentelemetry-instrumentation-flask>=0.42b0; extra == 'flask'
 Provides-Extra: httpx
 Requires-Dist: opentelemetry-instrumentation-httpx>=0.42b0; extra == 'httpx'
 Provides-Extra: psycopg
-Requires-Dist: opentelemetry-instrumentation-psycopg2>=0.42b0; extra == 'psycopg'
+Requires-Dist: opentelemetry-instrumentation-psycopg>=0.42b0; extra == 'psycopg'
 Requires-Dist: packaging; extra == 'psycopg'
 Provides-Extra: psycopg2
 Requires-Dist: opentelemetry-instrumentation-psycopg2>=0.42b0; extra == 'psycopg2'
 Requires-Dist: packaging; extra == 'psycopg2'
 Provides-Extra: pymongo
 Requires-Dist: opentelemetry-instrumentation-pymongo>=0.42b0; extra == 'pymongo'
 Provides-Extra: redis
```

