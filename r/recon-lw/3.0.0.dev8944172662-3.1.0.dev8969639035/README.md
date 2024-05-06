# Comparing `tmp/recon_lw-3.0.0.dev8944172662.tar.gz` & `tmp/recon_lw-3.1.0.dev8969639035.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-3.0.0.dev8944172662.tar", last modified: Fri May  3 19:54:30 2024, max compression
+gzip compressed data, was "recon_lw-3.1.0.dev8969639035.tar", last modified: Mon May  6 13:07:58 2024, max compression
```

## Comparing `recon_lw-3.0.0.dev8944172662.tar` & `recon_lw-3.1.0.dev8969639035.tar`

### file list

```diff
@@ -1,244 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/example/
--rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/example/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 19:54:14.000000 recon_lw-3.0.0.dev8944172662/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/StateStream.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/processor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/processor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/processor/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/message_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/one_many.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/pair_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/ts_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/type/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/type/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/event_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/recon_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/adapter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/equal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/condition/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/condition/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/empty_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/any_val.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/refdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/amend_reject.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/filter_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/non_empty_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/session_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_handling_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_handling_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/
--rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/context/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/simple_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/simple_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/matching_key_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/matching_key_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/matching_key_extractor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/matching_key_extractor/separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/one_many.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/pair_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/recon_lw_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/viewer/fields_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/exec_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/issue_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/event_category/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/event_category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/event_category/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/event_category/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/error_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/field_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/match_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/category_displayer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/color_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/color_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/color_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/color_provider/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/content_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/content_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/content_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/content_provider/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/style_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/style_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/style_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/style_provider/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/types/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/matcher_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/viewer/missing_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_metadata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/recon_lw/reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:54:30.000000 recon_lw-3.0.0.dev8944172662/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-03 19:53:55.000000 recon_lw-3.0.0.dev8944172662/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/example/
+-rw-r--r--   0 runner    (1001) docker     (127)    27554 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/example/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 13:07:39.000000 recon_lw-3.1.0.dev8969639035/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/StateStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/basic_recon_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/basic_recon_event/recon_event_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/message_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/one_many.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/pair_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/ts_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/type/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/event_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/recon_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/adapter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/equal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.238317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/empty_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/any_val.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/refdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/amend_reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/filter_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/non_empty_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/session_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.242317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.246317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/one_many.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/pair_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/recon_lw_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/fields_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/exec_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/field_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/match_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.250317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/category_displayer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/color_provider/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/types/category_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/missing_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_metadata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/recon_lw/reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.234317 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-06 13:07:58.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 13:07:57.000000 recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:07:58.254317 recon_lw-3.1.0.dev8969639035/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-06 13:07:28.000000 recon_lw-3.1.0.dev8969639035/test/test_recon_ob.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `recon_lw-3.0.0.dev8944172662/PKG-INFO` & `recon_lw-3.1.0.dev8969639035/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recon_lw
-Version: 3.0.0.dev8944172662
+Version: 3.1.0.dev8969639035
 Summary: recon_lw
 Home-page: https://github.com/th2-net/recon-lw
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Recon-lw
         
@@ -321,15 +321,15 @@
         #### Match Diff
         
         ##### Match Diff Categoriser
         - **Interface**: [link](recon_lw/reporting/match_diff/categorizer/base.py)
         - **Usage**: Defines how category names should be extracted from recon events.
         
         Implementations:
-        - [BasicErrorCategoriser](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
+        - [BasicErrorCategorizer](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
           - miss left
           - miss right
           - match
           - match diff
         
         ##### Match Diff Report Viewer
         - **Implementation**: [link](recon_lw/reporting/match_diff/viewer/category_displayer.py)
@@ -368,9 +368,9 @@
         - **Usage**: Defines basic miss categories table html viewer.
         
         ## Example
         
         Example featuring main functionality of the library can be found [here](example/example.ipynb) 
         
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `recon_lw-3.0.0.dev8944172662/README.md` & `recon_lw-3.1.0.dev8969639035/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 #### Match Diff
 
 ##### Match Diff Categoriser
 - **Interface**: [link](recon_lw/reporting/match_diff/categorizer/base.py)
 - **Usage**: Defines how category names should be extracted from recon events.
 
 Implementations:
-- [BasicErrorCategoriser](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
+- [BasicErrorCategorizer](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
   - miss left
   - miss right
   - match
   - match diff
 
 ##### Match Diff Report Viewer
 - **Implementation**: [link](recon_lw/reporting/match_diff/viewer/category_displayer.py)
```

### Comparing `recon_lw-3.0.0.dev8944172662/example/example.ipynb` & `recon_lw-3.1.0.dev8969639035/example/example.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979602324867096%*

 * *Differences: {"'cells'": "{1: {'metadata': {'jupyter': OrderedDict([('outputs_hidden', False)])}}, 2: "*

 * *            "{'metadata': {'jupyter': OrderedDict([('outputs_hidden', False)])}, 'source': "*

 * *            "{insert: [(0, 'from recon_lw.interpretation.field_extractor import "*

 * *            "BasicConverterExtractor, BasicDictExtractor\\n'), (13, 'stream1_extractors_mapping = "*

 * *            '{\\n\'), (14, "    \'key1\': \'KeyField1\', # Default dictionary field '*

 * *            'extraction\\n"), (15, "    \'key2\': lambda x:  […]*

```diff
@@ -1,50 +1,67 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f1b89f0a-5a46-4bd9-b63e-83a64d52c868",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import os \n",
+                "os.chdir('..')"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "37b4ee336cf36aae",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Extractor"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7bc17082b6f68370",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
-                "from recon_lw.interpretation.field_extractor import BasicConverterExtractor\n",
+                "from recon_lw.interpretation.field_extractor import BasicConverterExtractor, BasicDictExtractor\n",
                 "from recon_lw.reporting.known_issues import Issue\n",
                 "\n",
                 "\"\"\"\n",
                 "Message example:\n",
                 "  {\n",
                 "     'KeyField1': 'KeyValue1',\n",
                 "     'KeyField2': 'KeyValue2.text',\n",
                 "     'Field1': '1000'\n",
                 "  }\n",
                 "\"\"\"\n",
                 "\n",
                 "\n",
-                "def stream1_extractors_mapping():\n",
-                "    return {\n",
-                "        'key1': 'KeyField1', # Default dictionary field extraction\n",
-                "        'key2': lambda x: x['KeyField2'].split('.'), # Lambda based field extraction\n",
-                "        'field1': BasicConverterExtractor(\n",
-                "            field_name='KeyField1',\n",
-                "            converter=lambda x, _: int(x) / 10\n",
-                "        )\n",
-                "    }\n",
+                "stream1_extractors_mapping = {\n",
+                "    'key1': 'KeyField1', # Default dictionary field extraction\n",
+                "    'key2': lambda x: x['KeyField2'].split('.'), # Lambda based field extraction\n",
+                "    'field1': BasicConverterExtractor(\n",
+                "        field_name='KeyField1',\n",
+                "        converter=lambda x, _: int(x) / 10,\n",
+                "        base_extractor=BasicDictExtractor('KeyField1')\n",
+                "    )\n",
+                "}\n",
                 "\n",
                 "\"\"\"\n",
                 "Messages example:\n",
                 "MessageType1:\n",
                 "    {\n",
                 "      'mt': 'MessageType1',\n",
                 "      'key_field_1': 'KeyValue1.text',\n",
@@ -55,80 +72,90 @@
                 "    {\n",
                 "      'mt': 'MessageType2',\n",
                 "      'key_field_1': 'KeyValue1',\n",
                 "      'key_field_2': 'KeyValue2',\n",
                 "      'field_1': '1000'\n",
                 "    }\n",
                 "\"\"\"\n",
-                "def stream2_mt1_extractors_mapping():\n",
-                "    return {\n",
-                "        'key1': lambda x: x['key_field_1'].split('.'), # Default dictionary field extraction\n",
-                "        'key2': 'key_field_2', # Default dictionary field extraction\n",
-                "        'field1': lambda x: int(x['Field1'])\n",
-                "    }\n",
+                "stream2_mt1_extractors_mapping = {\n",
+                "    'key1': lambda x: x['key_field_1'].split('.'), # Default dictionary field extraction\n",
+                "    'key2': 'key_field_2', # Default dictionary field extraction\n",
+                "    'field1': lambda x: int(x['Field1'])\n",
+                "}\n",
                 "\n",
-                "def stream2_mt2_extractors_mapping():\n",
-                "    return {\n",
-                "        'key1': 'key_field_1',\n",
-                "        'key2': 'key_field_2', # Default dictionary field extraction\n",
-                "        'field1': lambda x: int(x['Field1']) // 10\n",
-                "    }"
+                "stream2_mt2_extractors_mapping = {\n",
+                "    'key1': 'key_field_1',\n",
+                "    'key2': 'key_field_2', # Default dictionary field extraction\n",
+                "    'field1': lambda x: int(x['Field1']) // 10\n",
+                "}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8ca37ce967a523c2",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Adapters"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d7f973c93c7fc1e7",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.interpretation.adapter import SimpleAdapterBuilder, CompoundAdapter, SimpleAdapter\n",
                 "\n",
                 "# Using simple adapter with mapping\n",
                 "stream1_adapter = SimpleAdapterBuilder()\\\n",
-                "    .with_mapping(stream1_extractors_mapping())\\\n",
+                "    .with_mapping(stream1_extractors_mapping)\\\n",
                 "    .build()\n",
                 "\n",
                 "# Using compound adapter which allows to define different mapping for different message types\n",
                 "stream2_adapter = CompoundAdapter(\n",
                 "    adapters = [\n",
-                "        (lambda x, _: x['mt'] == 'MessageType1', SimpleAdapter(stream2_mt1_extractors_mapping())),\n",
-                "        (lambda x, _: x['mt'] == 'MessageType2', SimpleAdapter(stream2_mt2_extractors_mapping()))\n",
+                "        (lambda x, _: x['mt'] == 'MessageType1', SimpleAdapter(stream2_mt1_extractors_mapping)),\n",
+                "        (lambda x, _: x['mt'] == 'MessageType2', SimpleAdapter(stream2_mt2_extractors_mapping))\n",
                 "    ]\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "72653c04e455d2ea",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Messages Comparisons"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f29ee2602541e140",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.interpretation.field_checker import SimpleFieldChecker\n",
                 "from recon_lw.interpretation.check_rule import EqualFieldCheckRule, FieldToCheck\n",
                 "\n",
                 "# Defining simple equal field check rule that compares fields for equality\n",
@@ -151,40 +178,56 @@
                 "fields_checker = SimpleFieldChecker(checker_rules)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5aff6dd1204de8a",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Key Function"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7b7057a758ac1f1",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from typing import Dict, Any, Set, List, Optional\n",
                 "from recon_lw.interpretation.adapter import Adapter\n",
                 "from recon_lw.interpretation.filter import FilterChain, SessionAliasFilter\n",
                 "from recon_lw.matching.key_functions import BasicOriginalKeyFunctionProvider\n",
                 "\n",
-                "# Defining key fields that can be used to find pairs between streams\n",
+                "# Defining key fields that can be used to find pairs between streams (fields for matching)\n",
                 "\n",
                 "key_fields = {'key1', 'key2'}\n",
                 "\n",
                 "# Defining key function provider using common library\n",
-                "stream1_key_function = BasicOriginalKeyFunctionProvider(\n",
+                "\n",
+                "def stream1_key_extractor(adapter: Adapter, message: Dict[str, Any], fields: Set[str]) -> Optional[List[str]]:\n",
+                "    if message['sessionId'] != 'stream1_session_alias':\n",
+                "        return None\n",
+                "    collected_keys = []\n",
+                "    for field in fields:\n",
+                "        collected_keys.append(adapter.get(message, field))\n",
+                "    return [\":\".join(collected_keys)]\n",
+                "\n",
+                "stream1_key_function_builder = BasicOriginalKeyFunctionProvider(\n",
+                "    matching_key=stream1_key_extractor,\n",
                 "    filter_chain=FilterChain()\\\n",
                 "        .add_filter(SessionAliasFilter(whitelisted_aliases={'stream1_session_alias'})), # Filtering only message with session alias from whitelist\n",
                 "    key_fields=key_fields\n",
                 ")\n",
                 "\n",
                 "# Defining key function for stream2\n",
                 "\n",
@@ -197,30 +240,36 @@
                 "    return [\":\".join(collected_keys)]\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f853e98586a05a80",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Interpretation Function"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e81c04166110f4aa",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2024-03-19T15:03:29.770811100Z",
                     "start_time": "2024-03-19T15:03:29.580896200Z"
                 },
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.core.type.types import Message\n",
                 "from recon_lw.interpretation.interpretation_functions.event_enhancement import ReconEventChainEnhancement\n",
                 "from recon_lw.interpretation.interpretation_functions import BasicInterpretationFunctionProvider\n",
                 "\n",
@@ -244,84 +293,102 @@
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "96155f5b5b932f53",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Matching Rule Definition"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "30b35264dc0ce057",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.matching.stream_matcher.one_many import OneManyMatcher\n",
                 "from recon_lw.core.rule.one_many import OneManyRuleConfig\n",
                 "\n",
                 "# Defining OneManyRule with OneManyMatcher, key functions and interpretation functions defined above.\n",
                 "stream1_vs_stream2_rule = OneManyRuleConfig.from_defaults(\n",
                 "    name=\"stream1_vs_stream2\",\n",
                 "    horizon_delay=30,\n",
                 "    match_function=OneManyMatcher(),\n",
                 "    intepretation_function=interpretation_function.provide(),\n",
-                "    first_key_func=stream1_key_function.provide(stream1_adapter),\n",
+                "    first_key_func=stream1_key_function_builder.provide(stream1_adapter),\n",
                 "    second_key_func=stream2_key_extractor\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1ba3508f25e35bf9",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Reading data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6be4905c55da3ab2",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from th2_data_services.data import Data\n",
                 "\n",
                 "stream1_data = Data.from_json(\"data/stream1.json\")\n",
                 "stream2_data = Data.from_cache_file(\"data/stream2.pickle\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e69ebe01fb2b6459",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Clearing recon events"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e7c7810552cd36da",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "from recon_lw.recon_lw_entrypoint import execute_standalone\n",
                 "\n",
                 "# Cleaning recon events folder\n",
@@ -330,26 +397,32 @@
                 "[f.unlink() for f in local_events_folder_path.glob(\"*\") if f.is_file()]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4626972d2a01edcd",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Recon entrypoing"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ffd36297ba4600a8",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Executing previously defined rule on stream1 and stream2 data objects using rule defined above.\n",
                 "\n",
                 "execute_standalone(\n",
                 "    message_pickle_path=None,\n",
@@ -361,26 +434,32 @@
                 "print('DONE')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e5426f826b65b5bf",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Recon Context"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7e1675281c1360ed",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from th2_data_services.config import options\n",
                 "from recon_lw.reporting.recon_context.context import ReconContext\n",
                 "\n",
                 "# Defining recon context which knows how to extract fields from event and messages and also knows how to get recon events\n",
@@ -391,41 +470,50 @@
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "586e9e65acfb8e0",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# General events statistics"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2f0ee260902f4401",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.reporting.stats.stats import EventStatisticsTableReport\n",
                 "\n",
                 "# General Statistics Report Generator\n",
                 "stats = EventStatisticsTableReport(recon_context)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "293983f95ce8e62e",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Events table per event type\n",
                 "\"\"\"\n",
                 "+--------+--------------------+----------+---------+\n",
                 "|        | Event Type         | Status   |   count |\n",
@@ -447,15 +535,18 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7aed7cbcb17bd500",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Events table per event name\n",
                 "\"\"\"\n",
                 "+--------+-------------------------------------+----------+---------+\n",
                 "|        | Event Name                          | Status   |   count |\n",
@@ -476,26 +567,32 @@
                 "stats.get_event_names_report_table()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1a23189881ad6b1f",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Match Diff Categorisation and Report"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "71543f9f3797520b",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.reporting.known_issues import IssueStatus\n",
                 "from recon_lw.reporting.match_diff.categorizer.basic import BasicErrorCategoriser\n",
                 "from recon_lw.reporting.match_diff.categorizer.event_category.base import ErrorCategoryStrategy\n",
                 "from recon_lw.reporting.match_diff.categorizer.event_category.basic import BasicDiffCategoryExtractor, \\\n",
@@ -536,19 +633,22 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c44b36622bb2dd46",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
-                "from recon_lw.reporting.match_diff.viewer.content_provider.default import DefaultExampleContentProvider\n",
+                "from recon_lw.reporting.match_diff.viewer.content_provider.default import FullMessageExampleContentProvider\n",
                 "from recon_lw.reporting.match_diff.viewer.style_provider.default import DefaultErrorExamplesStyleProvider\n",
                 "from recon_lw.reporting.match_diff.viewer.color_provider.default import DefaultCategoryColorProvider\n",
                 "from recon_lw.reporting.match_diff.viewer.category_displayer import ErrorExampleDisplayer, MatchDiffViewer\n",
                 "\n",
                 "# Default Color Provider\n",
                 "color_provider = DefaultCategoryColorProvider()\n",
                 "# Non default color provider\n",
@@ -561,50 +661,58 @@
                 "    error_examples_styles_provider=DefaultErrorExamplesStyleProvider()\n",
                 ")\n",
                 "\n",
                 "# Running events categorisation\n",
                 "stats_context = categorizer.process_events(recon_context.get_recon_events())\n",
                 "\n",
                 "# Message key extractor\n",
-                "def id(x):\n",
-                "    if x['sessionId'] == 'stream1_session_alias':\n",
-                "        return stream1_key_function.provide(stream1_adapter)(x)\n",
-                "    else:\n",
-                "        return stream2_key_extractor(stream2_adapter, x, key_fields)\n",
+                "# This function returns the list of matching-keys. \n",
+                "#  e.g. ['key-field1-val:key-field2-val']\n",
+                "# def get_ord_id_to_build_order_history(x):\n",
+                "#     if x['sessionId'] == 'stream1_session_alias':\n",
+                "#         return stream1_key_function_builder.provide(stream1_adapter)(x)\n",
+                "#     else:\n",
+                "#         return stream2_key_extractor(stream2_adapter, x, key_fields)\n",
                 "\n",
                 "\n",
                 "# Defining match diff html report displayer to display categories found by categoriser\n",
                 "diff_viewer = MatchDiffViewer(\n",
                 "    recon_stats_context=stats_context,\n",
                 "    messages=stream1_adapter + stream2_adapter,\n",
                 "    data_objects=[stream1_data, stream2_data],\n",
-                "    message_business_ids_provider=id,\n",
-                "    message_content_provider=DefaultExampleContentProvider(),\n",
+                "    # message_business_ids_provider=get_ord_id_to_build_order_history,\n",
+                "    message_content_provider=FullMessageExampleContentProvider(),\n",
                 "    recon_context=recon_context,\n",
                 "    error_example_displayer=example_displayer\n",
                 ")\n",
                 "diff_viewer.display_report()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "625c468dbe0e7fdd",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Static misses categorisation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9edc57cdfb3fe282",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "from recon_lw.reporting.missing_messages.viewer.missing_message import MissingMessagesDisplayer\n",
                 "from recon_lw.reporting.missing_messages.categorizer.matchers_impl import SimpleMatcherFlat\n",
                 "from recon_lw.reporting.known_issues import Issue, IssueStatus\n",
                 "from recon_lw.reporting.missing_messages.categorizer.rule import MissCategorizationRule\n",
@@ -640,26 +748,32 @@
                 "report.display(messages)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f1779b619eb22084",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "source": [
                 "# Dynamic misses and match diffs categorisation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1bbdcc1b81bdf82b",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "def miss_orig_event_category(event) -> str:\n",
                 "    message = event['body']['messages'][0]\n",
                 "    return f'stream1 missing messages with key field {message[\"key_field_1\"]} and \"field1\" {message[\"field1\"]}'\n",
                 "\n",
@@ -675,15 +789,18 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8a35b20696a15726",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Displaing miss orig categories\n",
                 "from th2_data_services.utils.event_utils.totals import get_category_totals2\n",
                 "from th2_data_services.utils.category import Category\n",
                 "categories = [\n",
@@ -695,15 +812,18 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "732d933dc6da12e4",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Displaing miss copy categories\n",
                 "categories = [\n",
                 "    Category(\"recon_name\", lambda e: e['recon_name']),\n",
                 "    Category(\"type\", lambda e: e['eventType']),\n",
@@ -713,15 +833,18 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd5e30d51177d444",
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Displaing match diff categories\n",
                 "categories = [\n",
                 "    Category(\"recon_name\", lambda e: e['recon_name']),\n",
                 "    Category(\"type\", lambda e: e['eventType']),\n",
@@ -729,27 +852,27 @@
                 "]\n",
                 "get_category_totals2(recon_context.get_recon_events().filter(lambda e: e['eventType'] == 'BasicReconMatch' and not e['successful']), categories)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython3",
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/EventsSaver.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/SequenceCache.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/StateStream.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/StateStream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/cache/processor/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/cache/processor/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/message_utils.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/message_utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
-from recon_lw.core.EventsSaver import EventsSaver
+from recon_lw.core.EventsSaver import IEventsSaver
 from recon_lw.matching.init_function import AbstractMatcherContext
 
 
 class RuleContext:
     def __init__(self,
                  rule_root_event: dict,
-                 event_saver: EventsSaver,
+                 event_saver: IEventsSaver,
                  event_sequence: Dict[str, Any]
                  ):
         self.rule_root_event = rule_root_event
         self.event_saver = event_saver
         self.event_sequence = event_sequence
 
     @staticmethod
     def from_dict(rule_context: dict):
         return RuleContext(
             rule_context['events_saver'],
             rule_context['event_sequence'],
             rule_context['event']
         )
 
+
 class AbstractRule(ABC):
 
     def __init__(self):
         self.horizon_delay = None
         self.collect_func = None
         self.flush_func = None
 
@@ -39,15 +40,15 @@
 
     def set_rule_context(self, context: RuleContext):
         self.rule_context = context
 
     def get_root_event(self) -> Dict[str, Any]:
         return self.rule_context.rule_root_event
 
-    def get_event_saver(self) -> EventsSaver:
+    def get_event_saver(self) -> IEventsSaver:
         return self.rule_context.event_saver
 
     def get_event_sequence(self) -> Dict[str, Any]:
         return self.rule_context.event_sequence
 
     @abstractmethod
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/one_many.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/one_many.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/rule/pair_one.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/rule/pair_one.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/stream.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/ts_converters.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/ts_converters.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/core/utility/recon_utils.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/core/utility/recon_utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/adapter_context.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/adapter_context.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/compound.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/compound.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
 from recon_lw.interpretation.condition.base import Condition
 from recon_lw.interpretation.adapter.base import Adapter
-from typing import List, Optional, Tuple, Dict
+from typing import List, Optional, Tuple, Dict, Any
 
-from recon_lw.interpretation.field_extractor import Extractor
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from recon_lw.interpretation.field_extractor import Extractor
 
 
 class CompoundAdapter(Adapter):
     """
         A compound adapter composed of multiple adapters with associated conditions.
 
         This adapter selects the appropriate adapter based on conditions and delegates
@@ -49,14 +52,23 @@
         handler = self.get_adapter(m)
         return handler.on_message_exit(m)
 
     def get_fields_group(self, m, group_name):
         handler = self.get_adapter(m)
         return handler.get_fields_group(m, group_name)
 
+    def get_root_message_field(self, message, parameter_name,
+                               strict=False) -> Any:
+        # FIXME: Not implemented
+        pass
+
+    def get_metadata_field(self, message, field_name, strict=False) -> Any:
+        # FIXME: Not implemented
+        pass
+
 
 class CompoundAdapterBuilder:
     """
     A builder class for constructing instances of the CompoundAdapter class.
 
     Attributes:
         _conditions_and_adapters (List[Tuple[Condition, Adapter]]): A list of tuples
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/adapter/simple.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/adapter/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import List, Optional, Dict, Union
 
 from recon_lw.interpretation.adapter.base import Adapter
 from recon_lw.interpretation.field_extractor.base import Extractor, ExtractorProtocol
 
 
 class SimpleAdapter(Adapter):
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/adapter.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/adapter.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/check_result.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/check_result.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/check_rule/equal.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/check_rule/equal.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/condition/function.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/condition/function.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/__init__.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/boolean.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/boolean.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/chain.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/condition.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/condition.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/datetime.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/datetime.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/dictionary.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/dictionary.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/list.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/list.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/mapping.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/mapping.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/converter/type.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/converter/type.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_checker/simple.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_checker/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/any_val.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/any_val.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-from recon_lw.interpretation.adapter.base import Adapter
+from __future__ import annotations
 from recon_lw.core.type.types import Message
 from typing import Optional, Any, Protocol, runtime_checkable
-from abc import ABC, abstractmethod
+from abc import ABC
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from recon_lw.interpretation.adapter.base import Adapter
+
 
 class Extractor(ABC):
     """
     An abstract base class for all extractors.
     """
     NOT_EXTRACTED = "_NE_"
 
@@ -14,10 +20,11 @@
 
     def __call__(self, message: Message, adapter: Adapter) -> Optional[Any]:
         return self.extract(message, adapter)
 
     def extract(self, message: Message, adapter: Adapter) -> Optional[Any]:
         pass
 
+
 class ExtractorProtocol(Protocol):
     def __call__(self, message: Message, adapter: Adapter):
-        pass
+        pass
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/cache.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/cache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/concat.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/concat.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/condition.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/condition.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/dictionary.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/dictionary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 from recon_lw.interpretation.field_extractor.base import Extractor
 from recon_lw.interpretation.adapter.base import Adapter
 from typing import Optional
 from recon_lw.core.type.types import Message
 
 
 class BasicDictExtractor(Extractor):
-    def __init__(self, field_name: str, default_value: str = None, strip: bool = False, cast_to_str: bool = True):
+    def __init__(self, field_name: str, default_value: str = None,
+                 strip: bool = False, cast_to_str: bool = True):
         super().__init__(field_name)
         self.strip = strip
         self.default_value = default_value
         self.cast_to_str = cast_to_str
 
     def extract(self, message: Message, adapter: Adapter) -> Optional[str]:
-        val = message.get(self.field_name, self.default_value if self.default_value else Extractor.NOT_EXTRACTED)
+        val = message.get(self.field_name,
+                          self.default_value if self.default_value else Extractor.NOT_EXTRACTED)
         if self.cast_to_str:
             val = str(val)
             if self.strip:
                 val = val.strip()
 
         return val
-
-
-class BasicDictExtractorBuilder:
-    def __init__(self):
-        self.field_name = ""
-
-    def set_field_name(self, field_name: str) -> 'BasicDictExtractorBuilder':
-        self.field_name = field_name
-        return self
-
-    def set_strip(self, strip: bool) -> 'BasicDictExtractorBuilder':
-        self.strip = strip
-        return self
-
-    def build(self) -> BasicDictExtractor:
-        if not self.field_name:
-            raise ValueError("Field name must be set.")
-        return BasicDictExtractor(self.field_name)
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/list.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/list.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/one_of.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/one_of.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/field_extractor/refdata.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/field_extractor/refdata.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/amend_reject.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/amend_reject.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/field.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/field.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/filter_chain.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/filter_chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/filter/non_empty_field.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/filter/non_empty_field.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_enhancement/enhancement_chain.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_handling_strategy/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,11 @@
     def get_match_event_name(self):
         pass
 
     @abstractmethod
     def get_match_diff_event_name(self):
         pass
 
+
 class ReconEventNameProviderProtocol(Protocol):
-    def __call__(self, event_type: ReconType, successful: bool=True):
-        pass
+    def __call__(self, event_type: ReconType, successful: bool = True):
+        pass
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/interpretation_functions/event_name_provider/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     def get_miss_copy_event_name(self):
         return f"{self.event_name_prefix}[miss_copy]"
 
     def get_match_event_name(self):
         return f"{self.event_name_prefix}[match]"
 
     def get_match_diff_event_name(self):
-        return f"{self.event_name_prefix}[match[diff_found]]"
+        return f"{self.event_name_prefix}[match][diff_found]"
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/interpretation/recon_ob_stats.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/interpretation/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/LastStateMatcher.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/LiveObjectsCache.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/StateSequenceGenerator.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/TimeCacheMatcher.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/collect_matcher/default.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/collect_matcher/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/base.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/flush_function/default.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/flush_function/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/context/simple.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/context/simple.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/init_function/default.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/init_function/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/default.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/key_functions/simple_copy.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/key_functions/simple_copy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from recon_lw.matching.key_functions.base import KeyFunctionProvider
-from recon_lw.interpretation.filter import FilterChain, Filter
-from recon_lw.matching.matching_key_extractor import BasicSeparatorMatchingKeyExtractor
-from recon_lw.matching.matching_key_extractor.base import MatchingKeyExtractor, MatchingKeyExtractorProtocol
+from recon_lw.interpretation.filter import FilterChain
+from recon_lw.matching.matching_key_extractor.base import IMatchingKeyExtractor, \
+    MatchingKeyExtractorProtocol
 from typing import Set, List
 from recon_lw.interpretation.adapter.base import Adapter
 from recon_lw.core.type.types import KeyFunctionType, Message
 
+
 class BasicCopyKeyFunctionProvider(KeyFunctionProvider):
 
-    def __init__(self, filter_chain: FilterChain, matching_key: MatchingKeyExtractorProtocol, key_fields: Set[str]):
+    def __init__(self, filter_chain: FilterChain,
+                 matching_key: MatchingKeyExtractorProtocol,
+                 key_fields: Set[str]):
         super().__init__()
         self._filter_chain = filter_chain
         self._matching_key = matching_key
         self._key_fields = key_fields
 
     def provide(self, adapter: Adapter) -> KeyFunctionType:
         def key_function(message: Message):
@@ -21,9 +24,8 @@
                 mks = self._matching_key(adapter, message, self._key_fields)
                 if len(mks) > 1:
                     raise SystemError(
                         f"Copy matching fun can have only single value, received {mks}"
                     )
                 return mks[0]
 
-
-        return key_function
+        return key_function
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/matching_key_extractor/separator.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/matching_key_extractor/separator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import Any, Dict, Set, List
-from recon_lw.matching.matching_key_extractor.base import MatchingKeyExtractor
+from recon_lw.matching.matching_key_extractor.base import IMatchingKeyExtractor
 
 from recon_lw.interpretation.adapter.base import Adapter
 
 
-class BasicSeparatorMatchingKeyExtractor(MatchingKeyExtractor):
+class BasicSeparatorMatchingKeyExtractor(IMatchingKeyExtractor):
 
     def __init__(self, separator: str):
         self.separator = separator
 
     def extract(self, adapter: Adapter, message: Dict[str, Any], fields: Set[str]) -> List[str]:
         def scale_item(val, count):
             if len(val) == count:
                 for x in val:
                     yield x
             else:
                 v = val[0]
                 for _ in range(count):
                     yield v
 
-        result = []
         items = {}
         max_count = 1
         for field in fields:
             val = adapter.get(message, field, strict=True)
             if not isinstance(val, list):
                 val = [val]
             items[field] = val
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/matching.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/matching.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/old/utils.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/old/utils.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_ob.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_ob_cross_stream.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/recon_oe_ob.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/one_many.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/one_many.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/matching/stream_matcher/pair_one.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/matching/stream_matcher/pair_one.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/recon_lw_entrypoint.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/recon_lw_entrypoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from recon_lw.core.EventsSaver import EventsSaver
+from recon_lw.core.EventsSaver import EventsSaver, IEventsSaver
 from typing import Union, Callable, Any
 
 from recon_lw.core.rule import AbstractRule
 from recon_lw.core.rule.base import RuleContext
 from recon_lw.matching.collect_matcher import CollectMatcher
 
 from recon_lw.core.utility import *
 from recon_lw.matching.flush_function import FlushFunction
 from recon_lw.matching.old.matching import init_matcher, collect_matcher, flush_matcher
 
 
-def execute_standalone(message_pickle_path, sessions_list, result_events_path,
-                       rules: Dict[str, Dict[str, Union[Dict[str, Any], AbstractRule]]],
-                       data_objects=None,
-                       buffer_len=100):
+def execute_standalone(
+        message_pickle_path,
+        sessions_list,
+        result_events_path,
+        rules: Dict[str, Dict[str, Union[Dict[str, Any], AbstractRule]]],
+        data_objects=None,
+        buffer_len=100,
+        events_saver: Optional[IEventsSaver] = None,
+):
     """Entrypoint for recon-lw.
 
     It generates ReconEvents and stores them in the `result_events_path` file
     to disc in pickle format.
 
     It matches messages 1 to 1 or 1 to many  (depends on `rule_match_func` param
     in the config).
@@ -36,15 +41,16 @@
         rules_settings_dict: { ReconRuleName: {}, ... }
         data_objects:
 
     Returns:
 
     """
     box_ts = datetime.now()
-    events_saver = EventsSaver(result_events_path)
+    if events_saver is None:
+        events_saver = EventsSaver(result_events_path)
 
     event_sequence = EventSequence(name="recon_lw", timestamp=str(box_ts.timestamp()), n=0).to_dict()
     root_event = create_event("recon_lw " + box_ts.isoformat(), "Microservice", event_sequence)
 
     events_saver.save_events([root_event])
     new_rules_settings_dict = {}
     for rule_key, rule_settings in rules.items():
@@ -116,34 +122,38 @@
             )
         else:
             rule_settings["flush_func"](None, rule_settings, event_sequence,
                                         lambda ev_batch: events_saver.save_events(ev_batch))
     # one final flush
     events_saver.flush()
 
+    # TODO
+    #   Probably It's a good idea to return ReconContext here.
+
+
 def preprocess_rule_config_object(
     rule_key: str,
     event_sequence: dict,
     root_event: dict,
     rule: AbstractRule,
-    events_saver: EventsSaver
+    events_saver: IEventsSaver
 ) -> AbstractRule:
     rule_root_event = create_event(rule_key, "LwReconRule",
                                    event_sequence,
                                    parentId=root_event["eventId"])
 
     rule.set_rule_context(RuleContext(rule_root_event, events_saver, event_sequence))
     return rule
 
 def preprocess_rule_config_dict(
     rule_key: str,
     event_sequence: dict,
     root_event: dict,
     rule: dict,
-    events_saver: EventsSaver
+    events_saver: IEventsSaver
 ) -> dict:
     rule_root_event = create_event(rule_key, "LwReconRule",
                                    event_sequence,
                                    parentId=root_event["eventId"])
 
     rule["rule_root_event"] = rule_root_event
     rule["events_saver"] = events_saver
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/coverage/viewer/fields_viewer.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/coverage/viewer/fields_viewer.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/known_issues/issue.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/known_issues/issue.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,26 +5,38 @@
 from recon_lw.reporting.match_diff.categorizer.types import ErrorCategoriesStats
 from recon_lw.reporting.match_diff.categorizer.types.error_examples import ErrorExamples
 from recon_lw.reporting.match_diff.categorizer.types import ProblemFields
 from recon_lw.reporting.match_diff.categorizer.types import MatchesStats
 
 
 class IErrorCategorizer(ABC):
-    def __init__(self):
-        self._error_stats = ErrorCategoriesStats()
-        self._matches_stats = MatchesStats()
-        self._problem_fields = ProblemFields()
-        self._error_examples = ErrorExamples()
+    def __init__(
+            self,
+            error_stats=ErrorCategoriesStats(),
+            matches_stats=MatchesStats(),
+            problem_fields=ProblemFields(),
+            error_examples=ErrorExamples(),
+    ):
+        self._error_stats = error_stats
+        self._matches_stats = matches_stats
+        self._problem_fields = problem_fields
+        self._error_examples = error_examples
 
     def process_events(self, events: List[dict]) -> ReconErrorStatsContext:
         for event in events:
             self.process_event(event)
         return ReconErrorStatsContext(
             error_examples=self._error_examples,
             error_stats=self._error_stats,
             problem_fields=self._problem_fields,
             matches_stats=self._matches_stats
         )
 
     @abstractmethod
     def process_event(self, event: dict):
-        pass
+        """It expects that this function will collect metadata and store it to:
+             - self._error_stats
+             - self._matches_stats
+             - self._problem_fields
+             - self._error_examples
+            """
+        pass
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/basic.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,49 @@
+from collections import defaultdict
+from io import FileIO
+
 from recon_lw.interpretation.interpretation_functions import ReconType
-from recon_lw.reporting.match_diff.categorizer.base import IErrorCategorizer
-from recon_lw.reporting.match_diff.categorizer.event_category.base import ErrorCategoryStrategy
+from recon_lw.reporting.missing_messages.categorizer.matcher_interface import MissCategorizer
 from recon_lw.reporting.recon_context.context import ReconContext
 
 
-class BasicErrorCategoriser(IErrorCategorizer):
-    def __init__(
-            self,
-            error_extractor_strategy: ErrorCategoryStrategy,
-            recon_context: ReconContext
-    ):
-        super().__init__()
-        self.error_extractor_strategy = error_extractor_strategy
+class MissedMessageHandler:
+    def __init__(self,
+                 recon_context: ReconContext,
+                 miss_categoriser: MissCategorizer):
+        self.recon_context = recon_context
         self.efr = recon_context.get_efr()
-        self.mfr = recon_context.get_mft()
+        self.mfr = recon_context.get_mfr()
+        self.miss_categoriser = miss_categoriser
 
+    def write_to_file(self, file: FileIO):
+        for e in self.recon_context.get_recon_events():
+            if self.efr.get_status(e):
+                continue
+            type = self.efr.get_type(e)
+            recon_name = e['reconName']
+            attached = e["attachedMessageIds"]
+            if type == ReconType.BasicReconMissLeft.value:
+                print("\t\t NO_ORIG", recon_name, attached, e['body']['key'], file)
+            elif type == ReconType.BasicReconMissRight.value:
+                print("\t\t NO_COPY", recon_name, attached, e['body']['key'], file)
+
+    def categorise_and_filter(self, messages):
+        missed_message_ids = {}
+        error_categories = defaultdict(int)
+        for e in self.recon_context.get_recon_events():
+            if self.efr.get_status(e):
+                continue
+            type = self.efr.get_type(e)
+            recon_name = e['recon_name']
+            attached = e["attachedMessageIds"]
+            if type == ReconType.BasicReconMissLeft.value:
+                error_kind = f"no_orig {recon_name}"
+            elif type == ReconType.BasicReconMissRight.value:
+                error_kind = f"no_copy {recon_name}"
+            else:
+                error_kind = None
+            if error_kind:
+                missed_message_ids[attached[0]] = error_kind
+                error_categories[(error_kind,) + self.miss_categoriser(error_kind, e)] += 1
+        return messages.filter(lambda m: m['messageId'] in missed_message_ids), error_categories
 
-    def process_event(
-            self,
-            event: dict,
-    ):
-        e = event
-        etype = self.efr.get_type(event)
-        status = self.efr.get_status(event)
-        recon_name = event["recon_name"]
-        body = event["body"]
-        body = body if body is not None else {}
-        is_match = etype == ReconType.BasicReconMatch.value
-        is_diff = body.get('diff') is not None
-
-        if is_match and not is_diff:
-            try:
-                orig, copy = self.efr.get_attached_messages_ids(event)
-            except ValueError:
-                # TODO: what to do with multimatches
-                return
-
-            if orig and copy:
-                category = self.error_extractor_strategy.match_extractor(recon_name, orig, copy, event)
-                recon_name = f"{recon_name} | [{category.name}]"
-
-            self._matches_stats.add_match(recon_name)
-
-        if is_match and is_diff:
-            try:
-                orig, copy = self.efr.get_attached_messages_ids(event)
-            except ValueError:
-                # TODO: what to do with multimatches
-                return
-
-            if orig and copy:
-                category = self.error_extractor_strategy.match_diff_extractor(recon_name, orig, copy, event)
-                recon_name = f"{recon_name} | [{category.name}]"
-
-            for diff in event['body']['diff']:
-                category = self.error_extractor_strategy.diff_category_extractor(recon_name, diff, event)
-                if not category:
-                    continue
-
-                field = diff["field_name"]
-                self._problem_fields.add_problem_field(recon_name, field)
-                self._error_stats.add_error_category(recon_name, category)
-                self._error_examples.add_error_example(recon_name, category, event['attachedMessageIds'])
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/event_category/base.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/event_category/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from typing import Protocol
 
 
 @dataclass(frozen=True)
 class EventCategory:
     name: str
 
+
 class IEventCategoryExtractor(ABC):
 
     def __call__(self, recon_name: str, orig, copy, event: dict) -> EventCategory:
         return self.extract_category(recon_name, orig, copy, event)
 
     @abstractmethod
     def extract_category(self, recon_name: str, orig, copy, event: dict) -> EventCategory:
         pass
 
+
 class IEventCategoryExtractorProtocol(Protocol):
-    def __call__(self, recon_name: str, orig, copy, event: dict):
+    def __call__(self, recon_name: str, orig, copy, event: dict) -> EventCategory:
         pass
 
+
 class IDiffCategoryExtractor(ABC):
     def __call__(self, recon_name: str, diff: dict, event: dict) -> EventCategory:
         return self.extract_category(recon_name, diff, event)
 
     @abstractmethod
     def extract_category(self, recon_name: str, diff: dict, event: dict) -> EventCategory:
         pass
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/context.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/context.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_categories_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/error_examples.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/error_examples.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 from collections import defaultdict
-from typing import Optional, List
+from typing import Optional, List, Dict
 
 from recon_lw.reporting.match_diff.categorizer.event_category import EventCategory
 
 
+recon_err_example_T = Dict[EventCategory, List[List[str]]]
+examples_T = Dict[str, recon_err_example_T]
+
+
 class ErrorExamples:
-    def __init__(self, category_example_limit=5):
-        self._error_examples = defaultdict(lambda: defaultdict(list))
+    def __init__(self, category_example_limit: int = 5):
+        """
+        Contains message Ids of error examples.
+
+        Args:
+            category_example_limit: The number of collected examples for every
+                category is limited by this parameter.
+        """
+        self._error_examples: examples_T = defaultdict(lambda: defaultdict(list))
         self.category_example_limit = category_example_limit
-        self._error_ids = []
+        self._error_ids = set()
 
-    def add_error_example(self, recon_name: str, error_category: EventCategory, attached_ids: Optional[List[str]]):
+    def add_error_example(self,
+                          recon_name: str,
+                          error_category: EventCategory,
+                          attached_ids: Optional[List[str]]):
         if attached_ids is not None:
             n = len(self._error_examples[recon_name][error_category])
             if n < self.category_example_limit:
                 self._error_examples[recon_name][error_category].append(attached_ids)
                 for attached_id in attached_ids:
-                    self._error_ids.append(attached_id)
+                    self._error_ids.add(attached_id)
 
     def is_id_affected(self, message_id):
         return message_id in self._error_ids
 
     def get_affected_recons(self):
         return self._error_examples.keys()
 
-    def get_examples(self, recon_name) -> dict:
-        return self._error_examples[recon_name]
+    def get_examples(self, recon_name) -> recon_err_example_T:
+        """Returns {EventCategory: [ [id1, id2], [id3, id4, id5], ... ]}"""
+        return self._error_examples[recon_name]
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/categorizer/types/field_problems.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/categorizer/types/field_problems.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/style_provider/default.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/style_provider/default.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/match_diff/viewer/utils.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/match_diff/viewer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,47 @@
-from typing import List, Callable
+from typing import List, Callable, Dict
 
 from th2_data_services.data import Data
 from th2_data_services.utils.converters import Th2TimestampConverter
 
 from recon_lw.core.type.types import Message
 
 from th2_data_services.config import options as o
 
 
-def get_group_data_map(datas_list: List[Data], default: str):
+def get_group_data_map(datas_list: List[Data], default: str) -> Dict[str, Data]:
+    """
+
+    Args:
+        datas_list:
+        default:
+
+    Returns:
+        {group-name: Data object}
+
+    """
     return {do.metadata.get('group', default): do for do in datas_list}
 
-def get_msgs_by_id(data: Data, ids: list, id_function: Callable[[Message], List[str]]):
+
+def get_msgs_by_id(data: Data, ids: list,
+                   id_function: Callable[[Message], List[str]]):
     ids = set(ids)
 
     res = []
     for m in data:
         m_ids = id_function(m)
         for id in m_ids:
             if id in ids:
                 res.append(m)
     return res
 
+
 def get_group_from_id(msg_id: str):
     return msg_id.split(':', 2)[1]
 
+
 def get_timestamp_ns(m):
     return Th2TimestampConverter.to_microseconds(o.emfr.get_timestamp(m))
 
+
 def sort_msgs_by_th2_timestamp(msgs: List[Message]):
-    return sorted(msgs, key=get_timestamp_ns)
+    return sorted(msgs, key=get_timestamp_ns)
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/categorizer/matchers_impl.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/missing_messages/viewer/missing_message.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/missing_messages/viewer/missing_message.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/recon_context/context.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/recon_context/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 from typing import Dict
 
-from th2_data_services.data_source.lwdp.resolver import MessageFieldResolver, EventFieldResolver
-
-from recon_lw.interpretation.interpretation_functions import ReconType
+from th2_data_services.data import Data
+from th2_data_services.interfaces.utils import resolver as i_resolver
 from recon_lw.reporting.recon_metadata.base import ReconMetadata
 from recon_lw.reporting.utils import get_recon_events
 
 
 class ReconContext:
+    # TODO
+    #   This class, probably, can be used not only by reporting, but by the
+    #   whole framework.
     def __init__(self,
                  recon_events_directory: str,
-                 message_fields_resolver: MessageFieldResolver,
-                 event_fields_resolver: EventFieldResolver
-    ):
+                 message_fields_resolver: i_resolver.MessageFieldResolver,
+                 event_fields_resolver: i_resolver.EventFieldResolver
+                 ):
+        """
+
+        Args:
+            recon_events_directory: Recon results directory.
+                The path to folder with .pickle files.
+            message_fields_resolver:
+            event_fields_resolver:
+        """
         self.recon_events_directory = recon_events_directory
         self._recons_metadata = {}
         self._recon_events: Dict[str, ReconMetadata] = None
-        self.mft = message_fields_resolver
-        self.eft = event_fields_resolver
+        self.mfr = message_fields_resolver
+        self.efr = event_fields_resolver
 
     def get_efr(self):
-        return self.eft
+        return self.efr
 
-    def get_mft(self):
-        return self.mft
+    def get_mfr(self):
+        return self.mfr
 
-    def get_recon_events(self, update_cache: bool = False):
+    def get_recon_events(self, update_cache: bool = False) -> Data:
         if self._recon_events and not update_cache:
             return self._recon_events
         self._recon_events = get_recon_events(self.recon_events_directory)
         return self._recon_events
 
-
     def update_recon_metadata(self, recon_metadata: ReconMetadata):
         self._recons_metadata[recon_metadata.recon_name] = recon_metadata
 
-    def get_metadata(self)-> Dict[str, ReconMetadata]:
-        return self._recons_metadata
+    def get_metadata(self) -> Dict[str, ReconMetadata]:
+        return self._recons_metadata
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw/reporting/stats/stats.py` & `recon_lw-3.1.0.dev8969639035/recon_lw/reporting/stats/stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/PKG-INFO` & `recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recon-lw
-Version: 3.0.0.dev8944172662
+Version: 3.1.0.dev8969639035
 Summary: recon_lw
 Home-page: https://github.com/th2-net/recon-lw
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Recon-lw
         
@@ -321,15 +321,15 @@
         #### Match Diff
         
         ##### Match Diff Categoriser
         - **Interface**: [link](recon_lw/reporting/match_diff/categorizer/base.py)
         - **Usage**: Defines how category names should be extracted from recon events.
         
         Implementations:
-        - [BasicErrorCategoriser](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
+        - [BasicErrorCategorizer](recon_lw/reporting/match_diff/categorizer/basic.py) - describes simple error categoriser which collects categories basing on [category extractor strategy](recon_lw/reporting/match_diff/categorizer/event_category/base.py) which desribes the way to extract category name for different event types:
           - miss left
           - miss right
           - match
           - match diff
         
         ##### Match Diff Report Viewer
         - **Implementation**: [link](recon_lw/reporting/match_diff/viewer/category_displayer.py)
@@ -368,9 +368,9 @@
         - **Usage**: Defines basic miss categories table html viewer.
         
         ## Example
         
         Example featuring main functionality of the library can be found [here](example/example.ipynb) 
         
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `recon_lw-3.0.0.dev8944172662/recon_lw.egg-info/SOURCES.txt` & `recon_lw-3.1.0.dev8969639035/recon_lw.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 recon_lw/core/SequenceCache.py
 recon_lw/core/StateStream.py
 recon_lw/core/__init__.py
 recon_lw/core/_types.py
 recon_lw/core/message_utils.py
 recon_lw/core/stream.py
 recon_lw/core/ts_converters.py
+recon_lw/core/basic_recon_event/__init__.py
+recon_lw/core/basic_recon_event/basic_recon_event.py
+recon_lw/core/basic_recon_event/event_type.py
+recon_lw/core/basic_recon_event/recon_event_diff.py
 recon_lw/core/cache/__init__.py
 recon_lw/core/cache/processor/__init__.py
 recon_lw/core/cache/processor/base.py
 recon_lw/core/cache/processor/chain.py
 recon_lw/core/rule/__init__.py
 recon_lw/core/rule/base.py
 recon_lw/core/rule/one_many.py
@@ -163,19 +167,20 @@
 recon_lw/reporting/match_diff/viewer/utils.py
 recon_lw/reporting/match_diff/viewer/color_provider/__init__.py
 recon_lw/reporting/match_diff/viewer/color_provider/base.py
 recon_lw/reporting/match_diff/viewer/color_provider/default.py
 recon_lw/reporting/match_diff/viewer/content_provider/__init__.py
 recon_lw/reporting/match_diff/viewer/content_provider/base.py
 recon_lw/reporting/match_diff/viewer/content_provider/default.py
+recon_lw/reporting/match_diff/viewer/content_provider/er_history_provider.py
 recon_lw/reporting/match_diff/viewer/style_provider/__init__.py
 recon_lw/reporting/match_diff/viewer/style_provider/base.py
 recon_lw/reporting/match_diff/viewer/style_provider/default.py
 recon_lw/reporting/match_diff/viewer/types/__init__.py
-recon_lw/reporting/match_diff/viewer/types/types.py
+recon_lw/reporting/match_diff/viewer/types/category_table_view.py
 recon_lw/reporting/missing_messages/__init__.py
 recon_lw/reporting/missing_messages/utils.py
 recon_lw/reporting/missing_messages/categorizer/__init__.py
 recon_lw/reporting/missing_messages/categorizer/categorizer_impl.py
 recon_lw/reporting/missing_messages/categorizer/matcher_interface.py
 recon_lw/reporting/missing_messages/categorizer/matchers_impl.py
 recon_lw/reporting/missing_messages/categorizer/rule.py
```

### Comparing `recon_lw-3.0.0.dev8944172662/setup.py` & `recon_lw-3.1.0.dev8969639035/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     description=package_name,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="TH2-devs",
     author_email="th2-devs@exactprosystems.com",
     url="https://github.com/th2-net/recon-lw",
     license="Apache License 2.0",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=requirements,
     packages=find_packages(include=["recon_lw*"]),
     include_package_data=True,
 )
```

### Comparing `recon_lw-3.0.0.dev8944172662/test/test_recon_ob.py` & `recon_lw-3.1.0.dev8969639035/test/test_recon_ob.py`

 * *Files identical despite different names*

