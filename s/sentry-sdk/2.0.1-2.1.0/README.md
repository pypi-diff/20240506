# Comparing `tmp/sentry_sdk-2.0.1.tar.gz` & `tmp/sentry_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_sdk-2.0.1.tar", last modified: Fri Apr 26 07:36:52 2024, max compression
+gzip compressed data, was "sentry_sdk-2.1.0.tar", last modified: Mon May  6 09:04:51 2024, max compression
```

## Comparing `sentry_sdk-2.0.1.tar` & `sentry_sdk-2.1.0.tar`

### file list

```diff
@@ -1,165 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.193295 sentry_sdk-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-26 07:36:52.193295 sentry_sdk-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.169295 sentry_sdk-2.0.1/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/_werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.169295 sentry_sdk-2.0.1/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.169295 sentry_sdk-2.0.1/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.169295 sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.181295 sentry_sdk-2.0.1/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.181295 sentry_sdk-2.0.1/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.181295 sentry_sdk-2.0.1/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.181295 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.181295 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.185295 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.185295 sentry_sdk-2.0.1/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.185295 sentry_sdk-2.0.1/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55858 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    38688 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.189295 sentry_sdk-2.0.1/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 07:36:52.000000 sentry_sdk-2.0.1/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:36:52.193295 sentry_sdk-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:36:52.189295 sentry_sdk-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_propagationcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-26 07:36:44.000000 sentry_sdk-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_werkzeug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/huggingface_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.313579 sentry_sdk-2.1.0/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.313579 sentry_sdk-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_propagationcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_utils.py
```

### Comparing `sentry_sdk-2.0.1/LICENSE` & `sentry_sdk-2.1.0/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Functional Software, Inc. dba Sentry
+Copyright (c) 2018-2024 Functional Software, Inc. dba Sentry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sentry_sdk-2.0.1/PKG-INFO` & `sentry_sdk-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
@@ -26,14 +26,16 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.26.11
 Requires-Dist: certifi
 Provides-Extra: aiohttp
 Requires-Dist: aiohttp>=3.5; extra == "aiohttp"
+Provides-Extra: anthropic
+Requires-Dist: anthropic>=0.16; extra == "anthropic"
 Provides-Extra: arq
 Requires-Dist: arq>=0.23; extra == "arq"
 Provides-Extra: asyncpg
 Requires-Dist: asyncpg>=0.23; extra == "asyncpg"
 Provides-Extra: beam
 Requires-Dist: apache-beam>=2.12; extra == "beam"
 Provides-Extra: bottle
@@ -58,14 +60,18 @@
 Requires-Dist: markupsafe; extra == "flask"
 Provides-Extra: grpcio
 Requires-Dist: grpcio>=1.21.1; extra == "grpcio"
 Provides-Extra: httpx
 Requires-Dist: httpx>=0.16.0; extra == "httpx"
 Provides-Extra: huey
 Requires-Dist: huey>=2; extra == "huey"
+Provides-Extra: huggingface-hub
+Requires-Dist: huggingface_hub>=0.22; extra == "huggingface-hub"
+Provides-Extra: langchain
+Requires-Dist: langchain>=0.0.210; extra == "langchain"
 Provides-Extra: loguru
 Requires-Dist: loguru>=0.5; extra == "loguru"
 Provides-Extra: openai
 Requires-Dist: openai>=1.0.0; extra == "openai"
 Requires-Dist: tiktoken>=0.3.0; extra == "openai"
 Provides-Extra: opentelemetry
 Requires-Dist: opentelemetry-distro>=0.35b0; extra == "opentelemetry"
@@ -178,21 +184,21 @@
 - [Google Cloud Functions](https://docs.sentry.io/platforms/python/integrations/gcp-functions/)
 
 
 ## Migrating
 
 ### Migrating From `1.x` to `2.x`
 
-If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
+If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/1.x-to-2.x) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
 
 ### Migrating From `raven-python`
 
 The old `raven-python` client has entered maintenance mode and was moved [here](https://github.com/getsentry/raven-python).
 
-If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/).
+If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/raven-to-sentry-sdk/).
 
 ## Contributing to the SDK
 
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Getting Help/Support
```

### Comparing `sentry_sdk-2.0.1/README.md` & `sentry_sdk-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,21 @@
 - [Google Cloud Functions](https://docs.sentry.io/platforms/python/integrations/gcp-functions/)
 
 
 ## Migrating
 
 ### Migrating From `1.x` to `2.x`
 
-If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
+If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/1.x-to-2.x) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
 
 ### Migrating From `raven-python`
 
 The old `raven-python` client has entered maintenance mode and was moved [here](https://github.com/getsentry/raven-python).
 
-If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/).
+If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/raven-to-sentry-sdk/).
 
 ## Contributing to the SDK
 
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Getting Help/Support
```

#### html2text {}

```diff
@@ -40,24 +40,24 @@
 [Loguru](https://docs.sentry.io/platforms/python/integrations/loguru/) -
 [HTTPX](https://docs.sentry.io/platforms/python/integrations/httpx/) - [AWS
 Lambda](https://docs.sentry.io/platforms/python/integrations/aws-lambda/) -
 [Google Cloud Functions](https://docs.sentry.io/platforms/python/integrations/
 gcp-functions/) ## Migrating ### Migrating From `1.x` to `2.x` If you're on SDK
 version 1.x, we highly recommend updating to the 2.x major. To make the process
 easier we've prepared a [migration guide](https://docs.sentry.io/platforms/
-python/migration/) with the most common changes as well as a [detailed
-changelog](MIGRATION_GUIDE.md). ### Migrating From `raven-python` The old
-`raven-python` client has entered maintenance mode and was moved [here](https:/
-/github.com/getsentry/raven-python). If you're using `raven-python`, we
+python/migration/1.x-to-2.x) with the most common changes as well as a
+[detailed changelog](MIGRATION_GUIDE.md). ### Migrating From `raven-python` The
+old `raven-python` client has entered maintenance mode and was moved [here]
+(https://github.com/getsentry/raven-python). If you're using `raven-python`, we
 recommend you to migrate to this new SDK. You can find the benefits of
 migrating and how to do it in our [migration guide](https://docs.sentry.io/
-platforms/python/migration/). ## Contributing to the SDK Please refer to
-[CONTRIBUTING.md](CONTRIBUTING.md). ## Getting Help/Support If you need help
-setting up or configuring the Python SDK (or anything else in the Sentry
-universe) please head over to the [Sentry Community on Discord](https://
+platforms/python/migration/raven-to-sentry-sdk/). ## Contributing to the SDK
+Please refer to [CONTRIBUTING.md](CONTRIBUTING.md). ## Getting Help/Support If
+you need help setting up or configuring the Python SDK (or anything else in the
+Sentry universe) please head over to the [Sentry Community on Discord](https://
 discord.com/invite/Ww9hbqr). There is a ton of great people in our Discord
 community ready to help you! ## Resources - [![Documentation](https://
 img.shields.io/badge/documentation-sentry.io-green.svg)](https://
 docs.sentry.io/quickstart/) - [![Forum](https://img.shields.io/badge/forum-
 sentry-green.svg)](https://forum.sentry.io/c/sdks) - [![Discord](https://
 img.shields.io/discord/621778831602221064)](https://discord.gg/Ww9hbqr) - [!
 [Stack Overflow](https://img.shields.io/badge/stack%20overflow-sentry-
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "new_scope",
     "push_scope",
     "set_context",
     "set_extra",
     "set_level",
     "set_measurement",
     "set_tag",
+    "set_tags",
     "set_user",
     "start_span",
     "start_transaction",
 ]
 
 # Initialize the debug support after everything is loaded
 from sentry_sdk.debug import init_debug_support
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/_compat.py` & `sentry_sdk-2.1.0/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/_lru_cache.py` & `sentry_sdk-2.1.0/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/_queue.py` & `sentry_sdk-2.1.0/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/_types.py` & `sentry_sdk-2.1.0/sentry_sdk/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,53 @@
     from typing import Type
     from typing import Union
     from typing_extensions import Literal, TypedDict
 
     # "critical" is an alias of "fatal" recognized by Relay
     LogLevelStr = Literal["fatal", "critical", "error", "warning", "info", "debug"]
 
+    DurationUnit = Literal[
+        "nanosecond",
+        "microsecond",
+        "millisecond",
+        "second",
+        "minute",
+        "hour",
+        "day",
+        "week",
+    ]
+
+    InformationUnit = Literal[
+        "bit",
+        "byte",
+        "kilobyte",
+        "kibibyte",
+        "megabyte",
+        "mebibyte",
+        "gigabyte",
+        "gibibyte",
+        "terabyte",
+        "tebibyte",
+        "petabyte",
+        "pebibyte",
+        "exabyte",
+        "exbibyte",
+    ]
+
+    FractionUnit = Literal["ratio", "percent"]
+    MeasurementUnit = Union[DurationUnit, InformationUnit, FractionUnit, str]
+
+    MeasurementValue = TypedDict(
+        "MeasurementValue",
+        {
+            "value": float,
+            "unit": Optional[MeasurementUnit],
+        },
+    )
+
     Event = TypedDict(
         "Event",
         {
             "breadcrumbs": dict[
                 Literal["values"], list[dict[str, Any]]
             ],  # TODO: We can expand on this type
             "check_in_id": str,
@@ -45,15 +84,15 @@
                 Literal["values"], list[dict[str, Any]]
             ],  # TODO: We can expand on this type
             "extra": MutableMapping[str, object],
             "fingerprint": list[str],
             "level": LogLevelStr,
             "logentry": Mapping[str, object],
             "logger": str,
-            "measurements": dict[str, object],
+            "measurements": dict[str, MeasurementValue],
             "message": str,
             "modules": dict[str, str],
             "monitor_config": Mapping[str, object],
             "monitor_slug": Optional[str],
             "platform": Literal["python"],
             "profile": object,  # Should be sentry_sdk.profiler.Profile, but we can't import that here due to circular imports
             "release": str,
@@ -114,45 +153,14 @@
         "internal",
         "profile",
         "metric_bucket",
         "monitor",
     ]
     SessionStatus = Literal["ok", "exited", "crashed", "abnormal"]
 
-    DurationUnit = Literal[
-        "nanosecond",
-        "microsecond",
-        "millisecond",
-        "second",
-        "minute",
-        "hour",
-        "day",
-        "week",
-    ]
-
-    InformationUnit = Literal[
-        "bit",
-        "byte",
-        "kilobyte",
-        "kibibyte",
-        "megabyte",
-        "mebibyte",
-        "gigabyte",
-        "gibibyte",
-        "terabyte",
-        "tebibyte",
-        "petabyte",
-        "pebibyte",
-        "exabyte",
-        "exbibyte",
-    ]
-
-    FractionUnit = Literal["ratio", "percent"]
-    MeasurementUnit = Union[DurationUnit, InformationUnit, FractionUnit, str]
-
     ProfilerMode = Literal["sleep", "thread", "gevent", "unknown"]
 
     # Type of the metric.
     MetricType = Literal["d", "s", "g", "c"]
 
     # Value of the metric.
     MetricValue = Union[int, float, str]
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/_werkzeug.py` & `sentry_sdk-2.1.0/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/api.py` & `sentry_sdk-2.1.0/sentry_sdk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from sentry_sdk import tracing_utils, Client
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import INSTRUMENTER
 from sentry_sdk.scope import Scope, _ScopeManager, new_scope, isolation_scope
 from sentry_sdk.tracing import NoOpSpan, Transaction
 
 if TYPE_CHECKING:
+    from collections.abc import Mapping
+
     from typing import Any
     from typing import Dict
     from typing import Generator
     from typing import Optional
     from typing import overload
     from typing import Callable
     from typing import TypeVar
@@ -60,14 +62,15 @@
     "new_scope",
     "push_scope",
     "set_context",
     "set_extra",
     "set_level",
     "set_measurement",
     "set_tag",
+    "set_tags",
     "set_user",
     "start_span",
     "start_transaction",
 ]
 
 
 def scopemethod(f):
@@ -236,14 +239,20 @@
 @scopemethod
 def set_tag(key, value):
     # type: (str, Any) -> None
     return Scope.get_isolation_scope().set_tag(key, value)
 
 
 @scopemethod
+def set_tags(tags):
+    # type: (Mapping[str, object]) -> None
+    Scope.get_isolation_scope().set_tags(tags)
+
+
+@scopemethod
 def set_context(key, value):
     # type: (str, Dict[str, Any]) -> None
     return Scope.get_isolation_scope().set_context(key, value)
 
 
 @scopemethod
 def set_extra(key, value):
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/attachments.py` & `sentry_sdk-2.1.0/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/client.py` & `sentry_sdk-2.1.0/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/consts.py` & `sentry_sdk-2.1.0/sentry_sdk/consts.py`

 * *Files 13% similar despite different names*

```diff
@@ -87,14 +87,93 @@
 
 class SPANDATA:
     """
     Additional information describing the type of the span.
     See: https://develop.sentry.dev/sdk/performance/span-data-conventions/
     """
 
+    AI_INPUT_MESSAGES = "ai.input_messages"
+    """
+    The input messages to an LLM call.
+    Example: [{"role": "user", "message": "hello"}]
+    """
+
+    AI_MODEL_ID = "ai.model_id"
+    """
+    The unique descriptor of the model being execugted
+    Example: gpt-4
+    """
+
+    AI_METADATA = "ai.metadata"
+    """
+    Extra metadata passed to an AI pipeline step.
+    Example: {"executed_function": "add_integers"}
+    """
+
+    AI_TAGS = "ai.tags"
+    """
+    Tags that describe an AI pipeline step.
+    Example: {"executed_function": "add_integers"}
+    """
+
+    AI_STREAMING = "ai.streaming"
+    """
+    Whether or not the AI model call's repsonse was streamed back asynchronously
+    Example: true
+    """
+
+    AI_TEMPERATURE = "ai.temperature"
+    """
+    For an AI model call, the temperature parameter. Temperature essentially means how random the output will be.
+    Example: 0.5
+    """
+
+    AI_TOP_P = "ai.top_p"
+    """
+    For an AI model call, the top_p parameter. Top_p essentially controls how random the output will be.
+    Example: 0.5
+    """
+
+    AI_TOP_K = "ai.top_k"
+    """
+    For an AI model call, the top_k parameter. Top_k essentially controls how random the output will be.
+    Example: 35
+    """
+
+    AI_FUNCTION_CALL = "ai.function_call"
+    """
+    For an AI model call, the function that was called. This is deprecated for OpenAI, and replaced by tool_calls
+    """
+
+    AI_TOOL_CALLS = "ai.tool_calls"
+    """
+    For an AI model call, the function that was called. This is deprecated for OpenAI, and replaced by tool_calls
+    """
+
+    AI_TOOLS = "ai.tools"
+    """
+    For an AI model call, the functions that are available
+    """
+
+    AI_RESPONSE_FORMAT = "ai.response_format"
+    """
+    For an AI model call, the format of the response
+    """
+
+    AI_LOGIT_BIAS = "ai.response_format"
+    """
+    For an AI model call, the logit bias
+    """
+
+    AI_RESPONSES = "ai.responses"
+    """
+    The responses to an AI model call. Always as a list.
+    Example: ["hello", "world"]
+    """
+
     DB_NAME = "db.name"
     """
     The name of the database being accessed. For commands that switch the database, this should be set to the target database (even if the command fails).
     Example: myDatabase
     """
 
     DB_USER = "db.user"
@@ -213,14 +292,15 @@
     """
     Label identifying a thread from where the span originated. This should be a string.
     Example: "MainThread"
     """
 
 
 class OP:
+    ANTHROPIC_MESSAGES_CREATE = "ai.messages.create.anthropic"
     CACHE_GET_ITEM = "cache.get_item"
     DB = "db"
     DB_REDIS = "db.redis"
     EVENT_DJANGO = "event.django"
     FUNCTION = "function"
     FUNCTION_AWS = "function.aws"
     FUNCTION_GCP = "function.gcp"
@@ -241,14 +321,22 @@
     MIDDLEWARE_STARLETTE_RECEIVE = "middleware.starlette.receive"
     MIDDLEWARE_STARLETTE_SEND = "middleware.starlette.send"
     MIDDLEWARE_STARLITE = "middleware.starlite"
     MIDDLEWARE_STARLITE_RECEIVE = "middleware.starlite.receive"
     MIDDLEWARE_STARLITE_SEND = "middleware.starlite.send"
     OPENAI_CHAT_COMPLETIONS_CREATE = "ai.chat_completions.create.openai"
     OPENAI_EMBEDDINGS_CREATE = "ai.embeddings.create.openai"
+    HUGGINGFACE_HUB_CHAT_COMPLETIONS_CREATE = (
+        "ai.chat_completions.create.huggingface_hub"
+    )
+    LANGCHAIN_PIPELINE = "ai.pipeline.langchain"
+    LANGCHAIN_RUN = "ai.run.langchain"
+    LANGCHAIN_TOOL = "ai.tool.langchain"
+    LANGCHAIN_AGENT = "ai.agent.langchain"
+    LANGCHAIN_CHAT_COMPLETIONS_CREATE = "ai.chat_completions.create.langchain"
     QUEUE_SUBMIT_ARQ = "queue.submit.arq"
     QUEUE_TASK_ARQ = "queue.task.arq"
     QUEUE_SUBMIT_CELERY = "queue.submit.celery"
     QUEUE_TASK_CELERY = "queue.task.celery"
     QUEUE_TASK_RQ = "queue.task.rq"
     QUEUE_SUBMIT_HUEY = "queue.submit.huey"
     QUEUE_TASK_HUEY = "queue.task.huey"
@@ -341,8 +429,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.0.1"
+VERSION = "2.1.0"
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/crons/api.py` & `sentry_sdk-2.1.0/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/crons/decorator.py` & `sentry_sdk-2.1.0/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/django.py` & `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/debug.py` & `sentry_sdk-2.1.0/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/envelope.py` & `sentry_sdk-2.1.0/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/hub.py` & `sentry_sdk-2.1.0/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     "sentry_sdk.integrations.falcon.FalconIntegration",
     "sentry_sdk.integrations.fastapi.FastApiIntegration",
     "sentry_sdk.integrations.flask.FlaskIntegration",
     "sentry_sdk.integrations.gql.GQLIntegration",
     "sentry_sdk.integrations.graphene.GrapheneIntegration",
     "sentry_sdk.integrations.httpx.HttpxIntegration",
     "sentry_sdk.integrations.huey.HueyIntegration",
+    "sentry_sdk.integrations.huggingface_hub.HuggingfaceHubIntegration",
+    "sentry_sdk.integrations.langchain.LangchainIntegration",
     "sentry_sdk.integrations.loguru.LoguruIntegration",
     "sentry_sdk.integrations.openai.OpenAIIntegration",
     "sentry_sdk.integrations.pymongo.PyMongoIntegration",
     "sentry_sdk.integrations.pyramid.PyramidIntegration",
     "sentry_sdk.integrations.quart.QuartIntegration",
     "sentry_sdk.integrations.redis.RedisIntegration",
     "sentry_sdk.integrations.rq.RqIntegration",
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/_asgi_common.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/_wsgi_common.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/aiohttp.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/argv.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/ariadne.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/arq.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/asgi.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/asyncio.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/asyncpg.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/atexit.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/aws_lambda.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/beam.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/boto3.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/bottle.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/celery/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/celery/beat.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/beat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/celery/utils.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/chalice.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/clickhouse_driver.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/cloud_resource_context.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/dedupe.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/asgi.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/asgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Since this file contains `async def` it is conditionally imported in
 `sentry_sdk.integrations.django` (depending on the existence of
 `django.core.handlers.asgi`.
 """
 
 import asyncio
 import functools
+import inspect
 
 from django.core.handlers.wsgi import WSGIRequest
 
 import sentry_sdk
 from sentry_sdk import Scope
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
@@ -21,22 +22,39 @@
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     ensure_integration_enabled,
 )
 
 
 if TYPE_CHECKING:
-    from collections.abc import Callable
-    from typing import Any, Union
+    from typing import Any, Callable, Union, TypeVar
 
     from django.core.handlers.asgi import ASGIRequest
     from django.http.response import HttpResponse
 
     from sentry_sdk._types import Event, EventProcessor
 
+    _F = TypeVar("_F", bound=Callable[..., Any])
+
+
+# Python 3.12 deprecates asyncio.iscoroutinefunction() as an alias for
+# inspect.iscoroutinefunction(), whilst also removing the _is_coroutine marker.
+# The latter is replaced with the inspect.markcoroutinefunction decorator.
+# Until 3.12 is the minimum supported Python version, provide a shim.
+# This was copied from https://github.com/django/asgiref/blob/main/asgiref/sync.py
+if hasattr(inspect, "markcoroutinefunction"):
+    iscoroutinefunction = inspect.iscoroutinefunction
+    markcoroutinefunction = inspect.markcoroutinefunction
+else:
+    iscoroutinefunction = asyncio.iscoroutinefunction  # type: ignore[assignment]
+
+    def markcoroutinefunction(func: "_F") -> "_F":
+        func._is_coroutine = asyncio.coroutines._is_coroutine  # type: ignore
+        return func
+
 
 def _make_asgi_request_event_processor(request):
     # type: (ASGIRequest) -> EventProcessor
     def asgi_request_event_processor(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         # if the request is gone we are fine not logging the data from
         # it.  This might happen if the processor is pushed away to
@@ -177,24 +195,24 @@
         def _async_check(self):
             # type: () -> None
             """
             If get_response is a coroutine function, turns us into async mode so
             a thread is not consumed during a whole request.
             Taken from django.utils.deprecation::MiddlewareMixin._async_check
             """
-            if asyncio.iscoroutinefunction(self.get_response):
-                self._is_coroutine = asyncio.coroutines._is_coroutine  # type: ignore
+            if iscoroutinefunction(self.get_response):
+                markcoroutinefunction(self)
 
         def async_route_check(self):
             # type: () -> bool
             """
             Function that checks if we are in async mode,
             and if we are forwards the handling of requests to __acall__
             """
-            return asyncio.iscoroutinefunction(self.get_response)
+            return iscoroutinefunction(self.get_response)
 
         async def __acall__(self, *args, **kwargs):
             # type: (*Any, **Any) -> Any
             f = self._acall_method
             if f is None:
                 if hasattr(self._inner, "__acall__"):
                     self._acall_method = f = self._inner.__acall__  # type: ignore
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/caching.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/middleware.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/signals_handlers.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/templates.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/transactions.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/django/views.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/excepthook.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/executing.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/falcon.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/fastapi.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/flask.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/gcp.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/gnu_backtrace.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/gql.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/graphene.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/client.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/aio/server.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/client.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/grpc/server.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/httpx.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/huey.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/logging.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/loguru.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/modules.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/openai.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from functools import wraps
 
 from sentry_sdk import consts
 from sentry_sdk._types import TYPE_CHECKING
+from sentry_sdk.ai.monitoring import record_token_usage
+from sentry_sdk.consts import SPANDATA
+from sentry_sdk.ai.utils import set_data_normalized
 
 if TYPE_CHECKING:
     from typing import Any, Iterable, List, Optional, Callable, Iterator
     from sentry_sdk.tracing import Span
 
 import sentry_sdk
 from sentry_sdk.scope import should_send_default_pii
@@ -44,19 +47,14 @@
     )
 
     def count_tokens(s):
         # type: (str) -> int
         return 0
 
 
-COMPLETION_TOKENS_USED = "ai.completion_tоkens.used"
-PROMPT_TOKENS_USED = "ai.prompt_tоkens.used"
-TOTAL_TOKENS_USED = "ai.total_tоkens.used"
-
-
 class OpenAIIntegration(Integration):
     identifier = "openai"
 
     def __init__(self, include_prompts=True):
         # type: (OpenAIIntegration, bool) -> None
         self.include_prompts = include_prompts
 
@@ -73,43 +71,21 @@
         exc,
         client_options=sentry_sdk.get_client().options,
         mechanism={"type": "openai", "handled": False},
     )
     sentry_sdk.capture_event(event, hint=hint)
 
 
-def _normalize_data(data):
-    # type: (Any) -> Any
-
-    # convert pydantic data (e.g. OpenAI v1+) to json compatible format
-    if hasattr(data, "model_dump"):
-        try:
-            return data.model_dump()
-        except Exception as e:
-            logger.warning("Could not convert pydantic data to JSON: %s", e)
-            return data
-    if isinstance(data, list):
-        return list(_normalize_data(x) for x in data)
-    if isinstance(data, dict):
-        return {k: _normalize_data(v) for (k, v) in data.items()}
-    return data
-
-
-def set_data_normalized(span, key, value):
-    # type: (Span, str, Any) -> None
-    span.set_data(key, _normalize_data(value))
-
-
 def _calculate_chat_completion_usage(
     messages, response, span, streaming_message_responses=None
 ):
     # type: (Iterable[ChatCompletionMessageParam], Any, Span, Optional[List[str]]) -> None
-    completion_tokens = 0
-    prompt_tokens = 0
-    total_tokens = 0
+    completion_tokens = 0  # type: Optional[int]
+    prompt_tokens = 0  # type: Optional[int]
+    total_tokens = 0  # type: Optional[int]
     if hasattr(response, "usage"):
         if hasattr(response.usage, "completion_tokens") and isinstance(
             response.usage.completion_tokens, int
         ):
             completion_tokens = response.usage.completion_tokens
         if hasattr(response.usage, "prompt_tokens") and isinstance(
             response.usage.prompt_tokens, int
@@ -130,23 +106,21 @@
             for message in streaming_message_responses:
                 completion_tokens += count_tokens(message)
         elif hasattr(response, "choices"):
             for choice in response.choices:
                 if hasattr(choice, "message"):
                     completion_tokens += count_tokens(choice.message)
 
+    if prompt_tokens == 0:
+        prompt_tokens = None
+    if completion_tokens == 0:
+        completion_tokens = None
     if total_tokens == 0:
-        total_tokens = prompt_tokens + completion_tokens
-
-    if completion_tokens != 0:
-        set_data_normalized(span, COMPLETION_TOKENS_USED, completion_tokens)
-    if prompt_tokens != 0:
-        set_data_normalized(span, PROMPT_TOKENS_USED, prompt_tokens)
-    if total_tokens != 0:
-        set_data_normalized(span, TOTAL_TOKENS_USED, total_tokens)
+        total_tokens = None
+    record_token_usage(span, prompt_tokens, completion_tokens, total_tokens)
 
 
 def _wrap_chat_completion_create(f):
     # type: (Callable[..., Any]) -> Callable[..., Any]
     @wraps(f)
     @ensure_integration_enabled(OpenAIIntegration, f)
     def new_chat_completion(*args, **kwargs):
@@ -163,32 +137,33 @@
 
         kwargs["messages"] = list(kwargs["messages"])
         messages = kwargs["messages"]
         model = kwargs.get("model")
         streaming = kwargs.get("stream")
 
         span = sentry_sdk.start_span(
-            op=consts.OP.OPENAI_CHAT_COMPLETIONS_CREATE, description="Chat Completion"
+            op=consts.OP.OPENAI_CHAT_COMPLETIONS_CREATE,
+            description="Chat Completion",
         )
         span.__enter__()
         try:
             res = f(*args, **kwargs)
         except Exception as e:
             _capture_exception(e)
             span.__exit__(None, None, None)
             raise e from None
 
         integration = sentry_sdk.get_client().get_integration(OpenAIIntegration)
 
         with capture_internal_exceptions():
             if should_send_default_pii() and integration.include_prompts:
-                set_data_normalized(span, "ai.input_messages", messages)
+                set_data_normalized(span, SPANDATA.AI_INPUT_MESSAGES, messages)
 
-            set_data_normalized(span, "ai.model_id", model)
-            set_data_normalized(span, "ai.streaming", streaming)
+            set_data_normalized(span, SPANDATA.AI_MODEL_ID, model)
+            set_data_normalized(span, SPANDATA.AI_STREAMING, streaming)
 
             if hasattr(res, "choices"):
                 if should_send_default_pii() and integration.include_prompts:
                     set_data_normalized(
                         span,
                         "ai.responses",
                         list(map(lambda x: x.message, res.choices)),
@@ -220,15 +195,17 @@
                             all_responses = list(
                                 map(lambda chunk: "".join(chunk), data_buf)
                             )
                             if (
                                 should_send_default_pii()
                                 and integration.include_prompts
                             ):
-                                set_data_normalized(span, "ai.responses", all_responses)
+                                set_data_normalized(
+                                    span, SPANDATA.AI_RESPONSES, all_responses
+                                )
                             _calculate_chat_completion_usage(
                                 messages, res, span, all_responses
                             )
                     span.__exit__(None, None, None)
 
                 res._iterator = new_iterator()
             else:
@@ -281,16 +258,12 @@
                     response.usage.total_tokens, int
                 ):
                     total_tokens = response.usage.total_tokens
 
             if prompt_tokens == 0:
                 prompt_tokens = count_tokens(kwargs["input"] or "")
 
-            if total_tokens == 0:
-                total_tokens = prompt_tokens
-
-            set_data_normalized(span, PROMPT_TOKENS_USED, prompt_tokens)
-            set_data_normalized(span, TOTAL_TOKENS_USED, total_tokens)
+            record_token_usage(span, prompt_tokens, None, total_tokens or prompt_tokens)
 
             return response
 
     return new_embeddings_create
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/pure_eval.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/pymongo.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/pyramid.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/quart.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/quart.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,19 @@
         patch_scaffold_route()
 
 
 def patch_asgi_app():
     # type: () -> None
     old_app = Quart.__call__
 
-    @ensure_integration_enabled(QuartIntegration, old_app)
     async def sentry_patched_asgi_app(self, scope, receive, send):
         # type: (Any, Any, Any, Any) -> Any
+        if sentry_sdk.get_client().get_integration(QuartIntegration) is None:
+            return await old_app(self, scope, receive, send)
+
         middleware = SentryAsgiMiddleware(lambda *a, **kw: old_app(self, *a, **kw))
         middleware.__call__ = middleware._run_asgi3
         return await middleware(scope, receive, send)
 
     Quart.__call__ = sentry_patched_asgi_app
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/redis/__init__.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/redis/asyncio.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/rq.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/sanic.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/serverless.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/socket.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/spark/spark_driver.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/spark/spark_worker.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/sqlalchemy.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/starlette.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/starlite.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/stdlib.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/strawberry.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/threading.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/tornado.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/trytond.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/integrations/wsgi.py` & `sentry_sdk-2.1.0/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/metrics.py` & `sentry_sdk-2.1.0/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/monitor.py` & `sentry_sdk-2.1.0/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/profiler.py` & `sentry_sdk-2.1.0/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/scope.py` & `sentry_sdk-2.1.0/sentry_sdk/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ContextVar,
     event_from_exception,
     exc_info_from_error,
     logger,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import MutableMapping
+    from collections.abc import Mapping, MutableMapping
 
     from typing import Any
     from typing import Callable
     from typing import Deque
     from typing import Dict
     from typing import Generator
     from typing import Iterator
@@ -795,14 +795,33 @@
 
         :param key: Key of the tag to set.
 
         :param value: Value of the tag to set.
         """
         self._tags[key] = value
 
+    def set_tags(self, tags):
+        # type: (Mapping[str, object]) -> None
+        """Sets multiple tags at once.
+
+        This method updates multiple tags at once. The tags are passed as a dictionary
+        or other mapping type.
+
+        Calling this method is equivalent to calling `set_tag` on each key-value pair
+        in the mapping. If a tag key already exists in the scope, its value will be
+        updated. If the tag key does not exist in the scope, the key-value pair will
+        be added to the scope.
+
+        This method only modifies tag keys in the `tags` mapping passed to the method.
+        `scope.set_tags({})` is, therefore, a no-op.
+
+        :param tags: A mapping of tag keys to tag values to set.
+        """
+        self._tags.update(tags)
+
     def remove_tag(self, key):
         # type: (str) -> None
         """
         Removes a specific tag.
 
         :param key: Key of the tag to remove.
         """
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/scrubber.py` & `sentry_sdk-2.1.0/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/serializer.py` & `sentry_sdk-2.1.0/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/session.py` & `sentry_sdk-2.1.0/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/sessions.py` & `sentry_sdk-2.1.0/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/spotlight.py` & `sentry_sdk-2.1.0/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/tracing.py` & `sentry_sdk-2.1.0/sentry_sdk/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     get_current_thread_meta,
     is_valid_sample_rate,
     logger,
     nanosecond_time,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
-
 if TYPE_CHECKING:
     from collections.abc import Callable, Mapping, MutableMapping
     from typing import Any
     from typing import Dict
     from typing import Iterator
     from typing import List
     from typing import Optional
@@ -28,15 +27,20 @@
 
     from typing_extensions import TypedDict, Unpack
 
     P = ParamSpec("P")
     R = TypeVar("R")
 
     import sentry_sdk.profiler
-    from sentry_sdk._types import Event, MeasurementUnit, SamplingContext
+    from sentry_sdk._types import (
+        Event,
+        MeasurementUnit,
+        SamplingContext,
+        MeasurementValue,
+    )
 
     class SpanKwargs(TypedDict, total=False):
         trace_id: str
         """
         The trace ID of the root span. If this new span is to be the root span,
         omit this parameter, and a new trace ID will be generated.
         """
@@ -185,14 +189,15 @@
         "trace_id",
         "span_id",
         "parent_span_id",
         "same_process_as_parent",
         "sampled",
         "op",
         "description",
+        "_measurements",
         "start_timestamp",
         "_start_timestamp_monotonic_ns",
         "status",
         "timestamp",
         "_tags",
         "_data",
         "_span_recorder",
@@ -225,14 +230,15 @@
         self.same_process_as_parent = same_process_as_parent
         self.sampled = sampled
         self.op = op
         self.description = description
         self.status = status
         self.hub = hub
         self.scope = scope
+        self._measurements = {}  # type: Dict[str, MeasurementValue]
         self._tags = {}  # type: MutableMapping[str, str]
         self._data = {}  # type: Dict[str, Any]
         self._containing_transaction = containing_transaction
         if start_timestamp is None:
             start_timestamp = datetime.now(timezone.utc)
         elif isinstance(start_timestamp, float):
             start_timestamp = datetime.fromtimestamp(start_timestamp, timezone.utc)
@@ -484,14 +490,18 @@
         # type: (str, Any) -> None
         self._data[key] = value
 
     def set_status(self, value):
         # type: (str) -> None
         self.status = value
 
+    def set_measurement(self, name, value, unit=""):
+        # type: (str, float, MeasurementUnit) -> None
+        self._measurements[name] = {"value": value, "unit": unit}
+
     def set_thread(self, thread_id, thread_name):
         # type: (Optional[int], Optional[str]) -> None
 
         if thread_id is not None:
             self.set_data(SPANDATA.THREAD_ID, str(thread_id))
 
             if thread_name is not None:
@@ -594,14 +604,17 @@
             self._tags["status"] = self.status
 
         if self._local_aggregator is not None:
             metrics_summary = self._local_aggregator.to_json()
             if metrics_summary:
                 rv["_metrics_summary"] = metrics_summary
 
+        if len(self._measurements) > 0:
+            rv["measurements"] = self._measurements
+
         tags = self._tags
         if tags:
             rv["tags"] = tags
 
         data = self._data
         if data:
             rv["data"] = data
@@ -670,15 +683,15 @@
 
         super().__init__(**kwargs)
 
         self.name = name
         self.source = source
         self.sample_rate = None  # type: Optional[float]
         self.parent_sampled = parent_sampled
-        self._measurements = {}  # type: Dict[str, Any]
+        self._measurements = {}  # type: Dict[str, MeasurementValue]
         self._contexts = {}  # type: Dict[str, Any]
         self._profile = None  # type: Optional[sentry_sdk.profiler.Profile]
         self._baggage = baggage
 
     def __repr__(self):
         # type: () -> str
         return (
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk/tracing_utils.py` & `sentry_sdk-2.1.0/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/transport.py` & `sentry_sdk-2.1.0/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/types.py` & `sentry_sdk-2.1.0/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/utils.py` & `sentry_sdk-2.1.0/sentry_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk/worker.py` & `sentry_sdk-2.1.0/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/sentry_sdk.egg-info/PKG-INFO` & `sentry_sdk-2.1.0/sentry_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
@@ -26,14 +26,16 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.26.11
 Requires-Dist: certifi
 Provides-Extra: aiohttp
 Requires-Dist: aiohttp>=3.5; extra == "aiohttp"
+Provides-Extra: anthropic
+Requires-Dist: anthropic>=0.16; extra == "anthropic"
 Provides-Extra: arq
 Requires-Dist: arq>=0.23; extra == "arq"
 Provides-Extra: asyncpg
 Requires-Dist: asyncpg>=0.23; extra == "asyncpg"
 Provides-Extra: beam
 Requires-Dist: apache-beam>=2.12; extra == "beam"
 Provides-Extra: bottle
@@ -58,14 +60,18 @@
 Requires-Dist: markupsafe; extra == "flask"
 Provides-Extra: grpcio
 Requires-Dist: grpcio>=1.21.1; extra == "grpcio"
 Provides-Extra: httpx
 Requires-Dist: httpx>=0.16.0; extra == "httpx"
 Provides-Extra: huey
 Requires-Dist: huey>=2; extra == "huey"
+Provides-Extra: huggingface-hub
+Requires-Dist: huggingface_hub>=0.22; extra == "huggingface-hub"
+Provides-Extra: langchain
+Requires-Dist: langchain>=0.0.210; extra == "langchain"
 Provides-Extra: loguru
 Requires-Dist: loguru>=0.5; extra == "loguru"
 Provides-Extra: openai
 Requires-Dist: openai>=1.0.0; extra == "openai"
 Requires-Dist: tiktoken>=0.3.0; extra == "openai"
 Provides-Extra: opentelemetry
 Requires-Dist: opentelemetry-distro>=0.35b0; extra == "opentelemetry"
@@ -178,21 +184,21 @@
 - [Google Cloud Functions](https://docs.sentry.io/platforms/python/integrations/gcp-functions/)
 
 
 ## Migrating
 
 ### Migrating From `1.x` to `2.x`
 
-If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
+If you're on SDK version 1.x, we highly recommend updating to the 2.x major. To make the process easier we've prepared a [migration guide](https://docs.sentry.io/platforms/python/migration/1.x-to-2.x) with the most common changes as well as a [detailed changelog](MIGRATION_GUIDE.md).
 
 ### Migrating From `raven-python`
 
 The old `raven-python` client has entered maintenance mode and was moved [here](https://github.com/getsentry/raven-python).
 
-If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/).
+If you're using `raven-python`, we recommend you to migrate to this new SDK. You can find the benefits of migrating and how to do it in our [migration guide](https://docs.sentry.io/platforms/python/migration/raven-to-sentry-sdk/).
 
 ## Contributing to the SDK
 
 Please refer to [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Getting Help/Support
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk.egg-info/SOURCES.txt` & `sentry_sdk-2.1.0/sentry_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,26 +34,30 @@
 sentry_sdk/worker.py
 sentry_sdk.egg-info/PKG-INFO
 sentry_sdk.egg-info/SOURCES.txt
 sentry_sdk.egg-info/dependency_links.txt
 sentry_sdk.egg-info/not-zip-safe
 sentry_sdk.egg-info/requires.txt
 sentry_sdk.egg-info/top_level.txt
+sentry_sdk/ai/__init__.py
+sentry_sdk/ai/monitoring.py
+sentry_sdk/ai/utils.py
 sentry_sdk/crons/__init__.py
 sentry_sdk/crons/api.py
 sentry_sdk/crons/consts.py
 sentry_sdk/crons/decorator.py
 sentry_sdk/db/__init__.py
 sentry_sdk/db/explain_plan/__init__.py
 sentry_sdk/db/explain_plan/django.py
 sentry_sdk/db/explain_plan/sqlalchemy.py
 sentry_sdk/integrations/__init__.py
 sentry_sdk/integrations/_asgi_common.py
 sentry_sdk/integrations/_wsgi_common.py
 sentry_sdk/integrations/aiohttp.py
+sentry_sdk/integrations/anthropic.py
 sentry_sdk/integrations/argv.py
 sentry_sdk/integrations/ariadne.py
 sentry_sdk/integrations/arq.py
 sentry_sdk/integrations/asgi.py
 sentry_sdk/integrations/asyncio.py
 sentry_sdk/integrations/asyncpg.py
 sentry_sdk/integrations/atexit.py
@@ -72,14 +76,16 @@
 sentry_sdk/integrations/flask.py
 sentry_sdk/integrations/gcp.py
 sentry_sdk/integrations/gnu_backtrace.py
 sentry_sdk/integrations/gql.py
 sentry_sdk/integrations/graphene.py
 sentry_sdk/integrations/httpx.py
 sentry_sdk/integrations/huey.py
+sentry_sdk/integrations/huggingface_hub.py
+sentry_sdk/integrations/langchain.py
 sentry_sdk/integrations/logging.py
 sentry_sdk/integrations/loguru.py
 sentry_sdk/integrations/modules.py
 sentry_sdk/integrations/openai.py
 sentry_sdk/integrations/pure_eval.py
 sentry_sdk/integrations/pymongo.py
 sentry_sdk/integrations/pyramid.py
```

### Comparing `sentry_sdk-2.0.1/sentry_sdk.egg-info/requires.txt` & `sentry_sdk-2.1.0/sentry_sdk.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 urllib3>=1.26.11
 certifi
 
 [aiohttp]
 aiohttp>=3.5
 
+[anthropic]
+anthropic>=0.16
+
 [arq]
 arq>=0.23
 
 [asyncpg]
 asyncpg>=0.23
 
 [beam]
@@ -47,14 +50,20 @@
 
 [httpx]
 httpx>=0.16.0
 
 [huey]
 huey>=2
 
+[huggingface_hub]
+huggingface_hub>=0.22
+
+[langchain]
+langchain>=0.0.210
+
 [loguru]
 loguru>=0.5
 
 [openai]
 openai>=1.0.0
 tiktoken>=0.3.0
```

### Comparing `sentry_sdk-2.0.1/setup.py` & `sentry_sdk-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.0.1",
+    version="2.1.0",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
@@ -40,14 +40,15 @@
     python_requires=">=3.6",
     install_requires=[
         "urllib3>=1.26.11",
         "certifi",
     ],
     extras_require={
         "aiohttp": ["aiohttp>=3.5"],
+        "anthropic": ["anthropic>=0.16"],
         "arq": ["arq>=0.23"],
         "asyncpg": ["asyncpg>=0.23"],
         "beam": ["apache-beam>=2.12"],
         "bottle": ["bottle>=0.12.13"],
         "celery": ["celery>=3"],
         "celery-redbeat": ["celery-redbeat>=2"],
         "chalice": ["chalice>=1.16.0"],
@@ -55,14 +56,16 @@
         "django": ["django>=1.8"],
         "falcon": ["falcon>=1.4"],
         "fastapi": ["fastapi>=0.79.0"],
         "flask": ["flask>=0.11", "blinker>=1.1", "markupsafe"],
         "grpcio": ["grpcio>=1.21.1"],
         "httpx": ["httpx>=0.16.0"],
         "huey": ["huey>=2"],
+        "huggingface_hub": ["huggingface_hub>=0.22"],
+        "langchain": ["langchain>=0.0.210"],
         "loguru": ["loguru>=0.5"],
         "openai": ["openai>=1.0.0", "tiktoken>=0.3.0"],
         "opentelemetry": ["opentelemetry-distro>=0.35b0"],
         "opentelemetry-experimental": [
             "opentelemetry-distro~=0.40b0",
             "opentelemetry-instrumentation-aiohttp-client~=0.40b0",
             "opentelemetry-instrumentation-django~=0.40b0",
```

### Comparing `sentry_sdk-2.0.1/tests/test_basics.py` & `sentry_sdk-2.1.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_client.py` & `sentry_sdk-2.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_conftest.py` & `sentry_sdk-2.1.0/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_crons.py` & `sentry_sdk-2.1.0/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_envelope.py` & `sentry_sdk-2.1.0/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_exceptiongroup.py` & `sentry_sdk-2.1.0/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_lru_cache.py` & `sentry_sdk-2.1.0/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_metrics.py` & `sentry_sdk-2.1.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_monitor.py` & `sentry_sdk-2.1.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_new_scopes_compat.py` & `sentry_sdk-2.1.0/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_new_scopes_compat_event.py` & `sentry_sdk-2.1.0/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_profiler.py` & `sentry_sdk-2.1.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_propagationcontext.py` & `sentry_sdk-2.1.0/tests/test_propagationcontext.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_scope.py` & `sentry_sdk-2.1.0/tests/test_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,7 +792,33 @@
     assert should_send_default_pii() is True
 
 
 def test_should_send_default_pii_false(sentry_init):
     sentry_init(send_default_pii=False)
 
     assert should_send_default_pii() is False
+
+
+def test_set_tags():
+    scope = Scope()
+    scope.set_tags({"tag1": "value1", "tag2": "value2"})
+    event = scope.apply_to_event({}, {})
+
+    assert event["tags"] == {"tag1": "value1", "tag2": "value2"}, "Setting tags failed"
+
+    scope.set_tags({"tag2": "updated", "tag3": "new"})
+    event = scope.apply_to_event({}, {})
+
+    assert event["tags"] == {
+        "tag1": "value1",
+        "tag2": "updated",
+        "tag3": "new",
+    }, "Updating tags failed"
+
+    scope.set_tags({})
+    event = scope.apply_to_event({}, {})
+
+    assert event["tags"] == {
+        "tag1": "value1",
+        "tag2": "updated",
+        "tag3": "new",
+    }, "Updating tags with empty dict changed tags"
```

### Comparing `sentry_sdk-2.0.1/tests/test_scrubber.py` & `sentry_sdk-2.1.0/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_serializer.py` & `sentry_sdk-2.1.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_sessions.py` & `sentry_sdk-2.1.0/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_spotlight.py` & `sentry_sdk-2.1.0/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_transport.py` & `sentry_sdk-2.1.0/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_types.py` & `sentry_sdk-2.1.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.0.1/tests/test_utils.py` & `sentry_sdk-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

