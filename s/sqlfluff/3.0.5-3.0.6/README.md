# Comparing `tmp/sqlfluff-3.0.5.tar.gz` & `tmp/sqlfluff-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff-3.0.5.tar", last modified: Fri Apr 19 13:48:27 2024, max compression
+gzip compressed data, was "sqlfluff-3.0.6.tar", last modified: Mon May  6 19:38:40 2024, max compression
```

## Comparing `sqlfluff-3.0.5.tar` & `sqlfluff-3.0.6.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.644667 sqlfluff-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)   501370 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:48:27.644667 sqlfluff-3.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.584667 sqlfluff-3.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.592667 sqlfluff-3.0.5/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    49340 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.600667 sqlfluff-3.0.5/src/sqlfluff/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.600667 sqlfluff-3.0.5/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    45903 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/match_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49362 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/bracketed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46392 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.612667 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.620667 sqlfluff-3.0.5/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   139271 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    73562 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    36216 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    93480 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    33399 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)   191523 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    73019 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   242562 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (127)   105180 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   189871 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    66185 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.620667 sqlfluff-3.0.5/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.628667 sqlfluff-3.0.5/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.628667 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.632667 sqlfluff-3.0.5/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.632667 sqlfluff-3.0.5/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/test/testing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)   507355 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.927252 sqlfluff-3.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.931252 sqlfluff-3.0.6/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.935252 sqlfluff-3.0.6/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.935252 sqlfluff-3.0.6/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51559 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47948 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.943252 sqlfluff-3.0.6/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.943252 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/match_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.947252 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49362 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/bracketed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.947252 sqlfluff-3.0.6/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45600 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46401 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139271 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82970 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40104 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93480 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33399 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192309 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73019 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   242793 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105781 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194021 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66185 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.967252 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.967252 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/test/testing_test.py
```

### Comparing `sqlfluff-3.0.5/CHANGELOG.md` & `sqlfluff-3.0.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,73 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [3.0.6] - 2024-05-06
+
+## Highlights
+
+This release primarily fixes an issue introduced by the recent dbt 1.7.14 release,
+and better support for dbt 1.7+. It also includes a range of dialect improvements
+and CLI refinements.
+
+This release also includes the groundwork for linting the unrendered sections of
+Jinja templates. More documentation on this will be released in due course when
+it's ready for beta testing.
+
+Thanks also to [@padraic00](https://github.com/padraic00) &
+[@burhanyasar](https://github.com/burhanyasar) who made their first contributions
+in this release. 🎉🎉🏆🎉🎉
+
+## What’s Changed
+
+* [fix_clickhouse] Temporary Table Create AS SELECT [#5843](https://github.com/sqlfluff/sqlfluff/pull/5843) [@konnectr](https://github.com/konnectr)
+* Bugfix: ST02 - Compare entire condition expression [#5850](https://github.com/sqlfluff/sqlfluff/pull/5850) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Clichouse prewhere [#5849](https://github.com/sqlfluff/sqlfluff/pull/5849) [@konnectr](https://github.com/konnectr)
+* BigQuery: Support missing DROP statements [#5848](https://github.com/sqlfluff/sqlfluff/pull/5848) [@kzosabe](https://github.com/kzosabe)
+* BigQuery: various CREATE statements [#5846](https://github.com/sqlfluff/sqlfluff/pull/5846) [@greg-finley](https://github.com/greg-finley)
+* BigQuery Alter Schema [#5835](https://github.com/sqlfluff/sqlfluff/pull/5835) [@greg-finley](https://github.com/greg-finley)
+* Snowflake execute immediate from [#5836](https://github.com/sqlfluff/sqlfluff/pull/5836) [@greg-finley](https://github.com/greg-finley)
+* Support dbt 1.7 [#5842](https://github.com/sqlfluff/sqlfluff/pull/5842) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Postgres: Create extension cascade [#5834](https://github.com/sqlfluff/sqlfluff/pull/5834) [@greg-finley](https://github.com/greg-finley)
+* Postgres: Add Support for PostGIS operators [#5830](https://github.com/sqlfluff/sqlfluff/pull/5830) [@burhanyasar](https://github.com/burhanyasar)
+* Db2: Support additional CREATE INDEX options [#5827](https://github.com/sqlfluff/sqlfluff/pull/5827) [@keraion](https://github.com/keraion)
+* Allow to align all siblings when respacing [#5826](https://github.com/sqlfluff/sqlfluff/pull/5826) [@borchero](https://github.com/borchero)
+* BigQuery: Support EXECUTE IMMEDIATE [#5820](https://github.com/sqlfluff/sqlfluff/pull/5820) [@keraion](https://github.com/keraion)
+* BigQuery: Support CREATE ROW ACCESS POLICY statement [#5821](https://github.com/sqlfluff/sqlfluff/pull/5821) [@kzosabe](https://github.com/kzosabe)
+* Fix Jinja variant location correction [#5814](https://github.com/sqlfluff/sqlfluff/pull/5814) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Test cases for linter fails. [#5815](https://github.com/sqlfluff/sqlfluff/pull/5815) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* BigQuery: Support nested BEGIN, Fix CREATE PROCEDURE OPTIONS [#5816](https://github.com/sqlfluff/sqlfluff/pull/5816) [@keraion](https://github.com/keraion)
+* Bring multiple jinja variants through to the parser. [#5794](https://github.com/sqlfluff/sqlfluff/pull/5794) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix placeholder labelling [#5813](https://github.com/sqlfluff/sqlfluff/pull/5813) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Tighten up the return from .process() [#5810](https://github.com/sqlfluff/sqlfluff/pull/5810) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* BigQuery: Support CREATE MATERIALIZED VIEW AS REPLICA OF [#5811](https://github.com/sqlfluff/sqlfluff/pull/5811) [@kzosabe](https://github.com/kzosabe)
+* BigQuery: Support OPTIONS in CREATE FUNCTION statement [#5812](https://github.com/sqlfluff/sqlfluff/pull/5812) [@kzosabe](https://github.com/kzosabe)
+* TSQL: fix `ALTER TABLE ... SWITCH PARTITION` [#5807](https://github.com/sqlfluff/sqlfluff/pull/5807) [@keen85](https://github.com/keen85)
+* SparkSQL: Add functions that use UNIT keywords [#5806](https://github.com/sqlfluff/sqlfluff/pull/5806) [@keraion](https://github.com/keraion)
+* CLI: Add `--stdin-filename` option [#5805](https://github.com/sqlfluff/sqlfluff/pull/5805) [@keraion](https://github.com/keraion)
+* TSQL: parse `CREATE/ALTER/DROP MASTER KEY` [#5802](https://github.com/sqlfluff/sqlfluff/pull/5802) [@keen85](https://github.com/keen85)
+* Jinja Variant Configuration [#5785](https://github.com/sqlfluff/sqlfluff/pull/5785) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Small refactor in jinja templater [#5786](https://github.com/sqlfluff/sqlfluff/pull/5786) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* BigQuery: Support FOR SYSTEM_TIME AS OF in CREATE TABLE CLONE statement [#5798](https://github.com/sqlfluff/sqlfluff/pull/5798) [@kzosabe](https://github.com/kzosabe)
+* TSQL: support for `CREATE/ALTER PARTITION FUNCTION/SCHEME` [#5793](https://github.com/sqlfluff/sqlfluff/pull/5793) [@keen85](https://github.com/keen85)
+* BigQuery: Support DEFAULT COLLATE segment [#5790](https://github.com/sqlfluff/sqlfluff/pull/5790) [@kzosabe](https://github.com/kzosabe)
+* TSQL: support computed columns [#5792](https://github.com/sqlfluff/sqlfluff/pull/5792) [@keen85](https://github.com/keen85)
+* Simplify one of the lexer methods [#5788](https://github.com/sqlfluff/sqlfluff/pull/5788) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Improve light colour highlight [#5784](https://github.com/sqlfluff/sqlfluff/pull/5784) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* SparkSQL: Support TIMESTAMP_LTZ and TIMESTAMP_NTZ types [#5783](https://github.com/sqlfluff/sqlfluff/pull/5783) [@padraic00](https://github.com/padraic00)
+
+## New Contributors
+
+* [@padraic00](https://github.com/padraic00) made their first contribution in [#5783](https://github.com/sqlfluff/sqlfluff/pull/5783)
+* [@burhanyasar](https://github.com/burhanyasar) made their first contribution in [#5830](https://github.com/sqlfluff/sqlfluff/pull/5830)
+
 ## [3.0.5] - 2024-04-19
 
 ## Highlights
 
 This release contains one larger change, which is a big upgrade to case sensitivity in
 the alias use rules. Also allowing the customisation of how SQLFluff uses case sensitivity
 in rules like AL05. Beyond that, this also includes a handful of dialect improvements.
```

### Comparing `sqlfluff-3.0.5/LICENSE.md` & `sqlfluff-3.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/PKG-INFO` & `sqlfluff-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.5
+Version: 3.0.6
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff-3.0.5/README.md` & `sqlfluff-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/pyproject.toml` & `sqlfluff-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sqlfluff"
-version = "3.0.5"
+version = "3.0.6"
 description = "The SQL Linter for Humans"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
   {name = "Alan Cruickshank", email = "alan@designingoverload.com"},
 ]
 license = {file = "LICENSE.md"}
@@ -125,15 +125,15 @@
 sqlfluff_rules_convention = "sqlfluff.rules.convention"
 sqlfluff_rules_jinja = "sqlfluff.rules.jinja"
 sqlfluff_rules_tsql = "sqlfluff.rules.tsql"
 
 
 [tool.sqlfluff_docs]
 # NOTE: Stable version is used by docs/conf.py
-stable_version = "3.0.5"
+stable_version = "3.0.6"
 
 
 [tool.setuptools.package-data]
 sqlfluff = ["core/default_config.cfg", "py.typed"]
 
 
 [tool.importlinter]
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/api/simple.py` & `sqlfluff-3.0.6/src/sqlfluff/api/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -167,24 +167,32 @@
             to use for the operation. Defaults to None.
         config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config,
             which is only used if a `config` is not already provided.
             Defaults to None.
 
     Returns:
         :obj:`Dict[str, Any]` JSON containing the parsed structure.
+
+    Note:
+        In the case of multiple potential variants from the raw source file
+        only the first variant is returned by the simple API. For access to
+        the other variants, use the underlying main API directly.
     """
     cfg = config or get_simple_config(
         dialect=dialect,
         config_path=config_path,
     )
     linter = Linter(config=cfg)
 
     parsed = linter.parse_string(sql)
     # If we encounter any parsing errors, raise them in a combined issue.
-    if parsed.violations:
-        raise APIParsingError(parsed.violations)
+    violations = parsed.violations
+    if violations:
+        raise APIParsingError(violations)
     # Return a JSON representation of the parse tree.
-    if parsed.tree is None:  # pragma: no cover
-        return {}
-    record = parsed.tree.as_record(show_raw=True)
+    # NOTE: For the simple API - only a single variant is returned.
+    root_variant = parsed.root_variant()
+    assert root_variant, "Files parsed without violations must have a valid variant"
+    assert root_variant.tree, "Files parsed without violations must have a valid tree"
+    record = root_variant.tree.as_record(show_raw=True)
     assert record
     return record
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-3.0.6/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/cli/commands.py` & `sqlfluff-3.0.6/src/sqlfluff/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,25 @@
         help=(
             "Override the `library_path` value from the [sqlfluff:templater:jinja]"
             " configuration value. Set this to 'none' to disable entirely."
             " This overrides any values set by users in configuration files or"
             " inline directives."
         ),
     )(f)
+    f = click.option(
+        "--stdin-filename",
+        default=None,
+        help=(
+            "When using stdin as an input, load the configuration as if the contents"
+            " of stdin was in a file in the listed location."
+            " This is useful for some editors that pass file contents from the editor"
+            " that might not match the content on disk."
+        ),
+        type=click.Path(allow_dash=False),
+    )(f)
     return f
 
 
 def lint_options(f: Callable) -> Callable:
     """Add lint operation options to commands via a decorator.
 
     These are cli commands that do linting, i.e. `lint` and `fix`.
@@ -572,14 +583,15 @@
     logger: Optional[logging.Logger] = None,
     bench: bool = False,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
     persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
+    stdin_filename: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Lint SQL files via passing a list of files or using stdin.
 
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
@@ -620,14 +632,16 @@
     # Output the results as we go
     if verbose >= 1 and not non_human_output:
         click.echo(format_linting_result_header())
 
     with PathAndUserErrorHandler(formatter):
         # add stdin if specified via lone '-'
         if ("-",) == paths:
+            if stdin_filename:
+                lnt.config = lnt.config.make_child_from_path(stdin_filename)
             result = lnt.lint_string_wrapped(sys.stdin.read(), fname="stdin")
         else:
             result = lnt.lint_paths(
                 paths,
                 ignore_non_existent_files=False,
                 ignore_files=not disregard_sqlfluffignores,
                 processes=processes,
@@ -1028,14 +1042,15 @@
     logger: Optional[logging.Logger] = None,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
     persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     show_lint_violations: bool = False,
+    stdin_filename: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Fix SQL files.
 
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
@@ -1082,14 +1097,16 @@
             ),
             err=True,
         )
 
     with PathAndUserErrorHandler(formatter):
         # handle stdin case. should output formatted sql to stdout and nothing else.
         if fixing_stdin:
+            if stdin_filename:
+                lnt.config = lnt.config.make_child_from_path(stdin_filename)
             _stdin_fix(lnt, formatter, fix_even_unparsable)
         else:
             _paths_fix(
                 lnt,
                 formatter,
                 paths,
                 processes,
@@ -1119,14 +1136,15 @@
     fixed_suffix: str = "",
     logger: Optional[logging.Logger] = None,
     processes: Optional[int] = None,
     disable_progress_bar: Optional[bool] = False,
     persist_timing: Optional[str] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
+    stdin_filename: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Autoformat SQL files.
 
     This effectively force applies `sqlfluff fix` with a known subset of fairly
     stable rules. Enabled rules are ignored, but rule exclusions (via CLI) or
     config are still respected.
@@ -1181,14 +1199,16 @@
         logger=logger,
         stderr_output=fixing_stdin,
     )
 
     with PathAndUserErrorHandler(formatter):
         # handle stdin case. should output formatted sql to stdout and nothing else.
         if fixing_stdin:
+            if stdin_filename:
+                lnt.config = lnt.config.make_child_from_path(stdin_filename)
             _stdin_fix(lnt, formatter, fix_even_unparsable=False)
         else:
             _paths_fix(
                 lnt,
                 formatter,
                 paths,
                 processes,
@@ -1274,14 +1294,15 @@
     write_output: Optional[str],
     bench: bool,
     nofail: bool,
     logger: Optional[logging.Logger] = None,
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     parse_statistics: bool = False,
+    stdin_filename: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Parse SQL files and just spit out the result.
 
     PATH is the path to a sql file or directory to lint. This can be either a
     file ('path/to/file.sql'), a path ('directory/of/sql/files'), a single ('-')
     character to indicate reading from *stdin* or a dot/blank ('.'/' ') which will
@@ -1310,19 +1331,22 @@
     )
 
     t0 = time.monotonic()
 
     # handle stdin if specified via lone '-'
     with PathAndUserErrorHandler(formatter):
         if "-" == path:
+            file_config = lnt.config
+            if stdin_filename:
+                file_config = file_config.make_child_from_path(stdin_filename)
             parsed_strings = [
                 lnt.parse_string(
                     sys.stdin.read(),
                     "stdin",
-                    config=lnt.config,
+                    config=file_config,
                     parse_statistics=parse_statistics,
                 ),
             ]
         else:
             # A single path must be specified for this command
             parsed_strings = list(
                 lnt.parse_path(
@@ -1336,27 +1360,32 @@
 
     # iterative print for human readout
     if format == FormatType.human.value:
         violations_count = formatter.print_out_violations_and_timing(
             output_stream, bench, code_only, total_time, verbose, parsed_strings
         )
     else:
-        parsed_strings_dict = [
-            dict(
-                filepath=linted_result.fname,
-                segments=(
-                    linted_result.tree.as_record(
-                        code_only=code_only, show_raw=True, include_meta=include_meta
-                    )
-                    if linted_result.tree
-                    else None
-                ),
+        parsed_strings_dict = []
+        for parsed_string in parsed_strings:
+            # TODO: Multiple variants aren't yet supported here in the non-human
+            # output of the parse command.
+            root_variant = parsed_string.root_variant()
+            # Updating violation count ensures the correct return code below.
+            violations_count += len(parsed_string.violations)
+            if root_variant:
+                assert root_variant.tree
+                segments = root_variant.tree.as_record(
+                    code_only=code_only, show_raw=True, include_meta=include_meta
+                )
+            else:
+                # Parsing failed - return null for segments.
+                segments = None
+            parsed_strings_dict.append(
+                {"filepath": parsed_string.fname, "segments": segments}
             )
-            for linted_result in parsed_strings
-        ]
 
         if format == FormatType.yaml.value:
             # For yaml dumping always dump double quoted strings if they contain
             # tabs or newlines.
             yaml.add_representer(str, quoted_presenter)
             file_output = yaml.dump(parsed_strings_dict, sort_keys=False)
         elif format == FormatType.json.value:
@@ -1427,15 +1456,33 @@
         rendered = lnt.render_string(raw_sql, fname, file_config, "utf8")
 
         if rendered.templater_violations:
             for v in rendered.templater_violations:
                 click.echo(formatter.format_violation(v))
             sys.exit(EXIT_FAIL)
         else:
-            click.echo(rendered.templated_file.templated_str)
+            _num_variants = len(rendered.templated_variants)
+            if _num_variants > 1:
+                click.echo(
+                    formatter.colorize(
+                        f"SQLFluff rendered {_num_variants} variants of this file",
+                        Color.blue,
+                    )
+                )
+                for idx, variant in enumerate(rendered.templated_variants):
+                    click.echo(
+                        formatter.colorize(
+                            f"Variant {idx + 1}:",
+                            Color.blue,
+                        )
+                    )
+                    click.echo(variant)
+            else:
+                # No preamble if there's only one.
+                click.echo(rendered.templated_variants[0])
             sys.exit(EXIT_SUCCESS)
 
 
 # This "__main__" handler allows invoking SQLFluff using "python -m", which
 # simplifies the use of cProfile, e.g.:
 # python -m cProfile -s cumtime -m sqlfluff.cli.commands lint slow_file.sql
 if __name__ == "__main__":
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/cli/formatters.py` & `sqlfluff-3.0.6/src/sqlfluff/cli/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         """Dispatch filenames during a persist operation."""
         # Only show the skip records at higher levels of verbosity
         if self.verbosity >= 2 or result != "SKIP":
             self._dispatch(self.format_filename(filename=filename, success=result))
 
     def _format_path(self, path: str) -> str:
         """Format paths."""
-        return f"=== [ path: {self.colorize(path, Color.lightgrey)} ] ===\n"
+        return f"=== [ path: {self.colorize(path, Color.light)} ] ===\n"
 
     def dispatch_path(self, path: str) -> None:
         """Dispatch paths for display."""
         if self.verbosity > 0:
             self._dispatch(self._format_path(path))
 
     def dispatch_template_header(
@@ -193,22 +193,22 @@
                     filename=fname, success=f"LINTING ({', '.join(rules)})"
                 )
             )
 
     def dispatch_compilation_header(self, templater: str, message: str) -> None:
         """Dispatch the header displayed before linting."""
         self._dispatch(
-            f"=== [{self.colorize(templater, Color.lightgrey)}] {message}"
+            f"=== [{self.colorize(templater, Color.light)}] {message}"
         )  # pragma: no cover
 
     def dispatch_processing_header(self, processes: int) -> None:
         """Dispatch the header displayed before linting."""
         if self.verbosity > 0:
             self._dispatch(  # pragma: no cover
-                f"{self.colorize('effective configured processes: ', Color.lightgrey)} "
+                f"{self.colorize('effective configured processes: ', Color.light)} "
                 f"{processes}"
             )
 
     def dispatch_dialect_warning(self, dialect) -> None:
         """Dispatch a warning for dialects."""
         self._dispatch(self.format_dialect_warning(dialect))  # pragma: no cover
 
@@ -286,15 +286,15 @@
     def cli_table_row(
         self,
         fields: List[Tuple[str, str]],
         col_width,
         max_label_width=10,
         sep_char=": ",
         divider_char=" ",
-        label_color=Color.lightgrey,
+        label_color=Color.light,
         val_align="right",
     ) -> str:
         """Make a row of a CLI table, using wrapped values."""
         # Do some intel first
         cols = len(fields)
         last_col_idx = cols - 1
         wrapped_fields = [
@@ -346,15 +346,15 @@
     def cli_table(
         self,
         fields,
         col_width=20,
         cols=2,
         divider_char=" ",
         sep_char=": ",
-        label_color=Color.lightgrey,
+        label_color=Color.light,
         float_format="{0:.2f}",
         max_label_width=10,
         val_align="right",
     ) -> str:
         """Make a crude ascii table.
 
         Assume that `fields` is an iterable of (label, value) pairs.
@@ -403,15 +403,15 @@
             status_string = success_text if success else "FAIL"
 
         if status_string in ("PASS", "FIXED", success_text):
             status_string = self.colorize(status_string, Color.green)
         elif status_string in ("FAIL", "ERROR"):
             status_string = self.colorize(status_string, Color.red)
 
-        return f"== [{self.colorize(filename, Color.lightgrey)}] {status_string}"
+        return f"== [{self.colorize(filename, Color.light)}] {status_string}"
 
     def format_violation(
         self,
         violation: Union[SQLBaseError, dict],
         max_line_length: int = 90,
     ) -> str:
         """Format a violation.
@@ -437,23 +437,23 @@
         pos_elem = "   -" if line_pos is None else f"{line_pos:4d}"
 
         if warning:
             desc = "WARNING: " + desc  # pragma: no cover
 
         # If the rule has a name, add that the description.
         if name:
-            desc += f" [{self.colorize(name, Color.lightgrey)}]"
+            desc += f" [{self.colorize(name, Color.light)}]"
 
         split_desc = split_string_on_spaces(desc, line_length=max_line_length - 25)
 
         out_buff = ""
         # Grey out the violation if we're ignoring or warning it.
         section_color: Color
         if warning:
-            section_color = Color.lightgrey
+            section_color = Color.light
         else:
             section_color = Color.blue
 
         for idx, line in enumerate(split_desc):
             if idx == 0:
                 rule_code = code.rjust(4)
                 if "PRS" in rule_code:
@@ -512,17 +512,15 @@
     def format_config_vals(self, config_vals) -> str:
         """Format an iterable of config values from a config object."""
         text_buffer = StringIO()
         for i, k, v in config_vals:
             val = "" if v is None else str(v)
             text_buffer.write(
                 ("    " * i)
-                + self.colorize(
-                    pad_line(str(k) + ":", 20, "left"), color=Color.lightgrey
-                )
+                + self.colorize(pad_line(str(k) + ":", 20, "left"), color=Color.light)
                 + pad_line(val, 20, "left")
                 + "\n"
             )
         return text_buffer.getvalue()
 
     def _format_rule_description(self, rule) -> str:
         """Format individual rule.
@@ -532,18 +530,18 @@
         if rule.name:
             name = self.colorize(rule.name, Color.blue)
             description = f"[{name}] {rule.description}"
         else:
             description = rule.description
 
         if rule.groups:
-            groups = self.colorize(", ".join(rule.groups), Color.lightgrey)
+            groups = self.colorize(", ".join(rule.groups), Color.light)
             description += f"\ngroups: {groups}"
         if rule.aliases:
-            aliases = self.colorize(", ".join(rule.aliases), Color.lightgrey)
+            aliases = self.colorize(", ".join(rule.aliases), Color.light)
             description += f" aliases: {aliases}"
         return description
 
     def format_rules(self, linter: Linter, verbose: int = 0) -> str:
         """Format the a set of rules given a `Linter`."""
         text_buffer = StringIO()
         text_buffer.write("==== sqlfluff - rules ====\n")
@@ -589,15 +587,15 @@
     def format_dialect_warning(self, dialect) -> str:
         """Output a warning for parsing errors."""
         return self.colorize(
             (
                 "WARNING: Parsing errors found and dialect is set to "
                 f"'{dialect}'. Have you configured your dialect correctly?"
             ),
-            Color.lightgrey,
+            Color.light,
         )
 
     def print_out_residual_error_counts(
         self, total_errors: int, num_filtered_errors: int, force_stderr: bool = False
     ) -> None:
         """Output the residual error totals for the file.
 
@@ -633,33 +631,61 @@
         output_stream: OutputStream,
         bench: bool,
         code_only: bool,
         total_time: float,
         verbose: int,
         parsed_strings: List[ParsedString],
     ) -> int:
-        """Used by human formatting during the parse."""
+        """Used by human formatting during the `sqlfluff parse` command."""
         violations_count = 0
         timing = TimingSummary()
 
         for parsed_string in parsed_strings:
             timing.add(parsed_string.time_dict)
 
-            if parsed_string.tree:
-                output_stream.write(parsed_string.tree.stringify(code_only=code_only))
-            else:
+            num_variants = len(parsed_string.parsed_variants)
+            root_variant = parsed_string.root_variant()
+            if not root_variant:
                 # TODO: Make this prettier
-                output_stream.write("...Failed to Parse...")  # pragma: no cover
+                output_stream.write(
+                    self.colorize("...Failed to Parse...", Color.red)
+                )  # pragma: no cover
+            elif num_variants == 1:
+                # Backward compatible single parse
+                assert root_variant.tree
+                output_stream.write(root_variant.tree.stringify(code_only=code_only))
+            else:
+                # Multi variant parse setup.
+                output_stream.write(
+                    self.colorize(
+                        f"SQLFluff parsed {num_variants} variants of this file",
+                        Color.blue,
+                    )
+                )
+                for idx, variant in enumerate(parsed_string.parsed_variants):
+                    output_stream.write(
+                        self.colorize(
+                            f"Variant {idx + 1}:",
+                            Color.blue,
+                        )
+                    )
+                    if variant.tree:
+                        output_stream.write(variant.tree.stringify(code_only=code_only))
+                    else:  # pragma: no cover
+                        output_stream.write(
+                            self.colorize("...Failed to Parse...", Color.red)
+                        )
 
-            violations_count += len(parsed_string.violations)
-            if parsed_string.violations:
+            violations = parsed_string.violations
+            violations_count += len(violations)
+            if violations:
                 output_stream.write("==== parsing violations ====")  # pragma: no cover
-            for v in parsed_string.violations:
+            for v in violations:
                 output_stream.write(self.format_violation(v))  # pragma: no cover
-            if parsed_string.violations:
+            if violations:
                 output_stream.write(
                     self.format_dialect_warning(parsed_string.config.get("dialect"))
                 )
 
             if verbose >= 2:
                 output_stream.write("==== timings ====")
                 output_stream.write(self.cli_table(parsed_string.time_dict.items()))
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/cli/helpers.py` & `sqlfluff-3.0.6/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/cli/outputstream.py` & `sqlfluff-3.0.6/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/config.py` & `sqlfluff-3.0.6/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/default_config.cfg` & `sqlfluff-3.0.6/src/sqlfluff/core/default_config.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 # If negative or zero, implies number_of_cpus - specified_number.
 # e.g. -1 means use all processors but one. 0  means all cpus.
 processes = 1
 # Max line length is set by default to be in line with the dbt style guide.
 # https://github.com/dbt-labs/corp/blob/main/dbt_style_guide.md
 # Set to zero or negative to disable checks.
 max_line_length = 80
+# NOTE: Templater Variant rendering should currently be considered EXPERIMENTAL.
+# Only set `render_variant_limit` to more than 1 if you know what you're doing!
+# Implementation of this will also depend on your templater.
+render_variant_limit = 1
 
 [sqlfluff:indentation]
 # See https://docs.sqlfluff.com/en/stable/layout.html#configuring-indent-locations
 indent_unit = space
 tab_space_size = 4
 indented_joins = False
 indented_ctes = False
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/dialects/base.py` & `sqlfluff-3.0.6/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/dialects/common.py` & `sqlfluff-3.0.6/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/errors.py` & `sqlfluff-3.0.6/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/helpers/dict.py` & `sqlfluff-3.0.6/src/sqlfluff/core/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/helpers/file.py` & `sqlfluff-3.0.6/src/sqlfluff/core/helpers/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/helpers/slice.py` & `sqlfluff-3.0.6/src/sqlfluff/core/helpers/slice.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/helpers/string.py` & `sqlfluff-3.0.6/src/sqlfluff/core/helpers/string.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/fix.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """A class to store the idea of a linted file."""
 
     path: str
     violations: List[SQLBaseError]
     timings: Optional[FileTimings]
     tree: Optional[BaseSegment]
     ignore_mask: Optional[IgnoreMask]
-    templated_file: TemplatedFile
+    templated_file: Optional[TemplatedFile]
     encoding: str
 
     def check_tuples(
         self, raise_on_non_linting_violations: bool = True
     ) -> List[CheckTuple]:
         """Make a list of check_tuples.
 
@@ -190,16 +190,17 @@
         There is an important distinction here between Slices and
         Segments. A Slice is a portion of a file which is determined
         by the templater based on which portions of the source file
         are templated or not, and therefore before Lexing and so is
         completely dialect agnostic. A Segment is determined by the
         Lexer from portions of strings after templating.
         """
+        assert self.templated_file, "Fixing a string requires successful templating."
         linter_logger.debug("Original Tree: %r", self.templated_file.templated_str)
-        assert self.tree
+        assert self.tree, "Fixing a string requires successful parsing."
         linter_logger.debug("Fixed Tree: %r", self.tree.raw)
 
         # The sliced file is contiguous in the TEMPLATED space.
         # NB: It has gaps and repeats in the source space.
         # It's also not the FIXED file either.
         linter_logger.debug("### Templated File.")
         for idx, file_slice in enumerate(self.templated_file.sliced_file):
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/linter.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/linter.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,33 +25,40 @@
 from sqlfluff.core.errors import (
     SQLBaseError,
     SQLFluffSkipFile,
     SQLFluffUserError,
     SQLLexError,
     SQLLintError,
     SQLParseError,
+    SQLTemplaterError,
 )
 from sqlfluff.core.helpers.file import get_encoding
-from sqlfluff.core.linter.common import ParsedString, RenderedFile, RuleTuple
+from sqlfluff.core.linter.common import (
+    ParsedString,
+    ParsedVariant,
+    RenderedFile,
+    RuleTuple,
+)
 from sqlfluff.core.linter.fix import apply_fixes, compute_anchor_edit_info
 from sqlfluff.core.linter.linted_dir import LintedDir
 from sqlfluff.core.linter.linted_file import (
     TMP_PRS_ERROR_TYPES,
     FileTimings,
     LintedFile,
 )
 from sqlfluff.core.linter.linting_result import LintingResult
 from sqlfluff.core.parser import Lexer, Parser
 from sqlfluff.core.parser.segments.base import BaseSegment, SourceFix
 from sqlfluff.core.rules import BaseRule, RulePack, get_ruleset
 from sqlfluff.core.rules.noqa import IgnoreMask
 
 if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.dialects import Dialect
     from sqlfluff.core.parser.segments.meta import MetaSegment
-    from sqlfluff.core.templaters import TemplatedFile
+    from sqlfluff.core.templaters import RawTemplater, TemplatedFile
 
 
 WalkableType = Iterable[Tuple[str, Optional[List[str]], List[str]]]
 RuleTimingsType = List[Tuple[str, str, float]]
 
 # Instantiate the linter logger
 linter_logger: logging.Logger = logging.getLogger("sqlfluff.linter")
@@ -80,16 +87,18 @@
             exclude_rules=exclude_rules,
             # Don't require a dialect to be provided yet. Defer this until we
             # are actually linting something, since the directory we are linting
             # from may provide additional configuration, including a dialect.
             require_dialect=False,
         )
         # Get the dialect and templater
-        self.dialect = self.config.get("dialect_obj")
-        self.templater = self.config.get("templater_obj")
+        self.dialect: "Dialect" = cast("Dialect", self.config.get("dialect_obj"))
+        self.templater: "RawTemplater" = cast(
+            "RawTemplater", self.config.get("templater_obj")
+        )
         # Store the formatter for output
         self.formatter = formatter
         # Store references to user rule classes
         self.user_rules = user_rules or []
 
     def get_rulepack(self, config: Optional[FluffConfig] = None) -> RulePack:
         """Get hold of a set of rules."""
@@ -143,74 +152,68 @@
     def _normalise_newlines(string: str) -> str:
         """Normalise newlines to unix-style line endings."""
         return regex.sub(r"\r\n|\r", "\n", string)
 
     @staticmethod
     def _lex_templated_file(
         templated_file: "TemplatedFile", config: FluffConfig
-    ) -> Tuple[Optional[Sequence[BaseSegment]], List[SQLLexError], FluffConfig]:
-        """Lex a templated file.
-
-        NOTE: This potentially mutates the config, so make sure to
-        use the returned one.
-        """
+    ) -> Tuple[Optional[Sequence[BaseSegment]], List[SQLLexError]]:
+        """Lex a templated file."""
         violations = []
         linter_logger.info("LEXING RAW (%s)", templated_file.fname)
         # Get the lexer
         lexer = Lexer(config=config)
         # Lex the file and log any problems
         try:
-            tokens, lex_vs = lexer.lex(templated_file)
+            segments, lex_vs = lexer.lex(templated_file)
+            # NOTE: There will always be segments, even if it's
+            # just an end of file marker.
+            assert segments, "The token sequence should never be empty."
             # We might just get the violations as a list
             violations += lex_vs
-            linter_logger.info(
-                "Lexed tokens: %s", [seg.raw for seg in tokens] if tokens else None
-            )
+            linter_logger.info("Lexed segments: %s", [seg.raw for seg in segments])
         except SQLLexError as err:  # pragma: no cover
             linter_logger.info("LEXING FAILED! (%s): %s", templated_file.fname, err)
             violations.append(err)
-            return None, violations, config
-
-        if not tokens:  # pragma: no cover TODO?
-            return None, violations, config
+            return None, violations
 
         # Check that we've got sensible indentation from the lexer.
         # We might need to suppress if it's a complicated file.
         templating_blocks_indent = config.get("template_blocks_indent", "indentation")
         if isinstance(templating_blocks_indent, str):
             force_block_indent = templating_blocks_indent.lower().strip() == "force"
         else:
             force_block_indent = False
         templating_blocks_indent = bool(templating_blocks_indent)
         # If we're forcing it through we don't check.
         if templating_blocks_indent and not force_block_indent:
-            indent_balance = sum(getattr(elem, "indent_val", 0) for elem in tokens)
+            indent_balance = sum(getattr(elem, "indent_val", 0) for elem in segments)
             if indent_balance != 0:  # pragma: no cover
                 linter_logger.debug(
                     "Indent balance test failed for %r. Template indents will not be "
                     "linted for this file.",
                     templated_file.fname,
                 )
                 # Don't enable the templating blocks.
                 templating_blocks_indent = False
 
         # The file will have been lexed without config, so check all indents
         # are enabled.
-        new_tokens = []
-        for token in tokens:
-            if token.is_meta:
-                token = cast("MetaSegment", token)
-                if token.indent_val != 0:
+        new_segments = []
+        for segment in segments:
+            if segment.is_meta:
+                meta_segment = cast("MetaSegment", segment)
+                if meta_segment.indent_val != 0:
                     # Don't allow it if we're not linting templating block indents.
                     if not templating_blocks_indent:
                         continue  # pragma: no cover
-            new_tokens.append(token)
+            new_segments.append(segment)
 
         # Return new buffer
-        return new_tokens, violations, config
+        return new_segments, violations
 
     @staticmethod
     def _parse_tokens(
         tokens: Sequence[BaseSegment],
         config: FluffConfig,
         fname: Optional[str] = None,
         parse_statistics: bool = False,
@@ -302,52 +305,63 @@
     @classmethod
     def parse_rendered(
         cls,
         rendered: RenderedFile,
         parse_statistics: bool = False,
     ) -> ParsedString:
         """Parse a rendered file."""
-        t0 = time.monotonic()
-        violations = cast(List[SQLBaseError], rendered.templater_violations)
         tokens: Optional[Sequence[BaseSegment]]
-        if rendered.templated_file is not None:
-            tokens, lvs, config = cls._lex_templated_file(
-                rendered.templated_file, rendered.config
-            )
-            violations += lvs
-        else:
-            tokens = None
-
-        t1 = time.monotonic()
-        linter_logger.info("PARSING (%s)", rendered.fname)
+        parsed_variants: List[ParsedVariant] = []
+        _lexing_time = 0.0
+        _parsing_time = 0.0
 
-        if tokens:
-            parsed, pvs = cls._parse_tokens(
-                tokens,
-                rendered.config,
-                fname=rendered.fname,
-                parse_statistics=parse_statistics,
+        for idx, variant in enumerate(rendered.templated_variants):
+            t0 = time.monotonic()
+            linter_logger.info("Parse Rendered. Lexing Variant %s", idx)
+            tokens, lex_errors = cls._lex_templated_file(variant, rendered.config)
+            t1 = time.monotonic()
+            linter_logger.info("Parse Rendered. Parsing Variant %s", idx)
+            if tokens:
+                parsed, parse_errors = cls._parse_tokens(
+                    tokens,
+                    rendered.config,
+                    fname=rendered.fname,
+                    parse_statistics=parse_statistics,
+                )
+            else:  # pragma: no cover
+                parsed = None
+                parse_errors = []
+            _lt = t1 - t0
+            _pt = time.monotonic() - t1
+            linter_logger.info(
+                "Parse Rendered. Variant %s. Lex in %s. Parse in %s.", idx, _lt, _pt
             )
-            violations += pvs
-        else:
-            parsed = None
+            parsed_variants.append(
+                ParsedVariant(
+                    variant,
+                    parsed,
+                    lex_errors,
+                    parse_errors,
+                )
+            )
+            _lexing_time += _lt
+            _parsing_time += _pt
 
         time_dict = {
             **rendered.time_dict,
-            "lexing": t1 - t0,
-            "parsing": time.monotonic() - t1,
+            "lexing": _lexing_time,
+            "parsing": _parsing_time,
         }
         return ParsedString(
-            parsed,
-            violations,
-            time_dict,
-            rendered.templated_file,
-            rendered.config,
-            rendered.fname,
-            rendered.source_str,
+            parsed_variants=parsed_variants,
+            templating_violations=rendered.templater_violations,
+            time_dict=time_dict,
+            config=rendered.config,
+            fname=rendered.fname,
+            source_str=rendered.source_str,
         )
 
     @classmethod
     def lint_fix_parsed(
         cls,
         tree: BaseSegment,
         config: FluffConfig,
@@ -585,41 +599,46 @@
         fix: bool = False,
         formatter: Any = None,
         encoding: str = "utf8",
     ) -> LintedFile:
         """Lint a ParsedString and return a LintedFile."""
         violations = parsed.violations
         time_dict = parsed.time_dict
-        tree: Optional[BaseSegment]
-        if parsed.tree:
+        tree: Optional[BaseSegment] = None
+        # TODO: Eventually enable linting of more than just the first variant.
+        if parsed.parsed_variants:
+            tree = parsed.parsed_variants[0].tree
+            variant = parsed.parsed_variants[0].templated_file
+        else:
+            variant = None
+
+        if tree:
             t0 = time.monotonic()
             linter_logger.info("LINTING (%s)", parsed.fname)
             (
                 tree,
                 initial_linting_errors,
                 ignore_mask,
                 rule_timings,
             ) = cls.lint_fix_parsed(
-                parsed.tree,
+                tree,
                 config=parsed.config,
                 rule_pack=rule_pack,
                 fix=fix,
                 fname=parsed.fname,
-                templated_file=parsed.templated_file,
+                templated_file=variant,
                 formatter=formatter,
             )
             # Update the timing dict
             time_dict["linting"] = time.monotonic() - t0
 
             # We're only going to return the *initial* errors, rather
             # than any generated during the fixing cycle.
             violations += initial_linting_errors
         else:
-            # If no parsed tree, set to None
-            tree = None
             ignore_mask = None
             rule_timings = []
             if not parsed.config.get("disable_noqa"):
                 # Templating and/or parsing have failed. Look for "noqa"
                 # comments (the normal path for identifying these comments
                 # requires access to the parse tree, and because of the failure,
                 # we don't have a parse tree).
@@ -642,15 +661,15 @@
         linted_file = LintedFile(
             parsed.fname,
             # Deduplicate violations
             LintedFile.deduplicate_in_source_space(violations),
             FileTimings(time_dict, rule_timings),
             tree,
             ignore_mask=ignore_mask,
-            templated_file=parsed.templated_file,
+            templated_file=variant,
             encoding=encoding,
         )
 
         # This is the main command line output from linting.
         if formatter:
             formatter.dispatch_file_violations(
                 parsed.fname,
@@ -690,15 +709,15 @@
     # These are tied to a specific instance and so are not necessarily
     # safe to use in parallel operations.
 
     def render_string(
         self, in_str: str, fname: str, config: FluffConfig, encoding: str
     ) -> RenderedFile:
         """Template the file."""
-        linter_logger.info("TEMPLATING RAW [%s] (%s)", self.templater.name, fname)
+        linter_logger.info("Rendering String [%s] (%s)", self.templater.name, fname)
 
         # Start the templating timer
         t0 = time.monotonic()
 
         # Newlines are normalised to unix-style line endings (\n).
         # The motivation is that Jinja normalises newlines during templating and
         # we want consistent mapping between the raw and templated slices.
@@ -716,31 +735,51 @@
                     f"failed. Using {self.templater.name} templater. Templater cannot "
                     "be set in a .sqlfluff file in a subdirectory of the current "
                     "working directory. It can be set in a .sqlfluff in the current "
                     "working directory. See Nesting section of the docs for more "
                     "details."
                 )
             )
+
+        variant_limit = config.get("render_variant_limit")
+        templated_variants: List[TemplatedFile] = []
+        templater_violations: List[SQLTemplaterError] = []
+
         try:
-            templated_file, templater_violations = self.templater.process(
+            for variant, templater_errs in self.templater.process_with_variants(
                 in_str=in_str, fname=fname, config=config, formatter=self.formatter
-            )
-        except SQLFluffSkipFile as s:  # pragma: no cover
-            linter_logger.warning(str(s))
-            templated_file = None
-            templater_violations = []
+            ):
+                if variant:
+                    templated_variants.append(variant)
+                # NOTE: We could very easily end up with duplicate errors between
+                # different variants and this code doesn't currently do any
+                # deduplication between them. That will be resolved in further
+                # testing.
+                # TODO: Resolve potential duplicate templater violations between
+                # variants before we enable jinja variant linting by default.
+                templater_violations += templater_errs
+                if len(templated_variants) >= variant_limit:
+                    # Stop if we hit the limit.
+                    break
+        except SQLTemplaterError as templater_err:
+            # Fatal templating error. Capture it and don't generate a variant.
+            templater_violations.append(templater_err)
+        except SQLFluffSkipFile as skip_file_err:  # pragma: no cover
+            linter_logger.warning(str(skip_file_err))
 
-        if templated_file is None:
+        if not templated_variants:
             linter_logger.info("TEMPLATING FAILED: %s", templater_violations)
 
+        linter_logger.info("Rendered %s variants", len(templated_variants))
+
         # Record time
         time_dict = {"templating": time.monotonic() - t0}
 
         return RenderedFile(
-            templated_file,
+            templated_variants,
             templater_violations,
             config,
             time_dict,
             fname,
             encoding,
             in_str,
         )
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/patch.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/patch.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/linter/runner.py` & `sqlfluff-3.0.6/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/context.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,38 +437,35 @@
                 # NOTE: We mark the indent with the block uuid too.
                 block_uuid=block_stack.top(),
             )
 
         # Before we move on, we might have a _forward_ jump to the next
         # element. That element can handle itself, but we'll add a
         # placeholder for it here before we move on.
-        if next_tfs:
-            # Identify whether we have a skip.
-            skipped_chars = next_tfs.source_slice.start - tfs.source_slice.stop
-            placeholder_str = ""
-            if skipped_chars >= 10:
+        if next_tfs and next_tfs.source_slice.start > tfs.source_slice.stop:
+            # We do so extract the string.
+            placeholder_str = templated_file.source_str[
+                tfs.source_slice.stop : next_tfs.source_slice.start
+            ]
+            # Trim it if it's too long to show.
+            if len(placeholder_str) >= 20:
                 placeholder_str = (
-                    f"... [{skipped_chars} unused template " "characters] ..."
-                )
-            elif skipped_chars:
-                placeholder_str = "..."
-
-            # Handle it if we do.
-            if placeholder_str:
-                lexer_logger.debug("      Forward jump detected. Inserting placeholder")
-                yield TemplateSegment(
-                    pos_marker=PositionMarker(
-                        slice(tfs.source_slice.stop, next_tfs.source_slice.start),
-                        # Zero slice in the template.
-                        tfs.templated_slice,
-                        templated_file,
-                    ),
-                    source_str=placeholder_str,
-                    block_type="skipped_source",
+                    f"... [{len(placeholder_str)} unused template " "characters] ..."
                 )
+            lexer_logger.debug("      Forward jump detected. Inserting placeholder")
+            yield TemplateSegment(
+                pos_marker=PositionMarker(
+                    slice(tfs.source_slice.stop, next_tfs.source_slice.start),
+                    # Zero slice in the template.
+                    tfs.templated_slice,
+                    templated_file,
+                ),
+                source_str=placeholder_str,
+                block_type="skipped_source",
+            )
 
         # Move on
         return
 
     # Always return the slice, even if the source slice was also zero length.  Some
     # templaters might want to pass through totally zero length slices as a way of
     # marking locations in the middle of templated output.
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/markers.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/match_algorithms.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/match_algorithms.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/parser.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/bracketed.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/bracketed.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/common.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/file.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/keyword.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/keyword.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/parser/types.py` & `sqlfluff-3.0.6/src/sqlfluff/core/parser/types.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-3.0.6/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/plugin/host.py` & `sqlfluff-3.0.6/src/sqlfluff/core/plugin/host.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-3.0.6/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/base.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/context.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/fix.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/loader.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/noqa.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/noqa.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/rules/reference.py` & `sqlfluff-3.0.6/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/base.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines the templaters."""
 
 import logging
 from bisect import bisect_left
 from typing import Any, Dict, Iterable, Iterator, List, NamedTuple, Optional, Tuple
 
 from sqlfluff.core.config import FluffConfig
-from sqlfluff.core.errors import SQLFluffSkipFile
+from sqlfluff.core.errors import SQLFluffSkipFile, SQLTemplaterError
 from sqlfluff.core.helpers.slice import zero_slice
 
 # Instantiate the templater logger
 templater_logger = logging.getLogger("sqlfluff.templater")
 
 
 def iter_indices_of_newlines(raw_str: str) -> Iterator[int]:
@@ -515,42 +515,55 @@
     def process(
         self,
         *,
         in_str: str,
         fname: str,
         config: Optional[FluffConfig] = None,
         formatter=None,
-    ) -> Tuple[Optional[TemplatedFile], List]:
+    ) -> Tuple[TemplatedFile, List[SQLTemplaterError]]:
         """Process a string and return a TemplatedFile.
 
-        Note that the arguments are enforced as keywords
-        because Templaters can have differences in their
-        `process` method signature.
+        Note that the arguments are enforced as keywords because Templaters
+        can have differences in their `process` method signature.
         A Templater that only supports reading from a file
         would need the following signature:
             process(*, fname, in_str=None, config=None)
         (arguments are swapped)
 
         Args:
             in_str (:obj:`str`): The input string.
             fname (:obj:`str`, optional): The filename of this string. This is
                 mostly for loading config files at runtime.
             config (:obj:`FluffConfig`): A specific config to use for this
                 templating operation. Only necessary for some templaters.
             formatter (:obj:`CallbackFormatter`): Optional object for output.
 
+        Returns:
+            :obj:`tuple` of :obj:`TemplatedFile` and a list of SQLTemplaterError
+            if templating was successful enough that we may move to attempt parsing.
+
+        Raises:
+            SQLTemplaterError: If templating fails fatally, then this method
+                should raise a :obj:`SQLTemplaterError` instead which will be
+                caught and displayed appropriately.
+
         """
         return TemplatedFile(in_str, fname=fname), []
 
     @large_file_check
     def process_with_variants(
         self, *, in_str: str, fname: str, config=None, formatter=None
-    ) -> Iterator[Tuple[Optional[TemplatedFile], List]]:
-        """Extended version of `process` which returns multiple variants."""
-        raise NotImplementedError  # pragma: no cover
+    ) -> Iterator[Tuple[TemplatedFile, List[SQLTemplaterError]]]:
+        """Extended version of `process` which returns multiple variants.
+
+        Unless explicitly defined, this simply yields the result of .process().
+        """
+        yield self.process(
+            in_str=in_str, fname=fname, config=config, formatter=formatter
+        )
 
     def __eq__(self, other: Any) -> bool:
         """Return true if `other` is of the same class as this one.
 
         NB: This is useful in comparing configs.
         """
         return isinstance(other, self.__class__)
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/jinja.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,44 +3,85 @@
 import copy
 import importlib
 import logging
 import os.path
 import pkgutil
 import sys
 from functools import reduce
-from typing import Callable, Dict, Generator, Iterator, List, Optional, Set, Tuple, cast
+from typing import (
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    cast,
+)
 
 import jinja2.nodes
 from jinja2 import (
     Environment,
     FileSystemLoader,
     TemplateError,
     TemplateSyntaxError,
     meta,
 )
 from jinja2.exceptions import TemplateNotFound, UndefinedError
 from jinja2.ext import Extension
 from jinja2.sandbox import SandboxedEnvironment
 
 from sqlfluff.core.config import FluffConfig
-from sqlfluff.core.errors import SQLBaseError, SQLFluffUserError, SQLTemplaterError
+from sqlfluff.core.errors import SQLFluffUserError, SQLTemplaterError
 from sqlfluff.core.helpers.slice import is_zero_slice, slice_length
 from sqlfluff.core.templaters.base import (
     RawFileSlice,
     TemplatedFile,
     TemplatedFileSlice,
     large_file_check,
 )
 from sqlfluff.core.templaters.python import PythonTemplater
 from sqlfluff.core.templaters.slicers.tracer import JinjaAnalyzer, JinjaTrace
 
 # Instantiate the templater logger
 templater_logger = logging.getLogger("sqlfluff.templater")
 
 
+class UndefinedRecorder:
+    """Similar to jinja2.StrictUndefined, but remembers, not fails."""
+
+    # Tell Jinja this object is safe to call and does not alter data.
+    # https://jinja.palletsprojects.com/en/2.9.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
+    unsafe_callable = False
+    # https://jinja.palletsprojects.com/en/3.0.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
+    alters_data = False
+
+    def __init__(self, name: str, undefined_set: set) -> None:
+        self.name = name
+        # Reference to undefined set to modify, it is assumed that the
+        # calling code keeps a reference to this variable to they can
+        # continue to access it after modification by this class.
+        self.undefined_set = undefined_set
+
+    def __str__(self) -> str:
+        """Treat undefined vars as empty, but remember for later."""
+        self.undefined_set.add(self.name)
+        return ""
+
+    def __getattr__(self, item) -> "UndefinedRecorder":
+        """Don't fail when called, remember instead."""
+        self.undefined_set.add(self.name)
+        return UndefinedRecorder(f"{self.name}.{item}", self.undefined_set)
+
+    def __call__(self, *args, **kwargs) -> "UndefinedRecorder":
+        """Don't fail when called unlike parent class."""
+        return UndefinedRecorder(f"{self.name}()", self.undefined_set)
+
+
 class JinjaTemplater(PythonTemplater):
     """A templater using the jinja2 library.
 
     See: https://jinja.palletsprojects.com/
     """
 
     name = "jinja"
@@ -267,17 +308,15 @@
             # to be parsed TWICE if it uses this variable.
             "is_incremental": lambda: True,
             "this": ThisEmulator(),
         }
         return dbt_builtins
 
     @classmethod
-    def _crawl_tree(
-        cls, tree, variable_names, raw
-    ) -> Generator[SQLTemplaterError, None, None]:
+    def _crawl_tree(cls, tree, variable_names, raw) -> Iterator[SQLTemplaterError]:
         """Crawl the tree looking for occurrences of the undeclared values."""
         # First iterate through children
         for elem in tree.iter_child_nodes():
             yield from cls._crawl_tree(elem, variable_names, raw)
         # Then assess self
         if (
             isinstance(tree, jinja2.nodes.Name)
@@ -488,40 +527,78 @@
 
             This function is a closure capturing internal state from process().
             Note that creating templates involves quite a bit of state known to
             _this_ function but not to JinjaTracer.
 
             https://www.programiz.com/python-programming/closure
             """
-            # Load the template, passing the global context.
             try:
                 template = env.from_string(in_str, globals=live_context)
             except TemplateSyntaxError as err:  # pragma: no cover
-                # Something in the template didn't parse, return the original
-                # and a violation around what happened.
-                # NOTE: Most parsing exceptions will be captured when we call
-                # env.parse() in the .process() method. Hence this exception
-                # handling should never be called.
+                # NOTE: If the template fails to parse, then this clause
+                # will be triggered. However in normal that should never
+                # happen because the template should already have been
+                # validated by the point this is called. Typically that
+                # happens when searching for undefined variables.
                 raise SQLTemplaterError(
-                    f"Failure to parse jinja template: {err}.",
+                    f"Late failure to parse jinja template: {err}.",
                     line_no=err.lineno,
                 )
             return template.render()
 
         return env, live_context, render_func
 
+    def _generate_violations_for_undefined_variables(
+        self,
+        in_str: str,
+        syntax_tree: jinja2.nodes.Template,
+        undefined_variables: Set[str],
+    ) -> List[SQLTemplaterError]:
+        """Generates violations for any undefined variables."""
+        violations: List[SQLTemplaterError] = []
+        if undefined_variables:
+            # Lets go through and find out where they are:
+            for template_err_val in self._crawl_tree(
+                syntax_tree, undefined_variables, in_str
+            ):
+                violations.append(template_err_val)
+        return violations
+
+    @staticmethod
+    def _init_undefined_tracking(
+        live_context: dict,
+        potentially_undefined_variables: Iterable[str],
+        ignore_templating: bool = False,
+    ) -> Set[str]:
+        """Sets up tracing of undefined template variables.
+
+        NOTE: This works by mutating the `live_context` which
+        is being used by the environment.
+        """
+        # NOTE: This set is modified by the `UndefinedRecorder` when run.
+        undefined_variables: Set[str] = set()
+
+        for val in potentially_undefined_variables:
+            if val not in live_context:
+                if ignore_templating:
+                    live_context[val] = DummyUndefined.create(val)
+                else:
+                    live_context[val] = UndefinedRecorder(val, undefined_variables)
+
+        return undefined_variables
+
     @large_file_check
     def process(
         self,
         *,
         in_str: str,
         fname: str,
         config: Optional[FluffConfig] = None,
         formatter=None,
-    ) -> Tuple[Optional[TemplatedFile], list]:
+    ) -> Tuple[TemplatedFile, List[SQLTemplaterError]]:
         """Process a string and return the new string.
 
         Note that the arguments are enforced as keywords
         because Templaters can have differences in their `process`
         method signature. A Templater that only supports reading
         from a file would need the following signature:
             process(*, fname, in_str=None, config=None)
@@ -533,136 +610,91 @@
                 mostly for loading config files at runtime.
             config (FluffConfig): A specific config to use for this
                 templating operation. Only necessary for some templaters.
             formatter (CallbackFormatter): Optional object for output.
 
         Raises:
             ValueError: If the 'config' argument is not provided.
+            SQLTemplaterError: If templating fails fatally, then this method
+                should raise a :obj:`SQLTemplaterError` instead which will be
+                caught and displayed appropriately.
 
         Returns:
-            Tuple[Optional[TemplatedFile], list]: A tuple containing the
+            Tuple[TemplatedFile, List[SQLTemplaterError]]: A tuple containing the
             templated file and a list of violations.
         """
         if not config:  # pragma: no cover
             raise ValueError(
                 "For the jinja templater, the `process()` method requires a config "
                 "object."
             )
 
-        try:
-            env, live_context, render_func = self.construct_render_func(
-                fname=fname, config=config
-            )
-        except SQLTemplaterError as err:
-            return None, [err]
-
-        violations: List[SQLBaseError] = []
+        env, live_context, render_func = self.construct_render_func(
+            fname=fname, config=config
+        )
 
         # Attempt to identify any undeclared variables or syntax errors.
         # The majority of variables will be found during the _crawl_tree
         # step rather than this first Exception which serves only to catch
         # catastrophic errors.
         try:
             syntax_tree = env.parse(in_str)
             potentially_undefined_variables = meta.find_undeclared_variables(
                 syntax_tree
             )
         except Exception as err:
-            unrendered_out = TemplatedFile(
-                source_str=in_str,
-                fname=fname,
-            )
             templater_error = SQLTemplaterError(
                 "Failed to parse Jinja syntax. Correct the syntax or select an "
-                "alternative templater."
+                "alternative templater. Error: " + str(err)
             )
             # Capture a line number if we can.
             if isinstance(err, TemplateSyntaxError):
                 templater_error.line_no = err.lineno
-            return unrendered_out, [templater_error]
-
-        undefined_variables = set()
-
-        class UndefinedRecorder:
-            """Similar to jinja2.StrictUndefined, but remembers, not fails."""
+            raise templater_error
 
-            # Tell Jinja this object is safe to call and does not alter data.
-            # https://jinja.palletsprojects.com/en/2.9.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
-            unsafe_callable = False
-            # https://jinja.palletsprojects.com/en/3.0.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
-            alters_data = False
-
-            @classmethod
-            def create(cls, name: str) -> "UndefinedRecorder":
-                return UndefinedRecorder(name=name)
-
-            def __init__(self, name: str) -> None:
-                self.name = name
-
-            def __str__(self) -> str:
-                """Treat undefined vars as empty, but remember for later."""
-                undefined_variables.add(self.name)
-                return ""
-
-            def __getattr__(self, item) -> "UndefinedRecorder":
-                undefined_variables.add(self.name)
-                return UndefinedRecorder(f"{self.name}.{item}")
-
-            def __call__(self, *args, **kwargs) -> "UndefinedRecorder":
-                return UndefinedRecorder(f"{self.name}()")
-
-        Undefined = (
-            UndefinedRecorder
-            if "templating" not in config.get("ignore")
-            else DummyUndefined
+        undefined_variables = self._init_undefined_tracking(
+            live_context,
+            potentially_undefined_variables,
+            ignore_templating=("templating" in config.get("ignore")),
         )
-        for val in potentially_undefined_variables:
-            if val not in live_context:
-                live_context[val] = Undefined.create(val)  # type: ignore
 
         try:
             # Slice the file once rendered.
             raw_sliced, sliced_file, out_str = self.slice_file(
                 in_str,
                 render_func=render_func,
                 config=config,
             )
-            if undefined_variables:
-                # Lets go through and find out where they are:
-                for template_err_val in self._crawl_tree(
-                    syntax_tree, undefined_variables, in_str
-                ):
-                    violations.append(template_err_val)
             return (
                 TemplatedFile(
                     source_str=in_str,
                     templated_str=out_str,
                     fname=fname,
                     sliced_file=sliced_file,
                     raw_sliced=raw_sliced,
                 ),
-                violations,
+                self._generate_violations_for_undefined_variables(
+                    in_str, syntax_tree, undefined_variables
+                ),
             )
         except (TemplateError, TypeError) as err:
             templater_logger.info("Unrecoverable Jinja Error: %s", err, exc_info=True)
-            template_err: SQLBaseError = SQLTemplaterError(
+            raise SQLTemplaterError(
                 (
                     "Unrecoverable failure in Jinja templating: {}. Have you "
-                    "configured your variables? "
+                    "correctly configured your variables? "
                     "https://docs.sqlfluff.com/en/latest/configuration.html"
                 ).format(err),
                 # We don't have actual line number information, but specify
                 # line 1 so users can ignore with "noqa" if they want. (The
                 # default is line 0, which can't be ignored because it's not
                 # a valid line number.)
                 line_no=1,
                 line_pos=1,
             )
-            violations.append(template_err)
-            return None, violations
 
     def slice_file(
         self, raw_str: str, render_func: Callable[[str], str], config=None, **kwargs
     ) -> Tuple[List[RawFileSlice], List[TemplatedFileSlice], str]:
         """Slice the file to determine regions where we can fix.
 
         Args:
@@ -682,14 +714,102 @@
         templater_logger.info("Slicing File Template")
         templater_logger.debug("    Raw String: %r", raw_str[:80])
         analyzer = self._get_jinja_analyzer(raw_str, self._get_jinja_env(), config)
         tracer = analyzer.analyze(render_func)
         trace = tracer.trace(append_to_templated=kwargs.pop("append_to_templated", ""))
         return trace.raw_sliced, trace.sliced_file, trace.templated_str
 
+    @staticmethod
+    def _rectify_templated_slices(
+        length_deltas: Dict[int, int], sliced_template: List[TemplatedFileSlice]
+    ):
+        """This method rectifies the source slices of a variant template.
+
+        :TRICKY: We want to yield variants that _look like_ they were
+        rendered from the original template. However, they were actually
+        rendered from a modified template, which means they have source
+        indices which won't line up with the source files. We correct that
+        here by using the length deltas generated earlier from the
+        modifications.
+
+        This should ensure that lint issues and fixes for the variants are
+        handled correctly and can be combined with those from the original
+        template.
+        """
+        # NOTE: We sort the stack because it's important that it's in order
+        # because we're going to be popping from one end of it. There's no
+        # guarantee that the items are in a particular order a) because it's
+        # a dict and b) because they may have been generated out of order.
+        delta_stack = sorted(length_deltas.items(), key=lambda t: t[0])
+
+        adjusted_slices: List[TemplatedFileSlice] = []
+        carried_delta = 0
+        for tfs in sliced_template:
+            if delta_stack:
+                idx, d = delta_stack[0]
+                if idx == tfs.source_slice.start + carried_delta:
+                    adjusted_slices.append(
+                        tfs._replace(
+                            # "stretch" the slice by adjusting the end more
+                            # than the start.
+                            source_slice=slice(
+                                tfs.source_slice.start + carried_delta,
+                                tfs.source_slice.stop + carried_delta - d,
+                            )
+                        )
+                    )
+                    carried_delta -= d
+                    delta_stack.pop(0)
+                    continue
+
+            # No delta match. Just shift evenly.
+            adjusted_slices.append(
+                tfs._replace(
+                    source_slice=slice(
+                        tfs.source_slice.start + carried_delta,
+                        tfs.source_slice.stop + carried_delta,
+                    )
+                )
+            )
+        return adjusted_slices
+
+    @staticmethod
+    def _calculate_variant_score(
+        raw_sliced: List[RawFileSlice],
+        sliced_file: List[TemplatedFileSlice],
+        uncovered_slices: Set[int],
+        original_source_slices: Dict[int, slice],
+    ) -> int:
+        """Compute a score for the variant based from size of covered slices.
+
+        NOTE: We need to map this back to the positions in the original
+        file, and only have the positions in the modified file here.
+        That means we go translate back via the slice index in raw file.
+        """
+        # First, work out the literal positions in the modified file which
+        # are now covered.
+        covered_source_positions = {
+            tfs.source_slice.start
+            for tfs in sliced_file
+            if tfs.slice_type == "literal" and not is_zero_slice(tfs.templated_slice)
+        }
+        # Second, convert these back into indices so we can use them to
+        # refer to the unmodified source file.
+        covered_raw_slice_idxs = [
+            idx
+            for idx, raw_slice in enumerate(raw_sliced)
+            if raw_slice.source_idx in covered_source_positions
+        ]
+
+        return sum(
+            slice_length(original_source_slices[idx])
+            for idx in covered_raw_slice_idxs
+            if idx in uncovered_slices
+        )
+
     def _handle_unreached_code(
         self,
         in_str: str,
         render_func: Callable[[str], str],
         uncovered_slices: Set[int],
         append_to_templated="",
         config: Optional[FluffConfig] = None,
@@ -709,40 +829,48 @@
             config (:obj:`FluffConfig`, optional): Optional config object.
         """
         analyzer = self._get_jinja_analyzer(in_str, self._get_jinja_env(), config)
         tracer_copy = analyzer.analyze(render_func)
 
         max_variants_generated = 10
         max_variants_returned = 5
-        variants: Dict[str, Tuple[int, JinjaTrace]] = {}
+        variants: Dict[str, Tuple[int, JinjaTrace, Dict[int, int]]] = {}
 
         # Create a mapping of the original source slices before modification so
         # we can adjust the positions post-modification.
         original_source_slices = {
             idx: raw_slice.source_slice()
             for idx, raw_slice in enumerate(tracer_copy.raw_sliced)
         }
 
         for uncovered_slice in sorted(uncovered_slices)[:max_variants_generated]:
             tracer_probe = copy.deepcopy(tracer_copy)
             tracer_trace = copy.deepcopy(tracer_copy)
             override_raw_slices = []
+            # `length_deltas` is to keep track of the length changes associated
+            # with the changes we're making so we can correct the positions in
+            # the resulting template.
+            length_deltas: Dict[int, int] = {}
             # Find a path that takes us to 'uncovered_slice'.
             choices = tracer_probe.move_to_slice(uncovered_slice, 0)
             for branch, options in choices.items():
-                tag = tracer_probe.raw_sliced[branch].tag
-                if tag in ("if", "elif"):
+                raw_file_slice = tracer_probe.raw_sliced[branch]
+                if raw_file_slice.tag in ("if", "elif"):
                     # Replace the existing "if" of "elif" expression with a new,
                     # hardcoded value that hits the target slice in the template
                     # (here that is options[0]).
                     new_value = "True" if options[0] == branch + 1 else "False"
-                    tracer_trace.raw_slice_info[
-                        tracer_probe.raw_sliced[branch]
-                    ].alternate_code = f"{{% {tag} {new_value} %}}"
+                    new_source = f"{{% {raw_file_slice.tag} {new_value} %}}"
+                    tracer_trace.raw_slice_info[raw_file_slice].alternate_code = (
+                        new_source
+                    )
                     override_raw_slices.append(branch)
+                    length_deltas[raw_file_slice.source_idx] = len(new_source) - len(
+                        raw_file_slice.raw
+                    )
 
             # Render and analyze the template with the overrides.
             variant_key = tuple(
                 (
                     cast(str, tracer_trace.raw_slice_info[rs].alternate_code)
                     if idx in override_raw_slices
                     and tracer_trace.raw_slice_info[rs].alternate_code is not None
@@ -767,70 +895,45 @@
                     # If we get an error tracing the variant, skip it. This may
                     # happen for a variety of reasons. Basically there's no
                     # guarantee that the variant will be valid Jinja.
                     continue
                 else:
                     # Compute a score for the variant based on the size of initially
                     # uncovered literal slices it hits.
-                    # NOTE: We need to map this back to the positions in the original
-                    # file, and only have the positions in the modified file here.
-                    # That means we go translate back via the slice index in raw file.
-
-                    # First, work out the literal positions in the modified file which
-                    # are now covered.
-                    _covered_source_positions = {
-                        tfs.source_slice.start
-                        for tfs in trace.sliced_file
-                        if tfs.slice_type == "literal"
-                        and not is_zero_slice(tfs.templated_slice)
-                    }
-                    # Second, convert these back into indices so we can use them to
-                    # refer to the unmodified source file.
-                    _covered_raw_slice_idxs = [
-                        idx
-                        for idx, raw_slice in enumerate(trace.raw_sliced)
-                        if raw_slice.source_idx in _covered_source_positions
-                    ]
-
-                    score = sum(
-                        slice_length(original_source_slices[idx])
-                        for idx in _covered_raw_slice_idxs
-                        if idx in uncovered_slices
+                    score = self._calculate_variant_score(
+                        raw_sliced=trace.raw_sliced,
+                        sliced_file=trace.sliced_file,
+                        uncovered_slices=uncovered_slices,
+                        original_source_slices=original_source_slices,
                     )
 
-                    variants[variant_raw_str] = (score, trace)
+                    variants[variant_raw_str] = (score, trace, length_deltas)
 
         # Return the top-scoring variants.
-        sorted_variants: List[Tuple[int, JinjaTrace]] = sorted(
+        sorted_variants: List[Tuple[int, JinjaTrace, Dict[int, int]]] = sorted(
             variants.values(), key=lambda v: v[0], reverse=True
         )
-        for _, trace in sorted_variants[:max_variants_returned]:
-            # :TRICKY: Yield variants that _look like_ they were rendered from
-            # the original template, but actually were rendered from a modified
-            # template. This should ensure that lint issues and fixes for the
-            # variants are handled correctly and can be combined with those from
-            # the original template.
-            # To do this we run through modified slices and adjust their source
-            # slices to correspond with the original version. We do this by referencing
-            # their slice position in the original file, because we know we haven't
-            # changed the number or ordering of slices, just their length/content.
-            adjusted_slices: List[TemplatedFileSlice] = [
-                tfs._replace(source_slice=original_source_slices[idx])
-                for idx, tfs in enumerate(trace.sliced_file)
-            ]
+        for _, trace, deltas in sorted_variants[:max_variants_returned]:
+            # Rectify the source slices of the generated template, which should
+            # ensure that lint issues and fixes for the variants are handled
+            # correctly and can be combined with those from the original template.
+            adjusted_slices = self._rectify_templated_slices(
+                deltas,
+                trace.sliced_file,
+            )
             yield (
                 tracer_copy.raw_sliced,
                 adjusted_slices,
                 trace.templated_str,
             )
 
     @large_file_check
     def process_with_variants(
         self, *, in_str: str, fname: str, config=None, formatter=None
-    ) -> Iterator[Tuple[Optional[TemplatedFile], List]]:
+    ) -> Iterator[Tuple[Optional[TemplatedFile], List[SQLTemplaterError]]]:
         """Process a string and return one or more variant renderings.
 
         Note that the arguments are enforced as keywords
         because Templaters can have differences in their
         `process` method signature.
         A Templater that only supports reading from a file
         would need the following signature:
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Defines the placeholder template."""
 
 import logging
-from typing import Dict, Optional, Tuple
+from typing import Dict, List, Tuple
 
 import regex
 
+from sqlfluff.core.errors import SQLTemplaterError
 from sqlfluff.core.helpers.slice import offset_slice
 from sqlfluff.core.templaters.base import (
     RawFileSlice,
     RawTemplater,
     TemplatedFile,
     TemplatedFileSlice,
     large_file_check,
@@ -110,15 +111,15 @@
             )
 
         return live_context
 
     @large_file_check
     def process(
         self, *, in_str: str, fname: str, config=None, formatter=None
-    ) -> Tuple[Optional[TemplatedFile], list]:
+    ) -> Tuple[TemplatedFile, List[SQLTemplaterError]]:
         """Process a string and return a TemplatedFile.
 
         Note that the arguments are enforced as keywords
         because Templaters can have differences in their
         `process` method signature.
         A Templater that only supports reading from a file
         would need the following signature:
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/python.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         for k in loaded_context:
             live_context[k] = self.infer_type(live_context[k])
         return live_context
 
     @large_file_check
     def process(
         self, *, in_str: str, fname: str, config=None, formatter=None
-    ) -> Tuple[Optional[TemplatedFile], List]:
+    ) -> Tuple[TemplatedFile, List[SQLTemplaterError]]:
         """Process a string and return a TemplatedFile.
 
         Note that the arguments are enforced as keywords
         because Templaters can have differences in their
         `process` method signature.
         A Templater that only supports reading from a file
         would need the following signature:
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/core/timing.py` & `sqlfluff-3.0.6/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -496,25 +496,34 @@
     match_grammar = ansi.StatementSegment.match_grammar.copy(
         insert=[
             Ref("DeclareStatementSegment"),
             Ref("SetStatementSegment"),
             Ref("ExportStatementSegment"),
             Ref("CreateExternalTableStatementSegment"),
             Ref("CreateSnapshotTableStatementSegment"),
+            Ref("ExecuteImmediateSegment"),
             Ref("AssertStatementSegment"),
             Ref("CallStatementSegment"),
             Ref("ReturnStatementSegment"),
             Ref("BreakStatementSegment"),
             Ref("LeaveStatementSegment"),
             Ref("ContinueStatementSegment"),
             Ref("RaiseStatementSegment"),
             Ref("AlterViewStatementSegment"),
+            Ref("AlterSchemaStatementSegment"),
             Ref("CreateMaterializedViewStatementSegment"),
+            Ref("CreateMaterializedViewAsReplicaOfStatementSegment"),
             Ref("AlterMaterializedViewStatementSegment"),
             Ref("DropMaterializedViewStatementSegment"),
+            Ref("DropProcedureStatementSegment"),
+            Ref("UndropSchemaStatementSegment"),
+            Ref("CreateRowAccessPolicyStatementSegment"),
+            Ref("CreateCapacityStatementSegment"),
+            Ref("CreateReservationStatementSegment"),
+            Ref("CreateAssignmentStatementSegment"),
         ],
     )
 
 
 class AssertStatementSegment(BaseSegment):
     """ASSERT segment.
 
@@ -545,15 +554,15 @@
             OneOf(
                 Ref("StatementSegment"),
                 Ref("MultiStatementSegment"),
             ),
             Ref("DelimiterGrammar"),
         ),
         terminators=[Sequence("END", "FOR")],
-        parse_mode=ParseMode.GREEDY,
+        reset_terminators=True,
     )
 
 
 class ForInStatementSegment(BaseSegment):
     """FOR..IN...DO...END FOR statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#for-in
@@ -588,15 +597,15 @@
             OneOf(
                 Ref("StatementSegment"),
                 Ref("MultiStatementSegment"),
             ),
             Ref("DelimiterGrammar"),
         ),
         terminators=["UNTIL"],
-        parse_mode=ParseMode.GREEDY,
+        reset_terminators=True,
     )
 
 
 class RepeatStatementSegment(BaseSegment):
     """REPEAT...END REPEAT statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#repeat
@@ -631,15 +640,15 @@
             Ref("DelimiterGrammar"),
         ),
         terminators=[
             "ELSE",
             "ELSEIF",
             Sequence("END", "IF"),
         ],
-        parse_mode=ParseMode.GREEDY,
+        reset_terminators=True,
     )
 
 
 class IfStatementSegment(BaseSegment):
     """IF...END IF statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#if
@@ -687,15 +696,15 @@
             OneOf(
                 Ref("StatementSegment"),
                 Ref("MultiStatementSegment"),
             ),
             Ref("DelimiterGrammar"),
         ),
         terminators=[Sequence("END", "LOOP")],
-        parse_mode=ParseMode.GREEDY,
+        reset_terminators=True,
     )
 
 
 class LoopStatementSegment(BaseSegment):
     """LOOP...END LOOP statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#loop
@@ -721,15 +730,15 @@
     type = "while_statements"
     match_grammar = AnyNumberOf(
         Sequence(
             Ref("StatementSegment"),
             Ref("DelimiterGrammar"),
         ),
         terminators=[Sequence("END", "WHILE")],
-        parse_mode=ParseMode.GREEDY,
+        reset_terminators=True,
     )
 
 
 class WhileStatementSegment(BaseSegment):
     """WHILE...END WHILE statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#while
@@ -1059,14 +1068,15 @@
                     Ref("DoubleQuotedUDFBody"),
                     Ref("SingleQuotedUDFBody"),
                     Bracketed(
                         OneOf(Ref("ExpressionSegment"), Ref("SelectStatementSegment"))
                     ),
                 ),
             ),
+            Ref("OptionsSegment", optional=True),
         )
     )
 
 
 class WildcardExpressionSegment(ansi.WildcardExpressionSegment):
     """An extension of the star expression for Bigquery."""
 
@@ -1086,54 +1096,72 @@
     type = "select_except_clause"
     match_grammar = Sequence(
         "EXCEPT",
         Bracketed(Delimited(Ref("SingleIdentifierGrammar"))),
     )
 
 
+class TransactionStatementSegment(ansi.TransactionStatementSegment):
+    """A `BEGIN`, `COMMIT`, or `ROLLBACK` statement."""
+
+    match_grammar = Sequence(
+        OneOf("BEGIN", "COMMIT", "ROLLBACK"),
+        Ref.keyword("TRANSACTION", optional=True),
+        terminators=[Ref("DelimiterGrammar")],
+    )
+
+
 class BeginStatementSegment(BaseSegment):
     """A `BEGIN...EXCEPTION...END` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#beginexceptionend
     """
 
     type = "begin_statement"
 
     match_grammar = Sequence(
-        "BEGIN",
-        Indent,
-        AnyNumberOf(
-            Sequence(
-                Ref("StatementSegment"),
-                Ref("DelimiterGrammar"),
-            ),
-            min_times=1,
-            terminators=["END", "EXCEPTION"],
-            parse_mode=ParseMode.GREEDY,
+        Sequence(
+            Ref("SingleIdentifierFullGrammar"), Ref("ColonSegment"), optional=True
         ),
-        Dedent,
+        "BEGIN",
         Sequence(
-            "EXCEPTION",
-            "WHEN",
-            "ERROR",
-            "THEN",
             Indent,
             AnyNumberOf(
                 Sequence(
-                    Ref("StatementSegment"),
+                    OneOf(Ref("StatementSegment"), Ref("MultiStatementSegment")),
                     Ref("DelimiterGrammar"),
                 ),
+                # We can't terminate on `END` due to possible nesting
+                terminators=["EXCEPTION"],
+                reset_terminators=True,
                 min_times=1,
-                terminators=["END"],
-                parse_mode=ParseMode.GREEDY,
             ),
             Dedent,
+            Sequence(
+                "EXCEPTION",
+                "WHEN",
+                "ERROR",
+                "THEN",
+                Indent,
+                AnyNumberOf(
+                    Sequence(
+                        OneOf(Ref("StatementSegment"), Ref("MultiStatementSegment")),
+                        Ref("DelimiterGrammar"),
+                    ),
+                    min_times=1,
+                    # We can't terminate on `END` due to possible nesting
+                    reset_terminators=True,
+                ),
+                Dedent,
+                optional=True,
+            ),
             optional=True,
         ),
         "END",
+        Ref("SingleIdentifierFullGrammar", optional=True),
     )
 
 
 class ReplaceClauseSegment(BaseSegment):
     """SELECT REPLACE clause."""
 
     type = "select_replace_clause"
@@ -1499,14 +1527,48 @@
                 Ref("ArrayLiteralSegment"),
                 Ref("ExpressionSegment"),
             ),
         ),
     )
 
 
+class ExecuteImmediateSegment(BaseSegment):
+    """An EXECUTE IMMEDIATE statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#execute_immediate
+    """
+
+    type = "execute_immediate"
+    match_grammar = Sequence(
+        "EXECUTE",
+        "IMMEDIATE",
+        OptionallyBracketed(
+            OneOf(
+                Ref("QuotedLiteralSegment"),  # String
+                Ref("SingleIdentifierFullGrammar"),  # Variable
+                Ref("FunctionSegment"),  # Function
+                Ref("CaseExpressionSegment"),  # Conditional Expression
+                Bracketed(Ref("SelectableGrammar")),  # Expression Subquery
+            )
+        ),
+        Sequence("INTO", Delimited(Ref("SingleIdentifierFullGrammar")), optional=True),
+        Sequence(
+            "USING",
+            Delimited(
+                Sequence(
+                    Ref("BaseExpressionElementGrammar"),
+                    # The `AS` is required when using an alias in this context
+                    Sequence("AS", Ref("SingleIdentifierFullGrammar"), optional=True),
+                ),
+            ),
+            optional=True,
+        ),
+    )
+
+
 class PartitionBySegment(BaseSegment):
     """PARTITION BY partition_expression."""
 
     type = "partition_by_segment"
     match_grammar = Sequence(
         "PARTITION",
         "BY",
@@ -1521,14 +1583,46 @@
     match_grammar = Sequence(
         "CLUSTER",
         "BY",
         Delimited(Ref("ExpressionSegment")),
     )
 
 
+class DefaultCollateSegment(BaseSegment):
+    """DEFAULT COLLATE clause for a table or a dataset.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/collation-concepts#default_collation
+    """
+
+    type = "default_collate"
+    match_grammar: Matchable = Sequence(
+        "DEFAULT",
+        "COLLATE",
+        Ref("LiteralGrammar"),
+    )
+
+
+class GrantToSegment(BaseSegment):
+    """GRANT TO (grantee_list).
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_row_access_policy_statement
+    """
+
+    type = "grant_to_segment"
+    match_grammar: Matchable = Sequence(
+        "GRANT",
+        "TO",
+        Bracketed(
+            Delimited(
+                Ref("QuotedLiteralSegment"),
+            ),
+        ),
+    )
+
+
 class OptionsSegment(BaseSegment):
     """OPTIONS clause for a table."""
 
     type = "options_segment"
     match_grammar = Sequence(
         "OPTIONS",
         Bracketed(
@@ -1589,14 +1683,30 @@
 
     match_grammar: Matchable = Sequence(
         Ref("SingleIdentifierGrammar"),  # Column name
         Ref("OptionsSegment", optional=True),
     )
 
 
+class CreateSchemaStatementSegment(ansi.CreateSchemaStatementSegment):
+    """A `CREATE SCHEMA` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_schema_statement
+    """
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "SCHEMA",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("TableReferenceSegment"),
+        Ref("DefaultCollateSegment", optional=True),
+        Ref("OptionsSegment", optional=True),
+    )
+
+
 class CreateTableStatementSegment(ansi.CreateTableStatementSegment):
     """`CREATE TABLE` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_table_statement
     """
 
     match_grammar = Sequence(
@@ -1605,14 +1715,15 @@
         Ref("TemporaryTransientGrammar", optional=True),
         "TABLE",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         Sequence(
             OneOf("COPY", "LIKE", "CLONE"),
             Ref("TableReferenceSegment"),
+            Ref("ForSystemTimeAsOfSegment", optional=True),
             optional=True,
         ),
         # Column list
         Sequence(
             Bracketed(
                 Delimited(
                     OneOf(
@@ -1620,14 +1731,15 @@
                         Ref("TableConstraintSegment"),
                     ),
                     allow_trailing=True,
                 )
             ),
             optional=True,
         ),
+        Ref("DefaultCollateSegment", optional=True),
         Ref("PartitionBySegment", optional=True),
         Ref("ClusterBySegment", optional=True),
         Ref("OptionsSegment", optional=True),
         # Create AS syntax:
         Sequence(
             "AS",
             OptionallyBracketed(Ref("SelectableGrammar")),
@@ -1717,14 +1829,51 @@
                     ),
                 ),
             ),
         ),
     )
 
 
+class AlterSchemaStatementSegment(BaseSegment):
+    """A `ALTER SCHEMA` statement."""
+
+    type = "alter_schema_statement"
+
+    match_grammar: Matchable = Sequence(
+        "ALTER",
+        "SCHEMA",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("TableReferenceSegment"),
+        OneOf(
+            Sequence(
+                "SET",
+                OneOf(
+                    # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_schema_collate_statement
+                    Ref("DefaultCollateSegment"),
+                    # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_schema_set_options_statement
+                    Ref("OptionsSegment"),
+                ),
+            ),
+            # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_schema_add_replica_statement
+            Sequence(
+                "ADD",
+                "REPLICA",
+                Ref("BaseExpressionElementGrammar"),
+                Ref("OptionsSegment", optional=True),
+            ),
+            # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_schema_drop_replica_statement
+            Sequence(
+                "DROP",
+                "REPLICA",
+                Ref("BaseExpressionElementGrammar"),
+            ),
+        ),
+    )
+
+
 class CreateExternalTableStatementSegment(BaseSegment):
     """A `CREATE EXTERNAL TABLE` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_external_table_statement
     """
 
     type = "create_external_table_statement"
@@ -1849,14 +1998,35 @@
         Ref("ClusterBySegment", optional=True),
         Ref("OptionsSegment", optional=True),
         "AS",
         OptionallyBracketed(Ref("SelectableGrammar")),
     )
 
 
+class CreateMaterializedViewAsReplicaOfStatementSegment(BaseSegment):
+    """A `CREATE MATERIALIZED VIEW AS REPLICA OF` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_materialized_view_as_replica_of_statement
+    """
+
+    type = "create_materialized_view_as_replica_of_statement"
+
+    match_grammar = Sequence(
+        "CREATE",
+        "MATERIALIZED",
+        "VIEW",
+        Ref("TableReferenceSegment"),
+        Ref("OptionsSegment", optional=True),
+        "AS",
+        "REPLICA",
+        "OF",
+        Ref("TableReferenceSegment"),
+    )
+
+
 class AlterMaterializedViewStatementSegment(BaseSegment):
     """A `ALTER MATERIALIZED VIEW SET OPTIONS` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_materialized_view_set_options_statement
     """
 
     type = "alter_materialized_view_set_options_statement"
@@ -1868,14 +2038,82 @@
         Ref("IfExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         "SET",
         Ref("OptionsSegment"),
     )
 
 
+class DropTableStatementSegment(BaseSegment):
+    """A `DROP [SNAPSHOT | EXTERNAL] TABLE` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_table_statement
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_snapshot_table_statement
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_external_table_statement
+    """
+
+    type = "drop_table_statement"
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        OneOf("SNAPSHOT", "EXTERNAL", optional=True),
+        "TABLE",
+        Ref("IfExistsGrammar", optional=True),
+        Delimited(Ref("TableReferenceSegment")),
+    )
+
+
+class DropFunctionStatementSegment(BaseSegment):
+    """A `DROP [TABLE] FUNCTION` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_function_statement
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_table_function
+    """
+
+    type = "drop_function_statement"
+
+    match_grammar = Sequence(
+        "DROP",
+        Sequence("TABLE", optional=True),
+        "FUNCTION",
+        Ref("IfExistsGrammar", optional=True),
+        Ref("FunctionNameSegment"),
+    )
+
+
+class DropProcedureStatementSegment(BaseSegment):
+    """A `DROP PROCEDURE` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_procedure_statement
+    """
+
+    type = "drop_procedure_statement"
+
+    match_grammar = Sequence(
+        "DROP",
+        "PROCEDURE",
+        Ref("IfExistsGrammar", optional=True),
+        Ref("ProcedureNameSegment"),
+    )
+
+
+class UndropSchemaStatementSegment(BaseSegment):
+    """A `UNDROP SCHEMA` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#undrop_schema_statement
+    """
+
+    type = "undrop_schema_statement"
+    match_grammar: Matchable = Sequence(
+        "UNDROP",
+        "SCHEMA",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("SchemaReferenceSegment"),
+    )
+
+
 class DropMaterializedViewStatementSegment(BaseSegment):
     """A `DROP MATERIALIZED VIEW` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#drop_materialized_view_statement
     """
 
     type = "drop_materialized_view_statement"
@@ -2247,31 +2485,14 @@
         Delimited(
             Ref("ProcedureParameterGrammar"),
             optional=True,
         )
     )
 
 
-class ProcedureStatements(BaseSegment):
-    """Statements within a CREATE PROCEDURE statement.
-
-    https://cloud.google.com/bigquery/docs/procedures
-    """
-
-    type = "procedure_statements"
-    match_grammar = AnyNumberOf(
-        Sequence(
-            Ref("StatementSegment"),
-            Ref("DelimiterGrammar"),
-        ),
-        terminators=["END"],
-        parse_mode=ParseMode.GREEDY,
-    )
-
-
 class CreateProcedureStatementSegment(BaseSegment):
     """A `CREATE PROCEDURE` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_procedure
     """
 
     type = "create_procedure_statement"
@@ -2279,27 +2500,16 @@
     match_grammar: Matchable = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         "PROCEDURE",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("ProcedureNameSegment"),
         Ref("ProcedureParameterListSegment"),
-        Sequence(
-            "OPTIONS",
-            "strict_mode",
-            StringParser("strict_mode", CodeSegment, type="procedure_option"),
-            Ref("EqualsSegment"),
-            Ref("BooleanLiteralGrammar"),
-            optional=True,
-        ),
-        "BEGIN",
-        Indent,
-        Ref("ProcedureStatements"),
-        Dedent,
-        "END",
+        Ref("OptionsSegment", optional=True),
+        Ref("BeginStatementSegment", reset_terminators=True),
     )
 
 
 class CallStatementSegment(BaseSegment):
     """A `CALL` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/procedural-language#call
@@ -2386,7 +2596,82 @@
             "USING",
             "MESSAGE",
             Ref("EqualsSegment"),
             Ref("ExpressionSegment"),
             optional=True,
         ),
     )
+
+
+class CreateRowAccessPolicyStatementSegment(BaseSegment):
+    """A `CREATE ROW ACCESS POLICY` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_row_access_policy_statement
+    """
+
+    type = "create_row_access_policy_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        Ref("OrReplaceGrammar", optional=True),
+        "ROW",
+        "ACCESS",
+        "POLICY",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("NakedIdentifierSegment"),  # row_access_policy_name
+        "ON",
+        Ref("TableReferenceSegment"),
+        Ref("GrantToSegment", optional=True),
+        "FILTER",
+        "USING",
+        Bracketed(
+            Ref("ExpressionSegment"),
+        ),
+    )
+
+
+class CreateCapacityStatementSegment(BaseSegment):
+    """A `CREATE CAPACITY` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_capacity_statement
+    """
+
+    type = "create_capacity_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "CAPACITY",
+        Ref("TableReferenceSegment"),
+        Ref("OptionsSegment"),
+    )
+
+
+class CreateReservationStatementSegment(BaseSegment):
+    """A `CREATE RESERVATION` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_reservation_statement
+    """
+
+    type = "create_reservation_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "RESERVATION",
+        Ref("TableReferenceSegment"),
+        Ref("OptionsSegment"),
+    )
+
+
+class CreateAssignmentStatementSegment(BaseSegment):
+    """A `CREATE ASSIGNMENT` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_assignment_statement
+    """
+
+    type = "create_assignment_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "ASSIGNMENT",
+        Ref("TableReferenceSegment"),
+        Ref("OptionsSegment"),
+    )
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,29 +98,32 @@
 WHERE
 WINDOW
 WITH
 WITHIN"""
 
 # Note BigQuery doesn't have a list of Unreserved Keywords
 # so these are just ones we need to allow parsing to work
-bigquery_unreserved_keywords = """ACCOUNT
+bigquery_unreserved_keywords = """ACCESS
+ACCOUNT
 ADD
 ADMIN
 AFTER
 ALTER
 APPLY
+ASSIGNMENT
 ASSERT
 AUTO_INCREMENT
 BEGIN
 BERNOULLI
 BINARY
 BINDING
 BREAK
 CACHE
 CALL
+CAPACITY
 CASCADE
 CHAIN
 CHARACTER
 CHECK
 CLONE
 CLUSTER
 COLUMN
@@ -166,14 +169,15 @@
 FUNCTION
 FUTURE
 GRANT
 GRANTED
 GRANTS
 HOUR
 ILIKE
+IMMEDIATE
 IMPORTED
 IN
 INCREMENT
 INDEX
 INOUT
 INSERT
 INTEGRATION
@@ -233,14 +237,16 @@
 READ
 REFERENCE_USAGE
 REFERENCES
 RENAME
 REPEAT
 REPEATABLE
 REPLACE
+REPLICA
+RESERVATION
 RESOURCE
 RESTRICT
 RETURN
 RETURNS
 REVOKE
 RLIKE
 ROLE
@@ -276,14 +282,15 @@
 TIMESTAMP
 TRANSACTION
 TRANSIENT
 TRIGGER
 TRUNCATE
 TUESDAY
 TYPE
+UNDROP
 UNIQUE
 UNSIGNED
 UNTIL
 UPDATE
 USAGE
 USE
 USE_ANY_ROLE
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     BaseSegment,
     Bracketed,
     CodeSegment,
     Conditional,
     Dedent,
     Delimited,
     IdentifierSegment,
+    ImplicitIndent,
     Indent,
     LiteralSegment,
     Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
@@ -34,15 +35,14 @@
 from sqlfluff.dialects.dialect_clickhouse_keywords import UNRESERVED_KEYWORDS
 
 ansi_dialect = load_raw_dialect("ansi")
 
 clickhouse_dialect = ansi_dialect.copy_as("clickhouse")
 clickhouse_dialect.sets("unreserved_keywords").update(UNRESERVED_KEYWORDS)
 
-
 clickhouse_dialect.insert_lexer_matchers(
     # https://clickhouse.com/docs/en/sql-reference/functions#higher-order-functions---operator-and-lambdaparams-expr-function
     [StringLexer("lambda", r"->", SymbolSegment)],
     before="newline",
 )
 
 clickhouse_dialect.patch_lexer_matchers(
@@ -217,17 +217,64 @@
         Ref("SingleQuotedIdentifierSegment"),
         Ref("BackQuotedIdentifierSegment"),
     ),
     InOperatorGrammar=ansi_dialect.get_grammar("InOperatorGrammar").copy(
         insert=[Ref.keyword("GLOBAL", optional=True)],
         before=Ref.keyword("NOT", optional=True),
     ),
+    SelectClauseTerminatorGrammar=ansi_dialect.get_grammar(
+        "SelectClauseTerminatorGrammar"
+    ).copy(
+        insert=[Ref.keyword("PREWHERE")],
+        before=Ref.keyword("WHERE"),
+    ),
+    FromClauseTerminatorGrammar=ansi_dialect.get_grammar(
+        "FromClauseTerminatorGrammar"
+    ).copy(insert=[Ref.keyword("PREWHERE")], before=Ref.keyword("WHERE")),
 )
 
 
+class PreWhereClauseSegment(BaseSegment):
+    """A `PREWHERE` clause like in `SELECT` or `INSERT`."""
+
+    type = "prewhere_clause"
+    match_grammar: Matchable = Sequence(
+        "PREWHERE",
+        # NOTE: The indent here is implicit to allow
+        # constructions like:
+        #
+        #    PREWHERE a
+        #        AND b
+        #
+        # to be valid without forcing an indent between
+        # "PREWHERE" and "a".
+        ImplicitIndent,
+        OptionallyBracketed(Ref("ExpressionSegment")),
+        Dedent,
+    )
+
+
+class SelectStatementSegment(ansi.SelectStatementSegment):
+    """Enhance `SELECT` statement to include QUALIFY."""
+
+    match_grammar = ansi.SelectStatementSegment.match_grammar.copy(
+        insert=[Ref("PreWhereClauseSegment", optional=True)],
+        before=Ref("WhereClauseSegment", optional=True),
+    )
+
+
+class UnorderedSelectStatementSegment(ansi.UnorderedSelectStatementSegment):
+    """Enhance unordered `SELECT` statement to include QUALIFY."""
+
+    match_grammar = ansi.UnorderedSelectStatementSegment.match_grammar.copy(
+        insert=[Ref("PreWhereClauseSegment", optional=True)],
+        before=Ref("WhereClauseSegment", optional=True),
+    )
+
+
 class BracketedArguments(ansi.BracketedArguments):
     """A series of bracketed arguments.
 
     e.g. the bracketed part of numeric(1, 3)
     """
 
     match_grammar = Bracketed(
@@ -740,71 +787,129 @@
 
     As specified in
     https://clickhouse.com/docs/en/sql-reference/statements/create/table/
     """
 
     type = "create_table_statement"
 
-    match_grammar: Matchable = Sequence(
-        "CREATE",
-        OneOf(
-            Ref("OrReplaceGrammar"),
-            Ref.keyword("TEMPORARY"),
-            optional=True,
+    match_grammar: Matchable = OneOf(
+        Sequence(
+            "CREATE",
+            Ref("OrReplaceGrammar", optional=True),
+            "TABLE",
+            Ref("IfNotExistsGrammar", optional=True),
+            Ref("TableReferenceSegment"),
+            Ref("OnClusterClauseSegment", optional=True),
+            OneOf(
+                # CREATE TABLE (...):
+                Sequence(
+                    Bracketed(
+                        Delimited(
+                            OneOf(
+                                Ref("TableConstraintSegment"),
+                                Ref("ColumnDefinitionSegment"),
+                                Ref("ColumnConstraintSegment"),
+                            ),
+                        ),
+                        # Column definition may be missing if using AS SELECT
+                        optional=True,
+                    ),
+                    Ref("TableEngineSegment"),
+                    # CREATE TABLE (...) AS SELECT:
+                    Sequence(
+                        "AS",
+                        Ref("SelectableGrammar"),
+                        optional=True,
+                    ),
+                ),
+                # CREATE TABLE AS other_table:
+                Sequence(
+                    "AS",
+                    Ref("TableReferenceSegment"),
+                    Ref("TableEngineSegment", optional=True),
+                ),
+                # CREATE TABLE AS table_function():
+                Sequence(
+                    "AS",
+                    Ref("FunctionSegment"),
+                ),
+            ),
+            AnySetOf(
+                Sequence(
+                    "COMMENT",
+                    OneOf(
+                        Ref("SingleIdentifierGrammar"),
+                        Ref("QuotedIdentifierSegment"),
+                    ),
+                ),
+                Ref("TableTTLSegment"),
+                optional=True,
+            ),
+            Ref("TableEndClauseSegment", optional=True),
         ),
-        "TABLE",
-        Ref("IfNotExistsGrammar", optional=True),
-        Ref("TableReferenceSegment"),
-        Ref("OnClusterClauseSegment", optional=True),
-        OneOf(
-            # CREATE TABLE (...):
-            Sequence(
-                Bracketed(
-                    Delimited(
-                        OneOf(
-                            Ref("TableConstraintSegment"),
-                            Ref("ColumnDefinitionSegment"),
-                            Ref("ColumnConstraintSegment"),
+        # CREATE TEMPORARY TABLE
+        Sequence(
+            "CREATE",
+            Ref.keyword("TEMPORARY"),
+            "TABLE",
+            Ref("IfNotExistsGrammar", optional=True),
+            Ref("TableReferenceSegment"),
+            OneOf(
+                # CREATE TEMPORARY TABLE (...):
+                Sequence(
+                    Bracketed(
+                        Delimited(
+                            OneOf(
+                                Ref("TableConstraintSegment"),
+                                Ref("ColumnDefinitionSegment"),
+                                Ref("ColumnConstraintSegment"),
+                            ),
                         ),
+                        # Column definition may be missing if using AS SELECT
+                        optional=True,
                     ),
-                    # Column definition may be missing if using AS SELECT
-                    optional=True,
+                    Ref("TableEngineSegment"),
+                    # CREATE TEMPORARY TABLE (...) AS SELECT:
+                    Sequence(
+                        "AS",
+                        Ref("SelectableGrammar"),
+                        optional=True,
+                    ),
+                ),
+                # CREATE TEMPORARY TABLE AS other_table:
+                Sequence(
+                    "AS",
+                    Ref("TableReferenceSegment"),
+                    Ref("TableEngineSegment", optional=True),
                 ),
-                Ref("TableEngineSegment"),
-                # CREATE TABLE (...) AS SELECT:
+                # CREATE TEMPORARY TABLE AS table_function():
+                Sequence(
+                    "AS",
+                    Ref("FunctionSegment"),
+                ),
+                # CREATE TEMPORARY TABLE AS
                 Sequence(
                     "AS",
                     Ref("SelectableGrammar"),
                     optional=True,
                 ),
             ),
-            # CREATE TABLE AS other_table:
-            Sequence(
-                "AS",
-                Ref("TableReferenceSegment"),
-                Ref("TableEngineSegment", optional=True),
-            ),
-            # CREATE TABLE AS table_function():
-            Sequence(
-                "AS",
-                Ref("FunctionSegment"),
-            ),
-        ),
-        AnySetOf(
-            Sequence(
-                "COMMENT",
-                OneOf(
-                    Ref("SingleIdentifierGrammar"),
-                    Ref("QuotedIdentifierSegment"),
+            AnySetOf(
+                Sequence(
+                    "COMMENT",
+                    OneOf(
+                        Ref("SingleIdentifierGrammar"),
+                        Ref("QuotedIdentifierSegment"),
+                    ),
                 ),
+                Ref("TableTTLSegment"),
+                optional=True,
             ),
-            Ref("TableTTLSegment"),
-            optional=True,
+            Ref("TableEndClauseSegment", optional=True),
         ),
-        Ref("TableEndClauseSegment", optional=True),
     )
 
 
 class CreateMaterializedViewStatementSegment(BaseSegment):
     """A `CREATE MATERIALIZED VIEW` statement.
 
     https://clickhouse.com/docs/en/sql-reference/statements/create/table/
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 databricks_dialect.sets("unreserved_keywords").update(
     sparksql_dialect.sets("reserved_keywords")
 )
 databricks_dialect.sets("unreserved_keywords").difference_update(RESERVED_KEYWORDS)
 databricks_dialect.sets("reserved_keywords").clear()
 databricks_dialect.sets("reserved_keywords").update(RESERVED_KEYWORDS)
 
+databricks_dialect.sets("date_part_function_name").update(["TIMEDIFF"])
+
 
 databricks_dialect.add(
     DoubleQuotedUDFBody=TypedParser(
         "double_quote",
         CodeSegment,
         type="udf_body",
         trim_chars=('"',),
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2.py`

 * *Files 9% similar despite different names*

```diff
@@ -218,14 +218,33 @@
                 "TIME",
                 "TIMESTAMP",
                 "TIMEZONE",
                 "USER",
             ),
         ),
     ),
+    XmlIndexSpecificationGrammar=Sequence(
+        "GENERATE",
+        OneOf("KEY", "KEYS"),
+        "USING",
+        "XMLPATTERN",
+        Ref("QuotedLiteralSegment"),  # XmlPatternClause
+        Ref("XmlTypeClauseGrammar"),
+    ),
+    XmlTypeClauseGrammar=Sequence(
+        "AS",
+        "SQL",
+        Ref("DatatypeSegment"),
+        Sequence(
+            OneOf("IGNORE", "REJECT"),
+            "INVALID",
+            "VALUES",
+            optional=True,
+        ),
+    ),
 )
 
 
 class BareFunctionSegment(BaseSegment):
     """A function that can be called without parenthesis per ANSI specification.
 
     DB2 extends this to include `special registers`.
@@ -377,14 +396,94 @@
                 ),
             ),
             "RANDOM",
         ),
     )
 
 
+class IndexColumnDefinitionSegment(ansi.IndexColumnDefinitionSegment):
+    """A column definition for CREATE INDEX."""
+
+    type = "index_column_definition"
+    match_grammar = Sequence(
+        OneOf(
+            Ref("SingleIdentifierGrammar"),  # Column name
+            Ref("ExpressionSegment"),  # key expression
+        ),
+        OneOf("ASC", "DESC", "RANDOM", optional=True),
+    )
+
+
+class CreateIndexStatementSegment(ansi.CreateIndexStatementSegment):
+    """A `CREATE INDEX` statement.
+
+    https://www.ibm.com/docs/en/db2/11.5?topic=statements-create-index
+    """
+
+    type = "create_index_statement"
+    match_grammar = Sequence(
+        "CREATE",
+        Ref.keyword("UNIQUE", optional=True),
+        "INDEX",
+        Ref("IndexReferenceSegment"),
+        "ON",
+        Ref("TableReferenceSegment"),
+        Sequence(
+            Bracketed(
+                Delimited(
+                    Ref("IndexColumnDefinitionSegment"),
+                    Sequence("BUSINESS_TIME", "WITHOUT", "OVERLAPS"),
+                ),
+            )
+        ),
+        AnySetOf(
+            Sequence(Ref.keyword("NOT", optional=True), "PARTITIONED"),
+            Sequence("IN", Ref("TablespaceReferenceSegment")),
+            Sequence("SPECIFICATION", "ONLY"),
+            Sequence(
+                "INCLUDE",
+                Bracketed(
+                    Delimited(
+                        Ref("SingleIdentifierGrammar"),  # Column name
+                        Ref("ExpressionSegment"),  # key expression
+                    )
+                ),
+            ),
+            OneOf(
+                Ref("XmlIndexSpecificationGrammar"),
+                "CLUSTER",
+                Sequence(
+                    "EXTEND",
+                    "USING",
+                    OptionallyBracketed(
+                        Ref("IndexReferenceSegment"),
+                        Bracketed(Delimited(Ref("BaseExpressionElementGrammar"))),
+                    ),
+                ),
+            ),
+            Sequence("PCTFREE", Ref("NumericLiteralSegment")),
+            Sequence("LEVEL2", "PCTFREE", Ref("NumericLiteralSegment")),
+            Sequence("MINPCTUSED", Ref("NumericLiteralSegment")),
+            Sequence(OneOf("ALLOW", "DISALLOW"), "REVERSE", "SCANS"),
+            Sequence("PAGE", "SPLIT", OneOf("SYMMETRIC", "HIGH", "LOW")),
+            Sequence(
+                "COLLECT",
+                Sequence(
+                    OneOf("SAMPLED", "UNSAMPLED", optional=True),
+                    "DETAILED",
+                    optional=True,
+                ),
+                "STATISTICS",
+            ),
+            Sequence("COMPRESS", OneOf("YES", "NO")),
+            Sequence(OneOf("INCLUDE", "EXCLUDE"), "NULL", "KEYS"),
+        ),
+    )
+
+
 class NamedArgumentSegment(BaseSegment):
     """Named argument to a function.
 
     https://www.ibm.com/docs/en/db2/11.5?topic=statements-call
     """
 
     type = "named_argument"
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     "DEFAULTS",
     "DEFINITION",
     "DELETE",
     "DENSERANK",
     "DENSE_RANK",
     "DESCRIBE",
     "DESCRIPTOR",
+    "DETAILED",
     "DETERMINISTIC",
     "DIAGNOSTICS",
     "DISABLE",
     "DISALLOW",
     "DISCONNECT",
     "DISTINCT",
     "DISTRIBUTE",
@@ -132,14 +133,15 @@
     "EXCEPTION",
     "EXCLUDING",
     "EXCLUSIVE",
     "EXECUTE",
     "EXISTS",
     "EXIT",
     "EXPLAIN",
+    "EXTEND",
     "EXTENDED",
     "EXTERNAL",
     "EXTRACT",
     "FEDERATED",
     "FENCED",
     "FETCH",
     "FIELDPROC",
@@ -149,26 +151,28 @@
     "FOR",
     "FOREIGN",
     "FREE",
     "FROM",
     "FULL",
     "FUNCTION",
     "GENERAL",
+    "GENERATE",
     "GENERATED",
     "GET",
     "GLOBAL",
     "GO",
     "GOTO",
     "GRANT",
     "GRAPHIC",
     "GROUP",
     "HANDLER",
     "HASH",
     "HASHED_VALUE",
     "HAVING",
+    "HIGH",
     "HINT",
     "HOLD",
     "HOUR",
     "HOURS",
     "IDENTITY",
     "IF",
     "IMMEDIATE",
@@ -205,14 +209,15 @@
     "LAST",
     "LATERAL",
     "LC_CTYPE",
     "LC_MESSAGES",
     "LC_TIME",
     "LEAVE",
     "LEFT",
+    "LEVEL2",
     "LIKE",
     "LIMIT",
     "LINKTYPE",
     "LOCAL",
     "LOCALDATE",
     "LOCALE",
     "LOCALTIME",
@@ -221,20 +226,22 @@
     "LOCATORS",
     "LOCK",
     "LOCKMAX",
     "LOCKSIZE",
     "LOGGED",
     "LONG",
     "LOOP",
+    "LOW",
     "MAINTAINED",
     "MATERIALIZED",
     "MAXVALUE",
     "MDC",
     "MICROSECOND",
     "MICROSECONDS",
+    "MINPCTUSED",
     "MINUS",
     "MINUTE",
     "MINUTES",
     "MINVALUE",
     "MODE",
     "MODIFIES",
     "MONTH",
@@ -274,14 +281,15 @@
     "ORGANIZE",
     "OUT",
     "OUTER",
     "OVER",
     "OVERRIDING",
     "PACKAGE",
     "PADDED",
+    "PAGE",
     "PAGESIZE",
     "PARAMETER",
     "PART",
     "PARTITION",
     "PARTITIONED",
     "PARTITIONING",
     "PARTITIONS",
@@ -309,25 +317,27 @@
     "RANK",
     "READ",
     "READS",
     "RECOVERY",
     "REFERENCES",
     "REFERENCING",
     "REFRESH",
+    "REJECT",
     "RELEASE",
     "RENAME",
     "REPEAT",
     "RESET",
     "RESIGNAL",
     "RESTART",
     "RESTRICT",
     "RESULT",
     "RESULT_SET_LOCATOR",
     "RETURN",
     "RETURNS",
+    "REVERSE",
     "REVOKE",
     "RIGHT",
     "ROLE",
     "ROLLBACK",
     "ROLLOUT",
     "ROUND_CEILING",
     "ROUND_DOWN",
@@ -342,14 +352,16 @@
     "ROWNUMBER",
     "ROWS",
     "ROWSET",
     "ROW_NUMBER",
     "RRN",
     "RUN",
     "SAVEPOINT",
+    "SAMPLED",
+    "SCANS",
     "SCHEMA",
     "SCRATCHPAD",
     "SCROLL",
     "SEARCH",
     "SECOND",
     "SECONDS",
     "SECQTY",
@@ -363,14 +375,16 @@
     "SIGNAL",
     "SIMPLE",
     "SNAN",
     "SNAPSHOT",
     "SOME",
     "SOURCE",
     "SPECIFIC",
+    "SPECIFICATION",
+    "SPLIT",
     "SQL",
     "SQL_CCFLAGS",
     "SQLID",
     "STACKED",
     "STANDARD",
     "START",
     "STARTING",
@@ -405,14 +419,15 @@
     "TRUNCATE",
     "TYPE",
     "TYPES",
     "UNDO",
     "UNION",
     "UNIQUE",
     "UNTIL",
+    "UNSAMPLED",
     "UPDATE",
     "USAGE",
     "USER",
     "USING",
     "VALIDPROC",
     "VALUE",
     "VALUES",
@@ -431,10 +446,12 @@
     "WITHOUT",
     "WLM",
     "WRITE",
     "XMLELEMENT",
     "XMLEXISTS",
     "XMLNAMESPACES",
     "XMLPARSE",
+    "XMLPATTERN",
     "YEAR",
     "YEARS",
+    "YES",
 ]
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,36 @@
             CodeSegment,
         ),
         RegexLexer(
             "json_operator",
             r"->>|#>>|->|#>|@>|<@|\?\||\?|\?&|#-",
             SymbolSegment,
         ),
+        # r"|".join(
+        #     re.escape(operator)
+        #     for operator in [
+        #         "&&&",
+        #         "&<|",
+        #         "<<|",
+        #         "@",
+        #         "|&>",
+        #         "|>>",
+        #         "~=",
+        #         "<->",
+        #         "|=|",
+        #         "<#>",
+        #         "<<->>",
+        #         "<<#>>",
+        #     ]
+        # )
+        RegexLexer(
+            "postgis_operator",
+            r"\&\&\&|\&<\||<<\||@|\|\&>|\|>>|\~=|<\->|\|=\||<\#>|<<\->>|<<\#>>",
+            SymbolSegment,
+        ),
         StringLexer("at", "@", CodeSegment),
         # https://www.postgresql.org/docs/current/sql-syntax-lexical.html
         RegexLexer(
             "bit_string_literal",
             # binary (e.g. b'1001') or hex (e.g. X'1FF')
             r"[bBxX]'[0-9a-fA-F]*'",
             CodeSegment,
@@ -284,14 +306,17 @@
 # In Postgres, UNNEST() returns a "value table", similar to BigQuery
 postgres_dialect.sets("value_table_functions").update(["UNNEST", "GENERATE_SERIES"])
 
 postgres_dialect.add(
     JsonOperatorSegment=TypedParser(
         "json_operator", SymbolSegment, type="binary_operator"
     ),
+    PostgisOperatorSegment=TypedParser(
+        "postgis_operator", SymbolSegment, type="binary_operator"
+    ),
     SimpleGeometryGrammar=AnyNumberOf(Ref("NumericLiteralSegment")),
     # N.B. this MultilineConcatenateDelimiterGrammar is only created
     # to parse multiline-concatenated string literals
     # and shouldn't be used in other contexts.
     # In general let the parser handle newlines and whitespace.
     MultilineConcatenateNewline=TypedParser(
         "newline",
@@ -373,14 +398,15 @@
         Ref("LikeOperatorSegment"),
         Sequence("IS", "DISTINCT", "FROM"),
         Sequence("IS", "NOT", "DISTINCT", "FROM"),
         Ref("OverlapSegment"),
         Ref("NotExtendRightSegment"),
         Ref("NotExtendLeftSegment"),
         Ref("AdjacentSegment"),
+        Ref("PostgisOperatorSegment"),
     ),
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             # Can’t begin with $, must only contain digits, letters, underscore it $ but
             # can’t be all digits.
             r"([A-Z_]+|[0-9]+[A-Z_$])[A-Z0-9_$]*",
@@ -2416,14 +2442,15 @@
         "EXTENSION",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("ExtensionReferenceSegment"),
         Ref.keyword("WITH", optional=True),
         Sequence("SCHEMA", Ref("SchemaReferenceSegment"), optional=True),
         Sequence("VERSION", Ref("VersionIdentifierSegment"), optional=True),
         Sequence("FROM", Ref("VersionIdentifierSegment"), optional=True),
+        Ref.keyword("CASCADE", optional=True),
     )
 
 
 class DropExtensionStatementSegment(BaseSegment):
     """A `DROP EXTENSION` statement.
 
     https://www.postgresql.org/docs/14/sql-dropextension.html
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -6865,27 +6865,33 @@
         [ USING ( <bind_variable> [ , <bind_variable> ... ] ) ]
 
     EXECUTE IMMEDIATE <variable>
         [ USING ( <bind_variable> [ , <bind_variable> ... ] ) ]
 
     EXECUTE IMMEDIATE $<session_variable>
         [ USING ( <bind_variable> [ , <bind_variable> ... ] ) ]
+
+    EXECUTE IMMEDIATE
+        FROM { absoluteFilePath | relativeFilePath }
     ```
 
     https://docs.snowflake.com/en/sql-reference/sql/execute-immediate
+    https://docs.snowflake.com/en/sql-reference/sql/execute-immediate-from
     """
 
     type = "execute_immediate_clause"
 
     match_grammar = Sequence(
         "EXECUTE",
         "IMMEDIATE",
+        Ref.keyword("FROM", optional=True),
         OneOf(
             Ref("QuotedLiteralSegment"),
             Ref("ReferencedVariableNameSegment"),
+            Ref("StorageLocation"),
             Sequence(
                 Ref("ColonSegment"),
                 Ref("LocalVariableNameSegment"),
             ),
         ),
         Sequence(
             "USING",
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,27 @@
     [
         "CURRENT_DATE",
         "CURRENT_TIMESTAMP",
         "CURRENT_USER",
     ]
 )
 
+# Set the date part functions
+sparksql_dialect.sets("date_part_function_name").clear()
+sparksql_dialect.sets("date_part_function_name").update(
+    [
+        "DATE_ADD",
+        "DATE_DIFF",
+        "DATEADD",
+        "DATEDIFF",
+        "TIMESTAMPADD",
+        "TIMESTAMPDIFF",
+    ]
+)
+
 # Set the datetime units
 sparksql_dialect.sets("datetime_units").clear()
 sparksql_dialect.sets("datetime_units").update(
     [
         "YEAR",
         "YEARS",
         "YYYY",
@@ -194,14 +207,15 @@
         "MON",
         "MM",
         "WEEK",
         "WEEKS",
         "DAY",
         "DAYS",
         "DD",
+        "DAYOFYEAR",
         "HOUR",
         "HOURS",
         "MINUTE",
         "MINUTES",
         "SECOND",
         "SECONDS",
         "MILLISECOND",
@@ -220,14 +234,20 @@
     [
         ("angle", "StartAngleBracketSegment", "EndAngleBracketSegment", False),
     ]
 )
 
 # Real Segments
 sparksql_dialect.replace(
+    DateTimeLiteralGrammar=Sequence(
+        OneOf(
+            "DATE", "TIME", "TIMESTAMP", "INTERVAL", "TIMESTAMP_LTZ", "TIMESTAMP_NTZ"
+        ),
+        TypedParser("single_quote", LiteralSegment, type="date_constructor_literal"),
+    ),
     ComparisonOperatorGrammar=OneOf(
         Ref("EqualsSegment"),
         Ref("EqualsSegment_a"),
         Ref("EqualsSegment_b"),
         Ref("GreaterThanSegment"),
         Ref("LessThanSegment"),
         Ref("GreaterThanOrEqualToSegment"),
@@ -874,14 +894,16 @@
         "INTEGER",
         "BIGINT",
         "FLOAT",
         "REAL",
         "DOUBLE",
         "DATE",
         "TIMESTAMP",
+        "TIMESTAMP_LTZ",
+        "TIMESTAMP_NTZ",
         "STRING",
         Sequence(
             OneOf("CHAR", "CHARACTER", "VARCHAR", "DECIMAL", "DEC", "NUMERIC"),
             Ref("BracketedArguments", optional=True),
         ),
         "BINARY",
         "INTERVAL",
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,16 @@
     "TABLES",
     "TABLESAMPLE",
     "TBLPROPERTIES",
     "TEMP",
     "TEMPORARY",
     "TERMINATED",
     "TIME",
+    "TIMESTAMP_LTZ",
+    "TIMESTAMP_NTZ",
     "TOUCH",
     "TRANSACTION",
     "TRANSACTIONS",
     "TRANSFORM",
     "TRIM",
     "TRUE",
     "TRUNCATE",
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 6% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             type="date_format",
         )
     ),
 )
 
 tsql_dialect.replace(
     # Overriding to cover TSQL allowed identifier name characters
-    # https://docs.microsoft.com/en-us/sql/relational-databases/databases/database-identifiers?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/relational-databases/databases/database-identifiers
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             r"[A-Z_][A-Z0-9_@$#]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^("
@@ -669,14 +669,21 @@
             Ref("CreateExternalTableStatementSegment"),
             Ref("DropExternalTableStatementSegment"),
             Ref("CopyIntoTableStatementSegment"),
             Ref("CreateFullTextIndexStatementSegment"),
             Ref("AtomicBeginEndSegment"),
             Ref("ReconfigureStatementSegment"),
             Ref("CreateColumnstoreIndexStatementSegment"),
+            Ref("CreatePartitionFunctionSegment"),
+            Ref("AlterPartitionSchemeSegment"),
+            Ref("CreatePartitionSchemeSegment"),
+            Ref("AlterPartitionFunctionSegment"),
+            Ref("CreateMasterKeySegment"),
+            Ref("AlterMasterKeySegment"),
+            Ref("DropMasterKeySegment"),
         ],
         remove=[
             Ref("CreateModelStatementSegment"),
             Ref("DropModelStatementSegment"),
             Ref("DescribeStatementSegment"),
         ],
     )
@@ -771,15 +778,15 @@
     """Things that come after SELECT but before the columns."""
 
     type = "select_clause_modifier"
     match_grammar = AnyNumberOf(
         "DISTINCT",
         "ALL",
         Sequence(
-            # https://docs.microsoft.com/en-us/sql/t-sql/queries/top-transact-sql?view=sql-server-ver15
+            # https://docs.microsoft.com/en-us/sql/t-sql/queries/top-transact-sql
             "TOP",
             OptionallyBracketed(Ref("ExpressionSegment")),
             Sequence("PERCENT", optional=True),
             Sequence("WITH", "TIES", optional=True),
         ),
     )
 
@@ -847,15 +854,15 @@
         ),
     )
 
 
 class BulkInsertStatementSegment(BaseSegment):
     """A `BULK INSERT` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql
     """
 
     type = "bulk_insert_statement"
     match_grammar = Sequence(
         "BULK",
         "INSERT",
         Ref("TableReferenceSegment"),
@@ -864,15 +871,15 @@
         Ref("BulkInsertStatementWithSegment", optional=True),
     )
 
 
 class BulkInsertStatementWithSegment(BaseSegment):
     """A `WITH` segment in the BULK INSERT statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/bulk-insert-transact-sql
     """
 
     type = "bulk_insert_with_segment"
     match_grammar = Sequence(
         "WITH",
         Bracketed(
             Delimited(
@@ -977,15 +984,15 @@
         ]
     )
 
 
 class IntoTableSegment(BaseSegment):
     """`INTO` clause within `SELECT`.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/select-into-clause-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/select-into-clause-transact-sql
     """
 
     type = "into_table_clause"
     match_grammar = Sequence("INTO", Ref("ObjectReferenceSegment"))
 
 
 class WhereClauseSegment(BaseSegment):
@@ -1004,16 +1011,16 @@
         Dedent,
     )
 
 
 class CreateIndexStatementSegment(BaseSegment):
     """A `CREATE INDEX` or `CREATE STATISTICS` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-statistics-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-statistics-transact-sql
     """
 
     type = "create_index_statement"
     match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         Sequence("UNIQUE", optional=True),
@@ -1038,15 +1045,15 @@
         Dedent,
     )
 
 
 class CreateColumnstoreIndexStatementSegment(BaseSegment):
     """A `CREATE COLUMNSTORE INDEX` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-columnstore-index-transact-sql?view=sql-server-ver15
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-columnstore-index-transact-sql
     """
 
     type = "create_columnstore_index_statement"
 
     match_grammar = Sequence(
         "CREATE",
         OneOf("CLUSTERED", "NONCLUSTERED", optional=True),
@@ -1129,15 +1136,15 @@
         Ref("OnPartitionOrFilegroupOptionSegment", optional=True),
     )
 
 
 class CreateFullTextIndexStatementSegment(BaseSegment):
     """A `CREATE FULLTEXT INDEX` statement.
 
-    https://learn.microsoft.com/fr-fr/sql/t-sql/statements/create-fulltext-index-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/fr-fr/sql/t-sql/statements/create-fulltext-index-transact-sql
     """
 
     type = "create_fulltext_index_statement"
 
     _catalog_filegroup_option = Sequence(
         "ON",
         Delimited(
@@ -1233,15 +1240,15 @@
     )
 
 
 class AlterIndexStatementSegment(BaseSegment):
     """An ALTER INDEX statement.
 
     As per.
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-index-transact-sql?view=sql-server-ver15
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-index-transact-sql
     """
 
     type = "alter_index_statement"
 
     _low_priority_lock_wait = Sequence(
         "WAIT_AT_LOW_PRIORITY",
         Bracketed(
@@ -1528,31 +1535,31 @@
         ),
     )
 
 
 class OnPartitionOrFilegroupOptionSegment(BaseSegment):
     """ON partition scheme or filegroup option.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     type = "on_partition_or_filegroup_statement"
     match_grammar = OneOf(
         Ref("PartitionSchemeClause"),
         Ref("FilegroupClause"),
         Ref("LiteralGrammar"),  # for "default" value
     )
 
 
 class FilestreamOnOptionSegment(BaseSegment):
     """FILESTREAM_ON index option in `CREATE INDEX` and 'CREATE TABLE' statements.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     type = "filestream_on_option_statement"
     match_grammar = Sequence(
         "FILESTREAM_ON",
         OneOf(
             Ref("FilegroupNameSegment"),
@@ -1564,15 +1571,15 @@
         ),
     )
 
 
 class TextimageOnOptionSegment(BaseSegment):
     """TEXTIMAGE ON option in `CREATE TABLE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     type = "textimage_on_option_statement"
     match_grammar = Sequence(
         "TEXTIMAGE_ON",
         OneOf(
             Ref("FilegroupNameSegment"),
@@ -1580,15 +1587,15 @@
         ),
     )
 
 
 class TableOptionSegment(BaseSegment):
     """TABLE option in `CREATE TABLE` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     _ledger_view_option = Delimited(
         Sequence(
             OneOf(
                 "TRANSACTION_ID_COLUMN_NAME",
                 "SEQUENCE_NUMBER_COLUMN_NAME",
@@ -1791,15 +1798,15 @@
         ),
     )
 
 
 class ReferencesConstraintGrammar(BaseSegment):
     """REFERENCES constraint option in `CREATE TABLE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     type = "references_constraint_grammar"
     match_grammar = Sequence(
         # REFERENCES reftable [ ( refcolumn) ]
         "REFERENCES",
         Ref("TableReferenceSegment"),
@@ -1814,15 +1821,15 @@
         Sequence("NOT", "FOR", "REPLICATION", optional=True),
     )
 
 
 class CheckConstraintGrammar(BaseSegment):
     """CHECK constraint option in `CREATE TABLE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     """
 
     type = "check_constraint_grammar"
     match_grammar = Sequence(
         "CHECK",
         Sequence("NOT", "FOR", "REPLICATION", optional=True),
         Bracketed(
@@ -1830,15 +1837,15 @@
         ),
     )
 
 
 class RelationalIndexOptionsSegment(BaseSegment):
     """A relational index options in `CREATE INDEX` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
     """
 
     type = "relational_index_options"
     match_grammar = Sequence(
         "WITH",
         OptionallyBracketed(
             Delimited(
@@ -1924,15 +1931,15 @@
         ),
     )
 
 
 class MaxDurationSegment(BaseSegment):
     """A `MAX DURATION` clause.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
     """
 
     type = "max_duration"
     match_grammar = Sequence(
         "MAX_DURATION",
         Ref("EqualsSegment"),
         Ref("NumericLiteralSegment"),
@@ -1972,15 +1979,15 @@
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class UpdateStatisticsStatementSegment(BaseSegment):
     """An `UPDATE STATISTICS` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/update-statistics-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/update-statistics-transact-sql
     """
 
     type = "update_statistics_statement"
     match_grammar = Sequence(
         "UPDATE",
         "STATISTICS",
         Ref("ObjectReferenceSegment"),
@@ -1997,15 +2004,15 @@
         Sequence("WITH", OneOf("FULLSCAN", "RESAMPLE"), optional=True),
     )
 
 
 class ReconfigureStatementSegment(BaseSegment):
     """Reconfigure statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/language-elements/reconfigure-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/language-elements/reconfigure-transact-sql
     """
 
     type = "reconfigure_statement"
 
     match_grammar = Sequence(
         "RECONFIGURE",
         Sequence(
@@ -2108,15 +2115,15 @@
 
     type = "pivot_column_reference"
 
 
 class PivotUnpivotStatementSegment(BaseSegment):
     """Declaration of a variable.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/from-using-pivot-and-unpivot?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/from-using-pivot-and-unpivot
     """
 
     type = "from_pivot_expression"
     match_grammar = Sequence(
         OneOf(
             Sequence(
                 "PIVOT",
@@ -2147,15 +2154,15 @@
         Ref("TableReferenceSegment"),
     )
 
 
 class DeclareStatementSegment(BaseSegment):
     """Declaration of a variable.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/declare-local-variable-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/declare-local-variable-transact-sql
     """
 
     type = "declare_segment"
     match_grammar = Sequence(
         "DECLARE",
         Indent,
         Delimited(
@@ -2190,15 +2197,15 @@
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class DeclareCursorStatementSegment(BaseSegment):
     """Declaration of a cursor.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/declare-cursor-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/declare-cursor-transact-sql
     """
 
     type = "declare_segment"
     match_grammar = Sequence(
         "DECLARE",
         Ref("NakedIdentifierSegment"),
         "CURSOR",
@@ -2267,15 +2274,15 @@
         Ref("CharCharacterSetGrammar", optional=True),
     )
 
 
 class CreateSequenceOptionsSegment(BaseSegment):
     """Options for Create Sequence statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-sequence-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-sequence-transact-sql
     """
 
     type = "create_sequence_options_segment"
 
     match_grammar = OneOf(
         Sequence(
             "AS",
@@ -2313,15 +2320,15 @@
         Ref("ObjectReferenceSegment"),
     )
 
 
 class IfExpressionStatement(BaseSegment):
     """IF-ELSE statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/if-else-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/if-else-transact-sql
     """
 
     type = "if_then_statement"
 
     match_grammar = Sequence(
         Ref("IfClauseSegment"),
         Indent,
@@ -2359,15 +2366,15 @@
         Dedent,
     )
 
 
 class WhileExpressionStatement(BaseSegment):
     """WHILE statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/while-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/while-transact-sql
     """
 
     type = "while_statement"
 
     match_grammar = Sequence(
         "WHILE",
         Ref("ExpressionSegment"),
@@ -2376,41 +2383,41 @@
         Dedent,
     )
 
 
 class BreakStatement(BaseSegment):
     """BREAK statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/break-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/break-transact-sql
     """
 
     type = "break_statement"
 
     match_grammar = Sequence(
         "BREAK",
     )
 
 
 class ContinueStatement(BaseSegment):
     """CONTINUE statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/continue-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/continue-transact-sql
     """
 
     type = "continue_statement"
 
     match_grammar = Sequence(
         "CONTINUE",
     )
 
 
 class WaitForStatementSegment(BaseSegment):
     """WAITFOR statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/waitfor-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/waitfor-transact-sql
     Partially implemented, lacking Receive and Get Conversation Group statements for
     now.
     """
 
     type = "waitfor_statement"
 
     match_grammar = Sequence(
@@ -2424,15 +2431,15 @@
 
 
 class ColumnConstraintSegment(BaseSegment):
     """A column option; each CREATE TABLE column can have 0 or more."""
 
     type = "column_constraint_segment"
     # Column constraint from
-    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     match_grammar = Sequence(
         Sequence(
             "CONSTRAINT",
             Ref("ObjectReferenceSegment"),  # Constraint name
             optional=True,
         ),
         OneOf(
@@ -2486,17 +2493,14 @@
             Sequence(
                 "INDEX",
                 Ref("ObjectReferenceSegment"),  # index name
                 OneOf("CLUSTERED", "NONCLUSTERED", optional=True),
                 # other optional blocks (RelationalIndexOptionsSegment,
                 # OnIndexOptionSegment,FilestreamOnOptionSegment) are mentioned above
             ),
-            # computed_column_definition
-            Sequence("AS", Ref("ExpressionSegment")),
-            Sequence("PERSISTED", Sequence("NOT", "NULL", optional=True)),
             # other optional blocks (RelationalIndexOptionsSegment,
             # OnIndexOptionSegment, ReferencesConstraintGrammar, CheckConstraintGrammar)
             # are mentioned above
         ),
     )
 
 
@@ -2529,16 +2533,16 @@
 
     Updated to include AS after declaration of RETURNS. Might be integrated in ANSI
     though.
 
     https://www.postgresql.org/docs/9.1/sql-createfunction.html
     https://docs.snowflake.com/en/sql-reference/sql/create-function.html
     https://cloud.google.com/bigquery/docs/reference/standard-sql/user-defined-functions
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-function-transact-sql?view=sql-server-ver15
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-function-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-function-transact-sql
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-function-transact-sql
     """
 
     type = "create_function_statement"
 
     match_grammar = Sequence(
         OneOf("CREATE", "ALTER", Sequence("CREATE", "OR", "ALTER")),
         "FUNCTION",
@@ -2604,15 +2608,15 @@
         ),
     )
 
 
 class DropFunctionStatementSegment(BaseSegment):
     """A `DROP FUNCTION` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-function-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-function-transact-sql
     """
 
     type = "drop_function_statement"
 
     match_grammar = Sequence(
         "DROP",
         "FUNCTION",
@@ -2632,15 +2636,15 @@
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class ExecuteAsClauseSegment(BaseSegment):
     """An EXECUTE AS clause.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/execute-as-clause-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/execute-as-clause-transact-sql
     """
 
     type = "execute_as_clause"
     match_grammar = Sequence(
         OneOf("EXEC", "EXECUTE"),
         "AS",
         OneOf(
@@ -2652,17 +2656,17 @@
     )
 
 
 class SetStatementSegment(BaseSegment):
     """A Set statement.
 
     Setting an already declared variable or global variable.
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/set-statements-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/set-statements-transact-sql
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/set-local-variable-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/set-local-variable-transact-sql
     """
 
     type = "set_segment"
     match_grammar = Sequence(
         "SET",
         Indent,
         Delimited(
@@ -2737,15 +2741,15 @@
                     OneOf(
                         "ON",
                         "OFF",
                         Sequence(
                             Ref("EqualsSegment"),
                             Ref("ExpressionSegment"),
                         ),
-                        # The below for https://learn.microsoft.com/en-us/sql/t-sql/statements/set-deadlock-priority-transact-sql?view=sql-server-ver16 # noqa
+                        # The below for https://learn.microsoft.com/en-us/sql/t-sql/statements/set-deadlock-priority-transact-sql # noqa
                         "LOW",
                         "NORMAL",
                         "HIGH",
                         Ref("ParameterNameSegment"),
                         Ref("NumericLiteralSegment"),
                         Ref("QualifiedNumericLiteralSegment"),
                     ),
@@ -2810,16 +2814,16 @@
         ),
     )
 
 
 class CreateProcedureStatementSegment(BaseSegment):
     """A `CREATE OR ALTER PROCEDURE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-procedure-transact-sql?view=sql-server-ver15
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-procedure-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-procedure-transact-sql
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-procedure-transact-sql
     """
 
     type = "create_procedure_statement"
 
     _procedure_option = Sequence(
         "WITH",
         Delimited(
@@ -2853,15 +2857,15 @@
         Ref("ProcedureDefinitionGrammar"),
     )
 
 
 class DropProcedureStatementSegment(BaseSegment):
     """A `DROP PROCEDURE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-procedure-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-procedure-transact-sql
     """
 
     type = "drop_procedure_statement"
 
     match_grammar = Sequence(
         "DROP",
         OneOf("PROCEDURE", "PROC"),
@@ -2891,16 +2895,16 @@
     )
 
 
 class CreateViewStatementSegment(BaseSegment):
     """A `CREATE VIEW` statement.
 
     Adjusted to allow CREATE OR ALTER instead of CREATE OR REPLACE.
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-view-transact-sql?view=sql-server-ver15#examples
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-view-transact-sql?view=sql-server-ver15#examples
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-view-transact-sql#examples
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-view-transact-sql#examples
     """
 
     type = "create_view_statement"
     match_grammar = Sequence(
         OneOf("CREATE", "ALTER", Sequence("CREATE", "OR", "ALTER")),
         "VIEW",
         Ref("ObjectReferenceSegment"),
@@ -2998,17 +3002,17 @@
     )
 
 
 class WithinGroupFunctionNameSegment(BaseSegment):
     """WITHIN GROUP function name segment.
 
     For aggregation functions that use the WITHIN GROUP clause.
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/string-agg-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-cont-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-disc-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/string-agg-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-cont-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-disc-transact-sql
 
     Need to be able to specify this as type function_name
     so that linting rules identify it properly
     """
 
     type = "function_name"
     match_grammar = OneOf(
@@ -3018,16 +3022,16 @@
     )
 
 
 class WithinGroupClause(BaseSegment):
     """WITHIN GROUP clause.
 
     For a small set of aggregation functions.
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/string-agg-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-cont-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/string-agg-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/percentile-cont-transact-sql
     """
 
     type = "within_group_clause"
     match_grammar = Sequence(
         "WITHIN",
         "GROUP",
         Bracketed(
@@ -3040,15 +3044,15 @@
         ),
     )
 
 
 class PartitionClauseSegment(ansi.PartitionClauseSegment):
     """PARTITION BY clause.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/select-over-clause-transact-sql?view=sql-server-ver15#partition-by
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/select-over-clause-transact-sql#partition-by
     """
 
     type = "partitionby_clause"
     match_grammar = Sequence(
         "PARTITION",
         "BY",
         Delimited(
@@ -3061,15 +3065,15 @@
         ),
     )
 
 
 class OnPartitionsSegment(BaseSegment):
     """ON PARTITIONS clause.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
     """
 
     type = "on_partitions_clause"
     match_grammar = Sequence(
         "ON",
         "PARTITIONS",
         Bracketed(
@@ -3091,15 +3095,15 @@
     type = "partition_scheme_name"
     match_grammar = Ref("SingleIdentifierGrammar")
 
 
 class PartitionSchemeClause(BaseSegment):
     """Partition Scheme Clause segment.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql
     """
 
     type = "partition_scheme_clause"
     match_grammar = Sequence(
         "ON",
         Ref("PartitionSchemeNameSegment"),
         Bracketed(Ref("ColumnReferenceSegment")),
@@ -3143,28 +3147,28 @@
             "OVER",
             Bracketed(
                 Ref("PartitionClauseSegment", optional=True),
                 Ref("OrderByClauseSegment"),
             ),
         ),
         Sequence(
-            # https://docs.microsoft.com/en-us/sql/t-sql/functions/cast-and-convert-transact-sql?view=sql-server-ver15
+            # https://docs.microsoft.com/en-us/sql/t-sql/functions/cast-and-convert-transact-sql
             Ref("ConvertFunctionNameSegment"),
             Bracketed(
                 Ref("DatatypeSegment"),
                 Bracketed(Ref("NumericLiteralSegment"), optional=True),
                 Ref("CommaSegment"),
                 Ref("ExpressionSegment"),
                 Sequence(
                     Ref("CommaSegment"), Ref("NumericLiteralSegment"), optional=True
                 ),
             ),
         ),
         Sequence(
-            # https://docs.microsoft.com/en-us/sql/t-sql/functions/cast-and-convert-transact-sql?view=sql-server-ver15
+            # https://docs.microsoft.com/en-us/sql/t-sql/functions/cast-and-convert-transact-sql
             Ref("CastFunctionNameSegment"),
             Bracketed(
                 Ref("ExpressionSegment"),
                 "AS",
                 Ref("DatatypeSegment"),
             ),
         ),
@@ -3211,27 +3215,28 @@
     )
 
 
 class CreateTableStatementSegment(BaseSegment):
     """A `CREATE TABLE` statement."""
 
     type = "create_table_statement"
-    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
     # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-azure-sql-data-warehouse?view=aps-pdw-2016-au7
     match_grammar = Sequence(
         "CREATE",
         "TABLE",
         Ref("TableReferenceSegment"),
         OneOf(
             # Columns and comment syntax:
             Sequence(
                 Bracketed(
                     Delimited(
                         OneOf(
                             Ref("TableConstraintSegment"),
+                            Ref("ComputedColumnDefinitionSegment"),
                             Ref("ColumnDefinitionSegment"),
                             Ref("TableIndexSegment"),
                             Ref("PeriodSegment"),
                         ),
                         allow_trailing=True,
                     )
                 ),
@@ -3254,15 +3259,15 @@
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class AlterTableStatementSegment(BaseSegment):
     """An `ALTER TABLE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql
     Overriding ANSI to remove TSQL non-keywords MODIFY, FIRST
     TODO: Flesh out TSQL-specific functionality
     """
 
     type = "alter_table_statement"
     match_grammar = Sequence(
         "ALTER",
@@ -3280,14 +3285,15 @@
                     "ALTER",
                     "COLUMN",
                     Ref("ColumnDefinitionSegment"),
                 ),
                 Sequence(
                     "ADD",
                     Delimited(
+                        Ref("ComputedColumnDefinitionSegment"),
                         Ref("ColumnDefinitionSegment"),
                     ),
                 ),
                 Sequence(
                     "DROP",
                     "COLUMN",
                     Ref("IfExistsGrammar", optional=True),
@@ -3398,15 +3404,15 @@
         ),
     )
 
 
 class TableConstraintSegment(BaseSegment):
     """A table constraint, e.g. for CREATE TABLE."""
 
-    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
 
     type = "table_constraint"
     match_grammar = Sequence(
         Sequence(  # [ CONSTRAINT <Constraint name> ]
             "CONSTRAINT", Ref("ObjectReferenceSegment"), optional=True
         ),
         OneOf(
@@ -3428,15 +3434,15 @@
         ),
     )
 
 
 class TableIndexSegment(BaseSegment):
     """A table index, e.g. for CREATE TABLE."""
 
-    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
 
     type = "table_index_segment"
     match_grammar = Sequence(
         Sequence("INDEX", Ref("ObjectReferenceSegment"), optional=True),
         OneOf(
             Sequence(
                 Sequence("UNIQUE", optional=True),
@@ -3475,28 +3481,28 @@
     type = "filegroup_name"
     match_grammar = Ref("SingleIdentifierGrammar")
 
 
 class FilegroupClause(BaseSegment):
     """Filegroup Clause segment.
 
-    https://docs.microsoft.com/en-us/sql/relational-databases/databases/database-files-and-filegroups?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/relational-databases/databases/database-files-and-filegroups
     """
 
     type = "filegroup_clause"
     match_grammar = Sequence(
         "ON",
         Ref("FilegroupNameSegment"),
     )
 
 
 class IdentityGrammar(BaseSegment):
     """`IDENTITY (1,1)` in table schemas.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property
     """
 
     type = "identity_grammar"
     match_grammar = Sequence(
         "IDENTITY",
         # optional (seed, increment) e.g. (1, 1)
         Bracketed(
@@ -3509,15 +3515,15 @@
         ),
     )
 
 
 class EncryptedWithGrammar(BaseSegment):
     """ENCRYPTED WITH in table schemas.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property
     """
 
     type = "encrypted_with_grammar"
     match_grammar = Sequence(
         "ENCRYPTED",
         "WITH",
         Bracketed(
@@ -3648,28 +3654,54 @@
     )
 
 
 class AlterTableSwitchStatementSegment(BaseSegment):
     """An `ALTER TABLE SWITCH` statement."""
 
     type = "alter_table_switch_statement"
-    # https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql?view=sql-server-ver15
+    # https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-table-transact-sql
     # T-SQL's ALTER TABLE SWITCH grammar is different enough to core ALTER TABLE grammar
     # to merit its own definition
     match_grammar = Sequence(
         "ALTER",
         "TABLE",
         Ref("ObjectReferenceSegment"),
         "SWITCH",
         Sequence("PARTITION", Ref("NumericLiteralSegment"), optional=True),
         "TO",
         Ref("ObjectReferenceSegment"),
-        Sequence(  # Azure Synapse Analytics specific
+        Sequence("PARTITION", Ref("NumericLiteralSegment"), optional=True),
+        Sequence(
             "WITH",
-            Bracketed("TRUNCATE_TARGET", Ref("EqualsSegment"), OneOf("ON", "OFF")),
+            OneOf(
+                Bracketed(
+                    "WAIT_AT_LOW_PRIORITY",
+                    Bracketed(
+                        Delimited(
+                            Sequence(
+                                "MAX_DURATION",
+                                Ref("EqualsSegment"),
+                                Ref("NumericLiteralSegment"),
+                                Ref.keyword("MINUTES", optional=True),
+                            ),
+                            Sequence(
+                                "ABORT_AFTER_WAIT",
+                                Ref("EqualsSegment"),
+                                OneOf("NONE", "SELF", "BLOCKERS"),
+                            ),
+                        ),
+                    ),
+                ),
+                # Azure Synapse Analytics specific:
+                Bracketed(
+                    "TRUNCATE_TARGET",
+                    Ref("EqualsSegment"),
+                    OneOf("ON", "OFF"),
+                ),
+            ),
             optional=True,
         ),
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class CreateTableAsSelectStatementSegment(BaseSegment):
@@ -3696,15 +3728,15 @@
     """A `COMMIT`, `ROLLBACK` or `TRANSACTION` statement."""
 
     type = "transaction_statement"
     match_grammar = OneOf(
         # [ BEGIN | SAVE ] [ TRANSACTION | TRAN ] [ <Name> | <Variable> ]
         # COMMIT [ TRANSACTION | TRAN | WORK ]
         # ROLLBACK [ TRANSACTION | TRAN | WORK ] [ <Name> | <Variable> ]
-        # https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-transaction-transact-sql?view=sql-server-ver15
+        # https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-transaction-transact-sql
         Sequence(
             "BEGIN",
             Sequence("DISTRIBUTED", optional=True),
             Ref("TransactionGrammar"),
             Ref("SingleIdentifierGrammar", optional=True),
             Sequence("WITH", "MARK", Ref("QuotedIdentifierSegment"), optional=True),
             Ref("DelimiterGrammar", optional=True),
@@ -3737,15 +3769,15 @@
     )
 
 
 class BeginEndSegment(BaseSegment):
     """A `BEGIN/END` block.
 
     Encloses multiple statements into a single statement object.
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-end-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-end-transact-sql
     """
 
     type = "begin_end_block"
     match_grammar = Sequence(
         "BEGIN",
         Ref("DelimiterGrammar", optional=True),
         Indent,
@@ -3757,16 +3789,16 @@
 
 class AtomicBeginEndSegment(BaseSegment):
     """A special `BEGIN/END` block with atomic options.
 
     This is only dedicated to natively compiled stored procedures.
 
     Encloses multiple statements into a single statement object.
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-end-transact-sql?view=sql-server-ver15
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-procedure-transact-sql?view=sql-server-ver16#syntax
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-end-transact-sql
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-procedure-transact-sql#syntax
     """
 
     type = "atomic_begin_end_block"
     match_grammar = Sequence(
         "BEGIN",
         Sequence(
             "ATOMIC",
@@ -3817,15 +3849,15 @@
         Sequence("END", optional=True),
     )
 
 
 class TryCatchSegment(BaseSegment):
     """A `TRY/CATCH` block pair.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/try-catch-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/try-catch-transact-sql
     """
 
     type = "try_catch"
     match_grammar = Sequence(
         "BEGIN",
         "TRY",
         Ref("DelimiterGrammar", optional=True),
@@ -3884,15 +3916,15 @@
         ),
     )
 
 
 class OpenRowSetSegment(BaseSegment):
     """A `OPENROWSET` segment.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/functions/openrowset-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/functions/openrowset-transact-sql
     """
 
     type = "openrowset_segment"
     match_grammar = Sequence(
         "OPENROWSET",
         Bracketed(
             OneOf(
@@ -3995,15 +4027,15 @@
         ),
     )
 
 
 class DeleteStatementSegment(BaseSegment):
     """A `DELETE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/delete-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/delete-transact-sql
     Overriding ANSI to remove greedy logic which assumes statements have been
     delimited and to allow for Azure Synapse Analytics-specific DELETE statements
     """
 
     type = "delete_statement"
     # match grammar. This one makes sense in the context of knowing that it's
     # definitely a statement, we just don't know what type yet.
@@ -4222,15 +4254,15 @@
         Dedent,
     )
 
 
 class RenameStatementSegment(BaseSegment):
     """`RENAME` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/rename-transact-sql?view=aps-pdw-2016-au7
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/rename-transact-sql
     Azure Synapse Analytics-specific.
     """
 
     type = "rename_statement"
     match_grammar = Sequence(
         "RENAME",
         "OBJECT",
@@ -4345,30 +4377,30 @@
         Ref("DelimiterGrammar", optional=True),
     )
 
 
 class OptionClauseSegment(BaseSegment):
     """Query Hint clause.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-query?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-query
     """
 
     type = "option_clause"
     match_grammar = Sequence(
         "OPTION",
         Bracketed(
             Delimited(Ref("QueryHintSegment")),
         ),
     )
 
 
 class QueryHintSegment(BaseSegment):
     """Query Hint segment.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-query?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-query
     """
 
     type = "query_hint_segment"
     match_grammar = OneOf(
         Sequence(  # Azure Synapse Analytics specific
             "LABEL",
             Ref("EqualsSegment"),
@@ -4456,15 +4488,15 @@
         ),
     )
 
 
 class PostTableExpressionGrammar(BaseSegment):
     """Table Hint clause.  Overloading the PostTableExpressionGrammar to implement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-table?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-table
     """
 
     type = "post_table_expression"
     match_grammar = Sequence(
         Sequence("WITH", optional=True),
         Bracketed(
             Ref("TableHintSegment"),
@@ -4475,15 +4507,15 @@
         ),
     )
 
 
 class TableHintSegment(BaseSegment):
     """Table Hint segment.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-table?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/hints-transact-sql-table
     """
 
     type = "query_hint_segment"
     match_grammar = OneOf(
         "NOEXPAND",
         Sequence(
             "INDEX",
@@ -4678,15 +4710,15 @@
     )
 
 
 class ExecuteScriptSegment(BaseSegment):
     """`EXECUTE` statement.
 
     Matching segment name and type from exasol.
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/execute-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/execute-transact-sql
     """
 
     type = "execute_script_statement"
     match_grammar = Sequence(
         OneOf("EXEC", "EXECUTE"),
         Sequence(Ref("ParameterNameSegment"), Ref("EqualsSegment"), optional=True),
         OptionallyBracketed(
@@ -4722,15 +4754,15 @@
     )
 
 
 class CreateSchemaStatementSegment(BaseSegment):
     """A `CREATE SCHEMA` statement.
 
     Overriding ANSI to allow for AUTHORIZATION clause
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-schema-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-schema-transact-sql
 
     Not yet implemented: proper schema_element parsing.
     Once we have an AccessStatementSegment that works for TSQL, this definition should
     be tweaked to include schema elements.
     """
 
     type = "create_schema_statement"
@@ -4890,15 +4922,15 @@
         Dedent,
     )
 
 
 class OutputClauseSegment(BaseSegment):
     """OUTPUT Clause used within DELETE, INSERT, UPDATE, MERGE.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/queries/output-clause-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/queries/output-clause-transact-sql
     """
 
     type = "output_clause"
     match_grammar = AnyNumberOf(
         Sequence(
             "OUTPUT",
             Indent,
@@ -4930,15 +4962,15 @@
         ),
     )
 
 
 class ThrowStatementSegment(BaseSegment):
     """A THROW statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/throw-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/throw-transact-sql
     """
 
     type = "throw_statement"
     match_grammar = Sequence(
         "THROW",
         Sequence(
             OneOf(
@@ -4963,15 +4995,15 @@
         ),
     )
 
 
 class RaiserrorStatementSegment(BaseSegment):
     """RAISERROR statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/raiserror-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/raiserror-transact-sql
     """
 
     type = "raiserror_statement"
     match_grammar = Sequence(
         "RAISERROR",
         Bracketed(
             Delimited(
@@ -5025,39 +5057,39 @@
         optional=True,
     )
 
 
 class GotoStatement(BaseSegment):
     """GOTO statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/goto-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/goto-transact-sql
     """
 
     type = "goto_statement"
     match_grammar = Sequence("GOTO", Ref("SingleIdentifierGrammar"))
 
 
 class ExecuteAsClause(BaseSegment):
     """EXECUTE AS Clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/execute-as-clause-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/execute-as-clause-transact-sql
     """
 
     type = "execute_as_clause"
     match_grammar = Sequence(
         "EXECUTE",
         "AS",
         Ref("SingleQuotedIdentifierSegment"),
     )
 
 
 class CreateTriggerStatementSegment(BaseSegment):
     """Create Trigger Statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-trigger-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-trigger-transact-sql
     """
 
     type = "create_trigger"
 
     match_grammar: Matchable = Sequence(
         "CREATE",
         Sequence("OR", "ALTER", optional=True),
@@ -5100,15 +5132,15 @@
         # TODO: EXTERNAL NAME
     )
 
 
 class DropTriggerStatementSegment(BaseSegment):
     """Drop Trigger Statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-trigger-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-trigger-transact-sql
     """
 
     type = "drop_trigger"
 
     match_grammar: Matchable = Sequence(
         "DROP",
         "TRIGGER",
@@ -5117,15 +5149,15 @@
         Sequence("ON", OneOf("DATABASE", Sequence("ALL", "SERVER")), optional=True),
     )
 
 
 class DisableTriggerStatementSegment(BaseSegment):
     """Disable Trigger Statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/disable-trigger-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/disable-trigger-transact-sql
     """
 
     type = "disable_trigger"
 
     match_grammar: Matchable = Sequence(
         "DISABLE",
         "TRIGGER",
@@ -5140,30 +5172,30 @@
         ),
     )
 
 
 class LabelStatementSegment(BaseSegment):
     """Label Statement, for a GOTO statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/goto-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/goto-transact-sql
     """
 
     type = "label_segment"
 
     match_grammar: Matchable = Sequence(
         Ref("NakedIdentifierSegment"), Ref("ColonSegment"), allow_gaps=False
     )
 
 
 class AccessStatementSegment(BaseSegment):
     """A `GRANT` or `REVOKE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/grant-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/deny-transact-sql?view=sql-server-ver15
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/revoke-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/grant-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/deny-transact-sql
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/revoke-transact-sql
     """
 
     type = "access_statement"
 
     # Privileges that can be set on the account (specific to snowflake)
     _global_permissions = OneOf(
         Sequence(
@@ -5330,15 +5362,15 @@
         ),
     )
 
 
 class CreateTypeStatementSegment(BaseSegment):
     """A `CREATE TYPE` statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-type-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-type-transact-sql
     """
 
     type = "create_type_statement"
     match_grammar: Matchable = Sequence(
         "CREATE",
         "TYPE",
         Ref("ObjectReferenceSegment"),
@@ -5363,54 +5395,54 @@
         ),
     )
 
 
 class OpenCursorStatementSegment(BaseSegment):
     """An `OPEN` cursor statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/open-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/open-transact-sql
     """
 
     type = "open_cursor_statement"
     match_grammar: Matchable = Sequence(
         "OPEN",
         Ref("CursorNameGrammar"),
     )
 
 
 class CloseCursorStatementSegment(BaseSegment):
     """A `CLOSE` cursor statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/close-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/close-transact-sql
     """
 
     type = "close_cursor_statement"
     match_grammar: Matchable = Sequence(
         "CLOSE",
         Ref("CursorNameGrammar"),
     )
 
 
 class DeallocateCursorStatementSegment(BaseSegment):
     """A `DEALLOCATE` cursor statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/deallocate-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/deallocate-transact-sql
     """
 
     type = "deallocate_cursor_statement"
     match_grammar: Matchable = Sequence(
         "DEALLOCATE",
         Ref("CursorNameGrammar"),
     )
 
 
 class FetchCursorStatementSegment(BaseSegment):
     """A `FETCH` cursor statement.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/fetch-transact-sql?view=sql-server-ver15
+    https://docs.microsoft.com/en-us/sql/t-sql/language-elements/fetch-transact-sql
     """
 
     type = "fetch_cursor_statement"
     match_grammar: Matchable = Sequence(
         "FETCH",
         OneOf("NEXT", "PRIOR", "FIRST", "LAST", optional=True),
         "FROM",
@@ -5493,15 +5525,15 @@
         ),
     )
 
 
 class TemporalQuerySegment(BaseSegment):
     """A segment that allows Temporal Queries to be run.
 
-    https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal-tables?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/relational-databases/tables/temporal-tables
     """
 
     type = "temporal_query"
 
     match_grammar: Matchable = Sequence(
         "FOR",
         "SYSTEM_TIME",
@@ -5536,15 +5568,15 @@
         ),
     )
 
 
 class CreateDatabaseScopedCredentialStatementSegment(BaseSegment):
     """A statement to create a database scoped credential.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-database-scoped-credential-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-database-scoped-credential-transact-sql
     """
 
     type = "create_database_scoped_credential_statement"
 
     match_grammar: Matchable = Sequence(
         "CREATE",
         "DATABASE",
@@ -5555,15 +5587,15 @@
         Ref("CredentialGrammar"),
     )
 
 
 class CreateExternalDataSourceStatementSegment(BaseSegment):
     """A statement to create an external data source.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-data-source-transact-sql?view=sql-server-ver16&tabs=dedicated#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-data-source-transact-sql&tabs=dedicated#syntax
     """
 
     type = "create_external_data_source_statement"
 
     match_grammar: Matchable = Sequence(
         "CREATE",
         "EXTERNAL",
@@ -5593,16 +5625,16 @@
         ),
     )
 
 
 class PeriodSegment(BaseSegment):
     """A `PERIOD FOR SYSTEM_TIME` for `CREATE TABLE` of temporal tables.
 
-    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver15
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql?view=sql-server-ver16#generated-always-as--row--transaction_id--sequence_number----start--end---hidden---not-null-
+    https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql#generated-always-as--row--transaction_id--sequence_number----start--end---hidden---not-null-
     """
 
     type = "period_segment"
     match_grammar = Sequence(
         "PERIOD",
         "FOR",
         "SYSTEM_TIME",
@@ -5617,15 +5649,15 @@
 
 class SqlcmdCommandSegment(BaseSegment):
     """A `sqlcmd` command.
 
     Microsoft allows professional CI/CD deployment through so called 'SQL Database
     Projects'.
     There are proprietary `sqlcmd Commands` that can be part of an SQL file.
-    https://learn.microsoft.com/en-us/sql/tools/sqlcmd/sqlcmd-utility?view=sql-server-ver16#sqlcmd-commands
+    https://learn.microsoft.com/en-us/sql/tools/sqlcmd/sqlcmd-utility#sqlcmd-commands
     """
 
     type = "sqlcmd_command_segment"
 
     match_grammar: Matchable = OneOf(
         Sequence(
             Sequence(
@@ -5677,15 +5709,15 @@
         ),
     )
 
 
 class ExternalFileFormatDelimitedTextClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *Delimited text* clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=delimited#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=delimited#syntax
     """
 
     type = "external_file_delimited_text_clause"
 
     match_grammar = Delimited(
         Sequence(
             "FORMAT_TYPE",
@@ -5709,15 +5741,15 @@
         ),
     )
 
 
 class ExternalFileFormatRcClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *Record Columnar file format (RcFile)* clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=rc#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=rc#syntax
     """
 
     type = "external_file_rc_clause"
 
     match_grammar = Delimited(
         Sequence(
             "FORMAT_TYPE",
@@ -5737,15 +5769,15 @@
         ),
     )
 
 
 class ExternalFileFormatOrcClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *Optimized Row Columnar (ORC)* format clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=orc#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=orc#syntax
     """
 
     type = "external_file_orc_clause"
 
     match_grammar = Delimited(
         Sequence(
             "FORMAT_TYPE",
@@ -5760,15 +5792,15 @@
         ),
     )
 
 
 class ExternalFileFormatParquetClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *PARQUET* format clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=parquet#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=parquet#syntax
     """
 
     type = "external_file_parquet_clause"
 
     match_grammar = Delimited(
         Sequence(
             "FORMAT_TYPE",
@@ -5783,15 +5815,15 @@
         ),
     )
 
 
 class ExternalFileFormatJsonClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *JSON* format clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=json#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=json#syntax
     """
 
     type = "external_file_json_clause"
 
     match_grammar = Delimited(
         Sequence(
             "FORMAT_TYPE",
@@ -5806,30 +5838,30 @@
         ),
     )
 
 
 class ExternalFileFormatDeltaClause(BaseSegment):
     """`CREATE EXTERNAL FILE FORMAT` *Delta Lake* format clause.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=delta#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=delta#syntax
     """
 
     type = "external_file_delta_clause"
 
     match_grammar = Sequence(
         "FORMAT_TYPE",
         Ref("EqualsSegment"),
         "DELTA",
     )
 
 
 class CreateExternalFileFormat(BaseSegment):
     """A statement to create an `EXTERNAL FILE FORMAT` object.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql?view=sql-server-ver16&tabs=delta#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-file-format-transact-sql&tabs=delta#syntax
     """
 
     type = "create_external_file_format"
 
     match_grammar: Matchable = Sequence(
         "CREATE",
         "EXTERNAL",
@@ -5849,15 +5881,15 @@
         ),
     )
 
 
 class OpenJsonWithClauseSegment(BaseSegment):
     """A `WITH` clause of an `OPENJSON()` table-valued function.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/functions/openjson-transact-sql?view=sql-server-ver16#with_clause
+    https://learn.microsoft.com/en-us/sql/t-sql/functions/openjson-transact-sql#with_clause
     """
 
     type = "openjson_with_clause"
 
     match_grammar = Sequence(
         "WITH",
         Bracketed(
@@ -5876,15 +5908,15 @@
         ),
     )
 
 
 class OpenJsonSegment(BaseSegment):
     """An `OPENJSON()` table-valued function.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/functions/openjson-transact-sql?view=sql-server-ver16#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/functions/openjson-transact-sql#syntax
     """
 
     type = "openjson_segment"
 
     match_grammar = Sequence(
         "OPENJSON",
         Bracketed(
@@ -5898,15 +5930,15 @@
         Ref("OpenJsonWithClauseSegment", optional=True),
     )
 
 
 class CreateExternalTableStatementSegment(BaseSegment):
     """A `CREATE EXTERNAL TABLE` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-table-transact-sql?view=sql-server-ver16&tabs=dedicated
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-external-table-transact-sql&tabs=dedicated
     """
 
     type = "create_external_table_statement"
 
     match_grammar = Sequence(
         "CREATE",
         "EXTERNAL",
@@ -5955,15 +5987,15 @@
         ),
     )
 
 
 class CreateRoleStatementSegment(ansi.CreateRoleStatementSegment):
     """A `CREATE ROLE` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-role-transact-sql?view=sql-server-ver16
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-role-transact-sql
     """
 
     type = "create_role_statement"
 
     match_grammar = Sequence(
         "CREATE",
         "ROLE",
@@ -5990,29 +6022,29 @@
         Ref("TableReferenceSegment"),
     )
 
 
 class StorageLocationSegment(BaseSegment):
     """A tsql external storage location.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql?view=azure-sqldw-latest#external-locations
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql#external-locations
     """
 
     type = "storage_location"
 
     match_grammar = OneOf(
         Ref("AzureBlobStoragePath"),
         Ref("AzureDataLakeStorageGen2Path"),
     )
 
 
 class CopyIntoTableStatementSegment(BaseSegment):
     """A tsql `COPY INTO <table>` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql?view=azure-sqldw-latest
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/copy-into-transact-sql
     """
 
     type = "copy_into_table_statement"
 
     match_grammar = Sequence(
         "COPY",
         "INTO",
@@ -6106,21 +6138,224 @@
         ),
     )
 
 
 class CreateUserStatementSegment(ansi.CreateUserStatementSegment):
     """`CREATE USER` statement.
 
-    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-user-transact-sql?view=sql-server-ver16#syntax
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-user-transact-sql#syntax
     """
 
     match_grammar = Sequence(
         "CREATE",
         "USER",
         Ref("RoleReferenceSegment"),
         Sequence(
             OneOf("FROM", "FOR"),
             "LOGIN",
             Ref("ObjectReferenceSegment"),
             optional=True,
         ),
     )
+
+
+class ComputedColumnDefinitionSegment(BaseSegment):
+    """A computed column definition, e.g. for CREATE TABLE or ALTER TABLE.
+
+    https://learn.microsoft.com/en-us/sql/relational-databases/tables/specify-computed-columns-in-a-table
+    """
+
+    type = "computed_column_definition"
+
+    match_grammar: Matchable = Sequence(
+        Ref("SingleIdentifierGrammar"),  # Column name
+        "AS",
+        OptionallyBracketed(
+            OneOf(
+                Ref("FunctionSegment"),
+                Ref("BareFunctionSegment"),
+                Ref("ExpressionSegment"),
+            ),
+        ),
+        Sequence(
+            "PERSISTED",
+            Sequence("NOT", "NULL", optional=True),
+            optional=True,
+        ),
+        AnyNumberOf(
+            Ref("ColumnConstraintSegment", optional=True),
+        ),
+    )
+
+
+class CreatePartitionFunctionSegment(BaseSegment):
+    """A `CREATE PARTITION FUNCTION` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/create-partition-function-transact-sql
+
+    type = "create_partition_function_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "PARTITION",
+        "FUNCTION",
+        Ref("ObjectReferenceSegment"),
+        Bracketed(
+            Ref("DatatypeSegment"),
+        ),
+        "AS",
+        "RANGE",
+        OneOf(
+            "LEFT",
+            "RIGHT",
+        ),
+        "FOR",
+        "VALUES",
+        Bracketed(Delimited(Ref("LiteralGrammar"))),
+        # Bracketed(Delimited("LEFT")),
+    )
+
+
+class AlterPartitionFunctionSegment(BaseSegment):
+    """A `ALTER PARTITION FUNCTION` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-partition-function-transact-sql
+    # https://learn.microsoft.com/en-us/sql/relational-databases/partitions/modify-a-partition-function
+
+    type = "alter_partition_function_statement"
+
+    match_grammar: Matchable = Sequence(
+        "ALTER",
+        "PARTITION",
+        "FUNCTION",
+        Ref("ObjectReferenceSegment"),
+        Bracketed(),
+        OneOf(
+            Sequence("SPLIT", "RANGE", Bracketed(Ref("LiteralGrammar"))),
+            Sequence("MERGE", "RANGE", Bracketed(Ref("LiteralGrammar"))),
+        ),
+    )
+
+
+class CreatePartitionSchemeSegment(BaseSegment):
+    """A `CREATE PARTITION SCHEME` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/create-partition-scheme-transact-sql
+
+    type = "create_partition_scheme_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "PARTITION",
+        "SCHEME",
+        Ref("ObjectReferenceSegment"),
+        "AS",
+        "PARTITION",
+        Ref("ObjectReferenceSegment"),
+        Ref.keyword("ALL", optional=True),
+        "TO",
+        Bracketed(
+            Delimited(
+                OneOf(Ref("ObjectReferenceSegment"), "PRIMARY"),
+            ),
+        ),
+    )
+
+
+class AlterPartitionSchemeSegment(BaseSegment):
+    """A `ALTER PARTITION SCHEME` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-partition-scheme-transact-sql
+    # https://learn.microsoft.com/en-us/sql/relational-databases/partitions/modify-a-partition-scheme
+
+    type = "alter_partition_scheme_statement"
+
+    match_grammar: Matchable = Sequence(
+        "ALTER",
+        "PARTITION",
+        "SCHEME",
+        Ref("ObjectReferenceSegment"),
+        "NEXT",
+        "USED",
+        Ref("ObjectReferenceSegment", optional=True),
+    )
+
+
+class CreateMasterKeySegment(BaseSegment):
+    """A `CREATE MASTER KEY` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/create-master-key-transact-sql
+
+    type = "create_master_key_statement"
+
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "MASTER",
+        "KEY",
+        Sequence(
+            "ENCRYPTION",
+            "BY",
+            "PASSWORD",
+            Ref("EqualsSegment"),
+            Ref("QuotedLiteralSegment"),
+            optional=True,
+        ),
+    )
+
+
+class MasterKeyEncryptionSegment(BaseSegment):
+    """Master key encryptopn option."""
+
+    type = "master_key_encryption_option"
+
+    match_grammar: Matchable = OneOf(
+        Sequence("SERVICE", "MASTER", "KEY"),
+        Sequence(
+            "PASSWORD",
+            Ref("EqualsSegment"),
+            Ref("QuotedLiteralSegment"),
+        ),
+    )
+
+
+class AlterMasterKeySegment(BaseSegment):
+    """A `ALTER MASTER KEY` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-master-key-transact-sql
+
+    type = "alter_master_key_statement"
+
+    match_grammar: Matchable = Sequence(
+        "ALTER",
+        "MASTER",
+        "KEY",
+        OneOf(
+            Sequence(
+                Ref.keyword("FORCE", optional=True),
+                "REGENERATE",
+                "WITH",
+                "ENCRYPTION",
+                "BY",
+                Ref("MasterKeyEncryptionSegment"),
+            ),
+            Sequence(
+                OneOf("ADD", "DROP"),
+                "ENCRYPTION",
+                "BY",
+                Ref("MasterKeyEncryptionSegment"),
+            ),
+        ),
+    )
+
+
+class DropMasterKeySegment(BaseSegment):
+    """A `DROP MASTER KEY` statement."""
+
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/drop-master-key-transact-sql
+
+    type = "drop_master_key_statement"
+
+    match_grammar: Matchable = Sequence(
+        "DROP",
+        "MASTER",
+        "KEY",
+    )
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,42 +42,42 @@
     "BETWEEN",
     "BREAK",
     "BROWSE",
     "BULK",
     "BY",
     "CASCADE",
     "CASE",
+    "CHECK_CONSTRAINTS",
     "CHECK",
     "CHECKPOINT",
-    "CHECK_CONSTRAINTS",
     "CLOSE",
     "CLUSTERED",
     "COALESCE",
     "COLLATE",
     "COLUMN",
     "COMMIT",
     "COMPUTE",
     "CONSTRAINT",
     "CONTAINS",
     "CONTAINSTABLE",
     "CONTINUE",
     "CONVERT",
     "CREATE",
     "CROSS",
-    "CURRENT",
     "CURRENT_CATALOG",  # *future*
     "CURRENT_DATE",
     "CURRENT_DEFAULT_TRANSFORM_GROUP",  # *future*
     "CURRENT_PATH",  # *future*
     "CURRENT_ROLE",  # *future*
     "CURRENT_SCHEMA",  # *future*
     "CURRENT_TIME",
     "CURRENT_TIMESTAMP",
     "CURRENT_TRANSFORM_GROUP_FOR_TYPE",  # *future*
     "CURRENT_USER",
+    "CURRENT",
     "CURSOR",
     "DATABASE",
     "DBCC",
     "DEALLOCATE",
     "DECLARE",
     "DEFAULT",
     "DELETE",
@@ -99,16 +99,16 @@
     "EXIT",
     "EXTERNAL",
     "FAST_FORWARD",
     "FETCH",
     "FILE",
     "FILLFACTOR",
     "FOR",
-    "FORWARD_ONLY",
     "FOREIGN",
+    "FORWARD_ONLY",
     "FREETEXT",
     "FREETEXTTABLE",
     "FROM",
     "FULL",
     "FULLSCAN",
     "FUNCTION",
     "GLOBAL",
@@ -167,16 +167,16 @@
     "PLAN",
     "PRIMARY",
     "PRINT",
     "PROC",
     "PROCEDURE",
     "PUBLIC",
     "RAISERROR",
-    "READ",
     "READ_ONLY",
+    "READ",
     "READTEXT",
     "RECONFIGURE",
     "REFERENCES",
     "REPLICATION",
     "RESAMPLE",
     "RESTORE",
     "RESTRICT",
@@ -186,16 +186,16 @@
     "RIGHT",
     "ROLLBACK",
     "ROWCOUNT",
     "ROWGUIDCOL",
     "RULE",
     "SAVE",
     "SCHEMA",
-    "SCROLL",
     "SCROLL_LOCKS",
+    "SCROLL",
     "SELECT",
     "SEMANTICKEYPHRASETABLE",
     "SEMANTICSIMILARITYDETAILSTABLE",
     "SEMANTICSIMILARITYTABLE",
     "SESSION_USER",
     "SET",
     "SETUSER",
@@ -207,16 +207,16 @@
     "TABLE",
     "TABLESAMPLE",
     "TEXTSIZE",
     "THEN",
     "TO",
     "TOP",
     "TRAN",
-    "TRANSACTION",
     "TRAN",
+    "TRANSACTION",
     "TRIGGER",
     "TRUNCATE",
     "TRY_CONVERT",
     "TSEQUAL",
     "TYPE_WARNING",
     "UNION",
     "UNIQUE",
@@ -244,36 +244,36 @@
     "DESTROY",
     "END-EXEC",
     "EVERY",
     "LIKE_REGEX",
 ]
 
 UNRESERVED_KEYWORDS = [
-    "ABORT",
     "ABORT_AFTER_WAIT",
+    "ABORT",
     "ABSENT",
     "ACTION",
-    "ATOMIC",
     "AFTER",
     "ALGORITHM",
-    "ALLOWED",
     "ALLOW_PAGE_LOCKS",
     "ALLOW_ROW_LOCKS",
+    "ALLOWED",
     "ALWAYS",
     "ANSI_DEFAULTS",
     "ANSI_NULL_DFLT_OFF",
     "ANSI_NULL_DFLT_ON",
     "ANSI_NULLS",
     "ANSI_PADDING",
     "ANSI_WARNINGS",
     "APPEND_ONLY",
     "APPLY",
     "ARITHABORT",
     "ARITHIGNORE",
     "AT",
+    "ATOMIC",
     "AUTO_CREATE_TABLE",
     "AUTO",
     "BEFORE",  # *future*
     "BERNOULLI",
     "BINARY",
     "BLOCKERS",
     "BREAK",
@@ -293,16 +293,16 @@
     "COMPRESSION",
     "CONCAT_NULL_YIELDS_NULL",
     "CONCAT",
     "CONNECTION_OPTIONS",
     "CONTAINED",
     "CONTINUE",
     "CONTROL",
-    "CREDENTIAL",
     "COPY",
+    "CREDENTIAL",
     "CURSOR_CLOSE_ON_COMMIT",
     "CYCLE",
     "DATA_COMPRESSION",
     "DATA_CONSISTENCY_CHECK",
     "DATA_DELETION",
     "DATA_SOURCE",
     "DATA",
@@ -341,19 +341,19 @@
     "EXPLICIT",
     "EXTERNALPUSHDOWN",
     "FAST",
     "FIELD_TERMINATOR",
     "FIELDQUOTE",
     "FIELDTERMINATOR",
     "FILE_FORMAT",
+    "FILE_TYPE",
     "FILEGROUP",
-    "FILESTREAM",
     "FILESTREAM_ON",
     "FILESTREAM",
-    "FILE_TYPE",
+    "FILESTREAM",
     "FILETABLE_COLLATE_FILENAME",
     "FILETABLE_DIRECTORY",
     "FILETABLE_FULLPATH_UNIQUE_CONSTRAINT_NAME",
     "FILETABLE_PRIMARY_KEY_CONSTRAINT_NAME",
     "FILETABLE_STREAMID_UNIQUE_CONSTRAINT_NAME",
     "FILTER_COLUMN",
     "FILTER_PREDICATE",
@@ -407,28 +407,29 @@
     "KEEPIDENTITY",
     "KEEPNULLS",
     "KILOBYTES_PER_BATCH",
     "LABEL",  # *reserved* keyword in Azure Synapse; but would break TSQL parsing
     "LANGUAGE",
     "LAST",
     "LASTROW",
-    "LEDGER",
     "LEDGER_VIEW",
+    "LEDGER",
     "LEGACY_CARDINALITY_ESTIMATION",
     "LEVEL",
     "LOAD",  # listed as reserved but functionally unreserved
     "LOB_COMPACTION",
     "LOCATION",
     "LOCK_TIMEOUT",
     "LOG",
     "LOGIN",
     "LOOP",
     "LOW",
     "MANUAL",
     "MASKED",
+    "MASTER",
     "MATCHED",
     "MAX_DURATION",
     "MAX_GRANT_PERCENT",
     "MAX",
     "MAXDOP",
     "MAXERRORS",
     "MAXRECURSION",
@@ -467,22 +468,23 @@
     "OUTPUT",
     "OVERRIDE",
     "OWNER",
     "PAD_INDEX",
     "PAGE",
     "PAGLOCK",
     "PARAMETER",
-    "PARAMETERS",  # *future*
     "PARAMETERIZATION",
+    "PARAMETERS",  # *future*
     "PARQUET",
     "PARSEONLY",
     "PARSER_VERSION",
     "PARTIAL",  # *future*
     "PARTITION",
     "PARTITIONS",
+    "PASSWORD",
     "PATH",
     "PAUSE",
     "PAUSED",
     "PERCENTAGE",
     "PERCENTILE_CONT",
     "PERCENTILE_DISC",
     "PERIOD",
@@ -508,27 +510,28 @@
     "READONLY",
     "READPAST",
     "READUNCOMMITTED",
     "REBUILD",
     "RECEIVE",
     "RECOMPILE",
     "RECURSIVE",
+    "REGENERATE",
     "REGR_AVGX",  # *future*
     "REGR_AVGY",  # *future*
     "REGR_COUNT",  # *future*
     "REGR_INTERCEPT",  # *future*
     "REGR_R2",  # *future*
     "REGR_SLOPE",  # *future*
     "REGR_SXX",  # *future*
     "REGR_SXY",  # *future*
     "REGR_SYY",  # *future*
-    "REJECTED_ROW_LOCATION",
     "REJECT_SAMPLE_VALUE",
     "REJECT_TYPE",
     "REJECT_VALUE",
+    "REJECTED_ROW_LOCATION",
     "REMOTE_DATA_ARCHIVE",
     "REMOTE_PROC_TRANSACTIONS",
     "RENAME",  # Azure Synapse Analytics specific
     "REORGANIZE",
     "REPEATABLE",
     "REPEATABLEREAD",
     "REPLACE",
@@ -551,38 +554,41 @@
     "ROWS",
     "ROWTERMINATOR",
     "S",
     "SCALEOUTEXECUTION",
     "SCHEMA_AND_DATA",
     "SCHEMA_ONLY",
     "SCHEMABINDING",
+    "SCHEME",
     "SCOPED",
     "SEARCH",
     "SECRET",
     "SECURITYAUDIT",  # listed as reserved but functionally unreserved
     "SELF",
     "SEQUENCE_NUMBER_COLUMN_NAME",
     "SEQUENCE_NUMBER",
     "SEQUENCE",
     "SERDE_METHOD",
     "SERIALIZABLE",
     "SERVER",
+    "SERVICE",
     "SETERROR",
     "SETVAR",  # sqlcmd command
     "SHOWPLAN_ALL",
     "SHOWPLAN_TEXT",
     "SHOWPLAN_XML",
     "SINGLE_BLOB",
     "SINGLE_CLOB",
     "SINGLE_NCLOB",
     "SNAPSHOT",
     "SORT_IN_TEMPDB",
     "SOURCE",
     "SPARSE",
     "SPATIAL_WINDOW_MAX_CELLS",
+    "SPLIT",
     "START",
     "STATISTICAL_SEMANTICS",
     "STATISTICS_INCREMENTAL",
     "STATISTICS_NORECOMPUTE",
     "STOPLIST",
     "STRING_AGG",
     "STRING_DELIMITER",
@@ -607,28 +613,30 @@
     "TRY",
     "TYPE",
     "UNBOUNDED",
     "UNCOMMITTED",
     "UNKNOWN",
     "UPDLOCK",
     "USE_TYPE_DEFAULT",
+    "USED",
     "USER_DB",  # Azure Synapse Analytics specific, deprecated
     "USING",
     "VALUE",
     "VIEW_METADATA",
     "WAIT_AT_LOW_PRIORITY",
     "WAITFOR",
     "WEEK",
     "WEEKS",
     "WHILE",
     "WITHIN",
     "WITHOUT_ARRAY_WRAPPER",
     "WORK",
     "XACT_ABORT",
     "XLOCK",
+    "XML_COMPRESSION",
     "XML",
     "XMLAGG",  # *future*
     "XMLATTRIBUTES",  # *future*
     "XMLBINARY",  # *future*
     "XMLCAST",  # *future*
     "XMLCOMMENT",  # *future*
     "XMLCONCAT",  # *future*
@@ -643,13 +651,12 @@
     "XMLPI",  # *future*
     "XMLQUERY",  # *future*
     "XMLSCHEMA",
     "XMLSERIALIZE",  # *future*
     "XMLTABLE",  # *future*
     "XMLTEXT",  # *future*
     "XMLVALIDATE",  # *future*
-    "XML_COMPRESSION",
     "XSINIL",
     "YEAR",
     "YEARS",
     "ZONE",
 ]
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica_keywords.py` & `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-3.0.6/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL08.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL09.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST02.py`

 * *Files 7% similar despite different names*

```diff
@@ -190,33 +190,48 @@
 
                 # Locate column reference in condition expression.
                 column_reference_segment = (
                     Segments(condition_expression)
                     .children(sp.is_type("column_reference"))
                     .get()
                 )
+                array_accessor_segment = (
+                    Segments(condition_expression)
+                    .children(sp.is_type("array_accessor"))
+                    .get()
+                )
 
                 # Return None if none found (this condition does not apply to functions)
                 if not column_reference_segment:
                     return None
 
+                if array_accessor_segment:
+                    column_reference_segment_raw_upper = (
+                        column_reference_segment.raw_upper
+                        + array_accessor_segment.raw_upper
+                    )
+                else:
+                    column_reference_segment_raw_upper = (
+                        column_reference_segment.raw_upper
+                    )
+
                 if else_clauses:
                     else_expression = else_clauses.children(sp.is_type("expression"))[0]
                     # Check if we can reduce the CASE expression to a single coalesce
                     # function.
                     if (
                         not is_not_prefix
-                        and column_reference_segment.raw_upper
+                        and column_reference_segment_raw_upper
                         == else_expression.raw_upper
                     ):
                         coalesce_arg_1 = else_expression
                         coalesce_arg_2 = then_expression
                     elif (
                         is_not_prefix
-                        and column_reference_segment.raw_upper
+                        and column_reference_segment_raw_upper
                         == then_expression.raw_upper
                     ):
                         coalesce_arg_1 = then_expression
                         coalesce_arg_2 = else_expression
                     else:
                         return None
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST09.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/rules/tsql/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/rules/tsql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/analysis/query.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/analysis/query.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/context.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/identifers.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/respace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Static methods to support ReflowPoint.respace_point()."""
 
 import logging
+from collections import defaultdict
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, cast
 
 from sqlfluff.core.errors import SQLFluffUserError
 from sqlfluff.core.parser import (
     BaseSegment,
     PositionMarker,
     RawSegment,
@@ -231,32 +232,46 @@
             )
 
     # If the segment we're aligning, has position. Use that position.
     # If it doesn't, then use the provided one. We can't do sibling analysis without it.
     if next_seg.pos_marker:
         next_pos = next_seg.pos_marker
 
-    # Purge any siblings which are either self, or on the same line but after it.
-    _earliest_siblings: Dict[int, int] = {}
-    for sibling in siblings[:]:
+    # Purge any siblings which are either on the same line or on another line and
+    # have another index
+    siblings_by_line: Dict[int, List[BaseSegment]] = defaultdict(list)
+    for sibling in siblings:
         _pos = sibling.pos_marker
         assert _pos
-        _best_seen = _earliest_siblings.get(_pos.working_line_no, None)
-        # If we've already seen an earlier sibling on this line, ignore the later one.
-        if _best_seen is not None and _pos.working_line_pos > _best_seen:
-            siblings.remove(sibling)
-            continue
-        # Update best seen
-        _earliest_siblings[_pos.working_line_no] = _pos.working_line_pos
-
-        # We should also purge the sibling which matches the target.
-        if _pos.working_line_no == next_pos.working_line_no:
-            # Is it in the same position?
-            if _pos.working_line_pos != next_pos.working_line_pos:
-                siblings.remove(sibling)
+        siblings_by_line[_pos.working_line_no].append(sibling)
+
+    # Sort all segments by position to easily access index information
+    for line_siblings in siblings_by_line.values():
+        line_siblings.sort(
+            key=lambda s: cast(PositionMarker, s.pos_marker).working_line_pos
+        )
+
+    target_index = next(
+        idx
+        for idx, segment in enumerate(siblings_by_line[next_pos.working_line_no])
+        if (
+            cast(PositionMarker, segment.pos_marker).working_line_pos
+            == next_pos.working_line_pos
+        )
+    )
+
+    # Now that we know the target index, we can extract the relevant segment from
+    # all lines
+    siblings = [
+        segment
+        for segments in siblings_by_line.values()
+        for segment in (
+            [segments[target_index]] if target_index < len(segments) else []
+        )
+    ]
 
     # If there's only one sibling, we have nothing to compare to. Default to a single
     # space.
     if len(siblings) <= 1:
         desired_space = " "
         reflow_logger.debug(
             "    desired_space: %r (based on no other siblings)",
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-3.0.6/src/sqlfluff/utils/testing/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,21 +113,21 @@
         overrides["dialect"] = "ansi"
     cfg = FluffConfig(configs=configs, overrides=overrides)
     linter = Linter(config=cfg)
 
     # This section is mainly for aid in debugging.
     rendered = linter.render_string(sql, fname="<STR>", config=cfg, encoding="utf-8")
     parsed = linter.parse_rendered(rendered)
-    if parsed.violations:
+    tree = parsed.tree  # Delegate assertions to the `.tree` property
+    violations = parsed.violations
+    if violations:
         if msg:
             print(msg)  # pragma: no cover
-        assert parsed.tree
-        pytest.fail(parsed.violations[0].desc() + "\n" + parsed.tree.stringify())
-    assert parsed.tree
-    print(f"Parsed:\n {parsed.tree.stringify()}")
+        pytest.fail(violations[0].desc() + "\n" + tree.stringify())
+    print(f"Parsed:\n {tree.stringify()}")
 
     # Note that lint_string() runs the templater and parser again, in order to
     # test the whole linting pipeline in the same way that users do. In other
     # words, the "rendered" and "parsed" variables above are irrelevant to this
     # line of code.
     lint_result = linter.lint_string(sql, config=cfg, fname="<STR>")
     lerrs = lint_result.violations
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-3.0.6/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.5
+Version: 3.0.6
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff-3.0.5/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-3.0.6/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-3.0.6/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.5/test/testing_test.py` & `sqlfluff-3.0.6/test/testing_test.py`

 * *Files identical despite different names*

