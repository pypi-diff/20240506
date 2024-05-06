# Comparing `tmp/serpyco_rs-1.7.1.tar.gz` & `tmp/serpyco_rs-1.8.0.tar.gz`

## Comparing `serpyco_rs-1.7.1.tar` & `serpyco_rs-1.8.0.tar`

### file list

```diff
@@ -1,90 +1,92 @@
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 serpyco_rs-1.7.1/Cargo.toml
--rw-r--r--   0      501       20       25 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/.envrc.example
--rw-r--r--   0      501       20      196 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/.github/dependabot.yml
--rw-r--r--   0      501       20     9018 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/.gitignore
--rw-r--r--   0      501       20     1069 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/LICENSE
--rw-r--r--   0      501       20       34 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/MANIFEST.in
--rw-r--r--   0      501       20    12768 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/README.md
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/__init__.py
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/__init__.py
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/github_issue/__init__.py
--rw-r--r--   0      501       20      217 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/github_issue/_utils.py
--rw-r--r--   0      501       20     8489 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/github_issue/data.json
--rw-r--r--   0      501       20     3637 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/github_issue/mashumaro.py
--rw-r--r--   0      501       20     3272 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/github_issue/serpyco_rs.py
--rw-r--r--   0      501       20     1828 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/graph.py
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/__init__.py
--rw-r--r--   0      501       20      637 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/base.py
--rw-r--r--   0      501       20      334 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/marshmallow.py
--rw-r--r--   0      501       20      800 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/mashumaro.py
--rw-r--r--   0      501       20      504 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/pydantic.py
--rw-r--r--   0      501       20      329 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/serpyco.py
--rw-r--r--   0      501       20      320 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/libs/serpyco_rs.py
--rw-r--r--   0      501       20     1489 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/test_benchmarks.py
--rw-r--r--   0      501       20     1359 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/compare/test_github_issue.py
--rw-r--r--   0      501       20     1573 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/conftest.py
--rw-r--r--   0      501       20     8034 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/test_encoders.py
--rw-r--r--   0      501       20      907 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/test_full.py
--rw-r--r--   0      501       20      198 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/bench/utils.py
--rw-r--r--   0      501       20      111 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/build.rs
--rw-r--r--   0      501       20   379576 2024-04-23 17:03:15.000000 serpyco_rs-1.7.1/merged.profdata
--rw-r--r--   0      501       20     3039 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/noxfile.py
--rw-r--r--   0      501       20  1322229 2024-04-23 17:01:19.000000 serpyco_rs-1.7.1/pgo-wheel/serpyco_rs-1.7.1-cp312-cp312-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl
--rw-r--r--   0      501       20    69994 2024-04-23 16:59:35.000000 serpyco_rs-1.7.1/pgo-wheel/serpyco_rs-1.7.1.tar.gz
--rw-r--r--   0      501       20      253 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/__init__.py
--rw-r--r--   0      501       20    17681 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_describe.py
--rw-r--r--   0      501       20      969 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_impl.py
--rw-r--r--   0      501       20     6351 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_impl.pyi
--rw-r--r--   0      501       20      162 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/__init__.py
--rw-r--r--   0      501       20      108 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/_consts.py
--rw-r--r--   0      501       20     8195 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/_convert.py
--rw-r--r--   0      501       20     5414 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/_entities.py
--rw-r--r--   0      501       20     2953 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_main.py
--rw-r--r--   0      501       20      842 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_meta.py
--rw-r--r--   0      501       20    17854 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_type_utils.py
--rw-r--r--   0      501       20      323 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/_utils.py
--rw-r--r--   0      501       20      139 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/exceptions.py
--rw-r--r--   0      501       20     1450 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/metadata.py
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/python/serpyco_rs/py.typed
--rw-r--r--   0      501       20      141 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/requirements/bench.txt
--rw-r--r--   0      501       20      156 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/requirements/dev.txt
--rw-r--r--   0      501       20       17 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/requirements/lint.txt
--rw-r--r--   0      501       20       47 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/requirements/type_check.txt
--rw-r--r--   0      501       20     2461 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/ruff.toml
--rw-r--r--   0      501       20     3411 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/errors.rs
--rw-r--r--   0      501       20     1640 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/lib.rs
--rw-r--r--   0      501       20     4334 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/python/dateutil.rs
--rw-r--r--   0      501       20      545 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/python/macros.rs
--rw-r--r--   0      501       20      248 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/python/mod.rs
--rw-r--r--   0      501       20     2350 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/python/py.rs
--rw-r--r--   0      501       20     3584 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/python/types.rs
--rw-r--r--   0      501       20    32611 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/serializer/encoders.rs
--rw-r--r--   0      501       20    15502 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/serializer/main.rs
--rw-r--r--   0      501       20       51 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/serializer.rs
--rw-r--r--   0      501       20     2170 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/validator/context.rs
--rw-r--r--   0      501       20     1255 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/validator/errors.rs
--rw-r--r--   0      501       20      132 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/validator/mod.rs
--rw-r--r--   0      501       20    31929 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/validator/types.rs
--rw-r--r--   0      501       20     6118 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/src/validator/validators.rs
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/__init__.py
--rw-r--r--   0      501       20       88 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/conftest.py
--rw-r--r--   0      501       20        0 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/json_schema/__init__.py
--rw-r--r--   0      501       20    18524 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/json_schema/test_convert.py
--rw-r--r--   0      501       20     8313 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/json_schema/test_validator.py
--rw-r--r--   0      501       20    24101 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test__describe.py
--rw-r--r--   0      501       20      875 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_custom_encoder.py
--rw-r--r--   0      501       20     7462 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_encoders.py
--rw-r--r--   0      501       20     6412 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_generics.py
--rw-r--r--   0      501       20     1481 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_leak.py
--rw-r--r--   0      501       20     6777 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_load_query_params.py
--rw-r--r--   0      501       20     2520 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_metadata.py
--rw-r--r--   0      501       20     2624 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_recursive.py
--rw-r--r--   0      501       20     7934 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_simple.py
--rw-r--r--   0      501       20     4230 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_type_utils.py
--rw-r--r--   0      501       20     2638 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_type_utils_py311.py
--rw-r--r--   0      501       20     5487 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_union.py
--rw-r--r--   0      501       20    10438 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/tests/test_validation.py
--rw-r--r--   0      501       20     9479 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/Cargo.lock
--rw-r--r--   0      501       20     1009 2024-04-23 16:58:58.000000 serpyco_rs-1.7.1/pyproject.toml
--rw-r--r--   0        0        0    13757 1970-01-01 00:00:00.000000 serpyco_rs-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 serpyco_rs-1.8.0/Cargo.toml
+-rw-r--r--   0        0        0       26 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/.envrc.example
+-rw-r--r--   0        0        0      206 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     9323 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1090 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/LICENSE
+-rw-r--r--   0        0        0       34 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/MANIFEST.in
+-rw-r--r--   0        0        0    16519 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/github_issue/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/github_issue/_utils.py
+-rw-r--r--   0        0        0     8662 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/github_issue/data.json
+-rw-r--r--   0        0        0     3796 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/github_issue/mashumaro.py
+-rw-r--r--   0        0        0     3425 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/github_issue/serpyco_rs.py
+-rw-r--r--   0        0        0     1893 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/graph.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/base.py
+-rw-r--r--   0        0        0      352 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/marshmallow.py
+-rw-r--r--   0        0        0      843 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/mashumaro.py
+-rw-r--r--   0        0        0      534 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/pydantic.py
+-rw-r--r--   0        0        0      347 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/serpyco.py
+-rw-r--r--   0        0        0      338 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/libs/serpyco_rs.py
+-rw-r--r--   0        0        0     1531 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/test_benchmarks.py
+-rw-r--r--   0        0        0     1400 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/compare/test_github_issue.py
+-rw-r--r--   0        0        0     1633 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/conftest.py
+-rw-r--r--   0        0        0     8305 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/test_encoders.py
+-rw-r--r--   0        0        0      933 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/test_full.py
+-rw-r--r--   0        0        0      207 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/bench/utils.py
+-rw-r--r--   0        0        0      115 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/build.rs
+-rw-r--r--   0        0        0  5714760 2024-05-06 10:52:30.000000 serpyco_rs-1.8.0/merged.profdata
+-rw-r--r--   0        0        0     3143 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/noxfile.py
+-rw-r--r--   0        0        0   686588 2024-05-06 10:50:39.000000 serpyco_rs-1.8.0/pgo-wheel/serpyco_rs-1.8.0-cp310-none-win_amd64.whl
+-rw-r--r--   0        0        0    73672 2024-05-06 10:49:56.000000 serpyco_rs-1.8.0/pgo-wheel/serpyco_rs-1.8.0.tar.gz
+-rw-r--r--   0        0        0      312 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_custom_types.py
+-rw-r--r--   0        0        0    19383 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_describe.py
+-rw-r--r--   0        0        0     1036 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_impl.py
+-rw-r--r--   0        0        0     6746 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_impl.pyi
+-rw-r--r--   0        0        0      164 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/_consts.py
+-rw-r--r--   0        0        0     8651 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/_convert.py
+-rw-r--r--   0        0        0     5599 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/_entities.py
+-rw-r--r--   0        0        0     3562 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_main.py
+-rw-r--r--   0        0        0      871 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_meta.py
+-rw-r--r--   0        0        0    18354 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_type_utils.py
+-rw-r--r--   0        0        0      337 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/_utils.py
+-rw-r--r--   0        0        0      143 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/exceptions.py
+-rw-r--r--   0        0        0     1530 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/metadata.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/python/serpyco_rs/py.typed
+-rw-r--r--   0        0        0      152 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/requirements/bench.txt
+-rw-r--r--   0        0        0      102 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/requirements/dev.txt
+-rw-r--r--   0        0        0       20 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/requirements/lint.txt
+-rw-r--r--   0        0        0       52 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/requirements/type_check.txt
+-rw-r--r--   0        0        0     2550 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/ruff.toml
+-rw-r--r--   0        0        0     3536 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/errors.rs
+-rw-r--r--   0        0        0     1734 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/lib.rs
+-rw-r--r--   0        0        0     4487 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/python/dateutil.rs
+-rw-r--r--   0        0        0      568 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/python/macros.rs
+-rw-r--r--   0        0        0      258 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/python/mod.rs
+-rw-r--r--   0        0        0     2420 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/python/py.rs
+-rw-r--r--   0        0        0     3783 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/python/types.rs
+-rw-r--r--   0        0        0    34526 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/serializer/encoders.rs
+-rw-r--r--   0        0        0    16936 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/serializer/main.rs
+-rw-r--r--   0        0        0       55 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/serializer.rs
+-rw-r--r--   0        0        0     2262 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/validator/context.rs
+-rw-r--r--   0        0        0     1754 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/validator/errors.rs
+-rw-r--r--   0        0        0      180 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/validator/mod.rs
+-rw-r--r--   0        0        0    33841 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/validator/types.rs
+-rw-r--r--   0        0        0     6346 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/src/validator/validators.rs
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/json_schema/__init__.py
+-rw-r--r--   0        0        0    19002 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/json_schema/test_convert.py
+-rw-r--r--   0        0        0     8604 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/json_schema/test_validator.py
+-rw-r--r--   0        0        0    24906 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test__describe.py
+-rw-r--r--   0        0        0     1307 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_custom_encoder.py
+-rw-r--r--   0        0        0     2311 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_custom_types.py
+-rw-r--r--   0        0        0     7727 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_encoders.py
+-rw-r--r--   0        0        0     6607 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_generics.py
+-rw-r--r--   0        0        0     1551 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_leak.py
+-rw-r--r--   0        0        0     7006 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_load_query_params.py
+-rw-r--r--   0        0        0     2621 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     2720 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_recursive.py
+-rw-r--r--   0        0        0     8244 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_simple.py
+-rw-r--r--   0        0        0     4428 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_type_utils.py
+-rw-r--r--   0        0        0     2722 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_type_utils_py311.py
+-rw-r--r--   0        0        0     5713 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_union.py
+-rw-r--r--   0        0        0    10794 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/tests/test_validation.py
+-rw-r--r--   0        0        0     9830 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/Cargo.lock
+-rw-r--r--   0        0        0     1046 2024-05-06 10:48:58.000000 serpyco_rs-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    17508 1970-01-01 00:00:00.000000 serpyco_rs-1.8.0/PKG-INFO
```

### Comparing `serpyco_rs-1.7.1/Cargo.toml` & `serpyco_rs-1.8.0/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "serpyco-rs"
-version = "1.7.1"
+version = "1.8.0"
 edition = "2021"
 homepage = "https://github.com/ermakov-oleg/serpyco-rs"
 repository = "https://github.com/ermakov-oleg/serpyco-rs"
 
 [lib]
 name = "serpyco_rs"
 crate-type = ["cdylib"]
```

### Comparing `serpyco_rs-1.7.1/.github/workflows/CI.yml` & `serpyco_rs-1.8.0/.github/workflows/CI.yml`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,305 +1,305 @@
-name: CI
-
-on:
-  push:
-    tags:
-      - '**'
-    branches:
-      - main
-      - master
-  pull_request:
-  workflow_dispatch:
-
-jobs:
-  build:
-    strategy:
-      fail-fast: false
-      matrix:
-        os:
-          - ubuntu-latest
-          - windows-latest
-          - macos-latest
-        python-version:
-          - "3.9"
-          - "3.10"
-          - "3.11"
-          - "3.12"
-        include:
-          - os: macos-latest
-            target: universal2-apple-darwin
-    name: Build on ${{ matrix.os}} ${{ matrix.python-version }}
-    runs-on: ${{ matrix.os }}
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        id: python
-        with:
-          python-version: ${{ matrix.python-version }}
-          cache: 'pip'
-
-      - uses: actions/cache@v4
-        id: cache-uv
-        with:
-          path: ~/.cache/uv
-          key: ${{ runner.os }}-python-${{ matrix.python-version }}-uv
-
-      - name: Install rust stable
-        id: rust-toolchain
-        uses: dtolnay/rust-toolchain@stable
-        with:
-          components: llvm-tools
-
-      - uses: PyO3/maturin-action@v1
-        with:
-          manylinux: auto
-          target: ${{ matrix.target }}
-          rust-toolchain: stable
-          sccache: 'true'
-          args: >
-            --release 
-            --sdist 
-            --interpreter ${{ matrix.python-version }} 
-            --out pgo-wheel
-        env:
-          RUSTFLAGS: "-Cprofile-generate=${{ github.workspace }}/target/profdata"
-
-      - name: Get rust host
-        run: echo RUST_HOST=$(rustc -Vv | grep host | cut -d ' ' -f 2) >> "$GITHUB_ENV"
-        shell: bash
-
-      - name: Generate pgo data
-        run: |
-          pip install -U uv
-          uv pip install -r requirements/bench.txt --python ${{ steps.python.outputs.python-path }}
-          uv pip install serpyco_rs --no-index --no-deps --find-links pgo-wheel --force-reinstall --python ${{ steps.python.outputs.python-path }}
-          # Install package deps
-          uv pip install serpyco_rs --find-links pgo-wheel --python ${{ steps.python.outputs.python-path }}
-          pytest bench -k "not mashumaro and not marshmallow and not pydantic"
-          rustup run stable bash -c 'echo LLVM_PROFDATA=$RUSTUP_HOME/toolchains/$RUSTUP_TOOLCHAIN/lib/rustlib/${{ env.RUST_HOST }}/bin/llvm-profdata >> "$GITHUB_ENV"'
-
-#      - name: Setup upterm session
-#        uses: lhotari/action-upterm@v1
-
-      - name: Merge pgo data
-        run: ${{ env.LLVM_PROFDATA }} merge -o ${{ github.workspace }}/merged.profdata ${{ github.workspace }}/target/profdata
-
-      - name: Build pgo-optimized wheel
-        uses: PyO3/maturin-action@v1
-        with:
-          manylinux: auto
-          rust-toolchain: stable
-          command: build
-          target: ${{ matrix.target }}
-          sccache: 'true'
-          args: >
-            --release 
-            --sdist 
-            --interpreter ${{ matrix.python-version }} 
-            --out dist
-        env:
-          RUSTFLAGS: "-Cprofile-use=${{ github.workspace }}/merged.profdata"
-
-      - name: Upload wheels
-        uses: actions/upload-artifact@v2
-        with:
-          name: wheels
-          path: dist
-
-  linux-cross:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        platform:
-          - target: aarch64-unknown-linux-gnu
-            arch: aarch64
-            # and https://github.com/gnzlbg/jemallocator/issues/170#issuecomment-1503228963
-            maturin_docker_options: -e JEMALLOC_SYS_WITH_LG_PAGE=16
-          - target: armv7-unknown-linux-gnueabihf
-            arch: armv7
-          - target: s390x-unknown-linux-gnu
-            arch: s390x
-          - target: powerpc64le-unknown-linux-gnu
-            arch: ppc64le
-          - target: powerpc64-unknown-linux-gnu
-            arch: ppc64
-
-    steps:
-      - uses: actions/checkout@v4
-      - name: "Build wheels"
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.platform.target }}
-          manylinux: auto
-          docker-options: ${{ matrix.platform.maturin_docker_options }}
-          args: --release --sdist -o dist --interpreter 3.9 3.10 3.11 3.12
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v2
-        with:
-          name: wheels
-          path: dist
-
-  test:
-    needs: [ build ]
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [ ubuntu-latest, macos-latest, windows-latest ]
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
-
-    name: Test on ${{ matrix.os}} ${{ matrix.python-version }}
-    runs-on: ${{ matrix.os }}
-    steps:
-      - uses: actions/checkout@v3
-      - name: set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-      - uses: actions/download-artifact@v2
-        with:
-          name: wheels
-          path: wheels
-      - name: install dependencies
-        run: |
-          # https://github.com/astral-sh/uv/issues/2450
-          python -m pip install --upgrade pip nox uv==0.1.18
-      - name: tests
-        run: nox -s test
-        env:
-          CI: true
-      - name: lint
-        run: nox -s lint
-        env:
-          CI: true
-      - name: check types
-        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
-        run: nox -s type_check
-        env:
-          CI: true
-
-  benchmark:
-    needs: [ build ]
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [ ubuntu-latest, macos-latest ]
-    name: Benchmark on ${{ matrix.os}}
-    runs-on: ${{ matrix.os }}
-    steps:
-      - uses: actions/checkout@v3
-      - name: set up Python 3.11
-        uses: actions/setup-python@v4
-        with:
-          python-version: 3.11
-      - uses: actions/download-artifact@v2
-        with:
-          name: wheels
-          path: wheels
-      - name: install dependencies
-        run: |
-          # https://github.com/astral-sh/uv/issues/2450
-          python -m pip install --upgrade pip nox uv==0.1.18
-          nox -s bench --no-venv --install-only
-      - name: bench
-        run: nox -s bench --no-venv --no-install
-        env:
-          CI: true
-
-  test_rc_leaks:
-    name: Test reference count leaks
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: deadsnakes/action@v3.1.0
-        with:
-          python-version: 3.11
-          debug: true
-      - run: python3.11 --version --version && which python3.11 && python3.11 -c "import sys; print(sys.gettotalrefcount())"
-      - uses: PyO3/maturin-action@v1
-        with:
-          command: build
-          args: --release --sdist -o wheels
-      - name: install dependencies
-        run: |
-          # https://github.com/astral-sh/uv/issues/2450
-          python -m pip install --upgrade pip nox uv==0.1.18
-          nox -s test_rc_leaks --no-venv --install-only
-      - name: tests
-        run: nox -s test_rc_leaks --no-venv --no-install
-
-  benchmark-codespeed:
-    needs: [ build ]
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/cache@v4
-        id: cache-uv
-        with:
-          path: ~/.cache/uv
-          key: ubuntu-latest-python-3.12-uv
-      - name: set up Python 3.12
-        uses: actions/setup-python@v4
-        with:
-          python-version: 3.12
-          cache: 'pip'
-          cache-dependency-path: |
-            requirements/*.txt
-      - uses: actions/download-artifact@v2
-        with:
-          name: wheels
-          path: wheels
-      - name: install dependencies
-        run: |
-          # https://github.com/astral-sh/uv/issues/2450
-          python -m pip install --upgrade pip nox uv==0.1.18
-          nox -s bench_codespeed --no-venv --install-only
-      - name: Run benchmarks
-        uses: CodSpeedHQ/action@v2
-        with:
-          token: ${{ secrets.CODSPEED_TOKEN }}
-          run: nox -s bench_codespeed --no-venv --no-install
-        env:
-          CI: true
-
-  fmt:
-    name: rustfmt
-    runs-on: ubuntu-20.04
-    steps:
-      - uses: actions/checkout@v2
-      - uses: actions-rs/toolchain@v1
-        with:
-          profile: minimal
-          toolchain: stable
-          override: true
-          components: rustfmt
-      - run: cargo fmt --all -- --check
-
-  clippy:
-    name: clippy
-    runs-on: ubuntu-20.04
-    steps:
-      - uses: actions/checkout@v2
-      - uses: actions-rs/toolchain@v1
-        with:
-          profile: minimal
-          toolchain: stable
-          override: true
-          components: clippy
-      - run: cargo clippy --all-targets --all-features -- -D warnings
-
-  release:
-    name: release
-    runs-on: ubuntu-latest
-    if: startsWith(github.event.ref, 'refs/tags')
-    needs: [ build, linux-cross, test ]
-    steps:
-      - uses: actions/download-artifact@v2
-        with:
-          name: wheels
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
+name: CI
+
+on:
+  push:
+    tags:
+      - '**'
+    branches:
+      - main
+      - master
+  pull_request:
+  workflow_dispatch:
+
+jobs:
+  build:
+    strategy:
+      fail-fast: false
+      matrix:
+        os:
+          - ubuntu-latest
+          - windows-latest
+          - macos-latest
+        python-version:
+          - "3.9"
+          - "3.10"
+          - "3.11"
+          - "3.12"
+        include:
+          - os: macos-latest
+            target: universal2-apple-darwin
+    name: Build on ${{ matrix.os}} ${{ matrix.python-version }}
+    runs-on: ${{ matrix.os }}
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        id: python
+        with:
+          python-version: ${{ matrix.python-version }}
+          cache: 'pip'
+
+      - uses: actions/cache@v4
+        id: cache-uv
+        with:
+          path: ~/.cache/uv
+          key: ${{ runner.os }}-python-${{ matrix.python-version }}-uv
+
+      - name: Install rust stable
+        id: rust-toolchain
+        uses: dtolnay/rust-toolchain@stable
+        with:
+          components: llvm-tools
+
+      - uses: PyO3/maturin-action@v1
+        with:
+          manylinux: auto
+          target: ${{ matrix.target }}
+          rust-toolchain: stable
+          sccache: 'true'
+          args: >
+            --release 
+            --sdist 
+            --interpreter ${{ matrix.python-version }} 
+            --out pgo-wheel
+        env:
+          RUSTFLAGS: "-Cprofile-generate=${{ github.workspace }}/target/profdata"
+
+      - name: Get rust host
+        run: echo RUST_HOST=$(rustc -Vv | grep host | cut -d ' ' -f 2) >> "$GITHUB_ENV"
+        shell: bash
+
+      - name: Generate pgo data
+        run: |
+          pip install -U uv
+          uv pip install -r requirements/bench.txt --python ${{ steps.python.outputs.python-path }}
+          uv pip install serpyco_rs --no-index --no-deps --find-links pgo-wheel --force-reinstall --python ${{ steps.python.outputs.python-path }}
+          # Install package deps
+          uv pip install serpyco_rs --find-links pgo-wheel --python ${{ steps.python.outputs.python-path }}
+          pytest bench -k "not mashumaro and not marshmallow and not pydantic"
+          rustup run stable bash -c 'echo LLVM_PROFDATA=$RUSTUP_HOME/toolchains/$RUSTUP_TOOLCHAIN/lib/rustlib/${{ env.RUST_HOST }}/bin/llvm-profdata >> "$GITHUB_ENV"'
+
+#      - name: Setup upterm session
+#        uses: lhotari/action-upterm@v1
+
+      - name: Merge pgo data
+        run: ${{ env.LLVM_PROFDATA }} merge -o ${{ github.workspace }}/merged.profdata ${{ github.workspace }}/target/profdata
+
+      - name: Build pgo-optimized wheel
+        uses: PyO3/maturin-action@v1
+        with:
+          manylinux: auto
+          rust-toolchain: stable
+          command: build
+          target: ${{ matrix.target }}
+          sccache: 'true'
+          args: >
+            --release 
+            --sdist 
+            --interpreter ${{ matrix.python-version }} 
+            --out dist
+        env:
+          RUSTFLAGS: "-Cprofile-use=${{ github.workspace }}/merged.profdata"
+
+      - name: Upload wheels
+        uses: actions/upload-artifact@v2
+        with:
+          name: wheels
+          path: dist
+
+  linux-cross:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        platform:
+          - target: aarch64-unknown-linux-gnu
+            arch: aarch64
+            # and https://github.com/gnzlbg/jemallocator/issues/170#issuecomment-1503228963
+            maturin_docker_options: -e JEMALLOC_SYS_WITH_LG_PAGE=16
+          - target: armv7-unknown-linux-gnueabihf
+            arch: armv7
+          - target: s390x-unknown-linux-gnu
+            arch: s390x
+          - target: powerpc64le-unknown-linux-gnu
+            arch: ppc64le
+          - target: powerpc64-unknown-linux-gnu
+            arch: ppc64
+
+    steps:
+      - uses: actions/checkout@v4
+      - name: "Build wheels"
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.platform.target }}
+          manylinux: auto
+          docker-options: ${{ matrix.platform.maturin_docker_options }}
+          args: --release --sdist -o dist --interpreter 3.9 3.10 3.11 3.12
+          sccache: 'true'
+      - name: Upload wheels
+        uses: actions/upload-artifact@v2
+        with:
+          name: wheels
+          path: dist
+
+  test:
+    needs: [ build ]
+    strategy:
+      fail-fast: false
+      matrix:
+        os: [ ubuntu-latest, macos-latest, windows-latest ]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
+
+    name: Test on ${{ matrix.os}} ${{ matrix.python-version }}
+    runs-on: ${{ matrix.os }}
+    steps:
+      - uses: actions/checkout@v3
+      - name: set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+      - uses: actions/download-artifact@v2
+        with:
+          name: wheels
+          path: wheels
+      - name: install dependencies
+        run: |
+          # https://github.com/astral-sh/uv/issues/2450
+          python -m pip install --upgrade pip nox uv==0.1.18
+      - name: tests
+        run: nox -s test
+        env:
+          CI: true
+      - name: lint
+        run: nox -s lint
+        env:
+          CI: true
+      - name: check types
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
+        run: nox -s type_check
+        env:
+          CI: true
+
+  benchmark:
+    needs: [ build ]
+    strategy:
+      fail-fast: false
+      matrix:
+        os: [ ubuntu-latest, macos-latest ]
+    name: Benchmark on ${{ matrix.os}}
+    runs-on: ${{ matrix.os }}
+    steps:
+      - uses: actions/checkout@v3
+      - name: set up Python 3.11
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.11
+      - uses: actions/download-artifact@v2
+        with:
+          name: wheels
+          path: wheels
+      - name: install dependencies
+        run: |
+          # https://github.com/astral-sh/uv/issues/2450
+          python -m pip install --upgrade pip nox uv==0.1.18
+          nox -s bench --no-venv --install-only
+      - name: bench
+        run: nox -s bench --no-venv --no-install
+        env:
+          CI: true
+
+  test_rc_leaks:
+    name: Test reference count leaks
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: deadsnakes/action@v3.1.0
+        with:
+          python-version: 3.11
+          debug: true
+      - run: python3.11 --version --version && which python3.11 && python3.11 -c "import sys; print(sys.gettotalrefcount())"
+      - uses: PyO3/maturin-action@v1
+        with:
+          command: build
+          args: --release --sdist -o wheels
+      - name: install dependencies
+        run: |
+          # https://github.com/astral-sh/uv/issues/2450
+          python -m pip install --upgrade pip nox uv==0.1.18
+          nox -s test_rc_leaks --no-venv --install-only
+      - name: tests
+        run: nox -s test_rc_leaks --no-venv --no-install
+
+  benchmark-codespeed:
+    needs: [ build ]
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/cache@v4
+        id: cache-uv
+        with:
+          path: ~/.cache/uv
+          key: ubuntu-latest-python-3.12-uv
+      - name: set up Python 3.12
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.12
+          cache: 'pip'
+          cache-dependency-path: |
+            requirements/*.txt
+      - uses: actions/download-artifact@v2
+        with:
+          name: wheels
+          path: wheels
+      - name: install dependencies
+        run: |
+          # https://github.com/astral-sh/uv/issues/2450
+          python -m pip install --upgrade pip nox uv==0.1.18
+          nox -s bench_codespeed --no-venv --install-only
+      - name: Run benchmarks
+        uses: CodSpeedHQ/action@v2
+        with:
+          token: ${{ secrets.CODSPEED_TOKEN }}
+          run: nox -s bench_codespeed --no-venv --no-install
+        env:
+          CI: true
+
+  fmt:
+    name: rustfmt
+    runs-on: ubuntu-20.04
+    steps:
+      - uses: actions/checkout@v2
+      - uses: actions-rs/toolchain@v1
+        with:
+          profile: minimal
+          toolchain: stable
+          override: true
+          components: rustfmt
+      - run: cargo fmt --all -- --check
+
+  clippy:
+    name: clippy
+    runs-on: ubuntu-20.04
+    steps:
+      - uses: actions/checkout@v2
+      - uses: actions-rs/toolchain@v1
+        with:
+          profile: minimal
+          toolchain: stable
+          override: true
+          components: clippy
+      - run: cargo clippy --all-targets --all-features -- -D warnings
+
+  release:
+    name: release
+    runs-on: ubuntu-latest
+    if: startsWith(github.event.ref, 'refs/tags')
+    needs: [ build, linux-cross, test ]
+    steps:
+      - uses: actions/download-artifact@v2
+        with:
+          name: wheels
+      - name: Publish to PyPI
+        uses: PyO3/maturin-action@v1
+        env:
+          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
+        with:
+          command: upload
+          args: --skip-existing *
```

### Comparing `serpyco_rs-1.7.1/LICENSE` & `serpyco_rs-1.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ermakov-oleg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 ermakov-oleg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `serpyco_rs-1.7.1/README.md` & `serpyco_rs-1.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,455 +1,567 @@
-# serpyco-rs: a serializer for python dataclasses
-[![PyPI version](https://img.shields.io/pypi/v/serpyco-rs.svg)](https://pypi.org/project/serpyco-rs) [![Python
-versions](https://img.shields.io/pypi/pyversions/serpyco-rs.svg)](https://pypi.org/project/serpyco-rs) [![CI status](https://github.com/ermakov-oleg/serpyco-rs/actions/workflows/CI.yml/badge.svg)](https://github.com/ermakov-oleg/serpyco-rs/actions)
+Metadata-Version: 2.3
+Name: serpyco-rs
+Version: 1.8.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Rust
+Requires-Dist: typing-inspect >=0.8.0
+Requires-Dist: attributes-doc
+Requires-Dist: typing-extensions
+License-File: LICENSE
+Home-Page: https://github.com/ermakov-oleg/serpyco-rs
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/ermakov-oleg/serpyco-rs
+
+# serpyco-rs: a serializer for python dataclasses
+[![PyPI version](https://img.shields.io/pypi/v/serpyco-rs.svg)](https://pypi.org/project/serpyco-rs) [![Python
+versions](https://img.shields.io/pypi/pyversions/serpyco-rs.svg)](https://pypi.org/project/serpyco-rs) [![CI status](https://github.com/ermakov-oleg/serpyco-rs/actions/workflows/CI.yml/badge.svg)](https://github.com/ermakov-oleg/serpyco-rs/actions)
+
+## What is serpyco-rs ?
+
+
+Serpyco is a serialization library for [Python 3.9+ dataclasses](https://docs.python.org/3/library/dataclasses.html) that works just by defining your dataclasses:
+
+```python
+import dataclasses
+import serpyco_rs
+
+@dataclasses.dataclass
+class Example:
+    name: str
+    num: int
+    tags: list[str]
+
+
+serializer = serpyco_rs.Serializer(Example)
+
+result = serializer.dump(Example(name="foo", num=2, tags=["hello", "world"]))
+print(result)
+
+>> {'name': 'foo', 'num': 2, 'tags': ['hello', 'world']}
+```
+
+Inspired by [serpyco](https://pypi.org/project/serpyco/).
+
+serpyco-rs works by analysing the dataclass fields and can recognize many types : `list`, `tuple`, `Optional`... 
+You can also embed other dataclasses in a definition.
+
+The main use-case for serpyco-rs is to serialize objects for an API, but it can be helpful whenever you need to transform objects to/from builtin Python types.
+
+## Installation
+Use pip to install:
+
+```bash
+$ pip install serpyco-rs
+```
+
+
+## Features
+
+- Serialization and deserialization of dataclasses
+- Validation of input data
+- Very fast
+- Support recursive schemas
+- Generate JSON Schema Specification (Draft 2020-12)
+- Support custom encoders/decoders for fields
+- Support deserialization from query string parameters (MultiDict like structures) with from string coercion 
+
+## Supported field types
+There is support for generic types from the standard typing module:
+
+* Decimal
+* UUID
+* Time
+* Date
+* DateTime
+* Enum
+* List
+* Dict
+* Bytes (pass through)
+* TypedDict
+* Mapping
+* Sequence
+* Tuple (fixed size)
+* Literal[str, ...]
+* Unions / Tagged unions
+
+## Benchmarks
+
+<details>
+  <summary>Linux</summary>
+  
+  #### Load
+  
+  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
+  |-------------|---------------------------------|-------------------------|----------------------|
+  | serpyco_rs  |                            0.16 |                  6318.1 |                 1    |
+  | mashumaro   |                            0.45 |                  2244.4 |                 2.81 |
+  | pydantic    |                            0.57 |                  1753.9 |                 3.56 |
+  | serpyco     |                            0.82 |                  1228.3 |                 5.17 |
+  | marshmallow |                            8.49 |                   117.4 |                53.35 |
+  
+  #### Dump
+  
+  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
+  |-------------|---------------------------------|-------------------------|----------------------|
+  | serpyco_rs  |                            0.07 |                 13798   |                 1    |
+  | serpyco     |                            0.07 |                 13622   |                 1.02 |
+  | mashumaro   |                            0.1  |                 10219.5 |                 1.36 |
+  | pydantic    |                            0.22 |                  4615.5 |                 2.99 |
+  | marshmallow |                            2    |                   497   |                27.69 |
+</details>
+
+
+<details>
+  <summary>MacOS</summary>
+  macOS Monterey / Apple M1 Pro / 16GB RAM / Python 3.11.0
+  
+  #### Load
+  
+  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
+  |-------------|---------------------------------|-------------------------|----------------------|
+  | serpyco_rs  |                            0.1  |                  9865.1 |                 1    |
+  | mashumaro   |                            0.2  |                  4968   |                 2    |
+  | pydantic    |                            0.34 |                  2866.7 |                 3.42 |
+  | serpyco     |                            0.69 |                  1444.1 |                 6.87 |
+  | marshmallow |                            4.14 |                   241.8 |                41.05 |
+
+  #### Dump
+  
+  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
+  |-------------|---------------------------------|-------------------------|----------------------|
+  | serpyco_rs  |                            0.04 |                 22602.6 |                 1    |
+  | serpyco     |                            0.05 |                 21232.9 |                 1.06 |
+  | mashumaro   |                            0.06 |                 15903.4 |                 1.42 |
+  | pydantic    |                            0.16 |                  6262.6 |                 3.61 |
+  | marshmallow |                            1.04 |                   962   |                23.5  |
+</details>
+
+
+## Supported annotations
+
+`serpyco-rs` supports changing load/dump behavior with `typing.Annotated`.
+
+Currently available:
+* Alias
+* FieldFormat (CamelCase / NoFormat)
+* NoneFormat (OmitNone / KeepNone)
+* Discriminator
+* Min / Max
+* MinLength / MaxLength
+* CustomEncoder
+* NoneAsDefaultForOptional (ForceDefaultForOptional)
+
+
+### Alias
+`Alias` is needed to override the field name in the structure used for `load` / `dump`.
+
+```python
+from dataclasses import dataclass
+from typing import Annotated
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import Alias
+
+@dataclass
+class A:
+    foo: Annotated[int, Alias('bar')]
+
+ser = Serializer(A)
+
+print(ser.load({'bar': 1}))
+>> A(foo=1)
+
+print(ser.dump(A(foo=1)))
+>> {'bar': 1}
+```
+
+### FieldFormat
+Used to have response bodies in camelCase while keeping your python code in snake_case.
+
+```python
+from dataclasses import dataclass
+from typing import Annotated
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import CamelCase, NoFormat
+
+@dataclass
+class B:
+    buz_filed: str
+
+@dataclass
+class A:
+    foo_filed: int
+    bar_filed: Annotated[B, NoFormat]
+
+ser = Serializer(Annotated[A, CamelCase])  # or ser = Serializer(A, camelcase_fields=True)
+
+print(ser.dump(A(foo_filed=1, bar_filed=B(buz_filed='123'))))
+>> {'fooFiled': 1, 'barFiled': {'buz_filed': '123'}}
+
+print(ser.load({'fooFiled': 1, 'barFiled': {'buz_filed': '123'}}))
+>> A(foo_filed=1, bar_filed=B(buz_filed='123'))
+```
+
+### NoneFormat
+Via `OmitNone` we can drop None values for non required fields in the serialized dicts
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+
+@dataclass
+class A:
+    required_val: bool | None
+    optional_val: bool | None = None
+
+ser = Serializer(A, omit_none=True) # or Serializer(Annotated[A, OmitNone])
+
+print(ser.dump(A(required_val=None, optional_val=None)))
+>>> {'required_val': None}
+```
+
+### Unions
+
+`serpyco-rs` supports unions of types.
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+
+@dataclass
+class Foo:
+    val: int
+
+ser = Serializer(Foo | int)
+
+print(ser.load({'val': 1}))
+>> Foo(val=1)
+print(ser.load(1))
+>> 1
+```
+
+But performance of unions is worse than for single dataclasses. Because we need to check all possible types in the union.
+For better performance, you can use [Tagged unions](#tagged-unions).
+
+
+### Tagged unions
+
+Supports tagged joins with discriminator field.
+
+All classes in the union must be dataclasses or attrs with discriminator field `Literal[str]`.
+
+**The discriminator field is always mandatory.**
+
+```python
+from typing import Annotated, Literal
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import Discriminator
+
+@dataclass
+class Foo:
+    type: Literal['foo']
+    value: int
+
+@dataclass(kw_only=True)
+class Bar:
+    type: Literal['bar'] = 'bar'
+    value: str
+
+ser = Serializer(list[Annotated[Foo | Bar, Discriminator('type')]])
+
+print(ser.load([{'type': 'foo', 'value': 1}, {'type': 'bar', 'value': 'buz'}]))
+>>> [Foo(type='foo', value=1), Bar(type='bar', value='buz')]
+```
+
+### Min / Max
+
+Supported for `int` / `float` / `Decimal` types and only for validation on load.
+
+```python
+from typing import Annotated
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import Min, Max
+
+ser = Serializer(Annotated[int, Min(1), Max(10)])
+
+ser.load(123)
+>> SchemaValidationError: [ErrorItem(message='123 is greater than the maximum of 10', instance_path='')]
+```
+
+### MinLength / MaxLength
+`MinLength` / `MaxLength` can be used to restrict the length of loaded strings.
+
+```python
+from typing import Annotated
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import MinLength
+
+ser = Serializer(Annotated[str, MinLength(5)])
+
+ser.load("1234")
+>> SchemaValidationError: [ErrorItem(message='"1234" is shorter than 5 characters', instance_path='')]
+```
+
+### NoneAsDefaultForOptional
+`ForceDefaultForOptional` / `KeepDefaultForOptional` can be used to set None as default value for optional (nullable) fields.
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+
+
+@dataclass
+class Foo:
+    val: int                 # not nullable + required
+    val1: int | None         # nullable + required
+    val2: int | None = None  # nullable + not required
+
+ser_force_default = Serializer(Foo, force_default_for_optional=True)  # or Serializer(Annotated[Foo, ForceDefaultForOptional])
+ser = Serializer(Foo)
+
+# all fields except val are optional and nullable
+assert ser_force_default.load({'val': 1}) == Foo(val=1, val1=None, val2=None) 
+
+# val1 field is required and nullable and val1 should be present in the dict
+ser.load({'val': 1})
+>> SchemaValidationError: [ErrorItem(message='"val1" is a required property', instance_path='')]
+```
+
+
+### Custom encoders for fields
+
+You can provide CustomEncoder with `serialize` and `deserialize` functions, or `serialize_with` and `deserialize_with` annotations.
+
+```python
+from typing import Annotated
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+from serpyco_rs.metadata import CustomEncoder
+
+@dataclass
+class Foo:
+    val: Annotated[str, CustomEncoder[str, str](serialize=str.upper, deserialize=str.lower)]
+
+ser = Serializer(Foo)
+val = ser.dump(Foo(val='bar'))
+>> {'val': 'BAR'}
+assert ser.load(val) == Foo(val='bar') 
+```
+
+**Note:** `CustomEncoder` has no effect to validation and JSON Schema generation.
+
+### Bytes fields
+
+`serpyco-rs` can loads bytes fields as is (without base64 encoding and validation).
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+
+@dataclass
+class Foo:
+    val: bytes
+
+ser = Serializer(Foo)
+ser.load({'val': b'123'}) == Foo(val=b'123')
+```
+
+
+## Getting JSON Schema
+
+`serpyco-rs` can generate JSON Schema for your dataclasses (Draft 2020-12).
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer
+
+@dataclass
+class A:
+    """Description of A"""
+    foo: int
+    bar: str
+
+ser = Serializer(A)
+
+print(ser.get_json_schema())
+>> {
+    '$schema': 'https://json-schema.org/draft/2020-12/schema', 
+    '$ref': '#/components/schemas/A[no_format,keep_nones]', 
+    'components': {
+        'schemas': {
+            'A[no_format,keep_nones]': {
+                'properties': {
+                    'foo': {'type': 'integer'}, 
+                    'bar': {'type': 'string'}
+                }, 
+                'required': ['foo', 'bar'], 
+                'type': 'object', 
+                'description': 'Description of A'
+            }
+        }
+    }
+}
+```
+
+Also, you can configure the schema generation via `JsonSchemaBuilder`.
+
+
+```python
+from dataclasses import dataclass
+from serpyco_rs import Serializer, JsonSchemaBuilder
+
+@dataclass
+class A:
+    foo: int
+    bar: str
+
+ser = Serializer(A)
+
+builder = JsonSchemaBuilder(
+  add_dialect_uri=False,
+  ref_prefix='#/definitions',
+)
+
+print(builder.build(ser))
+>> {'$ref': '#/definitions/__main__.A[no_format,keep_nones]'}
+
+print(builder.get_definitions())
+>> {
+  "__main__.A[no_format,keep_nones]": {
+    "properties": {
+      "foo": {
+        "type": "integer"
+      },
+      "bar": {
+        "type": "string"
+      }
+    },
+    "required": [
+      "foo",
+      "bar"
+    ],
+    "type": "object"
+  }
+}
+```
+
+## Query string deserialization
+
+`serpyco-rs` can deserialize query string parameters (MultiDict like structures) with from string coercion.
+
+```python
+
+from dataclasses import dataclass
+from urllib.parse import parse_qsl
+
+from serpyco_rs import Serializer
+from multidict import MultiDict
+
+@dataclass
+class A:
+    foo: int
+    bar: str
+
+ser = Serializer(A)
+
+print(ser.load_query_params(MultiDict(parse_qsl('foo=1&bar=2'))))
+>> A(foo=1, bar='2')
+```
+
+## Custom Type Support
+
+In `serpyco-rs`, you can add support for your own types by using the `custom_type_resolver` parameter and the `CustomType` class. This allows you to define how your custom types should be serialized and deserialized.
+
+### CustomType
+
+The `CustomType` class is a way to define how a custom type should be serialized and deserialized. It is a generic class that takes two type parameters: the type of the object to be serialized/deserialized and the type of the serialized/deserialized object.
+
+Here is an example of a `CustomType` for `IPv4Address`:
+
+```python
+from serpyco_rs import CustomType
+from ipaddress import IPv4Address, AddressValueError
+
+class IPv4AddressType(CustomType[IPv4Address, str]):
+    def serialize(self, obj: IPv4Address) -> str:
+        return str(obj)
+
+    def deserialize(self, data: str) -> IPv4Address:
+        try:
+            return IPv4Address(data)
+        except AddressValueError:
+            raise ValueError(f"Invalid IPv4 address: {data}")
+
+    def get_json_schema(self) -> dict:
+        return {"type": "string", "format": "ipv4"}
+```
+
+In this example, `IPv4AddressType` is a `CustomType` that serializes `IPv4Address` objects to strings and deserializes strings to `IPv4Address` objects. The `get_json_schema` method returns the JSON schema for the custom type.
+
+### custom_type_resolver
+
+The `custom_type_resolver` is a function that takes a type as input and returns an instance of `CustomType` if the type is supported, or `None` otherwise. This function is passed to the `Serializer` constructor.
+
+Here is an example of a `custom_type_resolver` that supports `IPv4Address`:
+
+```python
+def custom_type_resolver(t: type) -> CustomType | None
+    if t is IPv4Address:
+        return IPv4AddressType()
+    return None
+
+ser = Serializer(MyDataclass, custom_type_resolver=custom_type_resolver)
+```
+
+In this example, the `custom_type_resolver` function checks if the type is `IPv4Address` and returns an instance of `IPv4AddressType` if it is. Otherwise, it returns `None`. This function is then passed to the `Serializer` constructor, which uses it to handle `IPv4Address` fields in the dataclass.
+
+### Full Example
+
+```python
+from dataclasses import dataclass
+from ipaddress import IPv4Address
+from serpyco_rs import Serializer, CustomType
+
+# Define custom type for IPv4Address
+class IPv4AddressType(CustomType[IPv4Address, str]):
+    def serialize(self, value: IPv4Address) -> str:
+        return str(value)
+
+    def deserialize(self, value: str) -> IPv4Address:
+        return IPv4Address(value)
+
+    def get_json_schema(self):
+        return {
+            'type': 'string',
+            'format': 'ipv4',
+        }
+
+# Defining custom_type_resolver
+def custom_type_resolver(t: type) -> CustomType | None:
+    if t is IPv4Address:
+        return IPv4AddressType()
+    return None
+
+@dataclass
+class Data:
+    ip: IPv4Address
+
+# Use custom_type_resolver in Serializer
+serializer = Serializer(Data, custom_type_resolver=custom_type_resolver)
+
+# Example usage
+data = Data(ip=IPv4Address('1.1.1.1'))
+serialized_data = serializer.dump(data)  # {'ip': '1.1.1.1'}
+deserialized_data = serializer.load(serialized_data)  # Data(ip=IPv4Address('1.1.1.1'))
+```
 
-## What is serpyco-rs ?
-
-
-Serpyco is a serialization library for [Python 3.9+ dataclasses](https://docs.python.org/3/library/dataclasses.html) that works just by defining your dataclasses:
-
-```python
-import dataclasses
-import serpyco_rs
-
-@dataclasses.dataclass
-class Example:
-    name: str
-    num: int
-    tags: list[str]
-
-
-serializer = serpyco_rs.Serializer(Example)
-
-result = serializer.dump(Example(name="foo", num=2, tags=["hello", "world"]))
-print(result)
-
->> {'name': 'foo', 'num': 2, 'tags': ['hello', 'world']}
-```
-
-Inspired by [serpyco](https://pypi.org/project/serpyco/).
-
-serpyco-rs works by analysing the dataclass fields and can recognize many types : `list`, `tuple`, `Optional`... 
-You can also embed other dataclasses in a definition.
-
-The main use-case for serpyco-rs is to serialize objects for an API, but it can be helpful whenever you need to transform objects to/from builtin Python types.
-
-## Installation
-Use pip to install:
-
-```bash
-$ pip install serpyco-rs
-```
-
-
-## Features
-
-- Serialization and deserialization of dataclasses
-- Validation of input data
-- Very fast
-- Support recursive schemas
-- Generate JSON Schema Specification (Draft 2020-12)
-- Support custom encoders/decoders for fields
-- Support deserialization from query string parameters (MultiDict like structures) with from string coercion 
-
-## Supported field types
-There is support for generic types from the standard typing module:
-
-* Decimal
-* UUID
-* Time
-* Date
-* DateTime
-* Enum
-* List
-* Dict
-* Bytes (pass through)
-* TypedDict
-* Mapping
-* Sequence
-* Tuple (fixed size)
-* Literal[str, ...]
-* Unions / Tagged unions
-
-## Benchmarks
-
-<details>
-  <summary>Linux</summary>
-  
-  #### Load
-  
-  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
-  |-------------|---------------------------------|-------------------------|----------------------|
-  | serpyco_rs  |                            0.16 |                  6318.1 |                 1    |
-  | mashumaro   |                            0.45 |                  2244.4 |                 2.81 |
-  | pydantic    |                            0.57 |                  1753.9 |                 3.56 |
-  | serpyco     |                            0.82 |                  1228.3 |                 5.17 |
-  | marshmallow |                            8.49 |                   117.4 |                53.35 |
-  
-  #### Dump
-  
-  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
-  |-------------|---------------------------------|-------------------------|----------------------|
-  | serpyco_rs  |                            0.07 |                 13798   |                 1    |
-  | serpyco     |                            0.07 |                 13622   |                 1.02 |
-  | mashumaro   |                            0.1  |                 10219.5 |                 1.36 |
-  | pydantic    |                            0.22 |                  4615.5 |                 2.99 |
-  | marshmallow |                            2    |                   497   |                27.69 |
-</details>
-
-
-<details>
-  <summary>MacOS</summary>
-  macOS Monterey / Apple M1 Pro / 16GB RAM / Python 3.11.0
-  
-  #### Load
-  
-  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
-  |-------------|---------------------------------|-------------------------|----------------------|
-  | serpyco_rs  |                            0.1  |                  9865.1 |                 1    |
-  | mashumaro   |                            0.2  |                  4968   |                 2    |
-  | pydantic    |                            0.34 |                  2866.7 |                 3.42 |
-  | serpyco     |                            0.69 |                  1444.1 |                 6.87 |
-  | marshmallow |                            4.14 |                   241.8 |                41.05 |
-
-  #### Dump
-  
-  | Library     |   Median latency (milliseconds) |   Operations per second |   Relative (latency) |
-  |-------------|---------------------------------|-------------------------|----------------------|
-  | serpyco_rs  |                            0.04 |                 22602.6 |                 1    |
-  | serpyco     |                            0.05 |                 21232.9 |                 1.06 |
-  | mashumaro   |                            0.06 |                 15903.4 |                 1.42 |
-  | pydantic    |                            0.16 |                  6262.6 |                 3.61 |
-  | marshmallow |                            1.04 |                   962   |                23.5  |
-</details>
-
-
-## Supported annotations
-
-`serpyco-rs` supports changing load/dump behavior with `typing.Annotated`.
-
-Currently available:
-* Alias
-* FieldFormat (CamelCase / NoFormat)
-* NoneFormat (OmitNone / KeepNone)
-* Discriminator
-* Min / Max
-* MinLength / MaxLength
-* CustomEncoder
-* NoneAsDefaultForOptional (ForceDefaultForOptional)
-
-
-### Alias
-`Alias` is needed to override the field name in the structure used for `load` / `dump`.
-
-```python
-from dataclasses import dataclass
-from typing import Annotated
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import Alias
-
-@dataclass
-class A:
-    foo: Annotated[int, Alias('bar')]
-
-ser = Serializer(A)
-
-print(ser.load({'bar': 1}))
->> A(foo=1)
-
-print(ser.dump(A(foo=1)))
->> {'bar': 1}
-```
-
-### FieldFormat
-Used to have response bodies in camelCase while keeping your python code in snake_case.
-
-```python
-from dataclasses import dataclass
-from typing import Annotated
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import CamelCase, NoFormat
-
-@dataclass
-class B:
-    buz_filed: str
-
-@dataclass
-class A:
-    foo_filed: int
-    bar_filed: Annotated[B, NoFormat]
-
-ser = Serializer(Annotated[A, CamelCase])  # or ser = Serializer(A, camelcase_fields=True)
-
-print(ser.dump(A(foo_filed=1, bar_filed=B(buz_filed='123'))))
->> {'fooFiled': 1, 'barFiled': {'buz_filed': '123'}}
-
-print(ser.load({'fooFiled': 1, 'barFiled': {'buz_filed': '123'}}))
->> A(foo_filed=1, bar_filed=B(buz_filed='123'))
-```
-
-### NoneFormat
-Via `OmitNone` we can drop None values for non required fields in the serialized dicts
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-
-@dataclass
-class A:
-    required_val: bool | None
-    optional_val: bool | None = None
-
-ser = Serializer(A, omit_none=True) # or Serializer(Annotated[A, OmitNone])
-
-print(ser.dump(A(required_val=None, optional_val=None)))
->>> {'required_val': None}
-```
-
-### Unions
-
-`serpyco-rs` supports unions of types.
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-
-@dataclass
-class Foo:
-    val: int
-
-ser = Serializer(Foo | int)
-
-print(ser.load({'val': 1}))
->> Foo(val=1)
-print(ser.load(1))
->> 1
-```
-
-But performance of unions is worse than for single dataclasses. Because we need to check all possible types in the union.
-For better performance, you can use [Tagged unions](#tagged-unions).
-
-
-### Tagged unions
-
-Supports tagged joins with discriminator field.
-
-All classes in the union must be dataclasses or attrs with discriminator field `Literal[str]`.
-
-**The discriminator field is always mandatory.**
-
-```python
-from typing import Annotated, Literal
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import Discriminator
-
-@dataclass
-class Foo:
-    type: Literal['foo']
-    value: int
-
-@dataclass(kw_only=True)
-class Bar:
-    type: Literal['bar'] = 'bar'
-    value: str
-
-ser = Serializer(list[Annotated[Foo | Bar, Discriminator('type')]])
-
-print(ser.load([{'type': 'foo', 'value': 1}, {'type': 'bar', 'value': 'buz'}]))
->>> [Foo(type='foo', value=1), Bar(type='bar', value='buz')]
-```
-
-### Min / Max
-
-Supported for `int` / `float` / `Decimal` types and only for validation on load.
-
-```python
-from typing import Annotated
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import Min, Max
-
-ser = Serializer(Annotated[int, Min(1), Max(10)])
-
-ser.load(123)
->> SchemaValidationError: [ErrorItem(message='123 is greater than the maximum of 10', instance_path='')]
-```
-
-### MinLength / MaxLength
-`MinLength` / `MaxLength` can be used to restrict the length of loaded strings.
-
-```python
-from typing import Annotated
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import MinLength
-
-ser = Serializer(Annotated[str, MinLength(5)])
-
-ser.load("1234")
->> SchemaValidationError: [ErrorItem(message='"1234" is shorter than 5 characters', instance_path='')]
-```
-
-### NoneAsDefaultForOptional
-`ForceDefaultForOptional` / `KeepDefaultForOptional` can be used to set None as default value for optional (nullable) fields.
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-
-
-@dataclass
-class Foo:
-    val: int                 # not nullable + required
-    val1: int | None         # nullable + required
-    val2: int | None = None  # nullable + not required
-
-ser_force_default = Serializer(Foo, force_default_for_optional=True)  # or Serializer(Annotated[Foo, ForceDefaultForOptional])
-ser = Serializer(Foo)
-
-# all fields except val are optional and nullable
-assert ser_force_default.load({'val': 1}) == Foo(val=1, val1=None, val2=None) 
-
-# val1 field is required and nullable and val1 should be present in the dict
-ser.load({'val': 1})
->> SchemaValidationError: [ErrorItem(message='"val1" is a required property', instance_path='')]
-```
-
-
-### Custom encoders for fields
-
-You can provide CustomEncoder with `serialize` and `deserialize` functions, or `serialize_with` and `deserialize_with` annotations.
-
-```python
-from typing import Annotated
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import CustomEncoder
-
-@dataclass
-class Foo:
-    val: Annotated[str, CustomEncoder[str, str](serialize=str.upper, deserialize=str.lower)]
-
-ser = Serializer(Foo)
-val = ser.dump(Foo(val='bar'))
->> {'val': 'BAR'}
-assert ser.load(val) == Foo(val='bar') 
-```
-
-**Note:** `CustomEncoder` has no effect to validation and JSON Schema generation.
-
-### Bytes fields
-
-`serpyco-rs` can loads bytes fields as is (without base64 encoding and validation).
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-
-@dataclass
-class Foo:
-    val: bytes
-
-ser = Serializer(Foo)
-ser.load({'val': b'123'}) == Foo(val=b'123')
-```
-
-
-## Getting JSON Schema
-
-`serpyco-rs` can generate JSON Schema for your dataclasses (Draft 2020-12).
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer
-
-@dataclass
-class A:
-    """Description of A"""
-    foo: int
-    bar: str
-
-ser = Serializer(A)
-
-print(ser.get_json_schema())
->> {
-    '$schema': 'https://json-schema.org/draft/2020-12/schema', 
-    '$ref': '#/components/schemas/A[no_format,keep_nones]', 
-    'components': {
-        'schemas': {
-            'A[no_format,keep_nones]': {
-                'properties': {
-                    'foo': {'type': 'integer'}, 
-                    'bar': {'type': 'string'}
-                }, 
-                'required': ['foo', 'bar'], 
-                'type': 'object', 
-                'description': 'Description of A'
-            }
-        }
-    }
-}
-```
-
-Also, you can configure the schema generation via `JsonSchemaBuilder`.
-
-
-```python
-from dataclasses import dataclass
-from serpyco_rs import Serializer, JsonSchemaBuilder
-
-@dataclass
-class A:
-    foo: int
-    bar: str
-
-ser = Serializer(A)
-
-builder = JsonSchemaBuilder(
-  add_dialect_uri=False,
-  ref_prefix='#/definitions',
-)
-
-print(builder.build(ser))
->> {'$ref': '#/definitions/__main__.A[no_format,keep_nones]'}
-
-print(builder.get_definitions())
->> {
-  "__main__.A[no_format,keep_nones]": {
-    "properties": {
-      "foo": {
-        "type": "integer"
-      },
-      "bar": {
-        "type": "string"
-      }
-    },
-    "required": [
-      "foo",
-      "bar"
-    ],
-    "type": "object"
-  }
-}
-```
-
-## Query string deserialization
-
-`serpyco-rs` can deserialize query string parameters (MultiDict like structures) with from string coercion.
-
-```python
-
-from dataclasses import dataclass
-from urllib.parse import parse_qsl
-
-from serpyco_rs import Serializer
-from multidict import MultiDict
-
-@dataclass
-class A:
-    foo: int
-    bar: str
-
-ser = Serializer(A)
-
-print(ser.load_query_params(MultiDict(parse_qsl('foo=1&bar=2'))))
->> A(foo=1, bar='2')
-```
```

### Comparing `serpyco_rs-1.7.1/bench/compare/github_issue/data.json` & `serpyco_rs-1.8.0/bench/compare/github_issue/data.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 12% similar despite different names*

```diff
@@ -1,531 +1,542 @@
-00000000: 7b0a 2020 2275 726c 223a 2022 6874 7470  {.  "url": "http
-00000010: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
-00000020: 6f6d 2f72 6570 6f73 2f6d 6963 726f 736f  om/repos/microso
-00000030: 6674 2f76 7363 6f64 652f 6973 7375 6573  ft/vscode/issues
-00000040: 2f31 3739 3038 3622 2c0a 2020 2272 6570  /179086",.  "rep
-00000050: 6f73 6974 6f72 795f 7572 6c22 3a20 2268  ository_url": "h
-00000060: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00000070: 622e 636f 6d2f 7265 706f 732f 6d69 6372  b.com/repos/micr
-00000080: 6f73 6f66 742f 7673 636f 6465 222c 0a20  osoft/vscode",. 
-00000090: 2022 6c61 6265 6c73 5f75 726c 223a 2022   "labels_url": "
-000000a0: 6874 7470 733a 2f2f 6170 692e 6769 7468  https://api.gith
-000000b0: 7562 2e63 6f6d 2f72 6570 6f73 2f6d 6963  ub.com/repos/mic
-000000c0: 726f 736f 6674 2f76 7363 6f64 652f 6973  rosoft/vscode/is
-000000d0: 7375 6573 2f31 3739 3038 362f 6c61 6265  sues/179086/labe
-000000e0: 6c73 7b2f 6e61 6d65 7d22 2c0a 2020 2263  ls{/name}",.  "c
-000000f0: 6f6d 6d65 6e74 735f 7572 6c22 3a20 2268  omments_url": "h
-00000100: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00000110: 622e 636f 6d2f 7265 706f 732f 6d69 6372  b.com/repos/micr
-00000120: 6f73 6f66 742f 7673 636f 6465 2f69 7373  osoft/vscode/iss
-00000130: 7565 732f 3137 3930 3836 2f63 6f6d 6d65  ues/179086/comme
-00000140: 6e74 7322 2c0a 2020 2265 7665 6e74 735f  nts",.  "events_
-00000150: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
-00000160: 7069 2e67 6974 6875 622e 636f 6d2f 7265  pi.github.com/re
-00000170: 706f 732f 6d69 6372 6f73 6f66 742f 7673  pos/microsoft/vs
-00000180: 636f 6465 2f69 7373 7565 732f 3137 3930  code/issues/1790
-00000190: 3836 2f65 7665 6e74 7322 2c0a 2020 2268  86/events",.  "h
-000001a0: 746d 6c5f 7572 6c22 3a20 2268 7474 7073  tml_url": "https
-000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d69  ://github.com/mi
-000001c0: 6372 6f73 6f66 742f 7673 636f 6465 2f69  crosoft/vscode/i
-000001d0: 7373 7565 732f 3137 3930 3836 222c 0a20  ssues/179086",. 
-000001e0: 2022 6964 223a 2031 3635 3332 3335 3531   "id": 165323551
-000001f0: 332c 0a20 2022 6e6f 6465 5f69 6422 3a20  3,.  "node_id": 
-00000200: 2249 5f6b 7744 4f41 6e38 524c 4d35 6969  "I_kwDOAn8RLM5ii
-00000210: 6c38 3522 2c0a 2020 226e 756d 6265 7222  l85",.  "number"
-00000220: 3a20 3137 3930 3836 2c0a 2020 2274 6974  : 179086,.  "tit
-00000230: 6c65 223a 2022 4754 4b2b 206d 6f64 756c  le": "GTK+ modul
-00000240: 6520 6c69 6263 616e 6265 7272 612d 6774  e libcanberra-gt
-00000250: 6b2d 6d6f 6475 6c65 2e73 6f20 6361 6e6e  k-module.so cann
-00000260: 6f74 2062 6520 6c6f 6164 6564 222c 0a20  ot be loaded",. 
-00000270: 2022 7573 6572 223a 207b 0a20 2020 2022   "user": {.    "
-00000280: 6c6f 6769 6e22 3a20 2250 6574 726f 7336  login": "Petros6
-00000290: 3236 222c 0a20 2020 2022 6964 223a 2036  26",.    "id": 6
-000002a0: 3233 3534 3732 312c 0a20 2020 2022 6e6f  2354721,.    "no
-000002b0: 6465 5f69 6422 3a20 224d 4451 3656 584e  de_id": "MDQ6VXN
-000002c0: 6c63 6a59 794d 7a55 304e 7a49 7822 2c0a  lcjYyMzU0NzIx",.
-000002d0: 2020 2020 2261 7661 7461 725f 7572 6c22      "avatar_url"
-000002e0: 3a20 2268 7474 7073 3a2f 2f61 7661 7461  : "https://avata
-000002f0: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
-00000300: 7465 6e74 2e63 6f6d 2f75 2f36 3233 3534  tent.com/u/62354
-00000310: 3732 313f 763d 3422 2c0a 2020 2020 2267  721?v=4",.    "g
-00000320: 7261 7661 7461 725f 6964 223a 2022 222c  ravatar_id": "",
-00000330: 0a20 2020 2022 7572 6c22 3a20 2268 7474  .    "url": "htt
-00000340: 7073 3a2f 2f61 7069 2e67 6974 6875 622e  ps://api.github.
-00000350: 636f 6d2f 7573 6572 732f 5065 7472 6f73  com/users/Petros
-00000360: 3632 3622 2c0a 2020 2020 2268 746d 6c5f  626",.    "html_
-00000370: 7572 6c22 3a20 2268 7474 7073 3a2f 2f67  url": "https://g
-00000380: 6974 6875 622e 636f 6d2f 5065 7472 6f73  ithub.com/Petros
-00000390: 3632 3622 2c0a 2020 2020 2266 6f6c 6c6f  626",.    "follo
-000003a0: 7765 7273 5f75 726c 223a 2022 6874 7470  wers_url": "http
-000003b0: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
-000003c0: 6f6d 2f75 7365 7273 2f50 6574 726f 7336  om/users/Petros6
-000003d0: 3236 2f66 6f6c 6c6f 7765 7273 222c 0a20  26/followers",. 
-000003e0: 2020 2022 666f 6c6c 6f77 696e 675f 7572     "following_ur
-000003f0: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
-00000400: 2e67 6974 6875 622e 636f 6d2f 7573 6572  .github.com/user
-00000410: 732f 5065 7472 6f73 3632 362f 666f 6c6c  s/Petros626/foll
-00000420: 6f77 696e 677b 2f6f 7468 6572 5f75 7365  owing{/other_use
-00000430: 727d 222c 0a20 2020 2022 6769 7374 735f  r}",.    "gists_
-00000440: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
-00000450: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
-00000460: 6572 732f 5065 7472 6f73 3632 362f 6769  ers/Petros626/gi
-00000470: 7374 737b 2f67 6973 745f 6964 7d22 2c0a  sts{/gist_id}",.
-00000480: 2020 2020 2273 7461 7272 6564 5f75 726c      "starred_url
-00000490: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
-000004a0: 6769 7468 7562 2e63 6f6d 2f75 7365 7273  github.com/users
-000004b0: 2f50 6574 726f 7336 3236 2f73 7461 7272  /Petros626/starr
-000004c0: 6564 7b2f 6f77 6e65 727d 7b2f 7265 706f  ed{/owner}{/repo
-000004d0: 7d22 2c0a 2020 2020 2273 7562 7363 7269  }",.    "subscri
-000004e0: 7074 696f 6e73 5f75 726c 223a 2022 6874  ptions_url": "ht
-000004f0: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
-00000500: 2e63 6f6d 2f75 7365 7273 2f50 6574 726f  .com/users/Petro
-00000510: 7336 3236 2f73 7562 7363 7269 7074 696f  s626/subscriptio
-00000520: 6e73 222c 0a20 2020 2022 6f72 6761 6e69  ns",.    "organi
-00000530: 7a61 7469 6f6e 735f 7572 6c22 3a20 2268  zations_url": "h
-00000540: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00000550: 622e 636f 6d2f 7573 6572 732f 5065 7472  b.com/users/Petr
-00000560: 6f73 3632 362f 6f72 6773 222c 0a20 2020  os626/orgs",.   
-00000570: 2022 7265 706f 735f 7572 6c22 3a20 2268   "repos_url": "h
-00000580: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00000590: 622e 636f 6d2f 7573 6572 732f 5065 7472  b.com/users/Petr
-000005a0: 6f73 3632 362f 7265 706f 7322 2c0a 2020  os626/repos",.  
-000005b0: 2020 2265 7665 6e74 735f 7572 6c22 3a20    "events_url": 
-000005c0: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-000005d0: 6875 622e 636f 6d2f 7573 6572 732f 5065  hub.com/users/Pe
-000005e0: 7472 6f73 3632 362f 6576 656e 7473 7b2f  tros626/events{/
-000005f0: 7072 6976 6163 797d 222c 0a20 2020 2022  privacy}",.    "
-00000600: 7265 6365 6976 6564 5f65 7665 6e74 735f  received_events_
-00000610: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
-00000620: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
-00000630: 6572 732f 5065 7472 6f73 3632 362f 7265  ers/Petros626/re
-00000640: 6365 6976 6564 5f65 7665 6e74 7322 2c0a  ceived_events",.
-00000650: 2020 2020 2274 7970 6522 3a20 2255 7365      "type": "Use
-00000660: 7222 2c0a 2020 2020 2273 6974 655f 6164  r",.    "site_ad
-00000670: 6d69 6e22 3a20 6661 6c73 650a 2020 7d2c  min": false.  },
-00000680: 0a20 2022 6c61 6265 6c73 223a 205b 0a20  .  "labels": [. 
-00000690: 2020 207b 0a20 2020 2020 2022 6964 223a     {.      "id":
-000006a0: 2032 3536 3132 3939 3933 2c0a 2020 2020   256129993,.    
-000006b0: 2020 226e 6f64 655f 6964 223a 2022 4d44    "node_id": "MD
-000006c0: 5536 5447 4669 5a57 7779 4e54 5978 4d6a  U6TGFiZWwyNTYxMj
-000006d0: 6b35 4f54 4d3d 222c 0a20 2020 2020 2022  k5OTM=",.      "
-000006e0: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
-000006f0: 7069 2e67 6974 6875 622e 636f 6d2f 7265  pi.github.com/re
-00000700: 706f 732f 6d69 6372 6f73 6f66 742f 7673  pos/microsoft/vs
-00000710: 636f 6465 2f6c 6162 656c 732f 6275 6722  code/labels/bug"
-00000720: 2c0a 2020 2020 2020 226e 616d 6522 3a20  ,.      "name": 
-00000730: 2262 7567 222c 0a20 2020 2020 2022 636f  "bug",.      "co
-00000740: 6c6f 7222 3a20 2238 4436 3637 3322 2c0a  lor": "8D6673",.
-00000750: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
-00000760: 2074 7275 652c 0a20 2020 2020 2022 6465   true,.      "de
-00000770: 7363 7269 7074 696f 6e22 3a20 2249 7373  scription": "Iss
-00000780: 7565 2069 6465 6e74 6966 6965 6420 6279  ue identified by
-00000790: 2056 5320 436f 6465 2054 6561 6d20 6d65   VS Code Team me
-000007a0: 6d62 6572 2061 7320 7072 6f62 6162 6c65  mber as probable
-000007b0: 2062 7567 220a 2020 2020 7d2c 0a20 2020   bug".    },.   
-000007c0: 207b 0a20 2020 2020 2022 6964 223a 2033   {.      "id": 3
-000007d0: 3030 3333 3437 3836 2c0a 2020 2020 2020  00334786,.      
-000007e0: 226e 6f64 655f 6964 223a 2022 4d44 5536  "node_id": "MDU6
-000007f0: 5447 4669 5a57 777a 4d44 417a 4d7a 5133  TGFiZWwzMDAzMzQ3
-00000800: 4f44 593d 222c 0a20 2020 2020 2022 7572  ODY=",.      "ur
-00000810: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
-00000820: 2e67 6974 6875 622e 636f 6d2f 7265 706f  .github.com/repo
-00000830: 732f 6d69 6372 6f73 6f66 742f 7673 636f  s/microsoft/vsco
-00000840: 6465 2f6c 6162 656c 732f 7665 7269 6669  de/labels/verifi
-00000850: 6361 7469 6f6e 2d66 6f75 6e64 222c 0a20  cation-found",. 
-00000860: 2020 2020 2022 6e61 6d65 223a 2022 7665       "name": "ve
-00000870: 7269 6669 6361 7469 6f6e 2d66 6f75 6e64  rification-found
-00000880: 222c 0a20 2020 2020 2022 636f 6c6f 7222  ",.      "color"
-00000890: 3a20 2266 3763 3663 3722 2c0a 2020 2020  : "f7c6c7",.    
-000008a0: 2020 2264 6566 6175 6c74 223a 2066 616c    "default": fal
-000008b0: 7365 2c0a 2020 2020 2020 2264 6573 6372  se,.      "descr
-000008c0: 6970 7469 6f6e 223a 2022 4973 7375 6520  iption": "Issue 
-000008d0: 7665 7269 6669 6361 7469 6f6e 2066 6169  verification fai
-000008e0: 6c65 6422 0a20 2020 207d 2c0a 2020 2020  led".    },.    
-000008f0: 7b0a 2020 2020 2020 2269 6422 3a20 3332  {.      "id": 32
-00000900: 3130 3932 3531 302c 0a20 2020 2020 2022  1092510,.      "
-00000910: 6e6f 6465 5f69 6422 3a20 224d 4455 3654  node_id": "MDU6T
-00000920: 4746 695a 5777 7a4d 6a45 774f 5449 314d  GFiZWwzMjEwOTI1M
-00000930: 5441 3d22 2c0a 2020 2020 2020 2275 726c  TA=",.      "url
-00000940: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
-00000950: 6769 7468 7562 2e63 6f6d 2f72 6570 6f73  github.com/repos
-00000960: 2f6d 6963 726f 736f 6674 2f76 7363 6f64  /microsoft/vscod
-00000970: 652f 6c61 6265 6c73 2f6c 696e 7578 222c  e/labels/linux",
-00000980: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
-00000990: 6c69 6e75 7822 2c0a 2020 2020 2020 2263  linux",.      "c
-000009a0: 6f6c 6f72 223a 2022 3030 3662 3735 222c  olor": "006b75",
-000009b0: 0a20 2020 2020 2022 6465 6661 756c 7422  .      "default"
-000009c0: 3a20 6661 6c73 652c 0a20 2020 2020 2022  : false,.      "
-000009d0: 6465 7363 7269 7074 696f 6e22 3a20 2249  description": "I
-000009e0: 7373 7565 7320 7769 7468 2056 5320 436f  ssues with VS Co
-000009f0: 6465 206f 6e20 4c69 6e75 7822 0a20 2020  de on Linux".   
-00000a00: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00000a10: 2269 6422 3a20 3336 3236 3934 3633 322c  "id": 362694632,
-00000a20: 0a20 2020 2020 2022 6e6f 6465 5f69 6422  .      "node_id"
-00000a30: 3a20 224d 4455 3654 4746 695a 5777 7a4e  : "MDU6TGFiZWwzN
-00000a40: 6a49 324f 5451 324d 7a49 3d22 2c0a 2020  jI2OTQ2MzI=",.  
-00000a50: 2020 2020 2275 726c 223a 2022 6874 7470      "url": "http
-00000a60: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
-00000a70: 6f6d 2f72 6570 6f73 2f6d 6963 726f 736f  om/repos/microso
-00000a80: 6674 2f76 7363 6f64 652f 6c61 6265 6c73  ft/vscode/labels
-00000a90: 2f74 6572 6d69 6e61 6c22 2c0a 2020 2020  /terminal",.    
-00000aa0: 2020 226e 616d 6522 3a20 2274 6572 6d69    "name": "termi
-00000ab0: 6e61 6c22 2c0a 2020 2020 2020 2263 6f6c  nal",.      "col
-00000ac0: 6f72 223a 2022 6335 6465 6635 222c 0a20  or": "c5def5",. 
-00000ad0: 2020 2020 2022 6465 6661 756c 7422 3a20       "default": 
-00000ae0: 6661 6c73 652c 0a20 2020 2020 2022 6465  false,.      "de
-00000af0: 7363 7269 7074 696f 6e22 3a20 2249 6e74  scription": "Int
-00000b00: 6567 7261 7465 6420 7465 726d 696e 616c  egrated terminal
-00000b10: 2069 7373 7565 7322 0a20 2020 207d 2c0a   issues".    },.
-00000b20: 2020 2020 7b0a 2020 2020 2020 2269 6422      {.      "id"
-00000b30: 3a20 3130 3334 3434 3539 3438 2c0a 2020  : 1034445948,.  
-00000b40: 2020 2020 226e 6f64 655f 6964 223a 2022      "node_id": "
-00000b50: 4d44 5536 5447 4669 5a57 7778 4d44 4d30  MDU6TGFiZWwxMDM0
-00000b60: 4e44 5131 4f54 5134 222c 0a20 2020 2020  NDQ1OTQ4",.     
-00000b70: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
-00000b80: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
-00000b90: 7265 706f 732f 6d69 6372 6f73 6f66 742f  repos/microsoft/
-00000ba0: 7673 636f 6465 2f6c 6162 656c 732f 736e  vscode/labels/sn
-00000bb0: 6170 222c 0a20 2020 2020 2022 6e61 6d65  ap",.      "name
-00000bc0: 223a 2022 736e 6170 222c 0a20 2020 2020  ": "snap",.     
-00000bd0: 2022 636f 6c6f 7222 3a20 2263 3564 6566   "color": "c5def
-00000be0: 3522 2c0a 2020 2020 2020 2264 6566 6175  5",.      "defau
-00000bf0: 6c74 223a 2066 616c 7365 2c0a 2020 2020  lt": false,.    
-00000c00: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00000c10: 2022 4973 7375 6573 2072 656c 6174 6564   "Issues related
-00000c20: 2074 6f20 7468 6520 736e 6170 2070 6163   to the snap pac
-00000c30: 6b61 6765 220a 2020 2020 7d2c 0a20 2020  kage".    },.   
-00000c40: 207b 0a20 2020 2020 2022 6964 223a 2031   {.      "id": 1
-00000c50: 3131 3937 3934 3437 342c 0a20 2020 2020  119794474,.     
-00000c60: 2022 6e6f 6465 5f69 6422 3a20 224d 4455   "node_id": "MDU
-00000c70: 3654 4746 695a 5777 784d 5445 354e 7a6b  6TGFiZWwxMTE5Nzk
-00000c80: 304e 4463 3022 2c0a 2020 2020 2020 2275  0NDc0",.      "u
-00000c90: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
-00000ca0: 692e 6769 7468 7562 2e63 6f6d 2f72 6570  i.github.com/rep
-00000cb0: 6f73 2f6d 6963 726f 736f 6674 2f76 7363  os/microsoft/vsc
-00000cc0: 6f64 652f 6c61 6265 6c73 2f63 6f6e 6669  ode/labels/confi
-00000cd0: 726d 6564 222c 0a20 2020 2020 2022 6e61  rmed",.      "na
-00000ce0: 6d65 223a 2022 636f 6e66 6972 6d65 6422  me": "confirmed"
-00000cf0: 2c0a 2020 2020 2020 2263 6f6c 6f72 223a  ,.      "color":
-00000d00: 2022 3030 3938 3030 222c 0a20 2020 2020   "009800",.     
-00000d10: 2022 6465 6661 756c 7422 3a20 6661 6c73   "default": fals
-00000d20: 652c 0a20 2020 2020 2022 6465 7363 7269  e,.      "descri
-00000d30: 7074 696f 6e22 3a20 2249 7373 7565 2068  ption": "Issue h
-00000d40: 6173 2062 6565 6e20 636f 6e66 6972 6d65  as been confirme
-00000d50: 6420 6279 2056 5320 436f 6465 2054 6561  d by VS Code Tea
-00000d60: 6d20 6d65 6d62 6572 220a 2020 2020 7d0a  m member".    }.
-00000d70: 2020 5d2c 0a20 2022 7374 6174 6522 3a20    ],.  "state": 
-00000d80: 226f 7065 6e22 2c0a 2020 226c 6f63 6b65  "open",.  "locke
-00000d90: 6422 3a20 6661 6c73 652c 0a20 2022 6173  d": false,.  "as
-00000da0: 7369 676e 6565 223a 207b 0a20 2020 2022  signee": {.    "
-00000db0: 6c6f 6769 6e22 3a20 2264 6565 7061 6b31  login": "deepak1
-00000dc0: 3535 3622 2c0a 2020 2020 2269 6422 3a20  556",.    "id": 
-00000dd0: 3936 3433 3836 2c0a 2020 2020 226e 6f64  964386,.    "nod
-00000de0: 655f 6964 223a 2022 4d44 5136 5658 4e6c  e_id": "MDQ6VXNl
-00000df0: 636a 6b32 4e44 4d34 4e67 3d3d 222c 0a20  cjk2NDM4Ng==",. 
-00000e00: 2020 2022 6176 6174 6172 5f75 726c 223a     "avatar_url":
-00000e10: 2022 6874 7470 733a 2f2f 6176 6174 6172   "https://avatar
-00000e20: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
-00000e30: 656e 742e 636f 6d2f 752f 3936 3433 3836  ent.com/u/964386
-00000e40: 3f76 3d34 222c 0a20 2020 2022 6772 6176  ?v=4",.    "grav
-00000e50: 6174 6172 5f69 6422 3a20 2222 2c0a 2020  atar_id": "",.  
-00000e60: 2020 2275 726c 223a 2022 6874 7470 733a    "url": "https:
-00000e70: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
-00000e80: 2f75 7365 7273 2f64 6565 7061 6b31 3535  /users/deepak155
-00000e90: 3622 2c0a 2020 2020 2268 746d 6c5f 7572  6",.    "html_ur
-00000ea0: 6c22 3a20 2268 7474 7073 3a2f 2f67 6974  l": "https://git
-00000eb0: 6875 622e 636f 6d2f 6465 6570 616b 3135  hub.com/deepak15
-00000ec0: 3536 222c 0a20 2020 2022 666f 6c6c 6f77  56",.    "follow
-00000ed0: 6572 735f 7572 6c22 3a20 2268 7474 7073  ers_url": "https
-00000ee0: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
-00000ef0: 6d2f 7573 6572 732f 6465 6570 616b 3135  m/users/deepak15
-00000f00: 3536 2f66 6f6c 6c6f 7765 7273 222c 0a20  56/followers",. 
-00000f10: 2020 2022 666f 6c6c 6f77 696e 675f 7572     "following_ur
-00000f20: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
-00000f30: 2e67 6974 6875 622e 636f 6d2f 7573 6572  .github.com/user
-00000f40: 732f 6465 6570 616b 3135 3536 2f66 6f6c  s/deepak1556/fol
-00000f50: 6c6f 7769 6e67 7b2f 6f74 6865 725f 7573  lowing{/other_us
-00000f60: 6572 7d22 2c0a 2020 2020 2267 6973 7473  er}",.    "gists
-00000f70: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
-00000f80: 6170 692e 6769 7468 7562 2e63 6f6d 2f75  api.github.com/u
-00000f90: 7365 7273 2f64 6565 7061 6b31 3535 362f  sers/deepak1556/
-00000fa0: 6769 7374 737b 2f67 6973 745f 6964 7d22  gists{/gist_id}"
-00000fb0: 2c0a 2020 2020 2273 7461 7272 6564 5f75  ,.    "starred_u
-00000fc0: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
-00000fd0: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
-00000fe0: 7273 2f64 6565 7061 6b31 3535 362f 7374  rs/deepak1556/st
-00000ff0: 6172 7265 647b 2f6f 776e 6572 7d7b 2f72  arred{/owner}{/r
-00001000: 6570 6f7d 222c 0a20 2020 2022 7375 6273  epo}",.    "subs
-00001010: 6372 6970 7469 6f6e 735f 7572 6c22 3a20  criptions_url": 
-00001020: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-00001030: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
-00001040: 6570 616b 3135 3536 2f73 7562 7363 7269  epak1556/subscri
-00001050: 7074 696f 6e73 222c 0a20 2020 2022 6f72  ptions",.    "or
-00001060: 6761 6e69 7a61 7469 6f6e 735f 7572 6c22  ganizations_url"
-00001070: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
-00001080: 6974 6875 622e 636f 6d2f 7573 6572 732f  ithub.com/users/
-00001090: 6465 6570 616b 3135 3536 2f6f 7267 7322  deepak1556/orgs"
-000010a0: 2c0a 2020 2020 2272 6570 6f73 5f75 726c  ,.    "repos_url
-000010b0: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
-000010c0: 6769 7468 7562 2e63 6f6d 2f75 7365 7273  github.com/users
-000010d0: 2f64 6565 7061 6b31 3535 362f 7265 706f  /deepak1556/repo
-000010e0: 7322 2c0a 2020 2020 2265 7665 6e74 735f  s",.    "events_
-000010f0: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
-00001100: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
-00001110: 6572 732f 6465 6570 616b 3135 3536 2f65  ers/deepak1556/e
-00001120: 7665 6e74 737b 2f70 7269 7661 6379 7d22  vents{/privacy}"
-00001130: 2c0a 2020 2020 2272 6563 6569 7665 645f  ,.    "received_
-00001140: 6576 656e 7473 5f75 726c 223a 2022 6874  events_url": "ht
-00001150: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
-00001160: 2e63 6f6d 2f75 7365 7273 2f64 6565 7061  .com/users/deepa
-00001170: 6b31 3535 362f 7265 6365 6976 6564 5f65  k1556/received_e
-00001180: 7665 6e74 7322 2c0a 2020 2020 2274 7970  vents",.    "typ
-00001190: 6522 3a20 2255 7365 7222 2c0a 2020 2020  e": "User",.    
-000011a0: 2273 6974 655f 6164 6d69 6e22 3a20 6661  "site_admin": fa
-000011b0: 6c73 650a 2020 7d2c 0a20 2022 6173 7369  lse.  },.  "assi
-000011c0: 676e 6565 7322 3a20 5b0a 2020 2020 7b0a  gnees": [.    {.
-000011d0: 2020 2020 2020 226c 6f67 696e 223a 2022        "login": "
-000011e0: 6465 6570 616b 3135 3536 222c 0a20 2020  deepak1556",.   
-000011f0: 2020 2022 6964 223a 2039 3634 3338 362c     "id": 964386,
-00001200: 0a20 2020 2020 2022 6e6f 6465 5f69 6422  .      "node_id"
-00001210: 3a20 224d 4451 3656 584e 6c63 6a6b 324e  : "MDQ6VXNlcjk2N
-00001220: 444d 344e 673d 3d22 2c0a 2020 2020 2020  DM4Ng==",.      
-00001230: 2261 7661 7461 725f 7572 6c22 3a20 2268  "avatar_url": "h
-00001240: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
-00001250: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001260: 2e63 6f6d 2f75 2f39 3634 3338 363f 763d  .com/u/964386?v=
-00001270: 3422 2c0a 2020 2020 2020 2267 7261 7661  4",.      "grava
-00001280: 7461 725f 6964 223a 2022 222c 0a20 2020  tar_id": "",.   
-00001290: 2020 2022 7572 6c22 3a20 2268 7474 7073     "url": "https
-000012a0: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
-000012b0: 6d2f 7573 6572 732f 6465 6570 616b 3135  m/users/deepak15
-000012c0: 3536 222c 0a20 2020 2020 2022 6874 6d6c  56",.      "html
-000012d0: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
-000012e0: 6769 7468 7562 2e63 6f6d 2f64 6565 7061  github.com/deepa
-000012f0: 6b31 3535 3622 2c0a 2020 2020 2020 2266  k1556",.      "f
-00001300: 6f6c 6c6f 7765 7273 5f75 726c 223a 2022  ollowers_url": "
-00001310: 6874 7470 733a 2f2f 6170 692e 6769 7468  https://api.gith
-00001320: 7562 2e63 6f6d 2f75 7365 7273 2f64 6565  ub.com/users/dee
-00001330: 7061 6b31 3535 362f 666f 6c6c 6f77 6572  pak1556/follower
-00001340: 7322 2c0a 2020 2020 2020 2266 6f6c 6c6f  s",.      "follo
-00001350: 7769 6e67 5f75 726c 223a 2022 6874 7470  wing_url": "http
-00001360: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
-00001370: 6f6d 2f75 7365 7273 2f64 6565 7061 6b31  om/users/deepak1
-00001380: 3535 362f 666f 6c6c 6f77 696e 677b 2f6f  556/following{/o
-00001390: 7468 6572 5f75 7365 727d 222c 0a20 2020  ther_user}",.   
-000013a0: 2020 2022 6769 7374 735f 7572 6c22 3a20     "gists_url": 
-000013b0: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-000013c0: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
-000013d0: 6570 616b 3135 3536 2f67 6973 7473 7b2f  epak1556/gists{/
-000013e0: 6769 7374 5f69 647d 222c 0a20 2020 2020  gist_id}",.     
-000013f0: 2022 7374 6172 7265 645f 7572 6c22 3a20   "starred_url": 
-00001400: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-00001410: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
-00001420: 6570 616b 3135 3536 2f73 7461 7272 6564  epak1556/starred
-00001430: 7b2f 6f77 6e65 727d 7b2f 7265 706f 7d22  {/owner}{/repo}"
-00001440: 2c0a 2020 2020 2020 2273 7562 7363 7269  ,.      "subscri
-00001450: 7074 696f 6e73 5f75 726c 223a 2022 6874  ptions_url": "ht
-00001460: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
-00001470: 2e63 6f6d 2f75 7365 7273 2f64 6565 7061  .com/users/deepa
-00001480: 6b31 3535 362f 7375 6273 6372 6970 7469  k1556/subscripti
-00001490: 6f6e 7322 2c0a 2020 2020 2020 226f 7267  ons",.      "org
-000014a0: 616e 697a 6174 696f 6e73 5f75 726c 223a  anizations_url":
-000014b0: 2022 6874 7470 733a 2f2f 6170 692e 6769   "https://api.gi
-000014c0: 7468 7562 2e63 6f6d 2f75 7365 7273 2f64  thub.com/users/d
-000014d0: 6565 7061 6b31 3535 362f 6f72 6773 222c  eepak1556/orgs",
-000014e0: 0a20 2020 2020 2022 7265 706f 735f 7572  .      "repos_ur
-000014f0: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
-00001500: 2e67 6974 6875 622e 636f 6d2f 7573 6572  .github.com/user
-00001510: 732f 6465 6570 616b 3135 3536 2f72 6570  s/deepak1556/rep
-00001520: 6f73 222c 0a20 2020 2020 2022 6576 656e  os",.      "even
-00001530: 7473 5f75 726c 223a 2022 6874 7470 733a  ts_url": "https:
-00001540: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
-00001550: 2f75 7365 7273 2f64 6565 7061 6b31 3535  /users/deepak155
-00001560: 362f 6576 656e 7473 7b2f 7072 6976 6163  6/events{/privac
-00001570: 797d 222c 0a20 2020 2020 2022 7265 6365  y}",.      "rece
-00001580: 6976 6564 5f65 7665 6e74 735f 7572 6c22  ived_events_url"
-00001590: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
-000015a0: 6974 6875 622e 636f 6d2f 7573 6572 732f  ithub.com/users/
-000015b0: 6465 6570 616b 3135 3536 2f72 6563 6569  deepak1556/recei
-000015c0: 7665 645f 6576 656e 7473 222c 0a20 2020  ved_events",.   
-000015d0: 2020 2022 7479 7065 223a 2022 5573 6572     "type": "User
-000015e0: 222c 0a20 2020 2020 2022 7369 7465 5f61  ",.      "site_a
-000015f0: 646d 696e 223a 2066 616c 7365 0a20 2020  dmin": false.   
-00001600: 207d 0a20 205d 2c0a 2020 226d 696c 6573   }.  ],.  "miles
-00001610: 746f 6e65 223a 206e 756c 6c2c 0a20 2022  tone": null,.  "
-00001620: 636f 6d6d 656e 7473 223a 2031 352c 0a20  comments": 15,. 
-00001630: 2022 6372 6561 7465 645f 6174 223a 2022   "created_at": "
-00001640: 3230 3233 2d30 342d 3034 5430 353a 3536  2023-04-04T05:56
-00001650: 3a34 375a 222c 0a20 2022 7570 6461 7465  :47Z",.  "update
-00001660: 645f 6174 223a 2022 3230 3233 2d30 372d  d_at": "2023-07-
-00001670: 3235 5431 333a 3338 3a35 305a 222c 0a20  25T13:38:50Z",. 
-00001680: 2022 636c 6f73 6564 5f61 7422 3a20 6e75   "closed_at": nu
-00001690: 6c6c 2c0a 2020 2261 7574 686f 725f 6173  ll,.  "author_as
-000016a0: 736f 6369 6174 696f 6e22 3a20 224e 4f4e  sociation": "NON
-000016b0: 4522 2c0a 2020 2261 6374 6976 655f 6c6f  E",.  "active_lo
-000016c0: 636b 5f72 6561 736f 6e22 3a20 6e75 6c6c  ck_reason": null
-000016d0: 2c0a 2020 2262 6f64 7922 3a20 2248 656c  ,.  "body": "Hel
-000016e0: 6c6f 2067 7579 732c 5c72 5c6e 5c72 5c6e  lo guys,\r\n\r\n
-000016f0: 4927 6d20 7573 696e 6720 5f4f 7065 6e43  I'm using _OpenC
-00001700: 565f 2069 6e20 5653 436f 6465 2028 5562  V_ in VSCode (Ub
-00001710: 756e 7475 2053 6f66 7477 6172 6520 696e  untu Software in
-00001720: 7374 616c 6c61 7469 6f6e 2920 616e 6420  stallation) and 
-00001730: 6576 6572 7974 6869 6e67 2077 6f72 6b65  everything worke
-00001740: 6420 6669 6e65 2c20 756e 7469 6c20 4920  d fine, until I 
-00001750: 7570 6461 7465 6420 6d79 206c 6962 7261  updated my libra
-00001760: 7269 6573 2028 6073 7564 6f20 6170 742d  ries (`sudo apt-
-00001770: 6765 7420 7570 6461 7465 2f75 7067 7261  get update/upgra
-00001780: 6465 2f66 756c 6c2d 7570 6772 6164 6560  de/full-upgrade`
-00001790: 2920 4920 6775 6573 732e 2042 7574 206e  ) I guess. But n
-000017a0: 6f77 2056 5343 6f64 6520 6f72 2072 6174  ow VSCode or rat
-000017b0: 6865 7220 5f4f 7065 6e43 565f 2063 616e  her _OpenCV_ can
-000017c0: 2774 2066 696e 6420 7468 6520 5f47 544b  't find the _GTK
-000017d0: 5f20 6c69 6272 6172 792e 205c 725c 6e5c  _ library. \r\n\
-000017e0: 725c 6e49 2776 6520 7465 7374 6564 2074  r\nI've tested t
-000017f0: 6869 7320 7375 6363 6573 6675 6c6c 793a  his succesfully:
-00001800: 5c72 5c6e 2060 4754 4b5f 5041 5448 3d2f  \r\n `GTK_PATH=/
-00001810: 7573 722f 6c69 622f 7838 365f 3634 2d6c  usr/lib/x86_64-l
-00001820: 696e 7578 2d67 6e75 2f67 746b 2d32 2e30  inux-gnu/gtk-2.0
-00001830: 202e 2f74 6573 7460 202d 2d3e 2077 6f72   ./test` --> wor
-00001840: 6b73 5c72 5c6e 5c72 5c6e 4275 7420 7768  ks\r\n\r\nBut wh
-00001850: 656e 2049 2073 7065 6369 6679 2074 6865  en I specify the
-00001860: 2076 6572 7369 6f6e 2067 746b 2d33 2e30   version gtk-3.0
-00001870: 3a5c 725c 6e60 4754 4b5f 5041 5448 3d2f  :\r\n`GTK_PATH=/
-00001880: 7573 722f 6c69 622f 7838 365f 3634 2d6c  usr/lib/x86_64-l
-00001890: 696e 7578 2d67 6e75 2f67 746b 2d33 2e30  inux-gnu/gtk-3.0
-000018a0: 202e 2f74 6573 7460 202d 2d3e 2066 6169   ./test` --> fai
-000018b0: 6c73 5c72 5c6e 5c72 5c6e 204e 6f72 6d61  ls\r\n\r\n Norma
-000018c0: 6c6c 7920 7468 6520 6c6f 6164 6564 2076  lly the loaded v
-000018d0: 6572 7369 6f6e 2077 6974 686f 7574 2075  ersion without u
-000018e0: 7369 6e67 2047 544b 5f50 4154 4820 6973  sing GTK_PATH is
-000018f0: 2067 746b 2d33 2e30 2061 6e64 2074 6865   gtk-3.0 and the
-00001900: 6e20 6974 2073 686f 7773 206d 6520 7468  n it shows me th
-00001910: 6973 2065 7272 6f72 3a5c 725c 6e21 5b69  is error:\r\n![i
-00001920: 6d61 6765 5d28 6874 7470 733a 2f2f 7573  mage](https://us
-00001930: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00001940: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001950: 3632 3335 3437 3231 2f32 3239 3433 3530  62354721/2294350
-00001960: 3739 2d61 3835 6335 6666 312d 6138 6333  79-a85c5ff1-a8c3
-00001970: 2d34 3837 302d 3933 3430 2d62 6463 3934  -4870-9340-bdc94
-00001980: 3034 6535 3935 622e 706e 6729 5c72 5c6e  04e595b.png)\r\n
-00001990: 5c72 5c6e 5c72 5c6e 4920 7665 7269 6669  \r\n\r\nI verifi
-000019a0: 6564 2074 6861 7420 7468 6520 696e 2060  ed that the in `
-000019b0: 2f75 7372 2f6c 6962 2f78 3836 5f36 342d  /usr/lib/x86_64-
-000019c0: 6c69 6e75 782d 676e 752f 6774 6b2d 332e  linux-gnu/gtk-3.
-000019d0: 302f 6d6f 6475 6c65 7360 2069 733a 5c72  0/modules` is:\r
-000019e0: 5c6e 5c72 5c6e 215b 696d 6167 655d 2868  \n\r\n![image](h
-000019f0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-00001a00: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-00001a10: 7465 6e74 2e63 6f6d 2f36 3233 3534 3732  tent.com/6235472
-00001a20: 312f 3232 3930 3539 3138 382d 3431 3731  1/229059188-4171
-00001a30: 6637 3330 2d64 3264 392d 3462 3663 2d62  f730-d2d9-4b6c-b
-00001a40: 3130 332d 3434 3763 6138 6565 3732 3762  103-447ca8ee727b
-00001a50: 2e70 6e67 295c 725c 6e5c 725c 6e57 6f75  .png)\r\n\r\nWou
-00001a60: 6c64 2061 7070 7265 6369 6174 6520 746f  ld appreciate to
-00001a70: 2073 6f6c 7665 2074 6869 7320 7761 726e   solve this warn
-00001a80: 696e 6720 616e 6420 746f 2075 6e64 6572  ing and to under
-00001a90: 7374 616e 6420 7768 7920 7468 6520 2e73  stand why the .s
-00001aa0: 6f20 6361 6e6e 6f74 2062 6520 6c6f 6164  o cannot be load
-00001ab0: 6564 2e5c 725c 6e5c 725c 6e54 6861 6e6b  ed.\r\n\r\nThank
-00001ac0: 7320 696e 2061 6476 616e 6365 5c72 5c6e  s in advance\r\n
-00001ad0: 5c72 5c6e 5c72 5c6e 2a2a 5550 4441 5445  \r\n\r\n**UPDATE
-00001ae0: 3a2a 2a20 7468 6520 6578 616d 706c 6520  :** the example 
-00001af0: 636f 6465 2063 616e 2062 6520 6578 6563  code can be exec
-00001b00: 7574 6564 2077 6974 686f 7574 2077 6172  uted without war
-00001b10: 6e69 6e67 7320 696e 2074 6865 206e 6f72  nings in the nor
-00001b20: 6d61 6c20 676e 6f6d 6520 7465 726d 696e  mal gnome termin
-00001b30: 616c 2c20 6275 7420 5653 436f 6465 2073  al, but VSCode s
-00001b40: 6565 6d73 2074 6f20 6861 6265 2070 726f  eems to habe pro
-00001b50: 626c 656d 7320 746f 2066 696e 6420 7468  blems to find th
-00001b60: 6520 7370 6563 6966 6963 206c 6962 7261  e specific libra
-00001b70: 7269 6573 2c20 736f 2069 7427 7320 6465  ries, so it's de
-00001b80: 6669 6e69 7465 6c79 205f 5653 436f 6465  finitely _VSCode
-00001b90: 5f2e 222c 0a20 2022 636c 6f73 6564 5f62  _.",.  "closed_b
-00001ba0: 7922 3a20 7b0a 2020 2020 226c 6f67 696e  y": {.    "login
-00001bb0: 223a 2022 6465 6570 616b 3135 3536 222c  ": "deepak1556",
-00001bc0: 0a20 2020 2022 6964 223a 2039 3634 3338  .    "id": 96438
-00001bd0: 362c 0a20 2020 2022 6e6f 6465 5f69 6422  6,.    "node_id"
-00001be0: 3a20 224d 4451 3656 584e 6c63 6a6b 324e  : "MDQ6VXNlcjk2N
-00001bf0: 444d 344e 673d 3d22 2c0a 2020 2020 2261  DM4Ng==",.    "a
-00001c00: 7661 7461 725f 7572 6c22 3a20 2268 7474  vatar_url": "htt
-00001c10: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
-00001c20: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001c30: 6f6d 2f75 2f39 3634 3338 363f 763d 3422  om/u/964386?v=4"
-00001c40: 2c0a 2020 2020 2267 7261 7661 7461 725f  ,.    "gravatar_
-00001c50: 6964 223a 2022 222c 0a20 2020 2022 7572  id": "",.    "ur
-00001c60: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
-00001c70: 2e67 6974 6875 622e 636f 6d2f 7573 6572  .github.com/user
-00001c80: 732f 6465 6570 616b 3135 3536 222c 0a20  s/deepak1556",. 
-00001c90: 2020 2022 6874 6d6c 5f75 726c 223a 2022     "html_url": "
-00001ca0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001cb0: 6f6d 2f64 6565 7061 6b31 3535 3622 2c0a  om/deepak1556",.
-00001cc0: 2020 2020 2266 6f6c 6c6f 7765 7273 5f75      "followers_u
-00001cd0: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
-00001ce0: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
-00001cf0: 7273 2f64 6565 7061 6b31 3535 362f 666f  rs/deepak1556/fo
-00001d00: 6c6c 6f77 6572 7322 2c0a 2020 2020 2266  llowers",.    "f
-00001d10: 6f6c 6c6f 7769 6e67 5f75 726c 223a 2022  ollowing_url": "
-00001d20: 6874 7470 733a 2f2f 6170 692e 6769 7468  https://api.gith
-00001d30: 7562 2e63 6f6d 2f75 7365 7273 2f64 6565  ub.com/users/dee
-00001d40: 7061 6b31 3535 362f 666f 6c6c 6f77 696e  pak1556/followin
-00001d50: 677b 2f6f 7468 6572 5f75 7365 727d 222c  g{/other_user}",
-00001d60: 0a20 2020 2022 6769 7374 735f 7572 6c22  .    "gists_url"
-00001d70: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
-00001d80: 6974 6875 622e 636f 6d2f 7573 6572 732f  ithub.com/users/
-00001d90: 6465 6570 616b 3135 3536 2f67 6973 7473  deepak1556/gists
-00001da0: 7b2f 6769 7374 5f69 647d 222c 0a20 2020  {/gist_id}",.   
-00001db0: 2022 7374 6172 7265 645f 7572 6c22 3a20   "starred_url": 
-00001dc0: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-00001dd0: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
-00001de0: 6570 616b 3135 3536 2f73 7461 7272 6564  epak1556/starred
-00001df0: 7b2f 6f77 6e65 727d 7b2f 7265 706f 7d22  {/owner}{/repo}"
-00001e00: 2c0a 2020 2020 2273 7562 7363 7269 7074  ,.    "subscript
-00001e10: 696f 6e73 5f75 726c 223a 2022 6874 7470  ions_url": "http
-00001e20: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
-00001e30: 6f6d 2f75 7365 7273 2f64 6565 7061 6b31  om/users/deepak1
-00001e40: 3535 362f 7375 6273 6372 6970 7469 6f6e  556/subscription
-00001e50: 7322 2c0a 2020 2020 226f 7267 616e 697a  s",.    "organiz
-00001e60: 6174 696f 6e73 5f75 726c 223a 2022 6874  ations_url": "ht
-00001e70: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
-00001e80: 2e63 6f6d 2f75 7365 7273 2f64 6565 7061  .com/users/deepa
-00001e90: 6b31 3535 362f 6f72 6773 222c 0a20 2020  k1556/orgs",.   
-00001ea0: 2022 7265 706f 735f 7572 6c22 3a20 2268   "repos_url": "h
-00001eb0: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
-00001ec0: 622e 636f 6d2f 7573 6572 732f 6465 6570  b.com/users/deep
-00001ed0: 616b 3135 3536 2f72 6570 6f73 222c 0a20  ak1556/repos",. 
-00001ee0: 2020 2022 6576 656e 7473 5f75 726c 223a     "events_url":
-00001ef0: 2022 6874 7470 733a 2f2f 6170 692e 6769   "https://api.gi
-00001f00: 7468 7562 2e63 6f6d 2f75 7365 7273 2f64  thub.com/users/d
-00001f10: 6565 7061 6b31 3535 362f 6576 656e 7473  eepak1556/events
-00001f20: 7b2f 7072 6976 6163 797d 222c 0a20 2020  {/privacy}",.   
-00001f30: 2022 7265 6365 6976 6564 5f65 7665 6e74   "received_event
-00001f40: 735f 7572 6c22 3a20 2268 7474 7073 3a2f  s_url": "https:/
-00001f50: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
-00001f60: 7573 6572 732f 6465 6570 616b 3135 3536  users/deepak1556
-00001f70: 2f72 6563 6569 7665 645f 6576 656e 7473  /received_events
-00001f80: 222c 0a20 2020 2022 7479 7065 223a 2022  ",.    "type": "
-00001f90: 5573 6572 222c 0a20 2020 2022 7369 7465  User",.    "site
-00001fa0: 5f61 646d 696e 223a 2066 616c 7365 0a20  _admin": false. 
-00001fb0: 207d 2c0a 2020 2272 6561 6374 696f 6e73   },.  "reactions
-00001fc0: 223a 207b 0a20 2020 2022 7572 6c22 3a20  ": {.    "url": 
-00001fd0: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
-00001fe0: 6875 622e 636f 6d2f 7265 706f 732f 6d69  hub.com/repos/mi
-00001ff0: 6372 6f73 6f66 742f 7673 636f 6465 2f69  crosoft/vscode/i
-00002000: 7373 7565 732f 3137 3930 3836 2f72 6561  ssues/179086/rea
-00002010: 6374 696f 6e73 222c 0a20 2020 2022 746f  ctions",.    "to
-00002020: 7461 6c5f 636f 756e 7422 3a20 302c 0a20  tal_count": 0,. 
-00002030: 2020 2022 2b31 223a 2030 2c0a 2020 2020     "+1": 0,.    
-00002040: 222d 3122 3a20 302c 0a20 2020 2022 6c61  "-1": 0,.    "la
-00002050: 7567 6822 3a20 302c 0a20 2020 2022 686f  ugh": 0,.    "ho
-00002060: 6f72 6179 223a 2030 2c0a 2020 2020 2263  oray": 0,.    "c
-00002070: 6f6e 6675 7365 6422 3a20 302c 0a20 2020  onfused": 0,.   
-00002080: 2022 6865 6172 7422 3a20 302c 0a20 2020   "heart": 0,.   
-00002090: 2022 726f 636b 6574 223a 2030 2c0a 2020   "rocket": 0,.  
-000020a0: 2020 2265 7965 7322 3a20 300a 2020 7d2c    "eyes": 0.  },
-000020b0: 0a20 2022 7469 6d65 6c69 6e65 5f75 726c  .  "timeline_url
-000020c0: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
-000020d0: 6769 7468 7562 2e63 6f6d 2f72 6570 6f73  github.com/repos
-000020e0: 2f6d 6963 726f 736f 6674 2f76 7363 6f64  /microsoft/vscod
-000020f0: 652f 6973 7375 6573 2f31 3739 3038 362f  e/issues/179086/
-00002100: 7469 6d65 6c69 6e65 222c 0a20 2022 7374  timeline",.  "st
-00002110: 6174 655f 7265 6173 6f6e 223a 2022 7265  ate_reason": "re
-00002120: 6f70 656e 6564 220a 7d                   opened".}
+00000000: 7b0d 0a20 2022 7572 6c22 3a20 2268 7474  {..  "url": "htt
+00000010: 7073 3a2f 2f61 7069 2e67 6974 6875 622e  ps://api.github.
+00000020: 636f 6d2f 7265 706f 732f 6d69 6372 6f73  com/repos/micros
+00000030: 6f66 742f 7673 636f 6465 2f69 7373 7565  oft/vscode/issue
+00000040: 732f 3137 3930 3836 222c 0d0a 2020 2272  s/179086",..  "r
+00000050: 6570 6f73 6974 6f72 795f 7572 6c22 3a20  epository_url": 
+00000060: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
+00000070: 6875 622e 636f 6d2f 7265 706f 732f 6d69  hub.com/repos/mi
+00000080: 6372 6f73 6f66 742f 7673 636f 6465 222c  crosoft/vscode",
+00000090: 0d0a 2020 226c 6162 656c 735f 7572 6c22  ..  "labels_url"
+000000a0: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
+000000b0: 6974 6875 622e 636f 6d2f 7265 706f 732f  ithub.com/repos/
+000000c0: 6d69 6372 6f73 6f66 742f 7673 636f 6465  microsoft/vscode
+000000d0: 2f69 7373 7565 732f 3137 3930 3836 2f6c  /issues/179086/l
+000000e0: 6162 656c 737b 2f6e 616d 657d 222c 0d0a  abels{/name}",..
+000000f0: 2020 2263 6f6d 6d65 6e74 735f 7572 6c22    "comments_url"
+00000100: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
+00000110: 6974 6875 622e 636f 6d2f 7265 706f 732f  ithub.com/repos/
+00000120: 6d69 6372 6f73 6f66 742f 7673 636f 6465  microsoft/vscode
+00000130: 2f69 7373 7565 732f 3137 3930 3836 2f63  /issues/179086/c
+00000140: 6f6d 6d65 6e74 7322 2c0d 0a20 2022 6576  omments",..  "ev
+00000150: 656e 7473 5f75 726c 223a 2022 6874 7470  ents_url": "http
+00000160: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+00000170: 6f6d 2f72 6570 6f73 2f6d 6963 726f 736f  om/repos/microso
+00000180: 6674 2f76 7363 6f64 652f 6973 7375 6573  ft/vscode/issues
+00000190: 2f31 3739 3038 362f 6576 656e 7473 222c  /179086/events",
+000001a0: 0d0a 2020 2268 746d 6c5f 7572 6c22 3a20  ..  "html_url": 
+000001b0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000001c0: 636f 6d2f 6d69 6372 6f73 6f66 742f 7673  com/microsoft/vs
+000001d0: 636f 6465 2f69 7373 7565 732f 3137 3930  code/issues/1790
+000001e0: 3836 222c 0d0a 2020 2269 6422 3a20 3136  86",..  "id": 16
+000001f0: 3533 3233 3535 3133 2c0d 0a20 2022 6e6f  53235513,..  "no
+00000200: 6465 5f69 6422 3a20 2249 5f6b 7744 4f41  de_id": "I_kwDOA
+00000210: 6e38 524c 4d35 6969 6c38 3522 2c0d 0a20  n8RLM5iil85",.. 
+00000220: 2022 6e75 6d62 6572 223a 2031 3739 3038   "number": 17908
+00000230: 362c 0d0a 2020 2274 6974 6c65 223a 2022  6,..  "title": "
+00000240: 4754 4b2b 206d 6f64 756c 6520 6c69 6263  GTK+ module libc
+00000250: 616e 6265 7272 612d 6774 6b2d 6d6f 6475  anberra-gtk-modu
+00000260: 6c65 2e73 6f20 6361 6e6e 6f74 2062 6520  le.so cannot be 
+00000270: 6c6f 6164 6564 222c 0d0a 2020 2275 7365  loaded",..  "use
+00000280: 7222 3a20 7b0d 0a20 2020 2022 6c6f 6769  r": {..    "logi
+00000290: 6e22 3a20 2250 6574 726f 7336 3236 222c  n": "Petros626",
+000002a0: 0d0a 2020 2020 2269 6422 3a20 3632 3335  ..    "id": 6235
+000002b0: 3437 3231 2c0d 0a20 2020 2022 6e6f 6465  4721,..    "node
+000002c0: 5f69 6422 3a20 224d 4451 3656 584e 6c63  _id": "MDQ6VXNlc
+000002d0: 6a59 794d 7a55 304e 7a49 7822 2c0d 0a20  jYyMzU0NzIx",.. 
+000002e0: 2020 2022 6176 6174 6172 5f75 726c 223a     "avatar_url":
+000002f0: 2022 6874 7470 733a 2f2f 6176 6174 6172   "https://avatar
+00000300: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00000310: 656e 742e 636f 6d2f 752f 3632 3335 3437  ent.com/u/623547
+00000320: 3231 3f76 3d34 222c 0d0a 2020 2020 2267  21?v=4",..    "g
+00000330: 7261 7661 7461 725f 6964 223a 2022 222c  ravatar_id": "",
+00000340: 0d0a 2020 2020 2275 726c 223a 2022 6874  ..    "url": "ht
+00000350: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
+00000360: 2e63 6f6d 2f75 7365 7273 2f50 6574 726f  .com/users/Petro
+00000370: 7336 3236 222c 0d0a 2020 2020 2268 746d  s626",..    "htm
+00000380: 6c5f 7572 6c22 3a20 2268 7474 7073 3a2f  l_url": "https:/
+00000390: 2f67 6974 6875 622e 636f 6d2f 5065 7472  /github.com/Petr
+000003a0: 6f73 3632 3622 2c0d 0a20 2020 2022 666f  os626",..    "fo
+000003b0: 6c6c 6f77 6572 735f 7572 6c22 3a20 2268  llowers_url": "h
+000003c0: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
+000003d0: 622e 636f 6d2f 7573 6572 732f 5065 7472  b.com/users/Petr
+000003e0: 6f73 3632 362f 666f 6c6c 6f77 6572 7322  os626/followers"
+000003f0: 2c0d 0a20 2020 2022 666f 6c6c 6f77 696e  ,..    "followin
+00000400: 675f 7572 6c22 3a20 2268 7474 7073 3a2f  g_url": "https:/
+00000410: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00000420: 7573 6572 732f 5065 7472 6f73 3632 362f  users/Petros626/
+00000430: 666f 6c6c 6f77 696e 677b 2f6f 7468 6572  following{/other
+00000440: 5f75 7365 727d 222c 0d0a 2020 2020 2267  _user}",..    "g
+00000450: 6973 7473 5f75 726c 223a 2022 6874 7470  ists_url": "http
+00000460: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+00000470: 6f6d 2f75 7365 7273 2f50 6574 726f 7336  om/users/Petros6
+00000480: 3236 2f67 6973 7473 7b2f 6769 7374 5f69  26/gists{/gist_i
+00000490: 647d 222c 0d0a 2020 2020 2273 7461 7272  d}",..    "starr
+000004a0: 6564 5f75 726c 223a 2022 6874 7470 733a  ed_url": "https:
+000004b0: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
+000004c0: 2f75 7365 7273 2f50 6574 726f 7336 3236  /users/Petros626
+000004d0: 2f73 7461 7272 6564 7b2f 6f77 6e65 727d  /starred{/owner}
+000004e0: 7b2f 7265 706f 7d22 2c0d 0a20 2020 2022  {/repo}",..    "
+000004f0: 7375 6273 6372 6970 7469 6f6e 735f 7572  subscriptions_ur
+00000500: 6c22 3a20 2268 7474 7073 3a2f 2f61 7069  l": "https://api
+00000510: 2e67 6974 6875 622e 636f 6d2f 7573 6572  .github.com/user
+00000520: 732f 5065 7472 6f73 3632 362f 7375 6273  s/Petros626/subs
+00000530: 6372 6970 7469 6f6e 7322 2c0d 0a20 2020  criptions",..   
+00000540: 2022 6f72 6761 6e69 7a61 7469 6f6e 735f   "organizations_
+00000550: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
+00000560: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
+00000570: 6572 732f 5065 7472 6f73 3632 362f 6f72  ers/Petros626/or
+00000580: 6773 222c 0d0a 2020 2020 2272 6570 6f73  gs",..    "repos
+00000590: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
+000005a0: 6170 692e 6769 7468 7562 2e63 6f6d 2f75  api.github.com/u
+000005b0: 7365 7273 2f50 6574 726f 7336 3236 2f72  sers/Petros626/r
+000005c0: 6570 6f73 222c 0d0a 2020 2020 2265 7665  epos",..    "eve
+000005d0: 6e74 735f 7572 6c22 3a20 2268 7474 7073  nts_url": "https
+000005e0: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
+000005f0: 6d2f 7573 6572 732f 5065 7472 6f73 3632  m/users/Petros62
+00000600: 362f 6576 656e 7473 7b2f 7072 6976 6163  6/events{/privac
+00000610: 797d 222c 0d0a 2020 2020 2272 6563 6569  y}",..    "recei
+00000620: 7665 645f 6576 656e 7473 5f75 726c 223a  ved_events_url":
+00000630: 2022 6874 7470 733a 2f2f 6170 692e 6769   "https://api.gi
+00000640: 7468 7562 2e63 6f6d 2f75 7365 7273 2f50  thub.com/users/P
+00000650: 6574 726f 7336 3236 2f72 6563 6569 7665  etros626/receive
+00000660: 645f 6576 656e 7473 222c 0d0a 2020 2020  d_events",..    
+00000670: 2274 7970 6522 3a20 2255 7365 7222 2c0d  "type": "User",.
+00000680: 0a20 2020 2022 7369 7465 5f61 646d 696e  .    "site_admin
+00000690: 223a 2066 616c 7365 0d0a 2020 7d2c 0d0a  ": false..  },..
+000006a0: 2020 226c 6162 656c 7322 3a20 5b0d 0a20    "labels": [.. 
+000006b0: 2020 207b 0d0a 2020 2020 2020 2269 6422     {..      "id"
+000006c0: 3a20 3235 3631 3239 3939 332c 0d0a 2020  : 256129993,..  
+000006d0: 2020 2020 226e 6f64 655f 6964 223a 2022      "node_id": "
+000006e0: 4d44 5536 5447 4669 5a57 7779 4e54 5978  MDU6TGFiZWwyNTYx
+000006f0: 4d6a 6b35 4f54 4d3d 222c 0d0a 2020 2020  Mjk5OTM=",..    
+00000700: 2020 2275 726c 223a 2022 6874 7470 733a    "url": "https:
+00000710: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
+00000720: 2f72 6570 6f73 2f6d 6963 726f 736f 6674  /repos/microsoft
+00000730: 2f76 7363 6f64 652f 6c61 6265 6c73 2f62  /vscode/labels/b
+00000740: 7567 222c 0d0a 2020 2020 2020 226e 616d  ug",..      "nam
+00000750: 6522 3a20 2262 7567 222c 0d0a 2020 2020  e": "bug",..    
+00000760: 2020 2263 6f6c 6f72 223a 2022 3844 3636    "color": "8D66
+00000770: 3733 222c 0d0a 2020 2020 2020 2264 6566  73",..      "def
+00000780: 6175 6c74 223a 2074 7275 652c 0d0a 2020  ault": true,..  
+00000790: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000007a0: 223a 2022 4973 7375 6520 6964 656e 7469  ": "Issue identi
+000007b0: 6669 6564 2062 7920 5653 2043 6f64 6520  fied by VS Code 
+000007c0: 5465 616d 206d 656d 6265 7220 6173 2070  Team member as p
+000007d0: 726f 6261 626c 6520 6275 6722 0d0a 2020  robable bug"..  
+000007e0: 2020 7d2c 0d0a 2020 2020 7b0d 0a20 2020    },..    {..   
+000007f0: 2020 2022 6964 223a 2033 3030 3333 3437     "id": 3003347
+00000800: 3836 2c0d 0a20 2020 2020 2022 6e6f 6465  86,..      "node
+00000810: 5f69 6422 3a20 224d 4455 3654 4746 695a  _id": "MDU6TGFiZ
+00000820: 5777 7a4d 4441 7a4d 7a51 334f 4459 3d22  WwzMDAzMzQ3ODY="
+00000830: 2c0d 0a20 2020 2020 2022 7572 6c22 3a20  ,..      "url": 
+00000840: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
+00000850: 6875 622e 636f 6d2f 7265 706f 732f 6d69  hub.com/repos/mi
+00000860: 6372 6f73 6f66 742f 7673 636f 6465 2f6c  crosoft/vscode/l
+00000870: 6162 656c 732f 7665 7269 6669 6361 7469  abels/verificati
+00000880: 6f6e 2d66 6f75 6e64 222c 0d0a 2020 2020  on-found",..    
+00000890: 2020 226e 616d 6522 3a20 2276 6572 6966    "name": "verif
+000008a0: 6963 6174 696f 6e2d 666f 756e 6422 2c0d  ication-found",.
+000008b0: 0a20 2020 2020 2022 636f 6c6f 7222 3a20  .      "color": 
+000008c0: 2266 3763 3663 3722 2c0d 0a20 2020 2020  "f7c6c7",..     
+000008d0: 2022 6465 6661 756c 7422 3a20 6661 6c73   "default": fals
+000008e0: 652c 0d0a 2020 2020 2020 2264 6573 6372  e,..      "descr
+000008f0: 6970 7469 6f6e 223a 2022 4973 7375 6520  iption": "Issue 
+00000900: 7665 7269 6669 6361 7469 6f6e 2066 6169  verification fai
+00000910: 6c65 6422 0d0a 2020 2020 7d2c 0d0a 2020  led"..    },..  
+00000920: 2020 7b0d 0a20 2020 2020 2022 6964 223a    {..      "id":
+00000930: 2033 3231 3039 3235 3130 2c0d 0a20 2020   321092510,..   
+00000940: 2020 2022 6e6f 6465 5f69 6422 3a20 224d     "node_id": "M
+00000950: 4455 3654 4746 695a 5777 7a4d 6a45 774f  DU6TGFiZWwzMjEwO
+00000960: 5449 314d 5441 3d22 2c0d 0a20 2020 2020  TI1MTA=",..     
+00000970: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
+00000980: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00000990: 7265 706f 732f 6d69 6372 6f73 6f66 742f  repos/microsoft/
+000009a0: 7673 636f 6465 2f6c 6162 656c 732f 6c69  vscode/labels/li
+000009b0: 6e75 7822 2c0d 0a20 2020 2020 2022 6e61  nux",..      "na
+000009c0: 6d65 223a 2022 6c69 6e75 7822 2c0d 0a20  me": "linux",.. 
+000009d0: 2020 2020 2022 636f 6c6f 7222 3a20 2230       "color": "0
+000009e0: 3036 6237 3522 2c0d 0a20 2020 2020 2022  06b75",..      "
+000009f0: 6465 6661 756c 7422 3a20 6661 6c73 652c  default": false,
+00000a00: 0d0a 2020 2020 2020 2264 6573 6372 6970  ..      "descrip
+00000a10: 7469 6f6e 223a 2022 4973 7375 6573 2077  tion": "Issues w
+00000a20: 6974 6820 5653 2043 6f64 6520 6f6e 204c  ith VS Code on L
+00000a30: 696e 7578 220d 0a20 2020 207d 2c0d 0a20  inux"..    },.. 
+00000a40: 2020 207b 0d0a 2020 2020 2020 2269 6422     {..      "id"
+00000a50: 3a20 3336 3236 3934 3633 322c 0d0a 2020  : 362694632,..  
+00000a60: 2020 2020 226e 6f64 655f 6964 223a 2022      "node_id": "
+00000a70: 4d44 5536 5447 4669 5a57 777a 4e6a 4932  MDU6TGFiZWwzNjI2
+00000a80: 4f54 5132 4d7a 493d 222c 0d0a 2020 2020  OTQ2MzI=",..    
+00000a90: 2020 2275 726c 223a 2022 6874 7470 733a    "url": "https:
+00000aa0: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
+00000ab0: 2f72 6570 6f73 2f6d 6963 726f 736f 6674  /repos/microsoft
+00000ac0: 2f76 7363 6f64 652f 6c61 6265 6c73 2f74  /vscode/labels/t
+00000ad0: 6572 6d69 6e61 6c22 2c0d 0a20 2020 2020  erminal",..     
+00000ae0: 2022 6e61 6d65 223a 2022 7465 726d 696e   "name": "termin
+00000af0: 616c 222c 0d0a 2020 2020 2020 2263 6f6c  al",..      "col
+00000b00: 6f72 223a 2022 6335 6465 6635 222c 0d0a  or": "c5def5",..
+00000b10: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
+00000b20: 2066 616c 7365 2c0d 0a20 2020 2020 2022   false,..      "
+00000b30: 6465 7363 7269 7074 696f 6e22 3a20 2249  description": "I
+00000b40: 6e74 6567 7261 7465 6420 7465 726d 696e  ntegrated termin
+00000b50: 616c 2069 7373 7565 7322 0d0a 2020 2020  al issues"..    
+00000b60: 7d2c 0d0a 2020 2020 7b0d 0a20 2020 2020  },..    {..     
+00000b70: 2022 6964 223a 2031 3033 3434 3435 3934   "id": 103444594
+00000b80: 382c 0d0a 2020 2020 2020 226e 6f64 655f  8,..      "node_
+00000b90: 6964 223a 2022 4d44 5536 5447 4669 5a57  id": "MDU6TGFiZW
+00000ba0: 7778 4d44 4d30 4e44 5131 4f54 5134 222c  wxMDM0NDQ1OTQ4",
+00000bb0: 0d0a 2020 2020 2020 2275 726c 223a 2022  ..      "url": "
+00000bc0: 6874 7470 733a 2f2f 6170 692e 6769 7468  https://api.gith
+00000bd0: 7562 2e63 6f6d 2f72 6570 6f73 2f6d 6963  ub.com/repos/mic
+00000be0: 726f 736f 6674 2f76 7363 6f64 652f 6c61  rosoft/vscode/la
+00000bf0: 6265 6c73 2f73 6e61 7022 2c0d 0a20 2020  bels/snap",..   
+00000c00: 2020 2022 6e61 6d65 223a 2022 736e 6170     "name": "snap
+00000c10: 222c 0d0a 2020 2020 2020 2263 6f6c 6f72  ",..      "color
+00000c20: 223a 2022 6335 6465 6635 222c 0d0a 2020  ": "c5def5",..  
+00000c30: 2020 2020 2264 6566 6175 6c74 223a 2066      "default": f
+00000c40: 616c 7365 2c0d 0a20 2020 2020 2022 6465  alse,..      "de
+00000c50: 7363 7269 7074 696f 6e22 3a20 2249 7373  scription": "Iss
+00000c60: 7565 7320 7265 6c61 7465 6420 746f 2074  ues related to t
+00000c70: 6865 2073 6e61 7020 7061 636b 6167 6522  he snap package"
+00000c80: 0d0a 2020 2020 7d2c 0d0a 2020 2020 7b0d  ..    },..    {.
+00000c90: 0a20 2020 2020 2022 6964 223a 2031 3131  .      "id": 111
+00000ca0: 3937 3934 3437 342c 0d0a 2020 2020 2020  9794474,..      
+00000cb0: 226e 6f64 655f 6964 223a 2022 4d44 5536  "node_id": "MDU6
+00000cc0: 5447 4669 5a57 7778 4d54 4535 4e7a 6b30  TGFiZWwxMTE5Nzk0
+00000cd0: 4e44 6330 222c 0d0a 2020 2020 2020 2275  NDc0",..      "u
+00000ce0: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
+00000cf0: 692e 6769 7468 7562 2e63 6f6d 2f72 6570  i.github.com/rep
+00000d00: 6f73 2f6d 6963 726f 736f 6674 2f76 7363  os/microsoft/vsc
+00000d10: 6f64 652f 6c61 6265 6c73 2f63 6f6e 6669  ode/labels/confi
+00000d20: 726d 6564 222c 0d0a 2020 2020 2020 226e  rmed",..      "n
+00000d30: 616d 6522 3a20 2263 6f6e 6669 726d 6564  ame": "confirmed
+00000d40: 222c 0d0a 2020 2020 2020 2263 6f6c 6f72  ",..      "color
+00000d50: 223a 2022 3030 3938 3030 222c 0d0a 2020  ": "009800",..  
+00000d60: 2020 2020 2264 6566 6175 6c74 223a 2066      "default": f
+00000d70: 616c 7365 2c0d 0a20 2020 2020 2022 6465  alse,..      "de
+00000d80: 7363 7269 7074 696f 6e22 3a20 2249 7373  scription": "Iss
+00000d90: 7565 2068 6173 2062 6565 6e20 636f 6e66  ue has been conf
+00000da0: 6972 6d65 6420 6279 2056 5320 436f 6465  irmed by VS Code
+00000db0: 2054 6561 6d20 6d65 6d62 6572 220d 0a20   Team member".. 
+00000dc0: 2020 207d 0d0a 2020 5d2c 0d0a 2020 2273     }..  ],..  "s
+00000dd0: 7461 7465 223a 2022 6f70 656e 222c 0d0a  tate": "open",..
+00000de0: 2020 226c 6f63 6b65 6422 3a20 6661 6c73    "locked": fals
+00000df0: 652c 0d0a 2020 2261 7373 6967 6e65 6522  e,..  "assignee"
+00000e00: 3a20 7b0d 0a20 2020 2022 6c6f 6769 6e22  : {..    "login"
+00000e10: 3a20 2264 6565 7061 6b31 3535 3622 2c0d  : "deepak1556",.
+00000e20: 0a20 2020 2022 6964 223a 2039 3634 3338  .    "id": 96438
+00000e30: 362c 0d0a 2020 2020 226e 6f64 655f 6964  6,..    "node_id
+00000e40: 223a 2022 4d44 5136 5658 4e6c 636a 6b32  ": "MDQ6VXNlcjk2
+00000e50: 4e44 4d34 4e67 3d3d 222c 0d0a 2020 2020  NDM4Ng==",..    
+00000e60: 2261 7661 7461 725f 7572 6c22 3a20 2268  "avatar_url": "h
+00000e70: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
+00000e80: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000e90: 2e63 6f6d 2f75 2f39 3634 3338 363f 763d  .com/u/964386?v=
+00000ea0: 3422 2c0d 0a20 2020 2022 6772 6176 6174  4",..    "gravat
+00000eb0: 6172 5f69 6422 3a20 2222 2c0d 0a20 2020  ar_id": "",..   
+00000ec0: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
+00000ed0: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00000ee0: 7573 6572 732f 6465 6570 616b 3135 3536  users/deepak1556
+00000ef0: 222c 0d0a 2020 2020 2268 746d 6c5f 7572  ",..    "html_ur
+00000f00: 6c22 3a20 2268 7474 7073 3a2f 2f67 6974  l": "https://git
+00000f10: 6875 622e 636f 6d2f 6465 6570 616b 3135  hub.com/deepak15
+00000f20: 3536 222c 0d0a 2020 2020 2266 6f6c 6c6f  56",..    "follo
+00000f30: 7765 7273 5f75 726c 223a 2022 6874 7470  wers_url": "http
+00000f40: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+00000f50: 6f6d 2f75 7365 7273 2f64 6565 7061 6b31  om/users/deepak1
+00000f60: 3535 362f 666f 6c6c 6f77 6572 7322 2c0d  556/followers",.
+00000f70: 0a20 2020 2022 666f 6c6c 6f77 696e 675f  .    "following_
+00000f80: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
+00000f90: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
+00000fa0: 6572 732f 6465 6570 616b 3135 3536 2f66  ers/deepak1556/f
+00000fb0: 6f6c 6c6f 7769 6e67 7b2f 6f74 6865 725f  ollowing{/other_
+00000fc0: 7573 6572 7d22 2c0d 0a20 2020 2022 6769  user}",..    "gi
+00000fd0: 7374 735f 7572 6c22 3a20 2268 7474 7073  sts_url": "https
+00000fe0: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
+00000ff0: 6d2f 7573 6572 732f 6465 6570 616b 3135  m/users/deepak15
+00001000: 3536 2f67 6973 7473 7b2f 6769 7374 5f69  56/gists{/gist_i
+00001010: 647d 222c 0d0a 2020 2020 2273 7461 7272  d}",..    "starr
+00001020: 6564 5f75 726c 223a 2022 6874 7470 733a  ed_url": "https:
+00001030: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
+00001040: 2f75 7365 7273 2f64 6565 7061 6b31 3535  /users/deepak155
+00001050: 362f 7374 6172 7265 647b 2f6f 776e 6572  6/starred{/owner
+00001060: 7d7b 2f72 6570 6f7d 222c 0d0a 2020 2020  }{/repo}",..    
+00001070: 2273 7562 7363 7269 7074 696f 6e73 5f75  "subscriptions_u
+00001080: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
+00001090: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
+000010a0: 7273 2f64 6565 7061 6b31 3535 362f 7375  rs/deepak1556/su
+000010b0: 6273 6372 6970 7469 6f6e 7322 2c0d 0a20  bscriptions",.. 
+000010c0: 2020 2022 6f72 6761 6e69 7a61 7469 6f6e     "organization
+000010d0: 735f 7572 6c22 3a20 2268 7474 7073 3a2f  s_url": "https:/
+000010e0: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+000010f0: 7573 6572 732f 6465 6570 616b 3135 3536  users/deepak1556
+00001100: 2f6f 7267 7322 2c0d 0a20 2020 2022 7265  /orgs",..    "re
+00001110: 706f 735f 7572 6c22 3a20 2268 7474 7073  pos_url": "https
+00001120: 3a2f 2f61 7069 2e67 6974 6875 622e 636f  ://api.github.co
+00001130: 6d2f 7573 6572 732f 6465 6570 616b 3135  m/users/deepak15
+00001140: 3536 2f72 6570 6f73 222c 0d0a 2020 2020  56/repos",..    
+00001150: 2265 7665 6e74 735f 7572 6c22 3a20 2268  "events_url": "h
+00001160: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
+00001170: 622e 636f 6d2f 7573 6572 732f 6465 6570  b.com/users/deep
+00001180: 616b 3135 3536 2f65 7665 6e74 737b 2f70  ak1556/events{/p
+00001190: 7269 7661 6379 7d22 2c0d 0a20 2020 2022  rivacy}",..    "
+000011a0: 7265 6365 6976 6564 5f65 7665 6e74 735f  received_events_
+000011b0: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
+000011c0: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
+000011d0: 6572 732f 6465 6570 616b 3135 3536 2f72  ers/deepak1556/r
+000011e0: 6563 6569 7665 645f 6576 656e 7473 222c  eceived_events",
+000011f0: 0d0a 2020 2020 2274 7970 6522 3a20 2255  ..    "type": "U
+00001200: 7365 7222 2c0d 0a20 2020 2022 7369 7465  ser",..    "site
+00001210: 5f61 646d 696e 223a 2066 616c 7365 0d0a  _admin": false..
+00001220: 2020 7d2c 0d0a 2020 2261 7373 6967 6e65    },..  "assigne
+00001230: 6573 223a 205b 0d0a 2020 2020 7b0d 0a20  es": [..    {.. 
+00001240: 2020 2020 2022 6c6f 6769 6e22 3a20 2264       "login": "d
+00001250: 6565 7061 6b31 3535 3622 2c0d 0a20 2020  eepak1556",..   
+00001260: 2020 2022 6964 223a 2039 3634 3338 362c     "id": 964386,
+00001270: 0d0a 2020 2020 2020 226e 6f64 655f 6964  ..      "node_id
+00001280: 223a 2022 4d44 5136 5658 4e6c 636a 6b32  ": "MDQ6VXNlcjk2
+00001290: 4e44 4d34 4e67 3d3d 222c 0d0a 2020 2020  NDM4Ng==",..    
+000012a0: 2020 2261 7661 7461 725f 7572 6c22 3a20    "avatar_url": 
+000012b0: 2268 7474 7073 3a2f 2f61 7661 7461 7273  "https://avatars
+000012c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000012d0: 6e74 2e63 6f6d 2f75 2f39 3634 3338 363f  nt.com/u/964386?
+000012e0: 763d 3422 2c0d 0a20 2020 2020 2022 6772  v=4",..      "gr
+000012f0: 6176 6174 6172 5f69 6422 3a20 2222 2c0d  avatar_id": "",.
+00001300: 0a20 2020 2020 2022 7572 6c22 3a20 2268  .      "url": "h
+00001310: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
+00001320: 622e 636f 6d2f 7573 6572 732f 6465 6570  b.com/users/deep
+00001330: 616b 3135 3536 222c 0d0a 2020 2020 2020  ak1556",..      
+00001340: 2268 746d 6c5f 7572 6c22 3a20 2268 7474  "html_url": "htt
+00001350: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001360: 6465 6570 616b 3135 3536 222c 0d0a 2020  deepak1556",..  
+00001370: 2020 2020 2266 6f6c 6c6f 7765 7273 5f75      "followers_u
+00001380: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
+00001390: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
+000013a0: 7273 2f64 6565 7061 6b31 3535 362f 666f  rs/deepak1556/fo
+000013b0: 6c6c 6f77 6572 7322 2c0d 0a20 2020 2020  llowers",..     
+000013c0: 2022 666f 6c6c 6f77 696e 675f 7572 6c22   "following_url"
+000013d0: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
+000013e0: 6974 6875 622e 636f 6d2f 7573 6572 732f  ithub.com/users/
+000013f0: 6465 6570 616b 3135 3536 2f66 6f6c 6c6f  deepak1556/follo
+00001400: 7769 6e67 7b2f 6f74 6865 725f 7573 6572  wing{/other_user
+00001410: 7d22 2c0d 0a20 2020 2020 2022 6769 7374  }",..      "gist
+00001420: 735f 7572 6c22 3a20 2268 7474 7073 3a2f  s_url": "https:/
+00001430: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00001440: 7573 6572 732f 6465 6570 616b 3135 3536  users/deepak1556
+00001450: 2f67 6973 7473 7b2f 6769 7374 5f69 647d  /gists{/gist_id}
+00001460: 222c 0d0a 2020 2020 2020 2273 7461 7272  ",..      "starr
+00001470: 6564 5f75 726c 223a 2022 6874 7470 733a  ed_url": "https:
+00001480: 2f2f 6170 692e 6769 7468 7562 2e63 6f6d  //api.github.com
+00001490: 2f75 7365 7273 2f64 6565 7061 6b31 3535  /users/deepak155
+000014a0: 362f 7374 6172 7265 647b 2f6f 776e 6572  6/starred{/owner
+000014b0: 7d7b 2f72 6570 6f7d 222c 0d0a 2020 2020  }{/repo}",..    
+000014c0: 2020 2273 7562 7363 7269 7074 696f 6e73    "subscriptions
+000014d0: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
+000014e0: 6170 692e 6769 7468 7562 2e63 6f6d 2f75  api.github.com/u
+000014f0: 7365 7273 2f64 6565 7061 6b31 3535 362f  sers/deepak1556/
+00001500: 7375 6273 6372 6970 7469 6f6e 7322 2c0d  subscriptions",.
+00001510: 0a20 2020 2020 2022 6f72 6761 6e69 7a61  .      "organiza
+00001520: 7469 6f6e 735f 7572 6c22 3a20 2268 7474  tions_url": "htt
+00001530: 7073 3a2f 2f61 7069 2e67 6974 6875 622e  ps://api.github.
+00001540: 636f 6d2f 7573 6572 732f 6465 6570 616b  com/users/deepak
+00001550: 3135 3536 2f6f 7267 7322 2c0d 0a20 2020  1556/orgs",..   
+00001560: 2020 2022 7265 706f 735f 7572 6c22 3a20     "repos_url": 
+00001570: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
+00001580: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
+00001590: 6570 616b 3135 3536 2f72 6570 6f73 222c  epak1556/repos",
+000015a0: 0d0a 2020 2020 2020 2265 7665 6e74 735f  ..      "events_
+000015b0: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
+000015c0: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
+000015d0: 6572 732f 6465 6570 616b 3135 3536 2f65  ers/deepak1556/e
+000015e0: 7665 6e74 737b 2f70 7269 7661 6379 7d22  vents{/privacy}"
+000015f0: 2c0d 0a20 2020 2020 2022 7265 6365 6976  ,..      "receiv
+00001600: 6564 5f65 7665 6e74 735f 7572 6c22 3a20  ed_events_url": 
+00001610: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
+00001620: 6875 622e 636f 6d2f 7573 6572 732f 6465  hub.com/users/de
+00001630: 6570 616b 3135 3536 2f72 6563 6569 7665  epak1556/receive
+00001640: 645f 6576 656e 7473 222c 0d0a 2020 2020  d_events",..    
+00001650: 2020 2274 7970 6522 3a20 2255 7365 7222    "type": "User"
+00001660: 2c0d 0a20 2020 2020 2022 7369 7465 5f61  ,..      "site_a
+00001670: 646d 696e 223a 2066 616c 7365 0d0a 2020  dmin": false..  
+00001680: 2020 7d0d 0a20 205d 2c0d 0a20 2022 6d69    }..  ],..  "mi
+00001690: 6c65 7374 6f6e 6522 3a20 6e75 6c6c 2c0d  lestone": null,.
+000016a0: 0a20 2022 636f 6d6d 656e 7473 223a 2031  .  "comments": 1
+000016b0: 352c 0d0a 2020 2263 7265 6174 6564 5f61  5,..  "created_a
+000016c0: 7422 3a20 2232 3032 332d 3034 2d30 3454  t": "2023-04-04T
+000016d0: 3035 3a35 363a 3437 5a22 2c0d 0a20 2022  05:56:47Z",..  "
+000016e0: 7570 6461 7465 645f 6174 223a 2022 3230  updated_at": "20
+000016f0: 3233 2d30 372d 3235 5431 333a 3338 3a35  23-07-25T13:38:5
+00001700: 305a 222c 0d0a 2020 2263 6c6f 7365 645f  0Z",..  "closed_
+00001710: 6174 223a 206e 756c 6c2c 0d0a 2020 2261  at": null,..  "a
+00001720: 7574 686f 725f 6173 736f 6369 6174 696f  uthor_associatio
+00001730: 6e22 3a20 224e 4f4e 4522 2c0d 0a20 2022  n": "NONE",..  "
+00001740: 6163 7469 7665 5f6c 6f63 6b5f 7265 6173  active_lock_reas
+00001750: 6f6e 223a 206e 756c 6c2c 0d0a 2020 2262  on": null,..  "b
+00001760: 6f64 7922 3a20 2248 656c 6c6f 2067 7579  ody": "Hello guy
+00001770: 732c 5c72 5c6e 5c72 5c6e 4927 6d20 7573  s,\r\n\r\nI'm us
+00001780: 696e 6720 5f4f 7065 6e43 565f 2069 6e20  ing _OpenCV_ in 
+00001790: 5653 436f 6465 2028 5562 756e 7475 2053  VSCode (Ubuntu S
+000017a0: 6f66 7477 6172 6520 696e 7374 616c 6c61  oftware installa
+000017b0: 7469 6f6e 2920 616e 6420 6576 6572 7974  tion) and everyt
+000017c0: 6869 6e67 2077 6f72 6b65 6420 6669 6e65  hing worked fine
+000017d0: 2c20 756e 7469 6c20 4920 7570 6461 7465  , until I update
+000017e0: 6420 6d79 206c 6962 7261 7269 6573 2028  d my libraries (
+000017f0: 6073 7564 6f20 6170 742d 6765 7420 7570  `sudo apt-get up
+00001800: 6461 7465 2f75 7067 7261 6465 2f66 756c  date/upgrade/ful
+00001810: 6c2d 7570 6772 6164 6560 2920 4920 6775  l-upgrade`) I gu
+00001820: 6573 732e 2042 7574 206e 6f77 2056 5343  ess. But now VSC
+00001830: 6f64 6520 6f72 2072 6174 6865 7220 5f4f  ode or rather _O
+00001840: 7065 6e43 565f 2063 616e 2774 2066 696e  penCV_ can't fin
+00001850: 6420 7468 6520 5f47 544b 5f20 6c69 6272  d the _GTK_ libr
+00001860: 6172 792e 205c 725c 6e5c 725c 6e49 2776  ary. \r\n\r\nI'v
+00001870: 6520 7465 7374 6564 2074 6869 7320 7375  e tested this su
+00001880: 6363 6573 6675 6c6c 793a 5c72 5c6e 2060  ccesfully:\r\n `
+00001890: 4754 4b5f 5041 5448 3d2f 7573 722f 6c69  GTK_PATH=/usr/li
+000018a0: 622f 7838 365f 3634 2d6c 696e 7578 2d67  b/x86_64-linux-g
+000018b0: 6e75 2f67 746b 2d32 2e30 202e 2f74 6573  nu/gtk-2.0 ./tes
+000018c0: 7460 202d 2d3e 2077 6f72 6b73 5c72 5c6e  t` --> works\r\n
+000018d0: 5c72 5c6e 4275 7420 7768 656e 2049 2073  \r\nBut when I s
+000018e0: 7065 6369 6679 2074 6865 2076 6572 7369  pecify the versi
+000018f0: 6f6e 2067 746b 2d33 2e30 3a5c 725c 6e60  on gtk-3.0:\r\n`
+00001900: 4754 4b5f 5041 5448 3d2f 7573 722f 6c69  GTK_PATH=/usr/li
+00001910: 622f 7838 365f 3634 2d6c 696e 7578 2d67  b/x86_64-linux-g
+00001920: 6e75 2f67 746b 2d33 2e30 202e 2f74 6573  nu/gtk-3.0 ./tes
+00001930: 7460 202d 2d3e 2066 6169 6c73 5c72 5c6e  t` --> fails\r\n
+00001940: 5c72 5c6e 204e 6f72 6d61 6c6c 7920 7468  \r\n Normally th
+00001950: 6520 6c6f 6164 6564 2076 6572 7369 6f6e  e loaded version
+00001960: 2077 6974 686f 7574 2075 7369 6e67 2047   without using G
+00001970: 544b 5f50 4154 4820 6973 2067 746b 2d33  TK_PATH is gtk-3
+00001980: 2e30 2061 6e64 2074 6865 6e20 6974 2073  .0 and then it s
+00001990: 686f 7773 206d 6520 7468 6973 2065 7272  hows me this err
+000019a0: 6f72 3a5c 725c 6e21 5b69 6d61 6765 5d28  or:\r\n![image](
+000019b0: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
+000019c0: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
+000019d0: 6e74 656e 742e 636f 6d2f 3632 3335 3437  ntent.com/623547
+000019e0: 3231 2f32 3239 3433 3530 3739 2d61 3835  21/229435079-a85
+000019f0: 6335 6666 312d 6138 6333 2d34 3837 302d  c5ff1-a8c3-4870-
+00001a00: 3933 3430 2d62 6463 3934 3034 6535 3935  9340-bdc9404e595
+00001a10: 622e 706e 6729 5c72 5c6e 5c72 5c6e 5c72  b.png)\r\n\r\n\r
+00001a20: 5c6e 4920 7665 7269 6669 6564 2074 6861  \nI verified tha
+00001a30: 7420 7468 6520 696e 2060 2f75 7372 2f6c  t the in `/usr/l
+00001a40: 6962 2f78 3836 5f36 342d 6c69 6e75 782d  ib/x86_64-linux-
+00001a50: 676e 752f 6774 6b2d 332e 302f 6d6f 6475  gnu/gtk-3.0/modu
+00001a60: 6c65 7360 2069 733a 5c72 5c6e 5c72 5c6e  les` is:\r\n\r\n
+00001a70: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
+00001a80: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+00001a90: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001aa0: 6f6d 2f36 3233 3534 3732 312f 3232 3930  om/62354721/2290
+00001ab0: 3539 3138 382d 3431 3731 6637 3330 2d64  59188-4171f730-d
+00001ac0: 3264 392d 3462 3663 2d62 3130 332d 3434  2d9-4b6c-b103-44
+00001ad0: 3763 6138 6565 3732 3762 2e70 6e67 295c  7ca8ee727b.png)\
+00001ae0: 725c 6e5c 725c 6e57 6f75 6c64 2061 7070  r\n\r\nWould app
+00001af0: 7265 6369 6174 6520 746f 2073 6f6c 7665  reciate to solve
+00001b00: 2074 6869 7320 7761 726e 696e 6720 616e   this warning an
+00001b10: 6420 746f 2075 6e64 6572 7374 616e 6420  d to understand 
+00001b20: 7768 7920 7468 6520 2e73 6f20 6361 6e6e  why the .so cann
+00001b30: 6f74 2062 6520 6c6f 6164 6564 2e5c 725c  ot be loaded.\r\
+00001b40: 6e5c 725c 6e54 6861 6e6b 7320 696e 2061  n\r\nThanks in a
+00001b50: 6476 616e 6365 5c72 5c6e 5c72 5c6e 5c72  dvance\r\n\r\n\r
+00001b60: 5c6e 2a2a 5550 4441 5445 3a2a 2a20 7468  \n**UPDATE:** th
+00001b70: 6520 6578 616d 706c 6520 636f 6465 2063  e example code c
+00001b80: 616e 2062 6520 6578 6563 7574 6564 2077  an be executed w
+00001b90: 6974 686f 7574 2077 6172 6e69 6e67 7320  ithout warnings 
+00001ba0: 696e 2074 6865 206e 6f72 6d61 6c20 676e  in the normal gn
+00001bb0: 6f6d 6520 7465 726d 696e 616c 2c20 6275  ome terminal, bu
+00001bc0: 7420 5653 436f 6465 2073 6565 6d73 2074  t VSCode seems t
+00001bd0: 6f20 6861 6265 2070 726f 626c 656d 7320  o habe problems 
+00001be0: 746f 2066 696e 6420 7468 6520 7370 6563  to find the spec
+00001bf0: 6966 6963 206c 6962 7261 7269 6573 2c20  ific libraries, 
+00001c00: 736f 2069 7427 7320 6465 6669 6e69 7465  so it's definite
+00001c10: 6c79 205f 5653 436f 6465 5f2e 222c 0d0a  ly _VSCode_.",..
+00001c20: 2020 2263 6c6f 7365 645f 6279 223a 207b    "closed_by": {
+00001c30: 0d0a 2020 2020 226c 6f67 696e 223a 2022  ..    "login": "
+00001c40: 6465 6570 616b 3135 3536 222c 0d0a 2020  deepak1556",..  
+00001c50: 2020 2269 6422 3a20 3936 3433 3836 2c0d    "id": 964386,.
+00001c60: 0a20 2020 2022 6e6f 6465 5f69 6422 3a20  .    "node_id": 
+00001c70: 224d 4451 3656 584e 6c63 6a6b 324e 444d  "MDQ6VXNlcjk2NDM
+00001c80: 344e 673d 3d22 2c0d 0a20 2020 2022 6176  4Ng==",..    "av
+00001c90: 6174 6172 5f75 726c 223a 2022 6874 7470  atar_url": "http
+00001ca0: 733a 2f2f 6176 6174 6172 732e 6769 7468  s://avatars.gith
+00001cb0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00001cc0: 6d2f 752f 3936 3433 3836 3f76 3d34 222c  m/u/964386?v=4",
+00001cd0: 0d0a 2020 2020 2267 7261 7661 7461 725f  ..    "gravatar_
+00001ce0: 6964 223a 2022 222c 0d0a 2020 2020 2275  id": "",..    "u
+00001cf0: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
+00001d00: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
+00001d10: 7273 2f64 6565 7061 6b31 3535 3622 2c0d  rs/deepak1556",.
+00001d20: 0a20 2020 2022 6874 6d6c 5f75 726c 223a  .    "html_url":
+00001d30: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00001d40: 2e63 6f6d 2f64 6565 7061 6b31 3535 3622  .com/deepak1556"
+00001d50: 2c0d 0a20 2020 2022 666f 6c6c 6f77 6572  ,..    "follower
+00001d60: 735f 7572 6c22 3a20 2268 7474 7073 3a2f  s_url": "https:/
+00001d70: 2f61 7069 2e67 6974 6875 622e 636f 6d2f  /api.github.com/
+00001d80: 7573 6572 732f 6465 6570 616b 3135 3536  users/deepak1556
+00001d90: 2f66 6f6c 6c6f 7765 7273 222c 0d0a 2020  /followers",..  
+00001da0: 2020 2266 6f6c 6c6f 7769 6e67 5f75 726c    "following_url
+00001db0: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
+00001dc0: 6769 7468 7562 2e63 6f6d 2f75 7365 7273  github.com/users
+00001dd0: 2f64 6565 7061 6b31 3535 362f 666f 6c6c  /deepak1556/foll
+00001de0: 6f77 696e 677b 2f6f 7468 6572 5f75 7365  owing{/other_use
+00001df0: 727d 222c 0d0a 2020 2020 2267 6973 7473  r}",..    "gists
+00001e00: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
+00001e10: 6170 692e 6769 7468 7562 2e63 6f6d 2f75  api.github.com/u
+00001e20: 7365 7273 2f64 6565 7061 6b31 3535 362f  sers/deepak1556/
+00001e30: 6769 7374 737b 2f67 6973 745f 6964 7d22  gists{/gist_id}"
+00001e40: 2c0d 0a20 2020 2022 7374 6172 7265 645f  ,..    "starred_
+00001e50: 7572 6c22 3a20 2268 7474 7073 3a2f 2f61  url": "https://a
+00001e60: 7069 2e67 6974 6875 622e 636f 6d2f 7573  pi.github.com/us
+00001e70: 6572 732f 6465 6570 616b 3135 3536 2f73  ers/deepak1556/s
+00001e80: 7461 7272 6564 7b2f 6f77 6e65 727d 7b2f  tarred{/owner}{/
+00001e90: 7265 706f 7d22 2c0d 0a20 2020 2022 7375  repo}",..    "su
+00001ea0: 6273 6372 6970 7469 6f6e 735f 7572 6c22  bscriptions_url"
+00001eb0: 3a20 2268 7474 7073 3a2f 2f61 7069 2e67  : "https://api.g
+00001ec0: 6974 6875 622e 636f 6d2f 7573 6572 732f  ithub.com/users/
+00001ed0: 6465 6570 616b 3135 3536 2f73 7562 7363  deepak1556/subsc
+00001ee0: 7269 7074 696f 6e73 222c 0d0a 2020 2020  riptions",..    
+00001ef0: 226f 7267 616e 697a 6174 696f 6e73 5f75  "organizations_u
+00001f00: 726c 223a 2022 6874 7470 733a 2f2f 6170  rl": "https://ap
+00001f10: 692e 6769 7468 7562 2e63 6f6d 2f75 7365  i.github.com/use
+00001f20: 7273 2f64 6565 7061 6b31 3535 362f 6f72  rs/deepak1556/or
+00001f30: 6773 222c 0d0a 2020 2020 2272 6570 6f73  gs",..    "repos
+00001f40: 5f75 726c 223a 2022 6874 7470 733a 2f2f  _url": "https://
+00001f50: 6170 692e 6769 7468 7562 2e63 6f6d 2f75  api.github.com/u
+00001f60: 7365 7273 2f64 6565 7061 6b31 3535 362f  sers/deepak1556/
+00001f70: 7265 706f 7322 2c0d 0a20 2020 2022 6576  repos",..    "ev
+00001f80: 656e 7473 5f75 726c 223a 2022 6874 7470  ents_url": "http
+00001f90: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+00001fa0: 6f6d 2f75 7365 7273 2f64 6565 7061 6b31  om/users/deepak1
+00001fb0: 3535 362f 6576 656e 7473 7b2f 7072 6976  556/events{/priv
+00001fc0: 6163 797d 222c 0d0a 2020 2020 2272 6563  acy}",..    "rec
+00001fd0: 6569 7665 645f 6576 656e 7473 5f75 726c  eived_events_url
+00001fe0: 223a 2022 6874 7470 733a 2f2f 6170 692e  ": "https://api.
+00001ff0: 6769 7468 7562 2e63 6f6d 2f75 7365 7273  github.com/users
+00002000: 2f64 6565 7061 6b31 3535 362f 7265 6365  /deepak1556/rece
+00002010: 6976 6564 5f65 7665 6e74 7322 2c0d 0a20  ived_events",.. 
+00002020: 2020 2022 7479 7065 223a 2022 5573 6572     "type": "User
+00002030: 222c 0d0a 2020 2020 2273 6974 655f 6164  ",..    "site_ad
+00002040: 6d69 6e22 3a20 6661 6c73 650d 0a20 207d  min": false..  }
+00002050: 2c0d 0a20 2022 7265 6163 7469 6f6e 7322  ,..  "reactions"
+00002060: 3a20 7b0d 0a20 2020 2022 7572 6c22 3a20  : {..    "url": 
+00002070: 2268 7474 7073 3a2f 2f61 7069 2e67 6974  "https://api.git
+00002080: 6875 622e 636f 6d2f 7265 706f 732f 6d69  hub.com/repos/mi
+00002090: 6372 6f73 6f66 742f 7673 636f 6465 2f69  crosoft/vscode/i
+000020a0: 7373 7565 732f 3137 3930 3836 2f72 6561  ssues/179086/rea
+000020b0: 6374 696f 6e73 222c 0d0a 2020 2020 2274  ctions",..    "t
+000020c0: 6f74 616c 5f63 6f75 6e74 223a 2030 2c0d  otal_count": 0,.
+000020d0: 0a20 2020 2022 2b31 223a 2030 2c0d 0a20  .    "+1": 0,.. 
+000020e0: 2020 2022 2d31 223a 2030 2c0d 0a20 2020     "-1": 0,..   
+000020f0: 2022 6c61 7567 6822 3a20 302c 0d0a 2020   "laugh": 0,..  
+00002100: 2020 2268 6f6f 7261 7922 3a20 302c 0d0a    "hooray": 0,..
+00002110: 2020 2020 2263 6f6e 6675 7365 6422 3a20      "confused": 
+00002120: 302c 0d0a 2020 2020 2268 6561 7274 223a  0,..    "heart":
+00002130: 2030 2c0d 0a20 2020 2022 726f 636b 6574   0,..    "rocket
+00002140: 223a 2030 2c0d 0a20 2020 2022 6579 6573  ": 0,..    "eyes
+00002150: 223a 2030 0d0a 2020 7d2c 0d0a 2020 2274  ": 0..  },..  "t
+00002160: 696d 656c 696e 655f 7572 6c22 3a20 2268  imeline_url": "h
+00002170: 7474 7073 3a2f 2f61 7069 2e67 6974 6875  ttps://api.githu
+00002180: 622e 636f 6d2f 7265 706f 732f 6d69 6372  b.com/repos/micr
+00002190: 6f73 6f66 742f 7673 636f 6465 2f69 7373  osoft/vscode/iss
+000021a0: 7565 732f 3137 3930 3836 2f74 696d 656c  ues/179086/timel
+000021b0: 696e 6522 2c0d 0a20 2022 7374 6174 655f  ine",..  "state_
+000021c0: 7265 6173 6f6e 223a 2022 7265 6f70 656e  reason": "reopen
+000021d0: 6564 220d 0a7d                           ed"..}
```

### Comparing `serpyco_rs-1.7.1/bench/compare/github_issue/mashumaro.py` & `serpyco_rs-1.8.0/bench/compare/github_issue/mashumaro.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from dataclasses import dataclass, field
-from datetime import datetime
-from enum import Enum
-from typing import Optional, Union, Any
-
-from mashumaro import DataClassDictMixin, field_options, pass_through
-from mashumaro.config import BaseConfig
-
-from ._utils import get_dataclass_args
-
-
-class BaseModel(DataClassDictMixin):
-    class Config(BaseConfig):
-        lazy_compilation = True
-        serialize_by_alias = True
-        serialization_strategy = {
-            str: {'deserialize': str, 'serialize': pass_through},
-            int: {'serialize': pass_through},
-        }
-
-
-class IssueState(Enum):
-    OPEN = 'open'
-    CLOSED = 'closed'
-
-
-class MilestoneState(Enum):
-    OPEN = 'open'
-    CLOSED = 'closed'
-
-
-class IssueStateReason(Enum):
-    COMPLETED = 'completed'
-    REOPENED = 'reopened'
-    NOT_PLANNED = 'not_planned'
-
-
-class AuthorAssociation(Enum):
-    COLLABORATOR = 'COLLABORATOR'
-    CONTRIBUTOR = 'CONTRIBUTOR'
-    FIRST_TIMER = 'FIRST_TIMER'
-    FIRST_TIME_CONTRIBUTOR = 'FIRST_TIME_CONTRIBUTOR'
-    MANNEQUIN = 'MANNEQUIN'
-    MEMBER = 'MEMBER'
-    NONE = 'NONE'
-    OWNER = 'OWNER'
-
-
-@dataclass(**get_dataclass_args())
-class User(BaseModel):
-    login: str
-    id: int
-    node_id: str
-    avatar_url: str
-    gravatar_id: Optional[str]
-    url: str
-    html_url: str
-    followers_url: str
-    following_url: str
-    gists_url: str
-    starred_url: str
-    subscriptions_url: str
-    organizations_url: str
-    repos_url: str
-    events_url: str
-    received_events_url: str
-    type: str
-    site_admin: bool
-    name: Optional[str] = None
-    email: Optional[str] = None
-    starred_at: Optional[datetime] = None
-
-
-@dataclass(**get_dataclass_args())
-class IssueLabel(BaseModel):
-    id: int
-    node_id: str
-    url: str
-    name: str
-    description: Optional[str]
-    color: Optional[str]
-    default: bool
-
-
-@dataclass(**get_dataclass_args())
-class Milestone(BaseModel):
-    url: str
-    html_url: str
-    labels_url: str
-    id: int
-    node_id: str
-    number: int
-    title: str
-    description: Optional[str]
-    creator: Optional[User]
-    open_issues: int
-    closed_issues: int
-    created_at: datetime
-    updated_at: datetime
-    closed_at: Optional[datetime]
-    due_on: Optional[datetime]
-    state: MilestoneState = MilestoneState.OPEN
-
-
-@dataclass(**get_dataclass_args())
-class Reactions(BaseModel):
-    url: str
-    total_count: int
-    plus_one: int = field(metadata=field_options(alias='+1'))
-    minus_one: int = field(metadata=field_options(alias='-1'))
-    laugh: int
-    confused: int
-    heart: int
-    hooray: int
-    eyes: int
-    rocket: int
-
-
-@dataclass(**get_dataclass_args())
-class Issue(BaseModel):
-    id: int
-    node_id: str
-    url: str
-    repository_url: str
-    labels_url: str
-    comments_url: str
-    events_url: str
-    html_url: str
-    number: int
-    state: IssueState
-    state_reason: Optional[IssueStateReason]
-    title: str
-    body: Optional[str]
-    user: Optional[User]
-    labels: list[Union[IssueLabel, str]]
-    assignee: Optional[User]
-    assignees: Optional[list[User]]
-    milestone: Optional[Milestone]
-    locked: bool
-    active_lock_reason: Optional[str]
-    comments: int
-    closed_at: Optional[datetime]
-    created_at: datetime
-    updated_at: datetime
-    closed_by: Optional[User]
-    author_association: AuthorAssociation
-    draft: bool = False
-    body_html: Optional[str] = None
-    body_text: Optional[str] = None
-    timeline_url: Optional[str] = None
-    reactions: Optional[Reactions] = None
-
-
-def load(data: dict[str, Any]) -> Issue:
-    return Issue.from_dict(data)
-
-
-def dump(obj: Issue) -> dict[str, Any]:
-    return obj.to_dict()
+from dataclasses import dataclass, field
+from datetime import datetime
+from enum import Enum
+from typing import Optional, Union, Any
+
+from mashumaro import DataClassDictMixin, field_options, pass_through
+from mashumaro.config import BaseConfig
+
+from ._utils import get_dataclass_args
+
+
+class BaseModel(DataClassDictMixin):
+    class Config(BaseConfig):
+        lazy_compilation = True
+        serialize_by_alias = True
+        serialization_strategy = {
+            str: {'deserialize': str, 'serialize': pass_through},
+            int: {'serialize': pass_through},
+        }
+
+
+class IssueState(Enum):
+    OPEN = 'open'
+    CLOSED = 'closed'
+
+
+class MilestoneState(Enum):
+    OPEN = 'open'
+    CLOSED = 'closed'
+
+
+class IssueStateReason(Enum):
+    COMPLETED = 'completed'
+    REOPENED = 'reopened'
+    NOT_PLANNED = 'not_planned'
+
+
+class AuthorAssociation(Enum):
+    COLLABORATOR = 'COLLABORATOR'
+    CONTRIBUTOR = 'CONTRIBUTOR'
+    FIRST_TIMER = 'FIRST_TIMER'
+    FIRST_TIME_CONTRIBUTOR = 'FIRST_TIME_CONTRIBUTOR'
+    MANNEQUIN = 'MANNEQUIN'
+    MEMBER = 'MEMBER'
+    NONE = 'NONE'
+    OWNER = 'OWNER'
+
+
+@dataclass(**get_dataclass_args())
+class User(BaseModel):
+    login: str
+    id: int
+    node_id: str
+    avatar_url: str
+    gravatar_id: Optional[str]
+    url: str
+    html_url: str
+    followers_url: str
+    following_url: str
+    gists_url: str
+    starred_url: str
+    subscriptions_url: str
+    organizations_url: str
+    repos_url: str
+    events_url: str
+    received_events_url: str
+    type: str
+    site_admin: bool
+    name: Optional[str] = None
+    email: Optional[str] = None
+    starred_at: Optional[datetime] = None
+
+
+@dataclass(**get_dataclass_args())
+class IssueLabel(BaseModel):
+    id: int
+    node_id: str
+    url: str
+    name: str
+    description: Optional[str]
+    color: Optional[str]
+    default: bool
+
+
+@dataclass(**get_dataclass_args())
+class Milestone(BaseModel):
+    url: str
+    html_url: str
+    labels_url: str
+    id: int
+    node_id: str
+    number: int
+    title: str
+    description: Optional[str]
+    creator: Optional[User]
+    open_issues: int
+    closed_issues: int
+    created_at: datetime
+    updated_at: datetime
+    closed_at: Optional[datetime]
+    due_on: Optional[datetime]
+    state: MilestoneState = MilestoneState.OPEN
+
+
+@dataclass(**get_dataclass_args())
+class Reactions(BaseModel):
+    url: str
+    total_count: int
+    plus_one: int = field(metadata=field_options(alias='+1'))
+    minus_one: int = field(metadata=field_options(alias='-1'))
+    laugh: int
+    confused: int
+    heart: int
+    hooray: int
+    eyes: int
+    rocket: int
+
+
+@dataclass(**get_dataclass_args())
+class Issue(BaseModel):
+    id: int
+    node_id: str
+    url: str
+    repository_url: str
+    labels_url: str
+    comments_url: str
+    events_url: str
+    html_url: str
+    number: int
+    state: IssueState
+    state_reason: Optional[IssueStateReason]
+    title: str
+    body: Optional[str]
+    user: Optional[User]
+    labels: list[Union[IssueLabel, str]]
+    assignee: Optional[User]
+    assignees: Optional[list[User]]
+    milestone: Optional[Milestone]
+    locked: bool
+    active_lock_reason: Optional[str]
+    comments: int
+    closed_at: Optional[datetime]
+    created_at: datetime
+    updated_at: datetime
+    closed_by: Optional[User]
+    author_association: AuthorAssociation
+    draft: bool = False
+    body_html: Optional[str] = None
+    body_text: Optional[str] = None
+    timeline_url: Optional[str] = None
+    reactions: Optional[Reactions] = None
+
+
+def load(data: dict[str, Any]) -> Issue:
+    return Issue.from_dict(data)
+
+
+def dump(obj: Issue) -> dict[str, Any]:
+    return obj.to_dict()
```

### Comparing `serpyco_rs-1.7.1/bench/compare/github_issue/serpyco_rs.py` & `serpyco_rs-1.8.0/bench/compare/github_issue/serpyco_rs.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-from dataclasses import dataclass
-from datetime import datetime
-from enum import Enum
-from typing import Any, Union
-from typing import Optional, Annotated
-
-from serpyco_rs.metadata import Alias
-import serpyco_rs
-
-from ._utils import get_dataclass_args
-
-
-class IssueState(Enum):
-    OPEN = 'open'
-    CLOSED = 'closed'
-
-
-class MilestoneState(Enum):
-    OPEN = 'open'
-    CLOSED = 'closed'
-
-
-class IssueStateReason(Enum):
-    COMPLETED = 'completed'
-    REOPENED = 'reopened'
-    NOT_PLANNED = 'not_planned'
-
-
-class AuthorAssociation(Enum):
-    COLLABORATOR = 'COLLABORATOR'
-    CONTRIBUTOR = 'CONTRIBUTOR'
-    FIRST_TIMER = 'FIRST_TIMER'
-    FIRST_TIME_CONTRIBUTOR = 'FIRST_TIME_CONTRIBUTOR'
-    MANNEQUIN = 'MANNEQUIN'
-    MEMBER = 'MEMBER'
-    NONE = 'NONE'
-    OWNER = 'OWNER'
-
-
-@dataclass(**get_dataclass_args())
-class User:
-    login: str
-    id: int
-    node_id: str
-    avatar_url: str
-    gravatar_id: Optional[str]
-    url: str
-    html_url: str
-    followers_url: str
-    following_url: str
-    gists_url: str
-    starred_url: str
-    subscriptions_url: str
-    organizations_url: str
-    repos_url: str
-    events_url: str
-    received_events_url: str
-    type: str
-    site_admin: bool
-    name: Optional[str] = None
-    email: Optional[str] = None
-    starred_at: Optional[datetime] = None
-
-
-@dataclass(**get_dataclass_args())
-class IssueLabel:
-    id: int
-    node_id: str
-    url: str
-    name: str
-    description: Optional[str]
-    color: Optional[str]
-    default: bool
-
-
-@dataclass(**get_dataclass_args())
-class Milestone:
-    url: str
-    html_url: str
-    labels_url: str
-    id: int
-    node_id: str
-    number: int
-    title: str
-    description: Optional[str]
-    creator: Optional[User]
-    open_issues: int
-    closed_issues: int
-    created_at: datetime
-    updated_at: datetime
-    closed_at: Optional[datetime]
-    due_on: Optional[datetime]
-    state: MilestoneState = MilestoneState.OPEN
-
-
-@dataclass(**get_dataclass_args())
-class Reactions:
-    url: str
-    total_count: int
-    plus_one: Annotated[int, Alias('+1')]
-    minus_one: Annotated[int, Alias('-1')]
-    laugh: int
-    confused: int
-    heart: int
-    hooray: int
-    eyes: int
-    rocket: int
-
-
-@dataclass(**get_dataclass_args())
-class Issue:
-    id: int
-    node_id: str
-    url: str
-    repository_url: str
-    labels_url: str
-    comments_url: str
-    events_url: str
-    html_url: str
-    number: int
-    state: IssueState
-    state_reason: Optional[IssueStateReason]
-    title: str
-    body: Optional[str]
-    user: Optional[User]
-    labels: list[Union[IssueLabel, str]]
-    assignee: Optional[User]
-    assignees: Optional[list[User]]
-    milestone: Optional[Milestone]
-    locked: bool
-    active_lock_reason: Optional[str]
-    comments: int
-    closed_at: Optional[datetime]
-    created_at: datetime
-    updated_at: datetime
-    closed_by: Optional[User]
-    author_association: AuthorAssociation
-    draft: bool = False
-    body_html: Optional[str] = None
-    body_text: Optional[str] = None
-    timeline_url: Optional[str] = None
-    reactions: Optional[Reactions] = None
-
-
-_serializer = serpyco_rs.Serializer(Issue)
-
-
-def load(data: dict[str, Any]) -> Issue:
-    return _serializer.load(data)
-
-
-def dump(obj: Issue) -> dict[str, Any]:
-    return _serializer.dump(obj)
+from dataclasses import dataclass
+from datetime import datetime
+from enum import Enum
+from typing import Any, Union
+from typing import Optional, Annotated
+
+from serpyco_rs.metadata import Alias
+import serpyco_rs
+
+from ._utils import get_dataclass_args
+
+
+class IssueState(Enum):
+    OPEN = 'open'
+    CLOSED = 'closed'
+
+
+class MilestoneState(Enum):
+    OPEN = 'open'
+    CLOSED = 'closed'
+
+
+class IssueStateReason(Enum):
+    COMPLETED = 'completed'
+    REOPENED = 'reopened'
+    NOT_PLANNED = 'not_planned'
+
+
+class AuthorAssociation(Enum):
+    COLLABORATOR = 'COLLABORATOR'
+    CONTRIBUTOR = 'CONTRIBUTOR'
+    FIRST_TIMER = 'FIRST_TIMER'
+    FIRST_TIME_CONTRIBUTOR = 'FIRST_TIME_CONTRIBUTOR'
+    MANNEQUIN = 'MANNEQUIN'
+    MEMBER = 'MEMBER'
+    NONE = 'NONE'
+    OWNER = 'OWNER'
+
+
+@dataclass(**get_dataclass_args())
+class User:
+    login: str
+    id: int
+    node_id: str
+    avatar_url: str
+    gravatar_id: Optional[str]
+    url: str
+    html_url: str
+    followers_url: str
+    following_url: str
+    gists_url: str
+    starred_url: str
+    subscriptions_url: str
+    organizations_url: str
+    repos_url: str
+    events_url: str
+    received_events_url: str
+    type: str
+    site_admin: bool
+    name: Optional[str] = None
+    email: Optional[str] = None
+    starred_at: Optional[datetime] = None
+
+
+@dataclass(**get_dataclass_args())
+class IssueLabel:
+    id: int
+    node_id: str
+    url: str
+    name: str
+    description: Optional[str]
+    color: Optional[str]
+    default: bool
+
+
+@dataclass(**get_dataclass_args())
+class Milestone:
+    url: str
+    html_url: str
+    labels_url: str
+    id: int
+    node_id: str
+    number: int
+    title: str
+    description: Optional[str]
+    creator: Optional[User]
+    open_issues: int
+    closed_issues: int
+    created_at: datetime
+    updated_at: datetime
+    closed_at: Optional[datetime]
+    due_on: Optional[datetime]
+    state: MilestoneState = MilestoneState.OPEN
+
+
+@dataclass(**get_dataclass_args())
+class Reactions:
+    url: str
+    total_count: int
+    plus_one: Annotated[int, Alias('+1')]
+    minus_one: Annotated[int, Alias('-1')]
+    laugh: int
+    confused: int
+    heart: int
+    hooray: int
+    eyes: int
+    rocket: int
+
+
+@dataclass(**get_dataclass_args())
+class Issue:
+    id: int
+    node_id: str
+    url: str
+    repository_url: str
+    labels_url: str
+    comments_url: str
+    events_url: str
+    html_url: str
+    number: int
+    state: IssueState
+    state_reason: Optional[IssueStateReason]
+    title: str
+    body: Optional[str]
+    user: Optional[User]
+    labels: list[Union[IssueLabel, str]]
+    assignee: Optional[User]
+    assignees: Optional[list[User]]
+    milestone: Optional[Milestone]
+    locked: bool
+    active_lock_reason: Optional[str]
+    comments: int
+    closed_at: Optional[datetime]
+    created_at: datetime
+    updated_at: datetime
+    closed_by: Optional[User]
+    author_association: AuthorAssociation
+    draft: bool = False
+    body_html: Optional[str] = None
+    body_text: Optional[str] = None
+    timeline_url: Optional[str] = None
+    reactions: Optional[Reactions] = None
+
+
+_serializer = serpyco_rs.Serializer(Issue)
+
+
+def load(data: dict[str, Any]) -> Issue:
+    return _serializer.load(data)
+
+
+def dump(obj: Issue) -> dict[str, Any]:
+    return _serializer.dump(obj)
```

### Comparing `serpyco_rs-1.7.1/bench/compare/graph.py` & `serpyco_rs-1.8.0/bench/compare/graph.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import collections
-import io
-import json
-import os
-
-from tabulate import tabulate
-
-
-LIBRARIES = (
-    'serpyco_rs',
-    'serpyco',
-    'mashumaro',
-    'pydantic',
-    'marshmallow',
-)
-
-
-def aggregate():
-    benchmarks_dir = os.path.join('.benchmarks', os.listdir('.benchmarks')[0])
-    res = collections.defaultdict(dict)
-    for filename in os.listdir(benchmarks_dir):
-        with open(os.path.join(benchmarks_dir, filename)) as fileh:
-            data = json.loads(fileh.read())
-
-        for each in data['benchmarks']:
-            res[each['group']][each['extra_info']['lib']] = {
-                'data': [val * 1000 for val in each['stats']['data']],
-                'median': each['stats']['median'] * 1000,
-                'ops': each['stats']['ops'],
-                'correct': each['extra_info']['correct'],
-            }
-    return res
-
-
-def tab(obj):
-    buf = io.StringIO()
-    headers = (
-        'Library',
-        'Median latency (milliseconds)',
-        'Operations per second',
-        'Relative (latency)',
-    )
-    for group, val in sorted(obj.items(), reverse=True):
-        buf.write('\n' + '#### ' + group + '\n\n')
-        table = []
-        for lib in LIBRARIES:
-            correct = val[lib]['correct']
-            table.append(
-                [
-                    lib,
-                    val[lib]['median'] if correct else None,
-                    '%.1f' % val[lib]['ops'] if correct else None,
-                    0,
-                ]
-            )
-        baseline = table[0][1]
-        for each in table:
-            each[3] = '%.2f' % (each[1] / baseline) if isinstance(each[1], float) else None
-            each[1] = '%.2f' % each[1] if isinstance(each[1], float) else None
-        buf.write(tabulate(table, headers, tablefmt='github') + '\n')
-
-    print(buf.getvalue())
-
-
-tab(aggregate())
+import collections
+import io
+import json
+import os
+
+from tabulate import tabulate
+
+
+LIBRARIES = (
+    'serpyco_rs',
+    'serpyco',
+    'mashumaro',
+    'pydantic',
+    'marshmallow',
+)
+
+
+def aggregate():
+    benchmarks_dir = os.path.join('.benchmarks', os.listdir('.benchmarks')[0])
+    res = collections.defaultdict(dict)
+    for filename in os.listdir(benchmarks_dir):
+        with open(os.path.join(benchmarks_dir, filename)) as fileh:
+            data = json.loads(fileh.read())
+
+        for each in data['benchmarks']:
+            res[each['group']][each['extra_info']['lib']] = {
+                'data': [val * 1000 for val in each['stats']['data']],
+                'median': each['stats']['median'] * 1000,
+                'ops': each['stats']['ops'],
+                'correct': each['extra_info']['correct'],
+            }
+    return res
+
+
+def tab(obj):
+    buf = io.StringIO()
+    headers = (
+        'Library',
+        'Median latency (milliseconds)',
+        'Operations per second',
+        'Relative (latency)',
+    )
+    for group, val in sorted(obj.items(), reverse=True):
+        buf.write('\n' + '#### ' + group + '\n\n')
+        table = []
+        for lib in LIBRARIES:
+            correct = val[lib]['correct']
+            table.append(
+                [
+                    lib,
+                    val[lib]['median'] if correct else None,
+                    '%.1f' % val[lib]['ops'] if correct else None,
+                    0,
+                ]
+            )
+        baseline = table[0][1]
+        for each in table:
+            each[3] = '%.2f' % (each[1] / baseline) if isinstance(each[1], float) else None
+            each[1] = '%.2f' % each[1] if isinstance(each[1], float) else None
+        buf.write(tabulate(table, headers, tablefmt='github') + '\n')
+
+    print(buf.getvalue())
+
+
+tab(aggregate())
```

### Comparing `serpyco_rs-1.7.1/bench/compare/libs/base.py` & `serpyco_rs-1.8.0/bench/compare/libs/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from dataclasses import dataclass
-from typing import Optional
-
-
-@dataclass
-class Nested:
-    """
-    A nested type for Dataclass
-    """
-
-    name: str
-
-
-@dataclass
-class Dataclass:
-    """
-    A Dataclass class
-    """
-
-    name: str
-    value: int
-    f: float
-    b: bool
-    nest: list[Nested]
-    many: list[int]
-    option: Optional[str] = None
-
-
-def make_test_object(cls, nested_cls):
-    return cls(
-        name='Foo',
-        value=42,
-        f=12.34,
-        b=True,
-        nest=[nested_cls(name=f'Bar_{index}') for index in range(0, 1000)],
-        many=[1, 2, 3],
-    )
-
-
-test_object = make_test_object(Dataclass, Nested)
+from dataclasses import dataclass
+from typing import Optional
+
+
+@dataclass
+class Nested:
+    """
+    A nested type for Dataclass
+    """
+
+    name: str
+
+
+@dataclass
+class Dataclass:
+    """
+    A Dataclass class
+    """
+
+    name: str
+    value: int
+    f: float
+    b: bool
+    nest: list[Nested]
+    many: list[int]
+    option: Optional[str] = None
+
+
+def make_test_object(cls, nested_cls):
+    return cls(
+        name='Foo',
+        value=42,
+        f=12.34,
+        b=True,
+        nest=[nested_cls(name=f'Bar_{index}') for index in range(0, 1000)],
+        many=[1, 2, 3],
+    )
+
+
+test_object = make_test_object(Dataclass, Nested)
```

### Comparing `serpyco_rs-1.7.1/bench/compare/test_benchmarks.py` & `serpyco_rs-1.8.0/bench/compare/test_benchmarks.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import pytest
-
-from .libs import marshmallow, mashumaro, pydantic, serpyco, serpyco_rs
-
-serializers = {
-    'serpyco_rs': serpyco_rs,
-    'serpyco': serpyco,
-    'pydantic': pydantic,
-    'marshmallow': marshmallow,
-    'mashumaro': mashumaro,
-}
-
-
-@pytest.mark.parametrize('lib', serializers.keys())
-def test_dump(bench_or_check_refcount, lib):
-    serializer = serializers[lib]
-    serializer.dump(serializer.test_object)  # warmup
-
-    bench_or_check_refcount.group = 'dump'
-    bench_or_check_refcount.extra_info['lib'] = lib
-    bench_or_check_refcount.extra_info['correct'] = (
-        serializer.load(serializer.dump(serializer.test_object)) == serializer.test_object
-    )
-    if lib in {'serpyco', 'pydantic'}:
-        bench_or_check_refcount.skip_refcount = True
-    bench_or_check_refcount(serializer.dump, serializer.test_object)
-
-
-@pytest.mark.parametrize('lib', serializers.keys())
-def test_load_validate(bench_or_check_refcount, lib):
-    serializer = serializers[lib]
-    test_dict = serializer.dump(serializer.test_object)
-    serializer.load(test_dict)  # warmup
-
-    bench_or_check_refcount.group = 'load with validate'
-    bench_or_check_refcount.extra_info['lib'] = lib
-    bench_or_check_refcount.extra_info['correct'] = (
-        serializer.load(serializer.dump(serializer.test_object)) == serializer.test_object
-    )
-    if lib in {'serpyco', 'pydantic'}:
-        bench_or_check_refcount.skip_refcount = True
-    bench_or_check_refcount(serializer.load, test_dict)
+import pytest
+
+from .libs import marshmallow, mashumaro, pydantic, serpyco, serpyco_rs
+
+serializers = {
+    'serpyco_rs': serpyco_rs,
+    'serpyco': serpyco,
+    'pydantic': pydantic,
+    'marshmallow': marshmallow,
+    'mashumaro': mashumaro,
+}
+
+
+@pytest.mark.parametrize('lib', serializers.keys())
+def test_dump(bench_or_check_refcount, lib):
+    serializer = serializers[lib]
+    serializer.dump(serializer.test_object)  # warmup
+
+    bench_or_check_refcount.group = 'dump'
+    bench_or_check_refcount.extra_info['lib'] = lib
+    bench_or_check_refcount.extra_info['correct'] = (
+        serializer.load(serializer.dump(serializer.test_object)) == serializer.test_object
+    )
+    if lib in {'serpyco', 'pydantic'}:
+        bench_or_check_refcount.skip_refcount = True
+    bench_or_check_refcount(serializer.dump, serializer.test_object)
+
+
+@pytest.mark.parametrize('lib', serializers.keys())
+def test_load_validate(bench_or_check_refcount, lib):
+    serializer = serializers[lib]
+    test_dict = serializer.dump(serializer.test_object)
+    serializer.load(test_dict)  # warmup
+
+    bench_or_check_refcount.group = 'load with validate'
+    bench_or_check_refcount.extra_info['lib'] = lib
+    bench_or_check_refcount.extra_info['correct'] = (
+        serializer.load(serializer.dump(serializer.test_object)) == serializer.test_object
+    )
+    if lib in {'serpyco', 'pydantic'}:
+        bench_or_check_refcount.skip_refcount = True
+    bench_or_check_refcount(serializer.load, test_dict)
```

### Comparing `serpyco_rs-1.7.1/bench/compare/test_github_issue.py` & `serpyco_rs-1.8.0/bench/compare/test_github_issue.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Any
-from pathlib import Path
-import orjson
-
-import pytest
-
-from .github_issue import mashumaro, serpyco_rs
-
-serializers = {
-    'serpyco_rs': serpyco_rs,
-    'mashumaro': mashumaro,
-}
-
-
-@pytest.fixture(scope='module')
-def data() -> dict[str, Any]:
-    path = Path(__file__).parent / 'github_issue/data.json'
-    return orjson.loads(path.read_text())
-
-
-@pytest.mark.parametrize('lib', serializers.keys())
-def test_dump_github_issue(bench_or_check_refcount, lib, data):
-    serializer = serializers[lib]
-    test_object = serializer.load(data)
-    serializer.dump(test_object)  # warmup
-
-    bench_or_check_refcount.group = 'dump github issue'
-    bench_or_check_refcount.extra_info['lib'] = lib
-    bench_or_check_refcount.extra_info['correct'] = serializer.load(serializer.dump(test_object)) == test_object
-    bench_or_check_refcount(serializer.dump, test_object)
-
-
-@pytest.mark.parametrize('lib', serializers.keys())
-def test_load_github_issue(bench_or_check_refcount, lib, data):
-    serializer = serializers[lib]
-    test_object = serializer.load(data)  # warmup
-
-    bench_or_check_refcount.group = 'load github issue'
-    bench_or_check_refcount.extra_info['lib'] = lib
-    bench_or_check_refcount.extra_info['correct'] = serializer.load(serializer.dump(test_object)) == test_object
-    bench_or_check_refcount(serializer.load, data)
+from typing import Any
+from pathlib import Path
+import orjson
+
+import pytest
+
+from .github_issue import mashumaro, serpyco_rs
+
+serializers = {
+    'serpyco_rs': serpyco_rs,
+    'mashumaro': mashumaro,
+}
+
+
+@pytest.fixture(scope='module')
+def data() -> dict[str, Any]:
+    path = Path(__file__).parent / 'github_issue/data.json'
+    return orjson.loads(path.read_text())
+
+
+@pytest.mark.parametrize('lib', serializers.keys())
+def test_dump_github_issue(bench_or_check_refcount, lib, data):
+    serializer = serializers[lib]
+    test_object = serializer.load(data)
+    serializer.dump(test_object)  # warmup
+
+    bench_or_check_refcount.group = 'dump github issue'
+    bench_or_check_refcount.extra_info['lib'] = lib
+    bench_or_check_refcount.extra_info['correct'] = serializer.load(serializer.dump(test_object)) == test_object
+    bench_or_check_refcount(serializer.dump, test_object)
+
+
+@pytest.mark.parametrize('lib', serializers.keys())
+def test_load_github_issue(bench_or_check_refcount, lib, data):
+    serializer = serializers[lib]
+    test_object = serializer.load(data)  # warmup
+
+    bench_or_check_refcount.group = 'load github issue'
+    bench_or_check_refcount.extra_info['lib'] = lib
+    bench_or_check_refcount.extra_info['correct'] = serializer.load(serializer.dump(test_object)) == test_object
+    bench_or_check_refcount(serializer.load, data)
```

### Comparing `serpyco_rs-1.7.1/bench/test_encoders.py` & `serpyco_rs-1.8.0/bench/test_encoders.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-import enum
-import uuid
-from dataclasses import dataclass
-from datetime import date, datetime, time
-from decimal import Decimal
-from typing import Optional, Union
-
-from serpyco_rs import Serializer
-from .utils import repeat
-
-
-def test_dump_simple_types(bench_or_check_refcount):
-    serializer = Serializer(float)
-    bench_or_check_refcount.group = 'simple_types'
-    bench_or_check_refcount(repeat(lambda: serializer.dump(1)))
-
-
-def test_load_simple_types(bench_or_check_refcount):
-    serializer = Serializer(int)
-    bench_or_check_refcount.group = 'simple_types'
-    bench_or_check_refcount(repeat(lambda: serializer.load(1)))
-
-
-def test_dump_optional(bench_or_check_refcount):
-    serializer = Serializer(Optional[int])
-
-    bench_or_check_refcount.group = 'optional'
-
-    def inner():
-        repeat(lambda: serializer.dump(1))
-        repeat(lambda: serializer.dump(None))
-
-    bench_or_check_refcount(inner)
-
-
-def test_load_optional(bench_or_check_refcount):
-    serializer = Serializer(Optional[int])
-
-    bench_or_check_refcount.group = 'optional'
-
-    def inner():
-        repeat(lambda: serializer.load(1))
-        repeat(lambda: serializer.load(None))
-
-    bench_or_check_refcount(inner)
-
-
-def test_dump_list_simple_types(bench_or_check_refcount):
-    serializer = Serializer(list[int])
-    bench_or_check_refcount.group = 'list'
-    data = list(range(1000))
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_list_simple_types(bench_or_check_refcount):
-    serializer = Serializer(list[int])
-    bench_or_check_refcount.group = 'list'
-    data = list(range(1000))
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_small_list_simple_types(bench_or_check_refcount):
-    serializer = Serializer(list[int])
-    bench_or_check_refcount.group = 'small_list'
-    data = list(range(10))
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_small_list_simple_types(bench_or_check_refcount):
-    serializer = Serializer(list[int])
-    bench_or_check_refcount.group = 'small_list'
-    data = list(range(10))
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_tuple_simple_types(bench_or_check_refcount):
-    serializer = Serializer(tuple[int, str, bool])
-    bench_or_check_refcount.group = 'tuple'
-    bench_or_check_refcount(repeat(lambda: serializer.dump((123, 'foo', True))))
-
-
-def test_load_tuple_simple_types(bench_or_check_refcount):
-    serializer = Serializer(tuple[int, str, bool])
-    bench_or_check_refcount.group = 'tuple'
-    bench_or_check_refcount(repeat(lambda: serializer.load((123, 'foo', True))))
-
-
-def test_dump_dict_simple_types(bench_or_check_refcount):
-    serializer = Serializer(dict[str, int])
-    bench_or_check_refcount.group = 'dict'
-    data = {str(i): i for i in range(1000)}
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_dump_dict_dataclass_value(bench_or_check_refcount):
-    @dataclass
-    class Foo:
-        foo: int
-
-    serializer = Serializer(dict[str, Foo])
-    bench_or_check_refcount.group = 'dict'
-    data = {str(i): Foo(i) for i in range(12)}
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data), count=100))
-
-
-def test_load_dict_simple_types(bench_or_check_refcount):
-    serializer = Serializer(dict[str, int])
-    bench_or_check_refcount.group = 'dict'
-    data = {str(i): i for i in range(1000)}
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_uuid(bench_or_check_refcount):
-    serializer = Serializer(uuid.UUID)
-    bench_or_check_refcount.group = 'uuid'
-    data = uuid.uuid4()
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_uuid(bench_or_check_refcount):
-    serializer = Serializer(uuid.UUID)
-    bench_or_check_refcount.group = 'uuid'
-    data = str(uuid.uuid4())
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_date(bench_or_check_refcount):
-    serializer = Serializer(date)
-    bench_or_check_refcount.group = 'date'
-    data = date.today()
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_date(bench_or_check_refcount):
-    serializer = Serializer(date)
-    bench_or_check_refcount.group = 'date'
-    data = date.today().isoformat()
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_time(bench_or_check_refcount):
-    serializer = Serializer(time)
-    bench_or_check_refcount.group = 'time'
-    data = datetime.now().time()
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_time(bench_or_check_refcount):
-    serializer = Serializer(time)
-    bench_or_check_refcount.group = 'time'
-    data = datetime.now().time().isoformat()
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_datetime(bench_or_check_refcount):
-    serializer = Serializer(datetime)
-    bench_or_check_refcount.group = 'datetime'
-    data = datetime.now()
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_datetime(bench_or_check_refcount):
-    serializer = Serializer(datetime)
-    bench_or_check_refcount.group = 'datetime'
-    data = datetime.now().isoformat()
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_decimal(bench_or_check_refcount):
-    serializer = Serializer(Decimal)
-    bench_or_check_refcount.group = 'decimal'
-    data = Decimal('1.3')
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_decimal(bench_or_check_refcount):
-    serializer = Serializer(Decimal)
-    bench_or_check_refcount.group = 'decimal'
-    data = '1.3'
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-class FooEunm(enum.Enum):
-    foo = 'foo'
-    bar = 'bar'
-
-
-def test_dump_enum(bench_or_check_refcount):
-    serializer = Serializer(FooEunm)
-    bench_or_check_refcount.group = 'enum'
-    data = FooEunm.bar
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_enum(bench_or_check_refcount):
-    serializer = Serializer(FooEunm)
-    bench_or_check_refcount.group = 'enum'
-    data = 'foo'
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-@dataclass
-class FooDataclass:
-    foo: int
-    bar: str
-
-
-def test_dump_dataclass(bench_or_check_refcount):
-    serializer = Serializer(FooDataclass)
-    bench_or_check_refcount.group = 'dataclass'
-    data = FooDataclass(foo=1, bar='2')
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_dataclass(bench_or_check_refcount):
-    serializer = Serializer(FooDataclass)
-    bench_or_check_refcount.group = 'dataclass'
-    data = {'foo': 1, 'bar': '2'}
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-@dataclass
-class Node:
-    value: str
-    next: Optional['Node'] = None
-
-
-@dataclass
-class Root:
-    head: Node
-
-
-def test_dump_recursive(bench_or_check_refcount):
-    serializer = Serializer(Root)
-    bench_or_check_refcount.group = 'recursive'
-    data = Root(
-        head=Node(
-            value='1',
-            next=Node(value='2'),
-        ),
-    )
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_recursive(bench_or_check_refcount):
-    serializer = Serializer(Root)
-    bench_or_check_refcount.group = 'recursive'
-    data = {'head': {'next': {'next': None, 'value': '2'}, 'value': '1'}}
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
-
-
-def test_dump_union(bench_or_check_refcount):
-    @dataclass
-    class Foo:
-        foo: int
-
-    serializer = Serializer(Union[int, Foo])
-    data = Foo(foo=1)
-    bench_or_check_refcount.group = 'union'
-    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
-
-
-def test_load_union(bench_or_check_refcount):
-    @dataclass
-    class Foo:
-        foo: int
-
-    serializer = Serializer(Union[int, Foo])
-    data = {'foo': 1}
-    bench_or_check_refcount.group = 'union'
-    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+import enum
+import uuid
+from dataclasses import dataclass
+from datetime import date, datetime, time
+from decimal import Decimal
+from typing import Optional, Union
+
+from serpyco_rs import Serializer
+from .utils import repeat
+
+
+def test_dump_simple_types(bench_or_check_refcount):
+    serializer = Serializer(float)
+    bench_or_check_refcount.group = 'simple_types'
+    bench_or_check_refcount(repeat(lambda: serializer.dump(1)))
+
+
+def test_load_simple_types(bench_or_check_refcount):
+    serializer = Serializer(int)
+    bench_or_check_refcount.group = 'simple_types'
+    bench_or_check_refcount(repeat(lambda: serializer.load(1)))
+
+
+def test_dump_optional(bench_or_check_refcount):
+    serializer = Serializer(Optional[int])
+
+    bench_or_check_refcount.group = 'optional'
+
+    def inner():
+        repeat(lambda: serializer.dump(1))
+        repeat(lambda: serializer.dump(None))
+
+    bench_or_check_refcount(inner)
+
+
+def test_load_optional(bench_or_check_refcount):
+    serializer = Serializer(Optional[int])
+
+    bench_or_check_refcount.group = 'optional'
+
+    def inner():
+        repeat(lambda: serializer.load(1))
+        repeat(lambda: serializer.load(None))
+
+    bench_or_check_refcount(inner)
+
+
+def test_dump_list_simple_types(bench_or_check_refcount):
+    serializer = Serializer(list[int])
+    bench_or_check_refcount.group = 'list'
+    data = list(range(1000))
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_list_simple_types(bench_or_check_refcount):
+    serializer = Serializer(list[int])
+    bench_or_check_refcount.group = 'list'
+    data = list(range(1000))
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_small_list_simple_types(bench_or_check_refcount):
+    serializer = Serializer(list[int])
+    bench_or_check_refcount.group = 'small_list'
+    data = list(range(10))
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_small_list_simple_types(bench_or_check_refcount):
+    serializer = Serializer(list[int])
+    bench_or_check_refcount.group = 'small_list'
+    data = list(range(10))
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_tuple_simple_types(bench_or_check_refcount):
+    serializer = Serializer(tuple[int, str, bool])
+    bench_or_check_refcount.group = 'tuple'
+    bench_or_check_refcount(repeat(lambda: serializer.dump((123, 'foo', True))))
+
+
+def test_load_tuple_simple_types(bench_or_check_refcount):
+    serializer = Serializer(tuple[int, str, bool])
+    bench_or_check_refcount.group = 'tuple'
+    bench_or_check_refcount(repeat(lambda: serializer.load((123, 'foo', True))))
+
+
+def test_dump_dict_simple_types(bench_or_check_refcount):
+    serializer = Serializer(dict[str, int])
+    bench_or_check_refcount.group = 'dict'
+    data = {str(i): i for i in range(1000)}
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_dump_dict_dataclass_value(bench_or_check_refcount):
+    @dataclass
+    class Foo:
+        foo: int
+
+    serializer = Serializer(dict[str, Foo])
+    bench_or_check_refcount.group = 'dict'
+    data = {str(i): Foo(i) for i in range(12)}
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data), count=100))
+
+
+def test_load_dict_simple_types(bench_or_check_refcount):
+    serializer = Serializer(dict[str, int])
+    bench_or_check_refcount.group = 'dict'
+    data = {str(i): i for i in range(1000)}
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_uuid(bench_or_check_refcount):
+    serializer = Serializer(uuid.UUID)
+    bench_or_check_refcount.group = 'uuid'
+    data = uuid.uuid4()
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_uuid(bench_or_check_refcount):
+    serializer = Serializer(uuid.UUID)
+    bench_or_check_refcount.group = 'uuid'
+    data = str(uuid.uuid4())
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_date(bench_or_check_refcount):
+    serializer = Serializer(date)
+    bench_or_check_refcount.group = 'date'
+    data = date.today()
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_date(bench_or_check_refcount):
+    serializer = Serializer(date)
+    bench_or_check_refcount.group = 'date'
+    data = date.today().isoformat()
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_time(bench_or_check_refcount):
+    serializer = Serializer(time)
+    bench_or_check_refcount.group = 'time'
+    data = datetime.now().time()
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_time(bench_or_check_refcount):
+    serializer = Serializer(time)
+    bench_or_check_refcount.group = 'time'
+    data = datetime.now().time().isoformat()
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_datetime(bench_or_check_refcount):
+    serializer = Serializer(datetime)
+    bench_or_check_refcount.group = 'datetime'
+    data = datetime.now()
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_datetime(bench_or_check_refcount):
+    serializer = Serializer(datetime)
+    bench_or_check_refcount.group = 'datetime'
+    data = datetime.now().isoformat()
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_decimal(bench_or_check_refcount):
+    serializer = Serializer(Decimal)
+    bench_or_check_refcount.group = 'decimal'
+    data = Decimal('1.3')
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_decimal(bench_or_check_refcount):
+    serializer = Serializer(Decimal)
+    bench_or_check_refcount.group = 'decimal'
+    data = '1.3'
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+class FooEunm(enum.Enum):
+    foo = 'foo'
+    bar = 'bar'
+
+
+def test_dump_enum(bench_or_check_refcount):
+    serializer = Serializer(FooEunm)
+    bench_or_check_refcount.group = 'enum'
+    data = FooEunm.bar
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_enum(bench_or_check_refcount):
+    serializer = Serializer(FooEunm)
+    bench_or_check_refcount.group = 'enum'
+    data = 'foo'
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+@dataclass
+class FooDataclass:
+    foo: int
+    bar: str
+
+
+def test_dump_dataclass(bench_or_check_refcount):
+    serializer = Serializer(FooDataclass)
+    bench_or_check_refcount.group = 'dataclass'
+    data = FooDataclass(foo=1, bar='2')
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_dataclass(bench_or_check_refcount):
+    serializer = Serializer(FooDataclass)
+    bench_or_check_refcount.group = 'dataclass'
+    data = {'foo': 1, 'bar': '2'}
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+@dataclass
+class Node:
+    value: str
+    next: Optional['Node'] = None
+
+
+@dataclass
+class Root:
+    head: Node
+
+
+def test_dump_recursive(bench_or_check_refcount):
+    serializer = Serializer(Root)
+    bench_or_check_refcount.group = 'recursive'
+    data = Root(
+        head=Node(
+            value='1',
+            next=Node(value='2'),
+        ),
+    )
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_recursive(bench_or_check_refcount):
+    serializer = Serializer(Root)
+    bench_or_check_refcount.group = 'recursive'
+    data = {'head': {'next': {'next': None, 'value': '2'}, 'value': '1'}}
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
+
+
+def test_dump_union(bench_or_check_refcount):
+    @dataclass
+    class Foo:
+        foo: int
+
+    serializer = Serializer(Union[int, Foo])
+    data = Foo(foo=1)
+    bench_or_check_refcount.group = 'union'
+    bench_or_check_refcount(repeat(lambda: serializer.dump(data)))
+
+
+def test_load_union(bench_or_check_refcount):
+    @dataclass
+    class Foo:
+        foo: int
+
+    serializer = Serializer(Union[int, Foo])
+    data = {'foo': 1}
+    bench_or_check_refcount.group = 'union'
+    bench_or_check_refcount(repeat(lambda: serializer.load(data)))
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_describe.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_describe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,527 +1,557 @@
-import dataclasses
-import sys
-from collections.abc import Callable, Iterable, Mapping, Sequence
-from datetime import date, datetime, time
-from decimal import Decimal
-from enum import Enum, IntEnum
-from typing import (
-    Annotated,
-    Any,
-    ForwardRef,
-    Generic,
-    Literal,
-    Optional,
-    TypeVar,
-    Union,
-    cast,
-    get_origin,
-    overload,
-)
-from uuid import UUID
-
-from typing_extensions import NotRequired, Required, assert_never, get_args, is_typeddict
-
-from ._impl import (
-    NOT_SET,
-    AnyType,
-    ArrayType,
-    BaseType,
-    BooleanType,
-    BytesType,
-    CustomEncoder,
-    DateTimeType,
-    DateType,
-    DecimalType,
-    DefaultValue,
-    DictionaryType,
-    DiscriminatedUnionType,
-    EntityField,
-    EntityType,
-    EnumType,
-    FloatType,
-    IntegerType,
-    LiteralType,
-    OptionalType,
-    RecursionHolder,
-    StringType,
-    TimeType,
-    TupleType,
-    TypedDictType,
-    UnionType,
-    UUIDType,
-)
-from ._meta import Meta, MetaStateKey
-from ._type_utils import get_type_hints  # type: ignore[attr-defined]
-from ._utils import get_attributes_doc, to_camelcase
-from .metadata import (
-    Alias,
-    Discriminator,
-    FieldFormat,
-    Format,
-    KeepDefaultForOptional,
-    KeepNone,
-    Max,
-    MaxLength,
-    Min,
-    MinLength,
-    NoFormat,
-    NoneAsDefaultForOptional,
-    NoneFormat,
-    OmitNone,
-)
-
-
-if sys.version_info >= (3, 10):  # pragma: no cover
-    from types import UnionType as StdUnionType
-else:  # pragma: no cover
-    StdUnionType = None
-
-FrozenInstanceErrors: tuple[type[Exception], ...] = (dataclasses.FrozenInstanceError,)
-
-try:
-    import attr
-    from attr.exceptions import FrozenInstanceError
-
-    FrozenInstanceErrors += (FrozenInstanceError,)
-except ImportError:  # pragma: no cover
-    attr = None  # type: ignore
-    FrozenInstanceError = None  # type: ignore
-
-
-_NoneType = type(None)
-
-_T = TypeVar('_T')
-
-
-def describe_type(t: Any, meta: Optional[Meta] = None) -> BaseType:
-    args: tuple[Any, ...] = ()
-    metadata = _get_annotated_metadata(t)
-    type_repr = repr(t)
-    if get_origin(t) == Annotated:  # unwrap annotated
-        t = t.__origin__
-    original_t = t
-    if get_origin(t) in {Required, NotRequired}:  # unwrap TypedDict special forms
-        t = t.__args__[0]
-    if hasattr(t, '__origin__'):
-        args = t.__args__
-        t = t.__origin__
-    # StdUnionType has no __origin__
-    elif StdUnionType and isinstance(t, StdUnionType):  # type: ignore[truthy-function]
-        args = t.__args__
-        t = Union
-    elif hasattr(t, '__parameters__'):
-        # Если передан generic-класс без type-параметров, значит по PEP-484 заменяем все параметры на Any
-        args = (Any,) * len(t.__parameters__)
-
-    if not meta:
-        meta = Meta(globals=_get_globals(t), state={})
-
-    t = _evaluate_forwardref(t, meta)
-
-    filed_format = _find_metadata(metadata, FieldFormat, NoFormat)
-    none_format = _find_metadata(metadata, NoneFormat, KeepNone)
-    none_as_default_for_optional = _find_metadata(metadata, NoneAsDefaultForOptional, KeepDefaultForOptional)
-    custom_encoder = _find_metadata(metadata, CustomEncoder)
-    annotation_wrapper = _wrap_annotated([filed_format, none_format, none_as_default_for_optional])
-
-    meta_key = MetaStateKey(
-        cls=original_t,
-        field_format=filed_format,
-        none_format=none_format,
-        none_as_default_for_optional=none_as_default_for_optional,
-    )
-
-    if meta.has_in_state(meta_key):
-        return RecursionHolder(
-            name=_generate_name(original_t, filed_format, none_format, none_as_default_for_optional),
-            state_key=meta_key,
-            meta=meta,
-            custom_encoder=None,
-        )
-
-    if t is Any:
-        return AnyType(custom_encoder=custom_encoder)
-
-    if isinstance(t, type):
-        simple_type_mapping: Mapping[type, type[BaseType]] = {
-            bytes: BytesType,
-            bool: BooleanType,
-            date: DateType,
-            time: TimeType,
-            datetime: DateTimeType,
-            UUID: UUIDType,
-        }
-
-        if simple := simple_type_mapping.get(t):
-            return simple(custom_encoder=custom_encoder)
-
-        number_type_mapping: Mapping[type, type[Union[IntegerType, FloatType]]] = {
-            int: IntegerType,
-            float: FloatType,
-        }
-
-        if number_type := number_type_mapping.get(t):
-            min_meta = _find_metadata(metadata, Min)
-            max_meta = _find_metadata(metadata, Max)
-            return number_type(
-                min=cast(Any, min_meta.value) if min_meta else None,
-                max=cast(Any, max_meta.value) if max_meta else None,
-                custom_encoder=custom_encoder,
-            )
-
-        if t is Decimal:
-            min_meta = _find_metadata(metadata, Min)
-            max_meta = _find_metadata(metadata, Max)
-            return DecimalType(
-                min=min_meta.value if min_meta else None,
-                max=max_meta.value if max_meta else None,
-                custom_encoder=custom_encoder,
-            )
-
-        if t is str:
-            min_length_meta = _find_metadata(metadata, MinLength)
-            max_length_meta = _find_metadata(metadata, MaxLength)
-            return StringType(
-                min_length=min_length_meta.value if min_length_meta else None,
-                max_length=max_length_meta.value if max_length_meta else None,
-                custom_encoder=custom_encoder,
-            )
-
-        if t in {Sequence, list}:
-            return ArrayType(
-                item_type=(describe_type(annotation_wrapper(args[0]), meta) if args else AnyType(custom_encoder=None)),
-                custom_encoder=custom_encoder,
-            )
-
-        if t in {Mapping, dict}:
-            return DictionaryType(
-                key_type=(describe_type(annotation_wrapper(args[0]), meta) if args else AnyType(custom_encoder=None)),
-                value_type=(describe_type(annotation_wrapper(args[1]), meta) if args else AnyType(custom_encoder=None)),
-                omit_none=none_format.omit,
-                custom_encoder=custom_encoder,
-            )
-
-        if t is tuple:
-            if not args or Ellipsis in args:
-                raise RuntimeError('Variable length tuples are not supported')
-            return TupleType(
-                item_types=[describe_type(annotation_wrapper(arg), meta) for arg in args],
-                custom_encoder=custom_encoder,
-            )
-
-        if issubclass(t, (Enum, IntEnum)):
-            return EnumType(cls=t, items=list(t), custom_encoder=custom_encoder)
-
-        if dataclasses.is_dataclass(t) or _is_attrs(t) or is_typeddict(t):
-            meta.add_to_state(meta_key, None)
-            entity_type = _describe_entity(
-                t=t,
-                original_t=original_t,
-                cls_filed_format=filed_format,
-                cls_none_format=none_format,
-                custom_encoder=custom_encoder,
-                cls_none_as_default_for_optional=none_as_default_for_optional,
-                meta=meta,
-            )
-            meta.add_to_state(meta_key, entity_type)
-            return entity_type
-
-    if _is_literal_type(t):
-        if args and all(isinstance(arg, (str, int)) for arg in args):
-            return LiteralType(args=list(args), custom_encoder=custom_encoder)
-        raise RuntimeError('Supported only Literal[str | int, ...]')
-
-    if t is Union:
-        if _NoneType in args:
-            new_args = tuple(arg for arg in args if arg is not _NoneType)
-            new_t = Union[new_args] if len(new_args) > 1 else new_args[0]  # type: ignore[unused-ignore]
-            return OptionalType(
-                inner=describe_type(annotation_wrapper(new_t), meta),
-                custom_encoder=None,
-            )
-
-        discriminator = _find_metadata(metadata, Discriminator)
-        if not discriminator:
-            return UnionType(
-                item_types=[describe_type(annotation_wrapper(arg), meta) for arg in args],
-                union_repr=type_repr.removeprefix('typing.'),
-                custom_encoder=custom_encoder,
-            )
-
-        if not all(dataclasses.is_dataclass(arg) or _is_attrs(arg) for arg in args):
-            raise RuntimeError(
-                f'Unions supported only for dataclasses or attrs. Provided: {t}[{",".join(map(str, args))}]'
-            )
-
-        meta = dataclasses.replace(meta, discriminator_field=discriminator.name)
-        return DiscriminatedUnionType(
-            item_types={
-                _get_discriminator_value(arg, discriminator.name): describe_type(annotation_wrapper(arg), meta)
-                for arg in args
-            },
-            dump_discriminator=discriminator.name,
-            load_discriminator=_apply_format(filed_format, discriminator.name),
-            custom_encoder=custom_encoder,
-        )
-
-    if isinstance(t, TypeVar):
-        raise RuntimeError(f'Unfilled TypeVar: {t}')
-
-    raise RuntimeError(f'Unknown type {t!r}')
-
-
-@dataclasses.dataclass
-class _Field(Generic[_T]):
-    name: str
-    type: type[_T]
-    default: Union[DefaultValue[_T], DefaultValue[None]] = NOT_SET
-    default_factory: Union[DefaultValue[Callable[[], _T]], DefaultValue[None]] = NOT_SET
-
-
-def _describe_entity(
-    t: Any,
-    original_t: Any,
-    cls_filed_format: FieldFormat,
-    cls_none_format: NoneFormat,
-    cls_none_as_default_for_optional: NoneAsDefaultForOptional,
-    custom_encoder: Optional[CustomEncoder[Any, Any]],
-    meta: Meta,
-) -> Union[EntityType, TypedDictType]:
-    # PEP-484: Replace all unfilled type parameters with Any
-    if not hasattr(original_t, '__origin__') and getattr(original_t, '__parameters__', None):
-        original_t = original_t[(Any,) * len(t.__parameters__)]
-
-    docs = get_attributes_doc(t)
-    try:
-        types = get_type_hints(original_t, include_extras=True)
-    except Exception:  # pylint: disable=broad-except
-        types = {}
-
-    discriminator_field = meta.discriminator_field
-    meta = dataclasses.replace(meta, globals=_get_globals(t), discriminator_field=None)
-
-    fields = []
-    for field in _get_entity_fields(t):
-        type_ = types.get(field.name, field.type)
-        type_ = Annotated[type_, cls_filed_format, cls_none_format, cls_none_as_default_for_optional]
-
-        metadata = _get_annotated_metadata(type_)
-        field_type = describe_type(type_, meta)
-        alias = _find_metadata(metadata, Alias)
-        none_as_default_for_optional = _find_metadata(metadata, NoneAsDefaultForOptional)
-
-        is_discriminator_field = field.name == discriminator_field
-        required = not (field.default != NOT_SET or field.default_factory != NOT_SET) or is_discriminator_field
-
-        default = field.default
-        if (
-            isinstance(field_type, OptionalType)
-            and required
-            and none_as_default_for_optional
-            and none_as_default_for_optional.use
-        ):
-            default = DefaultValue.some(None)
-            required = False
-
-        fields.append(
-            EntityField(
-                name=field.name,
-                dict_key=alias.value if alias else _apply_format(cls_filed_format, field.name),
-                doc=docs.get(field.name),
-                field_type=field_type,
-                default=default,
-                default_factory=field.default_factory,
-                is_discriminator_field=is_discriminator_field,
-                required=required,
-            )
-        )
-
-    if is_typeddict(t):
-        return TypedDictType(
-            name=_generate_name(original_t, cls_filed_format, cls_none_format, cls_none_as_default_for_optional),
-            fields=fields,
-            omit_none=cls_none_format is OmitNone,
-            doc=t.__doc__,
-            custom_encoder=custom_encoder,
-        )
-
-    return EntityType(
-        cls=t,
-        name=_generate_name(original_t, cls_filed_format, cls_none_format, cls_none_as_default_for_optional),
-        fields=fields,
-        omit_none=cls_none_format is OmitNone,
-        is_frozen=_is_frozen_dataclass(t, fields[0]) if fields else False,
-        doc=_get_dataclass_doc(t),
-        custom_encoder=custom_encoder,
-    )
-
-
-def _get_entity_fields(t: Any) -> Sequence[_Field[Any]]:
-    if dataclasses.is_dataclass(t):
-        return [
-            _Field(
-                name=f.name,
-                type=f.type,
-                default=(DefaultValue.some(f.default) if f.default is not dataclasses.MISSING else NOT_SET),
-                default_factory=(
-                    DefaultValue.some(f.default_factory) if f.default_factory is not dataclasses.MISSING else NOT_SET
-                ),
-            )
-            for f in dataclasses.fields(t)
-        ]
-    if is_typeddict(t):
-        return [
-            _Field(
-                name=field_name,
-                type=field_type,
-                default=NOT_SET if _is_required_in_typeddict(t, field_name) else DefaultValue.some(None),
-                default_factory=NOT_SET,
-            )
-            for field_name, field_type in t.__annotations__.items()
-        ]
-    if _is_attrs(t):
-        assert attr
-        return [
-            _Field(
-                name=f.name,
-                type=f.type,
-                default=(
-                    DefaultValue.some(f.default)
-                    if (
-                        f.default is not attr.NOTHING and not isinstance(f.default, attr.Factory)  # type: ignore[arg-type]
-                    )
-                    else NOT_SET
-                ),
-                default_factory=(
-                    DefaultValue.some(f.default.factory)  # pyright: ignore
-                    if isinstance(f.default, attr.Factory)  # type: ignore[arg-type]
-                    else NOT_SET
-                ),
-            )
-            for f in attr.fields(t)
-        ]
-
-    raise RuntimeError(f"Unsupported type '{t}'")
-
-
-@overload
-def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: _T) -> _T: ...
-
-
-@overload
-def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: None = None) -> Optional[_T]: ...
-
-
-def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: Optional[_T] = None) -> Optional[_T]:
-    return next((ann for ann in annotations if isinstance(ann, type_)), default)
-
-
-def _wrap_annotated(annotations: Iterable[Any]) -> Callable[[_T], _T]:
-    def inner(type_: _T) -> _T:
-        for ann in annotations:
-            type_ = Annotated[type_, ann]  # type: ignore
-        return type_
-
-    return inner
-
-
-def _get_annotated_metadata(t: Any) -> tuple[Any, ...]:
-    if get_origin(t) == Annotated:
-        return getattr(t, '__metadata__', ())
-    return ()
-
-
-def _apply_format(f: Optional[FieldFormat], value: str) -> str:
-    if not f or f.format is Format.no_format:
-        return value
-    if f.format is Format.camel_case:
-        return to_camelcase(value)
-    assert_never(f.format)
-
-
-def _generate_name(
-    cls: Any,
-    field_format: FieldFormat,
-    none_format: NoneFormat,
-    cls_none_as_default_for_optional: NoneAsDefaultForOptional,
-) -> str:
-    name = repr(cls).removeprefix("<class '").removesuffix("'>")
-    nones = 'omit_nones' if none_format.omit else 'keep_nones'
-    force_none = ',force_none' if cls_none_as_default_for_optional.use else ''
-    return f'{name}[{field_format.format.value},{nones}{force_none}]'
-
-
-def _get_globals(t: Any) -> dict[str, Any]:
-    if t.__module__ in sys.modules:
-        return sys.modules[t.__module__].__dict__.copy()
-    return {}
-
-
-def _evaluate_forwardref(t: type[_T], meta: Meta) -> type[_T]:
-    if not isinstance(t, ForwardRef):
-        return t
-
-    return t._evaluate(meta.globals, {}, set())
-
-
-def _get_discriminator_value(t: Any, name: str) -> str:
-    fields = attr.fields(t) if attr and _is_attrs(t) else dataclasses.fields(t)
-    for field in fields:
-        if field.name == name:
-            if _is_str_literal(field.type):
-                args = get_args(field.type)
-                if len(args) != 1:
-                    raise RuntimeError(
-                        f'Type {t} has invalid discriminator field "{name}". '
-                        f'Discriminator supports only Literal[<str>] with one argument.'
-                    )
-
-                return cast(str, args[0])
-
-            raise RuntimeError(
-                f'Type {t} has invalid discriminator field "{name}" with type "{field.type!r}". '
-                f'Discriminator supports only Literal[<str>].'
-            )
-    raise RuntimeError(f'Type {t} does not have discriminator field "{name}"')
-
-
-def _is_str_literal(t: Any) -> bool:
-    if _is_literal_type(t):
-        args = get_args(t)
-        if args and all(isinstance(arg, str) for arg in args):
-            return True
-    return False
-
-
-def _is_literal_type(t: Any) -> bool:
-    return t is Literal or get_origin(t) is Literal
-
-
-def _is_attrs(t: Any) -> bool:
-    return attr is not None and attr.has(t)
-
-
-def _is_required_in_typeddict(t: Any, key: str) -> bool:
-    if is_typeddict(t):
-        if t.__total__:
-            return key not in t.__optional_keys__
-        return key in t.__required_keys__
-    raise RuntimeError(f'Expected TypedDict, got "{t!r}"')
-
-
-def _get_dataclass_doc(cls: Any) -> Optional[str]:
-    """Dataclass has automatically generated docstring, which is not very useful."""
-    doc: str = cls.__doc__
-    if doc is None or doc.startswith(f'{cls.__name__}('):
-        return None
-    return doc
-
-
-def _is_frozen_dataclass(cls: Any, field: EntityField) -> bool:
-    try:
-        obj = object.__new__(cls)
-        setattr(obj, field.name, None)
-    except FrozenInstanceErrors:
-        return True
-    else:
-        return False
+import dataclasses
+import sys
+from collections.abc import Callable, Iterable, Mapping, Sequence
+from datetime import date, datetime, time
+from decimal import Decimal
+from enum import Enum, IntEnum
+from typing import (
+    Annotated,
+    Any,
+    ForwardRef,
+    Generic,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    cast,
+    get_origin,
+    overload,
+)
+from uuid import UUID
+
+from typing_extensions import NotRequired, Required, assert_never, get_args, is_typeddict
+
+from ._custom_types import CustomType as CustomTypeMeta
+from ._impl import (
+    NOT_SET,
+    AnyType,
+    ArrayType,
+    BaseType,
+    BooleanType,
+    BytesType,
+    CustomEncoder,
+    CustomType,
+    DateTimeType,
+    DateType,
+    DecimalType,
+    DefaultValue,
+    DictionaryType,
+    DiscriminatedUnionType,
+    EntityField,
+    EntityType,
+    EnumType,
+    FloatType,
+    IntegerType,
+    LiteralType,
+    OptionalType,
+    RecursionHolder,
+    StringType,
+    TimeType,
+    TupleType,
+    TypedDictType,
+    UnionType,
+    UUIDType,
+)
+from ._meta import Meta, MetaStateKey
+from ._type_utils import get_type_hints  # type: ignore[attr-defined]
+from ._utils import get_attributes_doc, to_camelcase
+from .metadata import (
+    Alias,
+    Discriminator,
+    FieldFormat,
+    Format,
+    KeepDefaultForOptional,
+    KeepNone,
+    Max,
+    MaxLength,
+    Min,
+    MinLength,
+    NoFormat,
+    NoneAsDefaultForOptional,
+    NoneFormat,
+    OmitNone,
+)
+
+
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from types import UnionType as StdUnionType
+else:  # pragma: no cover
+    StdUnionType = None
+
+FrozenInstanceErrors: tuple[type[Exception], ...] = (dataclasses.FrozenInstanceError,)
+
+try:
+    import attr
+    from attr.exceptions import FrozenInstanceError
+
+    FrozenInstanceErrors += (FrozenInstanceError,)
+except ImportError:  # pragma: no cover
+    attr = None  # type: ignore
+    FrozenInstanceError = None  # type: ignore
+
+
+_NoneType = type(None)
+
+_T = TypeVar('_T')
+
+
+def describe_type(
+    t: Any,
+    meta: Optional[Meta] = None,
+    custom_type_resolver: Optional[Callable[[Any], Optional[CustomTypeMeta[Any, Any]]]] = None,
+) -> BaseType:
+    args: tuple[Any, ...] = ()
+    metadata = _get_annotated_metadata(t)
+    type_repr = repr(t)
+    if get_origin(t) == Annotated:  # unwrap annotated
+        t = t.__origin__
+    original_t = t
+    if get_origin(t) in {Required, NotRequired}:  # unwrap TypedDict special forms
+        t = t.__args__[0]
+    if hasattr(t, '__origin__'):
+        args = t.__args__
+        t = t.__origin__
+    # StdUnionType has no __origin__
+    elif StdUnionType and isinstance(t, StdUnionType):  # type: ignore[truthy-function]
+        args = t.__args__
+        t = Union
+    elif hasattr(t, '__parameters__'):
+        # Если передан generic-класс без type-параметров, значит по PEP-484 заменяем все параметры на Any
+        args = (Any,) * len(t.__parameters__)
+
+    if not meta:
+        meta = Meta(globals=_get_globals(t), state={})
+
+    t = _evaluate_forwardref(t, meta)
+
+    filed_format = _find_metadata(metadata, FieldFormat, NoFormat)
+    none_format = _find_metadata(metadata, NoneFormat, KeepNone)
+    none_as_default_for_optional = _find_metadata(metadata, NoneAsDefaultForOptional, KeepDefaultForOptional)
+    custom_encoder = _find_metadata(metadata, CustomEncoder)
+    annotation_wrapper = _wrap_annotated([filed_format, none_format, none_as_default_for_optional])
+
+    meta_key = MetaStateKey(
+        cls=original_t,
+        field_format=filed_format,
+        none_format=none_format,
+        none_as_default_for_optional=none_as_default_for_optional,
+    )
+
+    if meta.has_in_state(meta_key):
+        return RecursionHolder(
+            name=_generate_name(original_t, filed_format, none_format, none_as_default_for_optional),
+            state_key=meta_key,
+            meta=meta,
+            custom_encoder=None,
+        )
+
+    if custom_type_resolver and (custom_type := custom_type_resolver(t)):
+        if custom_encoder is None:
+            custom_encoder = CustomEncoder(
+                serialize=custom_type.serialize,
+                deserialize=custom_type.deserialize,
+            )
+        return CustomType(custom_encoder=custom_encoder, json_schema=custom_type.get_json_schema())
+
+    if t is Any:
+        return AnyType(custom_encoder=custom_encoder)
+
+    if isinstance(t, type):
+        simple_type_mapping: Mapping[type, type[BaseType]] = {
+            bytes: BytesType,
+            bool: BooleanType,
+            date: DateType,
+            time: TimeType,
+            datetime: DateTimeType,
+            UUID: UUIDType,
+        }
+
+        if simple := simple_type_mapping.get(t):
+            return simple(custom_encoder=custom_encoder)
+
+        number_type_mapping: Mapping[type, type[Union[IntegerType, FloatType]]] = {
+            int: IntegerType,
+            float: FloatType,
+        }
+
+        if number_type := number_type_mapping.get(t):
+            min_meta = _find_metadata(metadata, Min)
+            max_meta = _find_metadata(metadata, Max)
+            return number_type(
+                min=cast(Any, min_meta.value) if min_meta else None,
+                max=cast(Any, max_meta.value) if max_meta else None,
+                custom_encoder=custom_encoder,
+            )
+
+        if t is Decimal:
+            min_meta = _find_metadata(metadata, Min)
+            max_meta = _find_metadata(metadata, Max)
+            return DecimalType(
+                min=min_meta.value if min_meta else None,
+                max=max_meta.value if max_meta else None,
+                custom_encoder=custom_encoder,
+            )
+
+        if t is str:
+            min_length_meta = _find_metadata(metadata, MinLength)
+            max_length_meta = _find_metadata(metadata, MaxLength)
+            return StringType(
+                min_length=min_length_meta.value if min_length_meta else None,
+                max_length=max_length_meta.value if max_length_meta else None,
+                custom_encoder=custom_encoder,
+            )
+
+        if t in {Sequence, list}:
+            return ArrayType(
+                item_type=(
+                    describe_type(annotation_wrapper(args[0]), meta, custom_type_resolver)
+                    if args
+                    else AnyType(custom_encoder=None)
+                ),
+                custom_encoder=custom_encoder,
+            )
+
+        if t in {Mapping, dict}:
+            return DictionaryType(
+                key_type=(
+                    describe_type(annotation_wrapper(args[0]), meta, custom_type_resolver)
+                    if args
+                    else AnyType(custom_encoder=None)
+                ),
+                value_type=(
+                    describe_type(annotation_wrapper(args[1]), meta, custom_type_resolver)
+                    if args
+                    else AnyType(custom_encoder=None)
+                ),
+                omit_none=none_format.omit,
+                custom_encoder=custom_encoder,
+            )
+
+        if t is tuple:
+            if not args or Ellipsis in args:
+                raise RuntimeError('Variable length tuples are not supported')
+            return TupleType(
+                item_types=[describe_type(annotation_wrapper(arg), meta, custom_type_resolver) for arg in args],
+                custom_encoder=custom_encoder,
+            )
+
+        if issubclass(t, (Enum, IntEnum)):
+            return EnumType(cls=t, items=list(t), custom_encoder=custom_encoder)
+
+        if dataclasses.is_dataclass(t) or _is_attrs(t) or is_typeddict(t):
+            meta.add_to_state(meta_key, None)
+            entity_type = _describe_entity(
+                t=t,
+                original_t=original_t,
+                cls_filed_format=filed_format,
+                cls_none_format=none_format,
+                custom_encoder=custom_encoder,
+                cls_none_as_default_for_optional=none_as_default_for_optional,
+                meta=meta,
+                custom_type_resolver=custom_type_resolver,
+            )
+            meta.add_to_state(meta_key, entity_type)
+            return entity_type
+
+    if _is_literal_type(t):
+        if args and all(isinstance(arg, (str, int)) for arg in args):
+            return LiteralType(args=list(args), custom_encoder=custom_encoder)
+        raise RuntimeError('Supported only Literal[str | int, ...]')
+
+    if t is Union:
+        if _NoneType in args:
+            new_args = tuple(arg for arg in args if arg is not _NoneType)
+            new_t = Union[new_args] if len(new_args) > 1 else new_args[0]  # type: ignore[unused-ignore]
+            return OptionalType(
+                inner=describe_type(annotation_wrapper(new_t), meta, custom_type_resolver),
+                custom_encoder=None,
+            )
+
+        discriminator = _find_metadata(metadata, Discriminator)
+        if not discriminator:
+            return UnionType(
+                item_types=[describe_type(annotation_wrapper(arg), meta, custom_type_resolver) for arg in args],
+                union_repr=type_repr.removeprefix('typing.'),
+                custom_encoder=custom_encoder,
+            )
+
+        if not all(dataclasses.is_dataclass(arg) or _is_attrs(arg) for arg in args):
+            raise RuntimeError(
+                f'Unions supported only for dataclasses or attrs. Provided: {t}[{",".join(map(str, args))}]'
+            )
+
+        meta = dataclasses.replace(meta, discriminator_field=discriminator.name)
+        return DiscriminatedUnionType(
+            item_types={
+                _get_discriminator_value(arg, discriminator.name): describe_type(
+                    annotation_wrapper(arg), meta, custom_type_resolver
+                )
+                for arg in args
+            },
+            dump_discriminator=discriminator.name,
+            load_discriminator=_apply_format(filed_format, discriminator.name),
+            custom_encoder=custom_encoder,
+        )
+
+    if isinstance(t, TypeVar):
+        raise RuntimeError(f'Unfilled TypeVar: {t}')
+
+    raise RuntimeError(f'Unknown type {t!r}')
+
+
+@dataclasses.dataclass
+class _Field(Generic[_T]):
+    name: str
+    type: type[_T]
+    default: Union[DefaultValue[_T], DefaultValue[None]] = NOT_SET
+    default_factory: Union[DefaultValue[Callable[[], _T]], DefaultValue[None]] = NOT_SET
+
+
+def _describe_entity(
+    t: Any,
+    original_t: Any,
+    cls_filed_format: FieldFormat,
+    cls_none_format: NoneFormat,
+    cls_none_as_default_for_optional: NoneAsDefaultForOptional,
+    custom_encoder: Optional[CustomEncoder[Any, Any]],
+    meta: Meta,
+    custom_type_resolver: Optional[Callable[[Any], Optional[CustomTypeMeta[Any, Any]]]],
+) -> Union[EntityType, TypedDictType]:
+    # PEP-484: Replace all unfilled type parameters with Any
+    if not hasattr(original_t, '__origin__') and getattr(original_t, '__parameters__', None):
+        original_t = original_t[(Any,) * len(t.__parameters__)]
+
+    docs = get_attributes_doc(t)
+    try:
+        types = get_type_hints(original_t, include_extras=True)
+    except Exception:  # pylint: disable=broad-except
+        types = {}
+
+    discriminator_field = meta.discriminator_field
+    meta = dataclasses.replace(meta, globals=_get_globals(t), discriminator_field=None)
+
+    fields = []
+    for field in _get_entity_fields(t):
+        type_ = types.get(field.name, field.type)
+        type_ = Annotated[type_, cls_filed_format, cls_none_format, cls_none_as_default_for_optional]
+
+        metadata = _get_annotated_metadata(type_)
+        field_type = describe_type(type_, meta, custom_type_resolver)
+        alias = _find_metadata(metadata, Alias)
+        none_as_default_for_optional = _find_metadata(metadata, NoneAsDefaultForOptional)
+
+        is_discriminator_field = field.name == discriminator_field
+        required = not (field.default != NOT_SET or field.default_factory != NOT_SET) or is_discriminator_field
+
+        default = field.default
+        if (
+            isinstance(field_type, OptionalType)
+            and required
+            and none_as_default_for_optional
+            and none_as_default_for_optional.use
+        ):
+            default = DefaultValue.some(None)
+            required = False
+
+        fields.append(
+            EntityField(
+                name=field.name,
+                dict_key=alias.value if alias else _apply_format(cls_filed_format, field.name),
+                doc=docs.get(field.name),
+                field_type=field_type,
+                default=default,
+                default_factory=field.default_factory,
+                is_discriminator_field=is_discriminator_field,
+                required=required,
+            )
+        )
+
+    if is_typeddict(t):
+        return TypedDictType(
+            name=_generate_name(original_t, cls_filed_format, cls_none_format, cls_none_as_default_for_optional),
+            fields=fields,
+            omit_none=cls_none_format is OmitNone,
+            doc=t.__doc__,
+            custom_encoder=custom_encoder,
+        )
+
+    return EntityType(
+        cls=t,
+        name=_generate_name(original_t, cls_filed_format, cls_none_format, cls_none_as_default_for_optional),
+        fields=fields,
+        omit_none=cls_none_format is OmitNone,
+        is_frozen=_is_frozen_dataclass(t, fields[0]) if fields else False,
+        doc=_get_dataclass_doc(t),
+        custom_encoder=custom_encoder,
+    )
+
+
+def _get_entity_fields(t: Any) -> Sequence[_Field[Any]]:
+    if dataclasses.is_dataclass(t):
+        return [
+            _Field(
+                name=f.name,
+                type=f.type,
+                default=(DefaultValue.some(f.default) if f.default is not dataclasses.MISSING else NOT_SET),
+                default_factory=(
+                    DefaultValue.some(f.default_factory) if f.default_factory is not dataclasses.MISSING else NOT_SET
+                ),
+            )
+            for f in dataclasses.fields(t)
+        ]
+    if is_typeddict(t):
+        return [
+            _Field(
+                name=field_name,
+                type=field_type,
+                default=NOT_SET if _is_required_in_typeddict(t, field_name) else DefaultValue.some(None),
+                default_factory=NOT_SET,
+            )
+            for field_name, field_type in t.__annotations__.items()
+        ]
+    if _is_attrs(t):
+        assert attr
+        return [
+            _Field(
+                name=f.name,
+                type=f.type,
+                default=(
+                    DefaultValue.some(f.default)
+                    if (
+                        f.default is not attr.NOTHING and not isinstance(f.default, attr.Factory)  # type: ignore[arg-type]
+                    )
+                    else NOT_SET
+                ),
+                default_factory=(
+                    DefaultValue.some(f.default.factory)  # pyright: ignore
+                    if isinstance(f.default, attr.Factory)  # type: ignore[arg-type]
+                    else NOT_SET
+                ),
+            )
+            for f in attr.fields(t)
+        ]
+
+    raise RuntimeError(f"Unsupported type '{t}'")
+
+
+@overload
+def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: _T) -> _T: ...
+
+
+@overload
+def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: None = None) -> Optional[_T]: ...
+
+
+def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: Optional[_T] = None) -> Optional[_T]:
+    return next((ann for ann in annotations if isinstance(ann, type_)), default)
+
+
+def _wrap_annotated(annotations: Iterable[Any]) -> Callable[[_T], _T]:
+    def inner(type_: _T) -> _T:
+        for ann in annotations:
+            type_ = Annotated[type_, ann]  # type: ignore
+        return type_
+
+    return inner
+
+
+def _get_annotated_metadata(t: Any) -> tuple[Any, ...]:
+    if get_origin(t) == Annotated:
+        return getattr(t, '__metadata__', ())
+    return ()
+
+
+def _apply_format(f: Optional[FieldFormat], value: str) -> str:
+    if not f or f.format is Format.no_format:
+        return value
+    if f.format is Format.camel_case:
+        return to_camelcase(value)
+    assert_never(f.format)
+
+
+def _generate_name(
+    cls: Any,
+    field_format: FieldFormat,
+    none_format: NoneFormat,
+    cls_none_as_default_for_optional: NoneAsDefaultForOptional,
+) -> str:
+    name = repr(cls).removeprefix("<class '").removesuffix("'>")
+    nones = 'omit_nones' if none_format.omit else 'keep_nones'
+    force_none = ',force_none' if cls_none_as_default_for_optional.use else ''
+    return f'{name}[{field_format.format.value},{nones}{force_none}]'
+
+
+def _get_globals(t: Any) -> dict[str, Any]:
+    if t.__module__ in sys.modules:
+        return sys.modules[t.__module__].__dict__.copy()
+    return {}
+
+
+def _evaluate_forwardref(t: type[_T], meta: Meta) -> type[_T]:
+    if not isinstance(t, ForwardRef):
+        return t
+
+    return t._evaluate(meta.globals, {}, set())
+
+
+def _get_discriminator_value(t: Any, name: str) -> str:
+    fields = attr.fields(t) if attr and _is_attrs(t) else dataclasses.fields(t)
+    for field in fields:
+        if field.name == name:
+            if _is_str_literal(field.type):
+                args = get_args(field.type)
+                if len(args) != 1:
+                    raise RuntimeError(
+                        f'Type {t} has invalid discriminator field "{name}". '
+                        f'Discriminator supports only Literal[<str>] with one argument.'
+                    )
+
+                return cast(str, args[0])
+
+            raise RuntimeError(
+                f'Type {t} has invalid discriminator field "{name}" with type "{field.type!r}". '
+                f'Discriminator supports only Literal[<str>].'
+            )
+    raise RuntimeError(f'Type {t} does not have discriminator field "{name}"')
+
+
+def _is_str_literal(t: Any) -> bool:
+    if _is_literal_type(t):
+        args = get_args(t)
+        if args and all(isinstance(arg, str) for arg in args):
+            return True
+    return False
+
+
+def _is_literal_type(t: Any) -> bool:
+    return t is Literal or get_origin(t) is Literal
+
+
+def _is_attrs(t: Any) -> bool:
+    return attr is not None and attr.has(t)
+
+
+def _is_required_in_typeddict(t: Any, key: str) -> bool:
+    if is_typeddict(t):
+        if t.__total__:
+            return key not in t.__optional_keys__
+        return key in t.__required_keys__
+    raise RuntimeError(f'Expected TypedDict, got "{t!r}"')
+
+
+def _get_dataclass_doc(cls: Any) -> Optional[str]:
+    """Dataclass has automatically generated docstring, which is not very useful."""
+    doc: str = cls.__doc__
+    if doc is None or doc.startswith(f'{cls.__name__}('):
+        return None
+    return doc
+
+
+def _is_frozen_dataclass(cls: Any, field: EntityField) -> bool:
+    try:
+        obj = object.__new__(cls)
+        setattr(obj, field.name, None)
+    except FrozenInstanceErrors:
+        return True
+    else:
+        return False
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_impl.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_impl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from typing import Generic, TypeVar
-
-from ._serpyco_rs import (
-    AnyType,
-    ArrayType,
-    BaseType,
-    BooleanType,
-    BytesType,
-    CustomEncoder as _CustomEncoder,
-    DateTimeType,
-    DateType,
-    DecimalType,
-    DefaultValue as _DefaultValue,
-    DictionaryType,
-    DiscriminatedUnionType,
-    EntityField,
-    EntityType,
-    EnumType,
-    ErrorItem,
-    FloatType,
-    IntegerType,
-    LiteralType,
-    OptionalType,
-    RecursionHolder,
-    SchemaValidationError,
-    Serializer,
-    StringType,
-    TimeType,
-    TupleType,
-    TypedDictType,
-    UnionType,
-    UUIDType,
-    ValidationError,
-)
-
-
-_T = TypeVar('_T')
-_I = TypeVar('_I')
-_O = TypeVar('_O')
-
-
-class CustomEncoder(_CustomEncoder, Generic[_I, _O]):
-    """pyo3 doesn't support specifying concrete types for generic methods."""
-
-
-class DefaultValue(_DefaultValue, Generic[_T]):
-    """pyo3 doesn't support specifying concrete types for generic methods."""
-
-
-NOT_SET = DefaultValue.none()
+from typing import Generic, TypeVar
+
+from ._serpyco_rs import (
+    AnyType,
+    ArrayType,
+    BaseType,
+    BooleanType,
+    BytesType,
+    CustomEncoder as _CustomEncoder,
+    DateTimeType,
+    DateType,
+    DecimalType,
+    DefaultValue as _DefaultValue,
+    DictionaryType,
+    DiscriminatedUnionType,
+    EntityField,
+    EntityType,
+    EnumType,
+    ErrorItem,
+    FloatType,
+    IntegerType,
+    LiteralType,
+    OptionalType,
+    RecursionHolder,
+    SchemaValidationError,
+    Serializer,
+    StringType,
+    TimeType,
+    TupleType,
+    TypedDictType,
+    UnionType,
+    UUIDType,
+    ValidationError,
+    CustomType,
+)
+
+
+_T = TypeVar('_T')
+_I = TypeVar('_I')
+_O = TypeVar('_O')
+
+
+class CustomEncoder(_CustomEncoder, Generic[_I, _O]):
+    """pyo3 doesn't support specifying concrete types for generic methods."""
+
+
+class DefaultValue(_DefaultValue, Generic[_T]):
+    """pyo3 doesn't support specifying concrete types for generic methods."""
+
+
+NOT_SET = DefaultValue.none()
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_impl.pyi` & `serpyco_rs-1.8.0/python/serpyco_rs/_impl.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,230 +1,235 @@
-from collections.abc import Sequence
-from enum import Enum, IntEnum
-from typing import Any, Callable, Generic, TypeVar
-
-from ._meta import Meta, MetaStateKey
-
-_T = TypeVar('_T')
-_I = TypeVar('_I')
-_O = TypeVar('_O')
-
-class ValidationError(Exception):
-    message: str
-
-class ErrorItem:
-    message: str
-    instance_path: str
-
-    def __init__(self, message: str, instance_path: str): ...
-
-class SchemaValidationError(ValidationError):
-    errors: list[ErrorItem]
-
-class Serializer(Generic[_T]):
-    def __init__(self, py_class: BaseType, naive_datetime_to_utc: bool): ...
-    def dump(self, value: _T) -> Any: ...
-    def load(self, data: Any) -> _T: ...
-    def load_query_params(self, data: Any) -> _T: ...
-
-class CustomEncoder(Generic[_I, _O]):
-    serialize: Callable[[_I], _O] | None
-    deserialize: Callable[[_O], _I] | None
-
-    def __init__(self, serialize: Callable[[_I], _O] | None = None, deserialize: Callable[[_O], _I] | None = None): ...
-
-class BaseType:
-    custom_encoder: CustomEncoder[Any, Any] | None
-
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class IntegerType(BaseType):
-    min: int | None
-    max: int | None
-
-    def __init__(
-        self, min: int | None = None, max: int | None = None, custom_encoder: CustomEncoder[Any, Any] | None = None
-    ): ...
-
-class FloatType(BaseType):
-    min: float | None
-    max: float | None
-
-    def __init__(self, min: float | None, max: float | None, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class DecimalType(BaseType):
-    min: float | None
-    max: float | None
-
-    def __init__(self, min: float | None, max: float | None, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class StringType(BaseType):
-    min_length: int | None
-    max_length: int | None
-
-    def __init__(
-        self,
-        min_length: int | None = None,
-        max_length: int | None = None,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class BooleanType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class UUIDType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class TimeType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class DateTimeType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class DateType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
-
-class DefaultValue(Generic[_T]):
-    @staticmethod
-    def none() -> DefaultValue[None]: ...
-    @staticmethod
-    def some(value: _T) -> DefaultValue[_T]: ...
-    def is_none(self) -> bool: ...
-
-NOT_SET: DefaultValue[None]
-
-class EntityField(BaseType):
-    name: str
-    dict_key: str
-    field_type: BaseType
-    required: bool = True
-    is_discriminator_field: bool = False
-    default: DefaultValue[Any]
-    default_factory: DefaultValue[Callable[[], Any]]
-    doc: str | None
-
-    def __init__(
-        self,
-        name: str,
-        dict_key: str,
-        field_type: BaseType,
-        required: bool = True,
-        is_discriminator_field: bool = False,
-        default: DefaultValue[Any] = ...,
-        default_factory: DefaultValue[Callable[[], Any]] | DefaultValue[None] = ...,
-        doc: str | None = None,
-    ): ...
-
-class EntityType(BaseType):
-    cls: type[Any]
-    name: str
-    fields: Sequence[EntityField]
-    omit_none: bool
-    is_frozen: bool
-    doc: str | None
-
-    def __init__(
-        self,
-        cls: type[Any],
-        name: str,
-        fields: Sequence[EntityField],
-        omit_none: bool = False,
-        is_frozen: bool = False,
-        doc: str | None = None,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class TypedDictType(BaseType):
-    name: str
-    fields: Sequence[EntityField]
-    omit_none: bool
-    doc: str | None
-
-    def __init__(
-        self,
-        name: str,
-        fields: Sequence[EntityField],
-        omit_none: bool = False,
-        doc: str | None = None,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class ArrayType(BaseType):
-    item_type: BaseType
-
-    def __init__(self, item_type: BaseType, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class EnumType(BaseType):
-    cls: type[Enum | IntEnum]
-    items: list[Any]
-
-    def __init__(
-        self, cls: type[Enum | IntEnum], items: list[Any], custom_encoder: CustomEncoder[Any, Any] | None = None
-    ): ...
-
-class OptionalType(BaseType):
-    inner: BaseType
-
-    def __init__(self, inner: BaseType, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class DictionaryType(BaseType):
-    key_type: BaseType
-    value_type: BaseType
-    omit_none: bool
-
-    def __init__(
-        self,
-        key_type: BaseType,
-        value_type: BaseType,
-        omit_none: bool = False,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class TupleType(BaseType):
-    item_types: list[BaseType]
-
-    def __init__(self, item_types: list[BaseType], custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class BytesType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class AnyType(BaseType):
-    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class UnionType(BaseType):
-    item_types: list[BaseType]
-    union_repr: str
-
-    def __init__(
-        self,
-        item_types: list[BaseType],
-        union_repr: str,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class DiscriminatedUnionType(BaseType):
-    item_types: dict[str, BaseType]
-    dump_discriminator: str
-    load_discriminator: str
-
-    def __init__(
-        self,
-        item_types: dict[str, BaseType],
-        dump_discriminator: str,
-        load_discriminator: str,
-        custom_encoder: CustomEncoder[Any, Any] | None = None,
-    ): ...
-
-class LiteralType(BaseType):
-    args: list[str]
-
-    def __init__(self, args: list[str], custom_encoder: CustomEncoder[Any, Any] | None = None): ...
-
-class RecursionHolder(BaseType):
-    name: str
-    state_key: MetaStateKey
-    meta: Meta
-
-    def __init__(
-        self, name: str, state_key: MetaStateKey, meta: Meta, custom_encoder: CustomEncoder[Any, Any] | None = None
-    ): ...
-    def get_type(self) -> BaseType: ...
+from collections.abc import Sequence
+from enum import Enum, IntEnum
+from typing import Any, Callable, Generic, TypeVar
+
+from ._meta import Meta, MetaStateKey
+
+_T = TypeVar('_T')
+_I = TypeVar('_I')
+_O = TypeVar('_O')
+
+class ValidationError(Exception):
+    message: str
+
+class ErrorItem:
+    message: str
+    instance_path: str
+
+    def __init__(self, message: str, instance_path: str): ...
+
+class SchemaValidationError(ValidationError):
+    errors: list[ErrorItem]
+
+class Serializer(Generic[_T]):
+    def __init__(self, py_class: BaseType, naive_datetime_to_utc: bool): ...
+    def dump(self, value: _T) -> Any: ...
+    def load(self, data: Any) -> _T: ...
+    def load_query_params(self, data: Any) -> _T: ...
+
+class CustomEncoder(Generic[_I, _O]):
+    serialize: Callable[[_I], _O] | None
+    deserialize: Callable[[_O], _I] | None
+
+    def __init__(self, serialize: Callable[[_I], _O] | None = None, deserialize: Callable[[_O], _I] | None = None): ...
+
+class BaseType:
+    custom_encoder: CustomEncoder[Any, Any] | None
+
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class IntegerType(BaseType):
+    min: int | None
+    max: int | None
+
+    def __init__(
+        self, min: int | None = None, max: int | None = None, custom_encoder: CustomEncoder[Any, Any] | None = None
+    ): ...
+
+class FloatType(BaseType):
+    min: float | None
+    max: float | None
+
+    def __init__(self, min: float | None, max: float | None, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class DecimalType(BaseType):
+    min: float | None
+    max: float | None
+
+    def __init__(self, min: float | None, max: float | None, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class StringType(BaseType):
+    min_length: int | None
+    max_length: int | None
+
+    def __init__(
+        self,
+        min_length: int | None = None,
+        max_length: int | None = None,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class BooleanType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class UUIDType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class TimeType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class DateTimeType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class DateType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None): ...
+
+class DefaultValue(Generic[_T]):
+    @staticmethod
+    def none() -> DefaultValue[None]: ...
+    @staticmethod
+    def some(value: _T) -> DefaultValue[_T]: ...
+    def is_none(self) -> bool: ...
+
+NOT_SET: DefaultValue[None]
+
+class EntityField(BaseType):
+    name: str
+    dict_key: str
+    field_type: BaseType
+    required: bool = True
+    is_discriminator_field: bool = False
+    default: DefaultValue[Any]
+    default_factory: DefaultValue[Callable[[], Any]]
+    doc: str | None
+
+    def __init__(
+        self,
+        name: str,
+        dict_key: str,
+        field_type: BaseType,
+        required: bool = True,
+        is_discriminator_field: bool = False,
+        default: DefaultValue[Any] = ...,
+        default_factory: DefaultValue[Callable[[], Any]] | DefaultValue[None] = ...,
+        doc: str | None = None,
+    ): ...
+
+class EntityType(BaseType):
+    cls: type[Any]
+    name: str
+    fields: Sequence[EntityField]
+    omit_none: bool
+    is_frozen: bool
+    doc: str | None
+
+    def __init__(
+        self,
+        cls: type[Any],
+        name: str,
+        fields: Sequence[EntityField],
+        omit_none: bool = False,
+        is_frozen: bool = False,
+        doc: str | None = None,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class TypedDictType(BaseType):
+    name: str
+    fields: Sequence[EntityField]
+    omit_none: bool
+    doc: str | None
+
+    def __init__(
+        self,
+        name: str,
+        fields: Sequence[EntityField],
+        omit_none: bool = False,
+        doc: str | None = None,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class ArrayType(BaseType):
+    item_type: BaseType
+
+    def __init__(self, item_type: BaseType, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class EnumType(BaseType):
+    cls: type[Enum | IntEnum]
+    items: list[Any]
+
+    def __init__(
+        self, cls: type[Enum | IntEnum], items: list[Any], custom_encoder: CustomEncoder[Any, Any] | None = None
+    ): ...
+
+class OptionalType(BaseType):
+    inner: BaseType
+
+    def __init__(self, inner: BaseType, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class DictionaryType(BaseType):
+    key_type: BaseType
+    value_type: BaseType
+    omit_none: bool
+
+    def __init__(
+        self,
+        key_type: BaseType,
+        value_type: BaseType,
+        omit_none: bool = False,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class TupleType(BaseType):
+    item_types: list[BaseType]
+
+    def __init__(self, item_types: list[BaseType], custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class BytesType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class AnyType(BaseType):
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class UnionType(BaseType):
+    item_types: list[BaseType]
+    union_repr: str
+
+    def __init__(
+        self,
+        item_types: list[BaseType],
+        union_repr: str,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class DiscriminatedUnionType(BaseType):
+    item_types: dict[str, BaseType]
+    dump_discriminator: str
+    load_discriminator: str
+
+    def __init__(
+        self,
+        item_types: dict[str, BaseType],
+        dump_discriminator: str,
+        load_discriminator: str,
+        custom_encoder: CustomEncoder[Any, Any] | None = None,
+    ): ...
+
+class LiteralType(BaseType):
+    args: list[str]
+
+    def __init__(self, args: list[str], custom_encoder: CustomEncoder[Any, Any] | None = None): ...
+
+class RecursionHolder(BaseType):
+    name: str
+    state_key: MetaStateKey
+    meta: Meta
+
+    def __init__(
+        self, name: str, state_key: MetaStateKey, meta: Meta, custom_encoder: CustomEncoder[Any, Any] | None = None
+    ): ...
+    def get_type(self) -> BaseType: ...
+
+class CustomType(BaseType):
+    json_schema: dict[str, Any]
+
+    def __init__(self, custom_encoder: CustomEncoder[Any, Any], json_schema: dict[str, Any]): ...
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/_convert.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/_convert.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,253 +1,258 @@
-import sys
-import typing
-from functools import singledispatch
-from typing import Any, Optional, Union, cast
-
-from .._utils import get_attributes_doc
-from ._consts import DEFAULT_REF_PREFIX, SCHEMA_VERSION
-
-
-if sys.version_info >= (3, 10):
-    from typing import TypeGuard
-else:
-    from typing_extensions import TypeGuard
-
-from .. import _describe as describe
-from ._entities import (
-    ArrayType,
-    Boolean,
-    Config,
-    DiscriminatedUnionType,
-    Discriminator,
-    IntegerType,
-    Null,
-    NumberType,
-    ObjectType,
-    RefType,
-    Schema,
-    StringType,
-)
-
-
-if typing.TYPE_CHECKING:
-    from .._main import Serializer
-
-
-class JsonSchemaBuilder:
-    def __init__(self, add_dialect_uri: bool = False, ref_prefix: str = DEFAULT_REF_PREFIX):
-        self._definitions: dict[str, Any] = {}
-        self._ref_prefix = ref_prefix.rstrip('/')
-        self._add_dialect_uri = add_dialect_uri
-        self._config = Config(ref_prefix=ref_prefix)
-
-    def build(self, serializer: 'Serializer[Any]') -> dict[str, Any]:
-        schema = to_json_schema(serializer._type_info, config=self._config)
-        schema_def = schema.dump(self._definitions)
-        if self._add_dialect_uri:
-            schema_def['$schema'] = SCHEMA_VERSION
-        return schema_def
-
-    def get_definitions(self) -> dict[str, Any]:
-        return self._definitions
-
-
-def get_json_schema(t: describe.BaseType) -> dict[str, Any]:
-    schema = to_json_schema(t, config=Config())
-    definitions: dict[str, Any] = {}
-    schema_def = schema.dump(definitions)
-    components = {'components': {'schemas': definitions}} if definitions else {}
-    return {
-        '$schema': SCHEMA_VERSION,
-        **schema_def,
-        **components,
-    }
-
-
-@singledispatch
-def to_json_schema(_: Any, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Schema(description=doc, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.StringType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(minLength=arg.min_length, maxLength=arg.max_length, description=doc, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.IntegerType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return IntegerType(minimum=arg.min, maximum=arg.max, description=doc, config=config)
-
-
-@to_json_schema.register
-def _(_: describe.BytesType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(format='binary', description=doc, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.FloatType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return NumberType(minimum=arg.min, maximum=arg.max, description=doc, config=config)
-
-
-@to_json_schema.register
-def _(_: describe.DecimalType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    # todo: support min/max
-    return Schema(
-        oneOf=[
-            StringType(format='decimal', config=config),
-            NumberType(format='decimal', config=config),
-        ],
-        description=doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(_: describe.BooleanType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Boolean(config=config, description=doc)
-
-
-@to_json_schema.register
-def _(_: describe.UUIDType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(format='uuid', description=doc, config=config)
-
-
-@to_json_schema.register
-def _(_: describe.TimeType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(format='time', description=doc, config=config)
-
-
-@to_json_schema.register
-def _(_: describe.DateTimeType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(format='date-time', description=doc, config=config)
-
-
-@to_json_schema.register
-def _(_: describe.DateType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return StringType(format='date', description=doc, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.EnumType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    docs = get_attributes_doc(arg.cls)
-    enum_values = [item.value for item in arg.items]
-    type_ = None
-    if (types := {type(item.value) for item in arg.items}) and len(types) == 1:
-        type_ = {int: 'integer', str: 'string'}.get(types.pop(), None)
-
-    return Schema(
-        type=type_,
-        enum=enum_values,
-        description=doc,
-        config=config,
-        additionalArgs={f'x-{item.value}': docs.get(item.name) for item in arg.items},
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.OptionalType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Schema(
-        anyOf=[
-            Null(config=config),
-            to_json_schema(arg.inner, config=config),
-        ],
-        description=doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.EntityType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return ObjectType(
-        properties={prop.dict_key: to_json_schema(prop.field_type, prop.doc, config=config) for prop in arg.fields},
-        required=[prop.dict_key for prop in arg.fields if prop.required] or None,
-        name=arg.name,
-        description=arg.doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.TypedDictType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return ObjectType(
-        properties={prop.dict_key: to_json_schema(prop.field_type, prop.doc, config=config) for prop in arg.fields},
-        required=[prop.dict_key for prop in arg.fields if prop.required] or None,
-        name=arg.name,
-        description=arg.doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.ArrayType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return ArrayType(items=to_json_schema(arg.item_type, config=config), description=doc, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.DictionaryType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return ObjectType(
-        additionalProperties=to_json_schema(arg.value_type, config=config), description=doc, config=config
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.TupleType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return ArrayType(
-        prefixItems=[to_json_schema(item, config=config) for item in arg.item_types],
-        minItems=len(arg.item_types),
-        maxItems=len(arg.item_types),
-        description=doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(_: describe.AnyType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Schema(description=doc, config=config)
-
-
-@to_json_schema.register
-def _(holder: describe.RecursionHolder, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return RefType(description=doc, name=holder.name, config=config)
-
-
-@to_json_schema.register
-def _(arg: describe.LiteralType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Schema(
-        enum=list(arg.args),
-        description=doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.UnionType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    return Schema(
-        oneOf=[to_json_schema(t, config=config) for t in arg.item_types],
-        description=doc,
-        config=config,
-    )
-
-
-@to_json_schema.register
-def _(arg: describe.DiscriminatedUnionType, doc: Optional[str] = None, *, config: Config) -> Schema:
-    objects = {
-        name: schema
-        for name, t in arg.item_types.items()
-        if (schema := to_json_schema(t, config=config)) and _check_unions_schema_types(schema)
-    }
-
-    return DiscriminatedUnionType(
-        oneOf=list(objects.values()),
-        discriminator=Discriminator(
-            property_name=arg.load_discriminator,
-            mapping={name: val.ref for name, val in objects.items()},
-        ),
-        description=doc,
-        config=config,
-    )
-
-
-def _check_unions_schema_types(schema: Schema) -> TypeGuard[Union[ObjectType, RefType]]:
-    if isinstance(schema, (ObjectType, RefType)):
-        return True
-    raise RuntimeError(f'Unions schema items must be ObjectType or RefType. Current: {schema}')
+import sys
+import typing
+from functools import singledispatch
+from typing import Any, Optional, Union, cast
+
+from .._utils import get_attributes_doc
+from ._consts import DEFAULT_REF_PREFIX, SCHEMA_VERSION
+
+
+if sys.version_info >= (3, 10):
+    from typing import TypeGuard
+else:
+    from typing_extensions import TypeGuard
+
+from .. import _describe as describe
+from ._entities import (
+    ArrayType,
+    Boolean,
+    Config,
+    DiscriminatedUnionType,
+    Discriminator,
+    IntegerType,
+    Null,
+    NumberType,
+    ObjectType,
+    RefType,
+    Schema,
+    StringType,
+)
+
+
+if typing.TYPE_CHECKING:
+    from .._main import Serializer
+
+
+class JsonSchemaBuilder:
+    def __init__(self, add_dialect_uri: bool = False, ref_prefix: str = DEFAULT_REF_PREFIX):
+        self._definitions: dict[str, Any] = {}
+        self._ref_prefix = ref_prefix.rstrip('/')
+        self._add_dialect_uri = add_dialect_uri
+        self._config = Config(ref_prefix=ref_prefix)
+
+    def build(self, serializer: 'Serializer[Any]') -> dict[str, Any]:
+        schema = to_json_schema(serializer._type_info, config=self._config)
+        schema_def = schema.dump(self._definitions)
+        if self._add_dialect_uri:
+            schema_def['$schema'] = SCHEMA_VERSION
+        return schema_def
+
+    def get_definitions(self) -> dict[str, Any]:
+        return self._definitions
+
+
+def get_json_schema(t: describe.BaseType) -> dict[str, Any]:
+    schema = to_json_schema(t, config=Config())
+    definitions: dict[str, Any] = {}
+    schema_def = schema.dump(definitions)
+    components = {'components': {'schemas': definitions}} if definitions else {}
+    return {
+        '$schema': SCHEMA_VERSION,
+        **schema_def,
+        **components,
+    }
+
+
+@singledispatch
+def to_json_schema(_: Any, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(description=doc, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.StringType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(minLength=arg.min_length, maxLength=arg.max_length, description=doc, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.IntegerType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return IntegerType(minimum=arg.min, maximum=arg.max, description=doc, config=config)
+
+
+@to_json_schema.register
+def _(_: describe.BytesType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(format='binary', description=doc, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.FloatType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return NumberType(minimum=arg.min, maximum=arg.max, description=doc, config=config)
+
+
+@to_json_schema.register
+def _(_: describe.DecimalType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    # todo: support min/max
+    return Schema(
+        oneOf=[
+            StringType(format='decimal', config=config),
+            NumberType(format='decimal', config=config),
+        ],
+        description=doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(_: describe.BooleanType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Boolean(config=config, description=doc)
+
+
+@to_json_schema.register
+def _(_: describe.UUIDType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(format='uuid', description=doc, config=config)
+
+
+@to_json_schema.register
+def _(_: describe.TimeType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(format='time', description=doc, config=config)
+
+
+@to_json_schema.register
+def _(_: describe.DateTimeType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(format='date-time', description=doc, config=config)
+
+
+@to_json_schema.register
+def _(_: describe.DateType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return StringType(format='date', description=doc, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.EnumType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    docs = get_attributes_doc(arg.cls)
+    enum_values = [item.value for item in arg.items]
+    type_ = None
+    if (types := {type(item.value) for item in arg.items}) and len(types) == 1:
+        type_ = {int: 'integer', str: 'string'}.get(types.pop(), None)
+
+    return Schema(
+        type=type_,
+        enum=enum_values,
+        description=doc,
+        config=config,
+        additionalArgs={f'x-{item.value}': docs.get(item.name) for item in arg.items},
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.OptionalType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(
+        anyOf=[
+            Null(config=config),
+            to_json_schema(arg.inner, config=config),
+        ],
+        description=doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.EntityType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return ObjectType(
+        properties={prop.dict_key: to_json_schema(prop.field_type, prop.doc, config=config) for prop in arg.fields},
+        required=[prop.dict_key for prop in arg.fields if prop.required] or None,
+        name=arg.name,
+        description=arg.doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.TypedDictType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return ObjectType(
+        properties={prop.dict_key: to_json_schema(prop.field_type, prop.doc, config=config) for prop in arg.fields},
+        required=[prop.dict_key for prop in arg.fields if prop.required] or None,
+        name=arg.name,
+        description=arg.doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.ArrayType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return ArrayType(items=to_json_schema(arg.item_type, config=config), description=doc, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.DictionaryType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return ObjectType(
+        additionalProperties=to_json_schema(arg.value_type, config=config), description=doc, config=config
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.TupleType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return ArrayType(
+        prefixItems=[to_json_schema(item, config=config) for item in arg.item_types],
+        minItems=len(arg.item_types),
+        maxItems=len(arg.item_types),
+        description=doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(_: describe.AnyType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(description=doc, config=config)
+
+
+@to_json_schema.register
+def _(holder: describe.RecursionHolder, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return RefType(description=doc, name=holder.name, config=config)
+
+
+@to_json_schema.register
+def _(arg: describe.LiteralType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(
+        enum=list(arg.args),
+        description=doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.UnionType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(
+        oneOf=[to_json_schema(t, config=config) for t in arg.item_types],
+        description=doc,
+        config=config,
+    )
+
+
+@to_json_schema.register
+def _(arg: describe.DiscriminatedUnionType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    objects = {
+        name: schema
+        for name, t in arg.item_types.items()
+        if (schema := to_json_schema(t, config=config)) and _check_unions_schema_types(schema)
+    }
+
+    return DiscriminatedUnionType(
+        oneOf=list(objects.values()),
+        discriminator=Discriminator(
+            property_name=arg.load_discriminator,
+            mapping={name: val.ref for name, val in objects.items()},
+        ),
+        description=doc,
+        config=config,
+    )
+
+
+def _check_unions_schema_types(schema: Schema) -> TypeGuard[Union[ObjectType, RefType]]:
+    if isinstance(schema, (ObjectType, RefType)):
+        return True
+    raise RuntimeError(f'Unions schema items must be ObjectType or RefType. Current: {schema}')
+
+
+@to_json_schema.register
+def _(arg: describe.CustomType, doc: Optional[str] = None, *, config: Config) -> Schema:
+    return Schema(additionalArgs=arg.json_schema, description=doc, config=config)
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_json_schema/_entities.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_json_schema/_entities.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import Any
-
-from ._consts import DEFAULT_REF_PREFIX
-
-
-@dataclass
-class Config:
-    ref_prefix: str = DEFAULT_REF_PREFIX
-
-
-@dataclass
-class Schema:
-    config: Config
-
-    type: str | None = None
-    title: str | None = None
-    description: str | None = None
-    default: Any | None = None
-    enum: list[Any] | None = None
-
-    allOf: list[Schema] | None = None
-    anyOf: list[Schema] | None = None
-    oneOf: list[Schema] | None = None
-    additionalArgs: dict[str, Any] | None = None
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = {
-            'type': self.type,
-            'title': self.title,
-            'description': self.description,
-            'default': self.default,
-            'enum': self.enum,
-            'allOf': [item.dump(definitions) for item in self.allOf] if self.allOf else None,
-            'anyOf': [item.dump(definitions) for item in self.anyOf] if self.anyOf else None,
-            'oneOf': [item.dump(definitions) for item in self.oneOf] if self.oneOf else None,
-            **(self.additionalArgs or {}),
-        }
-        return {k: v for k, v in data.items() if v is not None}
-
-
-@dataclass
-class Boolean(Schema):
-    type: str = 'boolean'  # pyright: ignore[reportIncompatibleVariableOverride]
-
-
-@dataclass
-class Null(Schema):
-    type: str = 'null'  # pyright: ignore[reportIncompatibleVariableOverride]
-
-
-@dataclass
-class StringType(Schema):
-    type: str = 'string'  # pyright: ignore[reportIncompatibleVariableOverride]
-    minLength: int | None = None
-    maxLength: int | None = None
-    format: str | None = None
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        data = {
-            'minLength': self.minLength,
-            'maxLength': self.maxLength,
-            'format': self.format,
-            **data,
-        }
-        return {k: v for k, v in data.items() if v is not None}
-
-
-@dataclass
-class NumberType(Schema):
-    type: str = 'number'  # pyright: ignore[reportIncompatibleVariableOverride]
-    minimum: float | None = None
-    maximum: float | None = None
-    format: str | None = None
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        data = {
-            'minimum': self.minimum,
-            'maximum': self.maximum,
-            'format': self.format,
-            **data,
-        }
-        return {k: v for k, v in data.items() if v is not None}
-
-
-@dataclass
-class IntegerType(NumberType):
-    type: str = 'integer'
-
-
-@dataclass
-class ObjectType(Schema):
-    name: str | None = None
-    type: str = 'object'  # pyright: ignore[reportIncompatibleVariableOverride]
-    properties: dict[str, Schema] | None = None
-    additionalProperties: bool | Schema | None = None
-    required: list[str] | None = None
-
-    @property
-    def ref(self) -> str:
-        return f'{self.config.ref_prefix}/{self.name}'
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        data = {
-            'properties': {k: v.dump(definitions) for k, v in self.properties.items()} if self.properties else None,
-            'additionalProperties': (
-                self.additionalProperties.dump(definitions)
-                if isinstance(self.additionalProperties, Schema)
-                else self.additionalProperties
-            ),
-            'required': self.required,
-            **data,
-        }
-        data = {k: v for k, v in data.items() if v is not None}
-        if not self.name:
-            return data
-        definitions[self.name] = data
-        return {
-            '$ref': self.ref,
-        }
-
-
-@dataclass
-class ArrayType(Schema):
-    type: str = 'array'  # pyright: ignore[reportIncompatibleVariableOverride]
-    items: Schema | None = None
-    prefixItems: list[Schema] | None = None
-    minItems: int | None = None
-    maxItems: int | None = None
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        data = {
-            'items': self.items.dump(definitions) if self.items else None,
-            'prefixItems': [i.dump(definitions) for i in self.prefixItems] if self.prefixItems else None,
-            'minItems': self.minItems,
-            'maxItems': self.maxItems,
-            **data,
-        }
-        return {k: v for k, v in data.items() if v is not None}
-
-
-@dataclass
-class RefType(Schema):
-    name: str | None = None
-
-    @property
-    def ref(self) -> str:
-        return f'{self.config.ref_prefix}/{self.name}'
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        return {
-            '$ref': self.ref,
-            **data,
-        }
-
-
-@dataclass
-class DiscriminatedUnionType(Schema):
-    discriminator: Discriminator | None = None
-
-    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
-        data = super().dump(definitions)
-        return {
-            'discriminator': self.discriminator.dump() if self.discriminator else None,
-            **data,
-        }
-
-
-@dataclass
-class Discriminator:
-    property_name: str
-    mapping: dict[str, str]
-
-    def dump(self) -> dict[str, Any]:
-        return {
-            'propertyName': self.property_name,
-            'mapping': self.mapping,
-        }
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import Any
+
+from ._consts import DEFAULT_REF_PREFIX
+
+
+@dataclass
+class Config:
+    ref_prefix: str = DEFAULT_REF_PREFIX
+
+
+@dataclass
+class Schema:
+    config: Config
+
+    type: str | None = None
+    title: str | None = None
+    description: str | None = None
+    default: Any | None = None
+    enum: list[Any] | None = None
+
+    allOf: list[Schema] | None = None
+    anyOf: list[Schema] | None = None
+    oneOf: list[Schema] | None = None
+    additionalArgs: dict[str, Any] | None = None
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = {
+            'type': self.type,
+            'title': self.title,
+            'description': self.description,
+            'default': self.default,
+            'enum': self.enum,
+            'allOf': [item.dump(definitions) for item in self.allOf] if self.allOf else None,
+            'anyOf': [item.dump(definitions) for item in self.anyOf] if self.anyOf else None,
+            'oneOf': [item.dump(definitions) for item in self.oneOf] if self.oneOf else None,
+            **(self.additionalArgs or {}),
+        }
+        return {k: v for k, v in data.items() if v is not None}
+
+
+@dataclass
+class Boolean(Schema):
+    type: str = 'boolean'  # pyright: ignore[reportIncompatibleVariableOverride]
+
+
+@dataclass
+class Null(Schema):
+    type: str = 'null'  # pyright: ignore[reportIncompatibleVariableOverride]
+
+
+@dataclass
+class StringType(Schema):
+    type: str = 'string'  # pyright: ignore[reportIncompatibleVariableOverride]
+    minLength: int | None = None
+    maxLength: int | None = None
+    format: str | None = None
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        data = {
+            'minLength': self.minLength,
+            'maxLength': self.maxLength,
+            'format': self.format,
+            **data,
+        }
+        return {k: v for k, v in data.items() if v is not None}
+
+
+@dataclass
+class NumberType(Schema):
+    type: str = 'number'  # pyright: ignore[reportIncompatibleVariableOverride]
+    minimum: float | None = None
+    maximum: float | None = None
+    format: str | None = None
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        data = {
+            'minimum': self.minimum,
+            'maximum': self.maximum,
+            'format': self.format,
+            **data,
+        }
+        return {k: v for k, v in data.items() if v is not None}
+
+
+@dataclass
+class IntegerType(NumberType):
+    type: str = 'integer'
+
+
+@dataclass
+class ObjectType(Schema):
+    name: str | None = None
+    type: str = 'object'  # pyright: ignore[reportIncompatibleVariableOverride]
+    properties: dict[str, Schema] | None = None
+    additionalProperties: bool | Schema | None = None
+    required: list[str] | None = None
+
+    @property
+    def ref(self) -> str:
+        return f'{self.config.ref_prefix}/{self.name}'
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        data = {
+            'properties': {k: v.dump(definitions) for k, v in self.properties.items()} if self.properties else None,
+            'additionalProperties': (
+                self.additionalProperties.dump(definitions)
+                if isinstance(self.additionalProperties, Schema)
+                else self.additionalProperties
+            ),
+            'required': self.required,
+            **data,
+        }
+        data = {k: v for k, v in data.items() if v is not None}
+        if not self.name:
+            return data
+        definitions[self.name] = data
+        return {
+            '$ref': self.ref,
+        }
+
+
+@dataclass
+class ArrayType(Schema):
+    type: str = 'array'  # pyright: ignore[reportIncompatibleVariableOverride]
+    items: Schema | None = None
+    prefixItems: list[Schema] | None = None
+    minItems: int | None = None
+    maxItems: int | None = None
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        data = {
+            'items': self.items.dump(definitions) if self.items else None,
+            'prefixItems': [i.dump(definitions) for i in self.prefixItems] if self.prefixItems else None,
+            'minItems': self.minItems,
+            'maxItems': self.maxItems,
+            **data,
+        }
+        return {k: v for k, v in data.items() if v is not None}
+
+
+@dataclass
+class RefType(Schema):
+    name: str | None = None
+
+    @property
+    def ref(self) -> str:
+        return f'{self.config.ref_prefix}/{self.name}'
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        return {
+            '$ref': self.ref,
+            **data,
+        }
+
+
+@dataclass
+class DiscriminatedUnionType(Schema):
+    discriminator: Discriminator | None = None
+
+    def dump(self, definitions: dict[str, Any]) -> dict[str, Any]:
+        data = super().dump(definitions)
+        return {
+            'discriminator': self.discriminator.dump() if self.discriminator else None,
+            **data,
+        }
+
+
+@dataclass
+class Discriminator:
+    property_name: str
+    mapping: dict[str, str]
+
+    def dump(self) -> dict[str, Any]:
+        return {
+            'propertyName': self.property_name,
+            'mapping': self.mapping,
+        }
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_main.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,90 @@
-import abc
-from typing import Annotated, Any, Generic, Protocol, TypeVar, Union, cast, overload
-
-from ._describe import BaseType, describe_type
-from ._impl import Serializer as _Serializer
-from ._json_schema import get_json_schema
-from .metadata import CamelCase, ForceDefaultForOptional, OmitNone
-
-
-_T = TypeVar('_T', bound=Any)
-_D = TypeVar('_D')
-
-
-class _MultiMapping(Protocol[_T, _D]):
-    """Protocol for a multi-mapping type."""
-
-    @abc.abstractmethod
-    def __getitem__(self, __key: str) -> _T: ...
-
-    @overload
-    @abc.abstractmethod
-    def getall(self, key: str) -> list[_T]: ...
-    @overload
-    @abc.abstractmethod
-    def getall(self, key: str, default: _D) -> Union[list[_T], _D]: ...
-    @abc.abstractmethod
-    def getall(self, key: str, default: _D = ...) -> Union[list[_T], _D]: ...
-
-
-class Serializer(Generic[_T]):
-    _type_info: BaseType
-
-    def __init__(
-        self,
-        t: type[_T],
-        *,
-        camelcase_fields: bool = False,
-        omit_none: bool = False,
-        force_default_for_optional: bool = False,
-        naive_datetime_to_utc: bool = False,
-    ) -> None:
-        """
-        Create a serializer for the given type.
-
-        :param t: The type to serialize/deserialize.
-        :param camelcase_fields: If True, the serializer will convert field names to camelCase.
-        :param omit_none: If True, the serializer will omit None values from the output.
-        :param force_default_for_optional: If True, the serializer will force default values for optional fields.
-        :param naive_datetime_to_utc: If True, the serializer will convert naive datetimes to UTC.
-        """
-        if camelcase_fields:
-            t = cast(type[_T], Annotated[t, CamelCase])
-        if omit_none:
-            t = cast(type(_T), Annotated[t, OmitNone])  # type: ignore
-        if force_default_for_optional:
-            t = cast(type(_T), Annotated[t, ForceDefaultForOptional])  # type: ignore
-        self._type_info = describe_type(t)
-        self._schema = get_json_schema(self._type_info)
-        self._encoder: _Serializer[_T] = _Serializer(self._type_info, naive_datetime_to_utc)
-
-    def dump(self, value: _T) -> Any:
-        """Serialize the given value to a JSON-serializable object.
-
-        :param value: The value to serialize.
-        """
-        return self._encoder.dump(value)
-
-    def load(self, data: Any) -> _T:
-        """Deserialize the given JSON-serializable object to the target type.
-
-        :param data: The data to deserialize.
-        """
-        return self._encoder.load(data)
-
-    def load_query_params(self, data: _MultiMapping[Any, Any]) -> _T:
-        """Deserialize the given query parameters to the target type.
-
-        :param data: The query parameters to deserialize.
-        """
-        return self._encoder.load_query_params(data)
-
-    def get_json_schema(self) -> dict[str, Any]:
-        """Get the JSON schema for the target type."""
-        return self._schema
+import abc
+from collections.abc import Callable
+from typing import Annotated, Any, Generic, Optional, Protocol, TypeVar, Union, cast, overload
+
+from ._custom_types import CustomType
+from ._describe import BaseType, describe_type
+from ._impl import Serializer as _Serializer
+from ._json_schema import get_json_schema
+from .metadata import CamelCase, ForceDefaultForOptional, OmitNone
+
+
+_T = TypeVar('_T', bound=Any)
+_D = TypeVar('_D')
+
+
+class _MultiMapping(Protocol[_T, _D]):
+    """Protocol for a multi-mapping type."""
+
+    @abc.abstractmethod
+    def __getitem__(self, __key: str) -> _T: ...
+
+    @overload
+    @abc.abstractmethod
+    def getall(self, key: str) -> list[_T]: ...
+    @overload
+    @abc.abstractmethod
+    def getall(self, key: str, default: _D) -> Union[list[_T], _D]: ...
+    @abc.abstractmethod
+    def getall(self, key: str, default: _D = ...) -> Union[list[_T], _D]: ...
+
+
+class Serializer(Generic[_T]):
+    _type_info: BaseType
+
+    def __init__(
+        self,
+        t: type[_T],
+        *,
+        camelcase_fields: bool = False,
+        omit_none: bool = False,
+        force_default_for_optional: bool = False,
+        naive_datetime_to_utc: bool = False,
+        custom_type_resolver: Optional[Callable[[Any], Optional[CustomType[Any, Any]]]] = None,
+    ) -> None:
+        """
+        Create a serializer for the given type.
+
+        :param t: The type to serialize/deserialize.
+        :param camelcase_fields: If True, the serializer will convert field names to camelCase.
+        :param omit_none: If True, the serializer will omit None values from the output.
+        :param force_default_for_optional: If True, the serializer will force default values for optional fields.
+        :param naive_datetime_to_utc: If True, the serializer will convert naive datetimes to UTC.
+        :param custom_type_resolver: An optional callable that allows users to add support for their own types.
+            This parameter should be a function that takes a type as input and returns an instance of CustomType
+            if the user-defined type is supported, or None otherwise.
+        """
+        if camelcase_fields:
+            t = cast(type[_T], Annotated[t, CamelCase])
+        if omit_none:
+            t = cast(type(_T), Annotated[t, OmitNone])  # type: ignore
+        if force_default_for_optional:
+            t = cast(type(_T), Annotated[t, ForceDefaultForOptional])  # type: ignore
+        self._type_info = describe_type(t, custom_type_resolver=custom_type_resolver)
+        self._schema = get_json_schema(self._type_info)
+        self._encoder: _Serializer[_T] = _Serializer(self._type_info, naive_datetime_to_utc)
+
+    def dump(self, value: _T) -> Any:
+        """Serialize the given value to a JSON-serializable object.
+
+        :param value: The value to serialize.
+        """
+        return self._encoder.dump(value)
+
+    def load(self, data: Any) -> _T:
+        """Deserialize the given JSON-serializable object to the target type.
+
+        :param data: The data to deserialize.
+        """
+        return self._encoder.load(data)
+
+    def load_query_params(self, data: _MultiMapping[Any, Any]) -> _T:
+        """Deserialize the given query parameters to the target type.
+
+        :param data: The query parameters to deserialize.
+        """
+        return self._encoder.load_query_params(data)
+
+    def get_json_schema(self) -> dict[str, Any]:
+        """Get the JSON schema for the target type."""
+        return self._schema
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/_type_utils.py` & `serpyco_rs-1.8.0/python/serpyco_rs/_type_utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,500 +1,500 @@
-# Uses code from https://github.com/python/cpython/pull/111515
-# type: ignore
-import collections.abc
-import functools
-import operator
-import sys
-import types
-from collections import defaultdict
-from types import GenericAlias
-from typing import (
-    Any,
-    ForwardRef,
-    Generic,
-    TypeVar,
-    Union,
-    _AnnotatedAlias,
-    _eval_type,
-    _GenericAlias,
-    _type_check,
-    get_args,
-    get_origin,
-)
-
-from typing_extensions import NotRequired, ParamSpec, Required, TypeVarTuple, is_typeddict
-
-
-_allowed_types = (
-    types.FunctionType,
-    types.BuiltinFunctionType,
-    types.MethodType,
-    types.ModuleType,
-    types.WrapperDescriptorType,
-    types.MethodWrapperType,
-    types.MethodDescriptorType,
-)
-
-
-def get_type_hints(
-    obj: Any,
-    globalns: Union[dict[str, Any], None] = None,
-    localns: Union[dict[str, Any], None] = None,
-    include_extras: bool = False,
-) -> dict[str, Any]:
-    """Return type hints for an object.
-
-    This is often the same as obj.__annotations__, but it handles
-    forward references encoded as string literals, recursively replaces all
-    'Annotated[T, ...]' with 'T' (unless 'include_extras=True'), and resolves
-    type variables to their values as needed.
-
-    The argument may be a module, class, generic alias, method, or function.
-    The annotations are returned as a dictionary. For classes and generic aliases,
-    annotations also include inherited members.
-
-    TypeError is raised if the argument is not of a type that can contain
-    annotations, and an empty dictionary is returned if no annotations are
-    present.
-
-    BEWARE -- the behavior of globalns and localns is counterintuitive
-    (unless you are familiar with how eval() and exec() work).  The
-    search order is locals first, then globals.
-
-    - If no dict arguments are passed, an attempt is made to use the
-      globals from obj (or the respective module's globals for classes),
-      and these are also used as the locals.  If the object does not appear
-      to have globals, an empty dictionary is used.  For classes, the search
-      order is globals first then locals.
-
-    - If one dict argument is passed, it is used for both globals and
-      locals.
-
-    - If two dict arguments are passed, they specify globals and
-      locals, respectively.
-    """
-    if getattr(obj, '__no_type_check__', None):
-        return {}
-
-    # for Generic Aliases we need to inspect the origin
-    # then apply its args later
-    ga_args = None
-    if isinstance(obj, (_GenericAlias, GenericAlias)):
-        ga_args = get_args(obj)
-        obj = get_origin(obj)
-
-    # Classes require a special treatment.
-    if isinstance(obj, type):
-        # track typevars of each base
-        param_tracking = defaultdict(list)
-        # track type hints of each base
-        hint_tracking = {}
-        hints = {}
-        # typeddicts cannot redefine pre-existing keys
-        can_override = not is_typeddict(obj)
-        for base in _get_all_bases(obj):
-            # keep track of typevars and the values they are being
-            # replaced with
-            for cls, args in _track_parameter_changes(base):
-                param_tracking[cls].append(args)
-
-                if cls is not base:
-                    # if we previously scanned it and it found no type hints
-                    # then skip processing it
-                    if not hint_tracking[cls]:
-                        continue
-
-                    to_sub = _substitute_type_hints(param_tracking[cls], hint_tracking[cls])
-                    hints.update(to_sub)
-
-            if globalns is None:
-                base_globals = getattr(sys.modules.get(base.__module__, None), '__dict__', {})
-            else:
-                base_globals = globalns
-            ann = base.__dict__.get('__annotations__', {})
-            if isinstance(ann, types.GetSetDescriptorType):
-                ann = {}
-            base_locals = dict(vars(base)) if localns is None else localns
-            if localns is None and globalns is None:
-                # This is surprising, but required.  Before Python 3.10,
-                # get_type_hints only evaluated the globalns of
-                # a class.  To maintain backwards compatibility, we reverse
-                # the globalns and localns order so that eval() looks into
-                # *base_globals* first rather than *base_locals*.
-                # This only affects ForwardRefs.
-                base_globals, base_locals = base_locals, base_globals
-
-            hint_tracking[base] = {}
-            for name, value in ann.items():
-                # skip pre-existing keys for typeddict
-                if not can_override and name in hints:
-                    continue
-
-                if value is None:
-                    value = type(None)
-                if isinstance(value, str):
-                    value = ForwardRef(value, is_argument=False, is_class=True)
-                value = _eval_type(value, base_globals, base_locals)
-                hint_tracking[base][name] = value
-                hints[name] = value
-
-        # sub the original args back in
-        if ga_args is not None:
-            param_tracking[obj].append(ga_args)
-            to_sub = _substitute_type_hints(param_tracking[obj], hints)
-            hints.update(to_sub)
-
-        return hints if include_extras else {k: _strip_annotations(t) for k, t in hints.items()}
-
-    if globalns is None:
-        if isinstance(obj, types.ModuleType):
-            globalns = obj.__dict__
-        else:
-            nsobj = obj
-            # Find globalns for the unwrapped object.
-            while hasattr(nsobj, '__wrapped__'):
-                nsobj = nsobj.__wrapped__
-            globalns = getattr(nsobj, '__globals__', {})
-        if localns is None:
-            localns = globalns
-    elif localns is None:
-        localns = globalns
-    hints = getattr(obj, '__annotations__', None)
-    if hints is None:
-        # Return empty annotations for something that _could_ have them.
-        if isinstance(obj, _allowed_types):
-            return {}
-        else:  # noqa: RET505
-            raise TypeError(f'{obj!r} is not a module, class, method, ' 'or function.')
-    hints = dict(hints)
-    for name, value in hints.items():
-        if value is None:
-            value = type(None)
-        if isinstance(value, str):
-            # class-level forward refs were handled above, this must be either
-            # a module-level annotation or a function argument annotation
-            value = ForwardRef(
-                value,
-                is_argument=not isinstance(obj, types.ModuleType),
-                is_class=False,
-            )
-        hints[name] = _eval_type(value, globalns, localns)
-    return hints if include_extras else {k: _strip_annotations(t) for k, t in hints.items()}
-
-
-def _substitute_type_hints(substitutions: 'list[tuple[Any, ...]]', hints: 'dict[str, Any]'):
-    # nothing to substitute
-    if len(substitutions) < 2:
-        return {}
-
-    previous_params = substitutions[-2]
-    new_params = substitutions[-1]
-    new_substitutions = _repack_args(previous_params, new_params)
-
-    # get a mapping of typevar to value
-    mapping = {}
-    for i in range(len(previous_params)):
-        current = previous_params[i]
-        # if the previous parameter is *Ts
-        # make it {Ts: new Ts or value}
-        if _is_unpacked_typevartuple(current):
-            (previous_typevartuple,) = get_args(current)
-            new_value = new_substitutions[i]
-
-            if _is_unpacked_typevartuple(new_value):
-                (new_value,) = get_args(new_value)
-
-            mapping[previous_typevartuple] = new_value
-        else:
-            mapping[current] = new_substitutions[i]
-
-    hints_to_replace = {}
-
-    for name, value in hints.items():
-        origin = get_origin(value)
-        # if the typevar is nested, we must substitute the typevar all the way down.
-        if origin is not None:
-            new_args = tuple(_make_substitution(origin, get_args(value), mapping))
-            sub = _copy_with(value, new_args)
-        elif _is_typevar_like(value):
-            # https://github.com/python/cpython/pull/111515#issuecomment-2018336687
-            # sub = mapping[value]  # old
-            sub = mapping.get(value, value)
-        else:
-            continue
-
-        hints_to_replace[name] = sub
-
-    return hints_to_replace
-
-
-def _copy_with(t, new_args):
-    if new_args == t.__args__:
-        return t
-    if isinstance(t, GenericAlias):
-        return GenericAlias(t.__origin__, new_args)
-    if isinstance(t, _AnnotatedAlias):  # https://github.com/python/cpython/pull/111515#issuecomment-2018132920
-        return t.copy_with(new_args[:1])
-    if hasattr(types, 'UnionType') and isinstance(t, types.UnionType):
-        return functools.reduce(operator.or_, new_args)
-    else:  # noqa: RET505
-        return t.copy_with(new_args)
-
-
-def _make_substitution(origin, args, new_arg_by_param):
-    """Create a list of new type arguments."""
-    new_args = []
-    for old_arg in args:
-        if isinstance(old_arg, type):
-            new_args.append(old_arg)
-            continue
-
-        substfunc = getattr(old_arg, '__typing_subst__', None)
-        if substfunc:
-            new_arg = substfunc(new_arg_by_param[old_arg])
-        elif isinstance(old_arg, TypeVar) and sys.version_info[:2] <= (3, 10):
-            new_arg = _typevar_subst(new_arg_by_param[old_arg])
-        else:
-            subparams = getattr(old_arg, '__parameters__', ())
-            if not subparams:
-                new_arg = old_arg
-            else:
-                subargs = []
-                for x in subparams:
-                    if isinstance(x, TypeVarTuple):
-                        subargs.extend(new_arg_by_param[x])
-                    else:
-                        subargs.append(new_arg_by_param[x])
-                new_arg = old_arg[tuple(subargs)]
-
-        if origin == collections.abc.Callable and isinstance(new_arg, tuple):
-            # Consider the following `Callable`.
-            #   C = Callable[[int], str]
-            # Here, `C.__args__` should be (int, str) - NOT ([int], str).
-            # That means that if we had something like...
-            #   P = ParamSpec('P')
-            #   T = TypeVar('T')
-            #   C = Callable[P, T]
-            #   D = C[[int, str], float]
-            # ...we need to be careful; `new_args` should end up as
-            # `(int, str, float)` rather than `([int, str], float)`.
-            new_args.extend(new_arg)
-        elif _is_unpacked_typevartuple(old_arg):
-            # Consider the following `_GenericAlias`, `B`:
-            #   class A(Generic[*Ts]): ...
-            #   B = A[T, *Ts]
-            # If we then do:
-            #   B[float, int, str]
-            # The `new_arg` corresponding to `T` will be `float`, and the
-            # `new_arg` corresponding to `*Ts` will be `(int, str)`. We
-            # should join all these types together in a flat list
-            # `(float, int, str)` - so again, we should `extend`.
-            new_args.extend(new_arg)
-        elif isinstance(old_arg, tuple):
-            # Corner case:
-            #    P = ParamSpec('P')
-            #    T = TypeVar('T')
-            #    class Base(Generic[P]): ...
-            # Can be substituted like this:
-            #    X = Base[[int, T]]
-            # In this case, `old_arg` will be a tuple:
-            new_args.append(
-                tuple(_make_substitution(origin, old_arg, new_arg_by_param)),
-            )
-        else:
-            new_args.append(new_arg)
-    return new_args
-
-
-def _repack_args(reference, params):
-    """transforms params to match the requested arguments
-    of reference.
-
-    >>> _repack_args((T, U, *Ts), (int, str, float, bool))
-    (int, str, (float, bool))
-    >>> _repack_args((T, U, *Ts), (int, str, *Ts))
-    (int, str, *Ts)
-    """
-
-    # find bounds of potential typevar tuple
-    tuple_start, tuple_end = 0, None
-    found_typvartuple = False
-    for i, tv in enumerate(reference):
-        if _is_unpacked_typevartuple(tv) or isinstance(tv, TypeVarTuple):
-            tuple_start = i
-            found_typvartuple = True
-        elif found_typvartuple:
-            tuple_end = i
-            break
-
-    if found_typvartuple:
-        # if typevartuple doesnt consume rest
-        if tuple_end is not None:
-            tuple_end = tuple_end - len(reference)
-
-        # tuple of typevars
-        type_var_tuple_params = params[tuple_start:tuple_end]
-
-        # if params might contain typevartuple args
-        if len(params) > tuple_start:  # noqa: SIM102
-            # if params[tuple_start] is *Ts keep it as-is
-            if _is_unpacked_typevartuple(params[tuple_start]):
-                type_var_tuple_params = params[tuple_start]
-
-        # if starts with type var tuple
-        if tuple_start == 0:
-            # if there are type vars after it
-            if tuple_end is not None:
-                return (type_var_tuple_params, *params[tuple_end:])
-            return (type_var_tuple_params,)
-        # if it's at the end
-        elif tuple_end is None:  # noqa: RET505
-            return (*params[:tuple_start], type_var_tuple_params)
-        # if it's in the middle
-        return (*params[:tuple_start], type_var_tuple_params, *params[tuple_end:])
-    return params
-
-
-def _is_unpacked_typevartuple(x: Any) -> bool:
-    return (not isinstance(x, type)) and getattr(x, '__typing_is_unpacked_typevartuple__', False)
-
-
-def _is_typevar_like(x: Any) -> bool:
-    return isinstance(x, (TypeVar, ParamSpec)) or _is_unpacked_typevartuple(x)
-
-
-def _get_all_bases(cls):
-    """Correctly obtains the bases for classes
-    and typeddicts alike.
-    """
-    mro = reversed(cls.__mro__)
-
-    if not is_typeddict(cls):
-        yield from mro
-        return
-
-    traversing = list(mro)
-    visited = []
-
-    while traversing:
-        base = traversing.pop(0)
-
-        orig_bases = getattr(base, '__orig_bases__', ())
-        mro_changed = False
-
-        for orig_base in orig_bases:
-            origin = get_origin(orig_base)
-
-            if origin is not Generic:
-                new_base = orig_base if origin is None else origin
-                if new_base not in visited:
-                    traversing.insert(0, new_base)
-                    traversing.insert(1, base)
-                    mro_changed = True
-
-        if mro_changed:
-            continue
-
-        yield base
-
-        visited.append(base)
-
-
-def _track_parameter_changes(base):
-    """Track how a parameters values are substituted
-    or changed while traversing its bases.
-    """
-    orig_bases = getattr(base, '__orig_bases__', ())
-    generic_encountered = False
-
-    for orig_base in orig_bases:
-        origin = get_origin(orig_base)
-        if origin is None:
-            continue
-
-        args = get_args(orig_base)
-
-        if origin is Generic:
-            generic_encountered = True
-            yield base, args
-        else:
-            yield origin, args
-
-    # this occurs if obj is
-    # class Bar(Foo[str, U]): ...
-    # in this case, we need to imagine there's a generic base
-    # with the required typevars here.
-    if orig_bases and not generic_encountered:
-        # we need to collect all the typevars from all bases
-        # in the case that they have multiple generic bases
-        # class Baz(Foo[str, U], Bar[U, T]): ...
-        type_vars_for_generic = _collect_parameters(orig_bases)
-
-        # this may be empty if obj is
-        # class Bar(Foo[str]): ...
-        # we can skip adding typevars here.
-        if type_vars_for_generic:
-            yield base, type_vars_for_generic
-
-
-def _collect_parameters(args):
-    """Collect all type variables and parameter specifications in args
-    in order of first appearance (lexicographic order).
-
-    For example::
-
-        assert _collect_parameters((T, Callable[P, T])) == (T, P)
-    """
-    parameters = []
-    for t in args:
-        if isinstance(t, type):
-            # We don't want __parameters__ descriptor of a bare Python class.
-            pass
-        elif isinstance(t, tuple):
-            # `t` might be a tuple, when `ParamSpec` is substituted with
-            # `[T, int]`, or `[int, *Ts]`, etc.
-            for x in t:
-                for collected in _collect_parameters([x]):
-                    if collected not in parameters:
-                        parameters.append(collected)
-        elif hasattr(t, '__typing_subst__'):
-            if t not in parameters:
-                parameters.append(t)
-        else:
-            for x in getattr(t, '__parameters__', ()):
-                if x not in parameters:
-                    parameters.append(x)
-    return tuple(parameters)
-
-
-def _strip_annotations(t):
-    """Strip the annotations from a given type."""
-    if isinstance(t, _AnnotatedAlias):
-        return _strip_annotations(t.__origin__)
-    if hasattr(t, '__origin__') and t.__origin__ in (Required, NotRequired):
-        return _strip_annotations(t.__args__[0])
-    if isinstance(t, _GenericAlias):
-        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
-        if stripped_args == t.__args__:
-            return t
-        return t.copy_with(stripped_args)
-    if isinstance(t, GenericAlias):
-        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
-        if stripped_args == t.__args__:
-            return t
-        return GenericAlias(t.__origin__, stripped_args)
-    if hasattr(types, 'UnionType') and isinstance(t, types.UnionType):
-        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
-        if stripped_args == t.__args__:
-            return t
-        return functools.reduce(operator.or_, stripped_args)
-
-    return t
-
-
-# python 3.9 / 3.10 compatibility
-
-
-def _typevar_subst(arg):
-    msg = 'Parameters to generic types must be types.'
-    arg = _type_check(arg, msg, is_argument=True)
-    return arg
+# Uses code from https://github.com/python/cpython/pull/111515
+# type: ignore
+import collections.abc
+import functools
+import operator
+import sys
+import types
+from collections import defaultdict
+from types import GenericAlias
+from typing import (
+    Any,
+    ForwardRef,
+    Generic,
+    TypeVar,
+    Union,
+    _AnnotatedAlias,
+    _eval_type,
+    _GenericAlias,
+    _type_check,
+    get_args,
+    get_origin,
+)
+
+from typing_extensions import NotRequired, ParamSpec, Required, TypeVarTuple, is_typeddict
+
+
+_allowed_types = (
+    types.FunctionType,
+    types.BuiltinFunctionType,
+    types.MethodType,
+    types.ModuleType,
+    types.WrapperDescriptorType,
+    types.MethodWrapperType,
+    types.MethodDescriptorType,
+)
+
+
+def get_type_hints(
+    obj: Any,
+    globalns: Union[dict[str, Any], None] = None,
+    localns: Union[dict[str, Any], None] = None,
+    include_extras: bool = False,
+) -> dict[str, Any]:
+    """Return type hints for an object.
+
+    This is often the same as obj.__annotations__, but it handles
+    forward references encoded as string literals, recursively replaces all
+    'Annotated[T, ...]' with 'T' (unless 'include_extras=True'), and resolves
+    type variables to their values as needed.
+
+    The argument may be a module, class, generic alias, method, or function.
+    The annotations are returned as a dictionary. For classes and generic aliases,
+    annotations also include inherited members.
+
+    TypeError is raised if the argument is not of a type that can contain
+    annotations, and an empty dictionary is returned if no annotations are
+    present.
+
+    BEWARE -- the behavior of globalns and localns is counterintuitive
+    (unless you are familiar with how eval() and exec() work).  The
+    search order is locals first, then globals.
+
+    - If no dict arguments are passed, an attempt is made to use the
+      globals from obj (or the respective module's globals for classes),
+      and these are also used as the locals.  If the object does not appear
+      to have globals, an empty dictionary is used.  For classes, the search
+      order is globals first then locals.
+
+    - If one dict argument is passed, it is used for both globals and
+      locals.
+
+    - If two dict arguments are passed, they specify globals and
+      locals, respectively.
+    """
+    if getattr(obj, '__no_type_check__', None):
+        return {}
+
+    # for Generic Aliases we need to inspect the origin
+    # then apply its args later
+    ga_args = None
+    if isinstance(obj, (_GenericAlias, GenericAlias)):
+        ga_args = get_args(obj)
+        obj = get_origin(obj)
+
+    # Classes require a special treatment.
+    if isinstance(obj, type):
+        # track typevars of each base
+        param_tracking = defaultdict(list)
+        # track type hints of each base
+        hint_tracking = {}
+        hints = {}
+        # typeddicts cannot redefine pre-existing keys
+        can_override = not is_typeddict(obj)
+        for base in _get_all_bases(obj):
+            # keep track of typevars and the values they are being
+            # replaced with
+            for cls, args in _track_parameter_changes(base):
+                param_tracking[cls].append(args)
+
+                if cls is not base:
+                    # if we previously scanned it and it found no type hints
+                    # then skip processing it
+                    if not hint_tracking[cls]:
+                        continue
+
+                    to_sub = _substitute_type_hints(param_tracking[cls], hint_tracking[cls])
+                    hints.update(to_sub)
+
+            if globalns is None:
+                base_globals = getattr(sys.modules.get(base.__module__, None), '__dict__', {})
+            else:
+                base_globals = globalns
+            ann = base.__dict__.get('__annotations__', {})
+            if isinstance(ann, types.GetSetDescriptorType):
+                ann = {}
+            base_locals = dict(vars(base)) if localns is None else localns
+            if localns is None and globalns is None:
+                # This is surprising, but required.  Before Python 3.10,
+                # get_type_hints only evaluated the globalns of
+                # a class.  To maintain backwards compatibility, we reverse
+                # the globalns and localns order so that eval() looks into
+                # *base_globals* first rather than *base_locals*.
+                # This only affects ForwardRefs.
+                base_globals, base_locals = base_locals, base_globals
+
+            hint_tracking[base] = {}
+            for name, value in ann.items():
+                # skip pre-existing keys for typeddict
+                if not can_override and name in hints:
+                    continue
+
+                if value is None:
+                    value = type(None)
+                if isinstance(value, str):
+                    value = ForwardRef(value, is_argument=False, is_class=True)
+                value = _eval_type(value, base_globals, base_locals)
+                hint_tracking[base][name] = value
+                hints[name] = value
+
+        # sub the original args back in
+        if ga_args is not None:
+            param_tracking[obj].append(ga_args)
+            to_sub = _substitute_type_hints(param_tracking[obj], hints)
+            hints.update(to_sub)
+
+        return hints if include_extras else {k: _strip_annotations(t) for k, t in hints.items()}
+
+    if globalns is None:
+        if isinstance(obj, types.ModuleType):
+            globalns = obj.__dict__
+        else:
+            nsobj = obj
+            # Find globalns for the unwrapped object.
+            while hasattr(nsobj, '__wrapped__'):
+                nsobj = nsobj.__wrapped__
+            globalns = getattr(nsobj, '__globals__', {})
+        if localns is None:
+            localns = globalns
+    elif localns is None:
+        localns = globalns
+    hints = getattr(obj, '__annotations__', None)
+    if hints is None:
+        # Return empty annotations for something that _could_ have them.
+        if isinstance(obj, _allowed_types):
+            return {}
+        else:  # noqa: RET505
+            raise TypeError(f'{obj!r} is not a module, class, method, ' 'or function.')
+    hints = dict(hints)
+    for name, value in hints.items():
+        if value is None:
+            value = type(None)
+        if isinstance(value, str):
+            # class-level forward refs were handled above, this must be either
+            # a module-level annotation or a function argument annotation
+            value = ForwardRef(
+                value,
+                is_argument=not isinstance(obj, types.ModuleType),
+                is_class=False,
+            )
+        hints[name] = _eval_type(value, globalns, localns)
+    return hints if include_extras else {k: _strip_annotations(t) for k, t in hints.items()}
+
+
+def _substitute_type_hints(substitutions: 'list[tuple[Any, ...]]', hints: 'dict[str, Any]'):
+    # nothing to substitute
+    if len(substitutions) < 2:
+        return {}
+
+    previous_params = substitutions[-2]
+    new_params = substitutions[-1]
+    new_substitutions = _repack_args(previous_params, new_params)
+
+    # get a mapping of typevar to value
+    mapping = {}
+    for i in range(len(previous_params)):
+        current = previous_params[i]
+        # if the previous parameter is *Ts
+        # make it {Ts: new Ts or value}
+        if _is_unpacked_typevartuple(current):
+            (previous_typevartuple,) = get_args(current)
+            new_value = new_substitutions[i]
+
+            if _is_unpacked_typevartuple(new_value):
+                (new_value,) = get_args(new_value)
+
+            mapping[previous_typevartuple] = new_value
+        else:
+            mapping[current] = new_substitutions[i]
+
+    hints_to_replace = {}
+
+    for name, value in hints.items():
+        origin = get_origin(value)
+        # if the typevar is nested, we must substitute the typevar all the way down.
+        if origin is not None:
+            new_args = tuple(_make_substitution(origin, get_args(value), mapping))
+            sub = _copy_with(value, new_args)
+        elif _is_typevar_like(value):
+            # https://github.com/python/cpython/pull/111515#issuecomment-2018336687
+            # sub = mapping[value]  # old
+            sub = mapping.get(value, value)
+        else:
+            continue
+
+        hints_to_replace[name] = sub
+
+    return hints_to_replace
+
+
+def _copy_with(t, new_args):
+    if new_args == t.__args__:
+        return t
+    if isinstance(t, GenericAlias):
+        return GenericAlias(t.__origin__, new_args)
+    if isinstance(t, _AnnotatedAlias):  # https://github.com/python/cpython/pull/111515#issuecomment-2018132920
+        return t.copy_with(new_args[:1])
+    if hasattr(types, 'UnionType') and isinstance(t, types.UnionType):
+        return functools.reduce(operator.or_, new_args)
+    else:  # noqa: RET505
+        return t.copy_with(new_args)
+
+
+def _make_substitution(origin, args, new_arg_by_param):
+    """Create a list of new type arguments."""
+    new_args = []
+    for old_arg in args:
+        if isinstance(old_arg, type):
+            new_args.append(old_arg)
+            continue
+
+        substfunc = getattr(old_arg, '__typing_subst__', None)
+        if substfunc:
+            new_arg = substfunc(new_arg_by_param[old_arg])
+        elif isinstance(old_arg, TypeVar) and sys.version_info[:2] <= (3, 10):
+            new_arg = _typevar_subst(new_arg_by_param[old_arg])
+        else:
+            subparams = getattr(old_arg, '__parameters__', ())
+            if not subparams:
+                new_arg = old_arg
+            else:
+                subargs = []
+                for x in subparams:
+                    if isinstance(x, TypeVarTuple):
+                        subargs.extend(new_arg_by_param[x])
+                    else:
+                        subargs.append(new_arg_by_param[x])
+                new_arg = old_arg[tuple(subargs)]
+
+        if origin == collections.abc.Callable and isinstance(new_arg, tuple):
+            # Consider the following `Callable`.
+            #   C = Callable[[int], str]
+            # Here, `C.__args__` should be (int, str) - NOT ([int], str).
+            # That means that if we had something like...
+            #   P = ParamSpec('P')
+            #   T = TypeVar('T')
+            #   C = Callable[P, T]
+            #   D = C[[int, str], float]
+            # ...we need to be careful; `new_args` should end up as
+            # `(int, str, float)` rather than `([int, str], float)`.
+            new_args.extend(new_arg)
+        elif _is_unpacked_typevartuple(old_arg):
+            # Consider the following `_GenericAlias`, `B`:
+            #   class A(Generic[*Ts]): ...
+            #   B = A[T, *Ts]
+            # If we then do:
+            #   B[float, int, str]
+            # The `new_arg` corresponding to `T` will be `float`, and the
+            # `new_arg` corresponding to `*Ts` will be `(int, str)`. We
+            # should join all these types together in a flat list
+            # `(float, int, str)` - so again, we should `extend`.
+            new_args.extend(new_arg)
+        elif isinstance(old_arg, tuple):
+            # Corner case:
+            #    P = ParamSpec('P')
+            #    T = TypeVar('T')
+            #    class Base(Generic[P]): ...
+            # Can be substituted like this:
+            #    X = Base[[int, T]]
+            # In this case, `old_arg` will be a tuple:
+            new_args.append(
+                tuple(_make_substitution(origin, old_arg, new_arg_by_param)),
+            )
+        else:
+            new_args.append(new_arg)
+    return new_args
+
+
+def _repack_args(reference, params):
+    """transforms params to match the requested arguments
+    of reference.
+
+    >>> _repack_args((T, U, *Ts), (int, str, float, bool))
+    (int, str, (float, bool))
+    >>> _repack_args((T, U, *Ts), (int, str, *Ts))
+    (int, str, *Ts)
+    """
+
+    # find bounds of potential typevar tuple
+    tuple_start, tuple_end = 0, None
+    found_typvartuple = False
+    for i, tv in enumerate(reference):
+        if _is_unpacked_typevartuple(tv) or isinstance(tv, TypeVarTuple):
+            tuple_start = i
+            found_typvartuple = True
+        elif found_typvartuple:
+            tuple_end = i
+            break
+
+    if found_typvartuple:
+        # if typevartuple doesnt consume rest
+        if tuple_end is not None:
+            tuple_end = tuple_end - len(reference)
+
+        # tuple of typevars
+        type_var_tuple_params = params[tuple_start:tuple_end]
+
+        # if params might contain typevartuple args
+        if len(params) > tuple_start:  # noqa: SIM102
+            # if params[tuple_start] is *Ts keep it as-is
+            if _is_unpacked_typevartuple(params[tuple_start]):
+                type_var_tuple_params = params[tuple_start]
+
+        # if starts with type var tuple
+        if tuple_start == 0:
+            # if there are type vars after it
+            if tuple_end is not None:
+                return (type_var_tuple_params, *params[tuple_end:])
+            return (type_var_tuple_params,)
+        # if it's at the end
+        elif tuple_end is None:  # noqa: RET505
+            return (*params[:tuple_start], type_var_tuple_params)
+        # if it's in the middle
+        return (*params[:tuple_start], type_var_tuple_params, *params[tuple_end:])
+    return params
+
+
+def _is_unpacked_typevartuple(x: Any) -> bool:
+    return (not isinstance(x, type)) and getattr(x, '__typing_is_unpacked_typevartuple__', False)
+
+
+def _is_typevar_like(x: Any) -> bool:
+    return isinstance(x, (TypeVar, ParamSpec)) or _is_unpacked_typevartuple(x)
+
+
+def _get_all_bases(cls):
+    """Correctly obtains the bases for classes
+    and typeddicts alike.
+    """
+    mro = reversed(cls.__mro__)
+
+    if not is_typeddict(cls):
+        yield from mro
+        return
+
+    traversing = list(mro)
+    visited = []
+
+    while traversing:
+        base = traversing.pop(0)
+
+        orig_bases = getattr(base, '__orig_bases__', ())
+        mro_changed = False
+
+        for orig_base in orig_bases:
+            origin = get_origin(orig_base)
+
+            if origin is not Generic:
+                new_base = orig_base if origin is None else origin
+                if new_base not in visited:
+                    traversing.insert(0, new_base)
+                    traversing.insert(1, base)
+                    mro_changed = True
+
+        if mro_changed:
+            continue
+
+        yield base
+
+        visited.append(base)
+
+
+def _track_parameter_changes(base):
+    """Track how a parameters values are substituted
+    or changed while traversing its bases.
+    """
+    orig_bases = getattr(base, '__orig_bases__', ())
+    generic_encountered = False
+
+    for orig_base in orig_bases:
+        origin = get_origin(orig_base)
+        if origin is None:
+            continue
+
+        args = get_args(orig_base)
+
+        if origin is Generic:
+            generic_encountered = True
+            yield base, args
+        else:
+            yield origin, args
+
+    # this occurs if obj is
+    # class Bar(Foo[str, U]): ...
+    # in this case, we need to imagine there's a generic base
+    # with the required typevars here.
+    if orig_bases and not generic_encountered:
+        # we need to collect all the typevars from all bases
+        # in the case that they have multiple generic bases
+        # class Baz(Foo[str, U], Bar[U, T]): ...
+        type_vars_for_generic = _collect_parameters(orig_bases)
+
+        # this may be empty if obj is
+        # class Bar(Foo[str]): ...
+        # we can skip adding typevars here.
+        if type_vars_for_generic:
+            yield base, type_vars_for_generic
+
+
+def _collect_parameters(args):
+    """Collect all type variables and parameter specifications in args
+    in order of first appearance (lexicographic order).
+
+    For example::
+
+        assert _collect_parameters((T, Callable[P, T])) == (T, P)
+    """
+    parameters = []
+    for t in args:
+        if isinstance(t, type):
+            # We don't want __parameters__ descriptor of a bare Python class.
+            pass
+        elif isinstance(t, tuple):
+            # `t` might be a tuple, when `ParamSpec` is substituted with
+            # `[T, int]`, or `[int, *Ts]`, etc.
+            for x in t:
+                for collected in _collect_parameters([x]):
+                    if collected not in parameters:
+                        parameters.append(collected)
+        elif hasattr(t, '__typing_subst__'):
+            if t not in parameters:
+                parameters.append(t)
+        else:
+            for x in getattr(t, '__parameters__', ()):
+                if x not in parameters:
+                    parameters.append(x)
+    return tuple(parameters)
+
+
+def _strip_annotations(t):
+    """Strip the annotations from a given type."""
+    if isinstance(t, _AnnotatedAlias):
+        return _strip_annotations(t.__origin__)
+    if hasattr(t, '__origin__') and t.__origin__ in (Required, NotRequired):
+        return _strip_annotations(t.__args__[0])
+    if isinstance(t, _GenericAlias):
+        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return t.copy_with(stripped_args)
+    if isinstance(t, GenericAlias):
+        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return GenericAlias(t.__origin__, stripped_args)
+    if hasattr(types, 'UnionType') and isinstance(t, types.UnionType):
+        stripped_args = tuple(_strip_annotations(a) for a in t.__args__)
+        if stripped_args == t.__args__:
+            return t
+        return functools.reduce(operator.or_, stripped_args)
+
+    return t
+
+
+# python 3.9 / 3.10 compatibility
+
+
+def _typevar_subst(arg):
+    msg = 'Parameters to generic types must be types.'
+    arg = _type_check(arg, msg, is_argument=True)
+    return arg
```

### Comparing `serpyco_rs-1.7.1/python/serpyco_rs/metadata.py` & `serpyco_rs-1.8.0/python/serpyco_rs/metadata.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from collections.abc import Callable
-from dataclasses import dataclass
-from enum import Enum
-from typing import TypeVar, Union
-
-from ._impl import CustomEncoder
-
-
-@dataclass(frozen=True)
-class Min:
-    value: Union[int, float]
-
-
-@dataclass(frozen=True)
-class Max:
-    value: Union[int, float]
-
-
-@dataclass(frozen=True)
-class MinLength:
-    value: int
-
-
-@dataclass(frozen=True)
-class MaxLength:
-    value: int
-
-
-@dataclass(frozen=True)
-class Discriminator:
-    name: str
-
-
-@dataclass(frozen=True)
-class Alias:
-    value: str
-
-
-class Format(Enum):
-    no_format = 'no_format'
-    camel_case = 'camel_case'
-
-
-@dataclass(frozen=True)
-class FieldFormat:
-    format: Format
-
-
-CamelCase: FieldFormat = FieldFormat(Format.camel_case)
-NoFormat: FieldFormat = FieldFormat(Format.no_format)
-
-
-@dataclass(frozen=True)
-class NoneFormat:
-    omit: bool
-
-
-KeepNone: NoneFormat = NoneFormat(False)
-OmitNone: NoneFormat = NoneFormat(True)
-
-
-@dataclass(frozen=True)
-class NoneAsDefaultForOptional:
-    use: bool
-
-
-ForceDefaultForOptional: NoneAsDefaultForOptional = NoneAsDefaultForOptional(True)
-KeepDefaultForOptional: NoneAsDefaultForOptional = NoneAsDefaultForOptional(False)
-
-
-_I = TypeVar('_I')
-_O = TypeVar('_O')
-
-
-def serialize_with(func: Callable[[_I], _O]) -> CustomEncoder[_I, _O]:
-    return CustomEncoder[_I, _O](serialize=func)
-
-
-def deserialize_with(func: Callable[[_O], _I]) -> CustomEncoder[_I, _O]:
-    return CustomEncoder[_I, _O](deserialize=func)
+from collections.abc import Callable
+from dataclasses import dataclass
+from enum import Enum
+from typing import TypeVar, Union
+
+from ._impl import CustomEncoder
+
+
+@dataclass(frozen=True)
+class Min:
+    value: Union[int, float]
+
+
+@dataclass(frozen=True)
+class Max:
+    value: Union[int, float]
+
+
+@dataclass(frozen=True)
+class MinLength:
+    value: int
+
+
+@dataclass(frozen=True)
+class MaxLength:
+    value: int
+
+
+@dataclass(frozen=True)
+class Discriminator:
+    name: str
+
+
+@dataclass(frozen=True)
+class Alias:
+    value: str
+
+
+class Format(Enum):
+    no_format = 'no_format'
+    camel_case = 'camel_case'
+
+
+@dataclass(frozen=True)
+class FieldFormat:
+    format: Format
+
+
+CamelCase: FieldFormat = FieldFormat(Format.camel_case)
+NoFormat: FieldFormat = FieldFormat(Format.no_format)
+
+
+@dataclass(frozen=True)
+class NoneFormat:
+    omit: bool
+
+
+KeepNone: NoneFormat = NoneFormat(False)
+OmitNone: NoneFormat = NoneFormat(True)
+
+
+@dataclass(frozen=True)
+class NoneAsDefaultForOptional:
+    use: bool
+
+
+ForceDefaultForOptional: NoneAsDefaultForOptional = NoneAsDefaultForOptional(True)
+KeepDefaultForOptional: NoneAsDefaultForOptional = NoneAsDefaultForOptional(False)
+
+
+_I = TypeVar('_I')
+_O = TypeVar('_O')
+
+
+def serialize_with(func: Callable[[_I], _O]) -> CustomEncoder[_I, _O]:
+    return CustomEncoder[_I, _O](serialize=func)
+
+
+def deserialize_with(func: Callable[[_O], _I]) -> CustomEncoder[_I, _O]:
+    return CustomEncoder[_I, _O](deserialize=func)
```

### Comparing `serpyco_rs-1.7.1/ruff.toml` & `serpyco_rs-1.8.0/ruff.toml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-line-length = 120
-src = ["python/serpyco_rs", "tests"]
-exclude = ["pyproject.toml"]
-target-version = "py39"
-
-[lint]
-select = [
-    "F", # Pyflakes
-    "E", # Pycodestyle Error
-    "W", # PycodeStyle Warning
-    "I", # Isort
-    "N", # pep8-naming
-    "UP", # pyupgrade
-    "YTT", # flake8-2020
-    "B", # flake8-bugbear
-    "C4", # flake8-comprehensions
-    "DTZ", # flake8-datetimez
-    "T10", # flake8-debugger
-    "ISC", # flake8-implicit-str-concat
-    "G", # flake8-logging-format
-    "PIE", # flake8-pie
-    "T20", # flake8-print
-    "PYI", # flake8-pyi
-    "Q", # flake8-quotes
-    "RSE", # flake8-raise
-    "RET", # flake8-return
-    "SIM", # flake8-simplify
-    "TID", # flake8-tidy-imports
-    "PTH", # flake8-use-pathlib
-    "PGH", # pygrep-hooks
-    "PL", # Pylint
-    "TRY", # tryceratops
-    "RUF",  # Ruff-specific rules
-]
-
-ignore = [
-    "F401", # unused-import
-    "UP040", # non-pep695-type-alias
-    "B005", # strip-with-multi-characters
-    "B905", # zip-without-explicit-strict
-    "N818", # error-suffix-on-exception-name
-    "ISC001", # single-line-implicit-string-concatenation
-    "Q003", # avoidable-escaped-quote
-    "SIM108", # if-else-block-instead-of-if-exp
-    "SIM212", # if-expr-with-twisted-arms
-    "PTH123", # builtin-open
-    "PLR0911", # too-many-return-statements
-    "PLR0912", # too-many-branches
-    "PLR0913", # too-many-arguments
-    "PLR0915", # too-many-statements
-    "PLR2004", # magic-value-comparison
-    "PLW2901", # redefined-loop-name
-    "SIM300", # yoda-conditions
-    "TID252", # relative-imports
-    "PGH004", # blanket-noqa
-    "TRY002", # raise-vanilla-class
-    "TRY003", # raise-vanilla-args
-    "RUF001", # ambiguous-unicode-character-string
-    "RUF002", # ambiguous-unicode-character-docstring
-    "RUF003", # ambiguous-unicode-character-comment
-    "RUF005", # collection-literal-concatenation
-    "RUF006", # asyncio-dangling-task
-    "RUF012", # mutable-class-default
-    "RET504", # unnecessary-assign
-    "TRY004", # type-check-without-type-error
-    "PGH003", # blanket-type-ignore (todo: fix this)
-]
-
-[lint.per-file-ignores]
-"python/serpyco_rs/_impl.pyi" = [
-    "I001",
-]
-"python/serpyco_rs/_impl.py" = [
-    "I001",
-]
-"python/serpyco_rs/_json_schema/_entities.py" = [
-    "N815", # mixed-case-variable-name
-]
-
-[lint.flake8-quotes]
-inline-quotes = "single"
-
-[lint.isort]
-combine-as-imports = true
-lines-after-imports = 2
-no-lines-before = ["local-folder"]
-
-[format]
-quote-style = "single"
+line-length = 120
+src = ["python/serpyco_rs", "tests"]
+exclude = ["pyproject.toml"]
+target-version = "py39"
+
+[lint]
+select = [
+    "F", # Pyflakes
+    "E", # Pycodestyle Error
+    "W", # PycodeStyle Warning
+    "I", # Isort
+    "N", # pep8-naming
+    "UP", # pyupgrade
+    "YTT", # flake8-2020
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "DTZ", # flake8-datetimez
+    "T10", # flake8-debugger
+    "ISC", # flake8-implicit-str-concat
+    "G", # flake8-logging-format
+    "PIE", # flake8-pie
+    "T20", # flake8-print
+    "PYI", # flake8-pyi
+    "Q", # flake8-quotes
+    "RSE", # flake8-raise
+    "RET", # flake8-return
+    "SIM", # flake8-simplify
+    "TID", # flake8-tidy-imports
+    "PTH", # flake8-use-pathlib
+    "PGH", # pygrep-hooks
+    "PL", # Pylint
+    "TRY", # tryceratops
+    "RUF",  # Ruff-specific rules
+]
+
+ignore = [
+    "F401", # unused-import
+    "UP040", # non-pep695-type-alias
+    "B005", # strip-with-multi-characters
+    "B905", # zip-without-explicit-strict
+    "N818", # error-suffix-on-exception-name
+    "ISC001", # single-line-implicit-string-concatenation
+    "Q003", # avoidable-escaped-quote
+    "SIM108", # if-else-block-instead-of-if-exp
+    "SIM212", # if-expr-with-twisted-arms
+    "PTH123", # builtin-open
+    "PLR0911", # too-many-return-statements
+    "PLR0912", # too-many-branches
+    "PLR0913", # too-many-arguments
+    "PLR0915", # too-many-statements
+    "PLR2004", # magic-value-comparison
+    "PLW2901", # redefined-loop-name
+    "SIM300", # yoda-conditions
+    "TID252", # relative-imports
+    "PGH004", # blanket-noqa
+    "TRY002", # raise-vanilla-class
+    "TRY003", # raise-vanilla-args
+    "RUF001", # ambiguous-unicode-character-string
+    "RUF002", # ambiguous-unicode-character-docstring
+    "RUF003", # ambiguous-unicode-character-comment
+    "RUF005", # collection-literal-concatenation
+    "RUF006", # asyncio-dangling-task
+    "RUF012", # mutable-class-default
+    "RET504", # unnecessary-assign
+    "TRY004", # type-check-without-type-error
+    "PGH003", # blanket-type-ignore (todo: fix this)
+]
+
+[lint.per-file-ignores]
+"python/serpyco_rs/_impl.pyi" = [
+    "I001",
+]
+"python/serpyco_rs/_impl.py" = [
+    "I001",
+]
+"python/serpyco_rs/_json_schema/_entities.py" = [
+    "N815", # mixed-case-variable-name
+]
+
+[lint.flake8-quotes]
+inline-quotes = "single"
+
+[lint.isort]
+combine-as-imports = true
+lines-after-imports = 2
+no-lines-before = ["local-folder"]
+
+[format]
+quote-style = "single"
```

### Comparing `serpyco_rs-1.7.1/src/lib.rs` & `serpyco_rs-1.8.0/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-mod errors;
-mod python;
-mod serializer;
-mod validator;
-
-use pyo3::prelude::*;
-use validator::types;
-
-#[pymodule]
-fn _serpyco_rs(py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_class::<serializer::Serializer>()?;
-
-    // Types
-    m.add_class::<types::CustomEncoder>()?;
-    m.add_class::<types::BaseType>()?;
-    m.add_class::<types::IntegerType>()?;
-    m.add_class::<types::StringType>()?;
-    m.add_class::<types::FloatType>()?;
-    m.add_class::<types::DecimalType>()?;
-    m.add_class::<types::BooleanType>()?;
-    m.add_class::<types::UUIDType>()?;
-    m.add_class::<types::TimeType>()?;
-    m.add_class::<types::DateTimeType>()?;
-    m.add_class::<types::DateType>()?;
-    m.add_class::<types::EntityType>()?;
-    m.add_class::<types::TypedDictType>()?;
-    m.add_class::<types::EntityField>()?;
-    m.add_class::<types::DefaultValue>()?;
-    m.add_class::<types::ArrayType>()?;
-    m.add_class::<types::EnumType>()?;
-    m.add_class::<types::OptionalType>()?;
-    m.add_class::<types::DictionaryType>()?;
-    m.add_class::<types::TupleType>()?;
-    m.add_class::<types::BytesType>()?;
-    m.add_class::<types::AnyType>()?;
-    m.add_class::<types::UnionType>()?;
-    m.add_class::<types::DiscriminatedUnionType>()?;
-    m.add_class::<types::LiteralType>()?;
-    m.add_class::<types::RecursionHolder>()?;
-
-    // Errors
-    m.add(
-        "ValidationError",
-        py.get_type_bound::<errors::ValidationError>(),
-    )?;
-    m.add(
-        "SchemaValidationError",
-        py.get_type_bound::<errors::SchemaValidationError>(),
-    )?;
-    m.add("ErrorItem", py.get_type_bound::<errors::ErrorItem>())?;
-    Ok(())
-}
+mod errors;
+mod python;
+mod serializer;
+mod validator;
+
+use pyo3::prelude::*;
+use validator::types;
+
+#[pymodule]
+fn _serpyco_rs(py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
+    m.add_class::<serializer::Serializer>()?;
+
+    // Types
+    m.add_class::<types::CustomEncoder>()?;
+    m.add_class::<types::BaseType>()?;
+    m.add_class::<types::IntegerType>()?;
+    m.add_class::<types::StringType>()?;
+    m.add_class::<types::FloatType>()?;
+    m.add_class::<types::DecimalType>()?;
+    m.add_class::<types::BooleanType>()?;
+    m.add_class::<types::UUIDType>()?;
+    m.add_class::<types::TimeType>()?;
+    m.add_class::<types::DateTimeType>()?;
+    m.add_class::<types::DateType>()?;
+    m.add_class::<types::EntityType>()?;
+    m.add_class::<types::TypedDictType>()?;
+    m.add_class::<types::EntityField>()?;
+    m.add_class::<types::DefaultValue>()?;
+    m.add_class::<types::ArrayType>()?;
+    m.add_class::<types::EnumType>()?;
+    m.add_class::<types::OptionalType>()?;
+    m.add_class::<types::DictionaryType>()?;
+    m.add_class::<types::TupleType>()?;
+    m.add_class::<types::BytesType>()?;
+    m.add_class::<types::AnyType>()?;
+    m.add_class::<types::UnionType>()?;
+    m.add_class::<types::DiscriminatedUnionType>()?;
+    m.add_class::<types::LiteralType>()?;
+    m.add_class::<types::RecursionHolder>()?;
+    m.add_class::<types::CustomType>()?;
+
+    // Errors
+    m.add(
+        "ValidationError",
+        py.get_type_bound::<errors::ValidationError>(),
+    )?;
+    m.add(
+        "SchemaValidationError",
+        py.get_type_bound::<errors::SchemaValidationError>(),
+    )?;
+    m.add("ErrorItem", py.get_type_bound::<errors::ErrorItem>())?;
+    Ok(())
+}
```

### Comparing `serpyco_rs-1.7.1/src/python/macros.rs` & `serpyco_rs-1.8.0/src/python/macros.rs`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-macro_rules! ffi {
-    ($fn:ident()) => {
-        unsafe { pyo3_ffi::$fn() }
-    };
-
-    ($fn:ident($obj1:expr)) => {
-        unsafe { pyo3_ffi::$fn($obj1) }
-    };
-
-    ($fn:ident($obj1:expr, $obj2:expr)) => {
-        unsafe { pyo3_ffi::$fn($obj1, $obj2) }
-    };
-
-    ($fn:ident($obj1:expr, $obj2:expr, $obj3:expr)) => {
-        unsafe { pyo3_ffi::$fn($obj1, $obj2, $obj3) }
-    };
-
-    ($fn:ident($obj1:expr, $obj2:expr, $obj3:expr, $obj4:expr)) => {
-        unsafe { pyo3_ffi::$fn($obj1, $obj2, $obj3, $obj4) }
-    };
-}
-
-pub(crate) use ffi;
+macro_rules! ffi {
+    ($fn:ident()) => {
+        unsafe { pyo3_ffi::$fn() }
+    };
+
+    ($fn:ident($obj1:expr)) => {
+        unsafe { pyo3_ffi::$fn($obj1) }
+    };
+
+    ($fn:ident($obj1:expr, $obj2:expr)) => {
+        unsafe { pyo3_ffi::$fn($obj1, $obj2) }
+    };
+
+    ($fn:ident($obj1:expr, $obj2:expr, $obj3:expr)) => {
+        unsafe { pyo3_ffi::$fn($obj1, $obj2, $obj3) }
+    };
+
+    ($fn:ident($obj1:expr, $obj2:expr, $obj3:expr, $obj4:expr)) => {
+        unsafe { pyo3_ffi::$fn($obj1, $obj2, $obj3, $obj4) }
+    };
+}
+
+pub(crate) use ffi;
```

### Comparing `serpyco_rs-1.7.1/src/python/py.rs` & `serpyco_rs-1.8.0/src/python/py.rs`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-use std::os::raw::c_int;
-
-use pyo3::prelude::*;
-use pyo3::types::{PyDict, PyList, PyTuple};
-use pyo3::{ffi, PyErr, PyResult, Python};
-use pyo3_ffi::Py_ssize_t;
-
-use super::macros::ffi;
-
-#[inline]
-pub(crate) fn create_py_list(py: Python, size: usize) -> Bound<PyList> {
-    let size: Py_ssize_t = size.try_into().expect("size is too large");
-    unsafe { Bound::from_owned_ptr(py, ffi::PyList_New(size)).downcast_into_unchecked() }
-}
-
-#[inline]
-pub(crate) fn py_list_get_item<'a>(list: &'a Bound<'a, PyList>, index: usize) -> Bound<'a, PyAny> {
-    #[cfg(any(Py_LIMITED_API, PyPy))]
-    let item = list.get_item(index).expect("list.get failed");
-    #[cfg(not(any(Py_LIMITED_API, PyPy)))]
-    let item = unsafe { list.get_item_unchecked(index) };
-    item
-}
-
-#[inline]
-pub(crate) fn py_list_set_item(list: &Bound<PyList>, index: usize, value: Bound<PyAny>) {
-    let index: Py_ssize_t = index.try_into().expect("size is too large");
-    #[cfg(not(Py_LIMITED_API))]
-    ffi!(PyList_SET_ITEM(list.as_ptr(), index, value.into_ptr()));
-    #[cfg(Py_LIMITED_API)]
-    ffi!(PyList_SetItem(list.as_ptr(), index, value.into_ptr()));
-}
-
-#[inline]
-pub(crate) fn create_py_dict_known_size(py: Python, size: usize) -> Bound<PyDict> {
-    let size: Py_ssize_t = size.try_into().expect("size is too large");
-    unsafe { Bound::from_owned_ptr(py, ffi::_PyDict_NewPresized(size)).downcast_into_unchecked() }
-}
-
-#[inline]
-pub(crate) fn py_dict_set_item(
-    list: &Bound<PyDict>,
-    key: *mut ffi::PyObject,
-    value: Bound<PyAny>,
-) -> PyResult<()> {
-    // todo: Check performance
-    let result = ffi!(PyDict_SetItem(list.as_ptr(), key, value.as_ptr()));
-    error_on_minusone(result)
-}
-
-#[inline]
-pub(crate) fn create_py_tuple(py: Python, size: usize) -> Bound<PyTuple> {
-    let size: Py_ssize_t = size.try_into().expect("size is too large");
-    unsafe { Bound::from_owned_ptr(py, ffi::PyTuple_New(size)).downcast_into_unchecked() }
-}
-
-#[inline]
-pub(crate) fn py_tuple_set_item(list: &Bound<PyTuple>, index: usize, value: Bound<PyAny>) {
-    let index: Py_ssize_t = index.try_into().expect("size is too large");
-    ffi!(PyTuple_SetItem(list.as_ptr(), index, value.into_ptr()));
-}
-
-#[inline]
-pub(crate) fn error_on_minusone(result: c_int) -> PyResult<()> {
-    if result != -1 {
-        Ok(())
-    } else {
-        Err(Python::with_gil(PyErr::fetch))
-    }
-}
+use std::os::raw::c_int;
+
+use pyo3::prelude::*;
+use pyo3::types::{PyDict, PyList, PyTuple};
+use pyo3::{ffi, PyErr, PyResult, Python};
+use pyo3_ffi::Py_ssize_t;
+
+use super::macros::ffi;
+
+#[inline]
+pub(crate) fn create_py_list(py: Python, size: usize) -> Bound<PyList> {
+    let size: Py_ssize_t = size.try_into().expect("size is too large");
+    unsafe { Bound::from_owned_ptr(py, ffi::PyList_New(size)).downcast_into_unchecked() }
+}
+
+#[inline]
+pub(crate) fn py_list_get_item<'a>(list: &'a Bound<'a, PyList>, index: usize) -> Bound<'a, PyAny> {
+    #[cfg(any(Py_LIMITED_API, PyPy))]
+    let item = list.get_item(index).expect("list.get failed");
+    #[cfg(not(any(Py_LIMITED_API, PyPy)))]
+    let item = unsafe { list.get_item_unchecked(index) };
+    item
+}
+
+#[inline]
+pub(crate) fn py_list_set_item(list: &Bound<PyList>, index: usize, value: Bound<PyAny>) {
+    let index: Py_ssize_t = index.try_into().expect("size is too large");
+    #[cfg(not(Py_LIMITED_API))]
+    ffi!(PyList_SET_ITEM(list.as_ptr(), index, value.into_ptr()));
+    #[cfg(Py_LIMITED_API)]
+    ffi!(PyList_SetItem(list.as_ptr(), index, value.into_ptr()));
+}
+
+#[inline]
+pub(crate) fn create_py_dict_known_size(py: Python, size: usize) -> Bound<PyDict> {
+    let size: Py_ssize_t = size.try_into().expect("size is too large");
+    unsafe { Bound::from_owned_ptr(py, ffi::_PyDict_NewPresized(size)).downcast_into_unchecked() }
+}
+
+#[inline]
+pub(crate) fn py_dict_set_item(
+    list: &Bound<PyDict>,
+    key: *mut ffi::PyObject,
+    value: Bound<PyAny>,
+) -> PyResult<()> {
+    // todo: Check performance
+    let result = ffi!(PyDict_SetItem(list.as_ptr(), key, value.as_ptr()));
+    error_on_minusone(result)
+}
+
+#[inline]
+pub(crate) fn create_py_tuple(py: Python, size: usize) -> Bound<PyTuple> {
+    let size: Py_ssize_t = size.try_into().expect("size is too large");
+    unsafe { Bound::from_owned_ptr(py, ffi::PyTuple_New(size)).downcast_into_unchecked() }
+}
+
+#[inline]
+pub(crate) fn py_tuple_set_item(list: &Bound<PyTuple>, index: usize, value: Bound<PyAny>) {
+    let index: Py_ssize_t = index.try_into().expect("size is too large");
+    ffi!(PyTuple_SetItem(list.as_ptr(), index, value.into_ptr()));
+}
+
+#[inline]
+pub(crate) fn error_on_minusone(result: c_int) -> PyResult<()> {
+    if result != -1 {
+        Ok(())
+    } else {
+        Err(Python::with_gil(PyErr::fetch))
+    }
+}
```

### Comparing `serpyco_rs-1.7.1/src/python/types.rs` & `serpyco_rs-1.8.0/src/python/types.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-use pyo3::prelude::PyAnyMethods;
-use pyo3::Bound;
-use pyo3::{PyAny, PyResult};
-
-use crate::validator::types::{
-    AnyType, ArrayType, BaseType, BooleanType, BytesType, DateTimeType, DateType, DecimalType,
-    DictionaryType, DiscriminatedUnionType, EntityType, EnumType, FloatType, IntegerType,
-    LiteralType, OptionalType, RecursionHolder, StringType, TimeType, TupleType, TypedDictType,
-    UUIDType, UnionType,
-};
-
-#[derive(Clone, Debug)]
-pub enum Type<'a, Base = Bound<'a, BaseType>> {
-    Integer(Bound<'a, IntegerType>, Base),
-    Float(Bound<'a, FloatType>, Base),
-    Decimal(Bound<'a, DecimalType>, Base),
-    String(Bound<'a, StringType>, Base),
-    Boolean(Bound<'a, BooleanType>, Base),
-    Uuid(Bound<'a, UUIDType>, Base),
-    Bytes(Bound<'a, BytesType>, Base),
-    Time(Bound<'a, TimeType>, Base),
-    DateTime(Bound<'a, DateTimeType>, Base),
-    Date(Bound<'a, DateType>, Base),
-    Entity(Bound<'a, EntityType>, Base, usize),
-    TypedDict(Bound<'a, TypedDictType>, Base, usize),
-    Array(Bound<'a, ArrayType>, Base),
-    Enum(Bound<'a, EnumType>, Base),
-    Optional(Bound<'a, OptionalType>, Base),
-    Dictionary(Bound<'a, DictionaryType>, Base),
-    Tuple(Bound<'a, TupleType>, Base),
-    DiscriminatedUnion(Bound<'a, DiscriminatedUnionType>, Base),
-    Union(Bound<'a, UnionType>, Base),
-    Literal(Bound<'a, LiteralType>, Base),
-    Any(Bound<'a, AnyType>, Base),
-    RecursionHolder(Bound<'a, RecursionHolder>, Base),
-}
-
-pub fn get_object_type<'a>(type_info: &Bound<'a, PyAny>) -> PyResult<Type<'a>> {
-    let base_type = type_info.extract::<Bound<'_, BaseType>>()?;
-    check_type!(type_info, base_type, Integer, IntegerType);
-    check_type!(type_info, base_type, String, StringType);
-    check_type!(type_info, base_type, Float, FloatType);
-    check_type!(type_info, base_type, Decimal, DecimalType);
-    check_type!(type_info, base_type, Boolean, BooleanType);
-    check_type!(type_info, base_type, Uuid, UUIDType);
-    check_type!(type_info, base_type, Time, TimeType);
-    check_type!(type_info, base_type, DateTime, DateTimeType);
-    check_type!(type_info, base_type, Date, DateType);
-    check_type!(type_info, base_type, Enum, EnumType);
-    check_type!(type_info, base_type, Optional, OptionalType);
-    check_type!(type_info, base_type, Array, ArrayType);
-    check_type!(type_info, base_type, Dictionary, DictionaryType);
-    check_type!(type_info, base_type, Tuple, TupleType);
-    check_type!(type_info, base_type, Any, AnyType);
-    check_type!(type_info, base_type, Union, UnionType);
-    check_type!(
-        type_info,
-        base_type,
-        DiscriminatedUnion,
-        DiscriminatedUnionType
-    );
-    check_type!(type_info, base_type, Literal, LiteralType);
-    check_type!(type_info, base_type, Bytes, BytesType);
-    check_type!(type_info, base_type, RecursionHolder, RecursionHolder);
-
-    if let Ok(t) = type_info.extract::<Bound<'_, EntityType>>() {
-        let python_object_id = type_info.as_ptr() as *const _ as usize;
-        Ok(Type::Entity(t, base_type, python_object_id))
-    } else if let Ok(t) = type_info.extract::<Bound<'_, TypedDictType>>() {
-        let python_object_id = type_info.as_ptr() as *const _ as usize;
-        Ok(Type::TypedDict(t, base_type, python_object_id))
-    } else {
-        unreachable!("Unknown type: {:?}", type_info)
-    }
-}
-
-macro_rules! check_type {
-    ($type_info:ident, $base_type:ident, $enum:ident, $type:ident) => {
-        if let Ok(t) = $type_info.extract::<Bound<'_, $type>>() {
-            return Ok(Type::$enum(t, $base_type));
-        }
-    };
-}
-
-pub(crate) use check_type;
+use pyo3::prelude::PyAnyMethods;
+use pyo3::Bound;
+use pyo3::{PyAny, PyResult};
+
+use crate::validator::types::{
+    AnyType, ArrayType, BaseType, BooleanType, BytesType, CustomType, DateTimeType, DateType,
+    DecimalType, DictionaryType, DiscriminatedUnionType, EntityType, EnumType, FloatType,
+    IntegerType, LiteralType, OptionalType, RecursionHolder, StringType, TimeType, TupleType,
+    TypedDictType, UUIDType, UnionType,
+};
+
+#[derive(Clone, Debug)]
+pub enum Type<'a, Base = Bound<'a, BaseType>> {
+    Integer(Bound<'a, IntegerType>, Base),
+    Float(Bound<'a, FloatType>, Base),
+    Decimal(Bound<'a, DecimalType>, Base),
+    String(Bound<'a, StringType>, Base),
+    Boolean(Bound<'a, BooleanType>, Base),
+    Uuid(Bound<'a, UUIDType>, Base),
+    Bytes(Bound<'a, BytesType>, Base),
+    Time(Bound<'a, TimeType>, Base),
+    DateTime(Bound<'a, DateTimeType>, Base),
+    Date(Bound<'a, DateType>, Base),
+    Entity(Bound<'a, EntityType>, Base, usize),
+    TypedDict(Bound<'a, TypedDictType>, Base, usize),
+    Array(Bound<'a, ArrayType>, Base),
+    Enum(Bound<'a, EnumType>, Base),
+    Optional(Bound<'a, OptionalType>, Base),
+    Dictionary(Bound<'a, DictionaryType>, Base),
+    Tuple(Bound<'a, TupleType>, Base),
+    DiscriminatedUnion(Bound<'a, DiscriminatedUnionType>, Base),
+    Union(Bound<'a, UnionType>, Base),
+    Literal(Bound<'a, LiteralType>, Base),
+    Any(Bound<'a, AnyType>, Base),
+    RecursionHolder(Bound<'a, RecursionHolder>, Base),
+    Custom(Bound<'a, CustomType>, Base),
+}
+
+pub fn get_object_type<'a>(type_info: &Bound<'a, PyAny>) -> PyResult<Type<'a>> {
+    let base_type = type_info.extract::<Bound<'_, BaseType>>()?;
+    check_type!(type_info, base_type, Integer, IntegerType);
+    check_type!(type_info, base_type, String, StringType);
+    check_type!(type_info, base_type, Float, FloatType);
+    check_type!(type_info, base_type, Decimal, DecimalType);
+    check_type!(type_info, base_type, Boolean, BooleanType);
+    check_type!(type_info, base_type, Uuid, UUIDType);
+    check_type!(type_info, base_type, Time, TimeType);
+    check_type!(type_info, base_type, DateTime, DateTimeType);
+    check_type!(type_info, base_type, Date, DateType);
+    check_type!(type_info, base_type, Enum, EnumType);
+    check_type!(type_info, base_type, Optional, OptionalType);
+    check_type!(type_info, base_type, Array, ArrayType);
+    check_type!(type_info, base_type, Dictionary, DictionaryType);
+    check_type!(type_info, base_type, Tuple, TupleType);
+    check_type!(type_info, base_type, Any, AnyType);
+    check_type!(type_info, base_type, Union, UnionType);
+    check_type!(
+        type_info,
+        base_type,
+        DiscriminatedUnion,
+        DiscriminatedUnionType
+    );
+    check_type!(type_info, base_type, Literal, LiteralType);
+    check_type!(type_info, base_type, Bytes, BytesType);
+    check_type!(type_info, base_type, RecursionHolder, RecursionHolder);
+    check_type!(type_info, base_type, Custom, CustomType);
+
+    if let Ok(t) = type_info.extract::<Bound<'_, EntityType>>() {
+        let python_object_id = type_info.as_ptr() as *const _ as usize;
+        Ok(Type::Entity(t, base_type, python_object_id))
+    } else if let Ok(t) = type_info.extract::<Bound<'_, TypedDictType>>() {
+        let python_object_id = type_info.as_ptr() as *const _ as usize;
+        Ok(Type::TypedDict(t, base_type, python_object_id))
+    } else {
+        unreachable!("Unknown type: {:?}", type_info)
+    }
+}
+
+macro_rules! check_type {
+    ($type_info:ident, $base_type:ident, $enum:ident, $type:ident) => {
+        if let Ok(t) = $type_info.extract::<Bound<'_, $type>>() {
+            return Ok(Type::$enum(t, $base_type));
+        }
+    };
+}
+
+pub(crate) use check_type;
```

### Comparing `serpyco_rs-1.7.1/src/serializer/encoders.rs` & `serpyco_rs-1.8.0/src/serializer/encoders.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,1067 +1,1093 @@
-use std::collections::HashMap;
-use std::fmt::Debug;
-use std::sync::Arc;
-
-use atomic_refcell::AtomicRefCell;
-use dyn_clone::{clone_trait_object, DynClone};
-use pyo3::exceptions::PyRuntimeError;
-use pyo3::prelude::*;
-use pyo3::types::{
-    PyBool, PyBytes, PyDate, PyDateTime, PyDict, PyFloat, PyList, PyLong, PySequence, PyString,
-    PyTime,
-};
-use pyo3::{intern, Bound, Py, PyAny, PyResult};
-use uuid::Uuid;
-
-use crate::errors::{ToPyErr, ValidationError};
-use crate::python::{
-    create_py_dict_known_size, create_py_list, create_py_tuple, dump_date, dump_datetime,
-    dump_time, parse_date, parse_datetime, parse_time, py_dict_set_item, py_list_get_item,
-    py_list_set_item, py_tuple_set_item,
-};
-use crate::validator::types::{DecimalType, EnumItem, FloatType, IntegerType, StringType};
-use crate::validator::validators::{
-    check_bounds, check_length, check_sequence_size, invalid_enum_item, invalid_type,
-    invalid_type_dump, missing_required_property, no_encoder_for_discriminator, str_as_bool,
-};
-use crate::validator::{Context, InstancePath};
-
-pub type TEncoder = dyn Encoder + Send + Sync;
-
-pub trait Encoder: DynClone + Debug {
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>>;
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>>;
-
-    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
-        None
-    }
-    fn is_sequence(&self) -> bool {
-        false
-    }
-}
-
-pub struct EncoderField<'a> {
-    pub(crate) name: &'a Py<PyString>,
-    pub(crate) is_sequence: bool,
-}
-
-pub enum QueryFields<'a> {
-    Object(Vec<EncoderField<'a>>),
-    Dict(bool), // is_sequence
-}
-
-pub trait ContainerEncoder: Encoder {
-    fn get_fields(&self) -> QueryFields;
-}
-
-clone_trait_object!(Encoder);
-
-#[derive(Debug, Clone)]
-pub struct NoopEncoder;
-
-impl Encoder for NoopEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        _instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct IntEncoder {
-    pub(crate) type_info: IntegerType,
-}
-
-impl Encoder for IntEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyLong>() {
-            check_bounds!(val.extract()?, self.type_info, instance_path)?;
-            return Ok(value.clone());
-        }
-        if ctx.try_cast_from_string {
-            if let Ok(val) = value.downcast::<PyString>() {
-                if let Ok(val) = val.to_str()?.parse::<i64>() {
-                    check_bounds!(val, self.type_info, instance_path)?;
-                    return Ok(val.to_object(value.py()).into_bound(value.py()));
-                }
-            }
-        }
-        invalid_type!("integer", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct FloatEncoder {
-    pub(crate) type_info: FloatType,
-}
-
-impl Encoder for FloatEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyLong>() {
-            check_bounds!(val.extract()?, self.type_info, instance_path)?;
-            return Ok(value.clone());
-        }
-        if let Ok(val) = value.downcast::<PyFloat>() {
-            check_bounds!(val.extract()?, self.type_info, instance_path)?;
-            return Ok(value.clone());
-        }
-        if ctx.try_cast_from_string {
-            if let Ok(val) = value.downcast::<PyString>() {
-                if let Ok(val) = val.to_str()?.parse::<f64>() {
-                    check_bounds!(val, self.type_info, instance_path)?;
-                    return Ok(val.to_object(value.py()).into_bound(value.py()));
-                }
-            }
-        }
-        invalid_type!("number", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct DecimalEncoder {
-    pub(crate) type_info: DecimalType,
-    pub(crate) decimal_cls: Py<PyAny>,
-}
-
-impl Encoder for DecimalEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.str()?.into_any())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        let valid = if let Ok(val) = value.downcast::<PyFloat>() {
-            check_bounds!(val.value(), self.type_info, instance_path)?;
-            true
-        } else if let Ok(val) = value.downcast::<PyLong>() {
-            check_bounds!(val.extract()?, self.type_info, instance_path)?;
-            true
-        } else if let Ok(val) = value.downcast::<PyString>() {
-            match val.to_str()?.parse::<f64>() {
-                Ok(val_f64) => {
-                    check_bounds!(val_f64, self.type_info, instance_path)?;
-                    true
-                }
-                Err(_) => false,
-            }
-        } else {
-            false
-        };
-        if valid {
-            let str_value = value.str().expect("Failed to convert value to string.");
-            self.decimal_cls.bind(value.py()).call1((str_value,))
-        } else {
-            invalid_type!("decimal", value, instance_path)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct StringEncoder {
-    pub(crate) type_info: StringType,
-}
-
-impl Encoder for StringEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyString>() {
-            check_length(
-                val,
-                self.type_info.min_length,
-                self.type_info.max_length,
-                instance_path,
-            )?;
-            Ok(value.clone())
-        } else {
-            invalid_type!("string", value, instance_path)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct BooleanEncoder {}
-
-impl Encoder for BooleanEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(_val) = value.downcast::<PyBool>() {
-            return Ok(value.clone());
-        }
-        if ctx.try_cast_from_string {
-            if let Ok(val) = value.downcast::<PyString>() {
-                if let Some(val) = str_as_bool(val.to_str()?) {
-                    return Ok(val.to_object(value.py()).into_bound(value.py()));
-                }
-            }
-        }
-
-        invalid_type!("boolean", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct BytesEncoder {}
-
-impl Encoder for BytesEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(_val) = value.downcast::<PyBytes>() {
-            Ok(value.clone())
-        } else {
-            invalid_type!("bytes", value, instance_path)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct DictionaryEncoder {
-    pub(crate) key_encoder: Box<TEncoder>,
-    pub(crate) value_encoder: Box<TEncoder>,
-    pub(crate) omit_none: bool,
-}
-
-impl Encoder for DictionaryEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(dict) = value.downcast::<PyDict>() {
-            let result_dict = create_py_dict_known_size(dict.py(), dict.len());
-            for (k, v) in dict.iter() {
-                let key = self.key_encoder.dump(&k)?;
-                let value = self.value_encoder.dump(&v)?;
-                if !self.omit_none || !value.is_none() {
-                    py_dict_set_item(&result_dict, key.as_ptr(), value)?;
-                }
-            }
-            Ok(result_dict.into_any())
-        } else {
-            invalid_type_dump!("dict", value)
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyDict>() {
-            let result_dict = create_py_dict_known_size(val.py(), val.len());
-            for (k, v) in val.iter() {
-                let instance_path = instance_path.push(&k);
-                let key = self.key_encoder.load(&k, &instance_path, ctx)?;
-                let value = self.value_encoder.load(&v, &instance_path, ctx)?;
-                py_dict_set_item(&result_dict, key.as_ptr(), value)?;
-            }
-            Ok(result_dict.into_any())
-        } else {
-            invalid_type_dump!("dict", value)
-        }
-    }
-
-    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
-        Some(self)
-    }
-}
-
-impl ContainerEncoder for DictionaryEncoder {
-    fn get_fields(&self) -> QueryFields {
-        QueryFields::Dict(self.value_encoder.is_sequence())
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct ArrayEncoder {
-    pub(crate) encoder: Box<TEncoder>,
-}
-
-impl Encoder for ArrayEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(list) = value.downcast::<PyList>() {
-            let size = list.len();
-            let result = create_py_list(value.py(), size);
-
-            for index in 0..size {
-                let item = py_list_get_item(list, index);
-                let val = self.encoder.dump(&item)?;
-                py_list_set_item(&result, index, val);
-            }
-
-            Ok(result.into_any())
-        } else {
-            invalid_type_dump!("list", value)
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyList>() {
-            let size = val.len();
-            let result = create_py_list(value.py(), size);
-
-            for index in 0..size {
-                let item = py_list_get_item(val, index);
-                let instance_path = instance_path.push(index);
-                let val = self.encoder.load(&item, &instance_path, ctx)?;
-                py_list_set_item(&result, index, val);
-            }
-            Ok(result.into_any())
-        } else {
-            invalid_type!("list", value, instance_path)
-        }
-    }
-
-    fn is_sequence(&self) -> bool {
-        true
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct EntityEncoder {
-    pub(crate) cls: Py<PyAny>,
-    pub(crate) omit_none: bool,
-    pub(crate) is_frozen: bool,
-    pub(crate) fields: Vec<Field>,
-    pub(crate) create_object: Py<PyAny>,
-    pub(crate) object_set_attr: Py<PyAny>,
-}
-
-#[derive(Debug, Clone)]
-pub struct Field {
-    pub(crate) name: Py<PyString>,
-    pub(crate) dict_key: Py<PyString>,
-    pub(crate) dict_key_rs: String,
-    pub(crate) encoder: Box<TEncoder>,
-    pub(crate) required: bool,
-    pub(crate) default: Option<Py<PyAny>>,
-    pub(crate) default_factory: Option<Py<PyAny>>,
-}
-
-impl Encoder for EntityEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let dict = create_py_dict_known_size(value.py(), self.fields.len());
-
-        for field in &self.fields {
-            let field_val = value.getattr(&field.name)?;
-            let dump_result = field.encoder.dump(&field_val)?;
-            if field.required || !self.omit_none || !dump_result.is_none() {
-                py_dict_set_item(&dict, field.dict_key.as_ptr(), dump_result)?;
-            }
-        }
-
-        Ok(dict.into_any())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        let py_frozen_object_set_attr = self.object_set_attr.bind(value.py());
-        if let Ok(val) = value.downcast::<PyDict>() {
-            let obj = self
-                .create_object
-                .bind(value.py())
-                .call1((self.cls.bind(value.py()),))?;
-            for field in &self.fields {
-                let val = match val.get_item(&field.dict_key)? {
-                    Some(val) => {
-                        let instance_path =
-                            instance_path.push(field.dict_key.bind(value.py()).as_any());
-                        field.encoder.load(&val, &instance_path, ctx)?
-                    }
-                    None => match (&field.default, &field.default_factory) {
-                        (Some(val), _) => val.bind(value.py()).clone(),
-                        (_, Some(val)) => val.bind(value.py()).call0()?,
-                        (None, _) => {
-                            return Err(missing_required_property(
-                                &field.dict_key_rs,
-                                instance_path,
-                            ));
-                        }
-                    },
-                };
-
-                if self.is_frozen {
-                    py_frozen_object_set_attr.call1((&obj, &field.name, val))?;
-                } else {
-                    obj.setattr(&field.name, val)?;
-                };
-            }
-
-            Ok(obj)
-        } else {
-            invalid_type!("object", value, instance_path)
-        }
-    }
-
-    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
-        Some(self)
-    }
-}
-
-impl ContainerEncoder for EntityEncoder {
-    fn get_fields(&self) -> QueryFields {
-        QueryFields::Object(
-            self.fields
-                .iter()
-                .map(|f| EncoderField {
-                    name: &f.dict_key,
-                    is_sequence: f.encoder.is_sequence(),
-                })
-                .collect(),
-        )
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct TypedDictEncoder {
-    pub(crate) omit_none: bool,
-    pub(crate) fields: Vec<Field>,
-}
-
-impl Encoder for TypedDictEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let value = match value.downcast::<PyDict>() {
-            Ok(val) => val,
-            _ => invalid_type_dump!("dict", value),
-        };
-        let dict = create_py_dict_known_size(value.py(), self.fields.len());
-        for field in &self.fields {
-            let field_val = match value.get_item(&field.name) {
-                Ok(Some(val)) => val,
-                _ => {
-                    if field.required {
-                        return Err(ValidationError::new_err(format!(
-                            "data dictionary is missing required parameter {}",
-                            &field.name
-                        )));
-                    } else {
-                        continue;
-                    }
-                }
-            };
-            let dump_result = field.encoder.dump(&field_val)?;
-            if field.required || !self.omit_none || !dump_result.is_none() {
-                py_dict_set_item(&dict, field.dict_key.as_ptr(), dump_result)?;
-            }
-        }
-        Ok(dict.into_any())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        let value = match value.downcast::<PyDict>() {
-            Ok(val) => val,
-            Err(_) => {
-                invalid_type_dump!("dict", value);
-            }
-        };
-        let dict = create_py_dict_known_size(value.py(), self.fields.len());
-        for field in &self.fields {
-            let field_val = match value.get_item(&field.dict_key) {
-                Ok(Some(val)) => val,
-                _ => {
-                    if field.required {
-                        return Err(missing_required_property(&field.dict_key_rs, instance_path));
-                    } else {
-                        continue;
-                    }
-                }
-            };
-            let instance_path = instance_path.push(field.dict_key_rs.as_str());
-            let dump_result = field.encoder.load(&field_val, &instance_path, ctx)?;
-            py_dict_set_item(&dict, field.name.as_ptr(), dump_result)?;
-        }
-        Ok(dict.into_any())
-    }
-    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
-        Some(self)
-    }
-}
-
-impl ContainerEncoder for TypedDictEncoder {
-    fn get_fields(&self) -> QueryFields {
-        QueryFields::Object(
-            self.fields
-                .iter()
-                .map(|f| EncoderField {
-                    name: &f.dict_key,
-                    is_sequence: f.encoder.is_sequence(),
-                })
-                .collect(),
-        )
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct UUIDEncoder {
-    pub(crate) uuid_cls: Py<PyAny>,
-}
-
-impl Encoder for UUIDEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.str()?.into_any())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyString>() {
-            if Uuid::parse_str(val.to_str()?).is_ok() {
-                if let Ok(result) = self.uuid_cls.bind(value.py()).call1((val,)) {
-                    return Ok(result);
-                }
-            }
-        }
-        invalid_type!("uuid", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct EnumEncoder {
-    pub(crate) enum_items: Vec<(EnumItem, Py<PyAny>)>,
-}
-
-impl Encoder for EnumEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let value_str = intern!(value.py(), "value");
-        Ok(value.getattr(value_str)?.into_any())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        let val = if let Ok(val) = value.downcast::<PyString>() {
-            EnumItem::String(val.to_str()?.to_owned())
-        } else if let Ok(val) = value.downcast::<PyLong>() {
-            EnumItem::Int(val.extract()?)
-        } else {
-            invalid_enum_item!((&self.enum_items).into(), value, instance_path);
-        };
-
-        let index = self.enum_items.binary_search_by(|(e, _)| e.cmp(&val));
-
-        match index {
-            Ok(index) => {
-                let (_, py_item) = &self.enum_items[index];
-                return Ok(py_item.bind(value.py()).clone());
-            }
-            Err(_) if ctx.try_cast_from_string => {
-                if let Ok(value) = value.downcast::<PyString>() {
-                    if let Ok(val) = value.to_str()?.parse::<i64>() {
-                        if let Ok(index) = self
-                            .enum_items
-                            .binary_search_by(|(e, _)| e.cmp(&EnumItem::Int(val)))
-                        {
-                            let (_, py_item) = &self.enum_items[index];
-                            return Ok(py_item.bind(value.py()).clone());
-                        }
-                    }
-                }
-            }
-            _ => {}
-        }
-
-        invalid_enum_item!((&self.enum_items).into(), value, instance_path);
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct LiteralEncoder {
-    pub(crate) enum_items: Vec<(EnumItem, Py<PyAny>)>,
-}
-
-impl Encoder for LiteralEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        Ok(value.clone())
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        let val = if let Ok(val) = value.downcast::<PyString>() {
-            EnumItem::String(val.to_str()?.to_owned())
-        } else if let Ok(val) = value.downcast::<PyLong>() {
-            EnumItem::Int(val.extract()?)
-        } else {
-            invalid_enum_item!((&self.enum_items).into(), value, instance_path);
-        };
-
-        let index = self.enum_items.binary_search_by(|(e, _)| e.cmp(&val));
-
-        match index {
-            Ok(index) => {
-                let (_, py_item) = &self.enum_items[index];
-                return Ok(py_item.bind(value.py()).clone());
-            }
-            Err(_) if ctx.try_cast_from_string => {
-                if let Ok(value) = value.downcast::<PyString>() {
-                    if let Ok(val) = value.to_str()?.parse::<i64>() {
-                        if let Ok(index) = self
-                            .enum_items
-                            .binary_search_by(|(e, _)| e.cmp(&EnumItem::Int(val)))
-                        {
-                            let (_, py_item) = &self.enum_items[index];
-                            return Ok(py_item.bind(value.py()).clone());
-                        }
-                    }
-                }
-            }
-            _ => {}
-        }
-
-        invalid_enum_item!((&self.enum_items).into(), value, instance_path);
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct OptionalEncoder {
-    pub(crate) encoder: Box<TEncoder>,
-}
-
-impl Encoder for OptionalEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        if value.is_none() {
-            Ok(value.clone())
-        } else {
-            self.encoder.dump(value)
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if value.is_none() {
-            Ok(value.clone())
-        } else {
-            self.encoder.load(value, instance_path, ctx)
-        }
-    }
-
-    fn is_sequence(&self) -> bool {
-        self.encoder.is_sequence()
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct TupleEncoder {
-    pub(crate) encoders: Vec<Box<TEncoder>>,
-}
-
-impl Encoder for TupleEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(seq) = value.downcast::<PySequence>() {
-            let seq_len = seq.len()?;
-            check_sequence_size(seq, seq_len, self.encoders.len(), None)?;
-            let result = create_py_list(value.py(), seq_len);
-            for index in 0..seq_len {
-                let item = seq.get_item(index)?;
-                let val = self.encoders[index].dump(&item)?;
-                py_list_set_item(&result, index, val);
-            }
-
-            Ok(result.into_any())
-        } else {
-            invalid_type_dump!("sequence", value)
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        // Check sequence is not str
-        if let Ok(seq) = value.downcast::<PySequence>() {
-            if value.is_instance_of::<PyString>() {
-                invalid_type!("sequence", value, instance_path);
-            }
-            let seq_len = seq.len()?;
-            check_sequence_size(seq, seq_len, self.encoders.len(), Some(instance_path))?;
-            let result = create_py_tuple(value.py(), seq_len);
-            for index in 0..seq_len {
-                let item = seq.get_item(index)?;
-                let instance_path = instance_path.push(index);
-                let val = self.encoders[index].load(&item, &instance_path, ctx)?;
-                py_tuple_set_item(&result, index, val);
-            }
-            Ok(result.into_any())
-        } else {
-            invalid_type!("sequence", value, instance_path)
-        }
-    }
-
-    fn is_sequence(&self) -> bool {
-        true
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct UnionEncoder {
-    pub(crate) encoders: Vec<Box<TEncoder>>,
-    pub(crate) union_repr: String,
-}
-
-impl Encoder for UnionEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        for encoder in &self.encoders {
-            let result = encoder.dump(value);
-            if result.is_ok() {
-                return result;
-            }
-        }
-        invalid_type_dump!(&self.union_repr, value)
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        for encoder in &self.encoders {
-            let result = encoder.load(value, instance_path, ctx);
-            if result.is_ok() {
-                return result;
-            }
-        }
-        invalid_type!(&self.union_repr, value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct DiscriminatedUnionEncoder {
-    pub(crate) encoders: HashMap<String, Box<TEncoder>>,
-    pub(crate) dump_discriminator: Py<PyString>,
-    pub(crate) load_discriminator: Py<PyString>,
-    pub(crate) load_discriminator_rs: String,
-    pub(crate) keys: Vec<String>,
-}
-
-impl Encoder for DiscriminatedUnionEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let key = match value.getattr(&self.dump_discriminator) {
-            Ok(val) => val.str()?,
-            Err(_) => {
-                return Err(missing_required_property(
-                    self.dump_discriminator.bind(value.py()).str()?.to_str()?,
-                    &InstancePath::new(),
-                ));
-            }
-        };
-
-        let str_key = key.to_str()?;
-
-        let encoder = self.encoders.get(str_key).ok_or_else(|| {
-            let instance_path = InstancePath::new();
-            no_encoder_for_discriminator(str_key, &self.keys, &instance_path)
-        })?;
-        encoder.dump(value)
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyDict>() {
-            let key_any = match val.get_item(&self.load_discriminator) {
-                Ok(Some(k)) => k,
-                _ => {
-                    return Err(missing_required_property(
-                        &self.load_discriminator_rs,
-                        instance_path,
-                    ));
-                }
-            };
-
-            let key_py_string = key_any
-                .downcast::<PyString>()
-                .expect("key must be a string");
-            let key_str = key_py_string.to_str()?;
-            let encoder = self.encoders.get(key_str).ok_or_else(|| {
-                let instance_path = instance_path.push(self.load_discriminator_rs.as_str());
-                no_encoder_for_discriminator(key_str, &self.keys, &instance_path)
-            })?;
-            encoder.load(value, instance_path, ctx)
-        } else {
-            invalid_type!("dict", value, instance_path)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct TimeEncoder {}
-
-impl Encoder for TimeEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let py_time = value.downcast::<PyTime>()?;
-        let result = dump_time(py_time)?;
-        Ok(result.into_py(value.py()).into_bound(value.py()))
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyString>() {
-            if let Ok(result) = parse_time(value.py(), val.to_str()?) {
-                return Ok(result.into_any());
-            }
-        }
-        invalid_type!("time", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct DateTimeEncoder {
-    pub(crate) naive_datetime_to_utc: bool,
-}
-
-impl Encoder for DateTimeEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let py_datetime = value.downcast::<PyDateTime>()?;
-        let result = dump_datetime(py_datetime, self.naive_datetime_to_utc)?;
-        Ok(result.into_py(value.py()).into_bound(value.py()))
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyString>() {
-            if let Ok(result) = parse_datetime(value.py(), val.to_str()?) {
-                return Ok(result.into_any());
-            }
-        }
-        invalid_type!("datetime", value, instance_path)
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct DateEncoder {}
-
-impl Encoder for DateEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        let py_date = value.downcast::<PyDate>()?;
-        let result = dump_date(py_date)?;
-        Ok(result.into_py(value.py()).into_bound(value.py()))
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        _ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        if let Ok(val) = value.downcast::<PyString>() {
-            if let Ok(result) = parse_date(value.py(), val.to_str()?) {
-                return Ok(result.into_any());
-            }
-        }
-        invalid_type!("date", value, instance_path)
-    }
-}
-
-#[derive(Debug)]
-pub enum Encoders {
-    Entity(EntityEncoder),
-    TypedDict(TypedDictEncoder),
-}
-
-#[derive(Debug, Clone)]
-pub struct LazyEncoder {
-    pub(crate) inner: Arc<AtomicRefCell<Option<Encoders>>>,
-}
-
-impl Encoder for LazyEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        match self.inner.borrow().as_ref() {
-            Some(encoder) => match encoder {
-                Encoders::Entity(encoder) => encoder.dump(value),
-                Encoders::TypedDict(encoder) => encoder.dump(value),
-            },
-            None => Err(PyRuntimeError::new_err(
-                "[RUST] Invalid recursive encoder".to_string(),
-            )),
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        match self.inner.borrow().as_ref() {
-            Some(encoder) => match encoder {
-                Encoders::Entity(encoder) => encoder.load(value, instance_path, ctx),
-                Encoders::TypedDict(encoder) => encoder.load(value, instance_path, ctx),
-            },
-            None => Err(PyRuntimeError::new_err(
-                "[RUST] Invalid recursive encoder".to_string(),
-            )),
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct CustomEncoder {
-    pub(crate) inner: Box<TEncoder>,
-    pub(crate) dump: Option<Py<PyAny>>,
-    pub(crate) load: Option<Py<PyAny>>,
-}
-
-impl Encoder for CustomEncoder {
-    #[inline]
-    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
-        match self.dump {
-            Some(ref dump) => dump.bind(value.py()).call1((value,)),
-            None => self.inner.dump(value),
-        }
-    }
-
-    #[inline]
-    fn load<'a>(
-        &self,
-        value: &Bound<'a, PyAny>,
-        instance_path: &InstancePath,
-        ctx: &Context,
-    ) -> PyResult<Bound<'a, PyAny>> {
-        match self.load {
-            Some(ref load) => load.bind(value.py()).call1((value,)),
-            None => self.inner.load(value, instance_path, ctx),
-        }
-    }
-
-    fn is_sequence(&self) -> bool {
-        self.inner.is_sequence()
-    }
-}
+use std::collections::HashMap;
+use std::fmt::Debug;
+use std::sync::Arc;
+
+use atomic_refcell::AtomicRefCell;
+use dyn_clone::{clone_trait_object, DynClone};
+use pyo3::exceptions::PyRuntimeError;
+use pyo3::prelude::*;
+use pyo3::types::{
+    PyBool, PyBytes, PyDate, PyDateTime, PyDict, PyFloat, PyList, PyLong, PySequence, PyString,
+    PyTime,
+};
+use pyo3::{intern, Bound, Py, PyAny, PyResult};
+use uuid::Uuid;
+
+use crate::errors::{ToPyErr, ValidationError};
+use crate::python::{
+    create_py_dict_known_size, create_py_list, create_py_tuple, dump_date, dump_datetime,
+    dump_time, parse_date, parse_datetime, parse_time, py_dict_set_item, py_list_get_item,
+    py_list_set_item, py_tuple_set_item,
+};
+use crate::validator::types::{DecimalType, EnumItem, FloatType, IntegerType, StringType};
+use crate::validator::validators::{
+    check_bounds, check_length, check_sequence_size, invalid_enum_item, invalid_type,
+    invalid_type_dump, missing_required_property, no_encoder_for_discriminator, str_as_bool,
+};
+use crate::validator::{map_py_err_to_schema_validation_error, Context, InstancePath};
+
+pub type TEncoder = dyn Encoder + Send + Sync;
+
+pub trait Encoder: DynClone + Debug {
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>>;
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>>;
+
+    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
+        None
+    }
+    fn is_sequence(&self) -> bool {
+        false
+    }
+}
+
+pub struct EncoderField<'a> {
+    pub(crate) name: &'a Py<PyString>,
+    pub(crate) is_sequence: bool,
+}
+
+pub enum QueryFields<'a> {
+    Object(Vec<EncoderField<'a>>),
+    Dict(bool), // is_sequence
+}
+
+pub trait ContainerEncoder: Encoder {
+    fn get_fields(&self) -> QueryFields;
+}
+
+clone_trait_object!(Encoder);
+
+#[derive(Debug, Clone)]
+pub struct NoopEncoder;
+
+impl Encoder for NoopEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        _instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct IntEncoder {
+    pub(crate) type_info: IntegerType,
+}
+
+impl Encoder for IntEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyLong>() {
+            check_bounds!(val.extract()?, self.type_info, instance_path)?;
+            return Ok(value.clone());
+        }
+        if ctx.try_cast_from_string {
+            if let Ok(val) = value.downcast::<PyString>() {
+                if let Ok(val) = val.to_str()?.parse::<i64>() {
+                    check_bounds!(val, self.type_info, instance_path)?;
+                    return Ok(val.to_object(value.py()).into_bound(value.py()));
+                }
+            }
+        }
+        invalid_type!("integer", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct FloatEncoder {
+    pub(crate) type_info: FloatType,
+}
+
+impl Encoder for FloatEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyLong>() {
+            check_bounds!(val.extract()?, self.type_info, instance_path)?;
+            return Ok(value.clone());
+        }
+        if let Ok(val) = value.downcast::<PyFloat>() {
+            check_bounds!(val.extract()?, self.type_info, instance_path)?;
+            return Ok(value.clone());
+        }
+        if ctx.try_cast_from_string {
+            if let Ok(val) = value.downcast::<PyString>() {
+                if let Ok(val) = val.to_str()?.parse::<f64>() {
+                    check_bounds!(val, self.type_info, instance_path)?;
+                    return Ok(val.to_object(value.py()).into_bound(value.py()));
+                }
+            }
+        }
+        invalid_type!("number", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct DecimalEncoder {
+    pub(crate) type_info: DecimalType,
+    pub(crate) decimal_cls: Py<PyAny>,
+}
+
+impl Encoder for DecimalEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.str()?.into_any())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let valid = if let Ok(val) = value.downcast::<PyFloat>() {
+            check_bounds!(val.value(), self.type_info, instance_path)?;
+            true
+        } else if let Ok(val) = value.downcast::<PyLong>() {
+            check_bounds!(val.extract()?, self.type_info, instance_path)?;
+            true
+        } else if let Ok(val) = value.downcast::<PyString>() {
+            match val.to_str()?.parse::<f64>() {
+                Ok(val_f64) => {
+                    check_bounds!(val_f64, self.type_info, instance_path)?;
+                    true
+                }
+                Err(_) => false,
+            }
+        } else {
+            false
+        };
+        if valid {
+            let str_value = value.str().expect("Failed to convert value to string.");
+            self.decimal_cls.bind(value.py()).call1((str_value,))
+        } else {
+            invalid_type!("decimal", value, instance_path)
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct StringEncoder {
+    pub(crate) type_info: StringType,
+}
+
+impl Encoder for StringEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyString>() {
+            check_length(
+                val,
+                self.type_info.min_length,
+                self.type_info.max_length,
+                instance_path,
+            )?;
+            Ok(value.clone())
+        } else {
+            invalid_type!("string", value, instance_path)
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct BooleanEncoder {}
+
+impl Encoder for BooleanEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(_val) = value.downcast::<PyBool>() {
+            return Ok(value.clone());
+        }
+        if ctx.try_cast_from_string {
+            if let Ok(val) = value.downcast::<PyString>() {
+                if let Some(val) = str_as_bool(val.to_str()?) {
+                    return Ok(val.to_object(value.py()).into_bound(value.py()));
+                }
+            }
+        }
+
+        invalid_type!("boolean", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct BytesEncoder {}
+
+impl Encoder for BytesEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(_val) = value.downcast::<PyBytes>() {
+            Ok(value.clone())
+        } else {
+            invalid_type!("bytes", value, instance_path)
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct DictionaryEncoder {
+    pub(crate) key_encoder: Box<TEncoder>,
+    pub(crate) value_encoder: Box<TEncoder>,
+    pub(crate) omit_none: bool,
+}
+
+impl Encoder for DictionaryEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(dict) = value.downcast::<PyDict>() {
+            let result_dict = create_py_dict_known_size(dict.py(), dict.len());
+            for (k, v) in dict.iter() {
+                let key = self.key_encoder.dump(&k)?;
+                let value = self.value_encoder.dump(&v)?;
+                if !self.omit_none || !value.is_none() {
+                    py_dict_set_item(&result_dict, key.as_ptr(), value)?;
+                }
+            }
+            Ok(result_dict.into_any())
+        } else {
+            invalid_type_dump!("dict", value)
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyDict>() {
+            let result_dict = create_py_dict_known_size(val.py(), val.len());
+            for (k, v) in val.iter() {
+                let instance_path = instance_path.push(&k);
+                let key = self.key_encoder.load(&k, &instance_path, ctx)?;
+                let value = self.value_encoder.load(&v, &instance_path, ctx)?;
+                py_dict_set_item(&result_dict, key.as_ptr(), value)?;
+            }
+            Ok(result_dict.into_any())
+        } else {
+            invalid_type_dump!("dict", value)
+        }
+    }
+
+    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
+        Some(self)
+    }
+}
+
+impl ContainerEncoder for DictionaryEncoder {
+    fn get_fields(&self) -> QueryFields {
+        QueryFields::Dict(self.value_encoder.is_sequence())
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct ArrayEncoder {
+    pub(crate) encoder: Box<TEncoder>,
+}
+
+impl Encoder for ArrayEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(list) = value.downcast::<PyList>() {
+            let size = list.len();
+            let result = create_py_list(value.py(), size);
+
+            for index in 0..size {
+                let item = py_list_get_item(list, index);
+                let val = self.encoder.dump(&item)?;
+                py_list_set_item(&result, index, val);
+            }
+
+            Ok(result.into_any())
+        } else {
+            invalid_type_dump!("list", value)
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyList>() {
+            let size = val.len();
+            let result = create_py_list(value.py(), size);
+
+            for index in 0..size {
+                let item = py_list_get_item(val, index);
+                let instance_path = instance_path.push(index);
+                let val = self.encoder.load(&item, &instance_path, ctx)?;
+                py_list_set_item(&result, index, val);
+            }
+            Ok(result.into_any())
+        } else {
+            invalid_type!("list", value, instance_path)
+        }
+    }
+
+    fn is_sequence(&self) -> bool {
+        true
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct EntityEncoder {
+    pub(crate) cls: Py<PyAny>,
+    pub(crate) omit_none: bool,
+    pub(crate) is_frozen: bool,
+    pub(crate) fields: Vec<Field>,
+    pub(crate) create_object: Py<PyAny>,
+    pub(crate) object_set_attr: Py<PyAny>,
+}
+
+#[derive(Debug, Clone)]
+pub struct Field {
+    pub(crate) name: Py<PyString>,
+    pub(crate) dict_key: Py<PyString>,
+    pub(crate) dict_key_rs: String,
+    pub(crate) encoder: Box<TEncoder>,
+    pub(crate) required: bool,
+    pub(crate) default: Option<Py<PyAny>>,
+    pub(crate) default_factory: Option<Py<PyAny>>,
+}
+
+impl Encoder for EntityEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let dict = create_py_dict_known_size(value.py(), self.fields.len());
+
+        for field in &self.fields {
+            let field_val = value.getattr(&field.name)?;
+            let dump_result = field.encoder.dump(&field_val)?;
+            if field.required || !self.omit_none || !dump_result.is_none() {
+                py_dict_set_item(&dict, field.dict_key.as_ptr(), dump_result)?;
+            }
+        }
+
+        Ok(dict.into_any())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let py_frozen_object_set_attr = self.object_set_attr.bind(value.py());
+        if let Ok(val) = value.downcast::<PyDict>() {
+            let obj = self
+                .create_object
+                .bind(value.py())
+                .call1((self.cls.bind(value.py()),))?;
+            for field in &self.fields {
+                let val = match val.get_item(&field.dict_key)? {
+                    Some(val) => {
+                        let instance_path =
+                            instance_path.push(field.dict_key.bind(value.py()).as_any());
+                        field.encoder.load(&val, &instance_path, ctx)?
+                    }
+                    None => match (&field.default, &field.default_factory) {
+                        (Some(val), _) => val.bind(value.py()).clone(),
+                        (_, Some(val)) => val.bind(value.py()).call0()?,
+                        (None, _) => {
+                            return Err(missing_required_property(
+                                &field.dict_key_rs,
+                                instance_path,
+                            ));
+                        }
+                    },
+                };
+
+                if self.is_frozen {
+                    py_frozen_object_set_attr.call1((&obj, &field.name, val))?;
+                } else {
+                    obj.setattr(&field.name, val)?;
+                };
+            }
+
+            Ok(obj)
+        } else {
+            invalid_type!("object", value, instance_path)
+        }
+    }
+
+    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
+        Some(self)
+    }
+}
+
+impl ContainerEncoder for EntityEncoder {
+    fn get_fields(&self) -> QueryFields {
+        QueryFields::Object(
+            self.fields
+                .iter()
+                .map(|f| EncoderField {
+                    name: &f.dict_key,
+                    is_sequence: f.encoder.is_sequence(),
+                })
+                .collect(),
+        )
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct TypedDictEncoder {
+    pub(crate) omit_none: bool,
+    pub(crate) fields: Vec<Field>,
+}
+
+impl Encoder for TypedDictEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let value = match value.downcast::<PyDict>() {
+            Ok(val) => val,
+            _ => invalid_type_dump!("dict", value),
+        };
+        let dict = create_py_dict_known_size(value.py(), self.fields.len());
+        for field in &self.fields {
+            let field_val = match value.get_item(&field.name) {
+                Ok(Some(val)) => val,
+                _ => {
+                    if field.required {
+                        return Err(ValidationError::new_err(format!(
+                            "data dictionary is missing required parameter {}",
+                            &field.name
+                        )));
+                    } else {
+                        continue;
+                    }
+                }
+            };
+            let dump_result = field.encoder.dump(&field_val)?;
+            if field.required || !self.omit_none || !dump_result.is_none() {
+                py_dict_set_item(&dict, field.dict_key.as_ptr(), dump_result)?;
+            }
+        }
+        Ok(dict.into_any())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let value = match value.downcast::<PyDict>() {
+            Ok(val) => val,
+            Err(_) => {
+                invalid_type_dump!("dict", value);
+            }
+        };
+        let dict = create_py_dict_known_size(value.py(), self.fields.len());
+        for field in &self.fields {
+            let field_val = match value.get_item(&field.dict_key) {
+                Ok(Some(val)) => val,
+                _ => {
+                    if field.required {
+                        return Err(missing_required_property(&field.dict_key_rs, instance_path));
+                    } else {
+                        continue;
+                    }
+                }
+            };
+            let instance_path = instance_path.push(field.dict_key_rs.as_str());
+            let dump_result = field.encoder.load(&field_val, &instance_path, ctx)?;
+            py_dict_set_item(&dict, field.name.as_ptr(), dump_result)?;
+        }
+        Ok(dict.into_any())
+    }
+    fn as_container_encoder(&self) -> Option<&dyn ContainerEncoder> {
+        Some(self)
+    }
+}
+
+impl ContainerEncoder for TypedDictEncoder {
+    fn get_fields(&self) -> QueryFields {
+        QueryFields::Object(
+            self.fields
+                .iter()
+                .map(|f| EncoderField {
+                    name: &f.dict_key,
+                    is_sequence: f.encoder.is_sequence(),
+                })
+                .collect(),
+        )
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct UUIDEncoder {
+    pub(crate) uuid_cls: Py<PyAny>,
+}
+
+impl Encoder for UUIDEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.str()?.into_any())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyString>() {
+            if Uuid::parse_str(val.to_str()?).is_ok() {
+                if let Ok(result) = self.uuid_cls.bind(value.py()).call1((val,)) {
+                    return Ok(result);
+                }
+            }
+        }
+        invalid_type!("uuid", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct EnumEncoder {
+    pub(crate) enum_items: Vec<(EnumItem, Py<PyAny>)>,
+}
+
+impl Encoder for EnumEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let value_str = intern!(value.py(), "value");
+        Ok(value.getattr(value_str)?.into_any())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let val = if let Ok(val) = value.downcast::<PyString>() {
+            EnumItem::String(val.to_str()?.to_owned())
+        } else if let Ok(val) = value.downcast::<PyLong>() {
+            EnumItem::Int(val.extract()?)
+        } else {
+            invalid_enum_item!((&self.enum_items).into(), value, instance_path);
+        };
+
+        let index = self.enum_items.binary_search_by(|(e, _)| e.cmp(&val));
+
+        match index {
+            Ok(index) => {
+                let (_, py_item) = &self.enum_items[index];
+                return Ok(py_item.bind(value.py()).clone());
+            }
+            Err(_) if ctx.try_cast_from_string => {
+                if let Ok(value) = value.downcast::<PyString>() {
+                    if let Ok(val) = value.to_str()?.parse::<i64>() {
+                        if let Ok(index) = self
+                            .enum_items
+                            .binary_search_by(|(e, _)| e.cmp(&EnumItem::Int(val)))
+                        {
+                            let (_, py_item) = &self.enum_items[index];
+                            return Ok(py_item.bind(value.py()).clone());
+                        }
+                    }
+                }
+            }
+            _ => {}
+        }
+
+        invalid_enum_item!((&self.enum_items).into(), value, instance_path);
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct LiteralEncoder {
+    pub(crate) enum_items: Vec<(EnumItem, Py<PyAny>)>,
+}
+
+impl Encoder for LiteralEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        Ok(value.clone())
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let val = if let Ok(val) = value.downcast::<PyString>() {
+            EnumItem::String(val.to_str()?.to_owned())
+        } else if let Ok(val) = value.downcast::<PyLong>() {
+            EnumItem::Int(val.extract()?)
+        } else {
+            invalid_enum_item!((&self.enum_items).into(), value, instance_path);
+        };
+
+        let index = self.enum_items.binary_search_by(|(e, _)| e.cmp(&val));
+
+        match index {
+            Ok(index) => {
+                let (_, py_item) = &self.enum_items[index];
+                return Ok(py_item.bind(value.py()).clone());
+            }
+            Err(_) if ctx.try_cast_from_string => {
+                if let Ok(value) = value.downcast::<PyString>() {
+                    if let Ok(val) = value.to_str()?.parse::<i64>() {
+                        if let Ok(index) = self
+                            .enum_items
+                            .binary_search_by(|(e, _)| e.cmp(&EnumItem::Int(val)))
+                        {
+                            let (_, py_item) = &self.enum_items[index];
+                            return Ok(py_item.bind(value.py()).clone());
+                        }
+                    }
+                }
+            }
+            _ => {}
+        }
+
+        invalid_enum_item!((&self.enum_items).into(), value, instance_path);
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct OptionalEncoder {
+    pub(crate) encoder: Box<TEncoder>,
+}
+
+impl Encoder for OptionalEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        if value.is_none() {
+            Ok(value.clone())
+        } else {
+            self.encoder.dump(value)
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if value.is_none() {
+            Ok(value.clone())
+        } else {
+            self.encoder.load(value, instance_path, ctx)
+        }
+    }
+
+    fn is_sequence(&self) -> bool {
+        self.encoder.is_sequence()
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct TupleEncoder {
+    pub(crate) encoders: Vec<Box<TEncoder>>,
+}
+
+impl Encoder for TupleEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(seq) = value.downcast::<PySequence>() {
+            let seq_len = seq.len()?;
+            check_sequence_size(seq, seq_len, self.encoders.len(), None)?;
+            let result = create_py_list(value.py(), seq_len);
+            for index in 0..seq_len {
+                let item = seq.get_item(index)?;
+                let val = self.encoders[index].dump(&item)?;
+                py_list_set_item(&result, index, val);
+            }
+
+            Ok(result.into_any())
+        } else {
+            invalid_type_dump!("sequence", value)
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        // Check sequence is not str
+        if let Ok(seq) = value.downcast::<PySequence>() {
+            if value.is_instance_of::<PyString>() {
+                invalid_type!("sequence", value, instance_path);
+            }
+            let seq_len = seq.len()?;
+            check_sequence_size(seq, seq_len, self.encoders.len(), Some(instance_path))?;
+            let result = create_py_tuple(value.py(), seq_len);
+            for index in 0..seq_len {
+                let item = seq.get_item(index)?;
+                let instance_path = instance_path.push(index);
+                let val = self.encoders[index].load(&item, &instance_path, ctx)?;
+                py_tuple_set_item(&result, index, val);
+            }
+            Ok(result.into_any())
+        } else {
+            invalid_type!("sequence", value, instance_path)
+        }
+    }
+
+    fn is_sequence(&self) -> bool {
+        true
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct UnionEncoder {
+    pub(crate) encoders: Vec<Box<TEncoder>>,
+    pub(crate) union_repr: String,
+}
+
+impl Encoder for UnionEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        for encoder in &self.encoders {
+            let result = encoder.dump(value);
+            if result.is_ok() {
+                return result;
+            }
+        }
+        invalid_type_dump!(&self.union_repr, value)
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        for encoder in &self.encoders {
+            let result = encoder.load(value, instance_path, ctx);
+            if result.is_ok() {
+                return result;
+            }
+        }
+        invalid_type!(&self.union_repr, value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct DiscriminatedUnionEncoder {
+    pub(crate) encoders: HashMap<String, Box<TEncoder>>,
+    pub(crate) dump_discriminator: Py<PyString>,
+    pub(crate) load_discriminator: Py<PyString>,
+    pub(crate) load_discriminator_rs: String,
+    pub(crate) keys: Vec<String>,
+}
+
+impl Encoder for DiscriminatedUnionEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let key = match value.getattr(&self.dump_discriminator) {
+            Ok(val) => val.str()?,
+            Err(_) => {
+                return Err(missing_required_property(
+                    self.dump_discriminator.bind(value.py()).str()?.to_str()?,
+                    &InstancePath::new(),
+                ));
+            }
+        };
+
+        let str_key = key.to_str()?;
+
+        let encoder = self.encoders.get(str_key).ok_or_else(|| {
+            let instance_path = InstancePath::new();
+            no_encoder_for_discriminator(str_key, &self.keys, &instance_path)
+        })?;
+        encoder.dump(value)
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyDict>() {
+            let key_any = match val.get_item(&self.load_discriminator) {
+                Ok(Some(k)) => k,
+                _ => {
+                    return Err(missing_required_property(
+                        &self.load_discriminator_rs,
+                        instance_path,
+                    ));
+                }
+            };
+
+            let key_py_string = key_any
+                .downcast::<PyString>()
+                .expect("key must be a string");
+            let key_str = key_py_string.to_str()?;
+            let encoder = self.encoders.get(key_str).ok_or_else(|| {
+                let instance_path = instance_path.push(self.load_discriminator_rs.as_str());
+                no_encoder_for_discriminator(key_str, &self.keys, &instance_path)
+            })?;
+            encoder.load(value, instance_path, ctx)
+        } else {
+            invalid_type!("dict", value, instance_path)
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct TimeEncoder {}
+
+impl Encoder for TimeEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let py_time = value.downcast::<PyTime>()?;
+        let result = dump_time(py_time)?;
+        Ok(result.into_py(value.py()).into_bound(value.py()))
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyString>() {
+            if let Ok(result) = parse_time(value.py(), val.to_str()?) {
+                return Ok(result.into_any());
+            }
+        }
+        invalid_type!("time", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct DateTimeEncoder {
+    pub(crate) naive_datetime_to_utc: bool,
+}
+
+impl Encoder for DateTimeEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let py_datetime = value.downcast::<PyDateTime>()?;
+        let result = dump_datetime(py_datetime, self.naive_datetime_to_utc)?;
+        Ok(result.into_py(value.py()).into_bound(value.py()))
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyString>() {
+            if let Ok(result) = parse_datetime(value.py(), val.to_str()?) {
+                return Ok(result.into_any());
+            }
+        }
+        invalid_type!("datetime", value, instance_path)
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct DateEncoder {}
+
+impl Encoder for DateEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        let py_date = value.downcast::<PyDate>()?;
+        let result = dump_date(py_date)?;
+        Ok(result.into_py(value.py()).into_bound(value.py()))
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        if let Ok(val) = value.downcast::<PyString>() {
+            if let Ok(result) = parse_date(value.py(), val.to_str()?) {
+                return Ok(result.into_any());
+            }
+        }
+        invalid_type!("date", value, instance_path)
+    }
+}
+
+#[derive(Debug)]
+pub enum Encoders {
+    Entity(EntityEncoder),
+    TypedDict(TypedDictEncoder),
+}
+
+#[derive(Debug, Clone)]
+pub struct LazyEncoder {
+    pub(crate) inner: Arc<AtomicRefCell<Option<Encoders>>>,
+}
+
+impl Encoder for LazyEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        match self.inner.borrow().as_ref() {
+            Some(encoder) => match encoder {
+                Encoders::Entity(encoder) => encoder.dump(value),
+                Encoders::TypedDict(encoder) => encoder.dump(value),
+            },
+            None => Err(PyRuntimeError::new_err(
+                "[RUST] Invalid recursive encoder".to_string(),
+            )),
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        match self.inner.borrow().as_ref() {
+            Some(encoder) => match encoder {
+                Encoders::Entity(encoder) => encoder.load(value, instance_path, ctx),
+                Encoders::TypedDict(encoder) => encoder.load(value, instance_path, ctx),
+            },
+            None => Err(PyRuntimeError::new_err(
+                "[RUST] Invalid recursive encoder".to_string(),
+            )),
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct CustomEncoder {
+    pub(crate) inner: Box<TEncoder>,
+    pub(crate) dump: Option<Py<PyAny>>,
+    pub(crate) load: Option<Py<PyAny>>,
+}
+
+impl Encoder for CustomEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        match self.dump {
+            Some(ref dump) => dump.bind(value.py()).call1((value,)),
+            None => self.inner.dump(value),
+        }
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        match self.load {
+            Some(ref load) => load.bind(value.py()).call1((value,)).map_err(|err| {
+                map_py_err_to_schema_validation_error(value.py(), err, instance_path)
+            }),
+            None => self.inner.load(value, instance_path, ctx),
+        }
+    }
+
+    fn is_sequence(&self) -> bool {
+        self.inner.is_sequence()
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct CustomTypeEncoder {
+    pub(crate) dump: Py<PyAny>,
+    pub(crate) load: Py<PyAny>,
+}
+
+impl Encoder for CustomTypeEncoder {
+    #[inline]
+    fn dump<'a>(&self, value: &Bound<'a, PyAny>) -> PyResult<Bound<'a, PyAny>> {
+        self.dump.bind(value.py()).call1((value,))
+    }
+
+    #[inline]
+    fn load<'a>(
+        &self,
+        value: &Bound<'a, PyAny>,
+        instance_path: &InstancePath,
+        _ctx: &Context,
+    ) -> PyResult<Bound<'a, PyAny>> {
+        let result = self.load.bind(value.py()).call1((value,));
+        result.map_err(|err| map_py_err_to_schema_validation_error(value.py(), err, instance_path))
+    }
+}
```

### Comparing `serpyco_rs-1.7.1/src/serializer/main.rs` & `serpyco_rs-1.8.0/src/serializer/main.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,413 +1,435 @@
-use std::collections::HashMap;
-use std::sync::Arc;
-
-use atomic_refcell::AtomicRefCell;
-use pyo3::exceptions::{PyKeyError, PyRuntimeError};
-use pyo3::prelude::*;
-use pyo3::types::{PyDict, PyList, PyMapping, PyString};
-use pyo3::{intern, PyAny, PyResult};
-
-use crate::python::{get_object_type, Type};
-use crate::serializer::encoders::{
-    BooleanEncoder, BytesEncoder, FloatEncoder, IntEncoder, LiteralEncoder, QueryFields,
-    StringEncoder, TypedDictEncoder, UnionEncoder,
-};
-use crate::validator::types::{BaseType, EntityField};
-use crate::validator::{types, Context, InstancePath};
-
-use super::encoders::{
-    ArrayEncoder, DecimalEncoder, DictionaryEncoder, EntityEncoder, EnumEncoder, Field,
-    NoopEncoder, OptionalEncoder, TupleEncoder, UUIDEncoder,
-};
-use super::encoders::{
-    CustomEncoder, DateEncoder, DateTimeEncoder, DiscriminatedUnionEncoder, Encoders, LazyEncoder,
-    TEncoder, TimeEncoder,
-};
-
-type EncoderStateValue = Arc<AtomicRefCell<Option<Encoders>>>;
-
-#[pyclass(frozen, module = "serde_json")]
-#[derive(Debug)]
-pub struct Serializer {
-    pub encoder: Box<TEncoder>,
-}
-
-#[pymethods]
-impl Serializer {
-    #[new]
-    fn new(type_info: &Bound<'_, PyAny>, naive_datetime_to_utc: bool) -> PyResult<Self> {
-        let obj_type = get_object_type(type_info)?;
-        let mut encoder_state: HashMap<usize, EncoderStateValue> = HashMap::new();
-
-        let serializer = Self {
-            encoder: get_encoder(
-                type_info.py(),
-                obj_type,
-                &mut encoder_state,
-                naive_datetime_to_utc,
-            )?,
-        };
-        Ok(serializer)
-    }
-
-    #[inline]
-    pub fn dump<'py>(&'py self, value: &Bound<'py, PyAny>) -> PyResult<Bound<'py, PyAny>> {
-        self.encoder.dump(value)
-    }
-
-    #[inline]
-    pub fn load<'py>(&'py self, value: &Bound<'py, PyAny>) -> PyResult<Bound<'py, PyAny>> {
-        let instance_path = InstancePath::new();
-        let ctx = Context::new(false);
-        self.encoder.load(value, &instance_path, &ctx)
-    }
-
-    #[inline]
-    pub fn load_query_params<'py>(
-        &'py self,
-        data: &Bound<'py, PyAny>,
-    ) -> PyResult<Bound<'py, PyAny>> {
-        let instance_path = InstancePath::new();
-        let ctx = Context::new(true);
-        let py = data.py();
-
-        let encoder = if let Some(encoder) = self.encoder.as_container_encoder() {
-            encoder
-        } else {
-            Err(PyRuntimeError::new_err(
-                "This type is not deserializable from query params",
-            ))?
-        };
-
-        let data = data.downcast::<PyMapping>()?;
-        let fields = encoder.get_fields();
-
-        let new_data = match fields {
-            QueryFields::Object(fields) => {
-                let new_data = PyDict::new_bound(py);
-                for field in fields {
-                    let field_value = if field.is_sequence {
-                        data.call_method1(intern!(py, "getall"), (field.name,))
-                    } else {
-                        data.get_item(field.name)
-                    };
-
-                    match field_value {
-                        Ok(val) => new_data.set_item(field.name, val)?,
-                        Err(e) if e.is_instance_of::<PyKeyError>(py) => {}
-                        Err(e) => return Err(e),
-                    }
-                }
-                new_data.into_any()
-            }
-            QueryFields::Dict(true) => {
-                let new_data = PyDict::new_bound(py);
-                for key in data.keys()?.iter()? {
-                    let key = key?;
-                    let field_value = data
-                        .call_method1(intern!(py, "getall"), (&key,))
-                        .expect("Mapping changing during iteration");
-                    new_data.set_item(&key, field_value)?;
-                }
-                new_data.into_any()
-            }
-            QueryFields::Dict(false) => {
-                let new_data = PyDict::from_sequence_bound(&data.items()?.into_any())?;
-                new_data.into_any()
-            }
-        };
-
-        encoder.load(&new_data, &instance_path, &ctx)
-    }
-}
-
-pub fn get_encoder(
-    py: Python<'_>,
-    obj_type: Type,
-    encoder_state: &mut HashMap<usize, EncoderStateValue>,
-    naive_datetime_to_utc: bool,
-) -> PyResult<Box<TEncoder>> {
-    let encoder: Box<TEncoder> = match obj_type {
-        Type::Integer(type_info, base_type) => {
-            let type_info = type_info.get().clone();
-            let encoder = IntEncoder { type_info };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::String(type_info, base_type) => {
-            let type_info = type_info.get().clone();
-            let encoder = StringEncoder { type_info };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Float(type_info, base_type) => {
-            let type_info = type_info.get().clone();
-            let encoder = FloatEncoder { type_info };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Decimal(type_info, base_type) => {
-            let type_info = type_info.get().clone();
-            let decimal_module = PyModule::import_bound(py, "decimal")?;
-            let decimal_cls = decimal_module.getattr("Decimal")?;
-            let encoder = DecimalEncoder {
-                type_info,
-                decimal_cls: decimal_cls.unbind(),
-            };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Boolean(_, base_type) => {
-            let encoder = BooleanEncoder {};
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Uuid(_, base_type) => {
-            let uuid = PyModule::import_bound(py, "uuid")?;
-            let uuid_cls = uuid.getattr("UUID")?;
-
-            let encoder = UUIDEncoder {
-                uuid_cls: uuid_cls.unbind(),
-            };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Time(_, base_type) => {
-            let encoder = TimeEncoder {};
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::DateTime(_, base_type) => {
-            let encoder = DateTimeEncoder {
-                naive_datetime_to_utc,
-            };
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Date(_, base_type) => {
-            let encoder = DateEncoder {};
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Bytes(_, base_type) => {
-            let encoder = BytesEncoder {};
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::Any(_, base_type) => wrap_with_custom_encoder(py, base_type, Box::new(NoopEncoder))?,
-        Type::Literal(type_info, base_type) => wrap_with_custom_encoder(
-            py,
-            base_type,
-            Box::new(LiteralEncoder {
-                enum_items: type_info.get().enum_items.clone(),
-            }),
-        )?,
-        Type::Optional(type_info, base_type) => {
-            let inner = get_object_type(type_info.get().inner.bind(py))?;
-            let encoder = get_encoder(py, inner, encoder_state, naive_datetime_to_utc)?;
-            wrap_with_custom_encoder(py, base_type, Box::new(OptionalEncoder { encoder }))?
-        }
-        Type::Dictionary(type_info, base_type) => {
-            let key_type = get_object_type(type_info.get().key_type.bind(py))?;
-            let value_type = get_object_type(type_info.get().value_type.bind(py))?;
-
-            let key_encoder = get_encoder(py, key_type, encoder_state, naive_datetime_to_utc)?;
-            let value_encoder = get_encoder(py, value_type, encoder_state, naive_datetime_to_utc)?;
-
-            wrap_with_custom_encoder(
-                py,
-                base_type,
-                Box::new(DictionaryEncoder {
-                    key_encoder,
-                    value_encoder,
-                    omit_none: type_info.get().omit_none,
-                }),
-            )?
-        }
-        Type::Array(type_info, base_type) => {
-            let item_type = get_object_type(type_info.get().item_type.bind(py))?;
-            let encoder = get_encoder(py, item_type, encoder_state, naive_datetime_to_utc)?;
-            wrap_with_custom_encoder(py, base_type, Box::new(ArrayEncoder { encoder }))?
-        }
-        Type::Tuple(type_info, base_type) => {
-            let mut encoders = vec![];
-            for item_type in &type_info.get().item_types {
-                let item_type = item_type.bind(py);
-                let encoder = get_encoder(
-                    py,
-                    get_object_type(item_type)?,
-                    encoder_state,
-                    naive_datetime_to_utc,
-                )?;
-                encoders.push(encoder);
-            }
-            wrap_with_custom_encoder(py, base_type, Box::new(TupleEncoder { encoders }))?
-        }
-        Type::Union(type_info, base_type) => {
-            let item_types = type_info.get().item_types.bind(py).downcast::<PyList>()?;
-
-            let mut encoders = vec![];
-
-            for value in item_types.iter() {
-                let encoder = get_encoder(
-                    py,
-                    get_object_type(&value)?,
-                    encoder_state,
-                    naive_datetime_to_utc,
-                )?;
-                encoders.push(encoder);
-            }
-
-            wrap_with_custom_encoder(
-                py,
-                base_type,
-                Box::new(UnionEncoder {
-                    encoders,
-                    union_repr: type_info.get().union_repr.clone(),
-                }),
-            )?
-        }
-        Type::DiscriminatedUnion(type_info, base_type) => {
-            let dump_discriminator = type_info
-                .get()
-                .dump_discriminator
-                .bind(py)
-                .downcast::<PyString>()?;
-
-            let load_discriminator = type_info
-                .get()
-                .load_discriminator
-                .bind(py)
-                .downcast::<PyString>()?;
-
-            let item_types = type_info.get().item_types.bind(py).downcast::<PyDict>()?;
-
-            let mut encoders = HashMap::new();
-            let mut keys = vec![];
-
-            for (key, value) in item_types.iter() {
-                let key = key.downcast::<PyString>()?;
-                let encoder = get_encoder(
-                    py,
-                    get_object_type(&value)?,
-                    encoder_state,
-                    naive_datetime_to_utc,
-                )?;
-                let rs_key: String = key.to_string_lossy().into();
-                keys.push(rs_key.clone());
-                encoders.insert(rs_key, encoder);
-            }
-
-            wrap_with_custom_encoder(
-                py,
-                base_type,
-                Box::new(DiscriminatedUnionEncoder {
-                    encoders,
-                    dump_discriminator: dump_discriminator.clone().unbind(),
-                    load_discriminator: load_discriminator.clone().unbind(),
-                    load_discriminator_rs: load_discriminator.to_string_lossy().into(),
-                    keys,
-                }),
-            )?
-        }
-        Type::Entity(type_info, base_type, python_object_id) => {
-            let type_info = type_info.get();
-            let fields =
-                iterate_on_fields(py, &type_info.fields, encoder_state, naive_datetime_to_utc)?;
-
-            let builtins = PyModule::import_bound(py, intern!(py, "builtins"))?;
-            let object = builtins.getattr(intern!(py, "object"))?;
-            let create_object = object.getattr(intern!(py, "__new__"))?;
-            let object_set_attr = object.getattr("__setattr__")?;
-
-            let encoder = EntityEncoder {
-                fields,
-                omit_none: type_info.omit_none,
-                is_frozen: type_info.is_frozen,
-                create_object: create_object.unbind(),
-                object_set_attr: object_set_attr.unbind(),
-                cls: type_info.cls.clone(),
-            };
-            let val = encoder_state.entry(python_object_id).or_default();
-            AtomicRefCell::<Option<Encoders>>::borrow_mut(val)
-                .replace(Encoders::Entity(encoder.clone()));
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::TypedDict(type_info, base_type, python_object_id) => {
-            let fields = iterate_on_fields(
-                py,
-                &type_info.get().fields,
-                encoder_state,
-                naive_datetime_to_utc,
-            )?;
-
-            let encoder = TypedDictEncoder {
-                fields,
-                omit_none: type_info.get().omit_none,
-            };
-            let val = encoder_state.entry(python_object_id).or_default();
-            AtomicRefCell::<Option<Encoders>>::borrow_mut(val)
-                .replace(Encoders::TypedDict(encoder.clone()));
-            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
-        }
-        Type::RecursionHolder(type_info, base_type) => {
-            let inner_type = type_info.get().get_inner_type(py)?;
-            let python_object_id = inner_type.as_ptr() as *const _ as usize;
-            let encoder = encoder_state.entry(python_object_id).or_default();
-            wrap_with_custom_encoder(
-                py,
-                base_type,
-                Box::new(LazyEncoder {
-                    inner: encoder.clone(),
-                }),
-            )?
-        }
-        Type::Enum(type_info, base_type) => wrap_with_custom_encoder(
-            py,
-            base_type,
-            Box::new(EnumEncoder {
-                enum_items: type_info.get().enum_items.clone(),
-            }),
-        )?,
-    };
-
-    Ok(encoder)
-}
-
-fn wrap_with_custom_encoder(
-    py: Python<'_>,
-    base_type: Bound<'_, BaseType>,
-    original_encoder: Box<TEncoder>,
-) -> PyResult<Box<TEncoder>> {
-    if let Some(custom_encoder_py) = base_type.get().custom_encoder.clone() {
-        let custom_encoder = custom_encoder_py.extract::<types::CustomEncoder>(py)?;
-
-        if custom_encoder.serialize.is_none() && custom_encoder.deserialize.is_none() {
-            return Ok(original_encoder);
-        }
-
-        Ok(Box::new(CustomEncoder {
-            inner: original_encoder,
-            dump: custom_encoder.serialize,
-            load: custom_encoder.deserialize,
-        }))
-    } else {
-        Ok(original_encoder)
-    }
-}
-
-fn iterate_on_fields(
-    py: Python<'_>,
-    entity_fields: &Vec<EntityField>,
-    encoder_state: &mut HashMap<usize, EncoderStateValue>,
-    naive_datetime_to_utc: bool,
-) -> PyResult<Vec<Field>> {
-    let mut fields = vec![];
-    for field in entity_fields {
-        let f_name = field.name.downcast_bound::<PyString>(py)?;
-        let dict_key = field.dict_key.downcast_bound::<PyString>(py)?;
-        let f_type = get_object_type(field.field_type.bind(py))?;
-
-        let fld = Field {
-            name: f_name.clone().unbind(),
-            dict_key: dict_key.clone().unbind(),
-            dict_key_rs: dict_key.to_string_lossy().into(),
-            encoder: get_encoder(py, f_type, encoder_state, naive_datetime_to_utc)?,
-            required: field.required,
-            default: field.default.clone().into(),
-            default_factory: field.default_factory.clone().into(),
-        };
-        fields.push(fld);
-    }
-    Ok(fields)
-}
+use std::collections::HashMap;
+use std::sync::Arc;
+
+use atomic_refcell::AtomicRefCell;
+use pyo3::exceptions::{PyKeyError, PyRuntimeError};
+use pyo3::prelude::*;
+use pyo3::types::{PyDict, PyList, PyMapping, PyString};
+use pyo3::{intern, PyAny, PyResult};
+
+use crate::python::{get_object_type, Type};
+use crate::serializer::encoders::{
+    BooleanEncoder, BytesEncoder, CustomTypeEncoder, FloatEncoder, IntEncoder, LiteralEncoder,
+    QueryFields, StringEncoder, TypedDictEncoder, UnionEncoder,
+};
+use crate::validator::types::{BaseType, EntityField};
+use crate::validator::{types, Context, InstancePath};
+
+use super::encoders::{
+    ArrayEncoder, DecimalEncoder, DictionaryEncoder, EntityEncoder, EnumEncoder, Field,
+    NoopEncoder, OptionalEncoder, TupleEncoder, UUIDEncoder,
+};
+use super::encoders::{
+    CustomEncoder, DateEncoder, DateTimeEncoder, DiscriminatedUnionEncoder, Encoders, LazyEncoder,
+    TEncoder, TimeEncoder,
+};
+
+type EncoderStateValue = Arc<AtomicRefCell<Option<Encoders>>>;
+
+#[pyclass(frozen, module = "serde_json")]
+#[derive(Debug)]
+pub struct Serializer {
+    pub encoder: Box<TEncoder>,
+}
+
+#[pymethods]
+impl Serializer {
+    #[new]
+    fn new(type_info: &Bound<'_, PyAny>, naive_datetime_to_utc: bool) -> PyResult<Self> {
+        let obj_type = get_object_type(type_info)?;
+        let mut encoder_state: HashMap<usize, EncoderStateValue> = HashMap::new();
+
+        let serializer = Self {
+            encoder: get_encoder(
+                type_info.py(),
+                obj_type,
+                &mut encoder_state,
+                naive_datetime_to_utc,
+            )?,
+        };
+        Ok(serializer)
+    }
+
+    #[inline]
+    pub fn dump<'py>(&'py self, value: &Bound<'py, PyAny>) -> PyResult<Bound<'py, PyAny>> {
+        self.encoder.dump(value)
+    }
+
+    #[inline]
+    pub fn load<'py>(&'py self, value: &Bound<'py, PyAny>) -> PyResult<Bound<'py, PyAny>> {
+        let instance_path = InstancePath::new();
+        let ctx = Context::new(false);
+        self.encoder.load(value, &instance_path, &ctx)
+    }
+
+    #[inline]
+    pub fn load_query_params<'py>(
+        &'py self,
+        data: &Bound<'py, PyAny>,
+    ) -> PyResult<Bound<'py, PyAny>> {
+        let instance_path = InstancePath::new();
+        let ctx = Context::new(true);
+        let py = data.py();
+
+        let encoder = if let Some(encoder) = self.encoder.as_container_encoder() {
+            encoder
+        } else {
+            Err(PyRuntimeError::new_err(
+                "This type is not deserializable from query params",
+            ))?
+        };
+
+        let data = data.downcast::<PyMapping>()?;
+        let fields = encoder.get_fields();
+
+        let new_data = match fields {
+            QueryFields::Object(fields) => {
+                let new_data = PyDict::new_bound(py);
+                for field in fields {
+                    let field_value = if field.is_sequence {
+                        data.call_method1(intern!(py, "getall"), (field.name,))
+                    } else {
+                        data.get_item(field.name)
+                    };
+
+                    match field_value {
+                        Ok(val) => new_data.set_item(field.name, val)?,
+                        Err(e) if e.is_instance_of::<PyKeyError>(py) => {}
+                        Err(e) => return Err(e),
+                    }
+                }
+                new_data.into_any()
+            }
+            QueryFields::Dict(true) => {
+                let new_data = PyDict::new_bound(py);
+                for key in data.keys()?.iter()? {
+                    let key = key?;
+                    let field_value = data
+                        .call_method1(intern!(py, "getall"), (&key,))
+                        .expect("Mapping changing during iteration");
+                    new_data.set_item(&key, field_value)?;
+                }
+                new_data.into_any()
+            }
+            QueryFields::Dict(false) => {
+                let new_data = PyDict::from_sequence_bound(&data.items()?.into_any())?;
+                new_data.into_any()
+            }
+        };
+
+        encoder.load(&new_data, &instance_path, &ctx)
+    }
+}
+
+pub fn get_encoder(
+    py: Python<'_>,
+    obj_type: Type,
+    encoder_state: &mut HashMap<usize, EncoderStateValue>,
+    naive_datetime_to_utc: bool,
+) -> PyResult<Box<TEncoder>> {
+    let encoder: Box<TEncoder> = match obj_type {
+        Type::Integer(type_info, base_type) => {
+            let type_info = type_info.get().clone();
+            let encoder = IntEncoder { type_info };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::String(type_info, base_type) => {
+            let type_info = type_info.get().clone();
+            let encoder = StringEncoder { type_info };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Float(type_info, base_type) => {
+            let type_info = type_info.get().clone();
+            let encoder = FloatEncoder { type_info };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Decimal(type_info, base_type) => {
+            let type_info = type_info.get().clone();
+            let decimal_module = PyModule::import_bound(py, "decimal")?;
+            let decimal_cls = decimal_module.getattr("Decimal")?;
+            let encoder = DecimalEncoder {
+                type_info,
+                decimal_cls: decimal_cls.unbind(),
+            };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Boolean(_, base_type) => {
+            let encoder = BooleanEncoder {};
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Uuid(_, base_type) => {
+            let uuid = PyModule::import_bound(py, "uuid")?;
+            let uuid_cls = uuid.getattr("UUID")?;
+
+            let encoder = UUIDEncoder {
+                uuid_cls: uuid_cls.unbind(),
+            };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Time(_, base_type) => {
+            let encoder = TimeEncoder {};
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::DateTime(_, base_type) => {
+            let encoder = DateTimeEncoder {
+                naive_datetime_to_utc,
+            };
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Date(_, base_type) => {
+            let encoder = DateEncoder {};
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Bytes(_, base_type) => {
+            let encoder = BytesEncoder {};
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::Any(_, base_type) => wrap_with_custom_encoder(py, base_type, Box::new(NoopEncoder))?,
+        Type::Literal(type_info, base_type) => wrap_with_custom_encoder(
+            py,
+            base_type,
+            Box::new(LiteralEncoder {
+                enum_items: type_info.get().enum_items.clone(),
+            }),
+        )?,
+        Type::Optional(type_info, base_type) => {
+            let inner = get_object_type(type_info.get().inner.bind(py))?;
+            let encoder = get_encoder(py, inner, encoder_state, naive_datetime_to_utc)?;
+            wrap_with_custom_encoder(py, base_type, Box::new(OptionalEncoder { encoder }))?
+        }
+        Type::Dictionary(type_info, base_type) => {
+            let key_type = get_object_type(type_info.get().key_type.bind(py))?;
+            let value_type = get_object_type(type_info.get().value_type.bind(py))?;
+
+            let key_encoder = get_encoder(py, key_type, encoder_state, naive_datetime_to_utc)?;
+            let value_encoder = get_encoder(py, value_type, encoder_state, naive_datetime_to_utc)?;
+
+            wrap_with_custom_encoder(
+                py,
+                base_type,
+                Box::new(DictionaryEncoder {
+                    key_encoder,
+                    value_encoder,
+                    omit_none: type_info.get().omit_none,
+                }),
+            )?
+        }
+        Type::Array(type_info, base_type) => {
+            let item_type = get_object_type(type_info.get().item_type.bind(py))?;
+            let encoder = get_encoder(py, item_type, encoder_state, naive_datetime_to_utc)?;
+            wrap_with_custom_encoder(py, base_type, Box::new(ArrayEncoder { encoder }))?
+        }
+        Type::Tuple(type_info, base_type) => {
+            let mut encoders = vec![];
+            for item_type in &type_info.get().item_types {
+                let item_type = item_type.bind(py);
+                let encoder = get_encoder(
+                    py,
+                    get_object_type(item_type)?,
+                    encoder_state,
+                    naive_datetime_to_utc,
+                )?;
+                encoders.push(encoder);
+            }
+            wrap_with_custom_encoder(py, base_type, Box::new(TupleEncoder { encoders }))?
+        }
+        Type::Union(type_info, base_type) => {
+            let item_types = type_info.get().item_types.bind(py).downcast::<PyList>()?;
+
+            let mut encoders = vec![];
+
+            for value in item_types.iter() {
+                let encoder = get_encoder(
+                    py,
+                    get_object_type(&value)?,
+                    encoder_state,
+                    naive_datetime_to_utc,
+                )?;
+                encoders.push(encoder);
+            }
+
+            wrap_with_custom_encoder(
+                py,
+                base_type,
+                Box::new(UnionEncoder {
+                    encoders,
+                    union_repr: type_info.get().union_repr.clone(),
+                }),
+            )?
+        }
+        Type::DiscriminatedUnion(type_info, base_type) => {
+            let dump_discriminator = type_info
+                .get()
+                .dump_discriminator
+                .bind(py)
+                .downcast::<PyString>()?;
+
+            let load_discriminator = type_info
+                .get()
+                .load_discriminator
+                .bind(py)
+                .downcast::<PyString>()?;
+
+            let item_types = type_info.get().item_types.bind(py).downcast::<PyDict>()?;
+
+            let mut encoders = HashMap::new();
+            let mut keys = vec![];
+
+            for (key, value) in item_types.iter() {
+                let key = key.downcast::<PyString>()?;
+                let encoder = get_encoder(
+                    py,
+                    get_object_type(&value)?,
+                    encoder_state,
+                    naive_datetime_to_utc,
+                )?;
+                let rs_key: String = key.to_string_lossy().into();
+                keys.push(rs_key.clone());
+                encoders.insert(rs_key, encoder);
+            }
+
+            wrap_with_custom_encoder(
+                py,
+                base_type,
+                Box::new(DiscriminatedUnionEncoder {
+                    encoders,
+                    dump_discriminator: dump_discriminator.clone().unbind(),
+                    load_discriminator: load_discriminator.clone().unbind(),
+                    load_discriminator_rs: load_discriminator.to_string_lossy().into(),
+                    keys,
+                }),
+            )?
+        }
+        Type::Entity(type_info, base_type, python_object_id) => {
+            let type_info = type_info.get();
+            let fields =
+                iterate_on_fields(py, &type_info.fields, encoder_state, naive_datetime_to_utc)?;
+
+            let builtins = PyModule::import_bound(py, intern!(py, "builtins"))?;
+            let object = builtins.getattr(intern!(py, "object"))?;
+            let create_object = object.getattr(intern!(py, "__new__"))?;
+            let object_set_attr = object.getattr("__setattr__")?;
+
+            let encoder = EntityEncoder {
+                fields,
+                omit_none: type_info.omit_none,
+                is_frozen: type_info.is_frozen,
+                create_object: create_object.unbind(),
+                object_set_attr: object_set_attr.unbind(),
+                cls: type_info.cls.clone(),
+            };
+            let val = encoder_state.entry(python_object_id).or_default();
+            AtomicRefCell::<Option<Encoders>>::borrow_mut(val)
+                .replace(Encoders::Entity(encoder.clone()));
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::TypedDict(type_info, base_type, python_object_id) => {
+            let fields = iterate_on_fields(
+                py,
+                &type_info.get().fields,
+                encoder_state,
+                naive_datetime_to_utc,
+            )?;
+
+            let encoder = TypedDictEncoder {
+                fields,
+                omit_none: type_info.get().omit_none,
+            };
+            let val = encoder_state.entry(python_object_id).or_default();
+            AtomicRefCell::<Option<Encoders>>::borrow_mut(val)
+                .replace(Encoders::TypedDict(encoder.clone()));
+            wrap_with_custom_encoder(py, base_type, Box::new(encoder))?
+        }
+        Type::RecursionHolder(type_info, base_type) => {
+            let inner_type = type_info.get().get_inner_type(py)?;
+            let python_object_id = inner_type.as_ptr() as *const _ as usize;
+            let encoder = encoder_state.entry(python_object_id).or_default();
+            wrap_with_custom_encoder(
+                py,
+                base_type,
+                Box::new(LazyEncoder {
+                    inner: encoder.clone(),
+                }),
+            )?
+        }
+        Type::Enum(type_info, base_type) => wrap_with_custom_encoder(
+            py,
+            base_type,
+            Box::new(EnumEncoder {
+                enum_items: type_info.get().enum_items.clone(),
+            }),
+        )?,
+        Type::Custom(_, base_type) => {
+            if let Some(custom_encoder_py) = base_type.get().custom_encoder.clone() {
+                let custom_encoder = custom_encoder_py.extract::<types::CustomEncoder>(py)?;
+
+                if custom_encoder.serialize.is_none() || custom_encoder.deserialize.is_none() {
+                    return Err(PyRuntimeError::new_err(
+                        "CustomType must have both serialize and deserialize methods",
+                    ));
+                }
+                let serialize = custom_encoder.serialize.unwrap();
+                let deserialize = custom_encoder.deserialize.unwrap();
+
+                Box::new(CustomTypeEncoder {
+                    dump: serialize,
+                    load: deserialize,
+                })
+            } else {
+                return Err(PyRuntimeError::new_err(
+                    "CustomType must have both serialize and deserialize methods",
+                ));
+            }
+        }
+    };
+
+    Ok(encoder)
+}
+
+fn wrap_with_custom_encoder(
+    py: Python<'_>,
+    base_type: Bound<'_, BaseType>,
+    original_encoder: Box<TEncoder>,
+) -> PyResult<Box<TEncoder>> {
+    if let Some(custom_encoder_py) = base_type.get().custom_encoder.clone() {
+        let custom_encoder = custom_encoder_py.extract::<types::CustomEncoder>(py)?;
+
+        if custom_encoder.serialize.is_none() && custom_encoder.deserialize.is_none() {
+            return Ok(original_encoder);
+        }
+
+        Ok(Box::new(CustomEncoder {
+            inner: original_encoder,
+            dump: custom_encoder.serialize,
+            load: custom_encoder.deserialize,
+        }))
+    } else {
+        Ok(original_encoder)
+    }
+}
+
+fn iterate_on_fields(
+    py: Python<'_>,
+    entity_fields: &Vec<EntityField>,
+    encoder_state: &mut HashMap<usize, EncoderStateValue>,
+    naive_datetime_to_utc: bool,
+) -> PyResult<Vec<Field>> {
+    let mut fields = vec![];
+    for field in entity_fields {
+        let f_name = field.name.downcast_bound::<PyString>(py)?;
+        let dict_key = field.dict_key.downcast_bound::<PyString>(py)?;
+        let f_type = get_object_type(field.field_type.bind(py))?;
+
+        let fld = Field {
+            name: f_name.clone().unbind(),
+            dict_key: dict_key.clone().unbind(),
+            dict_key_rs: dict_key.to_string_lossy().into(),
+            encoder: get_encoder(py, f_type, encoder_state, naive_datetime_to_utc)?,
+            required: field.required,
+            default: field.default.clone().into(),
+            default_factory: field.default_factory.clone().into(),
+        };
+        fields.push(fld);
+    }
+    Ok(fields)
+}
```

### Comparing `serpyco_rs-1.7.1/src/validator/errors.rs` & `serpyco_rs-1.8.0/src/validator/errors.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-use pyo3::types::PyType;
-use pyo3::{PyErr, PyResult, Python};
-
-use crate::errors::ErrorItem;
-use crate::errors::SchemaValidationError;
-use crate::validator::context::PathChunk;
-use crate::validator::InstancePath;
-
-pub fn raise_error<T: Into<String>>(error: T, instance_path: &InstancePath) -> PyResult<()> {
-    Python::with_gil(|py| {
-        let errors: Vec<ErrorItem> = vec![into_err_item(error, instance_path)];
-
-        let pyerror_type = PyType::new_bound::<SchemaValidationError>(py);
-        Err(PyErr::from_type_bound(
-            pyerror_type,
-            ("Schema validation failed".to_string(), errors),
-        ))
-    })
-}
-
-fn into_err_item<T: Into<String>>(error: T, instance_path: &InstancePath) -> ErrorItem {
-    let instance_path = into_path(instance_path);
-    ErrorItem::new(error.into(), instance_path)
-}
-
-fn into_path(pointer: &InstancePath) -> String {
-    let mut path = vec![];
-    for chunk in pointer.to_vec() {
-        match chunk {
-            PathChunk::Property(property) => {
-                path.push(property.to_string());
-            }
-            PathChunk::Index(index) => path.push(index.to_string()),
-            PathChunk::PropertyValue(value) => path.push(value.to_string()),
-        };
-    }
-    path.join("/")
-}
+use pyo3::types::PyType;
+use pyo3::{PyErr, PyResult, Python};
+
+use crate::errors::ErrorItem;
+use crate::errors::SchemaValidationError;
+use crate::validator::context::PathChunk;
+use crate::validator::InstancePath;
+
+pub fn raise_error<T: Into<String>>(error: T, instance_path: &InstancePath) -> PyResult<()> {
+    Python::with_gil(|py| {
+        let errors: Vec<ErrorItem> = vec![into_err_item(error, instance_path)];
+
+        let pyerror_type = PyType::new_bound::<SchemaValidationError>(py);
+        Err(PyErr::from_type_bound(
+            pyerror_type,
+            ("Schema validation failed".to_string(), errors),
+        ))
+    })
+}
+
+fn into_err_item<T: Into<String>>(error: T, instance_path: &InstancePath) -> ErrorItem {
+    let instance_path = into_path(instance_path);
+    ErrorItem::new(error.into(), instance_path)
+}
+
+fn into_path(pointer: &InstancePath) -> String {
+    let mut path = vec![];
+    for chunk in pointer.to_vec() {
+        match chunk {
+            PathChunk::Property(property) => {
+                path.push(property.to_string());
+            }
+            PathChunk::Index(index) => path.push(index.to_string()),
+            PathChunk::PropertyValue(value) => path.push(value.to_string()),
+        };
+    }
+    path.join("/")
+}
+
+pub fn map_py_err_to_schema_validation_error(
+    py: Python<'_>,
+    error: PyErr,
+    instance_path: &InstancePath,
+) -> PyErr {
+    let error_message = format!("{}", &error);
+    let instance_path = into_path(instance_path);
+    let err = PyErr::new::<SchemaValidationError, _>((
+        "Schema validation failed".to_string(),
+        vec![ErrorItem::new(error_message, instance_path)],
+    ));
+    err.set_cause(py, Some(error));
+    err
+}
```

### Comparing `serpyco_rs-1.7.1/src/validator/validators.rs` & `serpyco_rs-1.8.0/src/validator/validators.rs`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-use crate::validator::types::EnumItems;
-use crate::validator::{raise_error, InstancePath};
-
-use pyo3::prelude::PyAnyMethods;
-use pyo3::types::{PySequence, PyString};
-use pyo3::{Bound, PyAny, PyErr, PyResult};
-use std::cmp::Ordering;
-use std::fmt::Display;
-
-pub fn check_lower_bound<T>(val: T, min: Option<T>, instance_path: &InstancePath) -> PyResult<()>
-where
-    T: PartialOrd + Display,
-{
-    if let Some(min) = min {
-        if val <= min {
-            raise_error(
-                format!("{} is less than the minimum of {}", val, min),
-                instance_path,
-            )?;
-        }
-    }
-    Ok(())
-}
-
-pub fn check_upper_bound<T>(val: T, max: Option<T>, instance_path: &InstancePath) -> PyResult<()>
-where
-    T: PartialOrd + Display,
-{
-    if let Some(max) = max {
-        if val > max {
-            raise_error(
-                format!("{} is greater than the maximum of {}", val, max),
-                instance_path,
-            )?;
-        }
-    }
-    Ok(())
-}
-
-pub fn _check_bounds<T>(
-    val: T,
-    min: Option<T>,
-    max: Option<T>,
-    instance_path: &InstancePath,
-) -> PyResult<()>
-where
-    T: PartialOrd + Display + Copy,
-{
-    if min.is_none() && max.is_none() {
-        return Ok(());
-    }
-    check_lower_bound(val, min, instance_path)?;
-    check_upper_bound(val, max, instance_path)?;
-    Ok(())
-}
-
-macro_rules! check_bounds {
-    ($val: expr, $type_info: expr, $path: expr) => {
-        crate::validator::validators::_check_bounds($val, $type_info.min, $type_info.max, $path)
-    };
-}
-
-pub fn check_min_length(
-    val: &Bound<'_, PyString>,
-    len: usize,
-    min: Option<usize>,
-    instance_path: &InstancePath,
-) -> PyResult<()> {
-    if let Some(min) = min {
-        if len <= min {
-            raise_error(
-                format!(r#""{}" is shorter than {} characters"#, val, min),
-                instance_path,
-            )?;
-        }
-    }
-    Ok(())
-}
-
-pub fn check_max_length(
-    val: &Bound<'_, PyString>,
-    len: usize,
-    max: Option<usize>,
-    instance_path: &InstancePath,
-) -> PyResult<()> {
-    if let Some(max) = max {
-        if len > max {
-            raise_error(
-                format!(r#""{}" is longer than {} characters"#, val, max),
-                instance_path,
-            )?;
-        }
-    }
-    Ok(())
-}
-
-pub fn check_length(
-    val: &Bound<'_, PyString>,
-    min: Option<usize>,
-    max: Option<usize>,
-    instance_path: &InstancePath,
-) -> PyResult<()> {
-    if min.is_none() && max.is_none() {
-        return Ok(());
-    }
-    let len = val.len()?;
-    check_min_length(val, len, min, instance_path)?;
-    check_max_length(val, len, max, instance_path)?;
-    Ok(())
-}
-
-#[cold]
-pub fn missing_required_property(property: &str, instance_path: &InstancePath) -> PyErr {
-    let instance_path = instance_path.push(property);
-    raise_error(
-        format!(r#""{}" is a required property"#, property),
-        &instance_path,
-    )
-    .unwrap_err()
-}
-
-pub fn check_sequence_size(
-    val: &Bound<'_, PySequence>,
-    seq_len: usize,
-    size: usize,
-    instance_path: Option<&InstancePath>,
-) -> PyResult<()> {
-    match seq_len.cmp(&size) {
-        Ordering::Equal => Ok(()),
-        Ordering::Less => {
-            let instance_path = instance_path.cloned().unwrap_or(InstancePath::new());
-            raise_error(
-                format!(r#"{} has less than {} items"#, val, size),
-                &instance_path,
-            )
-        }
-        Ordering::Greater => {
-            let instance_path = instance_path.cloned().unwrap_or(InstancePath::new());
-            raise_error(
-                format!(r#"{} has more than {} items"#, val, size),
-                &instance_path,
-            )
-        }
-    }
-}
-
-pub fn no_encoder_for_discriminator(
-    key: &str,
-    discriminators: &[String],
-    instance_path: &InstancePath,
-) -> PyErr {
-    let items = discriminators
-        .iter()
-        .map(|s| format!(r#""{}""#, s))
-        .collect::<Vec<_>>()
-        .join(", ");
-    raise_error(
-        format!(
-            r#""{}" is not one of [{}] discriminator values"#,
-            key, items
-        ),
-        instance_path,
-    )
-    .unwrap_err()
-}
-
-pub fn _invalid_type_new(
-    type_: &str,
-    value: &Bound<'_, PyAny>,
-    instance_path: &InstancePath,
-) -> PyResult<()> {
-    let error = match value.is_instance_of::<PyString>() {
-        true => format!(r#""{}" is not of type "{}""#, value, type_),
-        false => format!(r#"{} is not of type "{}""#, value, type_),
-    };
-    raise_error(error, instance_path)?;
-    Ok(())
-}
-
-macro_rules! invalid_type {
-    ($type_: expr, $value: expr, $path: expr) => {{
-        crate::validator::validators::_invalid_type_new($type_, $value, $path)?;
-        unreachable!(); // todo: Discard the use of unreachable
-    }};
-}
-
-macro_rules! invalid_type_dump {
-    ($type_: expr, $value: expr) => {{
-        let error = format!(r#""{}" is not of type "{}""#, $value.to_string(), $type_);
-        let instance_path = InstancePath::new();
-        crate::validator::raise_error(error, &instance_path)?;
-        unreachable!(); // todo: Discard the use of unreachable
-    }};
-}
-
-pub fn _invalid_enum_item(
-    items: EnumItems,
-    value: &Bound<'_, PyAny>,
-    instance_path: &InstancePath,
-) -> PyResult<()> {
-    let error = match value.is_instance_of::<PyString>() {
-        true => format!(r#""{}" is not one of {}"#, value, items),
-        false => format!(r#"{} is not one of {}"#, value, items),
-    };
-
-    raise_error(error, instance_path)?;
-    Ok(())
-}
-
-macro_rules! invalid_enum_item {
-    ($items: expr, $value: expr, $path: expr) => {{
-        crate::validator::validators::_invalid_enum_item($items, $value, $path)?;
-        unreachable!(); // todo: Discard the use of unreachable
-    }};
-}
-
-pub fn str_as_bool(str: &str) -> Option<bool> {
-    match str.as_bytes() {
-        [b't'] | [b'T'] | b"true" | b"True" | b"TRUE" => Some(true),
-        [b'f'] | [b'F'] | b"false" | b"False" | b"FALSE" => Some(false),
-        _ => None,
-    }
-}
-
-pub(crate) use check_bounds;
-pub(crate) use invalid_enum_item;
-pub(crate) use invalid_type;
-pub(crate) use invalid_type_dump;
+use crate::validator::types::EnumItems;
+use crate::validator::{raise_error, InstancePath};
+
+use pyo3::prelude::PyAnyMethods;
+use pyo3::types::{PySequence, PyString};
+use pyo3::{Bound, PyAny, PyErr, PyResult};
+use std::cmp::Ordering;
+use std::fmt::Display;
+
+pub fn check_lower_bound<T>(val: T, min: Option<T>, instance_path: &InstancePath) -> PyResult<()>
+where
+    T: PartialOrd + Display,
+{
+    if let Some(min) = min {
+        if val <= min {
+            raise_error(
+                format!("{} is less than the minimum of {}", val, min),
+                instance_path,
+            )?;
+        }
+    }
+    Ok(())
+}
+
+pub fn check_upper_bound<T>(val: T, max: Option<T>, instance_path: &InstancePath) -> PyResult<()>
+where
+    T: PartialOrd + Display,
+{
+    if let Some(max) = max {
+        if val > max {
+            raise_error(
+                format!("{} is greater than the maximum of {}", val, max),
+                instance_path,
+            )?;
+        }
+    }
+    Ok(())
+}
+
+pub fn _check_bounds<T>(
+    val: T,
+    min: Option<T>,
+    max: Option<T>,
+    instance_path: &InstancePath,
+) -> PyResult<()>
+where
+    T: PartialOrd + Display + Copy,
+{
+    if min.is_none() && max.is_none() {
+        return Ok(());
+    }
+    check_lower_bound(val, min, instance_path)?;
+    check_upper_bound(val, max, instance_path)?;
+    Ok(())
+}
+
+macro_rules! check_bounds {
+    ($val: expr, $type_info: expr, $path: expr) => {
+        crate::validator::validators::_check_bounds($val, $type_info.min, $type_info.max, $path)
+    };
+}
+
+pub fn check_min_length(
+    val: &Bound<'_, PyString>,
+    len: usize,
+    min: Option<usize>,
+    instance_path: &InstancePath,
+) -> PyResult<()> {
+    if let Some(min) = min {
+        if len <= min {
+            raise_error(
+                format!(r#""{}" is shorter than {} characters"#, val, min),
+                instance_path,
+            )?;
+        }
+    }
+    Ok(())
+}
+
+pub fn check_max_length(
+    val: &Bound<'_, PyString>,
+    len: usize,
+    max: Option<usize>,
+    instance_path: &InstancePath,
+) -> PyResult<()> {
+    if let Some(max) = max {
+        if len > max {
+            raise_error(
+                format!(r#""{}" is longer than {} characters"#, val, max),
+                instance_path,
+            )?;
+        }
+    }
+    Ok(())
+}
+
+pub fn check_length(
+    val: &Bound<'_, PyString>,
+    min: Option<usize>,
+    max: Option<usize>,
+    instance_path: &InstancePath,
+) -> PyResult<()> {
+    if min.is_none() && max.is_none() {
+        return Ok(());
+    }
+    let len = val.len()?;
+    check_min_length(val, len, min, instance_path)?;
+    check_max_length(val, len, max, instance_path)?;
+    Ok(())
+}
+
+#[cold]
+pub fn missing_required_property(property: &str, instance_path: &InstancePath) -> PyErr {
+    let instance_path = instance_path.push(property);
+    raise_error(
+        format!(r#""{}" is a required property"#, property),
+        &instance_path,
+    )
+    .unwrap_err()
+}
+
+pub fn check_sequence_size(
+    val: &Bound<'_, PySequence>,
+    seq_len: usize,
+    size: usize,
+    instance_path: Option<&InstancePath>,
+) -> PyResult<()> {
+    match seq_len.cmp(&size) {
+        Ordering::Equal => Ok(()),
+        Ordering::Less => {
+            let instance_path = instance_path.cloned().unwrap_or(InstancePath::new());
+            raise_error(
+                format!(r#"{} has less than {} items"#, val, size),
+                &instance_path,
+            )
+        }
+        Ordering::Greater => {
+            let instance_path = instance_path.cloned().unwrap_or(InstancePath::new());
+            raise_error(
+                format!(r#"{} has more than {} items"#, val, size),
+                &instance_path,
+            )
+        }
+    }
+}
+
+pub fn no_encoder_for_discriminator(
+    key: &str,
+    discriminators: &[String],
+    instance_path: &InstancePath,
+) -> PyErr {
+    let items = discriminators
+        .iter()
+        .map(|s| format!(r#""{}""#, s))
+        .collect::<Vec<_>>()
+        .join(", ");
+    raise_error(
+        format!(
+            r#""{}" is not one of [{}] discriminator values"#,
+            key, items
+        ),
+        instance_path,
+    )
+    .unwrap_err()
+}
+
+pub fn _invalid_type_new(
+    type_: &str,
+    value: &Bound<'_, PyAny>,
+    instance_path: &InstancePath,
+) -> PyResult<()> {
+    let error = match value.is_instance_of::<PyString>() {
+        true => format!(r#""{}" is not of type "{}""#, value, type_),
+        false => format!(r#"{} is not of type "{}""#, value, type_),
+    };
+    raise_error(error, instance_path)?;
+    Ok(())
+}
+
+macro_rules! invalid_type {
+    ($type_: expr, $value: expr, $path: expr) => {{
+        crate::validator::validators::_invalid_type_new($type_, $value, $path)?;
+        unreachable!(); // todo: Discard the use of unreachable
+    }};
+}
+
+macro_rules! invalid_type_dump {
+    ($type_: expr, $value: expr) => {{
+        let error = format!(r#""{}" is not of type "{}""#, $value.to_string(), $type_);
+        let instance_path = InstancePath::new();
+        crate::validator::raise_error(error, &instance_path)?;
+        unreachable!(); // todo: Discard the use of unreachable
+    }};
+}
+
+pub fn _invalid_enum_item(
+    items: EnumItems,
+    value: &Bound<'_, PyAny>,
+    instance_path: &InstancePath,
+) -> PyResult<()> {
+    let error = match value.is_instance_of::<PyString>() {
+        true => format!(r#""{}" is not one of {}"#, value, items),
+        false => format!(r#"{} is not one of {}"#, value, items),
+    };
+
+    raise_error(error, instance_path)?;
+    Ok(())
+}
+
+macro_rules! invalid_enum_item {
+    ($items: expr, $value: expr, $path: expr) => {{
+        crate::validator::validators::_invalid_enum_item($items, $value, $path)?;
+        unreachable!(); // todo: Discard the use of unreachable
+    }};
+}
+
+pub fn str_as_bool(str: &str) -> Option<bool> {
+    match str.as_bytes() {
+        [b't'] | [b'T'] | b"true" | b"True" | b"TRUE" => Some(true),
+        [b'f'] | [b'F'] | b"false" | b"False" | b"FALSE" => Some(false),
+        _ => None,
+    }
+}
+
+pub(crate) use check_bounds;
+pub(crate) use invalid_enum_item;
+pub(crate) use invalid_type;
+pub(crate) use invalid_type_dump;
```

### Comparing `serpyco_rs-1.7.1/tests/json_schema/test_convert.py` & `serpyco_rs-1.8.0/tests/json_schema/test_convert.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,478 +1,478 @@
-import sys
-from dataclasses import dataclass
-from datetime import datetime, time
-from decimal import Decimal
-from enum import Enum
-from typing import Annotated, Any, Literal, Optional, TypedDict, Union
-from uuid import UUID
-
-import pytest
-from serpyco_rs import Serializer, JsonSchemaBuilder
-from serpyco_rs.metadata import Alias, CamelCase, Discriminator, Max, MaxLength, Min, MinLength, OmitNone
-
-
-def test_to_json_schema():
-    class EnumCls(Enum):
-        a = 'a'
-
-    @dataclass
-    class InnerData:
-        """Some important entity"""
-
-        foo_filed: str
-
-    @dataclass
-    class OtherInnerData:
-        """OtherInnerData"""
-
-        optional_filed: Optional[InnerData] = None
-
-    class AnotherInnerData(TypedDict):
-        """AnotherInnerData"""
-
-        bar: str
-
-    @dataclass
-    class Data:
-        """Docs"""
-
-        a: Annotated[int, Min(0), Max(10)]
-        """A field with bounds"""
-        b: float
-        c: Decimal
-        d: bool
-        e: Annotated[str, MinLength(1), MaxLength(5)]
-        f: UUID
-        g: time
-        h: datetime
-        i: EnumCls
-        j: InnerData
-        k: list[int]
-        l: tuple[int, str, InnerData]
-        m: dict[str, int]
-        n: Any
-        o: Annotated[InnerData, CamelCase]
-        p: Annotated[OtherInnerData, OmitNone]
-        q: AnotherInnerData
-        some_filed: Annotated[str, Alias('fooFiled')]
-
-    serializer = Serializer(Data)
-
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.Data[no_format,keep_nones]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.Data[no_format,keep_nones]': {
-                    'description': 'Docs',
-                    'properties': {
-                        'a': {
-                            'description': 'A field with bounds',
-                            'maximum': 10,
-                            'minimum': 0,
-                            'type': 'integer',
-                        },
-                        'b': {'type': 'number'},
-                        'c': {
-                            'oneOf': [{'type': 'string', 'format': 'decimal'}, {'type': 'number', 'format': 'decimal'}]
-                        },
-                        'd': {'type': 'boolean'},
-                        'e': {'maxLength': 5, 'minLength': 1, 'type': 'string'},
-                        'f': {'format': 'uuid', 'type': 'string'},
-                        'g': {
-                            'format': 'time',
-                            'type': 'string',
-                        },
-                        'h': {
-                            'format': 'date-time',
-                            'type': 'string',
-                        },
-                        'i': {'enum': ['a'], 'type': 'string'},
-                        'j': {
-                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]'
-                        },
-                        'k': {'items': {'type': 'integer'}, 'type': 'array'},
-                        'l': {
-                            'maxItems': 3,
-                            'minItems': 3,
-                            'prefixItems': [
-                                {'type': 'integer'},
-                                {'type': 'string'},
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]'
-                                },
-                            ],
-                            'type': 'array',
-                        },
-                        'm': {'additionalProperties': {'type': 'integer'}, 'type': 'object'},
-                        'n': {},
-                        'p': {
-                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.OtherInnerData[no_format,omit_nones]'
-                        },
-                        'o': {
-                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[camel_case,keep_nones]'
-                        },
-                        'q': {
-                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.AnotherInnerData[no_format,keep_nones]'
-                        },
-                        'fooFiled': {'type': 'string'},
-                    },
-                    'required': [
-                        'a',
-                        'b',
-                        'c',
-                        'd',
-                        'e',
-                        'f',
-                        'g',
-                        'h',
-                        'i',
-                        'j',
-                        'k',
-                        'l',
-                        'm',
-                        'n',
-                        'o',
-                        'p',
-                        'q',
-                        'fooFiled',
-                    ],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]': {
-                    'description': 'Some important entity',
-                    'properties': {'foo_filed': {'type': 'string'}},
-                    'required': ['foo_filed'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,omit_nones]': {
-                    'description': 'Some important entity',
-                    'properties': {'foo_filed': {'type': 'string'}},
-                    'required': ['foo_filed'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[camel_case,keep_nones]': {
-                    'description': 'Some important entity',
-                    'properties': {'fooFiled': {'type': 'string'}},
-                    'required': ['fooFiled'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.OtherInnerData[no_format,omit_nones]': {
-                    'description': 'OtherInnerData',
-                    'properties': {
-                        'optional_filed': {
-                            'anyOf': [
-                                {'type': 'null'},
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,omit_nones]'
-                                },
-                            ]
-                        }
-                    },
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema.<locals>.AnotherInnerData[no_format,keep_nones]': {
-                    'description': 'AnotherInnerData',
-                    'properties': {'bar': {'type': 'string'}},
-                    'required': ['bar'],
-                    'type': 'object',
-                },
-            },
-        },
-    }
-
-
-@pytest.mark.skipif(sys.version_info < (3, 10), reason='New style unions available after 3.10')
-def test_to_json_schema__new_union_syntax():
-    @dataclass
-    class Data:
-        """Docs"""
-
-        a: int | None
-
-    serializer = Serializer(Data)
-
-    assert serializer.get_json_schema() == {
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__new_union_syntax.<locals>.Data[no_format,keep_nones]',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema__new_union_syntax.<locals>.Data[no_format,keep_nones]': {
-                    'description': 'Docs',
-                    'properties': {'a': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]}},
-                    'required': ['a'],
-                    'type': 'object',
-                }
-            },
-        },
-    }
-
-
-@dataclass
-class TreeNode:
-    """Node"""
-
-    data: str
-    left: Optional['TreeNode'] = None
-    right: Optional['TreeNode'] = None
-
-
-def test_to_json_schema__recursive_type():
-    serializer = Serializer(TreeNode)
-
-    assert serializer.get_json_schema() == {
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.TreeNode[no_format,keep_nones]': {
-                    'description': 'Node',
-                    'properties': {
-                        'data': {'type': 'string'},
-                        'left': {
-                            'anyOf': [
-                                {'type': 'null'},
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]'
-                                },
-                            ]
-                        },
-                        'right': {
-                            'anyOf': [
-                                {'type': 'null'},
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]'
-                                },
-                            ]
-                        },
-                    },
-                    'required': ['data'],
-                    'type': 'object',
-                }
-            }
-        },
-    }
-
-
-def test_to_json_schema__literal():
-    serializer = Serializer(Literal['foo'])
-    assert serializer.get_json_schema() == {
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'enum': ['foo'],
-    }
-
-
-def test_to_json_schema__tagged_union():
-    @dataclass
-    class Foo:
-        val: int
-        type: Literal['foo']
-
-    @dataclass
-    class Bar:
-        val: str
-        type: Literal['bar'] = 'bar'
-
-    @dataclass
-    class Base:
-        field: Annotated[Union[Foo, Bar], Discriminator('type')]
-
-    serializer = Serializer(Base)
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Base[no_format,keep_nones]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]': {
-                    'properties': {'type': {'enum': ['bar']}, 'val': {'type': 'string'}},
-                    'required': ['val', 'type'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Base[no_format,keep_nones]': {
-                    'properties': {
-                        'field': {
-                            'discriminator': {
-                                'mapping': {
-                                    'bar': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]',
-                                    'foo': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]',
-                                },
-                                'propertyName': 'type',
-                            },
-                            'oneOf': [
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]'
-                                },
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]'
-                                },
-                            ],
-                        }
-                    },
-                    'required': ['field'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]': {
-                    'properties': {'type': {'enum': ['foo']}, 'val': {'type': 'integer'}},
-                    'required': ['val', 'type'],
-                    'type': 'object',
-                },
-            }
-        },
-    }
-
-
-def test_to_json_schema__union():
-    @dataclass
-    class Foo:
-        val: int
-
-    @dataclass
-    class Bar:
-        val: str
-
-    @dataclass
-    class Base:
-        field: Union[Foo, Bar, str]
-
-    serializer = Serializer(Base)
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Base[no_format,keep_nones]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Bar[no_format,keep_nones]': {
-                    'properties': {'val': {'type': 'string'}},
-                    'required': ['val'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Base[no_format,keep_nones]': {
-                    'properties': {
-                        'field': {
-                            'oneOf': [
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Foo[no_format,keep_nones]'
-                                },
-                                {
-                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Bar[no_format,keep_nones]'
-                                },
-                                {'type': 'string'},
-                            ],
-                        }
-                    },
-                    'required': ['field'],
-                    'type': 'object',
-                },
-                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Foo[no_format,keep_nones]': {
-                    'properties': {'val': {'type': 'integer'}},
-                    'required': ['val'],
-                    'type': 'object',
-                },
-            }
-        },
-    }
-
-
-def test_to_json_schema__force_none_as_default_for_optional():
-    @dataclass
-    class Data:
-        a: Optional[int]
-
-    serializer = Serializer(Data, force_default_for_optional=True)
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__force_none_as_default_for_optional.<locals>.Data[no_format,keep_nones,force_none]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema__force_none_as_default_for_optional.<locals>.Data[no_format,keep_nones,force_none]': {
-                    'properties': {'a': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]}},
-                    'type': 'object',
-                }
-            }
-        },
-    }
-
-
-def test_to_json_schema__bytes():
-    @dataclass
-    class Data:
-        a: bytes
-
-    serializer = Serializer(Data)
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__bytes.<locals>.Data[no_format,keep_nones]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.json_schema.test_convert.test_to_json_schema__bytes.<locals>.Data[no_format,keep_nones]': {
-                    'properties': {'a': {'type': 'string', 'format': 'binary'}},
-                    'type': 'object',
-                    'required': ['a'],
-                }
-            }
-        },
-    }
-
-
-def test_enum_x_attrs():
-    class EnumCls(Enum):
-        a = 'a'
-        """a docstring"""
-
-    serializer = Serializer(EnumCls)
-    assert serializer.get_json_schema() == {
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'enum': ['a'],
-        'type': 'string',
-        'x-a': 'a docstring',
-    }
-
-
-def test_enum_multiply_types():
-    class EnumCls(Enum):
-        a = 'a'
-        """a docstring"""
-        b = 1
-        """b docstring"""
-
-    serializer = Serializer(EnumCls)
-    assert serializer.get_json_schema() == {
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'enum': ['a', 1],
-        'x-a': 'a docstring',
-        'x-1': 'b docstring',
-    }
-
-
-class TestJsonSchemaBuilder:
-    def test_build__use_custom_ref_prefix(self):
-        @dataclass
-        class Data:
-            a: int
-
-        serializer = Serializer(Data)
-        schema_builder = JsonSchemaBuilder(ref_prefix='#/foo/bar')
-        schema = schema_builder.build(serializer)
-        definitions = schema_builder.get_definitions()
-
-        assert schema == {
-            '$ref': '#/foo/bar/tests.json_schema.test_convert.TestJsonSchemaBuilder.test_build__use_custom_ref_prefix.<locals>.Data[no_format,keep_nones]',
-        }
-
-        assert definitions == {
-            'tests.json_schema.test_convert.TestJsonSchemaBuilder.test_build__use_custom_ref_prefix.<locals>.Data[no_format,keep_nones]': {
-                'properties': {'a': {'type': 'integer'}},
-                'required': ['a'],
-                'type': 'object',
-            }
-        }
-
-    def test_build__add_dialect_uri(self):
-        serializer = Serializer(int)
-        schema_builder = JsonSchemaBuilder(add_dialect_uri=True)
-        schema = schema_builder.build(serializer)
-
-        assert schema == {
-            'type': 'integer',
-            '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        }
-        assert schema_builder.get_definitions() == {}
+import sys
+from dataclasses import dataclass
+from datetime import datetime, time
+from decimal import Decimal
+from enum import Enum
+from typing import Annotated, Any, Literal, Optional, TypedDict, Union
+from uuid import UUID
+
+import pytest
+from serpyco_rs import Serializer, JsonSchemaBuilder
+from serpyco_rs.metadata import Alias, CamelCase, Discriminator, Max, MaxLength, Min, MinLength, OmitNone
+
+
+def test_to_json_schema():
+    class EnumCls(Enum):
+        a = 'a'
+
+    @dataclass
+    class InnerData:
+        """Some important entity"""
+
+        foo_filed: str
+
+    @dataclass
+    class OtherInnerData:
+        """OtherInnerData"""
+
+        optional_filed: Optional[InnerData] = None
+
+    class AnotherInnerData(TypedDict):
+        """AnotherInnerData"""
+
+        bar: str
+
+    @dataclass
+    class Data:
+        """Docs"""
+
+        a: Annotated[int, Min(0), Max(10)]
+        """A field with bounds"""
+        b: float
+        c: Decimal
+        d: bool
+        e: Annotated[str, MinLength(1), MaxLength(5)]
+        f: UUID
+        g: time
+        h: datetime
+        i: EnumCls
+        j: InnerData
+        k: list[int]
+        l: tuple[int, str, InnerData]
+        m: dict[str, int]
+        n: Any
+        o: Annotated[InnerData, CamelCase]
+        p: Annotated[OtherInnerData, OmitNone]
+        q: AnotherInnerData
+        some_filed: Annotated[str, Alias('fooFiled')]
+
+    serializer = Serializer(Data)
+
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.Data[no_format,keep_nones]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.Data[no_format,keep_nones]': {
+                    'description': 'Docs',
+                    'properties': {
+                        'a': {
+                            'description': 'A field with bounds',
+                            'maximum': 10,
+                            'minimum': 0,
+                            'type': 'integer',
+                        },
+                        'b': {'type': 'number'},
+                        'c': {
+                            'oneOf': [{'type': 'string', 'format': 'decimal'}, {'type': 'number', 'format': 'decimal'}]
+                        },
+                        'd': {'type': 'boolean'},
+                        'e': {'maxLength': 5, 'minLength': 1, 'type': 'string'},
+                        'f': {'format': 'uuid', 'type': 'string'},
+                        'g': {
+                            'format': 'time',
+                            'type': 'string',
+                        },
+                        'h': {
+                            'format': 'date-time',
+                            'type': 'string',
+                        },
+                        'i': {'enum': ['a'], 'type': 'string'},
+                        'j': {
+                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]'
+                        },
+                        'k': {'items': {'type': 'integer'}, 'type': 'array'},
+                        'l': {
+                            'maxItems': 3,
+                            'minItems': 3,
+                            'prefixItems': [
+                                {'type': 'integer'},
+                                {'type': 'string'},
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]'
+                                },
+                            ],
+                            'type': 'array',
+                        },
+                        'm': {'additionalProperties': {'type': 'integer'}, 'type': 'object'},
+                        'n': {},
+                        'p': {
+                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.OtherInnerData[no_format,omit_nones]'
+                        },
+                        'o': {
+                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[camel_case,keep_nones]'
+                        },
+                        'q': {
+                            '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.AnotherInnerData[no_format,keep_nones]'
+                        },
+                        'fooFiled': {'type': 'string'},
+                    },
+                    'required': [
+                        'a',
+                        'b',
+                        'c',
+                        'd',
+                        'e',
+                        'f',
+                        'g',
+                        'h',
+                        'i',
+                        'j',
+                        'k',
+                        'l',
+                        'm',
+                        'n',
+                        'o',
+                        'p',
+                        'q',
+                        'fooFiled',
+                    ],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,keep_nones]': {
+                    'description': 'Some important entity',
+                    'properties': {'foo_filed': {'type': 'string'}},
+                    'required': ['foo_filed'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,omit_nones]': {
+                    'description': 'Some important entity',
+                    'properties': {'foo_filed': {'type': 'string'}},
+                    'required': ['foo_filed'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[camel_case,keep_nones]': {
+                    'description': 'Some important entity',
+                    'properties': {'fooFiled': {'type': 'string'}},
+                    'required': ['fooFiled'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.OtherInnerData[no_format,omit_nones]': {
+                    'description': 'OtherInnerData',
+                    'properties': {
+                        'optional_filed': {
+                            'anyOf': [
+                                {'type': 'null'},
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema.<locals>.InnerData[no_format,omit_nones]'
+                                },
+                            ]
+                        }
+                    },
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema.<locals>.AnotherInnerData[no_format,keep_nones]': {
+                    'description': 'AnotherInnerData',
+                    'properties': {'bar': {'type': 'string'}},
+                    'required': ['bar'],
+                    'type': 'object',
+                },
+            },
+        },
+    }
+
+
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='New style unions available after 3.10')
+def test_to_json_schema__new_union_syntax():
+    @dataclass
+    class Data:
+        """Docs"""
+
+        a: int | None
+
+    serializer = Serializer(Data)
+
+    assert serializer.get_json_schema() == {
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__new_union_syntax.<locals>.Data[no_format,keep_nones]',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema__new_union_syntax.<locals>.Data[no_format,keep_nones]': {
+                    'description': 'Docs',
+                    'properties': {'a': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]}},
+                    'required': ['a'],
+                    'type': 'object',
+                }
+            },
+        },
+    }
+
+
+@dataclass
+class TreeNode:
+    """Node"""
+
+    data: str
+    left: Optional['TreeNode'] = None
+    right: Optional['TreeNode'] = None
+
+
+def test_to_json_schema__recursive_type():
+    serializer = Serializer(TreeNode)
+
+    assert serializer.get_json_schema() == {
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.TreeNode[no_format,keep_nones]': {
+                    'description': 'Node',
+                    'properties': {
+                        'data': {'type': 'string'},
+                        'left': {
+                            'anyOf': [
+                                {'type': 'null'},
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]'
+                                },
+                            ]
+                        },
+                        'right': {
+                            'anyOf': [
+                                {'type': 'null'},
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.TreeNode[no_format,keep_nones]'
+                                },
+                            ]
+                        },
+                    },
+                    'required': ['data'],
+                    'type': 'object',
+                }
+            }
+        },
+    }
+
+
+def test_to_json_schema__literal():
+    serializer = Serializer(Literal['foo'])
+    assert serializer.get_json_schema() == {
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'enum': ['foo'],
+    }
+
+
+def test_to_json_schema__tagged_union():
+    @dataclass
+    class Foo:
+        val: int
+        type: Literal['foo']
+
+    @dataclass
+    class Bar:
+        val: str
+        type: Literal['bar'] = 'bar'
+
+    @dataclass
+    class Base:
+        field: Annotated[Union[Foo, Bar], Discriminator('type')]
+
+    serializer = Serializer(Base)
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Base[no_format,keep_nones]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]': {
+                    'properties': {'type': {'enum': ['bar']}, 'val': {'type': 'string'}},
+                    'required': ['val', 'type'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Base[no_format,keep_nones]': {
+                    'properties': {
+                        'field': {
+                            'discriminator': {
+                                'mapping': {
+                                    'bar': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]',
+                                    'foo': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]',
+                                },
+                                'propertyName': 'type',
+                            },
+                            'oneOf': [
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]'
+                                },
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Bar[no_format,keep_nones]'
+                                },
+                            ],
+                        }
+                    },
+                    'required': ['field'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema__tagged_union.<locals>.Foo[no_format,keep_nones]': {
+                    'properties': {'type': {'enum': ['foo']}, 'val': {'type': 'integer'}},
+                    'required': ['val', 'type'],
+                    'type': 'object',
+                },
+            }
+        },
+    }
+
+
+def test_to_json_schema__union():
+    @dataclass
+    class Foo:
+        val: int
+
+    @dataclass
+    class Bar:
+        val: str
+
+    @dataclass
+    class Base:
+        field: Union[Foo, Bar, str]
+
+    serializer = Serializer(Base)
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Base[no_format,keep_nones]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Bar[no_format,keep_nones]': {
+                    'properties': {'val': {'type': 'string'}},
+                    'required': ['val'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Base[no_format,keep_nones]': {
+                    'properties': {
+                        'field': {
+                            'oneOf': [
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Foo[no_format,keep_nones]'
+                                },
+                                {
+                                    '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Bar[no_format,keep_nones]'
+                                },
+                                {'type': 'string'},
+                            ],
+                        }
+                    },
+                    'required': ['field'],
+                    'type': 'object',
+                },
+                'tests.json_schema.test_convert.test_to_json_schema__union.<locals>.Foo[no_format,keep_nones]': {
+                    'properties': {'val': {'type': 'integer'}},
+                    'required': ['val'],
+                    'type': 'object',
+                },
+            }
+        },
+    }
+
+
+def test_to_json_schema__force_none_as_default_for_optional():
+    @dataclass
+    class Data:
+        a: Optional[int]
+
+    serializer = Serializer(Data, force_default_for_optional=True)
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__force_none_as_default_for_optional.<locals>.Data[no_format,keep_nones,force_none]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema__force_none_as_default_for_optional.<locals>.Data[no_format,keep_nones,force_none]': {
+                    'properties': {'a': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]}},
+                    'type': 'object',
+                }
+            }
+        },
+    }
+
+
+def test_to_json_schema__bytes():
+    @dataclass
+    class Data:
+        a: bytes
+
+    serializer = Serializer(Data)
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.json_schema.test_convert.test_to_json_schema__bytes.<locals>.Data[no_format,keep_nones]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.json_schema.test_convert.test_to_json_schema__bytes.<locals>.Data[no_format,keep_nones]': {
+                    'properties': {'a': {'type': 'string', 'format': 'binary'}},
+                    'type': 'object',
+                    'required': ['a'],
+                }
+            }
+        },
+    }
+
+
+def test_enum_x_attrs():
+    class EnumCls(Enum):
+        a = 'a'
+        """a docstring"""
+
+    serializer = Serializer(EnumCls)
+    assert serializer.get_json_schema() == {
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'enum': ['a'],
+        'type': 'string',
+        'x-a': 'a docstring',
+    }
+
+
+def test_enum_multiply_types():
+    class EnumCls(Enum):
+        a = 'a'
+        """a docstring"""
+        b = 1
+        """b docstring"""
+
+    serializer = Serializer(EnumCls)
+    assert serializer.get_json_schema() == {
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'enum': ['a', 1],
+        'x-a': 'a docstring',
+        'x-1': 'b docstring',
+    }
+
+
+class TestJsonSchemaBuilder:
+    def test_build__use_custom_ref_prefix(self):
+        @dataclass
+        class Data:
+            a: int
+
+        serializer = Serializer(Data)
+        schema_builder = JsonSchemaBuilder(ref_prefix='#/foo/bar')
+        schema = schema_builder.build(serializer)
+        definitions = schema_builder.get_definitions()
+
+        assert schema == {
+            '$ref': '#/foo/bar/tests.json_schema.test_convert.TestJsonSchemaBuilder.test_build__use_custom_ref_prefix.<locals>.Data[no_format,keep_nones]',
+        }
+
+        assert definitions == {
+            'tests.json_schema.test_convert.TestJsonSchemaBuilder.test_build__use_custom_ref_prefix.<locals>.Data[no_format,keep_nones]': {
+                'properties': {'a': {'type': 'integer'}},
+                'required': ['a'],
+                'type': 'object',
+            }
+        }
+
+    def test_build__add_dialect_uri(self):
+        serializer = Serializer(int)
+        schema_builder = JsonSchemaBuilder(add_dialect_uri=True)
+        schema = schema_builder.build(serializer)
+
+        assert schema == {
+            'type': 'integer',
+            '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        }
+        assert schema_builder.get_definitions() == {}
```

### Comparing `serpyco_rs-1.7.1/tests/json_schema/test_validator.py` & `serpyco_rs-1.8.0/tests/json_schema/test_validator.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-import sys
-import textwrap
-import uuid
-from dataclasses import dataclass
-from datetime import date, datetime, time
-from decimal import Decimal
-from enum import Enum
-from typing import Annotated, Any, Callable, Literal, Optional, Union
-from unittest import mock
-
-import pytest
-from serpyco_rs import Serializer
-from serpyco_rs.exceptions import ErrorItem, SchemaValidationError, ValidationError
-from serpyco_rs.metadata import Discriminator, Max, MaxLength, Min, MinLength
-from typing_extensions import NotRequired, Required, TypedDict
-
-
-class EnumTest(Enum):
-    foo = 'foo'
-    bar = 'bar'
-
-
-@dataclass
-class EntityTest:
-    key: str
-
-
-@dataclass
-class Foo:
-    type: Literal['foo']
-    val: int
-
-
-@dataclass
-class Bar:
-    type: Literal['bar']
-    val: str
-
-
-class TypedDictTotalTrue(TypedDict):
-    foo: int
-    bar: NotRequired[str]
-
-
-class TypedDictTotalFalse(TypedDict, total=False):
-    foo: int
-    bar: Required[str]
-
-
-@pytest.mark.parametrize(
-    ['cls', 'value'],
-    (
-        (bool, True),
-        (bool, False),
-        (str, ''),
-        (Annotated[str, MinLength(1), MaxLength(3)], '12'),
-        (int, -99),
-        (Annotated[int, Min(1), Max(1000)], 99),
-        (float, 1.3),
-        (Annotated[float, Min(0), Max(0.4)], 0.1),
-        (Decimal, '0.1'),  # support str
-        (Decimal, 0.1),  # or int input
-        (Decimal, 'NaN'),  # or int input
-        (uuid.UUID, str(uuid.uuid4())),  # support only str input
-        (time, '12:34'),
-        (time, '12:34:56'),
-        (time, '12:34:56.000078'),
-        (time, '12:34Z'),
-        (time, '12:34+0300'),
-        (time, '12:34+03:00'),
-        (time, '12:34:00+03:00'),
-        (time, '12:34:56.000078+03:00'),
-        (time, '12:34:56.000078+00:00'),
-        (datetime, '2022-10-10T14:23:43'),
-        (datetime, '2022-10-10T14:23:43.123456'),
-        (datetime, '2022-10-10T14:23:43.123456Z'),
-        (datetime, '2022-10-10T14:23:43.123456+00:00'),
-        (datetime, '2022-10-10T14:23:43.123456-00:00'),
-        (date, '2020-07-17'),
-        (EnumTest, 'foo'),
-        (Optional[int], None),
-        (Optional[int], 1),
-        (EntityTest, {'key': 'val'}),
-        (list[int], [1, 2]),
-        (dict[str, int], {'a': 1}),
-        (tuple[str, int, bool], ['1', 2, True]),
-        (Annotated[Union[Foo, Bar], Discriminator('type')], {'type': 'foo', 'val': 1}),
-        (Annotated[Union[Foo, Bar], Discriminator('type')], {'type': 'bar', 'val': '1'}),
-        (Any, ['1', 2, True]),
-        (Any, {}),
-        (TypedDictTotalTrue, {'foo': 1}),
-        (TypedDictTotalTrue, {'foo': 1, 'bar': '1'}),
-        (TypedDictTotalFalse, {'bar': '1'}),
-        (TypedDictTotalFalse, {'foo': 1, 'bar': '1'}),
-    ),
-)
-def test_validate(cls, value):
-    Serializer(cls).load(value)
-
-
-if sys.version_info >= (3, 10):
-
-    @pytest.mark.parametrize(
-        ['cls', 'value'],
-        (
-            (Optional[int], None),
-            (int | None, None),
-            (int | None, 2),
-        ),
-    )
-    def test_validate_new_union(cls, value):
-        Serializer(cls).load(value)
-
-
-def _mk_e(m=mock.ANY, ip=mock.ANY) -> Callable[[ErrorItem], None]:
-    def cmp(e: ErrorItem) -> None:
-        assert e.message == m and e.instance_path == ip
-
-    return cmp
-
-
-@pytest.mark.parametrize(
-    ['cls', 'value', 'check'],
-    (
-        (bool, 1, _mk_e(m='1 is not of type "boolean"')),
-        (str, 1, _mk_e(m='1 is not of type "string"')),
-        (
-            Annotated[str, MinLength(2)],
-            'a',
-            _mk_e(m='"a" is shorter than 2 characters'),
-        ),
-        (
-            Annotated[str, MaxLength(2)],
-            'aaa',
-            _mk_e(m='"aaa" is longer than 2 characters'),
-        ),
-        (int, 9.1, _mk_e(m='9.1 is not of type "integer"')),
-        (int, '9', _mk_e(m='"9" is not of type "integer"')),
-        (
-            Annotated[int, Min(1)],
-            0,
-            _mk_e(m='0 is less than the minimum of 1'),
-        ),
-        (
-            Annotated[int, Max(1)],
-            10,
-            _mk_e(m='10 is greater than the maximum of 1'),
-        ),
-        (float, None, _mk_e(m='None is not of type "number"')),
-        (
-            Annotated[float, Min(1.1)],
-            0.1,
-            _mk_e(m='0.1 is less than the minimum of 1.1'),
-        ),
-        (
-            Annotated[float, Max(1.5)],
-            10.1,
-            _mk_e(m='10.1 is greater than the maximum of 1.5'),
-        ),
-        (uuid.UUID, 'asd', _mk_e(ip='')),
-        (time, '12:34:a', _mk_e(ip='')),
-        (datetime, '2022-10-10//12', _mk_e(ip='')),
-        (date, '17-02-2022', _mk_e(ip='')),
-        (datetime, '2022-10-10T14:23:43.123456-30:00', _mk_e(ip='')),
-        (EnumTest, 'buz', _mk_e(m='"buz" is not one of ["bar", "foo"]')),
-        (
-            Optional[int],
-            'foo',
-            _mk_e(m='"foo" is not of type "integer"'),
-        ),
-        (EntityTest, {}, _mk_e(m='"key" is a required property')),
-        (
-            list[int],
-            [1, '1'],
-            _mk_e(m='"1" is not of type "integer"', ip='1'),
-        ),
-        (
-            dict[str, int],
-            {'a': '1'},
-            _mk_e(m='"1" is not of type "integer"', ip='a'),
-        ),
-        (
-            tuple[str, int, bool],
-            ['1'],
-            _mk_e(m="['1'] has less than 3 items"),
-        ),
-        (
-            tuple[str, int, bool],
-            ['1', 1, True, 0],
-            _mk_e(m="['1', 1, True, 0] has more than 3 items"),
-        ),
-        (
-            tuple[str, bool],
-            ['1', 1],
-            _mk_e(
-                m='1 is not of type "boolean"',
-                ip='1',
-            ),
-        ),
-        (
-            Annotated[Union[Foo, Bar], Discriminator('type')],
-            {'type': 'buz'},
-            _mk_e(m='"buz" is not one of ["foo", "bar"] discriminator values'),
-        ),
-        (
-            Annotated[Union[Foo, Bar], Discriminator('type')],
-            {'type': 'foo', 'val': '123'},
-            _mk_e(ip='val', m='"123" is not of type "integer"'),
-        ),
-        (
-            Annotated[Union[Foo, Bar], Discriminator('type')],
-            {'type': 'bar', 'val': 1},
-            _mk_e(ip='val', m='1 is not of type "string"'),
-        ),
-        (TypedDictTotalTrue, {}, _mk_e(m='"foo" is a required property')),
-        (TypedDictTotalFalse, {}, _mk_e(m='"bar" is a required property')),
-    ),
-)
-def test_validate__validation_error(cls, value, check):
-    serializer = Serializer(cls)
-    with pytest.raises(SchemaValidationError) as exc_info:
-        serializer.load(value)
-
-    assert len(exc_info.value.errors) == 1
-    check(exc_info.value.errors[0])
-
-
-def test_validate__error_format():
-    @dataclass
-    class Inner:
-        baz: str
-
-    @dataclass
-    class A:
-        foo: int
-        bar: Inner
-
-    serializer = Serializer(A)
-
-    value = {'foo': '1', 'bar': {'buz': None}, 'qux': 0}
-
-    with pytest.raises(SchemaValidationError) as exc_info:
-        serializer.load(value)
-
-    assert exc_info.value.errors == [
-        ErrorItem(
-            message='"1" is not of type "integer"',
-            instance_path='foo',
-        ),
-    ]
-
-
-def test_validation_exceptions_inheritance():
-    serializer = Serializer(int)
-    with pytest.raises(SchemaValidationError) as exc_info:
-        serializer.load('1')
-
-    assert isinstance(exc_info.value, ValidationError)
-    assert exc_info.value.message == 'Schema validation failed'
-
-
-def test_validation_error_message():
-    @dataclass
-    class A:
-        foo: int
-        bar: str
-
-    serializer = Serializer(A)
-    with pytest.raises(SchemaValidationError) as exc_info:
-        serializer.load({'foo': '1', 'bar': 2})
-
-    error = exc_info.value
-    error_item = error.errors[0]
-
-    assert str(error_item) == (""""1" is not of type "integer" (instance_path='foo')""")
-    assert repr(error_item) == ("""ErrorItem(message='"1" is not of type "integer"', instance_path='foo')""")
-    assert str(error) == textwrap.dedent(
-        """\
-    Schema validation failed:
-    - "1" is not of type "integer" (instance_path='foo')
-      """
-    )
-    assert repr(error) == textwrap.dedent(
-        """\
-    SchemaValidationError(
-        message="Schema validation failed",
-        errors=[
-            ErrorItem(message='"1" is not of type "integer"', instance_path='foo'),
-        ]
-    )"""
-    )
+import sys
+import textwrap
+import uuid
+from dataclasses import dataclass
+from datetime import date, datetime, time
+from decimal import Decimal
+from enum import Enum
+from typing import Annotated, Any, Callable, Literal, Optional, Union
+from unittest import mock
+
+import pytest
+from serpyco_rs import Serializer
+from serpyco_rs.exceptions import ErrorItem, SchemaValidationError, ValidationError
+from serpyco_rs.metadata import Discriminator, Max, MaxLength, Min, MinLength
+from typing_extensions import NotRequired, Required, TypedDict
+
+
+class EnumTest(Enum):
+    foo = 'foo'
+    bar = 'bar'
+
+
+@dataclass
+class EntityTest:
+    key: str
+
+
+@dataclass
+class Foo:
+    type: Literal['foo']
+    val: int
+
+
+@dataclass
+class Bar:
+    type: Literal['bar']
+    val: str
+
+
+class TypedDictTotalTrue(TypedDict):
+    foo: int
+    bar: NotRequired[str]
+
+
+class TypedDictTotalFalse(TypedDict, total=False):
+    foo: int
+    bar: Required[str]
+
+
+@pytest.mark.parametrize(
+    ['cls', 'value'],
+    (
+        (bool, True),
+        (bool, False),
+        (str, ''),
+        (Annotated[str, MinLength(1), MaxLength(3)], '12'),
+        (int, -99),
+        (Annotated[int, Min(1), Max(1000)], 99),
+        (float, 1.3),
+        (Annotated[float, Min(0), Max(0.4)], 0.1),
+        (Decimal, '0.1'),  # support str
+        (Decimal, 0.1),  # or int input
+        (Decimal, 'NaN'),  # or int input
+        (uuid.UUID, str(uuid.uuid4())),  # support only str input
+        (time, '12:34'),
+        (time, '12:34:56'),
+        (time, '12:34:56.000078'),
+        (time, '12:34Z'),
+        (time, '12:34+0300'),
+        (time, '12:34+03:00'),
+        (time, '12:34:00+03:00'),
+        (time, '12:34:56.000078+03:00'),
+        (time, '12:34:56.000078+00:00'),
+        (datetime, '2022-10-10T14:23:43'),
+        (datetime, '2022-10-10T14:23:43.123456'),
+        (datetime, '2022-10-10T14:23:43.123456Z'),
+        (datetime, '2022-10-10T14:23:43.123456+00:00'),
+        (datetime, '2022-10-10T14:23:43.123456-00:00'),
+        (date, '2020-07-17'),
+        (EnumTest, 'foo'),
+        (Optional[int], None),
+        (Optional[int], 1),
+        (EntityTest, {'key': 'val'}),
+        (list[int], [1, 2]),
+        (dict[str, int], {'a': 1}),
+        (tuple[str, int, bool], ['1', 2, True]),
+        (Annotated[Union[Foo, Bar], Discriminator('type')], {'type': 'foo', 'val': 1}),
+        (Annotated[Union[Foo, Bar], Discriminator('type')], {'type': 'bar', 'val': '1'}),
+        (Any, ['1', 2, True]),
+        (Any, {}),
+        (TypedDictTotalTrue, {'foo': 1}),
+        (TypedDictTotalTrue, {'foo': 1, 'bar': '1'}),
+        (TypedDictTotalFalse, {'bar': '1'}),
+        (TypedDictTotalFalse, {'foo': 1, 'bar': '1'}),
+    ),
+)
+def test_validate(cls, value):
+    Serializer(cls).load(value)
+
+
+if sys.version_info >= (3, 10):
+
+    @pytest.mark.parametrize(
+        ['cls', 'value'],
+        (
+            (Optional[int], None),
+            (int | None, None),
+            (int | None, 2),
+        ),
+    )
+    def test_validate_new_union(cls, value):
+        Serializer(cls).load(value)
+
+
+def _mk_e(m=mock.ANY, ip=mock.ANY) -> Callable[[ErrorItem], None]:
+    def cmp(e: ErrorItem) -> None:
+        assert e.message == m and e.instance_path == ip
+
+    return cmp
+
+
+@pytest.mark.parametrize(
+    ['cls', 'value', 'check'],
+    (
+        (bool, 1, _mk_e(m='1 is not of type "boolean"')),
+        (str, 1, _mk_e(m='1 is not of type "string"')),
+        (
+            Annotated[str, MinLength(2)],
+            'a',
+            _mk_e(m='"a" is shorter than 2 characters'),
+        ),
+        (
+            Annotated[str, MaxLength(2)],
+            'aaa',
+            _mk_e(m='"aaa" is longer than 2 characters'),
+        ),
+        (int, 9.1, _mk_e(m='9.1 is not of type "integer"')),
+        (int, '9', _mk_e(m='"9" is not of type "integer"')),
+        (
+            Annotated[int, Min(1)],
+            0,
+            _mk_e(m='0 is less than the minimum of 1'),
+        ),
+        (
+            Annotated[int, Max(1)],
+            10,
+            _mk_e(m='10 is greater than the maximum of 1'),
+        ),
+        (float, None, _mk_e(m='None is not of type "number"')),
+        (
+            Annotated[float, Min(1.1)],
+            0.1,
+            _mk_e(m='0.1 is less than the minimum of 1.1'),
+        ),
+        (
+            Annotated[float, Max(1.5)],
+            10.1,
+            _mk_e(m='10.1 is greater than the maximum of 1.5'),
+        ),
+        (uuid.UUID, 'asd', _mk_e(ip='')),
+        (time, '12:34:a', _mk_e(ip='')),
+        (datetime, '2022-10-10//12', _mk_e(ip='')),
+        (date, '17-02-2022', _mk_e(ip='')),
+        (datetime, '2022-10-10T14:23:43.123456-30:00', _mk_e(ip='')),
+        (EnumTest, 'buz', _mk_e(m='"buz" is not one of ["bar", "foo"]')),
+        (
+            Optional[int],
+            'foo',
+            _mk_e(m='"foo" is not of type "integer"'),
+        ),
+        (EntityTest, {}, _mk_e(m='"key" is a required property')),
+        (
+            list[int],
+            [1, '1'],
+            _mk_e(m='"1" is not of type "integer"', ip='1'),
+        ),
+        (
+            dict[str, int],
+            {'a': '1'},
+            _mk_e(m='"1" is not of type "integer"', ip='a'),
+        ),
+        (
+            tuple[str, int, bool],
+            ['1'],
+            _mk_e(m="['1'] has less than 3 items"),
+        ),
+        (
+            tuple[str, int, bool],
+            ['1', 1, True, 0],
+            _mk_e(m="['1', 1, True, 0] has more than 3 items"),
+        ),
+        (
+            tuple[str, bool],
+            ['1', 1],
+            _mk_e(
+                m='1 is not of type "boolean"',
+                ip='1',
+            ),
+        ),
+        (
+            Annotated[Union[Foo, Bar], Discriminator('type')],
+            {'type': 'buz'},
+            _mk_e(m='"buz" is not one of ["foo", "bar"] discriminator values'),
+        ),
+        (
+            Annotated[Union[Foo, Bar], Discriminator('type')],
+            {'type': 'foo', 'val': '123'},
+            _mk_e(ip='val', m='"123" is not of type "integer"'),
+        ),
+        (
+            Annotated[Union[Foo, Bar], Discriminator('type')],
+            {'type': 'bar', 'val': 1},
+            _mk_e(ip='val', m='1 is not of type "string"'),
+        ),
+        (TypedDictTotalTrue, {}, _mk_e(m='"foo" is a required property')),
+        (TypedDictTotalFalse, {}, _mk_e(m='"bar" is a required property')),
+    ),
+)
+def test_validate__validation_error(cls, value, check):
+    serializer = Serializer(cls)
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load(value)
+
+    assert len(exc_info.value.errors) == 1
+    check(exc_info.value.errors[0])
+
+
+def test_validate__error_format():
+    @dataclass
+    class Inner:
+        baz: str
+
+    @dataclass
+    class A:
+        foo: int
+        bar: Inner
+
+    serializer = Serializer(A)
+
+    value = {'foo': '1', 'bar': {'buz': None}, 'qux': 0}
+
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load(value)
+
+    assert exc_info.value.errors == [
+        ErrorItem(
+            message='"1" is not of type "integer"',
+            instance_path='foo',
+        ),
+    ]
+
+
+def test_validation_exceptions_inheritance():
+    serializer = Serializer(int)
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load('1')
+
+    assert isinstance(exc_info.value, ValidationError)
+    assert exc_info.value.message == 'Schema validation failed'
+
+
+def test_validation_error_message():
+    @dataclass
+    class A:
+        foo: int
+        bar: str
+
+    serializer = Serializer(A)
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load({'foo': '1', 'bar': 2})
+
+    error = exc_info.value
+    error_item = error.errors[0]
+
+    assert str(error_item) == (""""1" is not of type "integer" (instance_path='foo')""")
+    assert repr(error_item) == ("""ErrorItem(message='"1" is not of type "integer"', instance_path='foo')""")
+    assert str(error) == textwrap.dedent(
+        """\
+    Schema validation failed:
+    - "1" is not of type "integer" (instance_path='foo')
+      """
+    )
+    assert repr(error) == textwrap.dedent(
+        """\
+    SchemaValidationError(
+        message="Schema validation failed",
+        errors=[
+            ErrorItem(message='"1" is not of type "integer"', instance_path='foo'),
+        ]
+    )"""
+    )
```

### Comparing `serpyco_rs-1.7.1/tests/test_custom_encoder.py` & `serpyco_rs-1.8.0/tests/test_custom_encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-from dataclasses import dataclass
-from datetime import datetime
-from typing import Annotated
-
-import pytest
-from serpyco_rs import Serializer
-from serpyco_rs.metadata import CustomEncoder, deserialize_with, serialize_with
-
-
-@dataclass
-class Foo:
-    val: Annotated[str, CustomEncoder[str, str](serialize=str.upper, deserialize=str.lower)]
-
-
-def test_custom_encoder():
-    serializer = Serializer(Foo)
-    val = Foo(val='foo')
-    raw = {'val': 'FOO'}
-    assert serializer.dump(val) == raw
-    assert serializer.load(raw) == val
-
-
-def test_serialize_with():
-    serializer = Serializer(Annotated[datetime, serialize_with(lambda x: x)])
-    val = datetime.now()
-    assert serializer.dump(val) is val
-
-
-def test_deserialize_with():
-    serializer = Serializer(Annotated[datetime, deserialize_with(lambda x: x)])
-    val = datetime.now()
-    assert serializer.load(val) is val
+from dataclasses import dataclass
+from datetime import datetime
+from typing import Annotated
+
+import pytest
+from serpyco_rs import Serializer, SchemaValidationError, ErrorItem
+from serpyco_rs.metadata import CustomEncoder, deserialize_with, serialize_with
+
+
+@dataclass
+class Foo:
+    val: Annotated[str, CustomEncoder[str, str](serialize=str.upper, deserialize=str.lower)]
+
+
+def test_custom_encoder():
+    serializer = Serializer(Foo)
+    val = Foo(val='foo')
+    raw = {'val': 'FOO'}
+    assert serializer.dump(val) == raw
+    assert serializer.load(raw) == val
+
+
+def test_serialize_with():
+    serializer = Serializer(Annotated[datetime, serialize_with(lambda x: x)])
+    val = datetime.now()
+    assert serializer.dump(val) is val
+
+
+def test_deserialize_with():
+    serializer = Serializer(Annotated[datetime, deserialize_with(lambda x: x)])
+    val = datetime.now()
+    assert serializer.load(val) is val
+
+
+def test_deserialize_with__validation_error():
+    serializer = Serializer(Annotated[int, deserialize_with(int)])
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load('foo')
+
+    assert exc_info.value.errors == [
+        ErrorItem(message="ValueError: invalid literal for int() with base 10: 'foo'", instance_path='')
+    ]
```

### Comparing `serpyco_rs-1.7.1/tests/test_encoders.py` & `serpyco_rs-1.8.0/tests/test_encoders.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-import json
-import sys
-import uuid
-from dataclasses import dataclass
-from datetime import date, datetime, time, timedelta, timezone
-from decimal import Decimal
-from enum import Enum, IntEnum
-from typing import Generic, Literal, TypeVar
-from zoneinfo import ZoneInfo
-
-import pytest
-from dateutil.tz import tzoffset
-from serpyco_rs import Serializer, ValidationError
-from typing_extensions import TypedDict
-
-
-@pytest.mark.parametrize(
-    ['type', 'value'],
-    (
-        (int, 44),
-        (str, '123'),
-        (float, 4.3),
-        (bool, True),
-    ),
-)
-def test_simple_types(type, value):
-    serializer = Serializer(type)
-    dump_result = serializer.dump(value)
-    assert serializer.load(dump_result) == value
-
-
-def test_decimal():
-    serializer = Serializer(Decimal)
-    assert serializer.dump(Decimal('123.1')) == '123.1'
-    assert serializer.load(123.1) == Decimal('123.1')
-    assert serializer.load('123.1') == Decimal('123.1')
-
-
-def test_decimal_invalid_value__raise_validation_error():
-    serializer = Serializer(Decimal)
-
-    with pytest.raises(ValidationError):
-        serializer.load('asd')
-
-
-def test_dict_encoder():
-    serializer = Serializer(dict[str, Decimal])
-    val = {'a': Decimal('123.3')}
-    assert serializer.dump(val) == {'a': '123.3'}
-    assert serializer.load({'a': '123.3'}) == val
-
-
-def test_array_encoder():
-    serializer = Serializer(list[int])
-    val = [1, 2, 3]
-    assert serializer.dump(val) == serializer.load(val) == val
-
-
-def test_entity_encoder():
-    @dataclass
-    class A:
-        int_f: int
-        float_f: float
-        bool_f: bool
-        str_f: str
-
-    serializer = Serializer(A)
-
-    obj = A(
-        int_f=123,
-        float_f=3.14,
-        bool_f=True,
-        str_f='Test',
-    )
-    expected = {'bool_f': True, 'float_f': 3.14, 'int_f': 123, 'str_f': 'Test'}
-    assert serializer.dump(obj) == expected
-    assert serializer.load(expected) == obj
-
-
-def test_uuid():
-    serializer = Serializer(uuid.UUID)
-    val = uuid.uuid4()
-    assert serializer.dump(val) == str(val)
-    assert serializer.load(str(val)) == val
-
-
-def test_enum():
-    class Foo(Enum):
-        foo = 'foo'
-
-    serializer = Serializer(Foo)
-    assert serializer.dump(Foo.foo) == 'foo'
-    assert serializer.load('foo') == Foo.foo
-
-
-def test_tuple():
-    serializer = Serializer(tuple[int, bool, str])
-    assert serializer.dump((1, True, 's')) == [1, True, 's']
-    assert serializer.load([1, True, 's']) == (1, True, 's')
-
-
-@pytest.mark.parametrize(
-    ['value', 'expected'],
-    (
-        (datetime(2022, 10, 10, 14, 23, 43), '2022-10-10T14:23:43'),
-        (datetime(2022, 10, 10, 14, 23, 43, 123456), '2022-10-10T14:23:43.123456'),
-        (
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
-            '2022-10-10T14:23:43Z',
-        ),
-        (
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone(timedelta(hours=1))),
-            '2022-10-10T14:23:43+01:00',
-        ),
-        (
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=ZoneInfo('Europe/Berlin')),
-            '2022-10-10T14:23:43+02:00',
-        ),
-    ),
-)
-def test_datetime_dump(value, expected):
-    serializer = Serializer(datetime)
-    assert serializer.dump(value) == expected
-
-
-def test_datetime_dump__naive_datetime_to_utc__expect_utc():
-    serializer = Serializer(datetime, naive_datetime_to_utc=True)
-    assert serializer.dump(datetime(2022, 10, 10, 14, 23, 43)) == '2022-10-10T14:23:43Z'
-
-
-@pytest.mark.parametrize(
-    ['value', 'expected'],
-    (
-        ('2022-10-10T14:23:43', datetime(2022, 10, 10, 14, 23, 43)),
-        ('2022-10-10T14:23:43.123456', datetime(2022, 10, 10, 14, 23, 43, 123456)),
-        (
-            '2022-10-10T14:23:43+00:00',
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
-        ),
-        (
-            '2022-10-10T14:23:43Z',
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
-        ),
-        (
-            '2022-10-10T14:23:43+01:00',
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone(timedelta(hours=1))),
-        ),
-        (
-            '2022-10-10T14:23:43+02:00',
-            datetime(2022, 10, 10, 14, 23, 43, tzinfo=ZoneInfo('Europe/Berlin')),
-        ),
-        (
-            '2024-04-02T12:21:53.725421224',
-            datetime(2024, 4, 2, 12, 21, 53, 725421),
-        ),
-    ),
-)
-def test_datetime_load(value, expected):
-    serializer = Serializer(datetime)
-    assert serializer.load(value) == expected
-
-
-@pytest.mark.parametrize(
-    ['value', 'expected'],
-    [
-        ('12:34', time(12, 34)),
-        ('12:34:56', time(12, 34, 56)),
-        ('12:34:56.000078', time(12, 34, 56, 78)),
-        ('12:34:57.000095987', time(12, 34, 57, 95)),
-        (
-            '12:34:56.000078+03:00',
-            time(12, 34, 56, 78, tzinfo=tzoffset(None, timedelta(hours=3))),
-        ),
-    ],
-)
-def test_time_load(value, expected):
-    serializer = Serializer(time)
-    assert serializer.load(value) == expected
-
-
-@pytest.mark.parametrize(
-    ['value', 'expected'],
-    [
-        (time(12, 34), '12:34:00'),
-        (time(12, 34, tzinfo=tzoffset(None, 10800)), '12:34:00+03:00'),
-        (time(12, 34, 56), '12:34:56'),
-        (time(12, 34, 56, 78), '12:34:56.000078'),
-        (time(12, 34, tzinfo=timezone.utc), '12:34:00Z'),
-        (time(12, 34, tzinfo=timezone(timedelta(hours=1))), '12:34:00+01:00'),
-    ],
-)
-def test_time_dump(value, expected):
-    serializer = Serializer(time)
-    assert serializer.dump(value) == expected
-
-
-def test_date():
-    serializer = Serializer(date)
-    assert serializer.load('2022-10-14') == date(2022, 10, 14)
-    assert serializer.dump(date(2022, 10, 13)) == '2022-10-13'
-
-
-def test_date__dump_datatime__expect_date():
-    serializer = Serializer(date)
-    assert serializer.dump(datetime(2022, 10, 13, 12, 34, 56)) == '2022-10-13'
-
-
-def test_literal():
-    serializer = Serializer(Literal['foo', 'bar'])
-    assert serializer.load('bar') == 'bar'
-    assert serializer.dump('foo') == 'foo'
-
-
-@pytest.mark.skipif(sys.version_info < (3, 10), reason='New style unions available after 3.10')
-def test_optional():
-    @dataclass
-    class T:
-        foo: int | None = None
-
-    serializer = Serializer(T)
-    assert serializer.dump(T()) == {'foo': None}
-    assert serializer.dump(T(foo=1)) == {'foo': 1}
-    assert serializer.load({}) == T()
-    assert serializer.load({'foo': 12}) == T(foo=12)
-
-
-def test_int_enum():
-    class Foo(IntEnum):
-        foo = 1
-        bar = 2
-
-    serializer = Serializer(Foo)
-    assert serializer.dump(Foo.foo) == 1
-    assert serializer.load(1) == Foo.foo
-
-
-@pytest.mark.skipif(sys.version_info < (3, 11), reason='StrEnum available after 3.11')
-def test_str_enum():
-    from enum import StrEnum
-
-    class Foo(StrEnum):
-        foo = 'foo'
-        bar = 'bar'
-
-    serializer = Serializer(Foo)
-    assert serializer.dump(Foo.foo) == 'foo'
-    assert serializer.load('bar') == Foo.bar
-
-
-def test_typed_dict():
-    _T = TypeVar('_T')
-
-    class T(TypedDict, Generic[_T]):
-        foo_filed: int
-        generic_field: _T
-
-    serializer = Serializer(T[bool], camelcase_fields=True)
-    assert serializer.dump({'foo_filed': 1, 'generic_field': True}) == {'fooFiled': 1, 'genericField': True}
-    assert serializer.load({'fooFiled': 1, 'genericField': True}) == {'foo_filed': 1, 'generic_field': True}
-
-
-def test_bytes():
-    serializer = Serializer(bytes)
-    assert serializer.dump(b'foo') == b'foo'
-    assert serializer.load(b'foo') == b'foo'
+import json
+import sys
+import uuid
+from dataclasses import dataclass
+from datetime import date, datetime, time, timedelta, timezone
+from decimal import Decimal
+from enum import Enum, IntEnum
+from typing import Generic, Literal, TypeVar
+from zoneinfo import ZoneInfo
+
+import pytest
+from dateutil.tz import tzoffset
+from serpyco_rs import Serializer, ValidationError
+from typing_extensions import TypedDict
+
+
+@pytest.mark.parametrize(
+    ['type', 'value'],
+    (
+        (int, 44),
+        (str, '123'),
+        (float, 4.3),
+        (bool, True),
+    ),
+)
+def test_simple_types(type, value):
+    serializer = Serializer(type)
+    dump_result = serializer.dump(value)
+    assert serializer.load(dump_result) == value
+
+
+def test_decimal():
+    serializer = Serializer(Decimal)
+    assert serializer.dump(Decimal('123.1')) == '123.1'
+    assert serializer.load(123.1) == Decimal('123.1')
+    assert serializer.load('123.1') == Decimal('123.1')
+
+
+def test_decimal_invalid_value__raise_validation_error():
+    serializer = Serializer(Decimal)
+
+    with pytest.raises(ValidationError):
+        serializer.load('asd')
+
+
+def test_dict_encoder():
+    serializer = Serializer(dict[str, Decimal])
+    val = {'a': Decimal('123.3')}
+    assert serializer.dump(val) == {'a': '123.3'}
+    assert serializer.load({'a': '123.3'}) == val
+
+
+def test_array_encoder():
+    serializer = Serializer(list[int])
+    val = [1, 2, 3]
+    assert serializer.dump(val) == serializer.load(val) == val
+
+
+def test_entity_encoder():
+    @dataclass
+    class A:
+        int_f: int
+        float_f: float
+        bool_f: bool
+        str_f: str
+
+    serializer = Serializer(A)
+
+    obj = A(
+        int_f=123,
+        float_f=3.14,
+        bool_f=True,
+        str_f='Test',
+    )
+    expected = {'bool_f': True, 'float_f': 3.14, 'int_f': 123, 'str_f': 'Test'}
+    assert serializer.dump(obj) == expected
+    assert serializer.load(expected) == obj
+
+
+def test_uuid():
+    serializer = Serializer(uuid.UUID)
+    val = uuid.uuid4()
+    assert serializer.dump(val) == str(val)
+    assert serializer.load(str(val)) == val
+
+
+def test_enum():
+    class Foo(Enum):
+        foo = 'foo'
+
+    serializer = Serializer(Foo)
+    assert serializer.dump(Foo.foo) == 'foo'
+    assert serializer.load('foo') == Foo.foo
+
+
+def test_tuple():
+    serializer = Serializer(tuple[int, bool, str])
+    assert serializer.dump((1, True, 's')) == [1, True, 's']
+    assert serializer.load([1, True, 's']) == (1, True, 's')
+
+
+@pytest.mark.parametrize(
+    ['value', 'expected'],
+    (
+        (datetime(2022, 10, 10, 14, 23, 43), '2022-10-10T14:23:43'),
+        (datetime(2022, 10, 10, 14, 23, 43, 123456), '2022-10-10T14:23:43.123456'),
+        (
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
+            '2022-10-10T14:23:43Z',
+        ),
+        (
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone(timedelta(hours=1))),
+            '2022-10-10T14:23:43+01:00',
+        ),
+        (
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=ZoneInfo('Europe/Berlin')),
+            '2022-10-10T14:23:43+02:00',
+        ),
+    ),
+)
+def test_datetime_dump(value, expected):
+    serializer = Serializer(datetime)
+    assert serializer.dump(value) == expected
+
+
+def test_datetime_dump__naive_datetime_to_utc__expect_utc():
+    serializer = Serializer(datetime, naive_datetime_to_utc=True)
+    assert serializer.dump(datetime(2022, 10, 10, 14, 23, 43)) == '2022-10-10T14:23:43Z'
+
+
+@pytest.mark.parametrize(
+    ['value', 'expected'],
+    (
+        ('2022-10-10T14:23:43', datetime(2022, 10, 10, 14, 23, 43)),
+        ('2022-10-10T14:23:43.123456', datetime(2022, 10, 10, 14, 23, 43, 123456)),
+        (
+            '2022-10-10T14:23:43+00:00',
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
+        ),
+        (
+            '2022-10-10T14:23:43Z',
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone.utc),
+        ),
+        (
+            '2022-10-10T14:23:43+01:00',
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=timezone(timedelta(hours=1))),
+        ),
+        (
+            '2022-10-10T14:23:43+02:00',
+            datetime(2022, 10, 10, 14, 23, 43, tzinfo=ZoneInfo('Europe/Berlin')),
+        ),
+        (
+            '2024-04-02T12:21:53.725421224',
+            datetime(2024, 4, 2, 12, 21, 53, 725421),
+        ),
+    ),
+)
+def test_datetime_load(value, expected):
+    serializer = Serializer(datetime)
+    assert serializer.load(value) == expected
+
+
+@pytest.mark.parametrize(
+    ['value', 'expected'],
+    [
+        ('12:34', time(12, 34)),
+        ('12:34:56', time(12, 34, 56)),
+        ('12:34:56.000078', time(12, 34, 56, 78)),
+        ('12:34:57.000095987', time(12, 34, 57, 95)),
+        (
+            '12:34:56.000078+03:00',
+            time(12, 34, 56, 78, tzinfo=tzoffset(None, timedelta(hours=3))),
+        ),
+    ],
+)
+def test_time_load(value, expected):
+    serializer = Serializer(time)
+    assert serializer.load(value) == expected
+
+
+@pytest.mark.parametrize(
+    ['value', 'expected'],
+    [
+        (time(12, 34), '12:34:00'),
+        (time(12, 34, tzinfo=tzoffset(None, 10800)), '12:34:00+03:00'),
+        (time(12, 34, 56), '12:34:56'),
+        (time(12, 34, 56, 78), '12:34:56.000078'),
+        (time(12, 34, tzinfo=timezone.utc), '12:34:00Z'),
+        (time(12, 34, tzinfo=timezone(timedelta(hours=1))), '12:34:00+01:00'),
+    ],
+)
+def test_time_dump(value, expected):
+    serializer = Serializer(time)
+    assert serializer.dump(value) == expected
+
+
+def test_date():
+    serializer = Serializer(date)
+    assert serializer.load('2022-10-14') == date(2022, 10, 14)
+    assert serializer.dump(date(2022, 10, 13)) == '2022-10-13'
+
+
+def test_date__dump_datatime__expect_date():
+    serializer = Serializer(date)
+    assert serializer.dump(datetime(2022, 10, 13, 12, 34, 56)) == '2022-10-13'
+
+
+def test_literal():
+    serializer = Serializer(Literal['foo', 'bar'])
+    assert serializer.load('bar') == 'bar'
+    assert serializer.dump('foo') == 'foo'
+
+
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='New style unions available after 3.10')
+def test_optional():
+    @dataclass
+    class T:
+        foo: int | None = None
+
+    serializer = Serializer(T)
+    assert serializer.dump(T()) == {'foo': None}
+    assert serializer.dump(T(foo=1)) == {'foo': 1}
+    assert serializer.load({}) == T()
+    assert serializer.load({'foo': 12}) == T(foo=12)
+
+
+def test_int_enum():
+    class Foo(IntEnum):
+        foo = 1
+        bar = 2
+
+    serializer = Serializer(Foo)
+    assert serializer.dump(Foo.foo) == 1
+    assert serializer.load(1) == Foo.foo
+
+
+@pytest.mark.skipif(sys.version_info < (3, 11), reason='StrEnum available after 3.11')
+def test_str_enum():
+    from enum import StrEnum
+
+    class Foo(StrEnum):
+        foo = 'foo'
+        bar = 'bar'
+
+    serializer = Serializer(Foo)
+    assert serializer.dump(Foo.foo) == 'foo'
+    assert serializer.load('bar') == Foo.bar
+
+
+def test_typed_dict():
+    _T = TypeVar('_T')
+
+    class T(TypedDict, Generic[_T]):
+        foo_filed: int
+        generic_field: _T
+
+    serializer = Serializer(T[bool], camelcase_fields=True)
+    assert serializer.dump({'foo_filed': 1, 'generic_field': True}) == {'fooFiled': 1, 'genericField': True}
+    assert serializer.load({'fooFiled': 1, 'genericField': True}) == {'foo_filed': 1, 'generic_field': True}
+
+
+def test_bytes():
+    serializer = Serializer(bytes)
+    assert serializer.dump(b'foo') == b'foo'
+    assert serializer.load(b'foo') == b'foo'
```

### Comparing `serpyco_rs-1.7.1/tests/test_generics.py` & `serpyco_rs-1.8.0/tests/test_generics.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from dataclasses import dataclass
-from typing import Generic, Optional, TypeVar
-from unittest import mock
-
-from serpyco_rs import Serializer
-
-
-T = TypeVar('T')
-
-
-@dataclass
-class GenericType(Generic[T]):
-    value: Optional[T] = None
-    path: Optional[str] = None
-
-
-@dataclass
-class CustomType:
-    q: str
-    w: int
-
-
-@dataclass
-class A:
-    a: GenericType[bool]
-    b: GenericType[CustomType]
-    c: GenericType[int]
-    d: GenericType[float]
-    e: GenericType[str]
-    f: GenericType[str]
-    g: Optional[GenericType[str]] = None
-
-
-def test_generics__serialization():
-    serializer = Serializer(A, omit_none=True)
-
-    a = A(
-        a=GenericType(
-            value=True,
-            path='some_path',
-        ),
-        b=GenericType(
-            value=CustomType(
-                q='q',
-                w=1,
-            ),
-            path='some_path',
-        ),
-        c=GenericType(
-            value=1,
-            path='some_path',
-        ),
-        d=GenericType(
-            value=2.0,
-            path='some_path',
-        ),
-        e=GenericType(
-            value='value',
-            path='some_path',
-        ),
-        f=GenericType(),
-        g=None,
-    )
-
-    raw_a = {
-        'a': {
-            'value': True,
-            'path': 'some_path',
-        },
-        'b': {
-            'value': {
-                'q': 'q',
-                'w': 1,
-            },
-            'path': 'some_path',
-        },
-        'c': {
-            'value': 1,
-            'path': 'some_path',
-        },
-        'd': {
-            'value': 2.0,
-            'path': 'some_path',
-        },
-        'e': {
-            'value': 'value',
-            'path': 'some_path',
-        },
-        'f': {},
-    }
-
-    assert serializer.dump(a) == raw_a
-    assert serializer.load(raw_a) == a
-
-
-def test_generics__swagger_schema():
-    serializer = Serializer(A)
-    assert serializer.get_json_schema() == {
-        '$ref': '#/components/schemas/tests.test_generics.A[no_format,keep_nones]',
-        '$schema': 'https://json-schema.org/draft/2020-12/schema',
-        'components': {
-            'schemas': {
-                'tests.test_generics.A[no_format,keep_nones]': {
-                    'properties': {
-                        'a': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[bool][no_format,keep_nones]'
-                        },
-                        'b': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[tests.test_generics.CustomType][no_format,keep_nones]'
-                        },
-                        'c': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[int][no_format,keep_nones]'
-                        },
-                        'd': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[float][no_format,keep_nones]'
-                        },
-                        'e': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
-                        },
-                        'f': {
-                            '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
-                        },
-                        'g': {
-                            'anyOf': [
-                                {'type': 'null'},
-                                {
-                                    '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
-                                },
-                            ]
-                        },
-                    },
-                    'required': ['a', 'b', 'c', 'd', 'e', 'f'],
-                    'type': 'object',
-                },
-                'tests.test_generics.CustomType[no_format,keep_nones]': {
-                    'properties': {'q': {'type': 'string'}, 'w': {'type': 'integer'}},
-                    'required': ['q', 'w'],
-                    'type': 'object',
-                },
-                'tests.test_generics.GenericType[bool][no_format,keep_nones]': {
-                    'properties': {
-                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                        'value': {'anyOf': [{'type': 'null'}, {'type': 'boolean'}]},
-                    },
-                    'type': 'object',
-                },
-                'tests.test_generics.GenericType[float][no_format,keep_nones]': {
-                    'properties': {
-                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                        'value': {'anyOf': [{'type': 'null'}, {'type': 'number'}]},
-                    },
-                    'type': 'object',
-                },
-                'tests.test_generics.GenericType[int][no_format,keep_nones]': {
-                    'properties': {
-                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                        'value': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]},
-                    },
-                    'type': 'object',
-                },
-                'tests.test_generics.GenericType[str][no_format,keep_nones]': {
-                    'properties': {
-                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                        'value': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                    },
-                    'type': 'object',
-                },
-                'tests.test_generics.GenericType[tests.test_generics.CustomType][no_format,keep_nones]': {
-                    'properties': {
-                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
-                        'value': {
-                            'anyOf': [
-                                {'type': 'null'},
-                                {'$ref': '#/components/schemas/tests.test_generics.CustomType[no_format,keep_nones]'},
-                            ]
-                        },
-                    },
-                    'type': 'object',
-                },
-            }
-        },
-    }
-
-
-def test_generics_inheritance():
-    @dataclass
-    class Parent(Generic[T]):
-        value: T
-
-    @dataclass
-    class Child(Parent[bool]):
-        pass
-
-    serializer = Serializer(Child)
-    assert serializer.dump(Child(42)) == {'value': 42}
+from dataclasses import dataclass
+from typing import Generic, Optional, TypeVar
+from unittest import mock
+
+from serpyco_rs import Serializer
+
+
+T = TypeVar('T')
+
+
+@dataclass
+class GenericType(Generic[T]):
+    value: Optional[T] = None
+    path: Optional[str] = None
+
+
+@dataclass
+class CustomType:
+    q: str
+    w: int
+
+
+@dataclass
+class A:
+    a: GenericType[bool]
+    b: GenericType[CustomType]
+    c: GenericType[int]
+    d: GenericType[float]
+    e: GenericType[str]
+    f: GenericType[str]
+    g: Optional[GenericType[str]] = None
+
+
+def test_generics__serialization():
+    serializer = Serializer(A, omit_none=True)
+
+    a = A(
+        a=GenericType(
+            value=True,
+            path='some_path',
+        ),
+        b=GenericType(
+            value=CustomType(
+                q='q',
+                w=1,
+            ),
+            path='some_path',
+        ),
+        c=GenericType(
+            value=1,
+            path='some_path',
+        ),
+        d=GenericType(
+            value=2.0,
+            path='some_path',
+        ),
+        e=GenericType(
+            value='value',
+            path='some_path',
+        ),
+        f=GenericType(),
+        g=None,
+    )
+
+    raw_a = {
+        'a': {
+            'value': True,
+            'path': 'some_path',
+        },
+        'b': {
+            'value': {
+                'q': 'q',
+                'w': 1,
+            },
+            'path': 'some_path',
+        },
+        'c': {
+            'value': 1,
+            'path': 'some_path',
+        },
+        'd': {
+            'value': 2.0,
+            'path': 'some_path',
+        },
+        'e': {
+            'value': 'value',
+            'path': 'some_path',
+        },
+        'f': {},
+    }
+
+    assert serializer.dump(a) == raw_a
+    assert serializer.load(raw_a) == a
+
+
+def test_generics__swagger_schema():
+    serializer = Serializer(A)
+    assert serializer.get_json_schema() == {
+        '$ref': '#/components/schemas/tests.test_generics.A[no_format,keep_nones]',
+        '$schema': 'https://json-schema.org/draft/2020-12/schema',
+        'components': {
+            'schemas': {
+                'tests.test_generics.A[no_format,keep_nones]': {
+                    'properties': {
+                        'a': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[bool][no_format,keep_nones]'
+                        },
+                        'b': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[tests.test_generics.CustomType][no_format,keep_nones]'
+                        },
+                        'c': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[int][no_format,keep_nones]'
+                        },
+                        'd': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[float][no_format,keep_nones]'
+                        },
+                        'e': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
+                        },
+                        'f': {
+                            '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
+                        },
+                        'g': {
+                            'anyOf': [
+                                {'type': 'null'},
+                                {
+                                    '$ref': '#/components/schemas/tests.test_generics.GenericType[str][no_format,keep_nones]'
+                                },
+                            ]
+                        },
+                    },
+                    'required': ['a', 'b', 'c', 'd', 'e', 'f'],
+                    'type': 'object',
+                },
+                'tests.test_generics.CustomType[no_format,keep_nones]': {
+                    'properties': {'q': {'type': 'string'}, 'w': {'type': 'integer'}},
+                    'required': ['q', 'w'],
+                    'type': 'object',
+                },
+                'tests.test_generics.GenericType[bool][no_format,keep_nones]': {
+                    'properties': {
+                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                        'value': {'anyOf': [{'type': 'null'}, {'type': 'boolean'}]},
+                    },
+                    'type': 'object',
+                },
+                'tests.test_generics.GenericType[float][no_format,keep_nones]': {
+                    'properties': {
+                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                        'value': {'anyOf': [{'type': 'null'}, {'type': 'number'}]},
+                    },
+                    'type': 'object',
+                },
+                'tests.test_generics.GenericType[int][no_format,keep_nones]': {
+                    'properties': {
+                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                        'value': {'anyOf': [{'type': 'null'}, {'type': 'integer'}]},
+                    },
+                    'type': 'object',
+                },
+                'tests.test_generics.GenericType[str][no_format,keep_nones]': {
+                    'properties': {
+                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                        'value': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                    },
+                    'type': 'object',
+                },
+                'tests.test_generics.GenericType[tests.test_generics.CustomType][no_format,keep_nones]': {
+                    'properties': {
+                        'path': {'anyOf': [{'type': 'null'}, {'type': 'string'}]},
+                        'value': {
+                            'anyOf': [
+                                {'type': 'null'},
+                                {'$ref': '#/components/schemas/tests.test_generics.CustomType[no_format,keep_nones]'},
+                            ]
+                        },
+                    },
+                    'type': 'object',
+                },
+            }
+        },
+    }
+
+
+def test_generics_inheritance():
+    @dataclass
+    class Parent(Generic[T]):
+        value: T
+
+    @dataclass
+    class Child(Parent[bool]):
+        pass
+
+    serializer = Serializer(Child)
+    assert serializer.dump(Child(42)) == {'value': 42}
```

### Comparing `serpyco_rs-1.7.1/tests/test_metadata.py` & `serpyco_rs-1.8.0/tests/test_metadata.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from dataclasses import dataclass
-from typing import Annotated, Optional
-
-import pytest
-from serpyco_rs import SchemaValidationError, Serializer
-from serpyco_rs.metadata import Alias, ForceDefaultForOptional, OmitNone
-
-
-def test_annotated_filed_alias():
-    @dataclass
-    class A:
-        foo: Annotated[str, Alias('bar')]
-
-    serializer = Serializer(A)
-
-    obj = A(foo='123')
-
-    expected = {'bar': '123'}
-    assert serializer.dump(obj) == expected
-    assert serializer.load(expected) == obj
-
-
-def test_omit_none():
-    @dataclass
-    class A:
-        required_val: Optional[bool]
-        optional_val: Optional[bool] = None
-
-    serializer = Serializer(Annotated[A, OmitNone])
-
-    expected = {'required_val': None}
-    assert serializer.dump(A(required_val=None)) == expected
-    assert serializer.load(expected) == A(required_val=None)
-
-
-@dataclass
-class Bar:
-    value: Optional[str] = None
-
-
-@dataclass
-class Foo:
-    bar: Optional[Bar] = None
-
-
-@pytest.mark.parametrize(
-    ['omit_none', 'foo', 'expected'],
-    [
-        (True, Foo(), {}),
-        (True, Foo(Bar()), {'bar': {}}),
-        (False, Foo(), {'bar': None}),
-        (False, Foo(Bar()), {'bar': {'value': None}}),
-    ],
-)
-def test_propagete__omit_none(omit_none, foo, expected):
-    serializer = Serializer(Foo, omit_none=omit_none)
-    res = serializer.dump(foo)
-
-    assert res == expected
-
-
-def test_omit_none_on_dict():
-    serializer = Serializer(dict[str, Optional[bool]], omit_none=True)
-    assert serializer.dump({'foo': True, 'bar': None}) == {'foo': True}
-
-
-def test_force_default_for_optional__propagate_to_nested():
-    @dataclass
-    class A:
-        bar: Optional[bool]
-
-    @dataclass
-    class B:
-        foo: Optional[A]
-
-    serializer = Serializer(B, force_default_for_optional=True)
-
-    assert serializer.load({}) == B(foo=None)
-    assert serializer.load({'foo': {}}) == B(foo=A(bar=None))
-
-
-def test_force_default_for_optional__override_by_annotated():
-    @dataclass
-    class A:
-        val: Optional[bool]
-
-    @dataclass
-    class B:
-        foo: Optional[A]
-        bar: Annotated[Optional[A], ForceDefaultForOptional]
-
-    serializer = Serializer(B)
-
-    assert serializer.load({'foo': None}) == B(foo=None, bar=None)
-
-    # foo is not annotated, and A.val is still nullable+required
-    with pytest.raises(SchemaValidationError):
-        serializer.load({'foo': {}})
-
-    # bar is annotated, and A.val is nullable+non required
-    assert serializer.load({'foo': None, 'bar': {}}) == B(foo=None, bar=A(val=None))
+from dataclasses import dataclass
+from typing import Annotated, Optional
+
+import pytest
+from serpyco_rs import SchemaValidationError, Serializer
+from serpyco_rs.metadata import Alias, ForceDefaultForOptional, OmitNone
+
+
+def test_annotated_filed_alias():
+    @dataclass
+    class A:
+        foo: Annotated[str, Alias('bar')]
+
+    serializer = Serializer(A)
+
+    obj = A(foo='123')
+
+    expected = {'bar': '123'}
+    assert serializer.dump(obj) == expected
+    assert serializer.load(expected) == obj
+
+
+def test_omit_none():
+    @dataclass
+    class A:
+        required_val: Optional[bool]
+        optional_val: Optional[bool] = None
+
+    serializer = Serializer(Annotated[A, OmitNone])
+
+    expected = {'required_val': None}
+    assert serializer.dump(A(required_val=None)) == expected
+    assert serializer.load(expected) == A(required_val=None)
+
+
+@dataclass
+class Bar:
+    value: Optional[str] = None
+
+
+@dataclass
+class Foo:
+    bar: Optional[Bar] = None
+
+
+@pytest.mark.parametrize(
+    ['omit_none', 'foo', 'expected'],
+    [
+        (True, Foo(), {}),
+        (True, Foo(Bar()), {'bar': {}}),
+        (False, Foo(), {'bar': None}),
+        (False, Foo(Bar()), {'bar': {'value': None}}),
+    ],
+)
+def test_propagete__omit_none(omit_none, foo, expected):
+    serializer = Serializer(Foo, omit_none=omit_none)
+    res = serializer.dump(foo)
+
+    assert res == expected
+
+
+def test_omit_none_on_dict():
+    serializer = Serializer(dict[str, Optional[bool]], omit_none=True)
+    assert serializer.dump({'foo': True, 'bar': None}) == {'foo': True}
+
+
+def test_force_default_for_optional__propagate_to_nested():
+    @dataclass
+    class A:
+        bar: Optional[bool]
+
+    @dataclass
+    class B:
+        foo: Optional[A]
+
+    serializer = Serializer(B, force_default_for_optional=True)
+
+    assert serializer.load({}) == B(foo=None)
+    assert serializer.load({'foo': {}}) == B(foo=A(bar=None))
+
+
+def test_force_default_for_optional__override_by_annotated():
+    @dataclass
+    class A:
+        val: Optional[bool]
+
+    @dataclass
+    class B:
+        foo: Optional[A]
+        bar: Annotated[Optional[A], ForceDefaultForOptional]
+
+    serializer = Serializer(B)
+
+    assert serializer.load({'foo': None}) == B(foo=None, bar=None)
+
+    # foo is not annotated, and A.val is still nullable+required
+    with pytest.raises(SchemaValidationError):
+        serializer.load({'foo': {}})
+
+    # bar is annotated, and A.val is nullable+non required
+    assert serializer.load({'foo': None, 'bar': {}}) == B(foo=None, bar=A(val=None))
```

### Comparing `serpyco_rs-1.7.1/tests/test_simple.py` & `serpyco_rs-1.8.0/tests/test_simple.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,310 +1,310 @@
-import sys
-from collections.abc import Mapping, Sequence
-from dataclasses import dataclass, field
-from typing import Annotated, Optional, Literal
-
-import attr
-import pytest
-from serpyco_rs import SchemaValidationError, Serializer
-from serpyco_rs.metadata import CamelCase, NoFormat
-
-
-def test_dump_simple_fields_types():
-    @dataclass
-    class A:
-        int_f: int
-        float_f: float
-        bool_f: bool
-        str_f: str
-
-    serializer = Serializer(A)
-
-    obj = A(
-        int_f=123,
-        float_f=3.14,
-        bool_f=True,
-        str_f='Test',
-    )
-    expected = {'bool_f': True, 'float_f': 3.14, 'int_f': 123, 'str_f': 'Test'}
-    assert serializer.dump(obj) == expected
-    assert serializer.load(expected) == obj
-
-
-def test_simple_nested_dataclasses():
-    @dataclass
-    class C:
-        value: int
-
-    @dataclass
-    class B:
-        value: str
-        nested: C
-
-    @dataclass
-    class A:
-        int_f: int
-        nested: B
-
-    serializer = Serializer(A)
-
-    obj = A(
-        int_f=123,
-        nested=B(value='test', nested=C(value=1)),
-    )
-
-    expected = {'int_f': 123, 'nested': {'nested': {'value': 1}, 'value': 'test'}}
-
-    assert serializer.dump(obj) == expected
-    assert serializer.load(expected) == obj
-
-
-def test_iterables():
-    @dataclass
-    class A:
-        iterable_builtins_list: list[int]
-        iterable_typing_list: list[int]
-        iterable_builtins_sequence: Sequence[int]
-
-    serializer = Serializer(A)
-
-    obj = A(
-        iterable_builtins_list=[1, 2, 3],
-        iterable_typing_list=[1, 2, 3],
-        iterable_builtins_sequence=[1, 2, 3],
-    )
-
-    expected = {
-        'iterable_builtins_list': [1, 2, 3],
-        'iterable_typing_list': [1, 2, 3],
-        'iterable_builtins_sequence': [1, 2, 3],
-    }
-
-    assert serializer.dump(obj) == expected
-    assert serializer.load(expected) == obj
-
-
-def test_mappings():
-    @dataclass
-    class B:
-        value: str
-
-    @dataclass
-    class A:
-        dict_field: dict[str, int]
-        mapping_field: Mapping[str, B]
-
-    serializer = Serializer(A)
-
-    obj = A(dict_field={'foo': 1}, mapping_field={'bar': B(value='123')})
-
-    expected = {
-        'dict_field': {'foo': 1},
-        'mapping_field': {'bar': {'value': '123'}},
-    }
-
-    assert serializer.load(expected) == obj
-    assert serializer.dump(obj) == expected
-
-
-def test_required_and_nullable():
-    @dataclass
-    class ReqNotNull:
-        foo: int
-
-    @dataclass
-    class ReqNullable:
-        foo: Optional[int]
-
-    @dataclass
-    class OptionalNotNull:
-        foo: int = 1
-
-    @dataclass
-    class OptionalNullable:
-        foo: Optional[int] = 1
-
-    req_not_null = Serializer(ReqNotNull)
-    req_nullable = Serializer(ReqNullable)
-    optional_not_null = Serializer(OptionalNotNull)
-    optional_nullable = Serializer(OptionalNullable)
-
-    assert req_not_null.load({'foo': 2}) == ReqNotNull(foo=2)
-    with pytest.raises(SchemaValidationError):
-        req_not_null.load({'foo': None})
-    with pytest.raises(SchemaValidationError):
-        req_not_null.load({})
-
-    assert req_nullable.load({'foo': 2}) == ReqNullable(foo=2)
-    assert req_nullable.load({'foo': None}) == ReqNullable(foo=None)
-    with pytest.raises(SchemaValidationError):
-        req_nullable.load({})
-
-    assert optional_not_null.load({'foo': 2}) == OptionalNotNull(foo=2)
-    with pytest.raises(SchemaValidationError):
-        assert optional_not_null.load({'foo': None})
-    assert optional_not_null.load({}) == OptionalNotNull(foo=1)
-
-    assert optional_nullable.load({'foo': 2}) == OptionalNullable(foo=2)
-    assert optional_nullable.load({'foo': None}) == OptionalNullable(foo=None)
-    assert optional_nullable.load({}) == OptionalNullable(foo=1)
-
-
-def test_nullable_without_default():
-    @dataclass
-    class Entity:
-        foo: Optional[int]
-
-    entity_serializer = Serializer(Entity)
-
-    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
-    with pytest.raises(SchemaValidationError):
-        entity_serializer.load({})
-
-
-def test_nullable_without_default__force_none_as_default_for_optional():
-    @dataclass
-    class Entity:
-        foo: Optional[int]
-
-    entity_serializer = Serializer(Entity, force_default_for_optional=True)
-
-    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
-    assert entity_serializer.load({}) == Entity(foo=None)
-
-
-def test_required__force_none_as_default_for_optional__required_field_not_changed():
-    @dataclass
-    class Entity:
-        foo: int
-
-    entity_serializer = Serializer(Entity, force_default_for_optional=True)
-
-    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
-    with pytest.raises(SchemaValidationError):
-        assert entity_serializer.load({})
-
-
-def test_required_and_nullable_list():
-    @dataclass
-    class Entity:
-        foo: Optional[list[Optional[int]]] = None
-
-    entity_serializer = Serializer(Entity)
-
-    assert entity_serializer.load({}) == Entity(foo=None)
-    assert entity_serializer.load({'foo': None}) == Entity(foo=None)
-    assert entity_serializer.load({'foo': []}) == Entity(foo=[])
-    assert entity_serializer.load({'foo': [1]}) == Entity(foo=[1])
-    assert entity_serializer.load({'foo': [1, None]}) == Entity(foo=[1, None])
-
-
-def test_defaults():
-    @dataclass
-    class Entity:
-        foo: str = '123'
-        bar: list[int] = field(default_factory=lambda: list([1, 2, 3]))
-
-    entity_serializer = Serializer(Entity)
-
-    assert entity_serializer.load({'bar': [1]}) == Entity(foo='123', bar=[1])
-    assert entity_serializer.load({}) == Entity(foo='123', bar=[1, 2, 3])
-
-
-if sys.version_info >= (3, 10):
-
-    def test_union_optional__dump_load__ok():
-        # arrange
-        @dataclass
-        class UnionClass:
-            name: str | None
-            count: None | int
-
-        # act
-        serializer = Serializer(UnionClass)
-
-        # assert
-        foo = UnionClass(name=None, count=None)
-        dict_foo = {'name': None, 'count': None}
-        assert serializer.dump(foo) == dict_foo
-        assert foo == serializer.load(dict_foo)
-
-        bar = UnionClass(name='try', count=5)
-        dict_bar = {'name': 'try', 'count': 5}
-        assert serializer.dump(bar) == dict_bar
-        assert bar == serializer.load(dict_bar)
-
-
-def test_serializer_with_camelcase():
-    @dataclass
-    class C:
-        foo_field: int
-
-    @dataclass
-    class B:
-        some_value: str
-        another_value: Annotated[C, CamelCase]
-
-    @dataclass
-    class A:
-        dict_field: dict[str, int]
-        inner_value_one: B
-        inner_value_two: Annotated[B, NoFormat]
-
-    serializer = Serializer(A, camelcase_fields=True)
-
-    obj = A(
-        dict_field={'foo': 1},
-        inner_value_one=B(some_value='123', another_value=C(11)),
-        inner_value_two=B(some_value='1', another_value=C(22)),
-    )
-
-    expected = {
-        'dictField': {'foo': 1},
-        'innerValueOne': {'someValue': '123', 'anotherValue': {'fooField': 11}},
-        'innerValueTwo': {'some_value': '1', 'another_value': {'fooField': 22}},
-    }
-
-    assert serializer.load(expected) == obj
-    assert serializer.dump(obj) == expected
-
-
-def test_load_frozen_dataclass():
-    @dataclass(frozen=True)
-    class Foo:
-        bar: bool
-
-    serializer = Serializer(Foo)
-
-    assert serializer.load({'bar': True}) == Foo(bar=True)
-
-
-def test_load_frozen_attrs():
-    @attr.frozen
-    class Foo:
-        bar: bool
-
-    serializer = Serializer(Foo)
-
-    assert serializer.load({'bar': True}) == Foo(bar=True)
-
-
-def test_load_literal():
-    @dataclass
-    class Foo:
-        bar: Literal[1, '2']
-
-    serializer = Serializer(Foo)
-
-    assert serializer.load({'bar': 1}) == Foo(bar=1)
-    assert serializer.load({'bar': '2'}) == Foo(bar='2')
-
-
-def test_dump_literal():
-    @dataclass
-    class Foo:
-        bar: Literal[1, '2']
-
-    serializer = Serializer(Foo)
-
-    assert serializer.dump(Foo(bar=1)) == {'bar': 1}
-    assert serializer.dump(Foo(bar='2')) == {'bar': '2'}
+import sys
+from collections.abc import Mapping, Sequence
+from dataclasses import dataclass, field
+from typing import Annotated, Optional, Literal
+
+import attr
+import pytest
+from serpyco_rs import SchemaValidationError, Serializer
+from serpyco_rs.metadata import CamelCase, NoFormat
+
+
+def test_dump_simple_fields_types():
+    @dataclass
+    class A:
+        int_f: int
+        float_f: float
+        bool_f: bool
+        str_f: str
+
+    serializer = Serializer(A)
+
+    obj = A(
+        int_f=123,
+        float_f=3.14,
+        bool_f=True,
+        str_f='Test',
+    )
+    expected = {'bool_f': True, 'float_f': 3.14, 'int_f': 123, 'str_f': 'Test'}
+    assert serializer.dump(obj) == expected
+    assert serializer.load(expected) == obj
+
+
+def test_simple_nested_dataclasses():
+    @dataclass
+    class C:
+        value: int
+
+    @dataclass
+    class B:
+        value: str
+        nested: C
+
+    @dataclass
+    class A:
+        int_f: int
+        nested: B
+
+    serializer = Serializer(A)
+
+    obj = A(
+        int_f=123,
+        nested=B(value='test', nested=C(value=1)),
+    )
+
+    expected = {'int_f': 123, 'nested': {'nested': {'value': 1}, 'value': 'test'}}
+
+    assert serializer.dump(obj) == expected
+    assert serializer.load(expected) == obj
+
+
+def test_iterables():
+    @dataclass
+    class A:
+        iterable_builtins_list: list[int]
+        iterable_typing_list: list[int]
+        iterable_builtins_sequence: Sequence[int]
+
+    serializer = Serializer(A)
+
+    obj = A(
+        iterable_builtins_list=[1, 2, 3],
+        iterable_typing_list=[1, 2, 3],
+        iterable_builtins_sequence=[1, 2, 3],
+    )
+
+    expected = {
+        'iterable_builtins_list': [1, 2, 3],
+        'iterable_typing_list': [1, 2, 3],
+        'iterable_builtins_sequence': [1, 2, 3],
+    }
+
+    assert serializer.dump(obj) == expected
+    assert serializer.load(expected) == obj
+
+
+def test_mappings():
+    @dataclass
+    class B:
+        value: str
+
+    @dataclass
+    class A:
+        dict_field: dict[str, int]
+        mapping_field: Mapping[str, B]
+
+    serializer = Serializer(A)
+
+    obj = A(dict_field={'foo': 1}, mapping_field={'bar': B(value='123')})
+
+    expected = {
+        'dict_field': {'foo': 1},
+        'mapping_field': {'bar': {'value': '123'}},
+    }
+
+    assert serializer.load(expected) == obj
+    assert serializer.dump(obj) == expected
+
+
+def test_required_and_nullable():
+    @dataclass
+    class ReqNotNull:
+        foo: int
+
+    @dataclass
+    class ReqNullable:
+        foo: Optional[int]
+
+    @dataclass
+    class OptionalNotNull:
+        foo: int = 1
+
+    @dataclass
+    class OptionalNullable:
+        foo: Optional[int] = 1
+
+    req_not_null = Serializer(ReqNotNull)
+    req_nullable = Serializer(ReqNullable)
+    optional_not_null = Serializer(OptionalNotNull)
+    optional_nullable = Serializer(OptionalNullable)
+
+    assert req_not_null.load({'foo': 2}) == ReqNotNull(foo=2)
+    with pytest.raises(SchemaValidationError):
+        req_not_null.load({'foo': None})
+    with pytest.raises(SchemaValidationError):
+        req_not_null.load({})
+
+    assert req_nullable.load({'foo': 2}) == ReqNullable(foo=2)
+    assert req_nullable.load({'foo': None}) == ReqNullable(foo=None)
+    with pytest.raises(SchemaValidationError):
+        req_nullable.load({})
+
+    assert optional_not_null.load({'foo': 2}) == OptionalNotNull(foo=2)
+    with pytest.raises(SchemaValidationError):
+        assert optional_not_null.load({'foo': None})
+    assert optional_not_null.load({}) == OptionalNotNull(foo=1)
+
+    assert optional_nullable.load({'foo': 2}) == OptionalNullable(foo=2)
+    assert optional_nullable.load({'foo': None}) == OptionalNullable(foo=None)
+    assert optional_nullable.load({}) == OptionalNullable(foo=1)
+
+
+def test_nullable_without_default():
+    @dataclass
+    class Entity:
+        foo: Optional[int]
+
+    entity_serializer = Serializer(Entity)
+
+    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
+    with pytest.raises(SchemaValidationError):
+        entity_serializer.load({})
+
+
+def test_nullable_without_default__force_none_as_default_for_optional():
+    @dataclass
+    class Entity:
+        foo: Optional[int]
+
+    entity_serializer = Serializer(Entity, force_default_for_optional=True)
+
+    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
+    assert entity_serializer.load({}) == Entity(foo=None)
+
+
+def test_required__force_none_as_default_for_optional__required_field_not_changed():
+    @dataclass
+    class Entity:
+        foo: int
+
+    entity_serializer = Serializer(Entity, force_default_for_optional=True)
+
+    assert entity_serializer.load({'foo': 1}) == Entity(foo=1)
+    with pytest.raises(SchemaValidationError):
+        assert entity_serializer.load({})
+
+
+def test_required_and_nullable_list():
+    @dataclass
+    class Entity:
+        foo: Optional[list[Optional[int]]] = None
+
+    entity_serializer = Serializer(Entity)
+
+    assert entity_serializer.load({}) == Entity(foo=None)
+    assert entity_serializer.load({'foo': None}) == Entity(foo=None)
+    assert entity_serializer.load({'foo': []}) == Entity(foo=[])
+    assert entity_serializer.load({'foo': [1]}) == Entity(foo=[1])
+    assert entity_serializer.load({'foo': [1, None]}) == Entity(foo=[1, None])
+
+
+def test_defaults():
+    @dataclass
+    class Entity:
+        foo: str = '123'
+        bar: list[int] = field(default_factory=lambda: list([1, 2, 3]))
+
+    entity_serializer = Serializer(Entity)
+
+    assert entity_serializer.load({'bar': [1]}) == Entity(foo='123', bar=[1])
+    assert entity_serializer.load({}) == Entity(foo='123', bar=[1, 2, 3])
+
+
+if sys.version_info >= (3, 10):
+
+    def test_union_optional__dump_load__ok():
+        # arrange
+        @dataclass
+        class UnionClass:
+            name: str | None
+            count: None | int
+
+        # act
+        serializer = Serializer(UnionClass)
+
+        # assert
+        foo = UnionClass(name=None, count=None)
+        dict_foo = {'name': None, 'count': None}
+        assert serializer.dump(foo) == dict_foo
+        assert foo == serializer.load(dict_foo)
+
+        bar = UnionClass(name='try', count=5)
+        dict_bar = {'name': 'try', 'count': 5}
+        assert serializer.dump(bar) == dict_bar
+        assert bar == serializer.load(dict_bar)
+
+
+def test_serializer_with_camelcase():
+    @dataclass
+    class C:
+        foo_field: int
+
+    @dataclass
+    class B:
+        some_value: str
+        another_value: Annotated[C, CamelCase]
+
+    @dataclass
+    class A:
+        dict_field: dict[str, int]
+        inner_value_one: B
+        inner_value_two: Annotated[B, NoFormat]
+
+    serializer = Serializer(A, camelcase_fields=True)
+
+    obj = A(
+        dict_field={'foo': 1},
+        inner_value_one=B(some_value='123', another_value=C(11)),
+        inner_value_two=B(some_value='1', another_value=C(22)),
+    )
+
+    expected = {
+        'dictField': {'foo': 1},
+        'innerValueOne': {'someValue': '123', 'anotherValue': {'fooField': 11}},
+        'innerValueTwo': {'some_value': '1', 'another_value': {'fooField': 22}},
+    }
+
+    assert serializer.load(expected) == obj
+    assert serializer.dump(obj) == expected
+
+
+def test_load_frozen_dataclass():
+    @dataclass(frozen=True)
+    class Foo:
+        bar: bool
+
+    serializer = Serializer(Foo)
+
+    assert serializer.load({'bar': True}) == Foo(bar=True)
+
+
+def test_load_frozen_attrs():
+    @attr.frozen
+    class Foo:
+        bar: bool
+
+    serializer = Serializer(Foo)
+
+    assert serializer.load({'bar': True}) == Foo(bar=True)
+
+
+def test_load_literal():
+    @dataclass
+    class Foo:
+        bar: Literal[1, '2']
+
+    serializer = Serializer(Foo)
+
+    assert serializer.load({'bar': 1}) == Foo(bar=1)
+    assert serializer.load({'bar': '2'}) == Foo(bar='2')
+
+
+def test_dump_literal():
+    @dataclass
+    class Foo:
+        bar: Literal[1, '2']
+
+    serializer = Serializer(Foo)
+
+    assert serializer.dump(Foo(bar=1)) == {'bar': 1}
+    assert serializer.dump(Foo(bar='2')) == {'bar': '2'}
```

### Comparing `serpyco_rs-1.7.1/tests/test_type_utils_py311.py` & `serpyco_rs-1.8.0/tests/test_type_utils_py311.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from typing import TypeVar, Generic, TypeVarTuple, Tuple, Unpack
-
-from serpyco_rs._type_utils import get_type_hints
-
-T = TypeVar('T')
-U = TypeVar('U')
-KT = TypeVar('KT')
-VT = TypeVar('VT')
-
-
-def test_get_type_hints_variadic_class():
-    T1 = TypeVar('T1')
-    T2 = TypeVar('T2')
-    Ts = TypeVarTuple('Ts')
-
-    class A(Generic[T1, T2, *Ts]):
-        t1: T1
-        t2: T2
-        ts: Tuple[*Ts]
-
-    assert get_type_hints(A[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
-    assert get_type_hints(A[int, str, float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
-    assert get_type_hints(A[int, str, float, bool]) == {'t1': int, 't2': str, 'ts': Tuple[float, bool]}
-
-    class B(Generic[T1, T2, Unpack[Ts]]):
-        t1: T1
-        t2: T2
-        ts: Tuple[Unpack[Ts]]
-
-    assert get_type_hints(B[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
-    assert get_type_hints(B[int, str, float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
-    assert get_type_hints(B[int, str, float, bool]) == {'t1': int, 't2': str, 'ts': Tuple[float, bool]}
-
-    class C(Generic[T1, *Ts, T2]):
-        t1: T1
-        ts: Tuple[*Ts]
-        t2: T2
-
-    assert get_type_hints(C[int, str]) == {'t1': int, 'ts': Tuple[()], 't2': str}
-    assert get_type_hints(C[int, str, float]) == {'t1': int, 'ts': Tuple[str], 't2': float}
-    assert get_type_hints(C[int, str, float, bool]) == {'t1': int, 'ts': Tuple[str, float], 't2': bool}
-
-    class E(Generic[*Ts, T1, T2]):
-        ts: Tuple[*Ts]
-        t1: T1
-        t2: T2
-
-    assert get_type_hints(E[int, str]) == {'ts': Tuple[()], 't1': int, 't2': str}
-    assert get_type_hints(E[int, str, float]) == {'ts': Tuple[int], 't1': str, 't2': float}
-    assert get_type_hints(E[int, str, float, bool]) == {'ts': Tuple[int, str], 't1': float, 't2': bool}
-
-
-def test_get_type_hints_variadic_type_parameter():
-    T1 = TypeVar('T1')
-    T2 = TypeVar('T2')
-    Ts = TypeVarTuple('Ts')
-
-    class A(Generic[T1, T2, *Ts]):
-        t1: T1
-        t2: T2
-        ts: Tuple[*Ts]
-
-    class B(A[int, str, *Ts]):
-        pass
-
-    assert get_type_hints(B) == {'t1': int, 't2': str, 'ts': Tuple[*Ts]}
-    assert get_type_hints(B[()]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
-    assert get_type_hints(B[float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
-
-
-def test_get_type_hints_variadic_with_typevars():
-    T1 = TypeVar('T1')
-    T2 = TypeVar('T2')
-    Ts = TypeVarTuple('Ts')
-
-    class A(Generic[T1, T2, *Ts]):
-        t1: T1
-        t2: T2
-        ts: Tuple[*Ts]
-
-    class D(A[int, str, T1, T2]):
-        pass
-
-    assert get_type_hints(D[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[int, str]}
+from typing import TypeVar, Generic, TypeVarTuple, Tuple, Unpack
+
+from serpyco_rs._type_utils import get_type_hints
+
+T = TypeVar('T')
+U = TypeVar('U')
+KT = TypeVar('KT')
+VT = TypeVar('VT')
+
+
+def test_get_type_hints_variadic_class():
+    T1 = TypeVar('T1')
+    T2 = TypeVar('T2')
+    Ts = TypeVarTuple('Ts')
+
+    class A(Generic[T1, T2, *Ts]):
+        t1: T1
+        t2: T2
+        ts: Tuple[*Ts]
+
+    assert get_type_hints(A[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
+    assert get_type_hints(A[int, str, float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
+    assert get_type_hints(A[int, str, float, bool]) == {'t1': int, 't2': str, 'ts': Tuple[float, bool]}
+
+    class B(Generic[T1, T2, Unpack[Ts]]):
+        t1: T1
+        t2: T2
+        ts: Tuple[Unpack[Ts]]
+
+    assert get_type_hints(B[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
+    assert get_type_hints(B[int, str, float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
+    assert get_type_hints(B[int, str, float, bool]) == {'t1': int, 't2': str, 'ts': Tuple[float, bool]}
+
+    class C(Generic[T1, *Ts, T2]):
+        t1: T1
+        ts: Tuple[*Ts]
+        t2: T2
+
+    assert get_type_hints(C[int, str]) == {'t1': int, 'ts': Tuple[()], 't2': str}
+    assert get_type_hints(C[int, str, float]) == {'t1': int, 'ts': Tuple[str], 't2': float}
+    assert get_type_hints(C[int, str, float, bool]) == {'t1': int, 'ts': Tuple[str, float], 't2': bool}
+
+    class E(Generic[*Ts, T1, T2]):
+        ts: Tuple[*Ts]
+        t1: T1
+        t2: T2
+
+    assert get_type_hints(E[int, str]) == {'ts': Tuple[()], 't1': int, 't2': str}
+    assert get_type_hints(E[int, str, float]) == {'ts': Tuple[int], 't1': str, 't2': float}
+    assert get_type_hints(E[int, str, float, bool]) == {'ts': Tuple[int, str], 't1': float, 't2': bool}
+
+
+def test_get_type_hints_variadic_type_parameter():
+    T1 = TypeVar('T1')
+    T2 = TypeVar('T2')
+    Ts = TypeVarTuple('Ts')
+
+    class A(Generic[T1, T2, *Ts]):
+        t1: T1
+        t2: T2
+        ts: Tuple[*Ts]
+
+    class B(A[int, str, *Ts]):
+        pass
+
+    assert get_type_hints(B) == {'t1': int, 't2': str, 'ts': Tuple[*Ts]}
+    assert get_type_hints(B[()]) == {'t1': int, 't2': str, 'ts': Tuple[()]}
+    assert get_type_hints(B[float]) == {'t1': int, 't2': str, 'ts': Tuple[float]}
+
+
+def test_get_type_hints_variadic_with_typevars():
+    T1 = TypeVar('T1')
+    T2 = TypeVar('T2')
+    Ts = TypeVarTuple('Ts')
+
+    class A(Generic[T1, T2, *Ts]):
+        t1: T1
+        t2: T2
+        ts: Tuple[*Ts]
+
+    class D(A[int, str, T1, T2]):
+        pass
+
+    assert get_type_hints(D[int, str]) == {'t1': int, 't2': str, 'ts': Tuple[int, str]}
```

### Comparing `serpyco_rs-1.7.1/tests/test_union.py` & `serpyco_rs-1.8.0/tests/test_union.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-import sys
-from dataclasses import dataclass
-from typing import Annotated, Literal, Optional, Union
-
-import pytest
-
-from serpyco_rs import Serializer, SchemaValidationError, ErrorItem
-from serpyco_rs.metadata import Discriminator
-
-
-@dataclass
-class Foo:
-    val: int
-    type: Literal['foo'] = 'foo'
-
-
-@dataclass
-class Bar:
-    type: Literal['bar']
-    val: str
-
-
-@dataclass
-class Buz:
-    type: int
-    val: str
-
-
-@dataclass
-class Buzz:
-    val: str
-
-
-@dataclass
-class Base:
-    childs: list[Annotated[Union[Foo, Bar], Discriminator('type')]]
-
-
-def test_tagged_union():
-    serializer = Serializer(Base)
-    val = Base(
-        childs=[
-            Foo(val=1),
-            Bar(type='bar', val='12'),
-        ]
-    )
-    raw = {'childs': [{'type': 'foo', 'val': 1}, {'type': 'bar', 'val': '12'}]}
-    assert serializer.dump(val) == raw
-    assert serializer.load(raw) == val
-
-
-def test_tagged_union__invalid_discriminator_type():
-    @dataclass
-    class Inner:
-        field: Annotated[Union[Foo, Bar, Buz], Discriminator('type')]
-
-    with pytest.raises(RuntimeError) as exc_info:
-        Serializer(Inner)
-
-    assert exc_info.type is RuntimeError
-    assert exc_info.value.args[0] == (
-        'Type <class \'tests.test_union.Buz\'> has invalid discriminator field "type" with type "<class \'int\'>". '
-        'Discriminator supports only Literal[<str>].'
-    )
-
-
-def test_tagged_union__union_arg_has_no_discriminator_field():
-    @dataclass
-    class Inner:
-        field: Annotated[Union[Foo, Bar, Buzz], Discriminator('type')]
-
-    with pytest.raises(RuntimeError) as exc_info:
-        Serializer(Inner)
-
-    assert exc_info.type is RuntimeError
-    assert exc_info.value.args[0] == 'Type <class \'tests.test_union.Buzz\'> does not have discriminator field "type"'
-
-
-def test_tagged_union__unsupported_types():
-    @dataclass
-    class Inner:
-        field: Annotated[Union[int, str], Discriminator('type')]
-
-    with pytest.raises(RuntimeError) as exc_info:
-        Serializer(Inner)
-
-    assert exc_info.type is RuntimeError
-    assert exc_info.value.args[0] == (
-        "Unions supported only for dataclasses or attrs. Provided: typing.Union[<class 'int'>,<class 'str'>]"
-    )
-
-
-@dataclass
-class A:
-    type: Literal['A']
-    params: int
-    children: Optional[list['ComponentsT']] = None
-
-
-@dataclass
-class B:
-    type: Literal['B']
-    params: str
-    children: Optional[list['ComponentsT']] = None
-
-
-ComponentsT = Annotated[Union[A, B], Discriminator('type')]
-
-
-@pytest.mark.skipif(sys.version_info < (3, 11), reason='requires python3.11 or higher')
-def test_tagged_union__with_forward_refs():
-    serializer = Serializer(ComponentsT, omit_none=True)
-    data: ComponentsT = A(
-        type='A',
-        params=123,
-        children=[
-            A(
-                type='A',
-                params=1234,
-            ),
-            B(
-                type='B',
-                params='foo',
-                children=[
-                    B(
-                        type='B',
-                        params='bar',
-                    )
-                ],
-            ),
-        ],
-    )
-    raw_data = {
-        'type': 'A',
-        'params': 123,
-        'children': [
-            {'params': 1234, 'type': 'A'},
-            {'children': [{'params': 'bar', 'type': 'B'}], 'params': 'foo', 'type': 'B'},
-        ],
-    }
-    assert serializer.dump(data) == raw_data
-    assert serializer.load(raw_data) == data
-
-
-def test_tagged_union__camel_case_filed_format():
-    @dataclass
-    class A:
-        discriminator_with_multiple_words: Literal['A']
-        a: int
-
-    @dataclass
-    class B:
-        discriminator_with_multiple_words: Literal['B']
-        b: str
-
-    raw_obj = [
-        {
-            'discriminatorWithMultipleWords': 'A',
-            'a': 128,
-        },
-        {
-            'discriminatorWithMultipleWords': 'B',
-            'b': 'foo',
-        },
-    ]
-    obj = [
-        A(
-            discriminator_with_multiple_words='A',
-            a=128,
-        ),
-        B(
-            discriminator_with_multiple_words='B',
-            b='foo',
-        ),
-    ]
-
-    serializer = Serializer(
-        list[Annotated[Union[A, B], Discriminator('discriminator_with_multiple_words')]],
-        camelcase_fields=True,
-    )
-
-    assert serializer.dump(obj) == raw_obj
-    assert serializer.load(raw_obj) == obj
-
-
-def test_union_simple_types():
-    serializer = Serializer(Union[int, str])
-    assert serializer.dump(123) == 123
-    assert serializer.load(123) == 123
-    assert serializer.dump('123') == '123'
-    assert serializer.load('123') == '123'
-
-
-def test_load_union():
-    @dataclass
-    class Foo:
-        val: int
-
-    @dataclass
-    class Bar:
-        val: str
-
-    serializer = Serializer(Union[Foo, Bar])
-
-    assert serializer.load({'val': 123}) == Foo(val=123)
-    assert serializer.load({'val': '123'}) == Bar(val='123')
-
-
-def test_load_optional_union():
-    @dataclass
-    class Foo:
-        val: int
-
-    serializer = Serializer(Union[Foo, list[Foo], None])
-
-    assert serializer.load({'val': 123}) == Foo(val=123)
-    assert serializer.load([{'val': 1}, {'val': 2}]) == [Foo(val=1), Foo(val=2)]
-    assert serializer.load(None) is None
-
-
-def test_load_union_simple_types__invalid_type():
-    serializer = Serializer(Union[int, str])
-    with pytest.raises(SchemaValidationError) as exc_info:
-        serializer.load(123.0)
-
-    assert exc_info.value.errors == [ErrorItem(message='123.0 is not of type "Union[int, str]"', instance_path='')]
+import sys
+from dataclasses import dataclass
+from typing import Annotated, Literal, Optional, Union
+
+import pytest
+
+from serpyco_rs import Serializer, SchemaValidationError, ErrorItem
+from serpyco_rs.metadata import Discriminator
+
+
+@dataclass
+class Foo:
+    val: int
+    type: Literal['foo'] = 'foo'
+
+
+@dataclass
+class Bar:
+    type: Literal['bar']
+    val: str
+
+
+@dataclass
+class Buz:
+    type: int
+    val: str
+
+
+@dataclass
+class Buzz:
+    val: str
+
+
+@dataclass
+class Base:
+    childs: list[Annotated[Union[Foo, Bar], Discriminator('type')]]
+
+
+def test_tagged_union():
+    serializer = Serializer(Base)
+    val = Base(
+        childs=[
+            Foo(val=1),
+            Bar(type='bar', val='12'),
+        ]
+    )
+    raw = {'childs': [{'type': 'foo', 'val': 1}, {'type': 'bar', 'val': '12'}]}
+    assert serializer.dump(val) == raw
+    assert serializer.load(raw) == val
+
+
+def test_tagged_union__invalid_discriminator_type():
+    @dataclass
+    class Inner:
+        field: Annotated[Union[Foo, Bar, Buz], Discriminator('type')]
+
+    with pytest.raises(RuntimeError) as exc_info:
+        Serializer(Inner)
+
+    assert exc_info.type is RuntimeError
+    assert exc_info.value.args[0] == (
+        'Type <class \'tests.test_union.Buz\'> has invalid discriminator field "type" with type "<class \'int\'>". '
+        'Discriminator supports only Literal[<str>].'
+    )
+
+
+def test_tagged_union__union_arg_has_no_discriminator_field():
+    @dataclass
+    class Inner:
+        field: Annotated[Union[Foo, Bar, Buzz], Discriminator('type')]
+
+    with pytest.raises(RuntimeError) as exc_info:
+        Serializer(Inner)
+
+    assert exc_info.type is RuntimeError
+    assert exc_info.value.args[0] == 'Type <class \'tests.test_union.Buzz\'> does not have discriminator field "type"'
+
+
+def test_tagged_union__unsupported_types():
+    @dataclass
+    class Inner:
+        field: Annotated[Union[int, str], Discriminator('type')]
+
+    with pytest.raises(RuntimeError) as exc_info:
+        Serializer(Inner)
+
+    assert exc_info.type is RuntimeError
+    assert exc_info.value.args[0] == (
+        "Unions supported only for dataclasses or attrs. Provided: typing.Union[<class 'int'>,<class 'str'>]"
+    )
+
+
+@dataclass
+class A:
+    type: Literal['A']
+    params: int
+    children: Optional[list['ComponentsT']] = None
+
+
+@dataclass
+class B:
+    type: Literal['B']
+    params: str
+    children: Optional[list['ComponentsT']] = None
+
+
+ComponentsT = Annotated[Union[A, B], Discriminator('type')]
+
+
+@pytest.mark.skipif(sys.version_info < (3, 11), reason='requires python3.11 or higher')
+def test_tagged_union__with_forward_refs():
+    serializer = Serializer(ComponentsT, omit_none=True)
+    data: ComponentsT = A(
+        type='A',
+        params=123,
+        children=[
+            A(
+                type='A',
+                params=1234,
+            ),
+            B(
+                type='B',
+                params='foo',
+                children=[
+                    B(
+                        type='B',
+                        params='bar',
+                    )
+                ],
+            ),
+        ],
+    )
+    raw_data = {
+        'type': 'A',
+        'params': 123,
+        'children': [
+            {'params': 1234, 'type': 'A'},
+            {'children': [{'params': 'bar', 'type': 'B'}], 'params': 'foo', 'type': 'B'},
+        ],
+    }
+    assert serializer.dump(data) == raw_data
+    assert serializer.load(raw_data) == data
+
+
+def test_tagged_union__camel_case_filed_format():
+    @dataclass
+    class A:
+        discriminator_with_multiple_words: Literal['A']
+        a: int
+
+    @dataclass
+    class B:
+        discriminator_with_multiple_words: Literal['B']
+        b: str
+
+    raw_obj = [
+        {
+            'discriminatorWithMultipleWords': 'A',
+            'a': 128,
+        },
+        {
+            'discriminatorWithMultipleWords': 'B',
+            'b': 'foo',
+        },
+    ]
+    obj = [
+        A(
+            discriminator_with_multiple_words='A',
+            a=128,
+        ),
+        B(
+            discriminator_with_multiple_words='B',
+            b='foo',
+        ),
+    ]
+
+    serializer = Serializer(
+        list[Annotated[Union[A, B], Discriminator('discriminator_with_multiple_words')]],
+        camelcase_fields=True,
+    )
+
+    assert serializer.dump(obj) == raw_obj
+    assert serializer.load(raw_obj) == obj
+
+
+def test_union_simple_types():
+    serializer = Serializer(Union[int, str])
+    assert serializer.dump(123) == 123
+    assert serializer.load(123) == 123
+    assert serializer.dump('123') == '123'
+    assert serializer.load('123') == '123'
+
+
+def test_load_union():
+    @dataclass
+    class Foo:
+        val: int
+
+    @dataclass
+    class Bar:
+        val: str
+
+    serializer = Serializer(Union[Foo, Bar])
+
+    assert serializer.load({'val': 123}) == Foo(val=123)
+    assert serializer.load({'val': '123'}) == Bar(val='123')
+
+
+def test_load_optional_union():
+    @dataclass
+    class Foo:
+        val: int
+
+    serializer = Serializer(Union[Foo, list[Foo], None])
+
+    assert serializer.load({'val': 123}) == Foo(val=123)
+    assert serializer.load([{'val': 1}, {'val': 2}]) == [Foo(val=1), Foo(val=2)]
+    assert serializer.load(None) is None
+
+
+def test_load_union_simple_types__invalid_type():
+    serializer = Serializer(Union[int, str])
+    with pytest.raises(SchemaValidationError) as exc_info:
+        serializer.load(123.0)
+
+    assert exc_info.value.errors == [ErrorItem(message='123.0 is not of type "Union[int, str]"', instance_path='')]
```

### Comparing `serpyco_rs-1.7.1/Cargo.lock` & `serpyco_rs-1.8.0/Cargo.lock`

 * *Files 20% similar despite different names*

```diff
@@ -1,351 +1,351 @@
-# This file is automatically @generated by Cargo.
-# It is not intended for manual editing.
-version = 3
-
-[[package]]
-name = "atomic_refcell"
-version = "0.1.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41e67cd8309bbd06cd603a9e693a784ac2e5d1e955f11286e355089fcab3047c"
-
-[[package]]
-name = "autocfg"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
-
-[[package]]
-name = "bitflags"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "cfg-if"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
-
-[[package]]
-name = "dyn-clone"
-version = "1.0.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
-
-[[package]]
-name = "heck"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
-
-[[package]]
-name = "indoc"
-version = "2.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
-
-[[package]]
-name = "libc"
-version = "0.2.153"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
-
-[[package]]
-name = "lock_api"
-version = "0.4.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
-dependencies = [
- "autocfg",
- "scopeguard",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "once_cell"
-version = "1.19.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
-
-[[package]]
-name = "parking_lot"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
-dependencies = [
- "lock_api",
- "parking_lot_core",
-]
-
-[[package]]
-name = "parking_lot_core"
-version = "0.9.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
-dependencies = [
- "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-targets",
-]
-
-[[package]]
-name = "portable-atomic"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
-
-[[package]]
-name = "proc-macro2"
-version = "1.0.81"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
-dependencies = [
- "unicode-ident",
-]
-
-[[package]]
-name = "pyo3"
-version = "0.21.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
-dependencies = [
- "cfg-if",
- "indoc",
- "libc",
- "memoffset",
- "parking_lot",
- "portable-atomic",
- "pyo3-build-config",
- "pyo3-ffi",
- "pyo3-macros",
- "unindent",
-]
-
-[[package]]
-name = "pyo3-build-config"
-version = "0.21.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-ffi"
-version = "0.21.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
-dependencies = [
- "libc",
- "pyo3-build-config",
-]
-
-[[package]]
-name = "pyo3-macros"
-version = "0.21.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
-dependencies = [
- "proc-macro2",
- "pyo3-macros-backend",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "pyo3-macros-backend"
-version = "0.21.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
-dependencies = [
- "heck",
- "proc-macro2",
- "pyo3-build-config",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "quote"
-version = "1.0.36"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
-dependencies = [
- "proc-macro2",
-]
-
-[[package]]
-name = "redox_syscall"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
-dependencies = [
- "bitflags",
-]
-
-[[package]]
-name = "rustversion"
-version = "1.0.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
-
-[[package]]
-name = "scopeguard"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
-
-[[package]]
-name = "serpyco-rs"
-version = "1.7.1"
-dependencies = [
- "atomic_refcell",
- "cfg-if",
- "dyn-clone",
- "pyo3",
- "pyo3-build-config",
- "pyo3-ffi",
- "speedate",
- "uuid",
-]
-
-[[package]]
-name = "smallvec"
-version = "1.13.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
-
-[[package]]
-name = "speedate"
-version = "0.14.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c323c4e6fece5a5a1a2a7f726d243144cce9fbcfe3ce4d9f3c6ede726a2bc780"
-dependencies = [
- "strum",
- "strum_macros",
-]
-
-[[package]]
-name = "strum"
-version = "0.25.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
-dependencies = [
- "strum_macros",
-]
-
-[[package]]
-name = "strum_macros"
-version = "0.25.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
-dependencies = [
- "heck",
- "proc-macro2",
- "quote",
- "rustversion",
- "syn",
-]
-
-[[package]]
-name = "syn"
-version = "2.0.60"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "target-lexicon"
-version = "0.12.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
-
-[[package]]
-name = "unicode-ident"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
-
-[[package]]
-name = "unindent"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
-
-[[package]]
-name = "uuid"
-version = "1.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
-
-[[package]]
-name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
-]
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+# This file is automatically @generated by Cargo.
+# It is not intended for manual editing.
+version = 3
+
+[[package]]
+name = "atomic_refcell"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41e67cd8309bbd06cd603a9e693a784ac2e5d1e955f11286e355089fcab3047c"
+
+[[package]]
+name = "autocfg"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+
+[[package]]
+name = "bitflags"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+
+[[package]]
+name = "cfg-if"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
+
+[[package]]
+name = "dyn-clone"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
+name = "indoc"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
+name = "libc"
+version = "0.2.153"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+
+[[package]]
+name = "lock_api"
+version = "0.4.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+dependencies = [
+ "autocfg",
+ "scopeguard",
+]
+
+[[package]]
+name = "memoffset"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "once_cell"
+version = "1.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
+
+[[package]]
+name = "parking_lot"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+dependencies = [
+ "lock_api",
+ "parking_lot_core",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.9.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall",
+ "smallvec",
+ "windows-targets",
+]
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
+name = "proc-macro2"
+version = "1.0.81"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+dependencies = [
+ "unicode-ident",
+]
+
+[[package]]
+name = "pyo3"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
+dependencies = [
+ "cfg-if",
+ "indoc",
+ "libc",
+ "memoffset",
+ "parking_lot",
+ "portable-atomic",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
+]
+
+[[package]]
+name = "pyo3-macros"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
+dependencies = [
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "pyo3-macros-backend"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "pyo3-build-config",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "quote"
+version = "1.0.36"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
+dependencies = [
+ "proc-macro2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "rustversion"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
+
+[[package]]
+name = "scopeguard"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
+
+[[package]]
+name = "serpyco-rs"
+version = "1.8.0"
+dependencies = [
+ "atomic_refcell",
+ "cfg-if",
+ "dyn-clone",
+ "pyo3",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "speedate",
+ "uuid",
+]
+
+[[package]]
+name = "smallvec"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
+name = "speedate"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c323c4e6fece5a5a1a2a7f726d243144cce9fbcfe3ce4d9f3c6ede726a2bc780"
+dependencies = [
+ "strum",
+ "strum_macros",
+]
+
+[[package]]
+name = "strum"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+dependencies = [
+ "strum_macros",
+]
+
+[[package]]
+name = "strum_macros"
+version = "0.25.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "target-lexicon"
+version = "0.12.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+
+[[package]]
+name = "unicode-ident"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
+
+[[package]]
+name = "unindent"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+
+[[package]]
+name = "windows-targets"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
```

### Comparing `serpyco_rs-1.7.1/pyproject.toml` & `serpyco_rs-1.8.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = ["maturin>=1,<2"]
-build-backend = "maturin"
-
-[tool.maturin]
-python-source = "python"
-module-name = "serpyco_rs._serpyco_rs"
-
-[project]
-name = "serpyco-rs"
-repository = "https://github.com/ermakov-oleg/serpyco-rs"
-requires-python = ">=3.9"
-license = {file = "LICENSE"}
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: MacOS",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python",
-    "Programming Language :: Rust",
-]
-
-dependencies = [
-    "typing-inspect>=0.8.0",
-    "attributes-doc",
-    "typing-extensions",
-]
-
-[tool.black]
-line-length = 120
-skip-string-normalization = true
+[build-system]
+requires = ["maturin>=1,<2"]
+build-backend = "maturin"
+
+[tool.maturin]
+python-source = "python"
+module-name = "serpyco_rs._serpyco_rs"
+
+[project]
+name = "serpyco-rs"
+repository = "https://github.com/ermakov-oleg/serpyco-rs"
+requires-python = ">=3.9"
+license = {file = "LICENSE"}
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python",
+    "Programming Language :: Rust",
+]
+
+dependencies = [
+    "typing-inspect>=0.8.0",
+    "attributes-doc",
+    "typing-extensions",
+]
+
+[tool.black]
+line-length = 120
+skip-string-normalization = true
```

