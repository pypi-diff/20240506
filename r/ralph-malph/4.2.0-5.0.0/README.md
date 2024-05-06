# Comparing `tmp/ralph-malph-4.2.0.tar.gz` & `tmp/ralph-malph-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-4.2.0.tar", last modified: Mon Apr  8 15:41:25 2024, max compression
+gzip compressed data, was "ralph-malph-5.0.0.tar", last modified: Mon May  6 08:12:37 2024, max compression
```

## Comparing `ralph-malph-4.2.0.tar` & `ralph-malph-5.0.0.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12817 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6868 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7122 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-08 15:41:25.094102 ralph-malph-4.2.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.050101 ralph-malph-4.2.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1514 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/auth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1948 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5810 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5162 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/oidc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2035 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/auth/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22459 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.054101 ralph-malph-4.2.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.058101 ralph-malph-4.2.0/src/ralph/backends/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11851 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10305 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14074 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8971 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/async_ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26653 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15896 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16196 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14832 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11544 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11101 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2301 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17787 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16547 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/data/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2826 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/loader.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.058101 ralph-malph-4.2.0/src/ralph/backends/lrs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/async_es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2120 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/async_mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7030 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15698 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5557 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/backends/lrs/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26509 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7543 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9412 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3670 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2833 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/bookmark/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/certificate/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2858 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4288 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/certificate/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/cohort/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2351 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/cohort/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3184 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2543 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.062101 ralph-malph-4.2.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1795 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1621 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/enrollment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7554 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1984 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2433 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      950 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4860 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3719 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/notes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6788 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/notes/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.066101 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9797 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8201 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/poll/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/poll/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12749 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/survey/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1728 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/survey/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.070101 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3914 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5549 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/teams_related/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10102 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12455 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3013 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7778 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5250 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.074102 ralph-malph-4.2.0/src/ralph/models/xapi/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/ifi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1479 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2367 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4105 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/base/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/audio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2933 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.078101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/lms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1095 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2182 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4613 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/lms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5807 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8206 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/lms/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9291 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6898 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/video/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.082101 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8052 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2896 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10245 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.086101 ralph-malph-4.2.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12817 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8538 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-08 15:41:25.000000 ralph-malph-4.2.0/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-08 15:41:25.086101 ralph-malph-4.2.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35542 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25068 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5995 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2374 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4823 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-04-08 15:41:23.000000 ralph-malph-4.2.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.016875 ralph-malph-5.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12856 2024-05-06 08:12:37.016875 ralph-malph-5.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6868 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7090 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-06 08:12:37.016875 ralph-malph-5.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.980875 ralph-malph-5.0.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.980875 ralph-malph-5.0.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.984875 ralph-malph-5.0.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1580 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.984875 ralph-malph-5.0.0/src/ralph/api/auth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1948 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/auth/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5845 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/auth/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5178 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/auth/oidc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1899 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/auth/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.984875 ralph-malph-5.0.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23832 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.984875 ralph-malph-5.0.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.984875 ralph-malph-5.0.0/src/ralph/backends/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11863 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/async_es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/async_lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14111 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/async_mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9036 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/async_ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26715 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15976 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16362 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15328 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11598 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11294 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2301 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18096 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15991 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16601 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/data/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2826 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/loader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/backends/lrs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/async_es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2120 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/async_mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4750 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7205 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5172 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15765 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5623 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/backends/lrs/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27061 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9385 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3670 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6675 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3085 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/bookmark/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/certificate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/certificate/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/certificate/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/certificate/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2967 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/certificate/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4288 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/certificate/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/cohort/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/cohort/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/cohort/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/cohort/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/cohort/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2351 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/cohort/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.988875 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2543 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1795 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/enrollment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7566 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1984 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2454 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1117 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4859 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1100 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3737 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.992875 ralph-malph-5.0.0/src/ralph/models/edx/notes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/notes/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/notes/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/notes/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3484 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/notes/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6788 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/notes/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10120 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8201 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      804 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/poll/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/poll/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/poll/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/poll/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/poll/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/poll/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13185 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/survey/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/survey/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/survey/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/survey/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/survey/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1728 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/survey/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:36.996875 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4019 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5549 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/teams_related/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10266 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12455 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7827 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5250 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3114 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/xapi/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1821 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2459 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/ifi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2370 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/base/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.000875 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.004875 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1566 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      952 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/audio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2933 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.004875 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/lms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.004875 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      753 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1109 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1246 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1700 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.004875 ralph-malph-5.0.0/src/ralph/models/xapi/lms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/lms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6080 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/lms/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2392 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/lms/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8206 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/lms/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.004875 ralph-malph-5.0.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/navigation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.008875 ralph-malph-5.0.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9695 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/video/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5462 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/video/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6898 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/video/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.008875 ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8144 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12740 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2896 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10245 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.008875 ralph-malph-5.0.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12856 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8538 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1505 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 08:12:37.008875 ralph-malph-5.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35602 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24968 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4201 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5995 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2374 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4823 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3918 2024-05-06 08:12:36.000000 ralph-malph-5.0.0/tests/test_utils.py
```

### Comparing `ralph-malph-4.2.0/LICENSE.md` & `ralph-malph-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/PKG-INFO` & `ralph-malph-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 4.2.0
+Version: 5.0.0
 Summary: Ralph, the ultimate Learning Record Store (and more!) for your learning analytics.
 Author-email: "Open FUN (France Université Numérique)" <fun.dev@fun-mooc.fr>
 License: MIT License
         
         Copyright (c) 2020-present France Université Numérique
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata<8.0,>=7.0.1
 Requires-Dist: langcodes>=3.2.0
-Requires-Dist: pydantic[dotenv,email]<2.0,>=1.10.0
+Requires-Dist: pydantic[email]<3.0,>=2.5.3
+Requires-Dist: pydantic_settings<3.0,>=2.1.0
 Requires-Dist: rfc3987>=1.3.0
 Provides-Extra: backend-clickhouse
 Requires-Dist: clickhouse-connect[numpy,pandas]<0.6; extra == "backend-clickhouse"
 Requires-Dist: python-dateutil>=2.8.2; extra == "backend-clickhouse"
 Provides-Extra: backend-es
 Requires-Dist: elasticsearch[async]>=8.0.0; extra == "backend-es"
 Provides-Extra: backend-ldp
@@ -77,45 +78,45 @@
 Provides-Extra: cli
 Requires-Dist: bcrypt>=4.0.0; extra == "cli"
 Requires-Dist: click>=8.1.0; extra == "cli"
 Requires-Dist: click-option-group>=0.5.0; extra == "cli"
 Requires-Dist: sentry-sdk[fastapi]>=1.9.0; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: anyio<4.3.1; extra == "dev"
-Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: factory-boy==3.3.0; extra == "dev"
-Requires-Dist: hypothesis<6.92.0; extra == "dev"
 Requires-Dist: logging-gelf==0.0.32; extra == "dev"
 Requires-Dist: mike==2.0.0; extra == "dev"
-Requires-Dist: mkdocs==1.5.3; extra == "dev"
+Requires-Dist: mkdocs==1.6.0; extra == "dev"
 Requires-Dist: mkdocs-click==0.8.1; extra == "dev"
-Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy]==0.24.3; extra == "dev"
-Requires-Dist: moto==5.0.5; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mkdocs-material==9.5.20; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy]==0.25.0; extra == "dev"
+Requires-Dist: moto==5.0.6; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: neoteroi-mkdocs==1.0.5; extra == "dev"
-Requires-Dist: pyfakefs==5.4.0; extra == "dev"
-Requires-Dist: pymdown-extensions==10.7.1; extra == "dev"
+Requires-Dist: polyfactory==2.15.0; extra == "dev"
+Requires-Dist: pyfakefs==5.4.1; extra == "dev"
+Requires-Dist: pymdown-extensions==10.8.1; extra == "dev"
 Requires-Dist: pytest<8.0.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-httpx<0.23.0; extra == "dev"
 Requires-Dist: requests-mock==1.12.1; extra == "dev"
 Requires-Dist: responses==0.24.1; extra == "dev"
-Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: ruff==0.4.2; extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Requires-Dist: types-python-jose==3.3.4.20240106; extra == "dev"
 Requires-Dist: types-requests<2.31.0.20240407; extra == "dev"
 Requires-Dist: types-cachetools==5.3.0.7; extra == "dev"
 Provides-Extra: lrs
 Requires-Dist: bcrypt==4.1.2; extra == "lrs"
-Requires-Dist: fastapi==0.110.1; extra == "lrs"
+Requires-Dist: fastapi==0.110.2; extra == "lrs"
 Requires-Dist: cachetools==5.3.3; extra == "lrs"
 Requires-Dist: httpx<0.25.0; extra == "lrs"
-Requires-Dist: sentry_sdk==1.44.1; extra == "lrs"
+Requires-Dist: sentry_sdk==2.0.1; extra == "lrs"
 Requires-Dist: python-jose==3.3.0; extra == "lrs"
 Requires-Dist: uvicorn[standard]==0.29.0; extra == "lrs"
 Provides-Extra: full
 Requires-Dist: ralph-malph[backends,cli,lrs]; extra == "full"
 
 
 <p align="center">
```

### Comparing `ralph-malph-4.2.0/README.md` & `ralph-malph-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/pyproject.toml` & `ralph-malph-5.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 license = { file = "LICENSE.md" }
 keywords = ["LRS", "Analytics", "xAPI", "Open edX"]
 dependencies = [
     # By default, we only consider core dependencies required to use Ralph as a
     # library (mostly models).
     "importlib-metadata>=7.0.1, <8.0",
     "langcodes>=3.2.0",
-    "pydantic[dotenv,email]>=1.10.0, <2.0",
+    "pydantic[email]>=2.5.3,<3.0",
+    "pydantic_settings>=2.1.0,<3.0",
     "rfc3987>=1.3.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://openfun.github.io/ralph/"
 "Bug Tracker" = "https://github.com/openfun/ralph/issues"
@@ -85,46 +86,46 @@
     "bcrypt>=4.0.0",
     "click>=8.1.0",
     "click-option-group>=0.5.0",
     "sentry-sdk[fastapi]>=1.9.0",
 ]
 dev = [
     "anyio<4.3.1", # unpin until fastapi supports new major version of anyio
-    "black==24.3.0",
+    "black==24.4.2",
     "cryptography==42.0.5",
     "factory-boy==3.3.0",
-    "hypothesis<6.92.0", # pin as hypothesis 6.92.0 observability feature seems broken
     "logging-gelf==0.0.32",
     "mike==2.0.0",
-    "mkdocs==1.5.3",
+    "mkdocs==1.6.0",
     "mkdocs-click==0.8.1",
-    "mkdocs-material==9.5.17",
-    "mkdocstrings[python-legacy]==0.24.3",
-    "moto==5.0.5",
-    "mypy==1.9.0",
+    "mkdocs-material==9.5.20",
+    "mkdocstrings[python-legacy]==0.25.0",
+    "moto==5.0.6",
+    "mypy==1.10.0",
     "neoteroi-mkdocs==1.0.5",
-    "pyfakefs==5.4.0",
-    "pymdown-extensions==10.7.1",
+    "polyfactory==2.15.0",
+    "pyfakefs==5.4.1",
+    "pymdown-extensions==10.8.1",
     "pytest<8.0.0", # pin as pytest-httpx<0.23.0 is not compatible with pytest 8.0.0 
     "pytest-cov==5.0.0",
     "pytest-httpx<0.23.0", # pin as Python 3.8 is no longer supported from release 0.23.0
     "requests-mock==1.12.1",
     "responses==0.24.1",
-    "ruff==0.3.5",
+    "ruff==0.4.2",
     "types-python-dateutil ==2.9.0.20240316",
     "types-python-jose ==3.3.4.20240106",
     "types-requests<2.31.0.20240407",
     "types-cachetools ==5.3.0.7",
 ]
 lrs = [
     "bcrypt==4.1.2",
-    "fastapi==0.110.1",
+    "fastapi==0.110.2",
     "cachetools==5.3.3",
     "httpx<0.25.0", # pin as `pytest-httpx<0.23.0` requires `httpx==0.24.*`
-    "sentry_sdk==1.44.1",
+    "sentry_sdk==2.0.1",
     "python-jose==3.3.0",
     "uvicorn[standard]==0.29.0",
 ]
 full = [
     "ralph-malph[backends,cli,lrs]",
 ]
```

### Comparing `ralph-malph-4.2.0/src/ralph/__main__.py` & `ralph-malph-5.0.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/api/__init__.py` & `ralph-malph-5.0.0/src/ralph/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,8 +47,11 @@
 
 
 @app.get("/whoami")
 async def whoami(
     user: AuthenticatedUser = Depends(get_authenticated_user),
 ) -> Dict[str, Any]:
     """Return the current user's username along with their scopes."""
-    return {"agent": user.agent, "scopes": user.scopes}
+    return {
+        "agent": user.agent.model_dump(mode="json", exclude_none=True),
+        "scopes": user.scopes,
+    }
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/auth/__init__.py` & `ralph-malph-5.0.0/src/ralph/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/api/auth/basic.py` & `ralph-malph-5.0.0/src/ralph/api/auth/basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Basic authentication & authorization related tools for the Ralph API."""
 
 import logging
+import os
 from functools import lru_cache
 from pathlib import Path
 from threading import Lock
 from typing import Any, Iterator, List, Optional
 
 import bcrypt
 from cachetools import TTLCache, cached
 from fastapi import Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
-from pydantic import BaseModel, root_validator
+from pydantic import RootModel, model_validator
 from starlette.authentication import AuthenticationError
 
 from ralph.api.auth.user import AuthenticatedUser
 from ralph.conf import settings
 
 # Unused password used to avoid timing attacks, by comparing passwords supplied
 # with invalid credentials to something innocuous with the same method as if
@@ -36,53 +37,50 @@
         username (str): Consists of the username for a declared user.
     """
 
     hash: str
     username: str
 
 
-class ServerUsersCredentials(BaseModel):
+class ServerUsersCredentials(RootModel[List[UserCredentials]]):
     """Custom root pydantic model.
 
     Describe expected list of all server users credentials as stored in
     the credentials file.
 
     Attributes:
-        __root__ (List): Custom root consisting of the
+        root (List): Custom root consisting of the
                         list of all server users credentials.
     """
 
-    __root__: List[UserCredentials]
-
     def __add__(self, other) -> Any:  # noqa: D105
-        return ServerUsersCredentials.parse_obj(self.__root__ + other.__root__)
+        return ServerUsersCredentials.model_validate(self.root + other.root)
 
     def __getitem__(self, item: int) -> UserCredentials:  # noqa: D105
-        return self.__root__[item]
+        return self.root[item]
 
     def __len__(self) -> int:  # noqa: D105
-        return len(self.__root__)
+        return len(self.root)
 
     def __iter__(self) -> Iterator[UserCredentials]:  # noqa: D105
-        return iter(self.__root__)
+        return iter(self.root)
 
-    @root_validator
-    @classmethod
-    def ensure_unique_username(cls, values: Any) -> Any:
+    @model_validator(mode="after")
+    def ensure_unique_username(self) -> Any:
         """Every username should be unique among registered users."""
-        usernames = [entry.username for entry in values.get("__root__")]
+        usernames = [entry.username for entry in self.root]
         if len(usernames) != len(set(usernames)):
             raise ValueError(
                 "You cannot create multiple credentials with the same username"
             )
-        return values
+        return self
 
 
 @lru_cache()
-def get_stored_credentials(auth_file: Path) -> ServerUsersCredentials:
+def get_stored_credentials(auth_file: os.PathLike) -> ServerUsersCredentials:
     """Helper to read the credentials/scopes file.
 
     Read credentials from JSON file and stored them to avoid reloading them with every
     request.
 
     Args:
         auth_file (Path): Path to the JSON credentials scope file.
@@ -92,15 +90,17 @@
 
     """
     auth_file = Path(auth_file)
     if not auth_file.exists():
         msg = "Credentials file <%s> not found."
         logger.warning(msg, auth_file)
         raise AuthenticationError(msg.format(auth_file))
-    return ServerUsersCredentials.parse_file(auth_file)
+
+    with open(auth_file, encoding=settings.LOCALE_ENCODING) as f:
+        return ServerUsersCredentials.model_validate_json(f.read())
 
 
 @cached(
     TTLCache(maxsize=settings.AUTH_CACHE_MAX_SIZE, ttl=settings.AUTH_CACHE_TTL),
     lock=Lock(),
     key=lambda credentials: (
         (
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/auth/oidc.py` & `ralph-malph-5.0.0/src/ralph/api/auth/oidc.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Optional
 
 import requests
 from fastapi import Depends, HTTPException, status
 from fastapi.security import HTTPBearer, OpenIdConnect
 from jose import ExpiredSignatureError, JWTError, jwt
 from jose.exceptions import JWTClaimsError
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 from typing_extensions import Annotated
 
 from ralph.api.auth.user import AuthenticatedUser, UserScopes
 from ralph.conf import settings
 
 OPENID_CONFIGURATION_PATH = "/.well-known/openid-configuration"
 oauth2_scheme = OpenIdConnect(
@@ -41,22 +41,21 @@
         iat (int): Time at which the JWT was issued.
         scope (str): Scope(s) for resource authorization.
         target (str): Target for storing the statements.
     """
 
     iss: str
     sub: str
-    aud: Optional[str]
+    aud: Optional[str] = None
     exp: int
     iat: int
-    scope: Optional[str]
-    target: Optional[str]
+    scope: Optional[str] = None
+    target: Optional[str] = None
 
-    class Config:  # noqa: D106
-        extra = Extra.ignore
+    model_config = ConfigDict(extra="ignore")
 
 
 @lru_cache()
 def discover_provider(base_url: AnyUrl) -> Dict:
     """Discover the authentication server (or OpenId Provider) configuration."""
     try:
         response = requests.get(f"{base_url}{OPENID_CONFIGURATION_PATH}", timeout=5)
@@ -140,15 +139,15 @@
         logger.error("Unable to decode the ID token: %s", exc)
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Could not validate credentials",
             headers={"WWW-Authenticate": "Bearer"},
         ) from exc
 
-    id_token = IDToken.parse_obj(decoded_token)
+    id_token = IDToken.model_validate(decoded_token)
 
     user = AuthenticatedUser(
         agent={"openid": f"{id_token.iss}/{id_token.sub}"},
         scopes=UserScopes(id_token.scope.split(" ") if id_token.scope else []),
         target=id_token.target,
     )
     return user
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/auth/user.py` & `ralph-malph-5.0.0/src/ralph/api/auth/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Authenticated user for the Ralph API."""
 
-from typing import Dict, FrozenSet, Literal, Optional
+from typing import FrozenSet, Literal, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, RootModel
+
+from ralph.models.xapi.base.agents import BaseXapiAgent
 
 Scope = Literal[
     "statements/write",
     "statements/read/mine",
     "statements/read",
     "state/write",
     "state/read",
@@ -14,15 +16,15 @@
     "profile/write",
     "profile/read",
     "all/read",
     "all",
 ]
 
 
-class UserScopes(FrozenSet[Scope]):
+class UserScopes(RootModel[FrozenSet[Scope]]):
     """Scopes available to users."""
 
     def is_authorized(self, requested_scope: Scope):
         """Check if the requested scope can be accessed based on user scopes."""
         expanded_scopes = {
             "statements/read": {"statements/read/mine", "statements/read"},
             "all/read": {
@@ -43,33 +45,25 @@
                 "profile/write",
                 "all/read",
                 "all",
             },
         }
 
         expanded_user_scopes = set()
-        for scope in self:
+        for scope in self.root:
             expanded_user_scopes.update(expanded_scopes.get(scope, {scope}))
 
         return requested_scope in expanded_user_scopes
 
-    @classmethod
-    def __get_validators__(cls):  # noqa: D105
-        def validate(value: FrozenSet[Scope]):
-            """Transform value to an instance of UserScopes."""
-            return cls(value)
-
-        yield validate
-
 
 class AuthenticatedUser(BaseModel):
     """Pydantic model for user authentication.
 
     Attributes:
         agent (dict): The agent representing the current user.
         scopes (list): The scopes the user has access to.
         target (str or None): The target index or database to store statements into.
     """
 
-    agent: Dict
+    agent: BaseXapiAgent
     scopes: UserScopes
-    target: Optional[str]
+    target: Optional[str] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/forwarding.py` & `ralph-malph-5.0.0/src/ralph/api/forwarding.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     """Forward xAPI statements."""
     for forwarding in get_active_xapi_forwardings():
         transport = AsyncHTTPTransport(retries=forwarding.max_retries)
         async with AsyncClient(transport=transport) as client:
             try:
                 # NB: post or put
                 req = await getattr(client, method)(
-                    forwarding.url,
+                    str(forwarding.url),
                     json=statements,
                     auth=(forwarding.basic_username, forwarding.basic_password),
                     timeout=forwarding.timeout,
                 )
                 req.raise_for_status()
                 msg = "Forwarded %s statements to %s with success."
                 if isinstance(statements, list):
-                    logger.debug(msg, len(statements), forwarding.url)
+                    logger.debug(msg, len(statements), str(forwarding.url))
                 else:
-                    logger.debug(msg, 1, forwarding.url)
+                    logger.debug(msg, 1, str(forwarding.url))
             except (RequestError, HTTPStatusError) as error:
                 logger.error("Failed to forward xAPI statements. %s", error)
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/models.py` & `ralph-malph-5.0.0/src/ralph/api/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Allows to be exactly as lax as we want when it comes to exact object shape and
 validation.
 """
 
 from typing import Optional, Union
 from uuid import UUID
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 
 from ..models.xapi.base.agents import BaseXapiAgent
 from ..models.xapi.base.groups import BaseXapiGroup
 
 
 class ErrorDetail(BaseModel):
     """Pydantic model for errors raised detail.
@@ -26,21 +26,15 @@
 class BaseModelWithLaxConfig(BaseModel):
     """Pydantic base model with lax configuration.
 
     Common base lax model to perform light input validation as
     we receive statements through the API.
     """
 
-    class Config:
-        """Enable extra properties.
-
-        Useful for not having to perform comprehensive validation.
-        """
-
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow", coerce_numbers_to_str=True)
 
 
 class LaxObjectField(BaseModelWithLaxConfig):
     """Pydantic model for lax `object` field.
 
     Lightest definition of an object field compliant to the specification.
     """
@@ -61,10 +55,10 @@
     """Pydantic model for lax statement.
 
     It accepts without validating all fields beyond the bare minimum required to
     qualify an object as an XAPI statement.
     """
 
     actor: Union[BaseXapiAgent, BaseXapiGroup]
-    id: Optional[UUID]
+    id: Optional[UUID] = None
     object: LaxObjectField
     verb: LaxVerbField
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/routers/health.py` & `ralph-malph-5.0.0/src/ralph/api/routers/health.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 
 @router.get("/__heartbeat__", status_code=status.HTTP_200_OK)
 async def heartbeat(response: Response) -> Heartbeat:
     """Application heartbeat.
 
     Return a 200 if all checks are successful.
     """
-    statuses = Heartbeat.construct(
+    statuses = Heartbeat.model_construct(
         database=await await_if_coroutine(BACKEND_CLIENT.status())
     )
     if not statuses.is_alive:
         response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
 
     return statuses
```

### Comparing `ralph-malph-4.2.0/src/ralph/api/routers/statements.py` & `ralph-malph-5.0.0/src/ralph/api/routers/statements.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Query,
     Request,
     Response,
     Security,
     status,
 )
 from fastapi.dependencies.models import Dependant
-from pydantic import parse_obj_as
+from pydantic import TypeAdapter
 from pydantic.types import Json
 from typing_extensions import Annotated
 
 from ralph.api.auth import get_authenticated_user
 from ralph.api.auth.user import AuthenticatedUser
 from ralph.api.forwarding import forward_xapi_statements, get_active_xapi_forwardings
 from ralph.api.models import ErrorDetail, LaxStatement
@@ -94,36 +94,39 @@
 
 
 def _enrich_statement_with_authority(
     statement: dict, current_user: AuthenticatedUser
 ) -> None:
     # authority: Information about whom or what has asserted the statement is true.
     # https://github.com/adlnet/xAPI-Spec/blob/master/xAPI-Data.md#249-authority
-    statement["authority"] = current_user.agent
+    statement["authority"] = current_user.agent.model_dump(
+        exclude_none=True, mode="json"
+    )
 
 
 def _parse_agent_parameters(agent_obj: dict) -> AgentParameters:
     """Parse a dict and return an AgentParameters object to use in queries."""
     # Transform agent to `dict` as FastAPI cannot parse JSON (seen as string)
 
-    agent = parse_obj_as(BaseXapiAgent, agent_obj)
+    adapter = TypeAdapter(BaseXapiAgent)
+    agent = adapter.validate_python(agent_obj)
 
     agent_query_params = {}
     if isinstance(agent, BaseXapiAgentWithMbox):
         agent_query_params["mbox"] = agent.mbox
     elif isinstance(agent, BaseXapiAgentWithMboxSha1Sum):
         agent_query_params["mbox_sha1sum"] = agent.mbox_sha1sum
     elif isinstance(agent, BaseXapiAgentWithOpenId):
         agent_query_params["openid"] = agent.openid
     elif isinstance(agent, BaseXapiAgentWithAccount):
         agent_query_params["account__name"] = agent.account.name
         agent_query_params["account__home_page"] = agent.account.homePage
 
     # Overwrite `agent` field
-    return AgentParameters.construct(**agent_query_params)
+    return AgentParameters.model_construct(**agent_query_params)
 
 
 def strict_query_params(request: Request) -> None:
     """Raise a 400 error when using extra query parameters."""
     dependant: Dependant = request.scope["route"].dependant
     allowed_params = [
         param.alias
@@ -137,154 +140,189 @@
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=f"The following parameter is not allowed: `{requested_param}`",
             )
 
 
 @router.get("")
 @router.get("/")
-async def get(  # noqa: PLR0913
+async def get(  # noqa: PLR0912,PLR0913
     request: Request,
     current_user: Annotated[
         AuthenticatedUser,
         Security(get_authenticated_user, scopes=["statements/read/mine"]),
     ],
     ###
     # Query string parameters defined by the LRS specification
     ###
-    statement_id: Optional[str] = Query(
-        None, description="Id of Statement to fetch", alias="statementId"
-    ),
-    voided_statement_id: Optional[str] = Query(
-        None,
-        description="**Not implemented** Id of voided Statement to fetch",
-        alias="voidedStatementId",
-    ),
-    agent: Optional[Json] = Query(
-        None,
-        description=(
-            "Filter, only return Statements for which the specified "
-            "Agent or Group is the Actor or Object of the Statement"
-        ),
-    ),
-    verb: Optional[str] = Query(
-        None,
-        description="Filter, only return Statements matching the specified Verb id",
-    ),
-    activity: Optional[IRI] = Query(
-        None,
-        description=(
-            "Filter, only return Statements for which the Object "
-            "of the Statement is an Activity with the specified id"
-        ),
-    ),
-    registration: Optional[UUID] = Query(
-        None,
-        description=(
-            "**Not implemented** "
-            "Filter, only return Statements matching the specified registration id"
-        ),
-    ),
-    related_activities: Optional[bool] = Query(
-        False,
-        description=(
-            "**Not implemented** "
-            "Apply the Activity filter broadly. Include Statements for which "
-            "the Object, any of the context Activities, or any of those properties "
-            "in a contained SubStatement match the Activity parameter, "
-            "instead of that parameter's normal behaviour"
-        ),
-    ),
-    related_agents: Optional[bool] = Query(
-        False,
-        description=(
-            "**Not implemented** "
-            "Apply the Agent filter broadly. Include Statements for which "
-            "the Actor, Object, Authority, Instructor, Team, or any of these "
-            "properties in a contained SubStatement match the Agent parameter, "
-            "instead of that parameter's normal behaviour."
-        ),
-    ),
-    since: Optional[datetime] = Query(
-        None,
-        description=(
-            "Only Statements stored since the "
-            "specified Timestamp (exclusive) are returned"
-        ),
-    ),
-    until: Optional[datetime] = Query(
-        None,
-        description=(
-            "Only Statements stored at or "
-            "before the specified Timestamp are returned"
-        ),
-    ),
-    limit: Optional[int] = Query(
-        settings.RUNSERVER_MAX_SEARCH_HITS_COUNT,
-        ge=0,
-        description=(
-            "Maximum number of Statements to return. "
-            "0 indicates return the maximum the server will allow"
-        ),
-    ),
-    format: Optional[Literal["ids", "exact", "canonical"]] = Query(  # noqa: ARG001
-        "exact",
-        description=(
-            "**Not implemented** "
-            'If "ids", only include minimum information necessary in Agent, Activity, '
-            "Verb and Group Objects to identify them. For Anonymous Groups this means "
-            "including the minimum information needed to identify each member. "
-            'If "exact", return Agent, Activity, Verb and Group Objects populated '
-            "exactly as they were when the Statement was received. An LRS requesting "
-            "Statements for the purpose of importing them would use a format of "
-            '"exact" in order to maintain Statement Immutability. '
-            'If "canonical", return Activity Objects and Verbs populated with the '
-            "canonical definition of the Activity Objects and Display of the Verbs "
-            "as determined by the LRS, after applying the language filtering process "
-            "defined below, and return the original Agent and Group Objects "
-            'as in "exact" mode.'
-        ),
-    ),
-    attachments: Optional[bool] = Query(  # noqa: ARG001
-        False,
-        description=(
-            "**Not implemented** "
-            'If "true", the LRS uses the multipart response format and includes '
-            'all attachments as described previously. If "false", the LRS sends '
-            "the prescribed response with Content-Type application/json and "
-            "does not send attachment data."
-        ),
-    ),
-    ascending: Optional[bool] = Query(  # noqa: ARG001
-        False, description='If "true", return results in ascending order of stored time'
-    ),
-    mine: Optional[bool] = Query(
-        False,
-        description=(
-            'If "true", return only the results for which the authority matches the '
-            '"agent" associated to the user that is making the query.'
+    statement_id: Annotated[
+        Optional[str],
+        Query(description="Id of Statement to fetch", alias="statementId"),
+    ] = None,
+    voided_statement_id: Annotated[
+        Optional[str],
+        Query(
+            description="**Not implemented** Id of voided Statement to fetch",
+            alias="voidedStatementId",
+        ),
+    ] = None,
+    agent: Annotated[
+        Optional[Json],
+        Query(
+            description=(
+                "Filter, only return Statements for which the specified "
+                "Agent or Group is the Actor or Object of the Statement"
+            ),
+        ),
+    ] = None,
+    verb: Annotated[
+        Optional[str],
+        Query(
+            description="Filter, only return Statements matching the specified Verb id",
+        ),
+    ] = None,
+    activity: Annotated[
+        Optional[str],
+        Query(
+            description=(
+                "Filter, only return Statements for which the Object "
+                "of the Statement is an Activity with the specified id"
+            ),
+        ),
+    ] = None,
+    registration: Annotated[
+        Optional[UUID],
+        Query(
+            description=(
+                "**Not implemented** "
+                "Filter, only return Statements matching the specified registration id"
+            ),
+        ),
+    ] = None,
+    related_activities: Annotated[
+        Optional[bool],
+        Query(
+            description=(
+                "**Not implemented** "
+                "Apply the Activity filter broadly. Include Statements for which "
+                "the Object, any of the context Activities, or any of those properties "
+                "in a contained SubStatement match the Activity parameter, "
+                "instead of that parameter's normal behaviour"
+            ),
+        ),
+    ] = False,
+    related_agents: Annotated[
+        Optional[bool],
+        Query(
+            description=(
+                "**Not implemented** "
+                "Apply the Agent filter broadly. Include Statements for which "
+                "the Actor, Object, Authority, Instructor, Team, or any of these "
+                "properties in a contained SubStatement match the Agent parameter, "
+                "instead of that parameter's normal behaviour."
+            ),
+        ),
+    ] = False,
+    since: Annotated[
+        Optional[datetime],
+        Query(
+            description=(
+                "Only Statements stored since the "
+                "specified Timestamp (exclusive) are returned"
+            ),
+        ),
+    ] = None,
+    until: Annotated[
+        Optional[datetime],
+        Query(
+            description=(
+                "Only Statements stored at or "
+                "before the specified Timestamp are returned"
+            ),
+        ),
+    ] = None,
+    limit: Annotated[
+        Optional[int],
+        Query(
+            ge=0,
+            description=(
+                "Maximum number of Statements to return. "
+                "0 indicates return the maximum the server will allow"
+            ),
+        ),
+    ] = settings.RUNSERVER_MAX_SEARCH_HITS_COUNT,
+    format: Annotated[  # noqa: ARG001
+        Optional[Literal["ids", "exact", "canonical"]],
+        Query(
+            description=(
+                "**Not implemented** "
+                'If "ids", only include minimum information necessary in Agent, '
+                "Activity, Verb and Group Objects to identify them. For Anonymous "
+                "Groups this means including the minimum information needed to "
+                'identify each member. If "exact", return Agent, Activity, Verb and '
+                "Group Objects populated exactly as they were when the Statement was "
+                "received. An LRS requesting Statements for the purpose of importing "
+                'them would use a format of "exact" in order to maintain Statement '
+                'Immutability. If "canonical", return Activity Objects and Verbs '
+                "populated with the canonical definition of the Activity Objects and "
+                "Display of the Verbs  as determined by the LRS, after applying the "
+                "language filtering process  defined below, and return the original "
+                'Agent and Group Objects as in "exact" mode.'
+            ),
+        ),
+    ] = "exact",
+    attachments: Annotated[  # noqa: ARG001
+        Optional[bool],
+        Query(
+            description=(
+                "**Not implemented** "
+                'If "true", the LRS uses the multipart response format and includes '
+                'all attachments as described previously. If "false", the LRS sends '
+                "the prescribed response with Content-Type application/json and "
+                "does not send attachment data."
+            ),
+        ),
+    ] = False,
+    ascending: Annotated[  # noqa: ARG001
+        Optional[bool],
+        Query(
+            description='If "true", return results in ascending order of stored time'
+        ),
+    ] = False,
+    mine: Annotated[
+        Optional[bool],
+        Query(
+            description=(
+                'If "true", return only the results for which the authority matches '
+                'the "agent" associated to the user that is making the query.'
+            ),
         ),
-    ),
+    ] = False,
     ###
     # Private use query string parameters
     ###
-    search_after: Optional[str] = Query(  # noqa: ARG001
-        None,
-        description=(
-            "Sorting data to allow pagination through large number of search results. "
-            "NB: for internal use, not part of the LRS specification."
-        ),
-    ),
-    pit_id: Optional[str] = Query(  # noqa: ARG001
-        None,
-        description=(
-            "Point-in-time ID to ensure consistency of search requests through "
-            "multiple pages."
-            "NB: for internal use, not part of the LRS specification."
+    search_after: Annotated[  # noqa: ARG001
+        Optional[str],
+        Query(
+            description=(
+                "Sorting data to allow pagination through large number of search "
+                "results."
+                "NB: for internal use, not part of the LRS specification."
+            ),
+        ),
+    ] = None,
+    pit_id: Annotated[  # noqa: ARG001
+        Optional[str],
+        Query(
+            description=(
+                "Point-in-time ID to ensure consistency of search requests through "
+                "multiple pages."
+                "NB: for internal use, not part of the LRS specification."
+            ),
         ),
-    ),
+    ] = None,
     _=Depends(strict_query_params),
 ) -> Dict:
     """Read a single xAPI Statement or multiple xAPI Statements.
 
     LRS Specification:
     https://github.com/adlnet/xAPI-Spec/blob/1.0.3/xAPI-Communication.md#213-get-statements
     """
@@ -330,36 +368,45 @@
     query_params = dict(request.query_params)
 
     # Parse the "agent" parameter (JSON) into multiple string parameters
     if query_params.get("agent") is not None:
         # Overwrite `agent` field
         query_params["agent"] = _parse_agent_parameters(
             json.loads(query_params["agent"])
-        )
+        ).model_dump(mode="json", exclude_none=True)
+
+    # Coerce `verb` and `activity` as IRI
+    if query_params.get("verb"):
+        query_params["verb"] = IRI(query_params["verb"])
+
+    if query_params.get("activity"):
+        query_params["activity"] = IRI(query_params["activity"])
 
     # mine: If using scopes, only restrict users with limited scopes
     if settings.LRS_RESTRICT_BY_SCOPES:
         if not current_user.scopes.is_authorized("statements/read"):
             mine = True
     # mine: If using only authority, always restrict (otherwise, use the default value)
     elif settings.LRS_RESTRICT_BY_AUTHORITY:
         mine = True
 
     # Filter by authority if using `mine`
     if mine:
-        query_params["authority"] = _parse_agent_parameters(current_user.agent)
+        query_params["authority"] = _parse_agent_parameters(
+            current_user.agent.model_dump(mode="json")
+        ).model_dump(mode="json", exclude_none=True)
 
     if "mine" in query_params:
         query_params.pop("mine")
 
     # Query Database
     try:
         query_result = await await_if_coroutine(
             BACKEND_CLIENT.query_statements(
-                params=RalphStatementsQuery.construct(
+                params=RalphStatementsQuery.model_construct(
                     **{**query_params, "limit": limit}
                 ),
                 target=current_user.target,
             )
         )
     except BackendException as error:
         raise HTTPException(
@@ -414,15 +461,15 @@
     _=Depends(strict_query_params),
 ) -> None:
     """Store a single statement as a single member of a set.
 
     LRS Specification:
     https://github.com/adlnet/xAPI-Spec/blob/1.0.3/xAPI-Communication.md#211-put-statements
     """
-    statement_as_dict = statement.dict(exclude_unset=True)
+    statement_as_dict = statement.model_dump(exclude_unset=True, mode="json")
     statement_id = str(statement_id)
 
     statement_as_dict.update(id=str(statement_as_dict.get("id", statement_id)))
     if statement_id != statement_as_dict["id"]:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail="xAPI statement id does not match given statementId",
@@ -512,15 +559,17 @@
     # As we accept both a single statement as a dict, and multiple statements as a list,
     # we need to normalize the data into a list in all cases before we can process it.
     if not isinstance(statements, list):
         statements = [statements]
 
     # Enrich statements before forwarding
     statements_dict = {}
-    for statement in (x.dict(exclude_unset=True) for x in statements):
+    for statement in (
+        x.model_dump(exclude_unset=True, mode="json") for x in statements
+    ):
         _enrich_statement_with_id(statement)
         # Requests with duplicate statement IDs are considered invalid
         if statement["id"] in statements_dict:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail="Duplicate statement IDs in the list of statements",
             )
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/async_es.py` & `ralph-malph-5.0.0/src/ralph/backends/data/async_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._client = None
 
     @property
     def client(self) -> AsyncElasticsearch:
         """Create an AsyncElasticsearch client if it doesn't exist."""
         if not self._client:
             self._client = AsyncElasticsearch(
-                self.settings.HOSTS, **self.settings.CLIENT_OPTIONS.dict()
+                self.settings.HOSTS, **self.settings.CLIENT_OPTIONS.model_dump()
             )
         return self._client
 
     async def status(self) -> DataBackendStatus:
         """Check Elasticsearch cluster connection and status."""
         try:
             await self.client.info()
@@ -175,15 +175,15 @@
                 )["id"]
             except (ApiError, TransportError, ValueError) as error:
                 msg = "Failed to open Elasticsearch point in time: %s"
                 logger.error(msg, error)
                 raise BackendException(msg % error) from error
 
         limit = query.size
-        kwargs = query.dict()
+        kwargs = query.model_dump()
         count = chunk_size
         # The first condition is set to comprise either limit as None
         # (when the backend query does not have `size` parameter),
         # or limit with a positive value.
         while limit != 0 and chunk_size == count:
             kwargs["size"] = limit if limit and limit < chunk_size else chunk_size
             try:
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/async_lrs.py` & `ralph-malph-5.0.0/src/ralph/backends/data/async_lrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from io import IOBase
 from typing import AsyncIterator, Iterable, Optional, Union
 from urllib.parse import ParseResult, parse_qs, urljoin, urlparse
 
 from httpx import AsyncClient, HTTPError, HTTPStatusError, RequestError
-from pydantic import AnyHttpUrl, PositiveInt, parse_obj_as
+from pydantic import AnyHttpUrl, PositiveInt, TypeAdapter
 
 from ralph.backends.data.base import (
     AsyncWritable,
     BaseAsyncDataBackend,
     BaseOperationType,
     DataBackendStatus,
 )
@@ -40,29 +40,29 @@
         """Instantiate the LRS HTTP (basic auth) backend client.
 
         Args:
             settings (LRSDataBackendSettings or None): The LRS data backend settings.
                 If `settings` is `None`, a default settings instance is used instead.
         """
         super().__init__(settings)
-        self.base_url = parse_obj_as(AnyHttpUrl, self.settings.BASE_URL)
+        self.base_url = TypeAdapter(AnyHttpUrl).validate_python(self.settings.BASE_URL)
         self.auth = (self.settings.USERNAME, self.settings.PASSWORD)
         self._client = None
 
     @property
     def client(self) -> AsyncClient:
         """Create a `httpx.AsyncClient` if it doesn't exist."""
         if not self._client:
-            headers = self.settings.HEADERS.dict(by_alias=True)
+            headers = self.settings.HEADERS.model_dump(by_alias=True)
             self._client = AsyncClient(auth=self.auth, headers=headers)
         return self._client
 
     async def status(self) -> DataBackendStatus:
         """HTTP backend check for server status."""
-        status_url = urljoin(self.base_url, self.settings.STATUS_ENDPOINT)
+        status_url = urljoin(str(self.base_url), self.settings.STATUS_ENDPOINT)
         try:
             response = await self.client.get(status_url)
             response.raise_for_status()
         except RequestError:
             logger.error("Unable to request the server")
             return DataBackendStatus.AWAY
         except HTTPStatusError:
@@ -134,25 +134,25 @@
                 "parameter value."
             )
 
         query.limit = chunk_size
 
         # Create request URL
         target = ParseResult(
-            scheme=urlparse(self.base_url).scheme,
-            netloc=urlparse(self.base_url).netloc,
+            scheme=self.base_url.scheme,
+            netloc=urlparse(str(self.base_url)).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
         statements = self._fetch_statements(
             target=target,
-            query_params=query.dict(exclude_none=True, exclude_unset=True),
+            query_params=query.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         # Iterate through results
         try:
             async for statement in statements:
                 yield statement
         except HTTPError as error:
@@ -200,16 +200,16 @@
         operation_type: BaseOperationType,  # noqa: ARG002
     ) -> int:
         """Method called by `self.write` writing dictionaries. See `self.write`."""
         if not target:
             target = self.settings.STATEMENTS_ENDPOINT
 
         target = ParseResult(
-            scheme=urlparse(self.base_url).scheme,
-            netloc=urlparse(self.base_url).netloc,
+            scheme=self.base_url.scheme,
+            netloc=urlparse(str(self.base_url)).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
         logger.debug(
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/async_mongo.py` & `ralph-malph-5.0.0/src/ralph/backends/data/async_mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,17 @@
     def __init__(self, settings: Optional[Settings] = None):
         """Instantiate the asynchronous MongoDB client.
 
         Args:
             settings (MongoDataBackendSettings or None): The data backend settings.
         """
         super().__init__(settings)
+        host = str(self.settings.CONNECTION_URI)
         self.client = AsyncIOMotorClient(
-            self.settings.CONNECTION_URI, **self.settings.CLIENT_OPTIONS.dict()
+            host, **self.settings.CLIENT_OPTIONS.model_dump()
         )
         self.database = self.client[self.settings.DEFAULT_DATABASE]
         self.collection = self.database[self.settings.DEFAULT_COLLECTION]
 
     async def status(self) -> DataBackendStatus:
         """Check the MongoDB connection status.
 
@@ -171,15 +172,15 @@
         self,
         query: MongoQuery,
         target: Optional[str],
         chunk_size: int,
         ignore_errors: bool,  # noqa: ARG002
     ) -> AsyncIterator[dict]:
         """Method called by `self.read` yielding dictionaries. See `self.read`."""
-        kwargs = query.dict(exclude_unset=True)
+        kwargs = query.model_dump(exclude_unset=True)
         collection = self._get_target_collection(target)
         try:
             async for document in collection.find(batch_size=chunk_size, **kwargs):
                 document.update({"_id": str(document.get("_id"))})
                 yield document
         except (PyMongoError, IndexError, TypeError, ValueError) as error:
             msg = "Failed to execute MongoDB query: %s"
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/async_ws.py` & `ralph-malph-5.0.0/src/ralph/backends/data/async_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Websocket stream backend for Ralph."""
 
 import logging
 from typing import AsyncIterator, Optional, Union
 
 import websockets
 from pydantic import AnyUrl, PositiveInt
+from pydantic_settings import SettingsConfigDict
 from websockets.http import USER_AGENT
 
 from ralph.backends.data.base import (
     BaseAsyncDataBackend,
     BaseDataBackendSettings,
     DataBackendStatus,
 )
-from ralph.conf import BaseSettingsConfig, ClientOptions
+from ralph.conf import BASE_SETTINGS_CONFIG, ClientOptions
 from ralph.exceptions import BackendException
 
 logger = logging.getLogger(__name__)
 
 
 class WSClientOptions(ClientOptions):
     """Client options for `websockets.connection`.
@@ -64,18 +65,18 @@
 
     Attributes:
         CLIENT_OPTIONS (dict): A dictionary of valid options for the websocket client
             connection. See `WSClientOptions`.
         URI (str): The URI to connect to.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__WS__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__WS__"),
+    }
 
     CLIENT_OPTIONS: WSClientOptions = WSClientOptions()
     URI: AnyUrl
 
 
 class AsyncWSDataBackend(BaseAsyncDataBackend[WSDataBackendSettings, str]):
     """Websocket stream backend."""
@@ -93,15 +94,15 @@
         self._client = None
 
     async def client(self) -> websockets.WebSocketClientProtocol:
         """Create a websocket client connected to `settings.URI` if it doesn't exist."""
         if not self._client:
             try:
                 self._client = await websockets.connect(
-                    self.settings.URI, **self.settings.CLIENT_OPTIONS.dict()
+                    str(self.settings.URI), **self.settings.CLIENT_OPTIONS.model_dump()
                 )
             except (websockets.WebSocketException, OSError, TimeoutError) as error:
                 msg = "Failed open websocket connection for %s: %s"
                 logger.error(msg, self.settings.URI, error)
                 raise BackendException(msg % (self.settings.URI, error)) from error
         return self._client
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/base.py` & `ralph-malph-5.0.0/src/ralph/backends/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 
-from pydantic import BaseModel, BaseSettings, PositiveInt, ValidationError
+from pydantic import BaseModel, PositiveInt, ValidationError
+from pydantic_settings import BaseSettings, SettingsConfigDict
 from typing_extensions import Self, get_original_bases
 
-from ralph.conf import BaseSettingsConfig, core_settings
+from ralph.conf import BASE_SETTINGS_CONFIG, core_settings
 from ralph.exceptions import BackendParameterException
 from ralph.utils import (
     async_parse_dict_to_bytes,
     async_parse_iterable_to_dict,
     gather_with_limited_concurrency,
     iter_by_batch,
     parse_dict_to_bytes,
@@ -38,33 +39,34 @@
 
 logger = logging.getLogger(__name__)
 
 
 class BaseDataBackendSettings(BaseSettings):
     """Data backend default configuration."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__"
-        env_file = ".env"
-        env_file_encoding = core_settings.LOCALE_ENCODING
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(
+            env_prefix="RALPH_BACKENDS__DATA__",
+            env_file=".env",
+            env_file_encoding=core_settings.LOCALE_ENCODING,
+        ),
+    }
 
     LOCALE_ENCODING: str = "utf8"
     READ_CHUNK_SIZE: int = 500
     WRITE_CHUNK_SIZE: int = 500
 
 
 class BaseQuery(BaseModel):
     """Base query model."""
 
-    class Config:
-        """Base query model configuration."""
-
-        extra = "forbid"
+    model_config = SettingsConfigDict(
+        extra="forbid",
+    )
 
     @classmethod
     def from_string(cls, query: str) -> Self:
         """Return an instance of BaseQuery from a string."""
         try:
             return cls.parse_raw(query)
         except ValidationError as error:
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/clickhouse.py` & `ralph-malph-5.0.0/src/ralph/backends/data/clickhouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 )
 from uuid import UUID, uuid4
 
 import clickhouse_connect
 from clickhouse_connect.driver.client import Client
 from clickhouse_connect.driver.exceptions import ClickHouseError
 from pydantic import BaseModel, PositiveInt, ValidationError
+from pydantic_settings import SettingsConfigDict
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     BaseQuery,
     DataBackendStatus,
     Listable,
     Writable,
 )
-from ralph.conf import BaseSettingsConfig, ClientOptions
+from ralph.conf import BASE_SETTINGS_CONFIG, ClientOptions
 from ralph.exceptions import BackendException
 from ralph.utils import iter_by_batch, parse_iterable_to_dict
 
 logger = logging.getLogger(__name__)
 
 
 class ClickHouseInsert(BaseModel):
@@ -73,18 +74,18 @@
         CLIENT_OPTIONS (ClickHouseClientOptions): A dictionary of valid options for the
             ClickHouse client connection.
         LOCALE_ENCODING (str): The locale encoding to use when none is provided.
         READ_CHUNK_SIZE (int): The default chunk size for reading.
         WRITE_CHUNK_SIZE (int): The default chunk size for writing.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__CLICKHOUSE__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__CLICKHOUSE__"),
+    }
 
     HOST: str = "localhost"
     PORT: int = 8123
     DATABASE: str = "xapi"
     EVENT_TABLE_NAME: str = "xapi_events_all"
     USERNAME: Optional[str] = None
     PASSWORD: Optional[str] = None
@@ -101,19 +102,19 @@
         limit (int): Maximum number of rows to return.
         sort (str): Order by expression determining the sorting direction.
         column_oriented (bool): Whether to return the results as a sequence of columns
             rather than a sequence of rows.
     """
 
     select: Union[str, List[str]] = "event"
-    where: Union[str, List[str], None]
-    parameters: Union[Dict, None]
-    limit: Union[int, None]
-    sort: Union[str, None]
-    column_oriented: Union[bool, None] = False
+    where: Optional[Union[str, List[str]]] = None
+    parameters: Optional[Dict] = None
+    limit: Optional[int] = None
+    sort: Optional[str] = None
+    column_oriented: Optional[bool] = False
 
 
 Settings = TypeVar("Settings", bound=ClickHouseDataBackendSettings)
 
 
 class ClickHouseDataBackend(
     BaseDataBackend[Settings, ClickHouseQuery],
@@ -154,15 +155,15 @@
         if not self._client:
             self._client = clickhouse_connect.get_client(
                 host=self.settings.HOST,
                 port=self.settings.PORT,
                 database=self.database,
                 username=self.settings.USERNAME,
                 password=self.settings.PASSWORD,
-                settings=self.settings.CLIENT_OPTIONS.dict(),
+                settings=self.settings.CLIENT_OPTIONS.model_dump(),
             )
         return self._client
 
     def status(self) -> DataBackendStatus:
         """Check ClickHouse connection status.
 
         Return:
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/es.py` & `ralph-malph-5.0.0/src/ralph/backends/data/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from io import IOBase
 from pathlib import Path
 from typing import Iterable, Iterator, List, Literal, Optional, TypeVar, Union
 
 from elasticsearch import ApiError, Elasticsearch, TransportError
 from elasticsearch.helpers import BulkIndexError, streaming_bulk
 from pydantic import BaseModel, PositiveInt, ValidationError
+from pydantic_settings import SettingsConfigDict
 from typing_extensions import Self
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     BaseQuery,
     DataBackendStatus,
     Listable,
     Writable,
 )
-from ralph.conf import BaseSettingsConfig, ClientOptions, CommaSeparatedTuple
+from ralph.conf import BASE_SETTINGS_CONFIG, ClientOptions, CommaSeparatedTuple
 from ralph.exceptions import BackendException
 
 logger = logging.getLogger(__name__)
 
 
 class ESClientOptions(ClientOptions):
     """Elasticsearch additional client options."""
@@ -48,38 +49,42 @@
             keep a point in time alive.
         READ_CHUNK_SIZE (int): The default chunk size for reading batches of documents.
         REFRESH_AFTER_WRITE (str or bool): Whether the Elasticsearch index should be
             refreshed after the write operation.
         WRITE_CHUNK_SIZE (int): The default chunk size for writing batches of documents.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__ES__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__ES__"),
+    }
 
     ALLOW_YELLOW_STATUS: bool = False
     CLIENT_OPTIONS: ESClientOptions = ESClientOptions()
     DEFAULT_INDEX: str = "statements"
-    HOSTS: CommaSeparatedTuple = ("http://localhost:9200",)
+    HOSTS: CommaSeparatedTuple = (
+        "http://localhost:9200"  # CommaSeparatedTuple("http://localhost:9200")
+    )
     POINT_IN_TIME_KEEP_ALIVE: str = "1m"
-    REFRESH_AFTER_WRITE: Union[Literal["false", "true", "wait_for"], bool, str, None]
+    REFRESH_AFTER_WRITE: Optional[
+        Union[Literal["false", "true", "wait_for"], bool, str]
+    ] = None
 
 
 class ESQueryPit(BaseModel):
     """Elasticsearch point in time (pit) query configuration.
 
     Attributes:
         id (str): Context identifier of the Elasticsearch point in time.
         keep_alive (str): The duration for which Elasticsearch should keep the point in
             time alive.
     """
 
-    id: Union[str, None]
-    keep_alive: Union[str, None]
+    id: Union[str, None] = None
+    keep_alive: Union[str, None] = None
 
 
 class ESQuery(BaseQuery):
     """Elasticsearch query model.
 
     Attributes:
         q (str): The Elastisearch query in the Lucene query string syntax.
@@ -138,15 +143,15 @@
         self._client = None
 
     @property
     def client(self) -> Elasticsearch:
         """Create an Elasticsearch client if it doesn't exist."""
         if not self._client:
             self._client = Elasticsearch(
-                self.settings.HOSTS, **self.settings.CLIENT_OPTIONS.dict()
+                self.settings.HOSTS, **self.settings.CLIENT_OPTIONS.model_dump()
             )
         return self._client
 
     def status(self) -> DataBackendStatus:
         """Check Elasticsearch cluster connection and status."""
         try:
             self.client.info()
@@ -258,15 +263,15 @@
                 )["id"]
             except (ApiError, TransportError, ValueError) as error:
                 msg = "Failed to open Elasticsearch point in time: %s"
                 logger.error(msg, error)
                 raise BackendException(msg % error) from error
 
         limit = query.size
-        kwargs = query.dict()
+        kwargs = query.model_dump()
         count = chunk_size
         # The first condition is set to comprise either limit as None
         # (when the backend query does not have `size` parameter),
         # or limit with a positive value.
         while limit != 0 and chunk_size == count:
             kwargs["size"] = limit if limit and limit < chunk_size else chunk_size
             try:
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/fs.py` & `ralph-malph-5.0.0/src/ralph/backends/data/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import os
 from datetime import datetime, timezone
 from io import BufferedReader, IOBase
 from pathlib import Path
 from typing import Iterable, Iterator, Optional, Tuple, TypeVar, Union
 from uuid import uuid4
 
-from pydantic import PositiveInt
+from pydantic import PositiveInt, model_validator
+from pydantic_settings import SettingsConfigDict
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     DataBackendStatus,
     Listable,
     Writable,
 )
 from ralph.backends.data.mixins import HistoryMixin
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 from ralph.utils import now, parse_iterable_to_dict
 
 logger = logging.getLogger(__name__)
 
 
 class FSDataBackendSettings(BaseDataBackendSettings):
@@ -35,24 +36,35 @@
         DEFAULT_QUERY_STRING (str): The default query string to match files for the read
             operation.
         LOCALE_ENCODING (str): The encoding used for writing dictionaries to files.
         READ_CHUNK_SIZE (int): The default chunk size for reading files.
         WRITE_CHUNK_SIZE (int): The default chunk size for writing files.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__FS__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__FS__"),
+    }
 
     DEFAULT_DIRECTORY_PATH: Path = Path(".")
     DEFAULT_QUERY_STRING: str = "*"
     READ_CHUNK_SIZE: int = 4096
     WRITE_CHUNK_SIZE: int = 4096
 
+    @model_validator(mode="before")
+    @classmethod
+    def validate_default_directory_path(cls, values):
+        """Coerce DEFAULT_DIRECTORY_PATH to `Path`."""
+        if "DEFAULT_DIRECTORY_PATH" in values:
+            if isinstance(values["DEFAULT_DIRECTORY_PATH"], str):
+                values["DEFAULT_DIRECTORY_PATH"] = Path(
+                    values["DEFAULT_DIRECTORY_PATH"]
+                )
+        return values
+
 
 Settings = TypeVar("Settings", bound=FSDataBackendSettings)
 
 
 class FSDataBackend(
     BaseDataBackend[Settings, str],
     Writable,
@@ -133,15 +145,14 @@
         if new:
             paths -= set(map(Path, self.get_command_history(self.name, "read")))
             logger.debug("New files: %d", len(paths))
 
         if not details:
             for path in paths:
                 yield str(path)
-
             return
 
         for path in paths:
             stats = path.stat()
             modified_at = datetime.fromtimestamp(int(stats.st_mtime), tz=timezone.utc)
             yield {
                 "path": str(path),
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/ldp.py` & `ralph-malph-5.0.0/src/ralph/backends/data/ldp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import logging
 from typing import Iterator, Literal, Optional, Union
 
 import ovh
 import requests
 from pydantic import PositiveInt
+from pydantic_settings import SettingsConfigDict
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     DataBackendStatus,
     Listable,
 )
 from ralph.backends.data.mixins import HistoryMixin
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 from ralph.utils import now
 
 logger = logging.getLogger(__name__)
 
 
 class LDPDataBackendSettings(BaseDataBackendSettings):
@@ -31,18 +32,18 @@
         DEFAULT_STREAM_ID (str):  The default stream identifier to query.
         ENDPOINT (str): The OVH API endpoint.
         READ_CHUNK_SIZE (str): The default chunk size for reading archives.
         REQUEST_TIMEOUT (int): HTTP request timeout in seconds.
         SERVICE_NAME (str): The default LDP account name.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__LDP__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__LDP__"),
+    }
 
     APPLICATION_KEY: Optional[str] = None
     APPLICATION_SECRET: Optional[str] = None
     CONSUMER_KEY: Optional[str] = None
     DEFAULT_STREAM_ID: Optional[str] = None
     ENDPOINT: Literal[
         "ovh-eu",
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/lrs.py` & `ralph-malph-5.0.0/src/ralph/backends/data/lrs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,46 @@
 
 import logging
 from io import IOBase
 from typing import Iterable, Iterator, List, Optional, Union
 from urllib.parse import ParseResult, parse_qs, urljoin, urlparse
 
 from httpx import Client, HTTPError, HTTPStatusError, RequestError
-from pydantic import AnyHttpUrl, BaseModel, Field, PositiveInt, parse_obj_as
+from pydantic import (
+    AnyHttpUrl,
+    BaseModel,
+    Field,
+    PositiveInt,
+    TypeAdapter,
+)
+from pydantic_settings import SettingsConfigDict
+from typing_extensions import Annotated
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     DataBackendStatus,
     Writable,
 )
 from ralph.backends.lrs.base import LRSStatementsQuery
-from ralph.conf import BaseSettingsConfig, HeadersParameters
+from ralph.conf import BASE_SETTINGS_CONFIG, HeadersParameters
 from ralph.exceptions import BackendException
 from ralph.utils import iter_by_batch
 
 logger = logging.getLogger(__name__)
 
 
 class LRSHeaders(HeadersParameters):
     """Pydantic model for LRS headers."""
 
-    X_EXPERIENCE_API_VERSION: str = Field("1.0.3", alias="X-Experience-API-Version")
-    CONTENT_TYPE: str = Field("application/json", alias="content-type")
+    X_EXPERIENCE_API_VERSION: Annotated[
+        str, Field(alias="X-Experience-API-Version")
+    ] = "1.0.3"
+    CONTENT_TYPE: Annotated[str, Field(alias="content-type")] = "application/json"
 
 
 class LRSDataBackendSettings(BaseDataBackendSettings):
     """LRS data backend default configuration.
 
     Attributes:
         BASE_URL (AnyHttpUrl): LRS server URL.
@@ -41,32 +51,32 @@
         LOCALE_ENCODING (str): The encoding used for reading statements.
         READ_CHUNK_SIZE (int): The default chunk size for reading statements.
         STATUS_ENDPOINT (str): Endpoint used to check server status.
         STATEMENTS_ENDPOINT (str): Default endpoint for LRS statements resource.
         WRITE_CHUNK_SIZE (int): The default chunk size for writing statements.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__LRS__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__LRS__"),
+    }
 
-    BASE_URL: AnyHttpUrl = Field("http://0.0.0.0:8100")
+    BASE_URL: Annotated[AnyHttpUrl, Field("http://0.0.0.0:8100")]
     USERNAME: str = "ralph"
     PASSWORD: str = "secret"
     HEADERS: LRSHeaders = LRSHeaders()
     STATUS_ENDPOINT: str = "/__heartbeat__"
     STATEMENTS_ENDPOINT: str = "/xAPI/statements"
 
 
 class StatementResponse(BaseModel):
     """Pydantic model for `get` statements response."""
 
     statements: Union[List[dict], dict]
-    more: Optional[str]
+    more: Optional[str] = None
 
 
 class LRSDataBackend(
     BaseDataBackend[LRSDataBackendSettings, LRSStatementsQuery], Writable
 ):
     """LRS data backend."""
 
@@ -82,29 +92,29 @@
         """Instantiate the LRS HTTP (basic auth) backend client.
 
         Args:
             settings (LRSDataBackendSettings or None): The LRS data backend settings.
                 If `settings` is `None`, a default settings instance is used instead.
         """
         super().__init__(settings)
-        self.base_url = parse_obj_as(AnyHttpUrl, self.settings.BASE_URL)
+        self.base_url = TypeAdapter(AnyHttpUrl).validate_python(self.settings.BASE_URL)
         self.auth = (self.settings.USERNAME, self.settings.PASSWORD)
         self._client = None
 
     @property
     def client(self) -> Client:
         """Create a `httpx.Client` if it doesn't exist."""
         if not self._client:
-            headers = self.settings.HEADERS.dict(by_alias=True)
+            headers = self.settings.HEADERS.model_dump(by_alias=True)
             self._client = Client(auth=self.auth, headers=headers)
         return self._client
 
     def status(self) -> DataBackendStatus:
         """HTTP backend check for server status."""
-        status_url = urljoin(self.base_url, self.settings.STATUS_ENDPOINT)
+        status_url = urljoin(str(self.base_url), self.settings.STATUS_ENDPOINT)
         try:
             response = self.client.get(status_url)
             response.raise_for_status()
         except RequestError:
             logger.error("Unable to request the server")
             return DataBackendStatus.AWAY
         except HTTPStatusError:
@@ -165,25 +175,25 @@
                 "parameter value."
             )
 
         query.limit = chunk_size
 
         # Create request URL
         target = ParseResult(
-            scheme=urlparse(self.base_url).scheme,
-            netloc=urlparse(self.base_url).netloc,
+            scheme=self.base_url.scheme,
+            netloc=urlparse(str(self.base_url)).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
         statements = self._fetch_statements(
             target=target,
-            query_params=query.dict(exclude_none=True, exclude_unset=True),
+            query_params=query.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         # Iterate through results
         try:
             for statement in statements:
                 yield statement
         except HTTPError as error:
@@ -226,16 +236,16 @@
         operation_type: BaseOperationType,  # noqa: ARG002
     ) -> int:
         """Method called by `self.write` writing dictionaries. See `self.write`."""
         if not target:
             target = self.settings.STATEMENTS_ENDPOINT
 
         target = ParseResult(
-            scheme=urlparse(self.base_url).scheme,
-            netloc=urlparse(self.base_url).netloc,
+            scheme=self.base_url.scheme,
+            netloc=urlparse(str(self.base_url)).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
         logger.debug(
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/mixins.py` & `ralph-malph-5.0.0/src/ralph/backends/data/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/mongo.py` & `ralph-malph-5.0.0/src/ralph/backends/data/mongo.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,35 +8,37 @@
 from io import IOBase
 from typing import Generator, Iterable, Iterator, List, Optional, Tuple, TypeVar, Union
 from uuid import uuid4
 
 from bson.errors import BSONError
 from bson.objectid import ObjectId
 from dateutil.parser import isoparse
-from pydantic import MongoDsn, PositiveInt, constr
+from pydantic import MongoDsn, PositiveInt, StringConstraints
+from pydantic_settings import SettingsConfigDict
 from pymongo import MongoClient, ReplaceOne
 from pymongo.collection import Collection
 from pymongo.errors import (
     BulkWriteError,
     ConnectionFailure,
     InvalidName,
     InvalidOperation,
     PyMongoError,
 )
+from typing_extensions import Annotated
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     BaseQuery,
     DataBackendStatus,
     Listable,
     Writable,
 )
-from ralph.conf import BaseSettingsConfig, ClientOptions
+from ralph.conf import BASE_SETTINGS_CONFIG, ClientOptions
 from ralph.exceptions import BackendException, BackendParameterException
 from ralph.utils import iter_by_batch
 
 logger = logging.getLogger(__name__)
 
 
 class MongoClientOptions(ClientOptions):
@@ -55,24 +57,29 @@
         DEFAULT_COLLECTION (str): The MongoDB database collection to get objects from.
         CLIENT_OPTIONS (MongoClientOptions): A dictionary of MongoDB client options.
         LOCALE_ENCODING (str): The locale encoding to use when none is provided.
         READ_CHUNK_SIZE (int): The default chunk size for reading batches of documents.
         WRITE_CHUNK_SIZE (int): The default chunk size for writing batches of documents.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__MONGO__"
-
-    CONNECTION_URI: MongoDsn = MongoDsn("mongodb://localhost:27017/", scheme="mongodb")
-    DEFAULT_DATABASE: constr(regex=r"^[^\s.$/\\\"\x00]+$") = "statements"
-    DEFAULT_COLLECTION: constr(regex=r"^(?!.*\.\.)[^.$\x00]+(?:\.[^.$\x00]+)*$") = (
-        "marsha"
-    )
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(
+            env_prefix="RALPH_BACKENDS__DATA__MONGO__", regex_engine="python-re"
+        ),
+    }  # We specify regex_engine as some regex are no longer supported in Pydantic V2
+
+    CONNECTION_URI: MongoDsn = MongoDsn("mongodb://localhost:27017/")
+    DEFAULT_DATABASE: Annotated[
+        str, StringConstraints(pattern=r"^[^\s.$/\\\"\x00]+$")
+    ] = "statements"
+    DEFAULT_COLLECTION: Annotated[
+        str,
+        StringConstraints(pattern=r"^(?!.*\.\.)[^.$\x00]+(?:\.[^.$\x00]+)*$"),
+    ] = "marsha"
     CLIENT_OPTIONS: MongoClientOptions = MongoClientOptions()
 
 
 class MongoQuery(BaseQuery):
     """MongoDB query model.
 
     Attributes:
@@ -101,17 +108,16 @@
         """Instantiate the MongoDB client.
 
         Args:
             settings (MongoDataBackendSettings or None): The data backend settings.
                 If `settings` is `None`, a default settings instance is used instead.
         """
         super().__init__(settings)
-        self.client = MongoClient(
-            self.settings.CONNECTION_URI, **self.settings.CLIENT_OPTIONS.dict()
-        )
+        host = str(self.settings.CONNECTION_URI)
+        self.client = MongoClient(host, **self.settings.CLIENT_OPTIONS.model_dump())
         self.database = self.client[self.settings.DEFAULT_DATABASE]
         self.collection = self.database[self.settings.DEFAULT_COLLECTION]
 
     def status(self) -> DataBackendStatus:
         """Check the MongoDB connection status.
 
         Return:
@@ -212,15 +218,15 @@
         self,
         query: MongoQuery,
         target: Optional[str],
         chunk_size: int,
         ignore_errors: bool,  # noqa: ARG002
     ) -> Iterator[dict]:
         """Method called by `self.read` yielding dictionaries. See `self.read`."""
-        kwargs = query.dict(exclude_unset=True)
+        kwargs = query.model_dump(exclude_unset=True)
         collection = self._get_target_collection(target)
         try:
             documents = collection.find(batch_size=chunk_size, **kwargs)
             yield from (d.update({"_id": str(d.get("_id"))}) or d for d in documents)
         except (PyMongoError, IndexError, TypeError, ValueError) as error:
             msg = "Failed to execute MongoDB query: %s"
             logger.error(msg, error)
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/s3.py` & `ralph-malph-5.0.0/src/ralph/backends/data/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,27 @@
     ClientError,
     EndpointConnectionError,
     ParamValidationError,
     ReadTimeoutError,
     ResponseStreamingError,
 )
 from pydantic import PositiveInt
+from pydantic_settings import SettingsConfigDict
 from requests_toolbelt import StreamingIterator
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     DataBackendStatus,
     Listable,
     Writable,
 )
 from ralph.backends.data.mixins import HistoryMixin
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 from ralph.utils import now, parse_iterable_to_dict
 
 logger = logging.getLogger(__name__)
 
 
 class S3DataBackendSettings(BaseDataBackendSettings):
@@ -45,18 +46,18 @@
         DEFAULT_REGION (str): The default region used in instantiating the client.
         DEFAULT_BUCKET_NAME (str): The default bucket name targeted.
         LOCALE_ENCODING (str): The encoding used for writing dictionaries to objects.
         READ_CHUNK_SIZE (str): The default chunk size for reading objects.
         WRITE_CHUNK_SIZE (str): The default chunk size for writing objects.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__S3__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__S3__"),
+    }
 
     ACCESS_KEY_ID: Optional[str] = None
     SECRET_ACCESS_KEY: Optional[str] = None
     SESSION_TOKEN: Optional[str] = None
     ENDPOINT_URL: Optional[str] = None
     DEFAULT_REGION: Optional[str] = None
     DEFAULT_BUCKET_NAME: Optional[str] = None
@@ -211,15 +212,15 @@
             raise BackendException(msg % (query)) from err
 
         # Archive fetched, add a new entry to the history.
         self.append_to_history(
             {
                 "backend": self.name,
                 "action": "read",
-                "id": target + "/" + query,
+                "id": target.rstrip("/") + "/" + query,
                 "size": response["ContentLength"],
                 "timestamp": now(),
             }
         )
 
     def _read_dicts(
         self,
@@ -240,15 +241,15 @@
             raise BackendException(msg % query) from err
 
         # Archive fetched, add a new entry to the history.
         self.append_to_history(
             {
                 "backend": self.name,
                 "action": "read",
-                "id": target + "/" + query,
+                "id": target.rstrip("/") + "/" + query,
                 "size": response["ContentLength"],
                 "timestamp": now(),
             }
         )
 
     def _get_object(self, bucket: Optional[str], key: str) -> dict:
         """Validate bucket (target) and key (query) and return the S3 object."""
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/data/swift.py` & `ralph-malph-5.0.0/src/ralph/backends/data/swift.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import logging
 from functools import cached_property
 from io import IOBase
 from typing import Any, Iterable, Iterator, Optional, Tuple, Union
 from uuid import uuid4
 
 from pydantic import PositiveInt
+from pydantic_settings import SettingsConfigDict
 from swiftclient.service import ClientException, Connection
 
 from ralph.backends.data.base import (
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseOperationType,
     DataBackendStatus,
     Listable,
     Writable,
 )
 from ralph.backends.data.mixins import HistoryMixin
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 from ralph.utils import now, parse_iterable_to_dict
 
 logger = logging.getLogger(__name__)
 
 
 class SwiftDataBackendSettings(BaseDataBackendSettings):
@@ -41,18 +42,18 @@
         USER_DOMAIN_NAME (str): The user domain name.
         DEFAULT_CONTAINER (str): The default target container.
         LOCALE_ENCODING (str): The encoding used for reading/writing documents.
         READ_CHUNK_SIZE (str): The default chunk size for reading objects.
         WRITE_CHUNK_SIZE (str): The default chunk size for writing objects.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__DATA__SWIFT__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__DATA__SWIFT__"),
+    }
 
     AUTH_URL: str = "https://auth.cloud.ovh.net/"
     DEFAULT_CONTAINER: Optional[str] = None
     IDENTITY_API_VERSION: str = "3"
     OBJECT_STORAGE_URL: Optional[str] = None
     PASSWORD: Optional[str] = None
     PROJECT_DOMAIN_NAME: str = "Default"
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/loader.py` & `ralph-malph-5.0.0/src/ralph/backends/loader.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/async_es.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/async_es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/async_mongo.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/async_mongo.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/base.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,120 +1,128 @@
 """Base LRS backend for Ralph."""
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, AsyncIterator, Iterator, List, Literal, Optional, TypeVar, Union
+from typing import (
+    Any,
+    AsyncIterator,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+)
 from uuid import UUID
 
-from pydantic import BaseModel, Field, NonNegativeInt
+from pydantic import AfterValidator, BaseModel, Field, NonNegativeInt
+from pydantic_settings import SettingsConfigDict
+from typing_extensions import Annotated
 
 from ralph.backends.data.base import (
     BaseAsyncDataBackend,
     BaseDataBackend,
     BaseDataBackendSettings,
     BaseQuery,
 )
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.models.xapi.base.agents import BaseXapiAgent
 from ralph.models.xapi.base.common import IRI
 from ralph.models.xapi.base.groups import BaseXapiGroup
 
 
 class BaseLRSBackendSettings(BaseDataBackendSettings):
     """LRS backend default configuration."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__LRS__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__LRS__"),
+    }
 
 
 @dataclass
 class StatementQueryResult:
     """Result of an LRS statements query."""
 
     statements: List[dict]
-    pit_id: Optional[str]
-    search_after: Optional[str]
+    pit_id: Optional[str] = None
+    search_after: Optional[str] = None
+
 
+def validate_iso_datetime_str(value: Union[str, datetime]) -> datetime:
+    """Value is expected to be an ISO 8601 date time string.
+
+    Note that we also accept datetime python instance that will be converted
+    to an ISO 8601 date time string.
+    """
+    if not isinstance(value, (str, datetime)):
+        raise TypeError("a string or datetime is required")
 
-class IsoDatetimeStr(str):
-    """ISO 8601 date time string field type."""
+    if isinstance(value, datetime):
+        return value.isoformat()
 
-    @classmethod
-    def __get_validators__(cls):
-        """Return expected validators for the custom field."""
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Value is expected to be an ISO 8601 date time string.
-
-        Note that we also accept datetime python instance that will be converted
-        to an ISO 8601 date time string.
-        """
-        if not isinstance(v, (str, datetime)):
-            raise TypeError("a string or datetime is required")
-
-        if isinstance(v, datetime):
-            return cls(v.isoformat())
-
-        # Validate iso-string
-        try:
-            datetime.fromisoformat(v)
-        except ValueError as err:
-            raise ValueError("invalid ISO 8601 date time string") from err
-        return cls(v)
+    # Validate iso-string
+    try:
+        datetime.fromisoformat(value)
+    except ValueError as err:
+        raise ValueError("invalid ISO 8601 date time string") from err
+
+
+IsoDatetimeStr = Annotated[
+    Union[str, datetime], AfterValidator(validate_iso_datetime_str)
+]
 
 
 class LRSStatementsQuery(BaseQuery):
     """Pydantic model for LRS query on Statements resource query parameters.
 
     LRS Specification:
     https://github.com/adlnet/xAPI-Spec/blob/1.0.3/xAPI-Communication.md#213-get-statements
     """
 
-    statement_id: Optional[str] = Field(None, alias="statementId")
-    voided_statement_id: Optional[str] = Field(None, alias="voidedStatementId")
-    agent: Optional[Union[BaseXapiAgent, BaseXapiGroup]]
-    verb: Optional[IRI]
-    activity: Optional[IRI]
-    registration: Optional[UUID]
+    statement_id: Annotated[Optional[str], Field(alias="statementId")] = None
+    voided_statement_id: Annotated[Optional[str], Field(alias="voidedStatementId")] = (
+        None
+    )
+    agent: Optional[Union[BaseXapiAgent, BaseXapiGroup]] = None
+    verb: Optional[IRI] = None
+    activity: Optional[IRI] = None
+    registration: Optional[UUID] = None
     related_activities: Optional[bool] = False
     related_agents: Optional[bool] = False
-    since: Optional[IsoDatetimeStr]
-    until: Optional[IsoDatetimeStr]
+    since: Optional[IsoDatetimeStr] = None
+    until: Optional[IsoDatetimeStr] = None
     limit: Optional[NonNegativeInt] = 0
     format: Optional[Literal["ids", "exact", "canonical"]] = "exact"
     attachments: Optional[bool] = False
     ascending: Optional[bool] = False
 
 
 class AgentParameters(BaseModel):
     """LRS query parameters for query on type Agent.
 
     NB: Agent refers to the data structure, NOT to the LRS query parameter.
     """
 
-    mbox: Optional[str]
-    mbox_sha1sum: Optional[str]
-    openid: Optional[str]
-    account__name: Optional[str]
-    account__home_page: Optional[str]
+    mbox: Optional[str] = None
+    mbox_sha1sum: Optional[str] = None
+    openid: Optional[str] = None
+    account__name: Optional[str] = None
+    account__home_page: Optional[str] = None
 
 
 class RalphStatementsQuery(LRSStatementsQuery):
     """Represents a dictionary of possible LRS query parameters."""
 
-    agent: Optional[AgentParameters] = AgentParameters.construct()
-    search_after: Optional[str]
-    pit_id: Optional[str]
-    authority: Optional[AgentParameters] = AgentParameters.construct()
-    ignore_order: Optional[bool]
+    agent: Optional[AgentParameters] = AgentParameters.model_construct()
+    search_after: Optional[str] = None
+    pit_id: Optional[str] = None
+    authority: Optional[AgentParameters] = AgentParameters.model_construct()
+    ignore_order: Optional[bool] = None
 
 
 Settings = TypeVar("Settings", bound=BaseLRSBackendSettings)
 
 
 class BaseLRSBackend(BaseDataBackend[Settings, Any]):
     """Base LRS backend interface."""
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/clickhouse.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/clickhouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 """ClickHouse LRS backend for Ralph."""
 
 import logging
 from typing import Generator, Iterator, List, Optional
 
+from pydantic_settings import SettingsConfigDict
+
 from ralph.backends.data.clickhouse import (
     ClickHouseDataBackend,
     ClickHouseDataBackendSettings,
 )
 from ralph.backends.lrs.base import (
     AgentParameters,
     BaseLRSBackend,
     BaseLRSBackendSettings,
     RalphStatementsQuery,
     StatementQueryResult,
 )
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 
 logger = logging.getLogger(__name__)
 
 
 class ClickHouseLRSBackendSettings(
     BaseLRSBackendSettings, ClickHouseDataBackendSettings
 ):
     """ClickHouse LRS backend default configuration.
 
     Attributes:
         IDS_CHUNK_SIZE (int): The chunk size for querying by ids.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__LRS__CLICKHOUSE__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__LRS__CLICKHOUSE__"),
+    }
 
     IDS_CHUNK_SIZE: int = 10000
 
 
 class ClickHouseLRSBackend(
     BaseLRSBackend[ClickHouseLRSBackendSettings], ClickHouseDataBackend
 ):
     """ClickHouse LRS backend implementation."""
 
     def query_statements(
         self, params: RalphStatementsQuery, target: Optional[str] = None
     ) -> StatementQueryResult:
         """Return the statements query payload using xAPI parameters."""
-        ch_params = params.dict(exclude_none=True)
+        ch_params = params.model_dump(exclude_none=True)
+
+        if "statement_id" in ch_params:
+            ch_params["statementId"] = ch_params["statement_id"]
+
         where = []
 
         if params.statement_id:
             where.append("event_id = {statementId:UUID}")
 
         self._add_agent_filters(ch_params, where, params.agent, "actor")
         ch_params.pop("agent", None)
@@ -90,14 +96,15 @@
         query = self.query_class(
             select=["event_id", "emission_time", "event"],
             where=where,
             parameters=ch_params,
             limit=params.limit,
             sort=order_by,
         )
+
         try:
             clickhouse_response = list(
                 self.read(
                     query=query,
                     target=target,
                     ignore_errors=True,
                 )
@@ -159,15 +166,15 @@
         target_field: str,
     ) -> None:
         """Add filters relative to agents to `where`."""
         if not agent_params:
             return
 
         if not isinstance(agent_params, dict):
-            agent_params = agent_params.dict()
+            agent_params = agent_params.model_dump()
 
         if agent_params.get("mbox"):
             ch_params[f"{target_field}__mbox"] = agent_params.get("mbox")
             where.append(
                 f"JSONExtractString(event, '{target_field}', 'mbox') = "
                 f"{{{target_field}__mbox:String}}"
             )
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/es.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/es.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Elasticsearch LRS backend for Ralph."""
 
 import logging
 from typing import Iterator, List, Optional
 
+from pydantic_settings import SettingsConfigDict
+
 from ralph.backends.data.es import (
     ESDataBackend,
     ESDataBackendSettings,
     ESQuery,
     ESQueryPit,
 )
 from ralph.backends.lrs.base import (
     AgentParameters,
     BaseLRSBackend,
     BaseLRSBackendSettings,
     RalphStatementsQuery,
     StatementQueryResult,
 )
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 
 logger = logging.getLogger(__name__)
 
 
 class ESLRSBackendSettings(BaseLRSBackendSettings, ESDataBackendSettings):
     """Elasticsearch LRS backend default configuration."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__LRS__ES__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__LRS__ES__"),
+    }
 
 
 class ESLRSBackend(BaseLRSBackend[ESLRSBackendSettings], ESDataBackend):
     """Elasticsearch LRS backend implementation."""
 
     def query_statements(
         self, params: RalphStatementsQuery, target: Optional[str] = None
@@ -88,40 +90,40 @@
         if params.since:
             es_query_filters += [{"range": {"timestamp": {"gt": params.since}}}]
 
         if params.until:
             es_query_filters += [{"range": {"timestamp": {"lte": params.until}}}]
 
         es_query = {
-            "pit": ESQueryPit.construct(id=params.pit_id),
+            "pit": ESQueryPit.model_construct(id=params.pit_id),
             "size": params.limit,
             "sort": [{"timestamp": {"order": "asc" if params.ascending else "desc"}}],
         }
         if len(es_query_filters) > 0:
             es_query["query"] = {"bool": {"filter": es_query_filters}}
 
         if params.ignore_order:
             es_query["sort"] = "_shard_doc"
 
         if params.search_after:
             es_query["search_after"] = params.search_after.split("|")
 
         # Note: `params` fields are validated thus we skip their validation in ESQuery.
-        return ESQuery.construct(**es_query)
+        return ESQuery.model_construct(**es_query)
 
     @staticmethod
     def _add_agent_filters(
         es_query_filters: list, agent_params: AgentParameters, target_field: str
     ) -> None:
         """Add filters relative to agents to `es_query_filters`."""
         if not agent_params:
             return
 
         if not isinstance(agent_params, dict):
-            agent_params = agent_params.dict()
+            agent_params = agent_params.model_dump()
 
         if agent_params.get("mbox"):
             field = f"{target_field}.mbox.keyword"
             es_query_filters += [{"term": {field: agent_params.get("mbox")}}]
         elif agent_params.get("mbox_sha1sum"):
             field = f"{target_field}.mbox_sha1sum.keyword"
             es_query_filters += [{"term": {field: agent_params.get("mbox_sha1sum")}}]
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/fs.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 import logging
 from datetime import datetime
 from io import IOBase
 from pathlib import Path
 from typing import Iterable, List, Literal, Optional, Union
 from uuid import UUID
 
+from pydantic_settings import SettingsConfigDict
+
 from ralph.backends.data.base import BaseOperationType
 from ralph.backends.data.fs import FSDataBackend, FSDataBackendSettings
 from ralph.backends.lrs.base import (
     AgentParameters,
     BaseLRSBackend,
     BaseLRSBackendSettings,
     RalphStatementsQuery,
     StatementQueryResult,
 )
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 
 logger = logging.getLogger(__name__)
 
 
 class FSLRSBackendSettings(BaseLRSBackendSettings, FSDataBackendSettings):
     """FileSystem LRS backend default configuration.
 
     Attributes:
         DEFAULT_LRS_FILE (str): The default LRS filename to store statements.
     """
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__LRS__FS__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__LRS__FS__"),
+    }
 
     DEFAULT_LRS_FILE: str = "fs_lrs.jsonl"
 
 
 class FSLRSBackend(BaseLRSBackend[FSLRSBackendSettings], FSDataBackend):
     """FileSystem LRS Backend."""
 
@@ -114,15 +116,15 @@
         filters: list, agent: Optional[AgentParameters], related: Optional[bool]
     ) -> None:
         """Add agent filters to `filters` if `agent` is set."""
         if not agent:
             return
 
         if not isinstance(agent, dict):
-            agent = agent.dict()
+            agent = agent.model_dump()
         FSLRSBackend._add_filter_by_mbox(filters, agent.get("mbox", None), related)
         FSLRSBackend._add_filter_by_sha1sum(
             filters, agent.get("mbox_sha1sum", None), related
         )
         FSLRSBackend._add_filter_by_openid(filters, agent.get("openid", None), related)
         FSLRSBackend._add_filter_by_account(
             filters,
@@ -137,15 +139,15 @@
         authority: Optional[AgentParameters],
     ) -> None:
         """Add authority filters to `filters` if `authority` is set."""
         if not authority:
             return
 
         if not isinstance(authority, dict):
-            authority = authority.dict()
+            authority = authority.model_dump()
         FSLRSBackend._add_filter_by_mbox(
             filters, authority.get("mbox", None), field="authority"
         )
         FSLRSBackend._add_filter_by_sha1sum(
             filters, authority.get("mbox_sha1sum", None), field="authority"
         )
         FSLRSBackend._add_filter_by_openid(
```

### Comparing `ralph-malph-4.2.0/src/ralph/backends/lrs/mongo.py` & `ralph-malph-5.0.0/src/ralph/backends/lrs/mongo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """MongoDB LRS backend for Ralph."""
 
 import logging
 from typing import Iterator, List, Optional
 
 from bson.objectid import ObjectId
+from pydantic_settings import SettingsConfigDict
 from pymongo import ASCENDING, DESCENDING
 
 from ralph.backends.data.mongo import (
     MongoDataBackend,
     MongoDataBackendSettings,
     MongoQuery,
 )
 from ralph.backends.lrs.base import (
     AgentParameters,
     BaseLRSBackend,
     BaseLRSBackendSettings,
     RalphStatementsQuery,
     StatementQueryResult,
 )
-from ralph.conf import BaseSettingsConfig
+from ralph.conf import BASE_SETTINGS_CONFIG
 from ralph.exceptions import BackendException, BackendParameterException
 
 logger = logging.getLogger(__name__)
 
 
 class MongoLRSBackendSettings(BaseLRSBackendSettings, MongoDataBackendSettings):
     """MongoDB LRS backend default configuration."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_prefix = "RALPH_BACKENDS__LRS__MONGO__"
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(env_prefix="RALPH_BACKENDS__LRS__MONGO__"),
+    }
 
 
 class MongoLRSBackend(BaseLRSBackend[MongoLRSBackendSettings], MongoDataBackend):
     """MongoDB LRS backend."""
 
     def query_statements(
         self, params: RalphStatementsQuery, target: Optional[str] = None
@@ -111,15 +112,15 @@
         mongo_sort_order = ASCENDING if params.ascending else DESCENDING
         mongo_query_sort = [
             ("_source.timestamp", mongo_sort_order),
             ("_id", mongo_sort_order),
         ]
 
         # Note: `params` fields are validated thus we skip MongoQuery validation.
-        return MongoQuery.construct(
+        return MongoQuery.model_construct(
             filter=mongo_query_filters, limit=params.limit, sort=mongo_query_sort
         )
 
     @staticmethod
     def _add_agent_filters(
         mongo_query_filters: dict, agent_params: AgentParameters, target_field: str
     ) -> None:
@@ -130,15 +131,15 @@
             agent_params (AgentParameters): Agent query parameters to search for.
             target_field (str): The target agent field name to perform the search.
         """
         if not agent_params:
             return
 
         if not isinstance(agent_params, dict):
-            agent_params = agent_params.dict()
+            agent_params = agent_params.model_dump()
 
         if agent_params.get("mbox"):
             key = f"_source.{target_field}.mbox"
             mongo_query_filters.update({key: agent_params.get("mbox")})
 
         if agent_params.get("mbox_sha1sum"):
             key = f"_source.{target_field}.mbox_sha1sum"
```

### Comparing `ralph-malph-4.2.0/src/ralph/cli.py` & `ralph-malph-5.0.0/src/ralph/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,29 +22,30 @@
     import uvicorn
 except ModuleNotFoundError:
     # This error will be caught in the runserver command. We should be able to
     # use all commands except the runserver command when lrs optional
     # dependencies are not installed.
     pass
 from click_option_group import optgroup
+from pydantic import AnyUrl
 
 from ralph import __version__ as ralph_version
 from ralph.backends.data.base import (
     AsyncWritable,
     BaseAsyncDataBackend,
     BaseOperationType,
     BaseQuery,
 )
 from ralph.backends.loader import (
     get_cli_backends,
     get_cli_list_backends,
     get_cli_write_backends,
     get_lrs_backends,
 )
-from ralph.conf import ClientOptions, CommaSeparatedTuple, HeadersParameters, settings
+from ralph.conf import ClientOptions, HeadersParameters, settings
 from ralph.logger import configure_logging
 from ralph.models.converter import Converter
 from ralph.models.selector import ModelSelector
 from ralph.models.validator import Validator
 from ralph.utils import (
     execute_async,
     get_backend_class,
@@ -74,14 +75,24 @@
                 param,
                 ctx,
             )
 
         return value
 
 
+class AnyUrlParamType(click.ParamType):
+    """AnyUrl parameter type."""
+
+    name = "URL"
+
+    def convert(self, value, param, ctx):  # noqa: ARG002
+        """Return str representation of AnyUrl instance."""
+        return str(value)
+
+
 class CommaSeparatedKeyValueParamType(click.ParamType):
     """Comma-separated key=value parameter type."""
 
     name = "key=value,key=value"
 
     def convert(self, value, param, ctx):
         """Split the values by comma and equal sign.
@@ -252,38 +263,40 @@
 def backends_options(backends: Dict[str, Type], name: Optional[str] = None):
     """Backend-related options decorator for Ralph commands."""
 
     def wrapper(command):
         backend_names = []
         for backend_name, backend in backends.items():
             backend_names.append(backend_name)
-            fields = backend.settings_class.__fields__.items()
+            fields = backend.settings_class.model_fields.items()
             for field_name, field in sorted(fields, key=lambda x: x[0], reverse=True):
-                field_type = field.type_
+                field_type = field.annotation
                 field_name = (  # noqa: PLW2901
                     f"{backend_name}-{field_name.lower()}".replace("_", "-")
                 )
                 option = f"--{field_name}"
                 option_kwargs = {"default": None}
                 if field.default:
                     option_kwargs["type"] = type(field.default)
                 # If the field is a boolean, convert it to a flag option
                 if field_type is bool:
                     option = f"{option}/--no-{field_name}"
                     option_kwargs["is_flag"] = True
                 elif field_type is dict:
                     option_kwargs["type"] = CommaSeparatedKeyValueParamType()
-                elif field_type is CommaSeparatedTuple:
+                elif field_type is tuple:  # CommaSeparatedTuple
                     option_kwargs["type"] = CommaSeparatedTupleParamType()
                 elif isclass(field_type) and issubclass(field_type, ClientOptions):
                     option_kwargs["type"] = ClientOptionsParamType(field_type)
                 elif isclass(field_type) and issubclass(field_type, HeadersParameters):
                     option_kwargs["type"] = HeadersParametersParamType(field_type)
                 elif field_type is Path:
                     option_kwargs["type"] = click.Path()
+                elif field_type is AnyUrl:
+                    option_kwargs["type"] = AnyUrlParamType()
 
                 command = optgroup.option(option.lower(), **option_kwargs)(command)
 
             command = (optgroup.group(f"{backend_name} backend"))(command)
 
         command = click.option(
             "-b",
@@ -464,29 +477,37 @@
         # Force Path object instantiation so that the file creation can be
         # faked in a test environment.
         auth_file = Path(settings.AUTH_FILE)
         # Create the authentication file if it does not exist
         auth_file.parent.mkdir(parents=True, exist_ok=True)
         auth_file.touch()
 
-        users = ServerUsersCredentials.parse_obj([])
+        users = ServerUsersCredentials.model_validate([])
         # Parse credentials file if not empty
         if auth_file.stat().st_size:
-            users = ServerUsersCredentials.parse_file(auth_file)
-        users += ServerUsersCredentials.parse_obj([credentials])
+            with open(auth_file, encoding=settings.LOCALE_ENCODING) as f:
+                users = ServerUsersCredentials.model_validate_json(f.read())
+
+        users += ServerUsersCredentials.model_validate(
+            [
+                credentials,
+            ]
+        )
+
         auth_file.write_text(
-            users.json(indent=2, exclude_none=True), encoding=settings.LOCALE_ENCODING
+            users.model_dump_json(indent=2, exclude_none=True),
+            encoding=settings.LOCALE_ENCODING,
         )
         logger.info("User %s has been added to: %s", username, settings.AUTH_FILE)
     else:
         click.echo(
             (
                 f"Copy/paste the following credentials to your LRS authentication "
                 f"file located in: {settings.AUTH_FILE}\n"
-                f"{credentials.json(indent=2, exclude_none=True)}"
+                f"{credentials.model_dump_json(indent=2, exclude_none=True)}"
             )
         )
 
 
 @cli.command()
 @click.option(
     "-p",
```

### Comparing `ralph-malph-4.2.0/src/ralph/conf.py` & `ralph-malph-5.0.0/src/ralph/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 """Configurations for Ralph."""
 
 import io
 from enum import Enum
 from pathlib import Path
-from typing import List, Sequence, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
-from pydantic import AnyHttpUrl, AnyUrl, BaseModel, BaseSettings, Extra, root_validator
+from pydantic import (
+    AfterValidator,
+    AnyHttpUrl,
+    AnyUrl,
+    BaseModel,
+    ConfigDict,
+    Field,
+    StringConstraints,
+    TypeAdapter,
+    model_validator,
+)
+from pydantic_settings import BaseSettings, SettingsConfigDict
+from typing_extensions import Annotated
 
 from ralph.exceptions import ConfigurationException
 from ralph.utils import import_string
 
 try:
     from click import get_app_dir
 except ImportError:
     # If we use Ralph as a library and Click is not installed, we consider the
     # application directory to be the current directory. For non-CLI usage, it
     # has no consequences.
     from unittest.mock import Mock
 
     get_app_dir = Mock(return_value=".")
 
-MODEL_PATH_SEPARATOR = "__"
 
+MODEL_PATH_SEPARATOR = "__"
 
-class BaseSettingsConfig:
-    """Pydantic model for BaseSettings Configuration."""
+NonEmptyStr = Annotated[str, Field(min_length=1)]
+NonEmptyStrictStr = Annotated[str, StringConstraints(min_length=1, strict=True)]
 
-    case_sensitive = True
-    env_nested_delimiter = "__"
-    env_prefix = "RALPH_"
-    extra = "ignore"
+BASE_SETTINGS_CONFIG = SettingsConfigDict(
+    case_sensitive=True, env_nested_delimiter="__", env_prefix="RALPH_", extra="ignore"
+)
 
 
 class CoreSettings(BaseSettings):
     """Pydantic model for Ralph's core settings."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
+    model_config = BASE_SETTINGS_CONFIG
 
     APP_DIR: Path = get_app_dir("ralph")
     LOCALE_ENCODING: str = getattr(io, "LOCALE_ENCODING", "utf8")
 
 
 core_settings = CoreSettings()
 
 
-class CommaSeparatedTuple(str):
-    """Pydantic field type validating comma-separated strings or lists/tuples."""
+def validate_comma_separated_tuple(value: Union[str, Tuple[str, ...]]) -> Tuple[str]:
+    """Checks whether the value is a comma separated string or a tuple."""
+    if isinstance(value, tuple):
+        return value
 
-    @classmethod
-    def __get_validators__(cls):  # noqa: D105
-        def validate(value: Union[str, Sequence[str]]) -> Sequence[str]:
-            """Check whether the value is a comma-separated string or a list/tuple."""
-            if isinstance(value, (tuple, list)):
-                return tuple(value)
+    if isinstance(value, str):
+        return tuple(value.split(","))
 
-            if isinstance(value, str):
-                return tuple(value.split(","))
+    raise TypeError("Invalid comma separated tuple")
 
-            raise TypeError("Invalid comma-separated list")
 
-        yield validate
+CommaSeparatedTuple = Annotated[
+    Union[str, Tuple[str, ...]], AfterValidator(validate_comma_separated_tuple)
+]
 
 
 class InstantiableSettingsItem(BaseModel):
     """Pydantic model for a settings configuration item that can be instantiated."""
 
-    class Config:  # noqa: D106
-        underscore_attrs_are_private = True
-
     _class_path: str = None
 
     def get_instance(self, **init_parameters):
         """Return an instance of the settings item class using its `_class_path`."""
         return import_string(self._class_path)(**init_parameters)
 
 
 class ClientOptions(BaseModel):
     """Pydantic model for additional client options."""
 
-    class Config:  # noqa: D106
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class HeadersParameters(BaseModel):
     """Pydantic model for headers parameters."""
 
-    class Config:  # noqa: D106
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow", populate_by_name=True)
 
 
 # Active parser Settings.
-
-
 class ESParserSettings(InstantiableSettingsItem):
     """Pydantic model for Elasticsearch parser configuration settings."""
 
     _class_path: str = "ralph.parsers.ElasticSearchParser"
 
 
 class GELFParserSettings(InstantiableSettingsItem):
@@ -111,77 +112,62 @@
     GELF: GELFParserSettings = GELFParserSettings()
     ES: ESParserSettings = ESParserSettings()
 
 
 class XapiForwardingConfigurationSettings(BaseModel):
     """Pydantic model for xAPI forwarding configuration item."""
 
-    class Config:  # noqa: D106
-        min_anystr_length = 1
-
     url: AnyUrl
     is_active: bool
-    basic_username: str
-    basic_password: str
+    basic_username: NonEmptyStr
+    basic_password: NonEmptyStr
     max_retries: int
     timeout: float
 
 
 class AuthBackend(str, Enum):
     """Model for valid authentication methods."""
 
     BASIC = "basic"
     OIDC = "oidc"
 
 
-class AuthBackends(Tuple[AuthBackend]):
-    """Model representing a tuple of authentication backends."""
-
-    @classmethod
-    def __get_validators__(cls):
-        """Check whether the value is a comma-separated string or a tuple representing
-        an AuthBackend.
-        """  # noqa: D205
-
-        def validate(
-            auth_backends: Union[
-                str, AuthBackend, Tuple[AuthBackend], List[AuthBackend]
-            ]
-        ) -> Tuple[AuthBackend]:
-            """Check whether the value is a comma-separated string or a list/tuple."""
-            if isinstance(auth_backends, str):
-                return tuple(
-                    AuthBackend(value.lower()) for value in auth_backends.split(",")
-                )
-
-            if isinstance(auth_backends, AuthBackend):
-                return (auth_backends,)
-
-            if isinstance(auth_backends, (tuple, list)):
-                return tuple(auth_backends)
-
-            raise TypeError("Invalid comma-separated list")
-
-        yield validate
+def validate_auth_backends(
+    value: Union[str, Tuple[str, ...], List[str]]
+) -> Tuple[AuthBackend]:
+    """Check whether the value is a comma separated string or a list/tuple."""
+    if isinstance(value, (tuple, list)):
+        return tuple(AuthBackend(val.lower()) for val in value)
+
+    if isinstance(value, str):
+        return tuple(AuthBackend(val) for val in value.lower().split(","))
+
+    raise TypeError("Invalid comma separated tuple")
+
+
+AuthBackends = Annotated[
+    Union[str, Tuple[str, ...], List[str]], AfterValidator(validate_auth_backends)
+]
 
 
 class Settings(BaseSettings):
     """Pydantic model for Ralph's global environment & configuration settings."""
 
-    class Config(BaseSettingsConfig):
-        """Pydantic Configuration."""
-
-        env_file = ".env"
-        env_file_encoding = core_settings.LOCALE_ENCODING
+    model_config = {
+        **BASE_SETTINGS_CONFIG,
+        **SettingsConfigDict(
+            env_file=".env", env_file_encoding=core_settings.LOCALE_ENCODING
+        ),
+    }
 
     _CORE: CoreSettings = core_settings
     AUTH_FILE: Path = _CORE.APP_DIR / "auth.json"
-    AUTH_CACHE_MAX_SIZE = 100
-    AUTH_CACHE_TTL = 3600
-    CONVERTER_EDX_XAPI_UUID_NAMESPACE: str = None
+    AUTH_CACHE_MAX_SIZE: int = 100
+    AUTH_CACHE_TTL: int = 3600
+    CONVERTER_EDX_XAPI_UUID_NAMESPACE: Optional[str] = None
     EXECUTION_ENVIRONMENT: str = "development"
     HISTORY_FILE: Path = _CORE.APP_DIR / "history.json"
     LOGGING: dict = {
         "version": 1,
         "propagate": True,
         "formatters": {
             "ralph": {
@@ -208,48 +194,57 @@
             "uvicorn": {
                 "handlers": ["console"],
                 "level": "INFO",
             },
         },
     }
     PARSERS: ParserSettings = ParserSettings()
-    RUNSERVER_AUTH_BACKENDS: AuthBackends = AuthBackends([AuthBackend.BASIC])
-    RUNSERVER_AUTH_OIDC_AUDIENCE: str = None
-    RUNSERVER_AUTH_OIDC_ISSUER_URI: AnyHttpUrl = None
+    RUNSERVER_AUTH_BACKENDS: AuthBackends = TypeAdapter(AuthBackends).validate_python(
+        "Basic"
+    )
+    RUNSERVER_AUTH_OIDC_AUDIENCE: Optional[str] = None
+    RUNSERVER_AUTH_OIDC_ISSUER_URI: Optional[AnyHttpUrl] = None
     RUNSERVER_BACKEND: str = "es"
     RUNSERVER_HOST: str = "0.0.0.0"  # noqa: S104
     RUNSERVER_MAX_SEARCH_HITS_COUNT: int = 100
     RUNSERVER_POINT_IN_TIME_KEEP_ALIVE: str = "1m"
     RUNSERVER_PORT: int = 8100
     LRS_RESTRICT_BY_AUTHORITY: bool = False
     LRS_RESTRICT_BY_SCOPES: bool = False
     SENTRY_CLI_TRACES_SAMPLE_RATE: float = 1.0
-    SENTRY_DSN: str = None
+    SENTRY_DSN: Optional[str] = None
     SENTRY_IGNORE_HEALTH_CHECKS: bool = False
     SENTRY_LRS_TRACES_SAMPLE_RATE: float = 1.0
     XAPI_FORWARDINGS: List[XapiForwardingConfigurationSettings] = []
 
     @property
     def APP_DIR(self) -> Path:
         """Return the path to Ralph's configuration directory."""
         return self._CORE.APP_DIR
 
     @property
     def LOCALE_ENCODING(self) -> str:
         """Return Ralph's default locale encoding."""
         return self._CORE.LOCALE_ENCODING
 
-    @root_validator(allow_reuse=True)
+    @model_validator(mode="before")
     @classmethod
-    def check_restriction_compatibility(cls, values):
+    def validate_paths(cls, values):
+        """Coerce fields to `Path`."""
+        for field in ["AUTH_FILE", "HISTORY_FILE"]:
+            if field in values:
+                if isinstance(values[field], str):
+                    values[field] = Path(values[field])
+        return values
+
+    @model_validator(mode="after")
+    def check_restriction_compatibility(self):
         """Raise an error if scopes are being used without authority restriction."""
-        if values.get("LRS_RESTRICT_BY_SCOPES") and not values.get(
-            "LRS_RESTRICT_BY_AUTHORITY"
-        ):
+        if self.LRS_RESTRICT_BY_SCOPES and not self.LRS_RESTRICT_BY_AUTHORITY:
             raise ConfigurationException(
                 "LRS_RESTRICT_BY_AUTHORITY must be set to True if using "
                 "LRS_RESTRICT_BY_SCOPES=True"
             )
-        return values
+        return self
 
 
 settings = Settings()
```

### Comparing `ralph-malph-4.2.0/src/ralph/exceptions.py` & `ralph-malph-5.0.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/filters.py` & `ralph-malph-5.0.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/converter.py` & `ralph-malph-5.0.0/src/ralph/models/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             ConversionException: When a field transformation fails.
         """
         if self.src:
             data = get_dict_value_from_path(data, self.src)
         try:
             for transformer in self.transformers:
                 data = transformer(data)
-        except Exception as err:  # noqa: BLE001
+        except Exception as err:
             msg = f"Failed to get the transformed value for field: {self.src}"
             raise ConversionException(msg) from err
         return data
 
 
 class BaseConversionSet(ABC):
     """ConversionSet Base Class.
@@ -133,14 +133,15 @@
     converted_event = {}
     for conversion_item in conversion_set:
         data = event_str if conversion_item.raw_input else event
         value = conversion_item.get_value(data)
         if value not in [None, "", {}]:
             set_dict_value_from_path(converted_event, conversion_item.dest, value)
     logger.debug("Intermediate converted event: %s", converted_event)
+
     return conversion_set.__dest__(**converted_event)
 
 
 def convert_str_event(event_str: str, conversion_set: BaseConversionSet) -> BaseModel:
     """Convert the event string using the provided conversion_set.
 
     Args:
@@ -194,15 +195,15 @@
     ) -> Generator:
         """Convert JSON event strings line by line."""
         total = 0
         success = 0
         for event_str in input_file:
             try:
                 total += 1
-                yield self._convert_event(event_str).json(
+                yield self._convert_event(event_str).model_dump_json(
                     exclude_none=True, by_alias=True
                 )
                 success += 1
             except (TypeError, json.JSONDecodeError) as err:
                 message = "Input event is not a valid JSON string"
                 self._log_error(message, event_str, err)
                 if not ignore_errors:
@@ -212,15 +213,15 @@
                 if fail_on_unknown:
                     raise err
             except ConversionException as err:
                 self._log_error(err, event_str)
                 if not ignore_errors:
                     raise err
             except ValidationError as err:
-                message = f"Converted event is not a valid ({err.model}) model"
+                message = "Converted event is not valid"
                 self._log_error(message, event_str, err)
                 if not ignore_errors:
                     raise err
         logger.info("Total events: %d, Invalid events: %d", total, total - success)
 
     def _convert_event(self, event_str: str) -> Any:
         """Convert a single JSON string event.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/__init__.py` & `ralph-malph-5.0.0/src/ralph/models/edx/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/base.py` & `ralph-malph-5.0.0/src/ralph/models/edx/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 """Base event model definitions."""
 
-import sys
 from datetime import datetime
 from ipaddress import IPv4Address
 from pathlib import Path
-from typing import Dict, Optional, Union
+from typing import Dict, Literal, Optional, Union
 
-from pydantic import AnyHttpUrl, BaseModel, constr
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from pydantic import (
+    AnyHttpUrl,
+    BaseModel,
+    ConfigDict,
+    Field,
+    StringConstraints,
+)
+from typing_extensions import Annotated
 
 
 class BaseModelWithConfig(BaseModel):
     """Pydantic model for base configuration shared among all models."""
 
-    class Config:  # noqa: D106
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid", coerce_numbers_to_str=True)
 
 
 class ContextModuleField(BaseModelWithConfig):
     """Pydantic model for `context`.`module` field.
 
     Attributes:
         usage_key (str): Consists of a block ID of the current component.
         display_name (str): Consists of a short description or title of the component.
     """
 
-    usage_key: constr(regex=r"^block-v1:.+\+.+\+.+type@.+@[a-f0-9]{32}$")
+    usage_key: Annotated[
+        str, StringConstraints(pattern=r"^block-v1:.+\+.+\+.+type@.+@[a-f0-9]{32}$")
+    ]
     display_name: str
     original_usage_key: Optional[
-        constr(regex=r"^block-v1:.+\+.+\+.+type@problem\+block@[a-f0-9]{32}$")
-    ]
-    original_usage_version: Optional[str]
+        Annotated[
+            str,
+            StringConstraints(
+                pattern=r"^block-v1:.+\+.+\+.+type@problem\+block@[a-f0-9]{32}$"
+            ),
+        ]
+    ] = None
+    original_usage_version: Optional[str] = None
 
 
 class BaseContextField(BaseModelWithConfig):
     """Pydantic model for core `context` field.
 
     Attributes:
         course_user_tags (Dict of str): Content from `user_api_usercoursetag` table.
@@ -75,20 +82,20 @@
                 Is an empty string when the requested page is not a course page.
         path (Path): Consist of the relative URL (without the hostname) of the
             requested page.
             Retrieved with::
                 `request.META['PATH_INFO']`
     """
 
-    course_id: constr(regex=r"^$|^course-v1:.+\+.+\+.+$")
-    course_user_tags: Optional[Dict[str, str]]
-    module: Optional[ContextModuleField]
+    course_id: Annotated[str, Field(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
+    course_user_tags: Optional[Dict[str, str]] = None
+    module: Optional[ContextModuleField] = None
     org_id: str
     path: Path
-    user_id: Union[int, Literal[""], None]
+    user_id: Union[int, Literal[""], None] = None
 
 
 class AbstractBaseEventField(BaseModelWithConfig):
     """Pydantic model for core `event` fields.
 
     The base model does not have any attributes as event field does not have common
     sub-fields.
@@ -145,15 +152,17 @@
             Retrieved with::
                 `datetime.datetime.utcnow()`
         page (None): Consists of the value `None`
             Note::
                 In JSON the value is `null` instead of `None`.
     """
 
-    username: Union[constr(min_length=2, max_length=30), Literal[""]]
+    username: Union[
+        Annotated[str, StringConstraints(min_length=2, max_length=30)], Literal[""]
+    ]
     ip: Union[IPv4Address, Literal[""]]
     agent: str
     host: str
     referer: Union[AnyHttpUrl, Literal[""]]
     accept_language: str
     context: BaseContextField
     time: datetime
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/bookmark/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/bookmark/fields/events.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Video event fields definitions."""
 
 import sys
 from typing import Optional
 
-from pydantic import constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -32,29 +33,34 @@
         "discussion",
         "html",
         "problem",
         "sequential",
         "vertical",
         "video",
     ]
-    component_usage_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@([a-z]+)\+block@[a-f0-9]{32}$"
-    )
+    component_usage_id: Annotated[
+        str,
+        StringConstraints(
+            pattern=(
+                r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+                r"type@([a-z]+)\+block@[a-f0-9]{32}$"
+            )
+        ),
+    ]
 
 
 class EdxBookmarkAddedEventField(EdxBookmarkBaseEventField):
     """Pydantic model for `edx.bookmark.added` `event` field.
 
     Attributes:
         course_id (str): Consists of the identifier of the course that includes
             the bookmark.
     """
 
-    course_id: constr(regex=r"^$|^course-v1:.+\+.+\+.+$")
+    course_id: Annotated[str, StringConstraints(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
 
 
 class EdxBookmarkListedEventField(AbstractBaseEventField):
     """Pydantic model for `edx.bookmark.listed` `event` field.
 
     Attributes:
         bookmarks_count (str): Consists of the number of pages a learner has bookmarked.
@@ -63,29 +69,31 @@
         list_type (str): Consists of either `per_course` or `all_courses` value.
         page_number(int): Consists of the current page number in the list of
             bookmarks.
         page_size (int): Consists of the number of bookmarks on the current page.
     """
 
     bookmarks_count: int
-    course_id: Optional[constr(regex=r"^$|^course-v1:.+\+.+\+.+$")]
+    course_id: Optional[
+        Annotated[str, StringConstraints(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
+    ]
     list_type: Literal["per_course", "all_courses"]
     page_number: int
     page_size: int
 
 
 class EdxBookmarkRemovedEventField(EdxBookmarkBaseEventField):
     """Pydantic model for `edx.bookmark.removed` `event` field.
 
     Attributes:
         course_id (str): Consists of the identifier of the course that includes
             the bookmark.
     """
 
-    course_id: constr(regex=r"^$|^course-v1:.+\+.+\+.+$")
+    course_id: Annotated[str, StringConstraints(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
 
 
 class UIEdxCourseToolAccessedEventField(AbstractBaseEventField):
     """Pydantic model for `edx.course.tool.accessed` `event` field.
 
     Attributes:
         tool_name (str): Consists of either `edx.bookmarks`, `edx.reviews`
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/bookmark/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/bookmark/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/browser.py` & `ralph-malph-5.0.0/src/ralph/models/edx/browser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Browser event model definitions."""
 
 import sys
 from typing import Union
 
-from pydantic import AnyUrl, constr
+from pydantic import AnyUrl, StringConstraints
+from typing_extensions import Annotated
 
 from .base import BaseEdxModel
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -25,8 +26,10 @@
                 `window.location.href` from the JavaScript front-end.
         session (str): Consists of the md5 encrypted Django session key or an empty
             string.
     """
 
     event_source: Literal["browser"]
     page: AnyUrl
-    session: Union[constr(regex=r"^[a-f0-9]{32}$"), Literal[""]]
+    session: Union[
+        Annotated[str, StringConstraints(pattern=r"^[a-f0-9]{32}$")], Literal[""]
+    ]
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/certificate/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/certificate/fields/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Cohort event field definition."""
 
 import sys
 from uuid import UUID
 
-from pydantic import AnyHttpUrl, constr
+from pydantic import AnyHttpUrl, StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -26,15 +27,15 @@
         user_id (int): Consists of the numeric ID of the learner who earned this
             certificate.
 
     """
 
     certificate_id: UUID
     certificate_url: AnyHttpUrl
-    course_id: constr(regex=r"^$|^course-v1:.+\+.+\+.+$")
+    course_id: Annotated[str, StringConstraints(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
     enrollment_mode: Literal["audit", "honor", "professional", "verified"]
     user_id: int
 
 
 class EdxCertificateCreatedEventField(CertificateBaseEventField):
     """Pydantic model for `edx.certificate.created` `event` field.
 
@@ -87,8 +88,8 @@
     """Pydantic model for certification generation core `event` field.
 
     Attributes:
         course_id (str): Consists of the ID of the course for which this
             certificate is issued.
     """
 
-    course_id: constr(regex=r"^$|^course-v1:.+\+.+\+.+$")
+    course_id: Annotated[str, StringConstraints(pattern=r"^$|^course-v1:.+\+.+\+.+$")]
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/certificate/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/certificate/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/cohort/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/cohort/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/cohort/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/cohort/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/fields/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             component that contains multiple parts.
         original_usage_key (str): Consists of the ID of the component in the library.
         original_usage_version (str): Consists of the version of the component
             in the library.
         usage_key (str): Consists of the location of this component in the course.
     """  # noqa: D205
 
-    descendants: Optional[list]
+    descendants: Optional[list] = None
     original_usage_key: str
     original_usage_version: str
     usage_key: str
 
 
 class ContentLibraryInteractionBaseEventField(AbstractBaseEventField):
     """Pydantic model for content library interaction core `event` field.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/content_library_interaction/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/content_library_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/enrollment.py` & `ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/enrollment.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,18 @@
         """Return a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
                     "object__id",
                     "event__course_id",
-                    lambda course_id: f"{self.platform_url}/courses/{course_id}/info",
+                    lambda course_id: (
+                        f"{self.platform_url.rstrip('/')}/courses/"
+                        f"{course_id.strip('/')}/info"
+                    ),
                 ),
                 ConversionItem(
                     "context__contextActivities__category",
                     None,
                     lambda _: [{"id": "https://w3id.org/xapi/lms"}],
                 ),
             },
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         """Return a set of ConversionItems used for conversion."""
         conversion_items = super()._get_conversion_items()
         return conversion_items.union(
             {
                 ConversionItem(
                     "object__id",
                     "event_type",
-                    lambda event_type: self.platform_url + event_type,
+                    lambda event_type: self.platform_url.rstrip("/") + event_type,
                 ),
             }
         )
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-5.0.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                     "object__definition__name",
                     "event__id",
                     lambda id: {LANG_EN_US_DISPLAY: id},
                 ),
                 ConversionItem(
                     "object__id",
                     None,
-                    lambda event: self.platform_url
+                    lambda event: self.platform_url.rstrip("/")
                     + "/xblock/block-v1:"
                     + event["context"]["course_id"]
                     + "-course-v1:+type@video+block@"
                     + event["event"]["id"],
                 ),
                 ConversionItem(
                     "context__contextActivities__category",
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/course_content_completion/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/course_content_completion/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/fields/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         manually (bool): Set to `true` when the learner manually closed the pop up
         dialog box, `false` when the browser closed it.
         truncated (bool): Set to `true` if the content was longer than 12500 characters.
     """
 
     content: str
     manually: bool
-    truncated: Optional[bool]
+    truncated: Optional[bool] = None
 
 
 class EdxDragAndDropV2ItemDroppedEventField(AbstractBaseEventField):
     """Pydantic model for `edx.drag_and_drop_v2.item.dropped` `event` field.
 
     Attributes:
         input (int): Consists of the number input value entered by the learner.
@@ -40,20 +40,20 @@
         location (str): Consists of the text identifier for the target zone in
             which the learner placed the item.
         location_id ((int): Consists of the automatically generated unique index
             assigned to the target zone in which the learner placed the item.
     """
 
     input: int
-    item: Optional[str]
+    item: Optional[str] = None
     item_id: int
     is_correct: bool
     is_correct_location: bool
     location: str
-    location_id: Optional[int]
+    location_id: Optional[int] = None
 
 
 class EdxDragAndDropV2ItemPickedUpEventField(AbstractBaseEventField):
     """Pydantic model for `edx.drag_and_drop_v2.item.picked_up` `event` field.
 
     Attributes:
         item_id (int): Consists of the index assigned to the draggable item
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/drag_and_drop/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/drag_and_drop/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Enrollment event models context fields definitions."""
 
 import sys
-from typing import Union
 
 from ...base import BaseContextField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -18,15 +17,15 @@
     `mode` context member field.
 
     Attributes:
         mode (str): Consists of either the `audit` or `honor` value. It identifies the
             enrollment mode when the user clicked <kbd>Challenge Yourself</kbd>.
     """
 
-    mode: Union[Literal["audit"], Literal["honor"]]
+    mode: Literal["audit", "honor"]
 
 
 class EdxCourseEnrollmentUpgradeSucceededContextField(BaseContextField):
     """Pydantic model for `edx.course.enrollment.upgrade.succeeded`.`context` field.
 
     In addition to the common context member fields, this statement also comprises the
     `mode` context member field.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         user_id (int): Identifies the student who was enrolled or unenrolled.
     """
 
     course_id: str
     mode: Union[
         Literal["audit"], Literal["honor"], Literal["professional"], Literal["verified"]
     ]
-    user_id: Union[int, Literal[""], None]
+    user_id: Union[int, Literal[""], None] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         event_type (str): Consists of the value `edx.course.enrollment.activated`.
         name (str): Consists of the value `edx.course.enrollment.activated`.
     """
 
     __selector__ = selector(
         event_source="server", event_type="edx.course.enrollment.activated"
     )
-
     event: Union[
         Json[EnrollmentEventField],
         EnrollmentEventField,
     ]
     event_type: Literal["edx.course.enrollment.activated"]
     name: Literal["edx.course.enrollment.activated"]
 
@@ -80,16 +79,16 @@
     """
 
     __selector__ = selector(
         event_source="server", event_type="edx.course.enrollment.mode_changed"
     )
 
     event: Union[
-        Json[EnrollmentEventField],
         EnrollmentEventField,
+        Json[EnrollmentEventField],
     ]
     event_type: Literal["edx.course.enrollment.mode_changed"]
     name: Literal["edx.course.enrollment.mode_changed"]
 
 
 class UIEdxCourseEnrollmentUpgradeClicked(BaseBrowserModel):
     """Pydantic model for `edx.course.enrollment.upgrade_clicked` statement.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Navigational event field definition."""
 
-from pydantic import constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 
 class NavigationalEventField(AbstractBaseEventField):
     """Pydantic model for navigational `event` field.
 
@@ -16,15 +17,18 @@
             For `seq_next` and `seq_prev`, it consists of the index of the unit being
             navigated to.
         new (int): For `seq_goto`, it consists of the index of the unit being jumped
             from. For `seq_next` and `seq_prev`, it consists of the index of the unit
             being navigated away from.
     """
 
-    id: constr(
-        regex=(
-            r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type"
-            r"@sequential\+block@[a-f0-9]{32}$"
-        )
-    )
+    id: Annotated[
+        str,
+        StringConstraints(
+            pattern=(
+                r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type"
+                r"@sequential\+block@[a-f0-9]{32}$"
+            )
+        ),
+    ]
     new: int
     old: int
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/navigational/statements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Navigational event model definitions."""
 
 import sys
 from typing import Union
 
-from pydantic import Json, validator
+from pydantic import Json, field_validator
 
 from ralph.models.selector import selector
 
 from ..browser import BaseBrowserModel
 from .fields.events import NavigationalEventField
 
 if sys.version_info >= (3, 8):
@@ -68,15 +68,15 @@
 
     __selector__ = selector(event_source="browser", event_type="seq_next")
 
     event: Union[Json[NavigationalEventField], NavigationalEventField]
     event_type: Literal["seq_next"]
     name: Literal["seq_next"]
 
-    @validator("event")
+    @field_validator("event")
     @classmethod
     def validate_next_jump_event_field(
         cls, value: Union[Json[NavigationalEventField], NavigationalEventField]
     ) -> Union[Json[NavigationalEventField], NavigationalEventField]:
         """Check that event.new is equal to event.old + 1."""
         if value.new != value.old + 1:
             raise ValueError("event.new - event.old should be equal to 1")
@@ -99,15 +99,15 @@
 
     __selector__ = selector(event_source="browser", event_type="seq_prev")
 
     event: Union[Json[NavigationalEventField], NavigationalEventField]
     event_type: Literal["seq_prev"]
     name: Literal["seq_prev"]
 
-    @validator("event")
+    @field_validator("event")
     @classmethod
     def validate_prev_jump_event_field(
         cls, value: Union[Json[NavigationalEventField], NavigationalEventField]
     ) -> Union[Json[NavigationalEventField], NavigationalEventField]:
         """Check that event.new is equal to event.old - 1."""
         if value.new != value.old - 1:
             raise ValueError("event.old - event.new should be equal to 1")
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/notes/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/notes/fields/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Notes event field definition."""
 
 import sys
 from typing import Dict, List
 
-from pydantic import constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -26,15 +27,15 @@
         tags (list): Consists of a list of tags the learner has specified.
         truncated (list): Consists of a list of names of any truncated fields.
     """
 
     component_usage_id: str
     highlighted_content: str
     note_id: str
-    note_text: constr(max_length=8333)
+    note_text: Annotated[str, StringConstraints(max_length=8333)]
     tags: List[str] = []
     truncated: List[
         Literal["note_text", "highlighted_content", "tags", "old_note_text", "old_tags"]
     ] = []
 
 
 class UIEdxCourseStudentNotesEditedEventField(NotesEventField):
@@ -43,15 +44,15 @@
     Attributes:
         old_note_text (str): Consists of the text of the note before the learner
             edited it.
         old_tags (list): Consists of a list of tags before the learner edited it.
 
     """
 
-    old_note_text: constr(max_length=8333)
+    old_note_text: Annotated[str, StringConstraints(max_length=8333)]
     old_tags: List[str] = []
 
 
 class UIEdxCourseStudentNotesNotesPageViewedEventField(AbstractBaseEventField):
     """Pydantic model for `edx.course.student_notes.notes_page_viewed` `event` field.
 
     Attributes:
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/notes/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/notes/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/fields/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Open Response Assessment events model event fields definitions."""
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 from uuid import UUID
 
-from pydantic import constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
 
 from ralph.models.edx.base import AbstractBaseEventField, BaseModelWithConfig
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -25,20 +26,23 @@
         requesting_student_id (str): Consists of the course-specific anonymized user ID
             of the learner who retrieved the response for peer assessment.
         submission_returned_uuid (str): Consists of the unique identifier of the
             response that was retrieved for assessment. Set to `None` if no assessment
             available.
     """
 
-    course_id: constr(max_length=255)
-    item_id: constr(
-        regex=(r"^block-v1:.+\+.+\+.+type@openassessment+block@[a-f0-9]{32}$")
-    )
+    course_id: Annotated[str, StringConstraints(max_length=255)]
+    item_id: Annotated[
+        str,
+        StringConstraints(
+            pattern=(r"^block-v1:.+\+.+\+.+type@openassessment+block@[a-f0-9]{32}$")
+        ),
+    ]
     requesting_student_id: str
-    submission_returned_uuid: Union[str, None]
+    submission_returned_uuid: Union[str, None] = None
 
 
 class ORAGetSubmissionForStaffGradingEventField(AbstractBaseEventField):
     """Pydantic model for `openassessmentblock.get_submission_for_staff_grading`.
     `event` field.
 
     Attributes:
@@ -49,18 +53,21 @@
             available.
         requesting_staff_id (str): Consists of the course-specific anonymized user ID
             of the course team member who is retrieved the response for grading.
         type (str): Consists of the type of staff grading that is being performed.
             Currently, set to `full-grade`.
     """  # noqa: D205
 
-    item_id: constr(
-        regex=(r"^block-v1:.+\+.+\+.+type@openassessment+block@[a-f0-9]{32}$")
-    )
-    submission_returned_uuid: Union[str, None]
+    item_id: Annotated[
+        str,
+        StringConstraints(
+            pattern=(r"^block-v1:.+\+.+\+.+type@openassessment+block@[a-f0-9]{32}$")
+        ),
+    ]
+    submission_returned_uuid: Union[str, None] = None
     requesting_staff_id: str
     type: Literal["full-grade"]
 
 
 class ORAAssessEventPartsCriterionField(BaseModelWithConfig):
     """Pydantic model for assessment `event`.`parts`.`criterion` field.
 
@@ -82,15 +89,15 @@
         criterion (dict): see ORAAssessEventPartsCriterionField.
         feedback (str): Consists of feedback comments that the learner could have
             supplied.
     """
 
     option: str
     criterion: ORAAssessEventPartsCriterionField
-    feedback: Optional[str]
+    feedback: Optional[str] = None
 
 
 class ORAAssessEventRubricField(BaseModelWithConfig):
     """Pydantic model for assessment `event`.`rubric` field.
 
     This field is defined in:
     - `openassessmentblock.peer_assess`
@@ -98,15 +105,15 @@
     - `openassessmentblock.staff_assess`
 
     Attributes:
         content_hash: Consists of the identifier of the rubric that the learner used to
             assess the response.
     """
 
-    content_hash: constr(regex=r"^[a-f0-9]{1,40}$")
+    content_hash: Annotated[str, StringConstraints(pattern=r"^[a-f0-9]{1,40}$")]
 
 
 class ORAAssessEventField(AbstractBaseEventField):
     """Pydantic model for assessment `event` field.
 
     This field is defined in:
         - `openassessmentblock.peer_assess`
@@ -127,15 +134,15 @@
             response.
     """
 
     feedback: str
     parts: List[ORAAssessEventPartsField]
     rubric: ORAAssessEventRubricField
     scored_at: datetime
-    scorer_id: constr(max_length=40)
+    scorer_id: Annotated[str, StringConstraints(max_length=40)]
     score_type: Literal["PE", "SE", "ST"]
     submission_uuid: UUID
 
 
 class ORAStaffAssessEventField(ORAAssessEventField):
     """Pydantic model for `openassessmentblock.staff_assess`.`event` field.
 
@@ -174,16 +181,16 @@
         file_keys (list): Consists of a list of file identifiers if files are given for
             answer.
         files_description (list): Consists of a list of file descriptions if files are
             given for answer.
     """  # noqa: D205
 
     parts: List[Dict[Literal["text"], str]]
-    file_keys: Optional[List[str]]
-    files_descriptions: Optional[List[str]]
+    file_keys: Optional[List[str]] = None
+    files_descriptions: Optional[List[str]] = None
 
 
 class ORACreateSubmissionEventField(AbstractBaseEventField):
     """Pydantic model for `openassessmentblock.create_submission`.`event` field.
 
     Attributes:
         answer (dict): see ORACreateSubmissionEventAnswerField.
@@ -210,15 +217,15 @@
         text (str): Consists of the response text.
         file_upload_key (str): Consists of the AWS S3 key that identifies the location
             of the uploaded file on the Amazon S3 storage service. Only present when
             responses include an image, .pdf, or other file.
     """
 
     text: str
-    file_upload_key: Optional[str]
+    file_upload_key: Optional[str] = None
 
 
 class ORASaveSubmissionEventField(AbstractBaseEventField):
     """Pydantic model for `openassessmentblock.save_submission`.`event` field.
 
     Attributes:
         saved_response (str): Consists of a JSON string of the users saved responses.
@@ -255,10 +262,10 @@
 
     Attributes:
         fileName (str): Consists of the name of the uploaded file.
         fileSize (int): Consists of the bytes size of the uploaded file.
         fileType (str): Consists of the MIME type of the uploaded file.
     """
 
-    fileName: constr(max_length=255)
+    fileName: Annotated[str, StringConstraints(max_length=255)]
     fileSize: int
     fileType: str
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/open_response_assessment/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/open_response_assessment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/fields/events.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Peer instruction event field definition."""
 
-from pydantic import constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 
 class PeerInstructionEventField(AbstractBaseEventField):
     """Pydantic model for peer instruction `event` field.
 
@@ -14,9 +15,9 @@
         rationale (str): Consists of the text entered by the learner to explain why
             they selected that answer choice.
         truncated (bool): `True` only if the rationale was longer than 12,500
             characters, which is the maximum included in the event.
     """
 
     answer: int
-    rationale: constr(max_length=12500)
+    rationale: Annotated[str, StringConstraints(max_length=12500)]
     truncated: bool
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/peer_instruction/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/peer_instruction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/poll/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/poll/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Problem interaction events model event fields definitions."""
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
-from pydantic import constr
+from pydantic import Field
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField, BaseModelWithConfig
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -37,39 +38,39 @@
         hint (str): Consists of optional hint.
         hint_mode (str): Consists either of the value `on_request` or `always` value.
         msg (str): Consists of extra message response.
         npoints (int): Consists of awarded points.
         queuestate (json): see QueueStateField.
     """
 
-    answervariable: Union[Literal[None], None, str]
-    correctness: Union[Literal["correct"], Literal["incorrect"]]
-    hint: Optional[str]
-    hintmode: Optional[Union[Literal["on_request"], Literal["always"]]]
+    answervariable: Optional[str] = None
+    correctness: Literal["correct", "incorrect"]
+    hint: Optional[str] = None
+    hintmode: Optional[Literal["on_request", "always"]] = None
     msg: str
-    npoints: Optional[int]
-    queuestate: Optional[QueueState]
+    npoints: Optional[int] = None
+    queuestate: Optional[QueueState] = None
 
 
 class State(BaseModelWithConfig):
     """Pydantic model for problem interaction `event`.`state` field.
 
     Attributes:
         correct_map (dict): see CorrectMapSubFields.
         done (bool): `True` if the problem is answered, else `False`.
         input_state (dict): Consists of the state field given before answering.
         seed (int): Consists of the seed element for the current state.
         student_answers (dict): Consists of the answer(s) given by the user.
     """
 
     correct_map: Dict[
-        constr(regex=r"^[a-f0-9]{32}_[0-9]_[0-9]$"),
+        Annotated[str, Field(pattern=r"^[a-f0-9]{32}_[0-9]_[0-9]$")],
         CorrectMap,
     ]
-    done: Optional[bool]
+    done: Optional[bool] = None
     input_state: dict
     seed: int
     student_answers: dict
 
 
 class SubmissionAnswerField(BaseModelWithConfig):
     """Pydantic model for `problem_check`.`event`.`submission` field.
@@ -131,29 +132,29 @@
         question_type (str): Consists of the XML tag that identifies the problem type.
         student_answer (list): Consists of the answer value(s) selected or supplied by
             the user.
         trigger_type (str): Identifies the type of feedback obtained by the
             `student_answer` response. Consists either of `single` or `compound` value.
     """
 
-    choice_all: Optional[List[str]]
+    choice_all: Optional[List[str]] = None
     correctness: bool
     hint_label: str
     hints: List[dict]
     module_id: str
     problem_part_id: str
-    question_type: Union[
-        Literal["stringresponse"],
-        Literal["choiceresponse"],
-        Literal["multiplechoiceresponse"],
-        Literal["numericalresponse"],
-        Literal["optionresponse"],
+    question_type: Literal[
+        "stringresponse",
+        "choiceresponse",
+        "multiplechoiceresponse",
+        "numericalresponse",
+        "optionresponse",
     ]
     student_answer: List[str]
-    trigger_type: Union[Literal["single"], Literal["compound"]]
+    trigger_type: Literal["single", "compound"]
 
 
 class ProblemCheckEventField(AbstractBaseEventField):
     """Pydantic model for `problem_check`.`event` field.
 
     Attributes:
         answers (dict): Consists of a dictionary of problem ID and the corresponding
@@ -166,56 +167,62 @@
         problem_id (str): Consists of the ID of the problem that was checked.
         state (json): Consists of the current problem state.
         submission (dict): Consists of a dictionary of data about the given answer.
         success (str): Consists of either the `correct` or `incorrect` value.
     """
 
     answers: Dict[
-        constr(regex=r"^[a-f0-9]{32}_[0-9]_[0-9]$"),
-        Union[List[str], str],
+        Annotated[str, Field(pattern=r"^[a-f0-9]{32}_[0-9]_[0-9]$")],
+        Union[str, List[str]],
     ]
     attempts: int
     correct_map: Dict[
-        constr(regex=r"^[a-f0-9]{32}_[0-9]_[0-9]$"),
+        Annotated[str, Field(pattern=r"^[a-f0-9]{32}_[0-9]_[0-9]$")],
         CorrectMap,
     ]
     grade: int
     max_grade: int
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
     state: State
     submission: Dict[
-        constr(regex=r"^[a-f0-9]{32}_[0-9]_[0-9]$"),
+        Annotated[str, Field(pattern=r"^[a-f0-9]{32}_[0-9]_[0-9]$")],
         SubmissionAnswerField,
     ]
-    success: Union[Literal["correct"], Literal["incorrect"]]
+    success: Literal["correct", "incorrect"]
 
 
 class ProblemCheckFailEventField(AbstractBaseEventField):
     """Pydantic model for `problem_check_fail`.`event` field.
 
     Attributes:
         answers (dict): Consists of a dictionary of problem ID and the internal answer
             identifier for each problem.
         failure (str): Consists either of the `closed` or `unreset` value.
         problem_id (str): Consists of the ID of the problem that was checked.
         state (dict): Consists of the current problem state.
     """
 
     answers: Dict[
-        constr(regex=r"^[a-f0-9]{32}_[0-9]_[0-9]$"),
-        Union[List[str], str],
+        Annotated[str, Field(pattern=r"^[a-f0-9]{32}_[0-9]_[0-9]$")],
+        Union[str, List[str]],
+    ]
+    failure: Literal["closed", "unreset"]
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
     ]
-    failure: Union[Literal["closed"], Literal["unreset"]]
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
     state: State
 
 
 class ProblemRescoreEventField(AbstractBaseEventField):
     """Pydantic model for `problem_rescore`.`event` field.
 
     Attributes:
@@ -231,36 +238,42 @@
 
     attempts: int
     correct_map: CorrectMap
     new_score: int
     new_total: int
     orig_score: int
     orig_total: int
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
     state: State
-    success: Union[Literal["correct"], Literal["incorrect"]]
+    success: Literal["correct", "incorrect"]
 
 
 class ProblemRescoreFailEventField(AbstractBaseEventField):
     """Pydantic model for `problem_rescore_fail`.`event` field.
 
     Attributes:
         failure (str): Consists either of the `closed` or `unreset` value.
         problem_id (str): Consists of the ID of the problem being checked.
         state (json): see StateField.
     """
 
-    failure: Union[Literal["closed"], Literal["unreset"]]
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    failure: Literal["closed", "unreset"]
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
     state: State
 
 
 class UIProblemResetEventField(AbstractBaseEventField):
     """Pydantic model for `problem_reset`.`event` field.
 
     Attributes:
@@ -289,79 +302,94 @@
         new_state (json): see StateField.
         old_state (json): see StateField.
         problem_id (str): Consists of the ID of the problem being reset.
     """
 
     new_state: State
     old_state: State
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
 
 
 class ResetProblemFailEventField(AbstractBaseEventField):
     """Pydantic model for `reset_problem_fail`.`event` field.
 
     Attributes:
         failure (str): Consists either of `closed` or `not_done` value.
         old_state (json): see StateField.
         problem_id (str): Consists of the ID of the problem being reset.
     """
 
-    failure: Union[Literal["closed"], Literal["not_done"]]
+    failure: Literal["closed", "not_done"]
     old_state: State
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
 
 
 class SaveProblemFailEventField(AbstractBaseEventField):
     """Pydantic model for `save_problem_fail`.`event` field.
 
     Attributes:
         answers (dict): Consists of a dict of the answer string or a list or a dict of
             the answer strings if multiple choices are allowed.
         failure (str): Consists either of `closed` or `done` value.
         problem_id (str): Consists of the ID of the problem being saved.
         state (json): see StateField.
     """
 
     answers: Dict[str, Union[int, str, list, dict]]
-    failure: Union[Literal["closed"], Literal["done"]]
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    failure: Literal["closed", "done"]
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
     state: State
 
 
 class SaveProblemSuccessEventField(AbstractBaseEventField):
     """Pydantic model for `save_problem_success`.`event` field.
 
     Attributes:
         answers (dict): Consists of a dict of the answer string or a list or a dict of
             the answer strings if multiple choices are allowed.
         problem_id (str): Consists of the ID of the problem being saved.
         state (json): see StateField.
     """
 
     answers: Dict[str, Union[int, str, list, dict]]
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
     state: State
 
 
 class ShowAnswerEventField(AbstractBaseEventField):
     """Pydantic model for `show_answer`.`event` field.
 
     Attributes:
         problem_id (str): Consists of the ID of the problem being shown.
     """
 
-    problem_id: constr(
-        regex=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
-        r"type@problem\+block@[a-f0-9]{32}$"
-    )
+    problem_id: Annotated[
+        str,
+        Field(
+            pattern=r"^block-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+"
+            r"type@problem\+block@[a-f0-9]{32}$"
+        ),
+    ]
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/server.py` & `ralph-malph-5.0.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/survey/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/survey/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/survey/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/survey/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/teams_related/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/teams_related/fields/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Peer instruction event field definition."""
 
 import sys
 from typing import List, Union
 
-from pydantic import constr, validator
+from pydantic import StringConstraints, validator
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -34,16 +35,16 @@
         old (str): Consists of the value of the field before the modification. If
             longer than 1250 characters, it is truncated and suffixed with `...`.
         truncated (list): Consists of the truncated values of `new` and `old` if
             the values are longer than 1250.
     """
 
     field: str
-    new: constr(max_length=1250)
-    old: constr(max_length=1250)
+    new: Annotated[str, StringConstraints(max_length=1250)]
+    old: Annotated[str, StringConstraints(max_length=1250)]
     truncated: List[str]
 
     @validator("truncated")
     def check_truncated_length(cls, v):
         """Check length of truncated field."""
         if not len(v) <= 2:  # noqa: PLR2004
             raise ValueError("truncated length must be lower than 2")
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/teams_related/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/teams_related/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Textbook interaction event fields definitions."""
 
 import sys
 from typing import Optional, Union
 
-from pydantic import Field, constr
+from pydantic import Field, StringConstraints
+from typing_extensions import Annotated
 
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -19,17 +20,20 @@
     Attributes:
         chapter (str): Consists of the name of the PDF file.
             It begins with the `block_id` value and ends with the `.pdf` extension.
         page (int): The number of the page that is open when the event is emitted.
     """
 
     page: int
-    chapter: constr(
-        regex=(r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$")
-    )
+    chapter: Annotated[
+        str,
+        StringConstraints(
+            pattern=r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$"
+        ),
+    ]
 
 
 class TextbookPdfThumbnailsToggledEventField(TextbookInteractionBaseEventField):
     """Pydantic model for `textbook.pdf.thumbnails.toggled`.`event` field.
 
     Attribute:
         name (str): Consists of the value `textbook.pdf.thumbnails.toggled`.
@@ -66,17 +70,20 @@
     Attributes:
         name (str): Consists of the value `textbook.pdf.chapter.navigated`.
         chapter (str): Consists of the name of the PDF file.
             It begins with the `block_id` value and ends with the `.pdf` extension.
     """
 
     name: Literal["textbook.pdf.chapter.navigated"]
-    chapter: constr(
-        regex=(r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$")
-    )
+    chapter: Annotated[
+        str,
+        StringConstraints(
+            pattern=r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$"
+        ),
+    ]
     chapter_title: str
 
 
 class TextbookPdfPageNavigatedEventField(TextbookInteractionBaseEventField):
     """Pydantic model for `textbook.pdf.page.navigated`.`event` field.
 
     Attribute:
@@ -91,15 +98,15 @@
 
     Attributes:
         name (str): Consists of the value `textbook.pdf.zoom.buttons.changed`.
         direction (str): Consists of either the `in` or `out` value.
     """
 
     name: Literal["textbook.pdf.zoom.buttons.changed"]
-    direction: Union[Literal["in"], Literal["out"]]
+    direction: Literal["in", "out"]
 
 
 class TextbookPdfZoomMenuChangedEventField(TextbookInteractionBaseEventField):
     """Pydantic model for `textbook.pdf.zoom.menu.changed`.`event` field.
 
     Attributes:
         name (str): Consists of the value `textbook.pdf.zoom.menu.changed`.
@@ -142,15 +149,15 @@
 
     Attributes:
         name (str): Consists of the value `textbook.pdf.page.scrolled`.
         direction (str): Consists either of the `up` or `down` value.
     """
 
     name: Literal["textbook.pdf.page.scrolled"]
-    direction: Union[Literal["up"], Literal["down"]]
+    direction: Literal["up", "down"]
 
 
 class TextbookPdfSearchExecutedEventField(TextbookInteractionBaseEventField):
     """Pydantic model for `textbook.pdf.search.executed`.`event` field.
 
     Attributes:
         name (str): Consists of the value `textbook.pdf.search.executed`.
@@ -252,18 +259,20 @@
         old (int): Consists of the original page number. It applies to `gotopage` event
             types only.
         type (str): Consists of `gotopage` value when a page loads after the student
             manually enters its number, `prevpage` value when the next page button is
             clicked or `nextpage` value when the previous page button is clicked.
     """
 
-    chapter: constr(
-        regex=(r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$")
-    )
-    name: Union[
-        Literal["textbook.pdf.page.loaded"], Literal["textbook.pdf.page.navigatednext"]
+    chapter: Annotated[
+        str,
+        StringConstraints(
+            pattern=r"^\/asset-v1:[^\/+]+(\/|\+)[^\/+]+(\/|\+)[^\/?]+type@asset\+block.+$"
+        ),
     ]
+    name: Literal["textbook.pdf.page.loaded", "textbook.pdf.page.navigatednext"]
     new: int
-    old: Optional[int]
-    type: Union[Literal["gotopage"], Literal["prevpage"], Literal["nextpage"]] = Field(
-        alias="type"
-    )
+    old: Optional[int] = None
+    type: Annotated[
+        Literal["gotopage", "prevpage", "nextpage"],
+        Field(alias="type"),
+    ]
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-5.0.0/src/ralph/models/edx/video/fields/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Video event fields definitions."""
 
 import sys
 
+from pydantic import ConfigDict, NonNegativeFloat
+
 from ...base import AbstractBaseEventField
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -16,97 +18,96 @@
     Attributes:
         code (str): Consists of the `html5` value for browser-played
             videos.
         id (str): Consists of the additional videos name if given by the
             course creators, or the system-generated hash code otherwise.
     """
 
-    class Config:  # noqa: D106
-        extra = "allow"
+    model_config = ConfigDict(extra="allow", coerce_numbers_to_str=True)
 
     code: str
     id: str
 
 
 class PlayVideoEventField(VideoBaseEventField):
     """Pydantic model for `play_video`.`event` field.
 
     Attributes:
         currentTime (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    currentTime: float
+    currentTime: NonNegativeFloat
 
 
 class PauseVideoEventField(VideoBaseEventField):
     """Pydantic model for `pause_video`.`event`.
 
     Attributes:
         currentTime (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    currentTime: float
+    currentTime: NonNegativeFloat
 
 
 class SeekVideoEventField(VideoBaseEventField):
     """Pydantic model for `seek_video`.`event` field.
 
     Attributes:
         new_time (float): Consists of the point in time the actor changed to in a media
             object during a seek operation.
         old_time (float): Consists of the point in time the actor changed from in a
             media object during a seek operation.
         type (str): Consists of the navigational method used to change position
             within the video, either `onCaptionSeek` or `onSlideSeek` value.
     """
 
-    new_time: float
-    old_time: float
+    new_time: NonNegativeFloat
+    old_time: NonNegativeFloat
     type: str
 
 
 class StopVideoEventField(VideoBaseEventField):
     """Pydantic model for `stop_video`.`event` field.
 
     Attributes:
         currentTime (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    currentTime: float
+    currentTime: NonNegativeFloat
 
 
 class VideoHideTranscriptEventField(VideoBaseEventField):
     """Pydantic model for `hide_transcript`.`event` field.
 
     Attributes:
         current_time (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    current_time: float
+    current_time: NonNegativeFloat
 
 
 class VideoShowTranscriptEventField(VideoBaseEventField):
     """Pydantic model for `show_transcript`.`event` field.
 
     Attributes:
         current_time (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    current_time: float
+    current_time: NonNegativeFloat
 
 
 class SpeedChangeVideoEventField(VideoBaseEventField):
     """Pydantic model for `speed_change_video`.`event` field.
 
     Attributes:
         currentTime (float): Consists of the time in the video at which
             the statement was emitted.
     """
 
-    currentTime: float
+    currentTime: NonNegativeFloat
     new_speed: Literal["0.75", "1.0", "1.25", "1.50", "2.0"]
     old_speed: Literal["0.75", "1.0", "1.25", "1.50", "2.0"]
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-5.0.0/src/ralph/models/edx/video/statements.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     __selector__ = selector(event_source="browser", event_type="play_video")
 
     event: Union[
         Json[PlayVideoEventField],
         PlayVideoEventField,
     ]
     event_type: Literal["play_video"]
-    name: Optional[Literal["play_video", "edx.video.played"]]
+    name: Optional[Literal["play_video", "edx.video.played"]] = None
 
 
 class UIPauseVideo(BaseBrowserModel):
     """Pydantic model for `pause_video` statement.
 
     The browser emits this statement when a user selects the video player's pause
     control.
@@ -84,15 +84,15 @@
     __selector__ = selector(event_source="browser", event_type="pause_video")
 
     event: Union[
         Json[PauseVideoEventField],
         PauseVideoEventField,
     ]
     event_type: Literal["pause_video"]
-    name: Optional[Literal["pause_video", "edx.video.paused"]]
+    name: Optional[Literal["pause_video", "edx.video.paused"]] = None
 
 
 class UISeekVideo(BaseBrowserModel):
     """Pydantic model for `seek_video` statement.
 
     The browser emits this statement when a user selects a user interface control to go
     to a different point in the video file.
@@ -107,15 +107,15 @@
     __selector__ = selector(event_source="browser", event_type="seek_video")
 
     event: Union[
         Json[SeekVideoEventField],
         SeekVideoEventField,
     ]
     event_type: Literal["seek_video"]
-    name: Optional[Literal["seek_video", "edx.video.position.changed"]]
+    name: Optional[Literal["seek_video", "edx.video.position.changed"]] = None
 
 
 class UIStopVideo(BaseBrowserModel):
     """Pydantic model for `stop_video` statement.
 
     The browser emits this statement when the video player reaches the end of the video
     file and play automatically stops.
@@ -129,15 +129,15 @@
     __selector__ = selector(event_source="browser", event_type="stop_video")
 
     event: Union[
         Json[StopVideoEventField],
         StopVideoEventField,
     ]
     event_type: Literal["stop_video"]
-    name: Optional[Literal["stop_video", "edx.video.stopped"]]
+    name: Optional[Literal["stop_video", "edx.video.stopped"]] = None
 
 
 class UIHideTranscript(BaseBrowserModel):
     """Pydantic model for `hide_transcript` statement.
 
     The browser emits this statement when a user selects <kbd>CC</kbd> to suppress
     display of the video transcript.
@@ -196,15 +196,15 @@
     __selector__ = selector(event_source="browser", event_type="speed_change_video")
 
     event: Union[
         Json[SpeedChangeVideoEventField],
         SpeedChangeVideoEventField,
     ]
     event_type: Literal["speed_change_video"]
-    name: Optional[Literal["speed_change_video"]]
+    name: Optional[Literal["speed_change_video"]] = None
 
 
 class UIVideoHideCCMenu(BaseBrowserModel):
     """Pydantic model for `video_hide_cc_menu` statement.
 
     The browser emits this statement when a user selects a language from the CC menu
     for a video that has transcripts in multiple languages
@@ -217,15 +217,15 @@
     __selector__ = selector(event_source="browser", event_type="video_hide_cc_menu")
 
     event: Union[
         Json[VideoBaseEventField],
         VideoBaseEventField,
     ]
     event_type: Literal["video_hide_cc_menu"]
-    name: Optional[Literal["video_hide_cc_menu"]]
+    name: Optional[Literal["video_hide_cc_menu"]] = None
 
 
 class UIVideoShowCCMenu(BaseBrowserModel):
     """Pydantic model for `video_show_cc_menu` statement.
 
     The browser emits this statement when a user selects CC for a video that has
     transcripts in multiple languages.
@@ -240,8 +240,8 @@
     __selector__ = selector(event_source="browser", event_type="video_show_cc_menu")
 
     event: Union[
         Json[VideoBaseEventField],
         VideoBaseEventField,
     ]
     event_type: Literal["video_show_cc_menu"]
-    name: Optional[Literal["video_show_cc_menu"]]
+    name: Optional[Literal["video_show_cc_menu"]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/selector.py` & `ralph-malph-5.0.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/validator.py` & `ralph-malph-5.0.0/src/ralph/models/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 if not ignore_errors:
                     raise BadFormatException(message) from err
             except UnknownEventException as err:
                 self._log_error(err, event_str)
                 if fail_on_unknown:
                     raise err
             except ValidationError as err:
-                message = f"Input event is not a valid {err.model.__name__} event."
+                message = "Input event is not valid."
                 self._log_error(message, event_str, err)
                 if not ignore_errors:
                     raise BadFormatException(message) from err
         logger.info("Total events: %d, Invalid events: %d", total, total - success)
 
     def get_first_valid_model(self, event: dict) -> Any:
         """Return the first successfully instantiated model for the event.
@@ -55,15 +55,14 @@
         """
         error: Optional[BaseException] = None
         for model in self.model_selector.get_models(event):
             try:
                 return model(**event)
             except ValidationError as err:
                 error = err
-
         raise error
 
     def _validate_event(self, event_str: str) -> Any:
         """Validate a single JSON string event.
 
         Raises:
             TypeError: When the event_str is not of type string.
@@ -71,15 +70,15 @@
             UnknownEventException: When no matching model is found for the event.
             ValidationError: When the event is failing the pydantic model validation.
 
         Returns:
             event_str (str): The cleaned JSON-formatted input event_str.
         """
         event = json.loads(event_str)
-        return self.get_first_valid_model(event).json()
+        return self.get_first_valid_model(event).model_dump_json()
 
     @staticmethod
     def _log_error(
         message: object, event_str: str, error: Optional[BaseException] = None
     ) -> None:
         logger.error(message)
         logger.debug("Raised error: %s, for event : %s", error, event_str)
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/__init__.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/agents.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Base xAPI `Agent` definitions."""
 
 import sys
 from abc import ABC
 from typing import Optional, Union
 
-from pydantic import StrictStr
+from ralph.conf import NonEmptyStrictStr
+from ralph.models.xapi.config import BaseModelWithConfig
 
-from ..config import BaseModelWithConfig
 from .common import IRI
 from .ifi import (
     BaseXapiAccountIFI,
     BaseXapiMboxIFI,
     BaseXapiMboxSha1SumIFI,
     BaseXapiOpenIdIFI,
 )
@@ -26,29 +26,29 @@
 
     Attributes:
         homePage (IRI): Consists of the home page of the account's service provider.
         name (str): Consists of the unique id or name of the Actor's account.
     """
 
     homePage: IRI
-    name: StrictStr
+    name: NonEmptyStrictStr
 
 
 class BaseXapiAgentCommonProperties(BaseModelWithConfig, ABC):
     """Pydantic model for core `Agent` type property.
 
     It defines who performed the action.
 
     Attributes:
         objectType (str): Consists of the value `Agent`.
         name (str): Consists of the full name of the Agent.
     """
 
-    objectType: Optional[Literal["Agent"]]
-    name: Optional[StrictStr]
+    objectType: Literal["Agent"] = "Agent"
+    name: Optional[NonEmptyStrictStr] = None
 
 
 class BaseXapiAgentWithMbox(BaseXapiAgentCommonProperties, BaseXapiMboxIFI):
     """Pydantic model for `Agent` type property.
 
     It is defined for agent type with a mailto IFI.
     """
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/attachments.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/attachments.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         length (int): Consists of the length of the Attachment's data in octets.
         sha2 (str): Consists of the SHA-2 hash of the Attachment data.
         fileUrl (URL): Consists of the URL from which the Attachment can be retrieved.
     """
 
     usageType: IRI
     display: LanguageMap
-    description: Optional[LanguageMap]
+    description: Optional[LanguageMap] = None
     contentType: str
     length: int
     sha2: str
-    fileUrl: Optional[AnyUrl]
+    fileUrl: Optional[AnyUrl] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/common.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 """Common for xAPI base definitions."""
 
-from typing import Dict, Generator, Type
+from typing import Dict, Type, Union
 
 from langcodes import tag_is_valid
-from pydantic import StrictStr, validate_email
+from pydantic import RootModel, model_validator, validate_email
 from rfc3987 import parse
 
+from ralph.conf import NonEmptyStrictStr
 
-class IRI(str):
+
+class IRI(RootModel[Union["IRI", str]]):
     """Pydantic custom data type validating RFC 3987 IRIs."""
 
-    @classmethod
-    def __get_validators__(cls) -> Generator:  # noqa: D105
-        def validate(iri: str) -> Type["IRI"]:
-            """Check whether the provided IRI is a valid RFC 3987 IRI."""
-            parse(iri, rule="IRI")
-            return cls(iri)
+    def __hash__(self):  # noqa: D105
+        return hash(str(self.root))
 
-        yield validate
+    def __str__(self):  # noqa: D105
+        return str(self.root)
 
+    @model_validator(mode="before")
+    @classmethod
+    def validate_iri(cls, iri):
+        """Check whether the provided IRI is a valid RFC 3987 IRI."""
+        parse(str(iri), rule="IRI")
+        return str(iri)
 
-class LanguageTag(str):
+
+class LanguageTag(RootModel[Union[str, "LanguageTag"]]):
     """Pydantic custom data type validating RFC 5646 Language tags."""
 
-    @classmethod
-    def __get_validators__(cls) -> Generator:  # noqa: D105
-        def validate(tag: str) -> Type["LanguageTag"]:
-            """Check whether the provided tag is a valid RFC 5646 Language tag."""
-            if not tag_is_valid(tag):
-                raise TypeError("Invalid RFC 5646 Language tag")
-            return cls(tag)
+    def __hash__(self):  # noqa: D105
+        return hash(str(self.root))
 
-        yield validate
+    def __str__(self):  # noqa: D105
+        return str(self.root)
 
+    @model_validator(mode="before")
+    @classmethod
+    def validate_language_tag(cls, tag):
+        """Check whether the provided tag is a valid RFC 5646 Language tag."""
+        if not tag_is_valid(str(tag)):
+            raise TypeError("Invalid RFC 5646 Language tag")
+        return str(tag)
 
-LanguageMap = Dict[LanguageTag, StrictStr]
 
+LanguageMap = Dict[LanguageTag, NonEmptyStrictStr]
 
-class MailtoEmail(str):
-    """Pydantic custom data type validating `mailto:email` format."""
 
-    @classmethod
-    def __get_validators__(cls) -> Generator:  # noqa: D105
-        def validate(mailto: str) -> Type["MailtoEmail"]:
-            """Check whether the provided value follows the `mailto:email` format."""
-            if not mailto.startswith("mailto:"):
-                raise TypeError("Invalid `mailto:email` value")
-            valid = validate_email(mailto[7:])
-            return cls(f"mailto:{valid[1]}")
+class MailtoEmail(RootModel[str]):
+    """Pydantic custom data type validating `mailto:email` format."""
 
-        yield validate
+    @model_validator(mode="after")
+    def validate(self) -> Type["MailtoEmail"]:
+        """Check whether the provided value follows the `mailto:email` format."""
+        if not self.root.startswith("mailto:"):
+            raise TypeError("Invalid `mailto:email` value")
+        valid = validate_email(self.root[7:])
+        self.root = f"mailto:{valid[1]}"
+        return self
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/contexts.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/contexts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base xAPI `Context` definitions."""
 
 from typing import Dict, List, Optional, Union
 from uuid import UUID
 
-from pydantic import StrictStr
+from ralph.conf import NonEmptyStrictStr
 
 from ..config import BaseModelWithConfig
 from .agents import BaseXapiAgent
 from .common import IRI, LanguageTag
 from .groups import BaseXapiGroup
 from .unnested_objects import BaseXapiActivity, BaseXapiStatementRef
 
@@ -21,18 +21,18 @@
         grouping (dict or list): An Activity with an indirect relation to the
             statement's Activity.
         category (dict or list): An Activity used to categorize the Statement.
         other (dict or list): A contextActivity that doesn't fit one of the other
             properties.
     """
 
-    parent: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]]
-    grouping: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]]
-    category: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]]
-    other: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]]
+    parent: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]] = None
+    grouping: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]] = None
+    category: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]] = None
+    other: Optional[Union[BaseXapiActivity, List[BaseXapiActivity]]] = None
 
 
 class BaseXapiContext(BaseModelWithConfig):
     """Pydantic model for `context` property.
 
     Attributes:
         registration (UUID): The registration that the Statement is associated with.
@@ -42,16 +42,16 @@
         revision (str): The revision of the activity associated with this Statement.
         platform (str): The platform where the learning activity took place.
         language (dict): The language in which the experience occurred.
         statement (dict): Another Statement giving context for this Statement.
         extensions (dict): Consists of a dictionary of other properties as needed.
     """
 
-    registration: Optional[UUID]
-    instructor: Optional[BaseXapiAgent]
-    team: Optional[BaseXapiGroup]
-    contextActivities: Optional[BaseXapiContextContextActivities]
-    revision: Optional[StrictStr]
-    platform: Optional[StrictStr]
-    language: Optional[LanguageTag]
-    statement: Optional[BaseXapiStatementRef]
-    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]]
+    registration: Optional[UUID] = None
+    instructor: Optional[BaseXapiAgent] = None
+    team: Optional[BaseXapiGroup] = None
+    contextActivities: Optional[BaseXapiContextContextActivities] = None
+    revision: Optional[NonEmptyStrictStr] = None
+    platform: Optional[NonEmptyStrictStr] = None
+    language: Optional[LanguageTag] = None
+    statement: Optional[BaseXapiStatementRef] = None
+    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/groups.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Base xAPI `Group` definitions."""
 
 import sys
 from abc import ABC
 from typing import List, Optional, Union
 
-from pydantic import StrictStr
-
 from ..config import BaseModelWithConfig
 from .agents import BaseXapiAgent
 from .ifi import (
     BaseXapiAccountIFI,
     BaseXapiMboxIFI,
     BaseXapiMboxSha1SumIFI,
     BaseXapiOpenIdIFI,
 )
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+from ralph.conf import NonEmptyStrictStr
+
 
 class BaseXapiGroupCommonProperties(BaseModelWithConfig, ABC):
     """Pydantic model for core `Group` type property.
 
     It is defined for the Group which performed the action.
 
     Attributes:
         objectType (str): Consists of the value `Group`.
         name (str): Consists of the full name of the Group.
     """
 
     objectType: Literal["Group"]
-    name: Optional[StrictStr]
+    name: Optional[NonEmptyStrictStr] = None
 
 
 class BaseXapiAnonymousGroup(BaseXapiGroupCommonProperties):
     """Pydantic model for `Group` type property.
 
     It is defined for Anonymous Group type.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/ifi.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/ifi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Base xAPI `Inverse Functional Identifier` definitions."""
 
-from pydantic import AnyUrl, StrictStr, constr
+from pydantic import StringConstraints
+from typing_extensions import Annotated
+
+from ralph.conf import NonEmptyStrictStr
 
 from ..config import BaseModelWithConfig
 from .common import IRI, MailtoEmail
 
 
 class BaseXapiAccount(BaseModelWithConfig):
     """Pydantic model for IFI `account` property.
 
     Attributes:
         homePage (IRI): Consists of the home page of the account's service provider.
         name (str): Consists of the unique id or name of the Actor's account.
     """
 
     homePage: IRI
-    name: StrictStr
+    name: NonEmptyStrictStr
 
 
 class BaseXapiMboxIFI(BaseModelWithConfig):
     """Pydantic model for mailto Inverse Functional Identifier.
 
     Attributes:
         mbox (MailtoEmail): Consists of the Agent's email address.
@@ -31,25 +34,25 @@
 class BaseXapiMboxSha1SumIFI(BaseModelWithConfig):
     """Pydantic model for hash Inverse Functional Identifier.
 
     Attributes:
         mbox_sha1sum (str): Consists of the SHA1 hash of the Agent's email address.
     """
 
-    mbox_sha1sum: constr(regex=r"^[0-9a-f]{40}$")
+    mbox_sha1sum: Annotated[str, StringConstraints(pattern=r"^[0-9a-f]{40}$")]
 
 
 class BaseXapiOpenIdIFI(BaseModelWithConfig):
     """Pydantic model for OpenID Inverse Functional Identifier.
 
     Attributes:
         openid (URI): Consists of an openID that uniquely identifies the Agent.
     """
 
-    openid: AnyUrl
+    openid: str
 
 
 class BaseXapiAccountIFI(BaseModelWithConfig):
     """Pydantic model for account Inverse Functional Identifier.
 
     Attributes:
         account (dict): See BaseXapiAccount.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/objects.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         objectType (dict): Consists of the value `SubStatement`.
     """
 
     actor: Union[BaseXapiAgent, BaseXapiGroup]
     verb: BaseXapiVerb
     object: BaseXapiUnnestedObject
     objectType: Literal["SubStatement"]
-    result: Optional[BaseXapiResult]
-    context: Optional[BaseXapiContext]
-    timestamp: Optional[datetime]
-    attachments: Optional[List[BaseXapiAttachment]]
+    result: Optional[BaseXapiResult] = None
+    context: Optional[BaseXapiContext] = None
+    timestamp: Optional[datetime] = None
+    attachments: Optional[List[BaseXapiAttachment]] = None
 
 
 BaseXapiObject = Union[
     BaseXapiUnnestedObject,
     BaseXapiSubStatement,
     BaseXapiAgent,
     BaseXapiGroup,
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/results.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/results.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Base xAPI `Result` definitions."""
 
 from datetime import timedelta
 from decimal import Decimal
 from typing import Any, Dict, Optional, Union
 
-from pydantic import StrictBool, StrictStr, conint, root_validator
+from pydantic import Field, StrictBool, model_validator
+from typing_extensions import Annotated
+
+from ralph.conf import NonEmptyStrictStr
 
 from ..config import BaseModelWithConfig
 from .common import IRI
 
 
 class BaseXapiResultScore(BaseModelWithConfig):
     """Pydantic model for result `score` property.
@@ -16,37 +19,31 @@
     Attributes:
         scaled (int): Consists of the normalized score related to the experience.
         raw (Decimal): Consists of the non-normalized score achieved by the Actor.
         min (Decimal): Consists of the lowest possible score.
         max (Decimal): Consists of the highest possible score.
     """
 
-    scaled: Optional[conint(ge=-1, le=1)]
-    raw: Optional[Decimal]
-    min: Optional[Decimal]
-    max: Optional[Decimal]
-
-    @root_validator
-    @classmethod
-    def check_raw_min_max_relation(cls, values: Any) -> Any:
-        """Check the relationship `min < raw < max`."""
-        raw_value = values.get("raw", None)
-        min_value = values.get("min", None)
-        max_value = values.get("max", None)
+    scaled: Optional[Annotated[int, Field(ge=-1, le=1)]] = None
+    raw: Optional[Decimal] = None
+    min: Optional[Decimal] = None
+    max: Optional[Decimal] = None
 
-        if min_value:
-            if max_value and min_value > max_value:
+    @model_validator(mode="after")
+    def check_raw_min_max_relation(self) -> Any:
+        """Check the relationship `min < raw < max`."""
+        if self.min:
+            if self.max and self.min > self.max:
                 raise ValueError("min cannot be greater than max")
-            if raw_value and min_value > raw_value:
+            if self.raw and self.min > self.raw:
                 raise ValueError("min cannot be greater than raw")
-        if max_value:
-            if raw_value and raw_value > max_value:
+        if self.max:
+            if self.raw and self.raw > self.max:
                 raise ValueError("raw cannot be greater than max")
-
-        return values
+        return self
 
 
 class BaseXapiResult(BaseModelWithConfig):
     """Pydantic model for `result` property.
 
     Attributes:
         score (dict): See BaseXapiResultScore.
@@ -54,13 +51,13 @@
         completion (bool): Indicates whether the Activity was completed.
         response (str): Consists of the response for the given Activity.
         duration (timedelta): Consists of the duration over which the Statement
             occurred.
         extensions (dict): Consists of a dictionary of other properties as needed.
     """
 
-    score: Optional[BaseXapiResultScore]
-    success: Optional[StrictBool]
-    completion: Optional[StrictBool]
-    response: Optional[StrictStr]
-    duration: Optional[timedelta]
-    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]]
+    score: Optional[BaseXapiResultScore] = None
+    success: Optional[StrictBool] = None
+    completion: Optional[StrictBool] = None
+    response: Optional[NonEmptyStrictStr] = None
+    duration: Optional[timedelta] = None
+    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/statements.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/statements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base xAPI `Statement` definitions."""
 
 from datetime import datetime
 from typing import Any, List, Optional, Union
 from uuid import UUID
 
-from pydantic import constr, root_validator
+from pydantic import StringConstraints, model_validator
+from typing_extensions import Annotated
 
 from ..config import BaseModelWithConfig
 from .agents import BaseXapiAgent
 from .attachments import BaseXapiAttachment
 from .contexts import BaseXapiContext
 from .groups import BaseXapiGroup
 from .objects import BaseXapiObject
@@ -29,27 +30,27 @@
         timestamp (datetime): Consists of the timestamp of when the event occurred.
         stored (datetime): Consists of the timestamp of when the event was recorded.
         authority (dict): Consists of the Actor asserting this Statement is true.
         version (str): Consists of the associated xAPI version of the Statement.
         attachments (list): Consists of a list of attachments.
     """
 
-    id: Optional[UUID]
+    id: Optional[UUID] = None
     actor: Union[BaseXapiAgent, BaseXapiGroup]
     verb: BaseXapiVerb
     object: BaseXapiObject
-    result: Optional[BaseXapiResult]
-    context: Optional[BaseXapiContext]
-    timestamp: Optional[datetime]
-    stored: Optional[datetime]
-    authority: Optional[Union[BaseXapiAgent, BaseXapiGroup]]
-    version: constr(regex=r"^1\.0\.[0-9]+$") = "1.0.0"
-    attachments: Optional[List[BaseXapiAttachment]]
+    result: Optional[BaseXapiResult] = None
+    context: Optional[BaseXapiContext] = None
+    timestamp: Optional[datetime] = None
+    stored: Optional[datetime] = None
+    authority: Optional[Union[BaseXapiAgent, BaseXapiGroup]] = None
+    version: Annotated[str, StringConstraints(pattern=r"^1\.0\.[0-9]+$")] = "1.0.0"
+    attachments: Optional[List[BaseXapiAttachment]] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
     def check_absence_of_empty_and_invalid_values(cls, values: Any) -> Any:
         """Check the model for empty and invalid values.
 
         Check that the `context` field contains `platform` and `revision` fields
         only if the `object.objectType` property is equal to `Activity`.
         """
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/base/unnested_objects.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/base/unnested_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 """Base xAPI `Object` definitions (1)."""
 
-import sys
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import AnyUrl, StrictStr, constr, validator
+from pydantic import AnyUrl, StringConstraints, field_validator
+from typing_extensions import Annotated
+
+from ralph.conf import NonEmptyStrictStr
 
 from ..config import BaseModelWithConfig
 from .common import IRI, LanguageMap
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 
 class BaseXapiActivityDefinition(BaseModelWithConfig):
     """Pydantic model for `Activity` type `definition` property.
 
     Attributes:
         name (LanguageMap): Consists of the human-readable/visual name of the Activity.
         description (LanguageMap): Consists of a description of the Activity.
         type (IRI): Consists of the type of the Activity.
         moreInfo (URL): Consists of an URL to a document about the Activity.
         extensions (dict): Consists of a dictionary of other properties as needed.
     """
 
-    name: Optional[LanguageMap]
-    description: Optional[LanguageMap]
-    type: Optional[IRI]
-    moreInfo: Optional[AnyUrl]
-    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]]
+    name: Optional[LanguageMap] = None
+    description: Optional[LanguageMap] = None
+    type: Optional[IRI] = None
+    moreInfo: Optional[AnyUrl] = None
+    extensions: Optional[Dict[IRI, Union[str, int, bool, list, dict, None]]] = None
 
 
 class BaseXapiInteractionComponent(BaseModelWithConfig):
     """Pydantic model for an interaction component.
 
     Attributes:
         id (str): Consists of an identifier of the interaction component.
         description (LanguageMap): Consists of the description of the interaction.
     """
 
-    id: constr(regex=r"^[^\s]+$")
-    description: Optional[LanguageMap]
+    id: Annotated[str, StringConstraints(pattern=r"^[^\s]+$")]
+    description: Optional[LanguageMap] = None
 
 
 class BaseXapiActivityInteractionDefinition(BaseXapiActivityDefinition):
     """Pydantic model for `Activity` type `definition` property.
 
     It is defined for field with interaction properties.
 
@@ -68,47 +65,47 @@
         "matching",
         "performance",
         "sequencing",
         "likert",
         "numeric",
         "other",
     ]
-    correctResponsesPattern: Optional[List[StrictStr]]
-    choices: Optional[List[BaseXapiInteractionComponent]]
-    scale: Optional[List[BaseXapiInteractionComponent]]
-    source: Optional[List[BaseXapiInteractionComponent]]
-    target: Optional[List[BaseXapiInteractionComponent]]
-    steps: Optional[List[BaseXapiInteractionComponent]]
+    correctResponsesPattern: Optional[List[NonEmptyStrictStr]] = None
+    choices: Optional[List[BaseXapiInteractionComponent]] = None
+    scale: Optional[List[BaseXapiInteractionComponent]] = None
+    source: Optional[List[BaseXapiInteractionComponent]] = None
+    target: Optional[List[BaseXapiInteractionComponent]] = None
+    steps: Optional[List[BaseXapiInteractionComponent]] = None
 
-    @validator("choices", "scale", "source", "target", "steps")
+    @field_validator("choices", "scale", "source", "target", "steps", mode="after")
     @classmethod
-    def check_unique_ids(cls, value: Any) -> None:
+    def check_unique_ids(cls, value: Optional[List[Any]]) -> None:
         """Check the uniqueness of interaction components IDs."""
-        if len(value) != len({x.id for x in value}):
+        if value and (len(value) != len({x.id for x in value if x})):
             raise ValueError("Duplicate InteractionComponents are not valid")
 
 
 class BaseXapiActivity(BaseModelWithConfig):
     """Pydantic model for `Activity` type property.
 
     Attributes:
         id (IRI): Consists of an identifier for a single unique Activity.
         objectType (str): Consists of the value `Activity`.
         definition (dict): See BaseXapiActivityDefinition and
             BaseXapiActivityInteractionDefinition.
     """
 
     id: IRI
-    objectType: Optional[Literal["Activity"]]
+    objectType: Optional[Literal["Activity"]] = None
     definition: Optional[
         Union[
             BaseXapiActivityDefinition,
             BaseXapiActivityInteractionDefinition,
         ]
-    ]
+    ] = None
 
 
 class BaseXapiStatementRef(BaseModelWithConfig):
     """Pydantic model for `StatementRef` type property.
 
     Attributes:
         objectType (str): Consists of the value `StatementRef`.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,17 @@
     """Pydantic model for webpage `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `https://w3id.org/xapi/acrossx/activities/webpage`.
     """
 
-    type: Literal["https://w3id.org/xapi/acrossx/activities/webpage"]
+    type: Literal["https://w3id.org/xapi/acrossx/activities/webpage"] = (
+        "https://w3id.org/xapi/acrossx/activities/webpage"
+    )
 
 
 class WebpageActivity(BaseXapiActivity):
     """Pydantic model for webpage `Activity` type.
 
     Attributes:
         definition (dict): see WebpageActivityDefinition.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 class FileActivityDefinition(BaseXapiActivityDefinition):
     """Pydantic model for file `Activity` type `definition` property.
 
     Attributes:
        type (str): Consists of the value `http://activitystrea.ms/file`.
     """
 
-    type: Literal["http://activitystrea.ms/file"]
+    type: Literal["http://activitystrea.ms/file"] = "http://activitystrea.ms/file"
 
 
 class FileActivity(BaseXapiActivity):
     """Pydantic model for file `Activity` type.
 
     Attributes:
         definition (dict): See FileActivityDefinition.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/audio.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/audio.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     """Pydantic model for audio `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
             `https://w3id.org/xapi/audio/activity-type/audio`.
     """
 
-    type: Literal["https://w3id.org/xapi/audio/activity-type/audio"]
+    type: Literal["https://w3id.org/xapi/audio/activity-type/audio"] = (
+        "https://w3id.org/xapi/audio/activity-type/audio"
+    )
 
 
 class AudioActivity(BaseXapiActivity):
     """Pydantic model for audio `Activity` type.
 
     Attributes:
         name (dict): Consists of the dictionary `{"en-US": <name of the audio>}`.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/tincan_vocabulary.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-"""`Scorm Profile` activity types definitions."""
+"""`Virtual classroom` activity types definitions."""
 
 import sys
 
 from ...base.unnested_objects import BaseXapiActivity, BaseXapiActivityDefinition
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
-# Document
+# Virtual classroom
 
 
-class DocumentActivityDefinition(BaseXapiActivityDefinition):
-    """Pydantic model for document `Activity` type `definition` property.
+class VirtualClassroomActivityDefinition(BaseXapiActivityDefinition):
+    """Pydantic model for virtual classroom `Activity` type `definition` property.
 
     Attributes:
         type (str): Consists of the value
-            `http://id.tincanapi.com/activitytype/document`.
+            `https://w3id.org/xapi/virtual-classroom/activity-types/virtual-classroom`.
     """
 
-    type: Literal["http://id.tincanapi.com/activitytype/document"]
+    type: Literal[
+        "https://w3id.org/xapi/virtual-classroom/activity-types/virtual-classroom"
+    ] = "https://w3id.org/xapi/virtual-classroom/activity-types/virtual-classroom"
 
 
-class DocumentActivity(BaseXapiActivity):
-    """Pydantic model for document `Activity` type.
+class VirtualClassroomActivity(BaseXapiActivity):
+    """Pydantic model for virtual classroom `Activity` type.
 
     Attributes:
-        definition (dict): see DocumentActivityDefinition.
+        definition (dict): See VirtualClassroomActivityDefinition.
     """
 
-    definition: DocumentActivityDefinition
+    definition: VirtualClassroomActivityDefinition = (
+        VirtualClassroomActivityDefinition()
+    )
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/activity_types/video.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/activity_types/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/constants/video.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/constants/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         id (str): Consists of the value `https://w3id.org/xapi/acrossx/verbs/posted`.
         display (dict): Consists of the dictionary `{"en-US": "posted"}`.
     """
 
     id: Literal["https://w3id.org/xapi/acrossx/verbs/posted"] = (
         "https://w3id.org/xapi/acrossx/verbs/posted"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["posted"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["posted"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
     Attributes:
         id (str): Consists of the value `http://activitystrea.ms/join`.
         display (dict): Consists of the dictionary `{"en-US": "joined"}`.
     """
 
     id: Literal["http://activitystrea.ms/join"] = "http://activitystrea.ms/join"
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["joined"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["joined"]]] = None
 
 
 class LeaveVerb(BaseXapiVerb):
     """Pydantic model for leave `verb`.
 
     Attributes:
         id (str): Consists of the value `http://activitystrea.ms/leave`.
         display (dict): Consists of the dictionary `{"en-US": "left"}`.
     """
 
     id: Literal["http://activitystrea.ms/leave"] = "http://activitystrea.ms/leave"
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["left"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["left"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,36 +19,36 @@
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/asked`.
         display (dict): Consists of the dictionary `{"en-US": "asked"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/asked"] = (
         "http://adlnet.gov/expapi/verbs/asked"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["asked"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["asked"]]] = None
 
 
 class AnsweredVerb(BaseXapiVerb):
     """Pydantic model for answered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/answered`.
         display (dict): Consists of the dictionary `{"en-US": "answered"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/answered"] = (
         "http://adlnet.gov/expapi/verbs/answered"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["answered"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["answered"]]] = None
 
 
 class RegisteredVerb(BaseXapiVerb):
     """Pydantic model for registered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/registered`.
         display (dict): Consists of the dictionary `{"en-US": "registered"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/registered"] = (
         "http://adlnet.gov/expapi/verbs/registered"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["registered"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["registered"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/navy_common_reference_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,22 @@
         id (str): Consists of the value `https://w3id.org/xapi/netc/verbs/accessed`.
         display (dict): Consists of the dictionary `{"en-US": "accessed"}`.
     """
 
     id: Literal["https://w3id.org/xapi/netc/verbs/accessed"] = (
         "https://w3id.org/xapi/netc/verbs/accessed"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["accessed"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["accessed"]]] = None
 
 
 class UploadedVerb(BaseXapiVerb):
     """Pydantic model for uploaded `verb`.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/netc/verbs/uploaded`.
         display (dict): Consists of the dictionary `{"en-US": "uploaded"}`.
     """
 
     id: Literal["https://w3id.org/xapi/netc/verbs/uploaded"] = (
         "https://w3id.org/xapi/netc/verbs/uploaded"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["uploaded"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["uploaded"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,50 +19,50 @@
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/completed`.
         display (dict): Consists of the dictionary `{"en-US": "completed"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/completed"] = (
         "http://adlnet.gov/expapi/verbs/completed"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["completed"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["completed"]]] = None
 
 
 class InitializedVerb(BaseXapiVerb):
     """Pydantic model for initialized `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/initialized`.
         display (Dict): Consists of the dictionary `{"en-US": "initialized"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/initialized"] = (
         "http://adlnet.gov/expapi/verbs/initialized"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["initialized"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["initialized"]]] = None
 
 
 class InteractedVerb(BaseXapiVerb):
     """Pydantic model for interacted `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/interacted`.
         display (dict): Consists of the dictionary `{"en-US": "interacted"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/interacted"] = (
         "http://adlnet.gov/expapi/verbs/interacted"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["interacted"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["interacted"]]] = None
 
 
 class TerminatedVerb(BaseXapiVerb):
     """Pydantic model for terminated `verb`.
 
     Attributes:
         id (str): Consists of the value `http://adlnet.gov/expapi/verbs/terminated`.
         display (dict): Consists of the dictionary `{"en-US": "terminated"}`.
     """
 
     id: Literal["http://adlnet.gov/expapi/verbs/terminated"] = (
         "http://adlnet.gov/expapi/verbs/terminated"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["terminated"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["terminated"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,36 +19,36 @@
         id (str): Consists of the value `http://id.tincanapi.com/verb/viewed`.
         display (dict): Consists of the dictionary `{"en-US": "viewed"}`.
     """
 
     id: Literal["http://id.tincanapi.com/verb/viewed"] = (
         "http://id.tincanapi.com/verb/viewed"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["viewed"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["viewed"]]] = None
 
 
 class DownloadedVerb(BaseXapiVerb):
     """Pydantic model for downloaded `verb`.
 
     Attributes:
         id (str): Consists of the value `http://id.tincanapi.com/verb/downloaded`.
         display (dict): Consists of the dictionary `{"en-US": "downloaded"}`.
     """
 
     id: Literal["http://id.tincanapi.com/verb/downloaded"] = (
         "http://id.tincanapi.com/verb/downloaded"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["downloaded"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["downloaded"]]] = None
 
 
 class UnregisteredVerb(BaseXapiVerb):
     """Pydantic model for unregistered `verb`.
 
     Attributes:
         id (str): Consists of the value `http://id.tincanapi.com/verb/unregistered`.
         display (dict): Consists of the dictionary `{"en-US": "unregistered"}`.
     """
 
     id: Literal["http://id.tincanapi.com/verb/unregistered"] = (
         "http://id.tincanapi.com/verb/unregistered"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unregistered"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unregistered"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/video.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,36 +19,36 @@
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/played`.
         display (dict): Consists of the dictionary `{"en-US": "played"}`.
     """
 
     id: Literal["https://w3id.org/xapi/video/verbs/played"] = (
         "https://w3id.org/xapi/video/verbs/played"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["played"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["played"]]] = None
 
 
 class PausedVerb(BaseXapiVerb):
     """Pydantic model for paused `verb` field.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/paused`.
         display (dict): Consists of the dictionary `{"en-US": "paused"}`.
     """
 
     id: Literal["https://w3id.org/xapi/video/verbs/paused"] = (
         "https://w3id.org/xapi/video/verbs/paused"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["paused"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["paused"]]] = None
 
 
 class SeekedVerb(BaseXapiVerb):
     """Pydantic model for seeked `verb` field.
 
     Attributes:
         id (str): Consists of the value `https://w3id.org/xapi/video/verbs/seeked`.
         display (dict): Consists of the dictionary `{"en-US": "seeked"}`.
     """
 
     id: Literal["https://w3id.org/xapi/video/verbs/seeked"] = (
         "https://w3id.org/xapi/video/verbs/seeked"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["seeked"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["seeked"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,113 +20,121 @@
             `https://w3id.org/xapi/virtual-classroom/verbs/muted`.
         display (dict): Consists of the dictionary `{"en-US": "muted"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/muted"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/muted"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["muted"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["muted"]]] = None
 
 
 class UnmutedVerb(BaseXapiVerb):
     """Pydantic model for unmuted `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/unmuted`.
         display (dict): Consists of the dictionary `{"en-US": "unmuted"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/unmuted"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/unmuted"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unmuted"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unmuted"]]] = None
 
 
 class StartedCameraVerb(BaseXapiVerb):
     """Pydantic model for started camera `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/started-camera`.
         display (dict): Consists of the dictionary `{"en-US": "started camera"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/started-camera"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/started-camera"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["started camera"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["started camera"]]] = (
+        None
+    )
 
 
 class StoppedCameraVerb(BaseXapiVerb):
     """Pydantic model for stopped camera `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera`.
         display (dict): Consists of the dictionary `{"en-US": "stopped camera"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/stopped-camera"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["stopped camera"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["stopped camera"]]] = (
+        None
+    )
 
 
 class SharedScreenVerb(BaseXapiVerb):
     """Pydantic model for shared screen `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/shared-screen`.
         display (dict): Consists of the dictionary `{"en-US": "shared screen"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/shared-screen"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/shared-screen"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["shared screen"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["shared screen"]]] = (
+        None
+    )
 
 
 class UnsharedScreenVerb(BaseXapiVerb):
     """Pydantic model for unshared screen `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen`.
         display (dict): Consists of the dictionary `{"en-US": "unshared screen"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/unshared-screen"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unshared screen"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["unshared screen"]]] = (
+        None
+    )
 
 
 class RaisedHandVerb(BaseXapiVerb):
     """Pydantic model for raised hand `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/raised-hand`.
         display (dict): Consists of the dictionary `{"en-US": "raised hand"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/raised-hand"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/raised-hand"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["raised hand"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["raised hand"]]] = None
 
 
 class LoweredHandVerb(BaseXapiVerb):
     """Pydantic model for lowered hand `verb`.
 
     Attributes:
         id (str): Consists of the value
             `https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand`.
         display (dict): Consists of the dictionary `{"en-US": "lowered hand"}`.
     """
 
     id: Literal["https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand"] = (
         "https://w3id.org/xapi/virtual-classroom/verbs/lowered-hand"
     )
-    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["lowered hand"]]]
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["lowered hand"]]] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/lms/contexts.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/lms/contexts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """LMS xAPI events context fields definitions."""
 
 import sys
 from datetime import datetime
 from typing import List, Optional, Union
 from uuid import UUID
 
-from pydantic import Field, NonNegativeFloat, PositiveInt, condecimal, validator
+from pydantic import Field, NonNegativeFloat, PositiveInt, condecimal, field_validator
+from typing_extensions import Annotated
 
 from ..base.contexts import BaseXapiContext, BaseXapiContextContextActivities
 from ..base.unnested_objects import BaseXapiActivity
 from ..concepts.activity_types.scorm_profile import ProfileActivity
 from ..concepts.constants.cmi5_profile import CONTEXT_EXTENSION_SESSION_ID
 from ..concepts.constants.lms import (
     CONTEXT_EXTENSION_ENDING_DATE,
@@ -45,15 +46,15 @@
         category (dict or list): see LMSProfileActivity.
     """
 
     category: Union[
         LMSProfileActivity, List[Union[LMSProfileActivity, BaseXapiActivity]]
     ]
 
-    @validator("category")
+    @field_validator("category")
     @classmethod
     def check_presence_of_profile_activity_category(
         cls,
         value: Union[
             LMSProfileActivity, List[Union[LMSProfileActivity, BaseXapiActivity]]
         ],
     ) -> Union[LMSProfileActivity, List[Union[LMSProfileActivity, BaseXapiActivity]]]:
@@ -90,92 +91,103 @@
             the normal format of ISO 8601.
         ending_date (datetime): Ending date of the activity, formatted according to the
             normal format of ISO 8601.
         role (str): Role of the actor. For example: `admin`, `manager`, `teacher`,
             `guest`, `learner` or `staff`.
     """
 
-    starting_date: Optional[datetime] = Field(alias=CONTEXT_EXTENSION_STARTING_DATE)
-    ending_date: Optional[datetime] = Field(alias=CONTEXT_EXTENSION_ENDING_DATE)
-    role: Optional[str] = Field(alias=CONTEXT_EXTENSION_ROLE)
+    starting_date: Annotated[
+        Optional[datetime], Field(alias=CONTEXT_EXTENSION_STARTING_DATE)
+    ] = None
+    ending_date: Annotated[
+        Optional[datetime], Field(alias=CONTEXT_EXTENSION_ENDING_DATE)
+    ] = None
+    role: Annotated[Optional[str], Field(alias=CONTEXT_EXTENSION_ROLE)]
 
 
 class LMSRegistrationContext(LMSContext):
     """Pydantic model for LMS registration statements `context` property.
 
     This model is used for `registered to a course` and
     `unregistered to a course` statement templates.
 
     Attributes:
         extensions (dict): see LMSRegistrationContextExtensions.
     """
 
-    extensions: Optional[LMSRegistrationContextExtensions]
+    extensions: Optional[LMSRegistrationContextExtensions] = None
 
 
 class LMSCommonContextExtensions(BaseExtensionModelWithConfig):
     """Pydantic model for common LMS statements `context`.`extensions` property.
 
     This model is used for `downloaded a video`, `downloaded a document`,
     `downloaded an audio`, `downloaded a file`,  `uploaded a video`,
     `uploaded a document` and `uploaded an audio`, `uploaded a file`
     statement templates.
 
     Attributes:
         session_id (uuid): ID of the active session.
     """
 
-    session_id: Optional[UUID] = Field(alias=CONTEXT_EXTENSION_SESSION_ID)
+    session_id: Annotated[Optional[UUID], Field(alias=CONTEXT_EXTENSION_SESSION_ID)] = (
+        None
+    )
 
 
 class LMSCommonContext(LMSContext):
     """Pydantic model for LMS common `context` property.
 
     Attributes:
         extensions (dict): See LMSCommonContextExtensions.
     """
 
-    extensions: Optional[LMSCommonContextExtensions]
+    extensions: Optional[LMSCommonContextExtensions] = None
 
 
 class LMSDownloadedVideoContextExtensions(LMSCommonContextExtensions):
     """Pydantic model for LMS downloaded video `context`.`extensions` property.
 
     Attributes:
         length (float): Length of the video.
         quality (int): Video resolution or quality of the video.
     """
 
-    length: Optional[condecimal(ge=0, decimal_places=3)] = Field(
-        alias=CONTEXT_EXTENSION_LENGTH
-    )
-    quality: Optional[PositiveInt] = Field(alias=CONTEXT_EXTENSION_QUALITY)
+    length: Annotated[
+        Optional[condecimal(ge=0, decimal_places=3)],
+        Field(alias=CONTEXT_EXTENSION_LENGTH),
+    ] = None
+    quality: Annotated[
+        Optional[PositiveInt], Field(alias=CONTEXT_EXTENSION_QUALITY)
+    ] = None
 
 
 class LMSDownloadedVideoContext(LMSContext):
     """Pydantic model for LMS downloaded video `context` property.
 
     Attributes:
         extensions (dict): See LMSDownloadedVideoContextExtensions.
     """
 
-    extensions: Optional[LMSDownloadedVideoContextExtensions]
+    extensions: Optional[LMSDownloadedVideoContextExtensions] = None
 
 
 class LMSDownloadedAudioContextExtensions(LMSCommonContextExtensions):
     """Pydantic model for LMS downloaded audio `context`.`extensions` property.
 
     Attributes:
         length (float): Length of the audio.
     """
 
-    length: Optional[NonNegativeFloat] = Field(alias=CONTEXT_EXTENSION_LENGTH)
+    length: Annotated[
+        Optional[NonNegativeFloat], Field(alias=CONTEXT_EXTENSION_LENGTH)
+    ] = None
 
 
 class LMSDownloadedAudioContext(LMSContext):
     """Pydantic model for LMS downloaded audio `context` property.
 
     Attributes:
         extensions (dict): See LMSDownloadedAudioContextExtensions.
     """
 
-    extensions: Optional[LMSDownloadedAudioContextExtensions]
+    extensions: Optional[LMSDownloadedAudioContextExtensions] = None
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/lms/objects.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/lms/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """LMS xAPI events object fields definitions."""
 
 import sys
 from typing import Optional
 
 from pydantic import Field
+from typing_extensions import Annotated
 
 from ..concepts.activity_types.acrossx_profile import (
     WebpageActivity,
     WebpageActivityDefinition,
 )
 from ..concepts.activity_types.activity_streams_vocabulary import (
     FileActivity,
@@ -29,27 +30,28 @@
     """Pydantic model for LMS page `object`.`definition`.`extensions` property.
 
     Attributes:
         type (str): Characterisation of the page. Can be either `course`,
             `course_list`, `user_space` value.
     """
 
-    type: Optional[Literal["course", "course_list", "user_space"]] = Field(
-        alias=ACTIVITY_EXTENSIONS_TYPE
-    )
+    type: Annotated[
+        Optional[Literal["course", "course_list", "user_space"]],
+        Field(alias=ACTIVITY_EXTENSIONS_TYPE),
+    ] = None
 
 
 class LMSPageObjectDefinition(WebpageActivityDefinition):
     """Pydantic model for LMS page `object`.`definition` property.
 
     Attributes:
         extensions (dict): see LMSPageObjectDefinitionExtensions.
     """
 
-    extensions: Optional[LMSPageObjectDefinitionExtensions]
+    extensions: Optional[LMSPageObjectDefinitionExtensions] = None
 
 
 class LMSPageObject(WebpageActivity):
     """Pydantic model for LMS page `object` property.
 
     Attributes:
         definition (dict): see LMSPageObjectDefinition.
@@ -64,25 +66,25 @@
 class LMSFileObjectDefinitionExtensions(BaseExtensionModelWithConfig):
     """Pydantic model for LMS file `object`.`definition`.`extensions` property.
 
     Attributes:
         type (str): Characterisation of the MIME type of the file.
     """
 
-    type: str = Field(alias=ACTIVITY_EXTENSIONS_TYPE)
+    type: Annotated[str, Field(alias=ACTIVITY_EXTENSIONS_TYPE)]
 
 
 class LMSFileObjectDefinition(FileActivityDefinition):
     """Pydantic model for LMS file `object`.`definition` property.
 
     Attributes:
         extensions (dict): see LMSFileObjectDefinitionExtensions.
     """
 
-    extensions: Optional[LMSFileObjectDefinitionExtensions]
+    extensions: Optional[LMSFileObjectDefinitionExtensions] = None
 
 
 class LMSFileObject(FileActivity):
     """Pydantic model for LMS file `object` property.
 
     Attributes:
         definition (dict): see LMSFileObjectDefinition.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/lms/statements.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/lms/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/video/contexts.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/video/contexts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Video xAPI events context fields definitions."""
 
 import sys
 from typing import List, Optional, Union
 from uuid import UUID
 
-from pydantic import Field, NonNegativeFloat, validator
+from pydantic import Field, NonNegativeFloat, field_validator
+from typing_extensions import Annotated
 
 from ..base.contexts import BaseXapiContext, BaseXapiContextContextActivities
 from ..base.unnested_objects import BaseXapiActivity
 from ..concepts.activity_types.scorm_profile import ProfileActivity
 from ..concepts.constants.video import (
     CONTEXT_EXTENSION_CC_ENABLED,
     CONTEXT_EXTENSION_CC_SUBTITLE_LANG,
@@ -47,15 +48,15 @@
         category (dict or list): see VideoProfileActivity.
     """
 
     category: Union[
         VideoProfileActivity, List[Union[VideoProfileActivity, BaseXapiActivity]]
     ]
 
-    @validator("category")
+    @field_validator("category")
     @classmethod
     def check_presence_of_profile_activity_category(
         cls,
         value: Union[
             VideoProfileActivity, List[Union[VideoProfileActivity, BaseXapiActivity]]
         ],
     ) -> Union[
@@ -86,15 +87,15 @@
 class VideoContextExtensions(BaseExtensionModelWithConfig):
     """Pydantic model for video core context `extensions` property.
 
     Attributes:
         session (uuid): Consists of the ID of the active session.
     """
 
-    session_id: Optional[UUID] = Field(alias=CONTEXT_EXTENSION_SESSION_ID)
+    session_id: Annotated[Optional[UUID], Field(alias=CONTEXT_EXTENSION_SESSION_ID)]
 
 
 class VideoInitializedContextExtensions(VideoContextExtensions):
     """Pydantic model for video initialized `context` `extensions` property.
 
     Attributes:
         length (float): Consists of the length of the video.
@@ -111,83 +112,95 @@
         userAgent (str): Consists of the User Agent string of the browser,
             if the video is launched in browser.
         volume (int): Consists of the volume of the video.
         completionThreshold (float): Consists of the percentage of media that should be
             consumed to trigger a completion.
     """
 
-    length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
-    ccSubtitleEnabled: Optional[bool] = Field(alias=CONTEXT_EXTENSION_CC_ENABLED)
-    ccSubtitleLang: Optional[str] = Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)
-    fullScreen: Optional[bool] = Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)
-    screenSize: Optional[str] = Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)
-    videoPlaybackSize: Optional[str] = Field(
-        alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE
+    length: Annotated[NonNegativeFloat, Field(alias=CONTEXT_EXTENSION_LENGTH)]
+    ccSubtitleEnabled: Annotated[
+        Optional[bool], Field(alias=CONTEXT_EXTENSION_CC_ENABLED)
+    ] = None
+    ccSubtitleLang: Annotated[
+        Optional[str], Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)
+    ] = None
+    fullScreen: Annotated[
+        Optional[bool], Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)
+    ] = None
+    screenSize: Annotated[Optional[str], Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)] = (
+        None
     )
-    speed: Optional[str] = Field(alias=CONTEXT_EXTENSION_SPEED)
-    userAgent: Optional[str] = Field(alias=CONTEXT_EXTENSION_USER_AGENT)
-    volume: Optional[int] = Field(alias=CONTEXT_EXTENSION_VOLUME)
-    completionThreshold: Optional[float] = Field(
-        alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD
+    videoPlaybackSize: Annotated[
+        Optional[str], Field(alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE)
+    ] = None
+    speed: Annotated[Optional[str], Field(alias=CONTEXT_EXTENSION_SPEED)] = None
+    userAgent: Annotated[Optional[str], Field(alias=CONTEXT_EXTENSION_USER_AGENT)] = (
+        None
     )
+    volume: Annotated[Optional[int], Field(alias=CONTEXT_EXTENSION_VOLUME)] = None
+    completionThreshold: Annotated[
+        Optional[float], Field(alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD)
+    ] = None
 
 
 class VideoBrowsingContextExtensions(VideoContextExtensions):
     """Pydantic model for video browsing `context`.`extensions` property.
 
     Such field is used in `paused`, `completed` and `terminated` events.
 
     Attributes:
         completionThreshold (float): Consists of the percentage of media that should
             be consumed to trigger a completion.
         length (float): Consists of the length of the video.
     """
 
-    length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
-    completionThreshold: Optional[float] = Field(
-        alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD
-    )
+    length: Annotated[NonNegativeFloat, Field(alias=CONTEXT_EXTENSION_LENGTH)]
+    completionThreshold: Annotated[
+        Optional[float], Field(alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD)
+    ] = None
 
 
 class VideoEnableClosedCaptioningContextExtensions(VideoContextExtensions):
     """Represents the context.extensions field for video `interacted` xAPI statement.
 
     Attributes:
         ccSubtitleLanguage (str): Consists of the language of subtitle or closed
             captioning.
     """
 
-    ccSubtitleLanguage: str = Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)
+    ccSubtitleLanguage: Annotated[str, Field(alias=CONTEXT_EXTENSION_CC_SUBTITLE_LANG)]
 
 
 class VideoVolumeChangeInteractionContextExtensions(VideoContextExtensions):
     """Pydantic model for video volume change interaction `context`.`extensions`
     property.
 
     Attributes:
         volume (int): Consists of the volume of the video.
     """  # noqa: D205
 
-    volume: int = Field(alias=CONTEXT_EXTENSION_VOLUME)
+    volume: Annotated[int, Field(alias=CONTEXT_EXTENSION_VOLUME)]
 
 
 class VideoScreenChangeInteractionContextExtensions(VideoContextExtensions):
     """Pydantic model for video screen change interaction `context`.`extensions`
     property.
 
     Attributes:
         fullScreen (bool): Indicates whether the video is played in full screen mode.
         screenSize (str): Expresses the total available screen size for Video playback.
         videoPlaybackSize (str): Consists of the size in Width x Height of the video as
             viewed by the user.
     """  # noqa: D205
 
-    fullScreen: bool = Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)
-    screenSize: str = Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)
-    videoPlaybackSize: str = Field(alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE)
+    fullScreen: Annotated[bool, Field(alias=CONTEXT_EXTENSION_FULL_SCREEN)]
+    screenSize: Annotated[str, Field(alias=CONTEXT_EXTENSION_SCREEN_SIZE)]
+    videoPlaybackSize: Annotated[
+        str, Field(alias=CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE)
+    ]
 
 
 class VideoInitializedContext(BaseVideoContext):
     """Pydantic model for video initialized `context` property.
 
     Attributes:
         extensions (dict): See VideoInitializedContextExtensions.
@@ -199,15 +212,15 @@
 class VideoPlayedContext(BaseVideoContext):
     """Pydantic model for video played `context` property.
 
     Attributes:
         extensions (dict): See VideoContextExtensions.
     """
 
-    extensions: Optional[VideoContextExtensions]
+    extensions: Optional[VideoContextExtensions] = None
 
 
 class VideoPausedContext(BaseVideoContext):
     """Pydantic model for video paused `context` property.
 
     Attributes:
         extensions (dict): See VideoBrowsingContextExtensions.
@@ -219,15 +232,15 @@
 class VideoSeekedContext(BaseVideoContext):
     """Pydantic model for video seeked `context` property.
 
     Attributes:
         extensions (dict): See VideoContextExtensions.
     """
 
-    extensions: Optional[VideoContextExtensions]
+    extensions: Optional[VideoContextExtensions] = None
 
 
 class VideoCompletedContext(BaseVideoContext):
     """Pydantic model for video completed `context` property.
 
     Attributes:
         extensions (dict): See VideoBrowsingContextExtensions.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/video/results.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/video/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Video xAPI events result fields definitions."""
 
 import sys
 from datetime import timedelta
 from typing import Optional
 
 from pydantic import Field, NonNegativeFloat
+from typing_extensions import Annotated
 
 from ..base.results import BaseXapiResult
 from ..concepts.constants.video import (
     CONTEXT_EXTENSION_CC_ENABLED,
     CONTEXT_EXTENSION_PLAYED_SEGMENTS,
     RESULT_EXTENSION_PROGRESS,
     RESULT_EXTENSION_TIME,
@@ -29,70 +30,74 @@
     Attributes:
         playedSegments (str): Consists of parts of the video the actor watched during
             current registration in chronological order (for example,
             "0[.]5[,]12[.]22[,]15[.]55[,]55[.]99.33[,]99.33").
         time (float): Consists of the video time code when the event was emitted.
     """
 
-    time: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME)
-    playedSegments: Optional[str] = Field(alias=CONTEXT_EXTENSION_PLAYED_SEGMENTS)
+    time: Annotated[NonNegativeFloat, Field(alias=RESULT_EXTENSION_TIME)]
+    playedSegments: Annotated[
+        Optional[str], Field(alias=CONTEXT_EXTENSION_PLAYED_SEGMENTS)
+    ] = None
 
 
 class VideoPausedResultExtensions(VideoResultExtensions):
     """Pydantic model for video paused `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the ratio of media consumed by the actor.
     """
 
-    progress: Optional[NonNegativeFloat] = Field(alias=RESULT_EXTENSION_PROGRESS)
+    progress: Annotated[
+        Optional[NonNegativeFloat], Field(alias=RESULT_EXTENSION_PROGRESS)
+    ] = None
 
 
 class VideoSeekedResultExtensions(BaseExtensionModelWithConfig):
     """Pydantic model for video seeked `result`.`extensions` property.
 
     Attributes:
         timeFrom (float): Consists of the point in time the actor changed from in a
             media object during a seek operation.
         timeTo (float): Consists of the point in time the actor changed to in a media
             object during a seek operation.
     """
 
-    timeFrom: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME_FROM)
-    timeTo: NonNegativeFloat = Field(alias=RESULT_EXTENSION_TIME_TO)
+    timeFrom: Annotated[NonNegativeFloat, Field(alias=RESULT_EXTENSION_TIME_FROM)]
+    timeTo: Annotated[NonNegativeFloat, Field(alias=RESULT_EXTENSION_TIME_TO)]
 
 
 class VideoCompletedResultExtensions(VideoResultExtensions):
     """Pydantic model for video completed `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the percentage of media consumed by the actor.
     """
 
-    progress: NonNegativeFloat = Field(alias=RESULT_EXTENSION_PROGRESS)
+    progress: Annotated[NonNegativeFloat, Field(alias=RESULT_EXTENSION_PROGRESS)]
 
 
 class VideoTerminatedResultExtensions(VideoResultExtensions):
     """Pydantic model for video terminated `result`.`extensions` property.
 
     Attributes:
         progress (float): Consists of the percentage of media consumed by the actor.
     """
 
-    progress: NonNegativeFloat = Field(alias=RESULT_EXTENSION_PROGRESS)
+    progress: Annotated[NonNegativeFloat, Field(alias=RESULT_EXTENSION_PROGRESS)]
 
 
 class VideoEnableClosedCaptioningResultExtensions(VideoResultExtensions):
     """Pydantic model for video enable closed captioning `result`.`extensions` property.
 
     Attributes:
         ccEnabled (bool): Indicates whether subtitles are enabled.
     """
 
-    ccEnabled: bool = Field(alias=CONTEXT_EXTENSION_CC_ENABLED)
+    ccEnabled: Annotated[bool, Field(alias=CONTEXT_EXTENSION_CC_ENABLED)]
 
 
 class VideoPlayedResult(BaseXapiResult):
     """Pydantic model for video played `result` property.
 
     Attributes:
         extensions (dict): See VideoResultExtensions.
@@ -128,16 +133,16 @@
         extensions (dict): See VideoCompletedResultExtensions.
         completion (bool): Consists of the value `True`.
         duration (str): Consists of the total time spent consuming the video under
             current registration.
     """
 
     extensions: VideoCompletedResultExtensions
-    completion: Optional[Literal[True]]
-    duration: Optional[timedelta]
+    completion: Optional[Literal[True]] = None
+    duration: Optional[timedelta] = None
 
 
 class VideoTerminatedResult(BaseXapiResult):
     """Pydantic model for video terminated `result` property.
 
     Attributes:
         extensions (dict): See VideoTerminatedResultExtensions.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/contexts.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Virtual classroom xAPI events context fields definitions."""
 
 import sys
 from datetime import datetime
 from typing import List, Optional, Union
 from uuid import UUID
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
+from typing_extensions import Annotated
 
 from ..base.contexts import BaseXapiContext, BaseXapiContextContextActivities
 from ..base.unnested_objects import BaseXapiActivity
 from ..concepts.activity_types.scorm_profile import ProfileActivity
 from ..concepts.activity_types.virtual_classroom import VirtualClassroomActivity
 from ..concepts.constants.cmi5_profile import CONTEXT_EXTENSION_SESSION_ID
 from ..concepts.constants.tincan_vocabulary import CONTEXT_EXTENSION_PLANNED_DURATION
@@ -41,15 +42,15 @@
     """
 
     category: Union[
         VirtualClassroomProfileActivity,
         List[Union[VirtualClassroomProfileActivity, BaseXapiActivity]],
     ]
 
-    @validator("category")
+    @field_validator("category")
     @classmethod
     def check_presence_of_profile_activity_category(
         cls,
         value: Union[
             VirtualClassroomProfileActivity,
             List[Union[VirtualClassroomProfileActivity, BaseXapiActivity]],
         ],
@@ -72,15 +73,15 @@
 class VirtualClassroomContextExtensions(BaseExtensionModelWithConfig):
     """Pydantic model for virtual classroom base `context`.`extensions` property.
 
     Attributes:
         session_id (str): Consists of the ID of the active session.
     """
 
-    session_id: str = Field(alias=CONTEXT_EXTENSION_SESSION_ID, default="")
+    session_id: Annotated[str, Field(alias=CONTEXT_EXTENSION_SESSION_ID, default="")]
 
 
 class VirtualClassroomContext(BaseXapiContext):
     """Pydantic model for virtual classroom base `context` property.
 
     Attributes:
         registration (uuid): the registration that the Statement is associated with.
@@ -99,17 +100,17 @@
     """Pydantic model for virtual classroom initialized `context`.`extensions` property.
 
     Attributes:
         planned_duration (datetime): Consists of the estimated duration of the scheduled
             virtual classroom.
     """
 
-    planned_duration: Optional[datetime] = Field(
-        alias=CONTEXT_EXTENSION_PLANNED_DURATION
-    )
+    planned_duration: Annotated[
+        Optional[datetime], Field(alias=CONTEXT_EXTENSION_PLANNED_DURATION)
+    ]
 
 
 class VirtualClassroomInitializedContext(VirtualClassroomContext):
     """Pydantic model for virtual classroom initialized `context` property.
 
     Attributes:
         extensions (dict): see VirtualClassroomInitializedContextExtensions.
@@ -125,17 +126,17 @@
     """Pydantic model for virtual classroom initialized `context`.`extensions` property.
 
     Attributes:
         planned_duration (datetime): Consists of the estimated duration of the scheduled
             virtual classroom.
     """
 
-    planned_duration: Optional[datetime] = Field(
-        alias=CONTEXT_EXTENSION_PLANNED_DURATION
-    )
+    planned_duration: Annotated[
+        Optional[datetime], Field(alias=CONTEXT_EXTENSION_PLANNED_DURATION)
+    ]
 
 
 class VirtualClassroomJoinedContext(VirtualClassroomContext):
     """Pydantic model for virtual classroom joined `context` property.
 
     Attributes:
         extensions (dict): see VirtualClassroomJoinedContextExtensions.
@@ -151,17 +152,17 @@
     """Pydantic model for virtual classroom terminated `context`.`extensions` property.
 
     Attributes:
         planned_duration (datetime): Consists of the estimated duration of the scheduled
             virtual classroom.
     """
 
-    planned_duration: Optional[datetime] = Field(
-        alias=CONTEXT_EXTENSION_PLANNED_DURATION
-    )
+    planned_duration: Annotated[
+        Optional[datetime], Field(alias=CONTEXT_EXTENSION_PLANNED_DURATION)
+    ]
 
 
 class VirtualClassroomTerminatedContext(VirtualClassroomContext):
     """Pydantic model for virtual classroom terminated `context` property.
 
     Attributes:
         extensions (dict): see VirtualClassroomInitializedContextExtensions.
```

### Comparing `ralph-malph-4.2.0/src/ralph/models/xapi/virtual_classroom/statements.py` & `ralph-malph-5.0.0/src/ralph/models/xapi/virtual_classroom/statements.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,14 @@
     Example: John answered to a poll question.
 
     Attributes:
         verb (dict): See AskedVerb.
         object (dict): See CMIInteractionActivity.
         context (dict): See VirtualClassroomAnsweredPollContext.
         result (dict): See AnsweredPollResult.
-        result (dict): See AnsweredPollResult.
         timestamp (datetime): Consists of the timestamp of when the event occurred.
         result (dict): See AnsweredPollResult.
         timestamp (datetime): Consists of the timestamp of when the event occurred.
     """
 
     __selector__ = selector(
         verb__id="http://adlnet.gov/expapi/verbs/answered",
```

### Comparing `ralph-malph-4.2.0/src/ralph/parsers.py` & `ralph-malph-5.0.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph/utils.py` & `ralph-malph-5.0.0/src/ralph/utils.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-5.0.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 4.2.0
+Version: 5.0.0
 Summary: Ralph, the ultimate Learning Record Store (and more!) for your learning analytics.
 Author-email: "Open FUN (France Université Numérique)" <fun.dev@fun-mooc.fr>
 License: MIT License
         
         Copyright (c) 2020-present France Université Numérique
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata<8.0,>=7.0.1
 Requires-Dist: langcodes>=3.2.0
-Requires-Dist: pydantic[dotenv,email]<2.0,>=1.10.0
+Requires-Dist: pydantic[email]<3.0,>=2.5.3
+Requires-Dist: pydantic_settings<3.0,>=2.1.0
 Requires-Dist: rfc3987>=1.3.0
 Provides-Extra: backend-clickhouse
 Requires-Dist: clickhouse-connect[numpy,pandas]<0.6; extra == "backend-clickhouse"
 Requires-Dist: python-dateutil>=2.8.2; extra == "backend-clickhouse"
 Provides-Extra: backend-es
 Requires-Dist: elasticsearch[async]>=8.0.0; extra == "backend-es"
 Provides-Extra: backend-ldp
@@ -77,45 +78,45 @@
 Provides-Extra: cli
 Requires-Dist: bcrypt>=4.0.0; extra == "cli"
 Requires-Dist: click>=8.1.0; extra == "cli"
 Requires-Dist: click-option-group>=0.5.0; extra == "cli"
 Requires-Dist: sentry-sdk[fastapi]>=1.9.0; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: anyio<4.3.1; extra == "dev"
-Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: factory-boy==3.3.0; extra == "dev"
-Requires-Dist: hypothesis<6.92.0; extra == "dev"
 Requires-Dist: logging-gelf==0.0.32; extra == "dev"
 Requires-Dist: mike==2.0.0; extra == "dev"
-Requires-Dist: mkdocs==1.5.3; extra == "dev"
+Requires-Dist: mkdocs==1.6.0; extra == "dev"
 Requires-Dist: mkdocs-click==0.8.1; extra == "dev"
-Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
-Requires-Dist: mkdocstrings[python-legacy]==0.24.3; extra == "dev"
-Requires-Dist: moto==5.0.5; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mkdocs-material==9.5.20; extra == "dev"
+Requires-Dist: mkdocstrings[python-legacy]==0.25.0; extra == "dev"
+Requires-Dist: moto==5.0.6; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: neoteroi-mkdocs==1.0.5; extra == "dev"
-Requires-Dist: pyfakefs==5.4.0; extra == "dev"
-Requires-Dist: pymdown-extensions==10.7.1; extra == "dev"
+Requires-Dist: polyfactory==2.15.0; extra == "dev"
+Requires-Dist: pyfakefs==5.4.1; extra == "dev"
+Requires-Dist: pymdown-extensions==10.8.1; extra == "dev"
 Requires-Dist: pytest<8.0.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-httpx<0.23.0; extra == "dev"
 Requires-Dist: requests-mock==1.12.1; extra == "dev"
 Requires-Dist: responses==0.24.1; extra == "dev"
-Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: ruff==0.4.2; extra == "dev"
 Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == "dev"
 Requires-Dist: types-python-jose==3.3.4.20240106; extra == "dev"
 Requires-Dist: types-requests<2.31.0.20240407; extra == "dev"
 Requires-Dist: types-cachetools==5.3.0.7; extra == "dev"
 Provides-Extra: lrs
 Requires-Dist: bcrypt==4.1.2; extra == "lrs"
-Requires-Dist: fastapi==0.110.1; extra == "lrs"
+Requires-Dist: fastapi==0.110.2; extra == "lrs"
 Requires-Dist: cachetools==5.3.3; extra == "lrs"
 Requires-Dist: httpx<0.25.0; extra == "lrs"
-Requires-Dist: sentry_sdk==1.44.1; extra == "lrs"
+Requires-Dist: sentry_sdk==2.0.1; extra == "lrs"
 Requires-Dist: python-jose==3.3.0; extra == "lrs"
 Requires-Dist: uvicorn[standard]==0.29.0; extra == "lrs"
 Provides-Extra: full
 Requires-Dist: ralph-malph[backends,cli,lrs]; extra == "full"
 
 
 <p align="center">
```

### Comparing `ralph-malph-4.2.0/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-5.0.0/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph_malph.egg-info/entry_points.txt` & `ralph-malph-5.0.0/src/ralph_malph.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-5.0.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 importlib-metadata<8.0,>=7.0.1
 langcodes>=3.2.0
-pydantic[dotenv,email]<2.0,>=1.10.0
+pydantic[email]<3.0,>=2.5.3
+pydantic_settings<3.0,>=2.1.0
 rfc3987>=1.3.0
 
 [backend-clickhouse]
 clickhouse-connect[numpy,pandas]<0.6
 python-dateutil>=2.8.2
 
 [backend-es]
@@ -44,44 +45,44 @@
 bcrypt>=4.0.0
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
 anyio<4.3.1
-black==24.3.0
+black==24.4.2
 cryptography==42.0.5
 factory-boy==3.3.0
-hypothesis<6.92.0
 logging-gelf==0.0.32
 mike==2.0.0
-mkdocs==1.5.3
+mkdocs==1.6.0
 mkdocs-click==0.8.1
-mkdocs-material==9.5.17
-mkdocstrings[python-legacy]==0.24.3
-moto==5.0.5
-mypy==1.9.0
+mkdocs-material==9.5.20
+mkdocstrings[python-legacy]==0.25.0
+moto==5.0.6
+mypy==1.10.0
 neoteroi-mkdocs==1.0.5
-pyfakefs==5.4.0
-pymdown-extensions==10.7.1
+polyfactory==2.15.0
+pyfakefs==5.4.1
+pymdown-extensions==10.8.1
 pytest<8.0.0
 pytest-cov==5.0.0
 pytest-httpx<0.23.0
 requests-mock==1.12.1
 responses==0.24.1
-ruff==0.3.5
+ruff==0.4.2
 types-python-dateutil==2.9.0.20240316
 types-python-jose==3.3.4.20240106
 types-requests<2.31.0.20240407
 types-cachetools==5.3.0.7
 
 [full]
 ralph-malph[backends,cli,lrs]
 
 [lrs]
 bcrypt==4.1.2
-fastapi==0.110.1
+fastapi==0.110.2
 cachetools==5.3.3
 httpx<0.25.0
-sentry_sdk==1.44.1
+sentry_sdk==2.0.1
 python-jose==3.3.0
 uvicorn[standard]==0.29.0
```

### Comparing `ralph-malph-4.2.0/tests/test_cli.py` & `ralph-malph-5.0.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import pytest
 from click.exceptions import BadParameter
 from click.testing import CliRunner
 from elasticsearch.helpers import bulk, scan
-from hypothesis import settings as hypothesis_settings
 from pydantic import ValidationError
 
 from ralph import cli as cli_module
 from ralph.backends.data.fs import FSDataBackend
 from ralph.backends.data.ldp import LDPDataBackend
 from ralph.cli import (
     CommaSeparatedKeyValueParamType,
@@ -26,21 +25,21 @@
 )
 from ralph.conf import settings
 from ralph.exceptions import BackendParameterException, ConfigurationException
 from ralph.models.edx.navigational.statements import UIPageClose
 from ralph.models.xapi.navigation.statements import PageTerminated
 from ralph.utils import iter_over_async
 
+from tests.factories import mock_instance
 from tests.fixtures.backends import (
     ES_TEST_HOSTS,
     ES_TEST_INDEX,
     WS_TEST_HOST,
     WS_TEST_PORT,
 )
-from tests.fixtures.hypothesis_strategies import custom_given
 
 test_logger = logging.getLogger("ralph")
 
 
 def test_cli_comma_separated_key_value_param_type():
     """Test the CommaSeparatedKeyValueParamType custom parameter type."""
     param_type = CommaSeparatedKeyValueParamType()
@@ -153,15 +152,15 @@
     ):
         param_type.convert(value, None, None)
 
 
 def test_cli_help_option():
     """Test ralph --help command."""
     runner = CliRunner()
-    result = runner.invoke(cli, ["--help"])
+    result = runner.invoke(cli, ["--help"], catch_exceptions=False)
 
     assert result.exit_code == 0
     assert (
         (
             "-v, --verbosity LVL  Either CRITICAL, ERROR, WARNING, INFO (default) or "
             "DEBUG"
         )
@@ -498,29 +497,30 @@
 
     runner = CliRunner()
     result = runner.invoke(cli, "extract -p es".split(), input=es_output)
     assert result.exit_code == 0
     assert "\n".join([json.dumps({"id": idx}) for idx in range(10)]) in result.output
 
 
-@custom_given(UIPageClose)
-def test_cli_validate_command_with_edx_format(event):
+def test_cli_validate_command_with_edx_format():
     """Test ralph validate command using the edx format."""
-    event_str = event.json()
+    event = mock_instance(UIPageClose)
+
+    event_str = event.model_dump_json()
     runner = CliRunner()
     result = runner.invoke(cli, ["validate", "-f", "edx"], input=event_str)
     assert event_str in result.output
 
 
-@hypothesis_settings(deadline=None)
-@custom_given(UIPageClose)
 @pytest.mark.parametrize("valid_uuid", ["ee241f8b-174f-5bdb-bae9-c09de5fe017f"])
-def test_cli_convert_command_from_edx_to_xapi_format(valid_uuid, event):
+def test_cli_convert_command_from_edx_to_xapi_format(valid_uuid):
     """Test ralph convert command from edx to xapi format."""
-    event_str = event.json()
+    event = mock_instance(UIPageClose)
+
+    event_str = event.model_dump_json()
     runner = CliRunner()
     command = f"-v ERROR convert -f edx -t xapi -u {valid_uuid} -p https://fun-mooc.fr"
     result = runner.invoke(cli, command.split(), input=event_str)
     assert result.exit_code == 0
     try:
         PageTerminated(**json.loads(result.output))
     except ValidationError as err:
@@ -647,18 +647,19 @@
     # As we bulk insert documents, the index needs to be refreshed before making
     # queries.
     es.indices.refresh(index=ES_TEST_INDEX)
 
     runner = CliRunner()
     es_hosts = ",".join(ES_TEST_HOSTS)
     es_client_options = "verify_certs=True"
-    command = f"""-v ERROR read -b es --es-hosts {es_hosts}
+    command = f"""-v ERROR read -b es
         --es-default-index {ES_TEST_INDEX}
-        --es-client-options {es_client_options}"""
-    result = runner.invoke(cli, command.split())
+        --es-hosts {es_hosts} --es-client-options {es_client_options}"""
+    result = runner.invoke(cli, command.split(), catch_exceptions=False)
+
     assert result.exit_code == 0
     expected = (
         "\n".join(
             [
                 json.dumps(
                     {
                         "_index": ES_TEST_INDEX,
@@ -678,16 +679,16 @@
 
 
 def test_cli_read_command_client_options_with_es_backend(es):
     """Test ralph read command with multiple client options using the es backend."""
 
     runner = CliRunner()
     es_client_options = "ca_certs=/path/,verify_certs=True"
-    command = f"""-v ERROR read -b es --es-client-options {es_client_options}"""
-    result = runner.invoke(cli, command.split())
+    command = f"""-v DEBUG read -b es --es-client-options {es_client_options}"""
+    result = runner.invoke(cli, command.split(), catch_exceptions=True)
     assert result.exit_code == 1
     assert "TLS options require scheme to be 'https'" in str(result.exception)
 
 
 def test_cli_read_command_with_es_backend_query(es):
     """Test ralph read command using the es backend and a query."""
 
@@ -746,19 +747,19 @@
     invalid_query_str = "wrong_query_string"
 
     command = f"-v ERROR read -b mongo {invalid_query_str}"
     result = runner.invoke(cli, command.split())
     assert result.exit_code > 0
     assert isinstance(result.exception, BackendParameterException)
     msg = (
-        "Invalid MongoQuery query string: "
-        "[{'loc': ('__root__',), 'msg': 'Expecting value: line 1 column 1 (char 0)', "
-        "'type': 'value_error.jsondecode', 'ctx': {'msg': 'Expecting value', "
-        "'doc': 'wrong_query_string', 'pos': 0, 'lineno': 1, 'colno': 1}}]"
+        "Invalid MongoQuery query string: [{'type': 'value_error.jsondecode',"
+        " 'loc': ('__root__',), 'msg': 'Expecting value: line 1 column 1 (char 0)',"
+        " 'input': 'wrong_query_string'}]"
     )
+
     assert str(result.exception) == msg
 
 
 def test_cli_read_command_with_ws_backend(events, ws):
     """Test ralph read command using the ws backend."""
 
     # The ws fixture is async, however the `CliRunner` does not support running in an
@@ -766,15 +767,20 @@
     @contextmanager
     def websocket():
         yield from iter_over_async(ws)
 
     with websocket():
         runner = CliRunner()
         uri = f"ws://{WS_TEST_HOST}:{WS_TEST_PORT}"
-        result = runner.invoke(cli, ["read", "-b", "async_ws", "--async-ws-uri", uri])
+        result = runner.invoke(
+            cli,
+            ["read", "-b", "async_ws", "--async-ws-uri", uri],
+            catch_exceptions=False,
+        )
+        assert result.exit_code == 0
         assert "\n".join([json.dumps(event) for event in events]) in result.output
 
 
 def test_cli_list_command_with_ldp_backend(monkeypatch):
     """Test ralph list command using the LDP backend."""
     archive_list = [
         "5d5c4c93-04a4-42c5-9860-f51fa4044aa1",
@@ -987,18 +993,20 @@
     """Test ralph write command using the es backend."""
 
     # Documents
     records = [{"id": idx} for idx in range(10)]
 
     runner = CliRunner()
     es_hosts = ",".join(ES_TEST_HOSTS)
+
     result = runner.invoke(
         cli,
         f"write -b es --es-hosts {es_hosts} --es-default-index {ES_TEST_INDEX}".split(),
         input="\n".join(json.dumps(record) for record in records),
+        catch_exceptions=False,
     )
     assert result.exit_code == 0
 
     # As we bulk insert documents, the index needs to be refreshed before making
     # queries.
     es.indices.refresh(index=ES_TEST_INDEX)
     documents = list(scan(es, index=ES_TEST_INDEX, size=10))
```

### Comparing `ralph-malph-4.2.0/tests/test_cli_usage.py` & `ralph-malph-5.0.0/tests/test_cli_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,56 +105,57 @@
 
 def test_cli_read_command_usage():
     """Test ralph read command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["read", "--help"])
 
     assert result.exit_code == 0
+
     assert (
         "Usage: ralph read [OPTIONS] [QUERY]\n\n"
         "  Read records matching the QUERY (json or string) from a configured backend."
         "\n\n"
         "Options:\n"
         "  -b, --backend "
         "[async_es|async_lrs|async_mongo|async_ws|clickhouse|es|fs|ldp|lrs|mongo|s3|"
         "swift]\n"
         "                                  Backend  [required]\n"
         "  async_es backend: \n"
         "    --async-es-allow-yellow-status / --no-async-es-allow-yellow-status\n"
         "    --async-es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --async-es-default-index TEXT\n"
-        "    --async-es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --async-es-hosts TEXT\n"
         "    --async-es-locale-encoding TEXT\n"
         "    --async-es-point-in-time-keep-alive TEXT\n"
         "    --async-es-read-chunk-size INTEGER\n"
         "    --async-es-refresh-after-write TEXT\n"
         "    --async-es-write-chunk-size INTEGER\n"
         "  async_lrs backend: \n"
-        "    --async-lrs-base-url TEXT\n"
+        "    --async-lrs-base-url URL\n"
         "    --async-lrs-headers KEY=VALUE,KEY=VALUE\n"
         "    --async-lrs-locale-encoding TEXT\n"
         "    --async-lrs-password TEXT\n"
         "    --async-lrs-read-chunk-size INTEGER\n"
         "    --async-lrs-statements-endpoint TEXT\n"
         "    --async-lrs-status-endpoint TEXT\n"
         "    --async-lrs-username TEXT\n"
         "    --async-lrs-write-chunk-size INTEGER\n"
         "  async_mongo backend: \n"
         "    --async-mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --async-mongo-connection-uri MONGODSN\n"
+        "    --async-mongo-connection-uri MULTIHOSTURL\n"
         "    --async-mongo-default-collection TEXT\n"
         "    --async-mongo-default-database TEXT\n"
         "    --async-mongo-locale-encoding TEXT\n"
         "    --async-mongo-read-chunk-size INTEGER\n"
         "    --async-mongo-write-chunk-size INTEGER\n"
         "  async_ws backend: \n"
         "    --async-ws-client-options KEY=VALUE,KEY=VALUE\n"
         "    --async-ws-locale-encoding TEXT\n"
         "    --async-ws-read-chunk-size INTEGER\n"
-        "    --async-ws-uri TEXT\n"
+        "    --async-ws-uri URL\n"
         "    --async-ws-write-chunk-size INTEGER\n"
         "  clickhouse backend: \n"
         "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
         "    --clickhouse-database TEXT\n"
         "    --clickhouse-event-table-name TEXT\n"
         "    --clickhouse-host TEXT\n"
         "    --clickhouse-locale-encoding TEXT\n"
@@ -163,15 +164,15 @@
         "    --clickhouse-read-chunk-size INTEGER\n"
         "    --clickhouse-username TEXT\n"
         "    --clickhouse-write-chunk-size INTEGER\n"
         "  es backend: \n"
         "    --es-allow-yellow-status / --no-es-allow-yellow-status\n"
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-default-index TEXT\n"
-        "    --es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --es-hosts TEXT\n"
         "    --es-locale-encoding TEXT\n"
         "    --es-point-in-time-keep-alive TEXT\n"
         "    --es-read-chunk-size INTEGER\n"
         "    --es-refresh-after-write TEXT\n"
         "    --es-write-chunk-size INTEGER\n"
         "  fs backend: \n"
         "    --fs-default-directory-path PATH\n"
@@ -187,26 +188,26 @@
         "    --ldp-endpoint TEXT\n"
         "    --ldp-locale-encoding TEXT\n"
         "    --ldp-read-chunk-size INTEGER\n"
         "    --ldp-request-timeout TEXT\n"
         "    --ldp-service-name TEXT\n"
         "    --ldp-write-chunk-size INTEGER\n"
         "  lrs backend: \n"
-        "    --lrs-base-url TEXT\n"
+        "    --lrs-base-url URL\n"
         "    --lrs-headers KEY=VALUE,KEY=VALUE\n"
         "    --lrs-locale-encoding TEXT\n"
         "    --lrs-password TEXT\n"
         "    --lrs-read-chunk-size INTEGER\n"
         "    --lrs-statements-endpoint TEXT\n"
         "    --lrs-status-endpoint TEXT\n"
         "    --lrs-username TEXT\n"
         "    --lrs-write-chunk-size INTEGER\n"
         "  mongo backend: \n"
         "    --mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --mongo-connection-uri MONGODSN\n"
+        "    --mongo-connection-uri MULTIHOSTURL\n"
         "    --mongo-default-collection TEXT\n"
         "    --mongo-default-database TEXT\n"
         "    --mongo-locale-encoding TEXT\n"
         "    --mongo-read-chunk-size INTEGER\n"
         "    --mongo-write-chunk-size INTEGER\n"
         "  s3 backend: \n"
         "    --s3-access-key-id TEXT\n"
@@ -263,23 +264,23 @@
         "Options:\n"
         "  -b, --backend [async_es|async_mongo|clickhouse|es|fs|ldp|mongo|s3|swift]\n"
         "                                  Backend  [required]\n"
         "  async_es backend: \n"
         "    --async-es-allow-yellow-status / --no-async-es-allow-yellow-status\n"
         "    --async-es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --async-es-default-index TEXT\n"
-        "    --async-es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --async-es-hosts TEXT\n"
         "    --async-es-locale-encoding TEXT\n"
         "    --async-es-point-in-time-keep-alive TEXT\n"
         "    --async-es-read-chunk-size INTEGER\n"
         "    --async-es-refresh-after-write TEXT\n"
         "    --async-es-write-chunk-size INTEGER\n"
         "  async_mongo backend: \n"
         "    --async-mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --async-mongo-connection-uri MONGODSN\n"
+        "    --async-mongo-connection-uri MULTIHOSTURL\n"
         "    --async-mongo-default-collection TEXT\n"
         "    --async-mongo-default-database TEXT\n"
         "    --async-mongo-locale-encoding TEXT\n"
         "    --async-mongo-read-chunk-size INTEGER\n"
         "    --async-mongo-write-chunk-size INTEGER\n"
         "  clickhouse backend: \n"
         "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
@@ -292,15 +293,15 @@
         "    --clickhouse-read-chunk-size INTEGER\n"
         "    --clickhouse-username TEXT\n"
         "    --clickhouse-write-chunk-size INTEGER\n"
         "  es backend: \n"
         "    --es-allow-yellow-status / --no-es-allow-yellow-status\n"
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-default-index TEXT\n"
-        "    --es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --es-hosts TEXT\n"
         "    --es-locale-encoding TEXT\n"
         "    --es-point-in-time-keep-alive TEXT\n"
         "    --es-read-chunk-size INTEGER\n"
         "    --es-refresh-after-write TEXT\n"
         "    --es-write-chunk-size INTEGER\n"
         "  fs backend: \n"
         "    --fs-default-directory-path PATH\n"
@@ -317,15 +318,15 @@
         "    --ldp-locale-encoding TEXT\n"
         "    --ldp-read-chunk-size INTEGER\n"
         "    --ldp-request-timeout TEXT\n"
         "    --ldp-service-name TEXT\n"
         "    --ldp-write-chunk-size INTEGER\n"
         "  mongo backend: \n"
         "    --mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --mongo-connection-uri MONGODSN\n"
+        "    --mongo-connection-uri MULTIHOSTURL\n"
         "    --mongo-default-collection TEXT\n"
         "    --mongo-default-database TEXT\n"
         "    --mongo-locale-encoding TEXT\n"
         "    --mongo-read-chunk-size INTEGER\n"
         "    --mongo-write-chunk-size INTEGER\n"
         "  s3 backend: \n"
         "    --s3-access-key-id TEXT\n"
@@ -382,33 +383,33 @@
         "[async_es|async_lrs|async_mongo|clickhouse|es|fs|lrs|mongo|s3|swift]"
         "\n"
         "                                  Backend  [required]\n"
         "  async_es backend: \n"
         "    --async-es-allow-yellow-status / --no-async-es-allow-yellow-status\n"
         "    --async-es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --async-es-default-index TEXT\n"
-        "    --async-es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --async-es-hosts TEXT\n"
         "    --async-es-locale-encoding TEXT\n"
         "    --async-es-point-in-time-keep-alive TEXT\n"
         "    --async-es-read-chunk-size INTEGER\n"
         "    --async-es-refresh-after-write TEXT\n"
         "    --async-es-write-chunk-size INTEGER\n"
         "  async_lrs backend: \n"
-        "    --async-lrs-base-url TEXT\n"
+        "    --async-lrs-base-url URL\n"
         "    --async-lrs-headers KEY=VALUE,KEY=VALUE\n"
         "    --async-lrs-locale-encoding TEXT\n"
         "    --async-lrs-password TEXT\n"
         "    --async-lrs-read-chunk-size INTEGER\n"
         "    --async-lrs-statements-endpoint TEXT\n"
         "    --async-lrs-status-endpoint TEXT\n"
         "    --async-lrs-username TEXT\n"
         "    --async-lrs-write-chunk-size INTEGER\n"
         "  async_mongo backend: \n"
         "    --async-mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --async-mongo-connection-uri MONGODSN\n"
+        "    --async-mongo-connection-uri MULTIHOSTURL\n"
         "    --async-mongo-default-collection TEXT\n"
         "    --async-mongo-default-database TEXT\n"
         "    --async-mongo-locale-encoding TEXT\n"
         "    --async-mongo-read-chunk-size INTEGER\n"
         "    --async-mongo-write-chunk-size INTEGER\n"
         "  clickhouse backend: \n"
         "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
@@ -421,39 +422,39 @@
         "    --clickhouse-read-chunk-size INTEGER\n"
         "    --clickhouse-username TEXT\n"
         "    --clickhouse-write-chunk-size INTEGER\n"
         "  es backend: \n"
         "    --es-allow-yellow-status / --no-es-allow-yellow-status\n"
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-default-index TEXT\n"
-        "    --es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --es-hosts TEXT\n"
         "    --es-locale-encoding TEXT\n"
         "    --es-point-in-time-keep-alive TEXT\n"
         "    --es-read-chunk-size INTEGER\n"
         "    --es-refresh-after-write TEXT\n"
         "    --es-write-chunk-size INTEGER\n"
         "  fs backend: \n"
         "    --fs-default-directory-path PATH\n"
         "    --fs-default-query-string TEXT\n"
         "    --fs-locale-encoding TEXT\n"
         "    --fs-read-chunk-size INTEGER\n"
         "    --fs-write-chunk-size INTEGER\n"
         "  lrs backend: \n"
-        "    --lrs-base-url TEXT\n"
+        "    --lrs-base-url URL\n"
         "    --lrs-headers KEY=VALUE,KEY=VALUE\n"
         "    --lrs-locale-encoding TEXT\n"
         "    --lrs-password TEXT\n"
         "    --lrs-read-chunk-size INTEGER\n"
         "    --lrs-statements-endpoint TEXT\n"
         "    --lrs-status-endpoint TEXT\n"
         "    --lrs-username TEXT\n"
         "    --lrs-write-chunk-size INTEGER\n"
         "  mongo backend: \n"
         "    --mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --mongo-connection-uri MONGODSN\n"
+        "    --mongo-connection-uri MULTIHOSTURL\n"
         "    --mongo-default-collection TEXT\n"
         "    --mongo-default-database TEXT\n"
         "    --mongo-locale-encoding TEXT\n"
         "    --mongo-read-chunk-size INTEGER\n"
         "    --mongo-write-chunk-size INTEGER\n"
         "  s3 backend: \n"
         "    --s3-access-key-id TEXT\n"
@@ -513,23 +514,23 @@
         "Options:\n"
         "  -b, --backend [async_es|async_mongo|clickhouse|es|fs|mongo]\n"
         "                                  Backend  [required]\n"
         "  async_es backend: \n"
         "    --async-es-allow-yellow-status / --no-async-es-allow-yellow-status\n"
         "    --async-es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --async-es-default-index TEXT\n"
-        "    --async-es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --async-es-hosts TEXT\n"
         "    --async-es-locale-encoding TEXT\n"
         "    --async-es-point-in-time-keep-alive TEXT\n"
         "    --async-es-read-chunk-size INTEGER\n"
         "    --async-es-refresh-after-write TEXT\n"
         "    --async-es-write-chunk-size INTEGER\n"
         "  async_mongo backend: \n"
         "    --async-mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --async-mongo-connection-uri MONGODSN\n"
+        "    --async-mongo-connection-uri MULTIHOSTURL\n"
         "    --async-mongo-default-collection TEXT\n"
         "    --async-mongo-default-database TEXT\n"
         "    --async-mongo-locale-encoding TEXT\n"
         "    --async-mongo-read-chunk-size INTEGER\n"
         "    --async-mongo-write-chunk-size INTEGER\n"
         "  clickhouse backend: \n"
         "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
@@ -543,30 +544,30 @@
         "    --clickhouse-read-chunk-size INTEGER\n"
         "    --clickhouse-username TEXT\n"
         "    --clickhouse-write-chunk-size INTEGER\n"
         "  es backend: \n"
         "    --es-allow-yellow-status / --no-es-allow-yellow-status\n"
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-default-index TEXT\n"
-        "    --es-hosts VALUE1,VALUE2,VALUE3\n"
+        "    --es-hosts TEXT\n"
         "    --es-locale-encoding TEXT\n"
         "    --es-point-in-time-keep-alive TEXT\n"
         "    --es-read-chunk-size INTEGER\n"
         "    --es-refresh-after-write TEXT\n"
         "    --es-write-chunk-size INTEGER\n"
         "  fs backend: \n"
         "    --fs-default-directory-path PATH\n"
         "    --fs-default-lrs-file TEXT\n"
         "    --fs-default-query-string TEXT\n"
         "    --fs-locale-encoding TEXT\n"
         "    --fs-read-chunk-size INTEGER\n"
         "    --fs-write-chunk-size INTEGER\n"
         "  mongo backend: \n"
         "    --mongo-client-options KEY=VALUE,KEY=VALUE\n"
-        "    --mongo-connection-uri MONGODSN\n"
+        "    --mongo-connection-uri MULTIHOSTURL\n"
         "    --mongo-default-collection TEXT\n"
         "    --mongo-default-database TEXT\n"
         "    --mongo-locale-encoding TEXT\n"
         "    --mongo-read-chunk-size INTEGER\n"
         "    --mongo-write-chunk-size INTEGER\n"
         "  -h, --host TEXT                 LRS server host name\n"
         "  -p, --port INTEGER              LRS server port\n"
```

### Comparing `ralph-malph-4.2.0/tests/test_conf.py` & `ralph-malph-5.0.0/tests/test_conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for Ralph's configuration loading."""
 
 from importlib import reload
 
 import pytest
+from pydantic import TypeAdapter, ValidationError
 
 from ralph import conf
 from ralph.backends.data.es import ESDataBackend
 from ralph.conf import (
     AuthBackend,
     AuthBackends,
     CommaSeparatedTuple,
@@ -48,24 +49,24 @@
         (("foo",), ("foo",)),
         (["foo"], ("foo",)),
         ("foo,bar,baz", ("foo", "bar", "baz")),
     ],
 )
 def test_conf_comma_separated_list_with_valid_values(value, expected, monkeypatch):
     """Test the CommaSeparatedTuple pydantic data type with valid values."""
-    assert next(CommaSeparatedTuple.__get_validators__())(value) == expected
+    assert TypeAdapter(CommaSeparatedTuple).validate_python(value) == expected
     monkeypatch.setenv("RALPH_BACKENDS__DATA__ES__HOSTS", "".join(value))
     assert ESDataBackend().settings.HOSTS == expected
 
 
 @pytest.mark.parametrize("value", [{}, None])
 def test_conf_comma_separated_list_with_invalid_values(value):
     """Test the CommaSeparatedTuple pydantic data type with invalid values."""
-    with pytest.raises(TypeError, match="Invalid comma-separated list"):
-        next(CommaSeparatedTuple.__get_validators__())(value)
+    with pytest.raises(ValidationError, match="2 validation errors for function-after"):
+        TypeAdapter(CommaSeparatedTuple).validate_python(value)
 
 
 @pytest.mark.parametrize(
     "value,is_valid,expected",
     [
         ("oidc", True, (AuthBackend.OIDC,)),
         ("basic", True, (AuthBackend.BASIC,)),
@@ -74,31 +75,31 @@
         ("notvalid", False, None),
         ("basic,notvalid", False, None),
     ],
 )
 def test_conf_auth_backend(value, is_valid, expected, monkeypatch):
     """Test the AuthBackends data type with valid and invalid values."""
     if is_valid:
-        assert next(AuthBackends.__get_validators__())(value) == expected
+        assert TypeAdapter(AuthBackends).validate_python(value) == expected
         monkeypatch.setenv("RALPH_RUNSERVER_AUTH_BACKENDS", "".join(value))
         reload(conf)
         assert conf.settings.RUNSERVER_AUTH_BACKENDS == expected
     else:
         with pytest.raises(ValueError, match="'notvalid' is not a valid AuthBackend"):
-            next(AuthBackends.__get_validators__())(value)
+            TypeAdapter(AuthBackends).validate_python(value)
 
 
 def test_conf_core_settings_should_impact_settings_defaults(monkeypatch):
     """Test that core settings update application settings values."""
     monkeypatch.setenv("RALPH_APP_DIR", "/foo")
     monkeypatch.setenv("RALPH_LOCALE_ENCODING", "ascii")
     reload(conf)
 
     # Configuration.
-    assert conf.Settings.Config.env_file_encoding == "ascii"
+    assert conf.Settings.model_config["env_file_encoding"] == "ascii"
 
     # Properties.
     assert str(conf.settings.APP_DIR) == "/foo"
     assert conf.settings.LOCALE_ENCODING == "ascii"
 
     # Defaults.
     assert str(conf.settings.AUTH_FILE) == "/foo/auth.json"
```

### Comparing `ralph-malph-4.2.0/tests/test_dependencies.py` & `ralph-malph-5.0.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/tests/test_filters.py` & `ralph-malph-5.0.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/tests/test_helpers.py` & `ralph-malph-5.0.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/tests/test_logger.py` & `ralph-malph-5.0.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/tests/test_parsers.py` & `ralph-malph-5.0.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-4.2.0/tests/test_utils.py` & `ralph-malph-5.0.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         settings_class = DummyTestBackendSettings
 
         def __init__(self, settings):
             self.settings = settings
 
     backend = ralph_utils.get_backend_instance(DummyTestBackend, options)
     assert isinstance(backend, DummyTestBackend)
-    assert backend.settings.dict() == expected
+    assert backend.settings.model_dump() == expected
 
 
 @pytest.mark.parametrize("path,value", [(["foo", "bar"], "bar_value")])
 def test_utils_get_dict_value_from_path_should_return_given_value(path, value):
     """Test the get_dict_value_from_path function should return the value when it's
     present.
     """
```

