# Comparing `tmp/ast_grep_py-0.21.3.tar.gz` & `tmp/ast_grep_py-0.21.4.tar.gz`

## Comparing `ast_grep_py-0.21.3.tar` & `ast_grep_py-0.21.4.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0     1001      127     2219 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1142 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13416 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3410 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2157 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/swift.rs
--rw-r--r--   0     1001      127      683 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     6091 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5213 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     7993 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    17323 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     7584 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    18996 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5226 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    16017 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    12633 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127    10865 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    10708 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127      693 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    15102 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    15050 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17980 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/traversal.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7731 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61091 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/Cargo.lock
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/pyproject.toml
--rw-r--r--   0     1001      127     1933 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1356 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1459 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/PKG-INFO
+-rw-r--r--   0     1001      127     2219 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1142 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13416 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3410 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2157 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/language/src/swift.rs
+-rw-r--r--   0     1001      127      693 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15050 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    17980 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/core/src/traversal.rs
+-rw-r--r--   0     1001      127      683 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     8074 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5244 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     8987 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    17978 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     8432 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    19521 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5481 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    17934 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    13810 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127     3341 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    11131 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127    11870 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/config/src/transform/transformation.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61091 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/Cargo.lock
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/pyproject.toml
+-rw-r--r--   0     1001      127     1933 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1356 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1459 2024-05-06 21:11:30.000000 ast_grep_py-0.21.4/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.21.4/PKG-INFO
```

### Comparing `ast_grep_py-0.21.3/crates/language/Cargo.toml` & `ast_grep_py-0.21.4/crates/language/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/bash.rs` & `ast_grep_py-0.21.4/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/cpp.rs` & `ast_grep_py-0.21.4/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/csharp.rs` & `ast_grep_py-0.21.4/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/css.rs` & `ast_grep_py-0.21.4/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/elixir.rs` & `ast_grep_py-0.21.4/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/go.rs` & `ast_grep_py-0.21.4/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/html.rs` & `ast_grep_py-0.21.4/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/json.rs` & `ast_grep_py-0.21.4/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/kotlin.rs` & `ast_grep_py-0.21.4/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/lib.rs` & `ast_grep_py-0.21.4/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/lua.rs` & `ast_grep_py-0.21.4/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/parsers.rs` & `ast_grep_py-0.21.4/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/python.rs` & `ast_grep_py-0.21.4/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/ruby.rs` & `ast_grep_py-0.21.4/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/rust.rs` & `ast_grep_py-0.21.4/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/scala.rs` & `ast_grep_py-0.21.4/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/language/src/swift.rs` & `ast_grep_py-0.21.4/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/Cargo.toml` & `ast_grep_py-0.21.4/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/src/check_var.rs` & `ast_grep_py-0.21.4/crates/config/src/check_var.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 use crate::fixer::Fixer;
 use crate::rule::Rule;
-use crate::rule_core::RuleConfigError;
-use crate::transform::Transformation;
+use crate::rule_config::RuleConfigError;
+use crate::rule_core::RuleCoreError;
+use crate::transform::{TransformError, Transformation};
 use crate::{GlobalRules, RuleCore};
 
 use ast_grep_core::language::Language;
 
 use std::collections::{HashMap, HashSet};
 
-type RResult<T> = std::result::Result<T, RuleConfigError>;
+type RResult<T> = std::result::Result<T, RuleCoreError>;
 
-pub fn check_rewriters_in_transform<L: Language>(
-  rule: &RuleCore<L>,
-  rewriters: &GlobalRules<L>,
-) -> Result<(), RuleConfigError> {
-  let rewriters = rewriters.read();
-  if let Some(err) = check_one_rewriter_in_rule(rule, &rewriters) {
-    return Err(err);
-  }
-  let error = rewriters
-    .values()
-    .find_map(|rewriter| check_one_rewriter_in_rule(rewriter, &rewriters));
-  if let Some(err) = error {
-    return Err(err);
-  }
-  Ok(())
+pub enum CheckHint<'r> {
+  Global,
+  Normal,
+  Rewriter(&'r HashSet<&'r str>),
 }
 
-fn check_one_rewriter_in_rule<L: Language>(
-  rule: &RuleCore<L>,
-  rewriters: &HashMap<String, RuleCore<L>>,
-) -> Option<RuleConfigError> {
-  let transform = rule.transform.as_ref()?;
-  let mut used_rewriters = transform
-    .values()
-    .flat_map(|trans| trans.used_rewriters().iter());
-  let undefined_writers = used_rewriters.find(|r| !rewriters.contains_key(*r))?;
-  Some(RuleConfigError::UndefinedRewriter(
-    undefined_writers.to_string(),
-  ))
+/// Different rule sections have different variable scopes/check procedure.
+/// so we need to check rules with different hints.
+pub fn check_rule_with_hint<'r, L: Language>(
+  rule: &'r Rule<L>,
+  constraints: &'r HashMap<String, Rule<L>>,
+  transform: &'r Option<HashMap<String, Transformation>>,
+  fixer: &Option<Fixer<L>>,
+  hint: CheckHint<'r>,
+) -> RResult<()> {
+  match hint {
+    CheckHint::Global => {
+      // do not check utils defined here because global rules are not yet ready
+      check_vars(rule, constraints, transform, fixer)?;
+    }
+    CheckHint::Normal => {
+      check_utils_defined(rule, constraints)?;
+      check_vars(rule, constraints, transform, fixer)?;
+    }
+    // upper_vars is needed to check metavar defined in containing vars
+    CheckHint::Rewriter(upper_vars) => {
+      check_utils_defined(rule, constraints)?;
+      check_vars_in_rewriter(rule, constraints, transform, fixer, upper_vars)?;
+    }
+  }
+  Ok(())
 }
 
-pub fn check_vars_in_rewriter<'r, L: Language>(
+fn check_vars_in_rewriter<'r, L: Language>(
   rule: &'r Rule<L>,
   constraints: &'r HashMap<String, Rule<L>>,
   transform: &'r Option<HashMap<String, Transformation>>,
   fixer: &Option<Fixer<L>>,
   upper_var: &HashSet<&str>,
 ) -> RResult<()> {
   let vars = check_var_in_constraints(rule, constraints)?;
@@ -53,15 +56,26 @@
   for v in upper_var {
     vars.insert(v);
   }
   check_var_in_fix(vars, fixer)?;
   Ok(())
 }
 
-pub fn check_vars<'r, L: Language>(
+fn check_utils_defined<L: Language>(
+  rule: &Rule<L>,
+  constraints: &HashMap<String, Rule<L>>,
+) -> RResult<()> {
+  rule.verify_util()?;
+  for constraint in constraints.values() {
+    constraint.verify_util()?;
+  }
+  Ok(())
+}
+
+fn check_vars<'r, L: Language>(
   rule: &'r Rule<L>,
   constraints: &'r HashMap<String, Rule<L>>,
   transform: &'r Option<HashMap<String, Transformation>>,
   fixer: &Option<Fixer<L>>,
 ) -> RResult<()> {
   let vars = check_var_in_constraints(rule, constraints)?;
   let vars = check_var_in_transform(vars, transform)?;
@@ -78,15 +92,15 @@
     for var in rule.defined_vars() {
       vars.insert(var);
     }
   }
   for var in constraints.keys() {
     let var: &str = var;
     if !vars.contains(var) {
-      return Err(RuleConfigError::UndefinedMetaVar(
+      return Err(RuleCoreError::UndefinedMetaVar(
         var.to_owned(),
         "constraints",
       ));
     }
   }
   Ok(vars)
 }
@@ -95,40 +109,76 @@
   mut vars: HashSet<&'r str>,
   transform: &'r Option<HashMap<String, Transformation>>,
 ) -> RResult<HashSet<&'r str>> {
   let Some(transform) = transform else {
     return Ok(vars);
   };
   for var in transform.keys() {
-    vars.insert(var);
+    // vars already has the transform value. Report error!
+    if !vars.insert(var) {
+      return Err(RuleCoreError::Transform(TransformError::AlreadyDefined(
+        var.to_string(),
+      )));
+    }
   }
   for trans in transform.values() {
     let needed = trans.used_vars();
     if !vars.contains(needed) {
-      return Err(RuleConfigError::UndefinedMetaVar(
+      return Err(RuleCoreError::UndefinedMetaVar(
         needed.to_string(),
         "transform",
       ));
     }
   }
   Ok(vars)
 }
 
 fn check_var_in_fix<L: Language>(vars: HashSet<&str>, fixer: &Option<Fixer<L>>) -> RResult<()> {
   let Some(fixer) = fixer else {
     return Ok(());
   };
   for var in fixer.used_vars() {
     if !vars.contains(&var) {
-      return Err(RuleConfigError::UndefinedMetaVar(var.to_string(), "fix"));
+      return Err(RuleCoreError::UndefinedMetaVar(var.to_string(), "fix"));
     }
   }
   Ok(())
 }
 
+pub fn check_rewriters_in_transform<L: Language>(
+  rule: &RuleCore<L>,
+  rewriters: &GlobalRules<L>,
+) -> Result<(), RuleConfigError> {
+  let rewriters = rewriters.read();
+  if let Some(err) = check_one_rewriter_in_rule(rule, &rewriters) {
+    return Err(err);
+  }
+  let error = rewriters
+    .values()
+    .find_map(|rewriter| check_one_rewriter_in_rule(rewriter, &rewriters));
+  if let Some(err) = error {
+    return Err(err);
+  }
+  Ok(())
+}
+
+fn check_one_rewriter_in_rule<L: Language>(
+  rule: &RuleCore<L>,
+  rewriters: &HashMap<String, RuleCore<L>>,
+) -> Option<RuleConfigError> {
+  let transform = rule.transform.as_ref()?;
+  let mut used_rewriters = transform
+    .values()
+    .flat_map(|trans| trans.used_rewriters().iter());
+  let undefined_writers = used_rewriters.find(|r| !rewriters.contains_key(*r))?;
+  Some(RuleConfigError::UndefinedRewriter(
+    undefined_writers.to_string(),
+  ))
+}
+
 #[cfg(test)]
 mod test {
   use super::*;
   use crate::test::TypeScript;
   use crate::{from_str, DeserializeEnv, SerializableRuleCore};
 
   #[test]
@@ -153,16 +203,16 @@
     );
   }
 
   fn get_undefined(src: &str) -> (String, &str) {
     let env = DeserializeEnv::new(TypeScript::Tsx);
     let ser_rule: SerializableRuleCore = from_str(src).expect("should deser");
     match ser_rule.get_matcher(env) {
-      Err(RuleConfigError::UndefinedMetaVar(name, section)) => (name, section),
-      _ => panic!("should error"),
+      Err(RuleCoreError::UndefinedMetaVar(name, section)) => (name, section),
+      _ => panic!("unexpected error"),
     }
   }
 
   #[test]
   fn test_undefined_vars_in_constraints() {
     let (name, section) = get_undefined(
       r"
@@ -229,8 +279,27 @@
   test1: { pattern: $B, inside: {matches: test2} }
   test2: { pattern: $A, has: {matches: test1} }",
     )
     .expect("should deser");
     let matcher = ser_rule.get_matcher(env).expect("should parse");
     assert_eq!(matcher.defined_vars(), ["A", "B"].into_iter().collect());
   }
+
+  #[test]
+  fn test_transform_already_defined() {
+    let env = DeserializeEnv::new(TypeScript::Tsx);
+    let ser_rule: SerializableRuleCore = from_str(
+      r"
+rule: { pattern: $A = $B }
+transform:
+  B: { substring: { source: $A } }",
+    )
+    .expect("should deser");
+    let matcher = ser_rule.get_matcher(env);
+    match matcher {
+      Err(RuleCoreError::Transform(TransformError::AlreadyDefined(b))) => {
+        assert_eq!(b, "B");
+      }
+      _ => panic!("unexpected error"),
+    }
+  }
 }
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/combined.rs` & `ast_grep_py-0.21.4/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/src/fixer.rs` & `ast_grep_py-0.21.4/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/src/lib.rs` & `ast_grep_py-0.21.4/crates/config/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 pub use combined::CombinedScan;
 pub use fixer::Fixer;
 pub use rule::referent_rule::GlobalRules;
 pub use rule::DeserializeEnv;
 pub use rule::{Rule, RuleSerializeError, SerializableRule};
 pub use rule_collection::RuleCollection;
-pub use rule_config::{
-  RuleConfig, RuleConfigError, RuleCore, SerializableRuleConfig, SerializableRuleCore, Severity,
-};
+pub use rule_config::{RuleConfig, RuleConfigError, SerializableRuleConfig, Severity};
+pub use rule_core::{RuleCore, RuleCoreError, SerializableRuleCore};
 pub use transform::Transformation;
 
 pub fn from_str<'de, T: Deserialize<'de>>(s: &'de str) -> Result<T, YamlError> {
   let deserializer = Deserializer::from_str(s);
   deserialize(deserializer)
 }
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/maybe.rs` & `ast_grep_py-0.21.4/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.21.4/crates/config/src/rule/deserialize_env.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use super::referent_rule::{GlobalRules, ReferentRuleError, RuleRegistration};
+use crate::check_var::CheckHint;
 use crate::maybe::Maybe;
 use crate::rule::{self, Rule, RuleSerializeError, SerializableRule};
-use crate::rule_config::RuleConfigError;
-use crate::rule_core::SerializableRuleCore;
+use crate::rule_core::{RuleCoreError, SerializableRuleCore};
+use crate::transform::Transformation;
 
 use ast_grep_core::language::Language;
 
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 
 use std::collections::HashMap;
@@ -26,95 +27,97 @@
 ) -> HashMap<String, (L, SerializableRuleCore)> {
   rules
     .into_iter()
     .map(|r| (r.id, (r.language, r.core)))
     .collect()
 }
 
-type OrderResult<T> = Result<T, ReferentRuleError>;
+type OrderResult<T> = Result<T, String>;
 
 /// A struct to store information to deserialize rules.
 pub struct DeserializeEnv<L: Language> {
   /// registration for global utility rules and local utility rules.
   pub(crate) registration: RuleRegistration<L>,
   /// current rules' language
   pub(crate) lang: L,
 }
 
 trait DependentRule: Sized {
-  fn visit_dependent_rules<'a>(&'a self, sorter: &mut TopologicalSort<'a, Self>)
-    -> OrderResult<()>;
+  fn visit_dependency<'a>(&'a self, sorter: &mut TopologicalSort<'a, Self>) -> OrderResult<()>;
 }
 
 impl DependentRule for SerializableRule {
-  fn visit_dependent_rules<'a>(
-    &'a self,
-    sorter: &mut TopologicalSort<'a, Self>,
-  ) -> OrderResult<()> {
+  fn visit_dependency<'a>(&'a self, sorter: &mut TopologicalSort<'a, Self>) -> OrderResult<()> {
     visit_dependent_rule_ids(self, sorter)
   }
 }
 
 impl<L: Language> DependentRule for (L, SerializableRuleCore) {
-  fn visit_dependent_rules<'a>(
-    &'a self,
-    sorter: &mut TopologicalSort<'a, Self>,
-  ) -> OrderResult<()> {
+  fn visit_dependency<'a>(&'a self, sorter: &mut TopologicalSort<'a, Self>) -> OrderResult<()> {
     visit_dependent_rule_ids(&self.1.rule, sorter)
   }
 }
 
+impl DependentRule for Transformation {
+  fn visit_dependency<'a>(&'a self, sorter: &mut TopologicalSort<'a, Self>) -> OrderResult<()> {
+    let used_var = self.used_vars();
+    sorter.visit(used_var)
+  }
+}
+
 /// A struct to topological sort rules
-/// it is used to report cyclic dependency errors in rules
+/// it is used to report cyclic dependency errors in rules/transformation
 struct TopologicalSort<'a, T: DependentRule> {
-  utils: &'a HashMap<String, T>,
-  order: Vec<&'a String>,
+  maps: &'a HashMap<String, T>,
+  order: Vec<&'a str>,
   // bool stands for if the rule has completed visit
-  seen: HashMap<&'a String, bool>,
+  seen: HashMap<&'a str, bool>,
 }
 
 impl<'a, T: DependentRule> TopologicalSort<'a, T> {
-  fn get_order(utils: &HashMap<String, T>) -> OrderResult<Vec<&String>> {
-    let mut top_sort = TopologicalSort::new(utils);
-    for rule_id in utils.keys() {
-      top_sort.visit(rule_id)?;
+  fn get_order(maps: &HashMap<String, T>) -> OrderResult<Vec<&str>> {
+    let mut top_sort = TopologicalSort::new(maps);
+    for key in maps.keys() {
+      top_sort.visit(key)?;
     }
     Ok(top_sort.order)
   }
 
-  fn new(utils: &'a HashMap<String, T>) -> Self {
+  fn new(maps: &'a HashMap<String, T>) -> Self {
     Self {
-      utils,
+      maps,
       order: vec![],
       seen: HashMap::new(),
     }
   }
 
-  fn visit(&mut self, rule_id: &'a String) -> OrderResult<()> {
-    if let Some(&completed) = self.seen.get(rule_id) {
+  fn visit(&mut self, key: &'a str) -> OrderResult<()> {
+    if let Some(&completed) = self.seen.get(key) {
       // if the rule has been seen but not completed
       // it means we have a cyclic dependency and report an error here
       return if completed {
         Ok(())
       } else {
-        Err(ReferentRuleError::CyclicRule)
+        Err(key.to_string())
       };
     }
-    let Some(rule) = self.utils.get(rule_id) else {
+    let Some(item) = self.maps.get(key) else {
+      // key can be found elsewhere
+      // e.g. if key is rule_id
       // if rule_id not found in global, it can be a local rule
       // if rule_id not found in local, it can be a global rule
       // TODO: add check here and return Err if rule not found
       return Ok(());
     };
     // mark the id as seen but not completed
-    self.seen.insert(rule_id, false);
-    rule.visit_dependent_rules(self)?;
+    self.seen.insert(key, false);
+    item.visit_dependency(self)?;
     // mark the id as seen and completed
-    self.seen.insert(rule_id, true);
-    self.order.push(rule_id);
+    self.seen.insert(key, true);
+    self.order.push(key);
     Ok(())
   }
 }
 
 fn visit_dependent_rule_ids<'a, T: DependentRule>(
   rule: &'a SerializableRule,
   sort: &mut TopologicalSort<'a, T>,
@@ -129,16 +132,16 @@
     }
   }
   if let Maybe::Present(any) = &rule.any {
     for sub in any {
       visit_dependent_rule_ids(sub, sort)?;
     }
   }
-  if let Maybe::Present(_not) = &rule.not {
-    // TODO: check cyclic here
+  if let Maybe::Present(not) = &rule.not {
+    visit_dependent_rule_ids(not, sort)?;
   }
   Ok(())
 }
 
 impl<L: Language> DeserializeEnv<L> {
   pub fn new(lang: L) -> Self {
     Self {
@@ -150,48 +153,59 @@
   /// register utils rule in the DeserializeEnv for later usage.
   /// N.B. This function will manage the util registration order
   /// by their dependency. `potential_kinds` need ordered insertion.
   pub fn register_local_utils(
     self,
     utils: &HashMap<String, SerializableRule>,
   ) -> Result<Self, RuleSerializeError> {
-    let order = TopologicalSort::get_order(utils)?;
+    let order = TopologicalSort::get_order(utils)
+      .map_err(ReferentRuleError::CyclicRule)
+      .map_err(RuleSerializeError::MatchesReference)?;
     for id in order {
       let rule = utils.get(id).expect("must exist");
       let rule = self.deserialize_rule(rule.clone())?;
       self.registration.insert_local(id, rule)?;
     }
     Ok(self)
   }
 
   /// register global utils rule discovered in the config.
   pub fn parse_global_utils(
     utils: Vec<SerializableGlobalRule<L>>,
-  ) -> Result<GlobalRules<L>, RuleConfigError> {
+  ) -> Result<GlobalRules<L>, RuleCoreError> {
     let registration = GlobalRules::default();
     let utils = into_map(utils);
-    let order = TopologicalSort::get_order(&utils).map_err(RuleSerializeError::from)?;
+    let order = TopologicalSort::get_order(&utils)
+      .map_err(ReferentRuleError::CyclicRule)
+      .map_err(RuleSerializeError::from)?;
     for id in order {
       let (lang, core) = utils.get(id).expect("must exist");
       let env = DeserializeEnv::new(lang.clone()).with_globals(&registration);
-      let matcher = core.get_matcher(env)?;
+      let matcher = core.get_matcher_with_hint(env, CheckHint::Global)?;
       registration
         .insert(id, matcher)
         .map_err(RuleSerializeError::MatchesReference)?;
     }
     Ok(registration)
   }
 
   pub fn deserialize_rule(
     &self,
     serialized: SerializableRule,
   ) -> Result<Rule<L>, RuleSerializeError> {
     rule::deserialize_rule(serialized, self)
   }
 
+  pub(crate) fn get_transform_order<'a>(
+    &self,
+    trans: &'a HashMap<String, Transformation>,
+  ) -> Result<Vec<&'a str>, String> {
+    TopologicalSort::get_order(trans)
+  }
+
   pub fn with_globals(self, globals: &GlobalRules<L>) -> Self {
     Self {
       registration: RuleRegistration::from_globals(globals),
       lang: self.lang,
     }
   }
   pub fn with_rewriters(self, globals: &GlobalRules<L>) -> Self {
@@ -287,8 +301,27 @@
     - matches: local-rule-a
 ",
     )?;
     let ret = DeserializeEnv::new(TypeScript::Tsx).register_local_utils(&utils);
     assert!(ret.is_err());
     Ok(())
   }
+
+  #[test]
+  fn test_cyclic_not() -> Result<()> {
+    let utils = from_str(
+      "
+local-rule-a:
+  not: {matches: local-rule-b}
+local-rule-b:
+  matches: local-rule-a",
+    )?;
+    let ret = DeserializeEnv::new(TypeScript::Tsx).register_local_utils(&utils);
+    assert!(matches!(
+      ret,
+      Err(RuleSerializeError::MatchesReference(
+        ReferentRuleError::CyclicRule(_)
+      ))
+    ));
+    Ok(())
+  }
 }
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule/mod.rs` & `ast_grep_py-0.21.4/crates/config/src/rule/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -206,14 +206,31 @@
       Rule::All(sub) => sub.inner().iter().flat_map(|r| r.defined_vars()).collect(),
       Rule::Any(sub) => sub.inner().iter().flat_map(|r| r.defined_vars()).collect(),
       Rule::Not(sub) => sub.inner().defined_vars(),
       // TODO: this is not correct, we are collecting util vars else where
       Rule::Matches(_r) => HashSet::new(),
     }
   }
+
+  /// check if util rules used are defined
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    match self {
+      Rule::Pattern(_) => Ok(()),
+      Rule::Kind(_) => Ok(()),
+      Rule::Regex(_) => Ok(()),
+      Rule::Has(c) => c.verify_util(),
+      Rule::Inside(p) => p.verify_util(),
+      Rule::Precedes(f) => f.verify_util(),
+      Rule::Follows(f) => f.verify_util(),
+      Rule::All(sub) => sub.inner().iter().try_for_each(|r| r.verify_util()),
+      Rule::Any(sub) => sub.inner().iter().try_for_each(|r| r.verify_util()),
+      Rule::Not(sub) => sub.inner().verify_util(),
+      Rule::Matches(r) => Ok(r.verify_util()?),
+    }
+  }
 }
 
 impl<L: Language> Matcher<L> for Rule<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.21.4/crates/config/src/rule/referent_rule.rs`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       return Err(ReferentRuleError::DuplicateRule(id.into()));
     }
     map.insert(id.to_string(), rule);
     let rule = map.get(id).unwrap();
     // TODO: we can skip check here because insertion order
     // is guaranteed in deserialize_env
     if rule.check_cyclic(id) {
-      return Err(ReferentRuleError::CyclicRule);
+      return Err(ReferentRuleError::CyclicRule(id.to_string()));
     }
     Ok(())
   }
 }
 
 impl<R> Default for Registration<R> {
   fn default() -> Self {
@@ -105,15 +105,15 @@
       return Err(ReferentRuleError::DuplicateRule(id.into()));
     }
     map.insert(id.to_string(), rule);
     let rule = map.get(id).unwrap();
     // TODO: we can skip check here because insertion order
     // is guaranteed in deserialize_env
     if rule.check_cyclic(id) {
-      return Err(ReferentRuleError::CyclicRule);
+      return Err(ReferentRuleError::CyclicRule(id.to_string()));
     }
     Ok(())
   }
 
   pub(crate) fn get_local_util_vars<'a>(&'a self) -> HashSet<&'a str> {
     let mut ret = HashSet::new();
     let utils = self.get_local();
@@ -152,20 +152,20 @@
       rewriters: Default::default(),
     }
   }
 }
 
 #[derive(Debug, Error)]
 pub enum ReferentRuleError {
-  #[error("Rule `{0}` is not found.")]
-  RuleNotFound(String),
+  #[error("Rule `{0}` is not defined.")]
+  UndefinedUtil(String),
   #[error("Duplicate rule id `{0}` is found.")]
   DuplicateRule(String),
-  #[error("Rule has a cyclic dependency in its `matches` sub-rule.")]
-  CyclicRule,
+  #[error("Rule `{0}` has a cyclic dependency in its `matches` sub-rule.")]
+  CyclicRule(String),
 }
 
 pub struct ReferentRule<L: Language> {
   pub(crate) rule_id: String,
   reg_ref: RegistrationRef<L>,
 }
 
@@ -195,14 +195,27 @@
     F: FnOnce(&RuleCore<L>) -> T,
   {
     let registration = self.reg_ref.unref();
     let rules = registration.get_global();
     let rule = rules.get(&self.rule_id)?;
     Some(func(rule))
   }
+
+  pub(super) fn verify_util(&self) -> Result<(), ReferentRuleError> {
+    let registration = self.reg_ref.unref();
+    let rules = registration.get_local();
+    if rules.contains_key(&self.rule_id) {
+      return Ok(());
+    }
+    let rules = registration.get_global();
+    if rules.contains_key(&self.rule_id) {
+      return Ok(());
+    }
+    Err(ReferentRuleError::UndefinedUtil(self.rule_id.clone()))
+  }
 }
 
 impl<L: Language> Matcher<L> for ReferentRule<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
@@ -240,25 +253,35 @@
 
   #[test]
   fn test_cyclic_error() -> Result {
     let registration = RuleRegistration::<TS>::default();
     let rule = ReferentRule::try_new("test".into(), &registration)?;
     let rule = Rule::Matches(rule);
     let error = registration.insert_local("test", rule);
-    assert!(matches!(error, Err(ReferentRuleError::CyclicRule)));
+    assert!(matches!(error, Err(ReferentRuleError::CyclicRule(_))));
     Ok(())
   }
 
   #[test]
   fn test_cyclic_all() -> Result {
     let registration = RuleRegistration::<TS>::default();
     let rule = ReferentRule::try_new("test".into(), &registration)?;
     let rule = Rule::All(o::All::new(std::iter::once(Rule::Matches(rule))));
     let error = registration.insert_local("test", rule);
-    assert!(matches!(error, Err(ReferentRuleError::CyclicRule)));
+    assert!(matches!(error, Err(ReferentRuleError::CyclicRule(_))));
+    Ok(())
+  }
+
+  #[test]
+  fn test_cyclic_not() -> Result {
+    let registration = RuleRegistration::<TS>::default();
+    let rule = ReferentRule::try_new("test".into(), &registration)?;
+    let rule = Rule::Not(Box::new(o::Not::new(Rule::Matches(rule))));
+    let error = registration.insert_local("test", rule);
+    assert!(matches!(error, Err(ReferentRuleError::CyclicRule(_))));
     Ok(())
   }
 
   #[test]
   fn test_success_rule() -> Result {
     let registration = RuleRegistration::<TS>::default();
     let rule = ReferentRule::try_new("test".into(), &registration)?;
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.21.4/crates/config/src/rule/relational_rule.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     self
       .outer
       .defined_vars()
       .union(&self.stop_by.defined_vars())
       .copied()
       .collect()
   }
+
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    self.outer.verify_util()?;
+    self.stop_by.verify_util()
+  }
 }
 
 impl<L: Language> Matcher<L> for Inside<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
@@ -104,14 +109,19 @@
     self
       .inner
       .defined_vars()
       .union(&self.stop_by.defined_vars())
       .copied()
       .collect()
   }
+
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    self.inner.verify_util()?;
+    self.stop_by.verify_util()
+  }
 }
 
 impl<L: Language> Matcher<L> for Has<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
@@ -179,14 +189,19 @@
     self
       .later
       .defined_vars()
       .union(&self.stop_by.defined_vars())
       .copied()
       .collect()
   }
+
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    self.later.verify_util()?;
+    self.stop_by.verify_util()
+  }
 }
 impl<L: Language> Matcher<L> for Precedes<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
   ) -> Option<Node<'tree, D>> {
@@ -215,14 +230,19 @@
     self
       .former
       .defined_vars()
       .union(&self.stop_by.defined_vars())
       .copied()
       .collect()
   }
+
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    self.former.verify_util()?;
+    self.stop_by.verify_util()
+  }
 }
 impl<L: Language> Matcher<L> for Follows<L> {
   fn match_node_with_env<'tree, D: Doc<Lang = L>>(
     &self,
     node: Node<'tree, D>,
     env: &mut Cow<MetaVarEnv<'tree, D>>,
   ) -> Option<Node<'tree, D>> {
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.21.4/crates/config/src/rule/stop_by.rs`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,24 @@
       S::Rule(r) => StopBy::Rule(env.deserialize_rule(r)?),
     })
   }
 
   pub fn defined_vars(&self) -> HashSet<&str> {
     match self {
       StopBy::Rule(rule) => rule.defined_vars(),
-      _ => HashSet::new(),
+      StopBy::End => HashSet::new(),
+      StopBy::Neighbor => HashSet::new(),
+    }
+  }
+
+  pub fn verify_util(&self) -> Result<(), RuleSerializeError> {
+    match self {
+      StopBy::Rule(rule) => rule.verify_util(),
+      StopBy::End => Ok(()),
+      StopBy::Neighbor => Ok(()),
     }
   }
 }
 
 impl<L: Language> StopBy<L> {
   // TODO: document this monster method
   pub(crate) fn find<'t, O, M, I, F, D>(
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule_collection.rs` & `ast_grep_py-0.21.4/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule_config.rs` & `ast_grep_py-0.21.4/crates/config/src/rule_config.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 use crate::GlobalRules;
 
-use crate::check_var::check_rewriters_in_transform;
+use crate::check_var::{check_rewriters_in_transform, CheckHint};
 use crate::fixer::Fixer;
 use crate::rule::DeserializeEnv;
-pub use crate::rule_core::{RuleConfigError, RuleCore, SerializableRuleCore};
+use crate::rule_core::{RuleCore, RuleCoreError, SerializableRuleCore};
+
 use ast_grep_core::language::Language;
 use ast_grep_core::replacer::Replacer;
 use ast_grep_core::{NodeMatch, StrDoc};
+
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
+use serde_yaml::Error as YamlError;
 use serde_yaml::{with::singleton_map_recursive::deserialize, Deserializer};
+use thiserror::Error;
 
-use std::collections::HashMap;
+use std::collections::{HashMap, HashSet};
 use std::ops::{Deref, DerefMut};
 
 #[derive(Serialize, Deserialize, Clone, Default, JsonSchema)]
 #[serde(rename_all = "camelCase")]
 pub enum Severity {
   #[default]
   /// A kind reminder for code with potential improvement.
@@ -26,14 +30,28 @@
   Warning,
   /// An error that code produces bugs or has logic errors.
   Error,
   /// Turns off the rule.
   Off,
 }
 
+#[derive(Debug, Error)]
+pub enum RuleConfigError {
+  #[error("Fail to parse yaml as RuleConfig")]
+  Yaml(#[from] YamlError),
+  #[error("Fail to parse yaml as Rule.")]
+  Core(#[from] RuleCoreError),
+  #[error("Rewriter rule `{1}` is not configured correctly.")]
+  Rewriter(#[source] RuleCoreError, String),
+  #[error("Undefined rewriter `{0}` used in transform.")]
+  UndefinedRewriter(String),
+  #[error("Rewriter rule `{0}` should have `fix`.")]
+  NoFixInRewriter(String),
+}
+
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 pub struct SerializableRewriter {
   #[serde(flatten)]
   pub core: SerializableRuleCore,
   /// Unique, descriptive identifier, e.g., no-unused-variable
   pub id: String,
 }
@@ -78,41 +96,59 @@
     // all RuleConfigs has one common globals
     // every sub-rule has one util
     let rewriters = GlobalRules::default();
     let env = DeserializeEnv::new(self.language.clone())
       .with_globals(globals)
       .with_rewriters(&rewriters);
     let rule = self.core.get_matcher(env)?;
-    self.register_rewriter(&rule, globals, &rewriters)?;
+    self.register_rewriters(&rule, globals, &rewriters)?;
     Ok(rule)
   }
 
-  fn register_rewriter(
+  fn register_rewriters(
     &self,
     rule: &RuleCore<L>,
     globals: &GlobalRules<L>,
     rewriters: &GlobalRules<L>,
   ) -> Result<(), RuleConfigError> {
     let Some(ser) = &self.rewriters else {
       return Ok(());
     };
     let vars = rule.defined_vars();
     for val in ser {
-      // NB should inherit env from matcher to inherit utils
-      // TODO: optimize duplicate env creation/util registration
-      let env = DeserializeEnv::new(self.language.clone())
-        .with_globals(globals)
-        .with_rewriters(rewriters);
-      let env = self.get_deserialize_env(env)?;
-      let rewriter = val.core.get_rewriter(env, &vars)?;
-      rewriters.insert(&val.id, rewriter).expect("should work");
+      if val.core.fix.is_none() {
+        return Err(RuleConfigError::NoFixInRewriter(val.id.clone()));
+      }
+      self
+        .register_one_rewriter(val, &vars, globals, rewriters)
+        .map_err(|e| RuleConfigError::Rewriter(e, val.id.clone()))?;
     }
     check_rewriters_in_transform(rule, rewriters)?;
     Ok(())
   }
+
+  fn register_one_rewriter(
+    &self,
+    val: &SerializableRewriter,
+    vars: &HashSet<&str>,
+    globals: &GlobalRules<L>,
+    rewriters: &GlobalRules<L>,
+  ) -> Result<(), RuleCoreError> {
+    // NB should inherit env from matcher to inherit utils
+    // TODO: optimize duplicate env creation/util registration
+    let env = DeserializeEnv::new(self.language.clone())
+      .with_globals(globals)
+      .with_rewriters(rewriters);
+    let env = self.get_deserialize_env(env)?;
+    let rewriter = val
+      .core
+      .get_matcher_with_hint(env, CheckHint::Rewriter(vars))?;
+    rewriters.insert(&val.id, rewriter).expect("should work");
+    Ok(())
+  }
 }
 
 impl<L: Language> Deref for SerializableRuleConfig<L> {
   type Target = SerializableRuleCore;
   fn deref(&self) -> &Self::Target {
     &self.core
   }
@@ -151,15 +187,15 @@
 
   pub fn get_message(&self, node: &NodeMatch<StrDoc<L>>) -> String {
     self.inner.get_message(node)
   }
   pub fn get_fixer(&self) -> Result<Option<Fixer<L>>, RuleConfigError> {
     if let Some(fix) = &self.fix {
       let env = self.matcher.get_env(self.language.clone());
-      let parsed = Fixer::parse(fix, &env, &self.transform)?;
+      let parsed = Fixer::parse(fix, &env, &self.transform).map_err(RuleCoreError::Fixer)?;
       Ok(Some(parsed))
     } else {
       Ok(None)
     }
   }
 }
 impl<L: Language> Deref for RuleConfig<L> {
@@ -425,18 +461,35 @@
   rule: {matches: num}
   fix: yjsnp
   utils:
     num: { kind: number }
     ",
     )
     .expect("should parse");
-    let rule = RuleConfig::try_from(rule, &Default::default()).expect("work");
-    let grep = TypeScript::Tsx.ast_grep("a = 456");
-    let nm = grep.root().find(&rule.matcher);
-    assert!(nm.is_none());
+    let ret = RuleConfig::try_from(rule, &Default::default());
+    assert!(matches!(ret, Err(RuleConfigError::Core(_))));
+  }
+
+  #[test]
+  fn test_rewriter_should_have_fix() {
+    let rule: SerializableRuleConfig<TypeScript> = from_str(
+      r"
+id: test
+rule: {kind: number}
+language: Tsx
+rewriters:
+- id: wrong
+  rule: {matches: num}",
+    )
+    .expect("should parse");
+    let ret = RuleConfig::try_from(rule, &Default::default());
+    match ret {
+      Err(RuleConfigError::NoFixInRewriter(name)) => assert_eq!(name, "wrong"),
+      _ => panic!("unexpected error"),
+    }
   }
 
   #[test]
   fn test_utils_in_rewriter_should_work() {
     let rule: SerializableRuleConfig<TypeScript> = from_str(
       r"
 id: test
@@ -513,14 +566,34 @@
 - id: re
   rule: {kind: number, pattern: $A}
   fix: hah
     ",
     );
     assert_eq!(undefined, "not-defined");
   }
+  #[test]
+  fn test_wrong_rewriter() {
+    let rule: SerializableRuleConfig<TypeScript> = from_str(
+      r"
+id: test
+rule: {pattern: 'a = $A'}
+language: Tsx
+rewriters:
+- id: wrong
+  rule: {kind: '114'}
+  fix: '1919810'
+    ",
+    )
+    .expect("should parse");
+    let ret = RuleConfig::try_from(rule, &Default::default());
+    match ret {
+      Err(RuleConfigError::Rewriter(_, name)) => assert_eq!(name, "wrong"),
+      _ => panic!("unexpected error"),
+    }
+  }
 
   #[test]
   fn test_undefined_rewriter_in_transform() {
     let undefined = make_undefined_error(
       r"
 id: test
 rule: {pattern: 'a = $A'}
@@ -541,15 +614,15 @@
   #[test]
   fn test_rewriter_use_upper_var() {
     let src = r"
 id: test
 rule: {pattern: '$B = $A'}
 language: Tsx
 transform:
-  B: { rewrite: { rewriters: [re], source: $A } }
+  D: { rewrite: { rewriters: [re], source: $A } }
 rewriters:
 - id: re
   rule: {kind: number, pattern: $C}
   fix: $B.$C
     ";
     let rule: SerializableRuleConfig<TypeScript> = from_str(src).expect("should parse");
     let ret = RuleConfig::try_from(rule, &Default::default());
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/rule_core.rs` & `ast_grep_py-0.21.4/crates/config/src/rule_core.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use crate::check_var::{check_vars, check_vars_in_rewriter};
+use crate::check_var::{check_rule_with_hint, CheckHint};
 use crate::fixer::{Fixer, FixerError, SerializableFixer};
 use crate::rule::referent_rule::RuleRegistration;
 use crate::rule::Rule;
 use crate::rule::{RuleSerializeError, SerializableRule};
-use crate::transform::{apply_env_transform, Transformation};
+use crate::transform::{Transform, TransformError, Transformation};
 use crate::DeserializeEnv;
 
 use ast_grep_core::language::Language;
 use ast_grep_core::meta_var::MetaVarEnv;
 use ast_grep_core::{Doc, Matcher, Node};
 use serde::{Deserialize, Serialize};
 use serde_yaml::Error as YamlError;
@@ -17,32 +17,32 @@
 use thiserror::Error;
 
 use std::borrow::Cow;
 use std::collections::{HashMap, HashSet};
 use std::ops::Deref;
 
 #[derive(Debug, Error)]
-pub enum RuleConfigError {
+pub enum RuleCoreError {
   #[error("Fail to parse yaml as RuleConfig")]
   Yaml(#[from] YamlError),
-  #[error("Rule is not configured correctly.")]
-  Rule(#[from] RuleSerializeError),
-  #[error("Utility rule is not configured correctly.")]
+  #[error("`utils` is not configured correctly.")]
   Utils(#[source] RuleSerializeError),
-  #[error("fix pattern is invalid.")]
-  Fixer(#[from] FixerError),
-  #[error("constraints is not configured correctly.")]
+  #[error("`rule` is not configured correctly.")]
+  Rule(#[from] RuleSerializeError),
+  #[error("`constraints` is not configured correctly.")]
   Constraints(#[source] RuleSerializeError),
-  #[error("Undefined meta var {0} used in {1}.")]
+  #[error("`transform` is not configured correctly.")]
+  Transform(#[from] TransformError),
+  #[error("`fix` pattern is invalid.")]
+  Fixer(#[from] FixerError),
+  #[error("Undefined meta var `{0}` used in `{1}`.")]
   UndefinedMetaVar(String, &'static str),
-  #[error("Undefined rewriter {0} used in transform.")]
-  UndefinedRewriter(String),
 }
 
-type RResult<T> = std::result::Result<T, RuleConfigError>;
+type RResult<T> = std::result::Result<T, RuleCoreError>;
 
 /// Used for global rules, rewriters, and pyo3/napi
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 pub struct SerializableRuleCore {
   /// A rule object to find matching AST nodes
   pub rule: SerializableRule,
   /// Additional meta variables pattern to filter matching
@@ -63,15 +63,15 @@
   pub(crate) fn get_deserialize_env<L: Language>(
     &self,
     env: DeserializeEnv<L>,
   ) -> RResult<DeserializeEnv<L>> {
     if let Some(utils) = &self.utils {
       let env = env
         .register_local_utils(utils)
-        .map_err(RuleConfigError::Utils)?;
+        .map_err(RuleCoreError::Utils)?;
       Ok(env)
     } else {
       Ok(env)
     }
   }
 
   fn get_constraints<L: Language>(
@@ -79,15 +79,18 @@
     env: &DeserializeEnv<L>,
   ) -> RResult<HashMap<String, Rule<L>>> {
     let mut constraints = HashMap::new();
     let Some(serde_cons) = &self.constraints else {
       return Ok(constraints);
     };
     for (key, ser) in serde_cons {
-      constraints.insert(key.to_string(), env.deserialize_rule(ser.clone())?);
+      let constraint = env
+        .deserialize_rule(ser.clone())
+        .map_err(RuleCoreError::Constraints)?;
+      constraints.insert(key.to_string(), constraint);
     }
     Ok(constraints)
   }
 
   fn get_fixer<L: Language>(&self, env: &DeserializeEnv<L>) -> RResult<Option<Fixer<L>>> {
     if let Some(fix) = &self.fix {
       let parsed = Fixer::parse(fix, env, &self.transform)?;
@@ -96,56 +99,56 @@
       Ok(None)
     }
   }
 
   fn get_matcher_from_env<L: Language>(&self, env: &DeserializeEnv<L>) -> RResult<RuleCore<L>> {
     let rule = env.deserialize_rule(self.rule.clone())?;
     let constraints = self.get_constraints(env)?;
-    let transform = self.transform.clone();
+    let transform = self
+      .transform
+      .as_ref()
+      .map(|t| Transform::deserialize(t, env))
+      .transpose()?;
     let fixer = self.get_fixer(env)?;
     Ok(
       RuleCore::new(rule)
         .with_matchers(constraints)
         .with_utils(env.registration.clone())
         .with_transform(transform)
         .with_fixer(fixer),
     )
   }
 
   pub fn get_matcher<L: Language>(&self, env: DeserializeEnv<L>) -> RResult<RuleCore<L>> {
-    let env = self.get_deserialize_env(env)?;
-    let ret = self.get_matcher_from_env(&env)?;
-    check_vars(&ret.rule, &ret.constraints, &ret.transform, &ret.fixer)?;
-    Ok(ret)
+    self.get_matcher_with_hint(env, CheckHint::Normal)
   }
 
-  /// this is needed for checking metavar defined in containing vars
-  pub(crate) fn get_rewriter<L: Language>(
+  pub(crate) fn get_matcher_with_hint<L: Language>(
     &self,
     env: DeserializeEnv<L>,
-    upper_vars: &HashSet<&str>,
+    hint: CheckHint,
   ) -> RResult<RuleCore<L>> {
     let env = self.get_deserialize_env(env)?;
     let ret = self.get_matcher_from_env(&env)?;
-    check_vars_in_rewriter(
+    check_rule_with_hint(
       &ret.rule,
       &ret.constraints,
-      &ret.transform,
+      &self.transform,
       &ret.fixer,
-      upper_vars,
+      hint,
     )?;
     Ok(ret)
   }
 }
 
 pub struct RuleCore<L: Language> {
   rule: Rule<L>,
   constraints: HashMap<String, Rule<L>>,
   kinds: Option<BitSet>,
-  pub(crate) transform: Option<HashMap<String, Transformation>>,
+  pub(crate) transform: Option<Transform>,
   pub fixer: Option<Fixer<L>>,
   // this is required to hold util rule reference
   utils: RuleRegistration<L>,
 }
 
 impl<L: Language> RuleCore<L> {
   #[inline]
@@ -168,15 +171,15 @@
 
   #[inline]
   pub fn with_utils(self, utils: RuleRegistration<L>) -> Self {
     Self { utils, ..self }
   }
 
   #[inline]
-  pub fn with_transform(self, transform: Option<HashMap<String, Transformation>>) -> Self {
+  pub fn with_transform(self, transform: Option<Transform>) -> Self {
     Self { transform, ..self }
   }
 
   #[inline]
   pub fn with_fixer(self, fixer: Option<Fixer<L>>) -> Self {
     Self { fixer, ..self }
   }
@@ -218,22 +221,22 @@
       }
     }
     let ret = self.rule.match_node_with_env(node, env)?;
     if !env.to_mut().match_constraints(&self.constraints) {
       return None;
     }
     if let Some(trans) = &self.transform {
-      let lang = ret.lang();
       let rewriters = self.utils.get_rewriters();
+      let rewriters = rewriters.read();
       let env = env.to_mut();
       if let Some(enclosing) = enclosing_env {
-        apply_env_transform(trans, lang, env, rewriters, enclosing);
+        trans.apply_transform(env, &rewriters, enclosing);
       } else {
         let enclosing = env.clone();
-        apply_env_transform(trans, lang, env, rewriters, &enclosing);
+        trans.apply_transform(env, &rewriters, &enclosing);
       };
     }
     Some(ret)
   }
 }
 impl<L: Language> Deref for RuleCore<L> {
   type Target = Rule<L>;
@@ -269,19 +272,70 @@
     self.rule.potential_kinds()
   }
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
-  use crate::rule::referent_rule::ReferentRule;
+  use crate::rule::referent_rule::{ReferentRule, ReferentRuleError};
   use crate::test::TypeScript;
   use crate::{from_str, GlobalRules};
   use ast_grep_core::matcher::{Pattern, RegexMatcher};
 
+  fn get_matcher(src: &str) -> RResult<RuleCore<TypeScript>> {
+    let env = DeserializeEnv::new(TypeScript::Tsx);
+    let rule: SerializableRuleCore = from_str(src).expect("should word");
+    rule.get_matcher(env)
+  }
+
+  #[test]
+  fn test_rule_error() {
+    let ret = get_matcher(r"rule: {kind: bbb}");
+    assert!(matches!(ret, Err(RuleCoreError::Rule(_))));
+  }
+
+  #[test]
+  fn test_utils_error() {
+    let ret = get_matcher(
+      r"
+rule: { kind: number }
+utils: { testa: {kind: bbb} }
+  ",
+    );
+    assert!(matches!(ret, Err(RuleCoreError::Utils(_))));
+  }
+
+  #[test]
+  fn test_undefined_utils_error() {
+    let ret = get_matcher(r"rule: { kind: number, matches: undefined-util }");
+    match ret {
+      Err(RuleCoreError::Rule(RuleSerializeError::MatchesReference(
+        ReferentRuleError::UndefinedUtil(name),
+      ))) => {
+        assert_eq!(name, "undefined-util");
+      }
+      _ => panic!("wrong error"),
+    }
+  }
+
+  #[test]
+  fn test_cyclic_transform_error() {
+    let ret = get_matcher(
+      r"
+rule: { kind: number }
+transform:
+  A: {substring: {source: $B}}
+  B: {substring: {source: $A}}",
+    );
+    assert!(matches!(
+      ret,
+      Err(RuleCoreError::Transform(TransformError::Cyclic(_)))
+    ));
+  }
+
   #[test]
   fn test_rule_reg_with_utils() {
     let env = DeserializeEnv::new(TypeScript::Tsx);
     let ser_rule: SerializableRuleCore =
       from_str("{rule: {matches: test}, utils: {test: {kind: number}} }").expect("should deser");
     let rule = ReferentRule::try_new("test".into(), &env.registration).expect("should work");
     let not = ReferentRule::try_new("test2".into(), &env.registration).expect("should work");
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/transform/mod.rs` & `ast_grep_py-0.21.4/crates/config/src/transform/transformation.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,41 @@
-mod rewrite;
-mod string_case;
-
-use crate::GlobalRules;
-use ast_grep_core::meta_var::{MetaVarEnv, MetaVariable};
+use super::rewrite::Rewrite;
+use super::{string_case, Ctx, TransformError};
+use ast_grep_core::meta_var::MetaVariable;
 use ast_grep_core::source::Content;
 use ast_grep_core::{Doc, Language};
-pub use rewrite::Rewrite;
 
 use regex::Regex;
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 
-use std::collections::HashMap;
 use string_case::{Separator, StringCase};
 
-fn get_text_from_env<D: Doc>(src: &str, ctx: &mut Ctx<D>) -> Option<String> {
-  let source = ctx.lang.pre_process_pattern(src);
-  let var = ctx.lang.extract_meta_var(&source)?;
-  if let MetaVariable::Capture(n, _) = &var {
-    if let Some(tr) = ctx.transforms.get(n) {
-      if ctx.env.get_transformed(n).is_none() {
-        tr.insert(n, ctx);
-      }
-    }
-  }
-  let bytes = ctx.env.get_var_bytes(&var)?;
+fn get_text_from_env<D: Doc>(var: &MetaVariable, ctx: &mut Ctx<D>) -> Option<String> {
+  // TODO: check if topological sort has resolved transform dependency
+  let bytes = ctx.env.get_var_bytes(var)?;
   Some(<D::Source as Content>::encode_bytes(bytes).into_owned())
 }
 
 /// Extracts a substring from the meta variable's text content.
 ///
 /// Both `start_char` and `end_char` support negative indexing,
 /// which counts character from the end of an array, moving backwards.
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 #[serde(rename_all = "camelCase")]
-pub struct Substring {
+pub struct Substring<T> {
   /// source meta variable to be transformed
-  source: String,
+  source: T,
   /// optional starting character index of the substring, defaults to 0.
   start_char: Option<i32>,
   /// optional ending character index of the substring, defaults to the end of the string.
   end_char: Option<i32>,
 }
 
-impl Substring {
+impl Substring<MetaVariable> {
   fn compute<D: Doc>(&self, ctx: &mut Ctx<D>) -> Option<String> {
     let text = get_text_from_env(&self.source, ctx)?;
     let chars: Vec<_> = text.chars().collect();
     let len = chars.len() as i32;
     let start = resolve_char(&self.start_char, 0, len);
     let end = resolve_char(&self.end_char, len, len);
     if start > end || start >= len as usize || end > len as usize {
@@ -72,61 +60,121 @@
     (len + c) as usize
   }
 }
 
 /// Replaces a substring in the meta variable's text content with another string.
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 #[serde(rename_all = "camelCase")]
-pub struct Replace {
+pub struct Replace<T> {
   /// source meta variable to be transformed
-  source: String,
+  source: T,
   /// a regex to find substring to be replaced
   replace: String,
   /// the replacement string
   by: String,
 }
-impl Replace {
+impl Replace<MetaVariable> {
   fn compute<D: Doc>(&self, ctx: &mut Ctx<D>) -> Option<String> {
     let text = get_text_from_env(&self.source, ctx)?;
     let re = Regex::new(&self.replace).unwrap();
     Some(re.replace_all(&text, &self.by).into_owned())
   }
 }
 
 /// Converts the source meta variable's text content to a specified case format.
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 #[serde(rename_all = "camelCase")]
-pub struct Convert {
+pub struct Convert<T> {
   /// source meta variable to be transformed
-  source: String,
+  source: T,
   /// the target case format to convert the text content to
   to_case: StringCase,
   /// optional separators to specify how to separate word
   separated_by: Option<Vec<Separator>>,
 }
-impl Convert {
+impl Convert<MetaVariable> {
   fn compute<D: Doc>(&self, ctx: &mut Ctx<D>) -> Option<String> {
     let text = get_text_from_env(&self.source, ctx)?;
     Some(self.to_case.apply(&text, self.separated_by.as_deref()))
   }
 }
 
 /// Represents a transformation that can be applied to a matched AST node.
 /// Available transformations are `substring`, `replace` and `convert`.
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 #[serde(rename_all = "camelCase")]
-pub enum Transformation {
-  Substring(Substring),
-  Replace(Replace),
-  Convert(Convert),
-  Rewrite(Rewrite),
+pub enum Transformation<T> {
+  Substring(Substring<T>),
+  Replace(Replace<T>),
+  Convert(Convert<T>),
+  Rewrite(Rewrite<T>),
+}
+
+pub(crate) fn parse_meta_var<L: Language>(
+  src: &str,
+  lang: &L,
+) -> Result<MetaVariable, TransformError> {
+  let source = lang.pre_process_pattern(src);
+  if let Some(var) = lang.extract_meta_var(&source) {
+    Ok(var)
+  } else {
+    Err(TransformError::MalformedVar(src.to_string()))
+  }
 }
 
-impl Transformation {
-  fn insert<D: Doc>(&self, key: &str, ctx: &mut Ctx<D>) {
+impl Transformation<String> {
+  pub fn parse<L: Language>(
+    &self,
+    lang: &L,
+  ) -> Result<Transformation<MetaVariable>, TransformError> {
+    use Transformation as T;
+    Ok(match self {
+      T::Replace(r) => T::Replace(Replace {
+        source: parse_meta_var(&r.source, lang)?,
+        replace: r.replace.clone(),
+        by: r.by.clone(),
+      }),
+      T::Substring(s) => T::Substring(Substring {
+        source: parse_meta_var(&s.source, lang)?,
+        start_char: s.start_char,
+        end_char: s.end_char,
+      }),
+      T::Convert(c) => T::Convert(Convert {
+        source: parse_meta_var(&c.source, lang)?,
+        to_case: c.to_case,
+        separated_by: c.separated_by.clone(),
+      }),
+      T::Rewrite(r) => T::Rewrite(r.parse(lang)?),
+    })
+  }
+
+  pub fn used_vars(&self) -> &str {
+    fn strip(s: &str) -> &str {
+      s.strip_prefix("$$$").unwrap_or_else(|| &s[1..])
+      // match s {
+      //   MetaVariable::Capture(s, _) => s,
+      //   MetaVariable::Dropped(_) => "",
+      //   MetaVariable::MultiCapture(s) => s,
+      //   MetaVariable::Multiple => "",
+      // }
+    }
+    use Transformation as T;
+    // NOTE: meta_var in transform always starts with `$`, for now
+    match self {
+      T::Replace(r) => strip(&r.source),
+      T::Substring(s) => strip(&s.source),
+      T::Convert(c) => strip(&c.source),
+      T::Rewrite(r) => strip(&r.source),
+    }
+  }
+}
+impl Transformation<MetaVariable> {
+  pub(super) fn insert<D: Doc>(&self, key: &str, ctx: &mut Ctx<D>) {
+    // TODO: add this debug assertion back
+    // debug_assert!(ctx.env.get_transformed(key).is_none());
     // avoid cyclic
     ctx.env.insert_transformation(key, vec![]);
     let opt = self.compute(ctx);
     let bytes = if let Some(s) = opt {
       <D::Source as Content>::decode_str(&s).to_vec()
     } else {
       vec![]
@@ -139,95 +187,63 @@
       T::Replace(r) => r.compute(ctx),
       T::Substring(s) => s.compute(ctx),
       T::Convert(c) => c.compute(ctx),
       T::Rewrite(r) => r.compute(ctx),
     }
   }
 
-  pub fn used_vars(&self) -> &str {
-    fn strip(s: &str) -> &str {
-      s.strip_prefix("$$$").unwrap_or_else(|| &s[1..])
-    }
-    use Transformation as T;
-    // NOTE: meta_var in transform always starts with `$`, for now
-    match self {
-      T::Replace(r) => strip(&r.source),
-      T::Substring(s) => strip(&s.source),
-      T::Convert(c) => strip(&c.source),
-      T::Rewrite(r) => strip(&r.source),
-    }
-  }
-
   pub fn used_rewriters(&self) -> &[String] {
     use Transformation as T;
     match self {
       T::Replace(_) => &[],
       T::Substring(_) => &[],
       T::Convert(_) => &[],
       T::Rewrite(r) => &r.rewriters,
     }
   }
 }
 
-// two lifetime to represent env root lifetime and lang/trans lifetime
-struct Ctx<'b, 'c, D: Doc> {
-  transforms: &'b HashMap<String, Transformation>,
-  lang: &'b D::Lang,
-  rewriters: GlobalRules<D::Lang>,
-  env: &'b mut MetaVarEnv<'c, D>,
-  enclosing_env: &'b MetaVarEnv<'c, D>,
-}
-
-pub fn apply_env_transform<'c, D: Doc>(
-  transforms: &HashMap<String, Transformation>,
-  lang: &D::Lang,
-  env: &mut MetaVarEnv<'c, D>,
-  rewriters: GlobalRules<D::Lang>,
-  enclosing_env: &MetaVarEnv<'c, D>,
-) {
-  let mut ctx = Ctx {
-    transforms,
-    lang,
-    env,
-    rewriters,
-    enclosing_env,
-  };
-  for (key, tr) in transforms {
-    tr.insert(key, &mut ctx);
-  }
-}
-
 #[cfg(test)]
 mod test {
+  use super::super::Transform;
   use super::*;
   use crate::test::TypeScript;
+  use crate::DeserializeEnv;
   use serde_yaml::with::singleton_map_recursive;
+  use std::collections::HashMap;
 
   type R = std::result::Result<(), ()>;
 
-  fn get_transformed(src: &str, pat: &str, trans: &Transformation) -> Option<String> {
+  fn get_transformed(src: &str, pat: &str, trans: &Transformation<String>) -> Option<String> {
     let grep = TypeScript::Tsx.ast_grep(src);
     let root = grep.root();
     let mut nm = root.find(pat).expect("should find");
     let mut ctx = Ctx {
-      lang: &TypeScript::Tsx,
-      transforms: &HashMap::new(),
       env: nm.get_env_mut(),
-      rewriters: Default::default(),
+      rewriters: &Default::default(),
       enclosing_env: &Default::default(),
     };
-    trans.compute(&mut ctx)
+    trans.parse(&TypeScript::Tsx).ok()?.compute(&mut ctx)
   }
 
-  fn parse(trans: &str) -> Result<Transformation, ()> {
+  fn parse(trans: &str) -> Result<Transformation<String>, ()> {
     let deserializer = serde_yaml::Deserializer::from_str(trans);
     singleton_map_recursive::deserialize(deserializer).map_err(|_| ())
   }
 
   #[test]
+  fn test_transform_parse_error() {
+    let str_trans = parse(r#"substring: { source: WRONG }"#).expect("should work");
+    match str_trans.parse(&TypeScript::Tsx) {
+      Err(TransformError::MalformedVar(n)) => assert_eq!(n, "WRONG"),
+      _ => panic!("should be malformed var"),
+    }
+  }
+
+  #[test]
   fn test_simple_replace() -> R {
     let trans = parse(
       r#"
       substring:
         source: "$A"
         startChar: 1
         endChar: -1
@@ -287,25 +303,21 @@
       replace:
         source: "$A"
     "#,
     );
     assert!(parsed.is_err());
   }
 
-  fn transform_env(trans: HashMap<String, Transformation>) -> HashMap<String, String> {
+  fn transform_env(trans: HashMap<String, Transformation<String>>) -> HashMap<String, String> {
     let grep = TypeScript::Tsx.ast_grep("let a = 123");
     let root = grep.root();
     let mut nm = root.find("let a = $A").expect("should find");
-    apply_env_transform(
-      &trans,
-      &TypeScript::Tsx,
-      nm.get_env_mut(),
-      Default::default(),
-      &Default::default(),
-    );
+    let env = DeserializeEnv::new(TypeScript::Tsx);
+    let trans = Transform::deserialize(&trans, &env).expect("should deserialize");
+    trans.apply_transform(nm.get_env_mut(), &Default::default(), &Default::default());
     nm.get_env().clone().into()
   }
 
   #[test]
   fn test_insert_env() -> R {
     let tr1 = parse(
       r#"
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.21.4/crates/config/src/transform/rewrite.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 use super::Ctx;
+use super::{transformation::parse_meta_var, TransformError};
 use crate::rule_core::RuleCore;
 
 use ast_grep_core::meta_var::MetaVariable;
 use ast_grep_core::source::{Content, Edit};
 use ast_grep_core::{Doc, Language, Node, NodeMatch};
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 
 #[derive(Serialize, Deserialize, Clone, JsonSchema)]
 #[serde(rename_all = "camelCase")]
-pub struct Rewrite {
-  pub(super) source: String,
+pub struct Rewrite<T> {
+  pub(super) source: T,
   pub(super) rewriters: Vec<String>,
   // do we need this?
   // sort_by: Option<String>,
-  join_by: Option<String>,
+  pub(super) join_by: Option<String>,
 }
 
 fn get_nodes_from_env<'b, D: Doc>(var: &MetaVariable, ctx: &Ctx<'_, 'b, D>) -> Vec<Node<'b, D>> {
   match var {
     MetaVariable::MultiCapture(n) => ctx.env.get_multiple_matches(n),
     MetaVariable::Capture(m, _) => {
       if let Some(n) = ctx.env.get_match(m) {
@@ -26,30 +27,39 @@
       } else {
         vec![]
       }
     }
     _ => vec![],
   }
 }
+impl Rewrite<String> {
+  pub fn parse<L: Language>(&self, lang: &L) -> Result<Rewrite<MetaVariable>, TransformError> {
+    let source = parse_meta_var(&self.source, lang)?;
+    Ok(Rewrite {
+      source,
+      rewriters: self.rewriters.clone(),
+      join_by: self.join_by.clone(),
+    })
+  }
+}
 
-impl Rewrite {
+impl Rewrite<MetaVariable> {
   pub(super) fn compute<D: Doc>(&self, ctx: &mut Ctx<D>) -> Option<String> {
-    let source = ctx.lang.pre_process_pattern(&self.source);
-    let var = ctx.lang.extract_meta_var(&source)?;
-    let nodes = get_nodes_from_env(&var, ctx);
+    let var = &self.source;
+    let nodes = get_nodes_from_env(var, ctx);
     if nodes.is_empty() {
       return None;
     }
-    let rewriters = ctx.rewriters.read();
+    let rewriters = ctx.rewriters;
     let start = nodes[0].range().start;
-    let bytes = ctx.env.get_var_bytes(&var)?;
+    let bytes = ctx.env.get_var_bytes(var)?;
     let rules: Vec<_> = self
       .rewriters
       .iter()
-      .filter_map(|id| rewriters.get(id)) // TODO: better handling
+      .filter_map(|id| rewriters.get(id)) // NOTE: rewriter must be defined
       .collect();
     let edits = find_and_make_edits(nodes, &rules, ctx);
     let rewritten = if let Some(joiner) = &self.join_by {
       let mut ret = vec![];
       let mut edits = edits.into_iter();
       if let Some(first) = edits.next() {
         let mut pos = first.position - start + first.deleted_length;
@@ -101,15 +111,15 @@
       // but match env will NOT inherited recursively!
       // e.g. $B is matched in parent linter and it is inherited.
       // $C is matched in rewriter but is NOT inherited in recursive rewriter
       // this is to enable recursive rewriter to match sub nodes
       // in future, we can use the explict `expose` to control env inheritance
       if let Some(n) = rule.do_match(child.clone(), &mut env, Some(ctx.enclosing_env)) {
         let nm = NodeMatch::new(n, env.into_owned());
-        edits.push(nm.make_edit(rule, rule.fixer.as_ref().expect("TODO")));
+        edits.push(nm.make_edit(rule, rule.fixer.as_ref().expect("rewriter must have fix")));
         // stop at first fix, skip duplicate fix
         break;
       }
     }
   }
   edits
 }
@@ -135,23 +145,24 @@
   new_content.extend_from_slice(&old_content[start..]);
   new_content
 }
 
 #[cfg(test)]
 mod test {
   use super::*;
+  use crate::check_var::CheckHint;
   use crate::from_str;
   use crate::rule::DeserializeEnv;
   use crate::rule_core::SerializableRuleCore;
   use crate::test::TypeScript;
   use crate::GlobalRules;
   use std::collections::HashSet;
 
   fn apply_transformation(
-    rewrite: Rewrite,
+    rewrite: Rewrite<String>,
     src: &str,
     pat: &str,
     rewriters: GlobalRules<TypeScript>,
   ) -> String {
     compute_rewritten(src, pat, rewrite, rewriters).expect("should have transforms")
   }
 
@@ -167,15 +178,17 @@
     pairs: &[(&str, &str)],
     vars: HashSet<&str>,
   ) -> GlobalRules<TypeScript> {
     let rewriters = GlobalRules::default();
     for (key, ser) in pairs {
       let serialized: SerializableRuleCore = from_str(ser).unwrap();
       let env = DeserializeEnv::new(TypeScript::Tsx).with_rewriters(&rewriters);
-      let rule = serialized.get_rewriter(env, &vars).unwrap();
+      let rule = serialized
+        .get_matcher_with_hint(env, CheckHint::Rewriter(&vars))
+        .unwrap();
       rewriters.insert(key, rule).unwrap();
     }
     rewriters
   }
 
   #[test]
   fn test_perform_one_rewrite() {
@@ -327,31 +340,30 @@
     let ret = apply_transformation(rewrite, "[1, 2]", "[$A, $C]", rewriters);
     assert_eq!(ret, "1 == 2");
   }
 
   fn compute_rewritten(
     src: &str,
     pat: &str,
-    rewrite: Rewrite,
+    rewrite: Rewrite<String>,
     rewriters: GlobalRules<TypeScript>,
   ) -> Option<String> {
     let grep = TypeScript::Tsx.ast_grep(src);
     let root = grep.root();
     let mut nm = root.find(pat).expect("should find");
     let before_vars: Vec<_> = nm.get_env().get_matched_variables().collect();
     let env = nm.get_env_mut();
     let enclosing = env.clone();
+    let rewriters = rewriters.read();
     let mut ctx = Ctx {
-      lang: &TypeScript::Tsx,
-      transforms: &Default::default(),
       env,
-      rewriters,
+      rewriters: &rewriters,
       enclosing_env: &enclosing,
     };
     let after_vars: Vec<_> = ctx.env.get_matched_variables().collect();
     assert_eq!(
       before_vars, after_vars,
       "rewrite should not write back to env"
     );
-    rewrite.compute(&mut ctx)
+    rewrite.parse(&TypeScript::Tsx).ok()?.compute(&mut ctx)
   }
 }
```

### Comparing `ast_grep_py-0.21.3/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.21.4/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/Cargo.toml` & `ast_grep_py-0.21.4/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/language.rs` & `ast_grep_py-0.21.4/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/lib.rs` & `ast_grep_py-0.21.4/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/match_tree.rs` & `ast_grep_py-0.21.4/crates/core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.21.4/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.21.4/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.21.4/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/matcher/text.rs` & `ast_grep_py-0.21.4/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/matcher.rs` & `ast_grep_py-0.21.4/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/meta_var.rs` & `ast_grep_py-0.21.4/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/node.rs` & `ast_grep_py-0.21.4/crates/core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/ops.rs` & `ast_grep_py-0.21.4/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/pinned.rs` & `ast_grep_py-0.21.4/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.21.4/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.21.4/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/replacer/template.rs` & `ast_grep_py-0.21.4/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/replacer.rs` & `ast_grep_py-0.21.4/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/source.rs` & `ast_grep_py-0.21.4/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/core/src/traversal.rs` & `ast_grep_py-0.21.4/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/Cargo.toml` & `ast_grep_py-0.21.4/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/README.md` & `ast_grep_py-0.21.4/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.21.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/src/lib.rs` & `ast_grep_py-0.21.4/crates/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.21.4/crates/pyo3/src/py_node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/src/range.rs` & `ast_grep_py-0.21.4/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.21.4/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.21.4/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.21.4/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.21.4/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.21.4/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/Cargo.lock` & `ast_grep_py-0.21.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -139,15 +139,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -155,38 +155,38 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
@@ -208,29 +208,29 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -240,15 +240,15 @@
  "tree-sitter-html",
  "tree-sitter-javascript",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
@@ -306,15 +306,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.21.3"
+version = "0.21.4"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -954,15 +954,15 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
@@ -1490,26 +1490,26 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `ast_grep_py-0.21.3/Cargo.toml` & `ast_grep_py-0.21.4/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.21.3"
+version = "0.21.4"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.21.3" }
-ast-grep-config = { path = "crates/config", version = "0.21.3" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.21.3" }
-ast-grep-language = { path = "crates/language", version = "0.21.3" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.21.3" }
+ast-grep-core = { path = "crates/core", version = "0.21.4" }
+ast-grep-config = { path = "crates/config", version = "0.21.4" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.21.4" }
+ast-grep-language = { path = "crates/language", version = "0.21.4" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.21.4" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
-serde = { version = "1.0", features = ["derive"] }
+serde = { version = "1.0.200", features = ["derive"] }
 tree-sitter = { version = "0.9.2", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
 schemars = "0.8.17"
 anyhow = "1.0.82"
```

### Comparing `ast_grep_py-0.21.3/pyproject.toml` & `ast_grep_py-0.21.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.21.3"
+version = "0.21.4"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.21.3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.21.4/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/ast_grep_py/__init__.py` & `ast_grep_py-0.21.4/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/README.md` & `ast_grep_py-0.21.4/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.3/PKG-INFO` & `ast_grep_py-0.21.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.21.3
+Version: 0.21.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

