# Comparing `tmp/cog-0.9.6-py3-none-any.whl.zip` & `tmp/cog-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,110 +1,111 @@
-Zip file size: 95519 bytes, number of entries: 108
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-19 20:25 cog/.gitignore
--rw-r--r--  2.0 unx      362 b- defN 24-Apr-19 20:25 cog/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Apr-19 20:25 cog/_version.py
--rw-r--r--  2.0 unx    10313 b- defN 24-Apr-19 20:25 cog/code_xforms.py
--rw-r--r--  2.0 unx      286 b- defN 24-Apr-19 20:25 cog/errors.py
--rw-r--r--  2.0 unx     2124 b- defN 24-Apr-19 20:25 cog/files.py
--rw-r--r--  2.0 unx     1945 b- defN 24-Apr-19 20:25 cog/json.py
--rw-r--r--  2.0 unx     3171 b- defN 24-Apr-19 20:25 cog/logging.py
--rw-r--r--  2.0 unx    17091 b- defN 24-Apr-19 20:25 cog/predictor.py
--rw-r--r--  2.0 unx     3308 b- defN 24-Apr-19 20:25 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 24-Apr-19 20:25 cog/suppress_output.py
--rw-r--r--  2.0 unx     8587 b- defN 24-Apr-19 20:25 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 cog/command/__init__.py
--rw-r--r--  2.0 unx    18782 b- defN 24-Apr-19 20:25 cog/command/ast_openapi_schema.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-19 20:25 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 24-Apr-19 20:25 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 24-Apr-19 20:25 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5349 b- defN 24-Apr-19 20:25 cog/server/helpers.py
--rw-r--r--  2.0 unx    16945 b- defN 24-Apr-19 20:25 cog/server/http.py
--rw-r--r--  2.0 unx      971 b- defN 24-Apr-19 20:25 cog/server/probes.py
--rw-r--r--  2.0 unx      689 b- defN 24-Apr-19 20:25 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    15515 b- defN 24-Apr-19 20:25 cog/server/runner.py
--rw-r--r--  2.0 unx     3326 b- defN 24-Apr-19 20:25 cog/server/webhook.py
--rw-r--r--  2.0 unx     8050 b- defN 24-Apr-19 20:25 cog/server/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 24-Apr-19 20:25 tests/conftest.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-19 20:25 tests/test_json.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-19 20:25 tests/test_predictor.py
--rw-r--r--  2.0 unx     4689 b- defN 24-Apr-19 20:25 tests/test_types.py
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-19 20:25 tests/fixtures/argv_override.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/server/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 24-Apr-19 20:25 tests/server/conftest.py
--rw-r--r--  2.0 unx     2564 b- defN 24-Apr-19 20:25 tests/server/test_code_xforms.py
--rw-r--r--  2.0 unx     4692 b- defN 24-Apr-19 20:25 tests/server/test_helpers.py
--rw-r--r--  2.0 unx    16956 b- defN 24-Apr-19 20:25 tests/server/test_http.py
--rw-r--r--  2.0 unx     8821 b- defN 24-Apr-19 20:25 tests/server/test_http_input.py
--rw-r--r--  2.0 unx     4020 b- defN 24-Apr-19 20:25 tests/server/test_http_output.py
--rw-r--r--  2.0 unx     2775 b- defN 24-Apr-19 20:25 tests/server/test_predictor.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-19 20:25 tests/server/test_probes.py
--rw-r--r--  2.0 unx     1210 b- defN 24-Apr-19 20:25 tests/server/test_response_throttler.py
--rw-r--r--  2.0 unx    10931 b- defN 24-Apr-19 20:25 tests/server/test_runner.py
--rw-r--r--  2.0 unx     3225 b- defN 24-Apr-19 20:25 tests/server/test_webhook.py
--rw-r--r--  2.0 unx    16162 b- defN 24-Apr-19 20:25 tests/server/test_worker.py
--rw-r--r--  2.0 unx      209 b- defN 24-Apr-19 20:25 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-19 20:25 tests/server/fixtures/catch_in_predict.py
--rw-r--r--  2.0 unx      232 b- defN 24-Apr-19 20:25 tests/server/fixtures/complex_output.py
--rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 20:25 tests/server/fixtures/count_up.py
--rw-r--r--  2.0 unx      136 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_predict.py
--rw-r--r--  2.0 unx      133 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_setup.py
--rw-r--r--  2.0 unx      151 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_setup_and_predict.py
--rw-r--r--  2.0 unx       56 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_on_import.py
--rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_in_predict.py
--rw-r--r--  2.0 unx      124 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_in_setup.py
--rw-r--r--  2.0 unx       23 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_on_import.py
--rw-r--r--  2.0 unx       58 b- defN 24-Apr-19 20:25 tests/server/fixtures/function.py
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-19 20:25 tests/server/fixtures/hello_world.py
--rw-r--r--  2.0 unx      197 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_choices_integer.py
--rw-r--r--  2.0 unx      139 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_file.py
--rw-r--r--  2.0 unx      160 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_ge_le.py
--rw-r--r--  2.0 unx      126 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_integer.py
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_integer_default.py
--rw-r--r--  2.0 unx      317 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_multiple.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_none.py
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_path.py
--rw-r--r--  2.0 unx      137 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_path_2.py
--rw-r--r--  2.0 unx      125 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_string.py
--rw-r--r--  2.0 unx      262 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_union_integer_or_list_of_integers.py
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_union_string_or_list_of_strings.py
--rw-r--r--  2.0 unx      205 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_unsupported_type.py
--rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_untyped.py
--rw-r--r--  2.0 unx      160 b- defN 24-Apr-19 20:25 tests/server/fixtures/killed_in_predict.py
--rw-r--r--  2.0 unx      882 b- defN 24-Apr-19 20:25 tests/server/fixtures/logging.py
--rw-r--r--  2.0 unx      109 b- defN 24-Apr-19 20:25 tests/server/fixtures/missing_predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/server/fixtures/missing_predictor.py
--rw-r--r--  2.0 unx      482 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_complex_input.py
--rw-r--r--  2.0 unx      332 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_custom_output_type.py
--rw-r--r--  2.0 unx      169 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_input_int_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_list.py
--rw-r--r--  2.0 unx      374 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_type.py
--rw-r--r--  2.0 unx      161 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_yield.py
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_complex.py
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_file.py
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_file_named.py
--rw-r--r--  2.0 unx      257 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_iterator_complex.py
--rw-r--r--  2.0 unx      151 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_numpy.py
--rw-r--r--  2.0 unx      355 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_path_image.py
--rw-r--r--  2.0 unx      323 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_path_text.py
--rw-r--r--  2.0 unx      115 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_wrong_type.py
--rw-r--r--  2.0 unx      175 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup.py
--rw-r--r--  2.0 unx      262 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup_uses_async.py
--rw-r--r--  2.0 unx      167 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup_weights.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-19 20:25 tests/server/fixtures/simple.py
--rw-r--r--  2.0 unx      193 b- defN 24-Apr-19 20:25 tests/server/fixtures/sleep.py
--rw-r--r--  2.0 unx      219 b- defN 24-Apr-19 20:25 tests/server/fixtures/slow_predict.py
--rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/slow_setup.py
--rw-r--r--  2.0 unx      290 b- defN 24-Apr-19 20:25 tests/server/fixtures/steps.py
--rw-r--r--  2.0 unx      359 b- defN 24-Apr-19 20:25 tests/server/fixtures/train.py
--rw-r--r--  2.0 unx      263 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_concatenate_iterator.py
--rw-r--r--  2.0 unx      506 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_files.py
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_strings.py
--rw-r--r--  2.0 unx      339 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_strings_file_input.py
--rw-r--r--  2.0 unx    11347 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    36704 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9536 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/RECORD
-108 files, 274299 bytes uncompressed, 80257 bytes compressed:  70.7%
+Zip file size: 96039 bytes, number of entries: 109
+-rw-r--r--  2.0 unx       13 b- defN 24-May-06 20:09 cog/.gitignore
+-rw-r--r--  2.0 unx      384 b- defN 24-May-06 20:09 cog/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-06 20:10 cog/_version.py
+-rw-r--r--  2.0 unx    10313 b- defN 24-May-06 20:09 cog/code_xforms.py
+-rw-r--r--  2.0 unx      286 b- defN 24-May-06 20:09 cog/errors.py
+-rw-r--r--  2.0 unx     2124 b- defN 24-May-06 20:09 cog/files.py
+-rw-r--r--  2.0 unx     1945 b- defN 24-May-06 20:09 cog/json.py
+-rw-r--r--  2.0 unx     3171 b- defN 24-May-06 20:09 cog/logging.py
+-rw-r--r--  2.0 unx    17163 b- defN 24-May-06 20:09 cog/predictor.py
+-rw-r--r--  2.0 unx     3308 b- defN 24-May-06 20:09 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 24-May-06 20:09 cog/suppress_output.py
+-rw-r--r--  2.0 unx     8993 b- defN 24-May-06 20:09 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 cog/command/__init__.py
+-rw-r--r--  2.0 unx    18782 b- defN 24-May-06 20:09 cog/command/ast_openapi_schema.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-06 20:09 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 24-May-06 20:09 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 24-May-06 20:09 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5349 b- defN 24-May-06 20:09 cog/server/helpers.py
+-rw-r--r--  2.0 unx    16945 b- defN 24-May-06 20:09 cog/server/http.py
+-rw-r--r--  2.0 unx      971 b- defN 24-May-06 20:09 cog/server/probes.py
+-rw-r--r--  2.0 unx      689 b- defN 24-May-06 20:09 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    15515 b- defN 24-May-06 20:09 cog/server/runner.py
+-rw-r--r--  2.0 unx     3326 b- defN 24-May-06 20:09 cog/server/webhook.py
+-rw-r--r--  2.0 unx     8050 b- defN 24-May-06 20:09 cog/server/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 24-May-06 20:09 tests/conftest.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-06 20:09 tests/test_json.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-06 20:09 tests/test_predictor.py
+-rw-r--r--  2.0 unx     4895 b- defN 24-May-06 20:09 tests/test_types.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-06 20:09 tests/fixtures/argv_override.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/server/__init__.py
+-rw-r--r--  2.0 unx     2800 b- defN 24-May-06 20:09 tests/server/conftest.py
+-rw-r--r--  2.0 unx     2564 b- defN 24-May-06 20:09 tests/server/test_code_xforms.py
+-rw-r--r--  2.0 unx     4692 b- defN 24-May-06 20:09 tests/server/test_helpers.py
+-rw-r--r--  2.0 unx    16956 b- defN 24-May-06 20:09 tests/server/test_http.py
+-rw-r--r--  2.0 unx     9181 b- defN 24-May-06 20:09 tests/server/test_http_input.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-06 20:09 tests/server/test_http_output.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-May-06 20:09 tests/server/test_predictor.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-06 20:09 tests/server/test_probes.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-May-06 20:09 tests/server/test_response_throttler.py
+-rw-r--r--  2.0 unx    10931 b- defN 24-May-06 20:09 tests/server/test_runner.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-May-06 20:09 tests/server/test_webhook.py
+-rw-r--r--  2.0 unx    16162 b- defN 24-May-06 20:09 tests/server/test_worker.py
+-rw-r--r--  2.0 unx      209 b- defN 24-May-06 20:09 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
+-rw-r--r--  2.0 unx      198 b- defN 24-May-06 20:09 tests/server/fixtures/catch_in_predict.py
+-rw-r--r--  2.0 unx      232 b- defN 24-May-06 20:09 tests/server/fixtures/complex_output.py
+-rw-r--r--  2.0 unx      131 b- defN 24-May-06 20:09 tests/server/fixtures/count_up.py
+-rw-r--r--  2.0 unx      136 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_predict.py
+-rw-r--r--  2.0 unx      133 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_setup.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-06 20:09 tests/server/fixtures/exc_in_setup_and_predict.py
+-rw-r--r--  2.0 unx       56 b- defN 24-May-06 20:09 tests/server/fixtures/exc_on_import.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/exit_in_predict.py
+-rw-r--r--  2.0 unx      124 b- defN 24-May-06 20:09 tests/server/fixtures/exit_in_setup.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-06 20:09 tests/server/fixtures/exit_on_import.py
+-rw-r--r--  2.0 unx       58 b- defN 24-May-06 20:09 tests/server/fixtures/function.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-06 20:09 tests/server/fixtures/hello_world.py
+-rw-r--r--  2.0 unx      197 b- defN 24-May-06 20:09 tests/server/fixtures/input_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-06 20:09 tests/server/fixtures/input_choices_integer.py
+-rw-r--r--  2.0 unx      139 b- defN 24-May-06 20:09 tests/server/fixtures/input_file.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-06 20:09 tests/server/fixtures/input_ge_le.py
+-rw-r--r--  2.0 unx      126 b- defN 24-May-06 20:09 tests/server/fixtures/input_integer.py
+-rw-r--r--  2.0 unx      152 b- defN 24-May-06 20:09 tests/server/fixtures/input_integer_default.py
+-rw-r--r--  2.0 unx      317 b- defN 24-May-06 20:09 tests/server/fixtures/input_multiple.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-06 20:09 tests/server/fixtures/input_none.py
+-rw-r--r--  2.0 unx      236 b- defN 24-May-06 20:09 tests/server/fixtures/input_path.py
+-rw-r--r--  2.0 unx      137 b- defN 24-May-06 20:09 tests/server/fixtures/input_path_2.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-06 20:09 tests/server/fixtures/input_secret.py
+-rw-r--r--  2.0 unx      125 b- defN 24-May-06 20:09 tests/server/fixtures/input_string.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-06 20:09 tests/server/fixtures/input_union_integer_or_list_of_integers.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-06 20:09 tests/server/fixtures/input_union_string_or_list_of_strings.py
+-rw-r--r--  2.0 unx      205 b- defN 24-May-06 20:09 tests/server/fixtures/input_unsupported_type.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/input_untyped.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-06 20:09 tests/server/fixtures/killed_in_predict.py
+-rw-r--r--  2.0 unx      882 b- defN 24-May-06 20:09 tests/server/fixtures/logging.py
+-rw-r--r--  2.0 unx      109 b- defN 24-May-06 20:09 tests/server/fixtures/missing_predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 20:09 tests/server/fixtures/missing_predictor.py
+-rw-r--r--  2.0 unx      482 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_complex_input.py
+-rw-r--r--  2.0 unx      332 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_custom_output_type.py
+-rw-r--r--  2.0 unx      169 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_input_int_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_list.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_type.py
+-rw-r--r--  2.0 unx      161 b- defN 24-May-06 20:09 tests/server/fixtures/openapi_output_yield.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-06 20:09 tests/server/fixtures/output_complex.py
+-rw-r--r--  2.0 unx      148 b- defN 24-May-06 20:09 tests/server/fixtures/output_file.py
+-rw-r--r--  2.0 unx      192 b- defN 24-May-06 20:09 tests/server/fixtures/output_file_named.py
+-rw-r--r--  2.0 unx      257 b- defN 24-May-06 20:09 tests/server/fixtures/output_iterator_complex.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-06 20:09 tests/server/fixtures/output_numpy.py
+-rw-r--r--  2.0 unx      355 b- defN 24-May-06 20:09 tests/server/fixtures/output_path_image.py
+-rw-r--r--  2.0 unx      323 b- defN 24-May-06 20:09 tests/server/fixtures/output_path_text.py
+-rw-r--r--  2.0 unx      115 b- defN 24-May-06 20:09 tests/server/fixtures/output_wrong_type.py
+-rw-r--r--  2.0 unx      175 b- defN 24-May-06 20:09 tests/server/fixtures/setup.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-06 20:09 tests/server/fixtures/setup_uses_async.py
+-rw-r--r--  2.0 unx      167 b- defN 24-May-06 20:09 tests/server/fixtures/setup_weights.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-06 20:09 tests/server/fixtures/simple.py
+-rw-r--r--  2.0 unx      193 b- defN 24-May-06 20:09 tests/server/fixtures/sleep.py
+-rw-r--r--  2.0 unx      219 b- defN 24-May-06 20:09 tests/server/fixtures/slow_predict.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-06 20:09 tests/server/fixtures/slow_setup.py
+-rw-r--r--  2.0 unx      290 b- defN 24-May-06 20:09 tests/server/fixtures/steps.py
+-rw-r--r--  2.0 unx      359 b- defN 24-May-06 20:09 tests/server/fixtures/train.py
+-rw-r--r--  2.0 unx      263 b- defN 24-May-06 20:09 tests/server/fixtures/yield_concatenate_iterator.py
+-rw-r--r--  2.0 unx      506 b- defN 24-May-06 20:09 tests/server/fixtures/yield_files.py
+-rw-r--r--  2.0 unx      245 b- defN 24-May-06 20:09 tests/server/fixtures/yield_strings.py
+-rw-r--r--  2.0 unx      339 b- defN 24-May-06 20:09 tests/server/fixtures/yield_strings_file_input.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    36704 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9629 b- defN 24-May-06 20:10 cog-0.9.7.dist-info/RECORD
+109 files, 275617 bytes uncompressed, 80627 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -195,14 +195,17 @@
 
 Filename: tests/server/fixtures/input_path.py
 Comment: 
 
 Filename: tests/server/fixtures/input_path_2.py
 Comment: 
 
+Filename: tests/server/fixtures/input_secret.py
+Comment: 
+
 Filename: tests/server/fixtures/input_string.py
 Comment: 
 
 Filename: tests/server/fixtures/input_union_integer_or_list_of_integers.py
 Comment: 
 
 Filename: tests/server/fixtures/input_union_string_or_list_of_strings.py
@@ -303,23 +306,23 @@
 
 Filename: tests/server/fixtures/yield_strings.py
 Comment: 
 
 Filename: tests/server/fixtures/yield_strings_file_input.py
 Comment: 
 
-Filename: cog-0.9.6.dist-info/LICENSE
+Filename: cog-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.9.6.dist-info/METADATA
+Filename: cog-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.9.6.dist-info/WHEEL
+Filename: cog-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.9.6.dist-info/top_level.txt
+Filename: cog-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.9.6.dist-info/RECORD
+Filename: cog-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/__init__.py

```diff
@@ -1,11 +1,11 @@
 from pydantic import BaseModel
 
 from .predictor import BasePredictor
-from .types import ConcatenateIterator, File, Input, Path
+from .types import ConcatenateIterator, File, Input, Path, Secret
 
 try:
     from ._version import __version__
 except ImportError:
     __version__ = "0.0.0+unknown"
 
 
@@ -13,8 +13,9 @@
     "__version__",
     "BaseModel",
     "BasePredictor",
     "ConcatenateIterator",
     "File",
     "Input",
     "Path",
+    "Secret",
 ]
```

## cog/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.6'
-__version_tuple__ = version_tuple = (0, 9, 6)
+__version__ = version = '0.9.7'
+__version_tuple__ = version_tuple = (0, 9, 7)
```

## cog/predictor.py

```diff
@@ -41,21 +41,28 @@
 from .types import (
     File as CogFile,
 )
 from .types import (
     Input,
     URLPath,
 )
-from .types import (
-    Path as CogPath,
-)
+from .types import Path as CogPath
+from .types import Secret as CogSecret
 
 log = structlog.get_logger("cog.server.predictor")
 
-ALLOWED_INPUT_TYPES: List[Type[Any]] = [str, int, float, bool, CogFile, CogPath]
+ALLOWED_INPUT_TYPES: List[Type[Any]] = [
+    str,
+    int,
+    float,
+    bool,
+    CogFile,
+    CogPath,
+    CogSecret,
+]
 
 
 class BasePredictor(ABC):
     def setup(self, weights: Optional[Union[CogFile, CogPath, str]] = None) -> None:
         """
         An optional method to prepare the model so multiple predictions run efficiently.
         """
```

## cog/types.py

```diff
@@ -5,15 +5,15 @@
 import shutil
 import tempfile
 import urllib.parse
 import urllib.request
 from typing import Any, Dict, Iterator, List, Optional, TypeVar, Union
 
 import requests
-from pydantic import Field
+from pydantic import Field, SecretStr
 
 FILENAME_ILLEGAL_CHARS = set("\u0000/")
 
 # Linux allows files up to 255 bytes long. We enforce a slightly shorter
 # filename so that there's room for prefixes added by
 # tempfile.NamedTemporaryFile, etc.
 FILENAME_MAX_LENGTH = 200
@@ -38,15 +38,30 @@
         min_length=min_length,
         max_length=max_length,
         regex=regex,
         choices=choices,
     )
 
 
+class Secret(SecretStr):
+    @classmethod
+    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
+        """Defines what this type should be in openapi.json"""
+        field_schema.update(
+            {
+                "type": "string",
+                "format": "password",
+                "x-cog-secret": True,
+            }
+        )
+
+
 class File(io.IOBase):
+    """Deprecated: use Path instead."""
+
     validate_always = True
 
     @classmethod
     def __get_validators__(cls) -> Iterator[Any]:
         yield cls.validate
 
     @classmethod
```

## tests/test_types.py

```diff
@@ -1,13 +1,13 @@
 import io
 import pickle
 
 import pytest
 import responses
-from cog.types import URLFile, get_filename
+from cog.types import Secret, URLFile, get_filename
 
 
 @responses.activate
 def test_urlfile_acts_like_response():
     responses.get(
         "https://example.com/some/url",
         json={"message": "hello world"},
@@ -115,7 +115,15 @@
             "https://coppermerchants.example/complaints/𒀀𒈾𒂍𒀀𒈾𒍢𒅕𒆠𒉈𒈠𒌝𒈠𒈾𒀭𒉌𒈠𒀀𒉡𒌑𒈠𒋫𒀠𒇷𒆪𒆠𒀀𒄠𒋫𒀝𒁉𒄠𒌝𒈠𒀜𒋫𒀀𒈠𒄖𒁀𒊑𒁕𒄠𒆪𒁴𒀀𒈾𒄀𒅖𒀭𒂗𒍪𒀀𒈾𒀜𒁲𒅔𒋫𒀠𒇷𒅅𒈠𒋫𒀝𒁉𒀀𒄠.tablet",
             "𒀀𒈾𒂍𒀀𒈾𒍢𒅕𒆠𒉈𒈠𒌝𒈠𒈾𒀭𒉌𒈠𒀀𒉡𒌑𒈠𒋫𒀠𒇷𒆪𒆠𒀀𒄠𒋫𒀝𒁉𒄠𒌝𒈠𒀜𒋫𒀀𒈠𒄖𒁀𒊑𒁕𒄠𒆪𒁴𒀀𒈾𒄀𒅖~.tablet",
         ),
     ],
 )
 def test_get_filename(url, filename):
     assert get_filename(url) == filename
+
+
+def test_secret_type():
+    secret_value = "sw0rdf1$h"  # noqa: S105
+    secret = Secret(secret_value)
+
+    assert secret.get_secret_value() == secret_value
+    assert str(secret) == "**********"
```

## tests/server/test_http_input.py

```diff
@@ -238,14 +238,24 @@
 
     resp = client.post("/predictions", json={"input": {"args": "abc"}})
     assert resp.status_code == 422
     resp = client.post("/predictions", json={"input": {"args": ["a", "b", "c"]}})
     assert resp.status_code == 422
 
 
+@uses_predictor("input_secret")
+def test_secret_str(client, match):
+    resp = client.post("/predictions", json={"input": {"secret": "foo"}})
+    assert resp.status_code == 200
+    assert resp.json() == match({"output": "foo", "status": "succeeded"})
+
+    resp = client.post("/predictions", json={"input": {"secret": {}}})
+    assert resp.status_code == 422
+
+
 def test_untyped_inputs():
     config = {"predict": _fixture_path("input_untyped")}
     app = create_app(
         config=config,
         shutdown_event=threading.Event(),
         upload_url="input_untyped",
     )
```

## Comparing `cog-0.9.6.dist-info/LICENSE` & `cog-0.9.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.9.6.dist-info/METADATA` & `cog-0.9.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.9.6
+Version: 0.9.7
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `cog-0.9.6.dist-info/RECORD` & `cog-0.9.7.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 cog/.gitignore,sha256=OIzCsCr9oYv3wBtJU_TppxWi-OhuDmwCBrrUqcE6kfY,13
-cog/__init__.py,sha256=qDIBBVsf5tfoaCGu49zQyYQb_AWtCwIxQrp9RLZlbbI,362
-cog/_version.py,sha256=11ciOFzse5i9Y6lr7kosD6U2UdIm5Bsf7hdpK0Hg_2I,411
+cog/__init__.py,sha256=QcRZ-RsRIoasGN4JsxgKSxfhtMyWbiOCn0sjQAQimB4,384
+cog/_version.py,sha256=4XC29QIe8f6Nj4TIXVcWdhsy0tKD5guALT5XGZC9sso,411
 cog/code_xforms.py,sha256=ZCiXn1bN5fIoY_GU91mwNeZr7B4rmE_GXiJVcZONyaM,10313
 cog/errors.py,sha256=pB29TjzvXmyqbqi3zPOlLobFJnVWb6GJ9WsLE-77TIQ,286
 cog/files.py,sha256=8PENbdvtuVl6sbgsoZSAHId60TSM8iU-dNMpNPS9h1A,2124
 cog/json.py,sha256=xNwlgqYY7egcHZzcWs94S17q3KbtZVyaDe5gCyZG-Vo,1945
 cog/logging.py,sha256=3I7jOG1HKU5oh6-xJF1dh_qFMJMBrjo9Z60zM6sr3qU,3171
-cog/predictor.py,sha256=JIgJzax9smlIDH-bax0PSY31NoUiD6b_92eOvgEFMfY,17091
+cog/predictor.py,sha256=4L5lGT89FJAeCo0n4GzM4zy0wwFSEc-1OuokEd2J2AE,17163
 cog/schema.py,sha256=NaVXnqMQ-duhWkS8vomg2NrXhdLn9nEkFKHPnhRtb7A,3308
 cog/suppress_output.py,sha256=HHSNGR9j4rkyLL4mGnkluxzSQAYYIUcEWGdNCtYfwZc,645
-cog/types.py,sha256=nYMt6hHND-tEvfdvKXoBEzRwatBrKKHHPxJDVZnOUAI,8587
+cog/types.py,sha256=aDKkuYeG55HNVo3JDzo_iFsxbznrZfEC9N1DTbi2M4U,8993
 cog/command/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/command/ast_openapi_schema.py,sha256=J42SekXuXHDmVbNKD29kMjWaRyxKnwFHY2BG8cVn28s,18782
 cog/command/openapi_schema.py,sha256=h-bfqVHkdOjnK469-mKhY9U18JaGK59W4Ur9bFWoM1U,1934
 cog/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/server/eventtypes.py,sha256=s2iJKjiXFG_cRIS_a4VQE_wVQosoyppRqTJfevBD_XI,593
 cog/server/exceptions.py,sha256=HknokO6g7gIlbIAMBM8685gE4Xgb8lykC-gTF6SLEYM,149
 cog/server/helpers.py,sha256=Z0mRZJOonbqc7Kir3JiGSbg-0svmtJCVpp3IaET3MlM,5349
@@ -23,22 +23,22 @@
 cog/server/runner.py,sha256=-fXchhxcPeuXMWtKbgajuIyePSxEKF5r-pe7cNo84xQ,15515
 cog/server/webhook.py,sha256=alohqVPU8aOsPz10N77uv2eFlvGMk8RBUj37eWFzLjY,3326
 cog/server/worker.py,sha256=VybuJ3bAFdNsOcqAkhv8M2-FkSx7sr8atN_fFAx2yLc,8050
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=KbeqWWshZoqqT6aLcZGB3_zLMe1G0IQ61BhoKQU1Xro,536
 tests/test_json.py,sha256=fkrKcif7qoHoSoQNwK24267MWeO5Lwyz8EMRUUT122Q,1737
 tests/test_predictor.py,sha256=K6yc1Va8isKetQxMIyQJ6WG92HJHKI8vvxGj4sA3rDY,1154
-tests/test_types.py,sha256=Okt_mbTcsVQapR5su0CIQEhMV-5xuFpXjzxKldFgR_Q,4689
+tests/test_types.py,sha256=yXePtMi7c1HIIpVzg8_qAIlqG4DqYDam3CToQ-a10WA,4895
 tests/fixtures/argv_override.py,sha256=dGjPI-zOkXaA0PVG1n_uKTxGB7WlSuuoa8WxBz6ZGoo,113
 tests/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/server/conftest.py,sha256=Njsjm2jgUf-4RaDMa3msxqgp0RMQIz0DZQtdP5i0sFQ,2800
 tests/server/test_code_xforms.py,sha256=3oBRcqz2UgzkBKvIIpicR0hWYpk5hTDHl6W9qVpCdYE,2564
 tests/server/test_helpers.py,sha256=XVpcv42AYwUmo1wAoR73FMdN4tOoRYkqaTjduKE_aDA,4692
 tests/server/test_http.py,sha256=3TqUNYjYkTktHE-8WskvTWQDRGWGFHSvqeuBgj6dr04,16956
-tests/server/test_http_input.py,sha256=7yRu_bUiUnT9-g_RaGlSXrP3X_SFlUjs1DPD7kD0rp4,8821
+tests/server/test_http_input.py,sha256=qd9RVyj9G7EDpbYKBMMy-bXibO2k4mtzI9QcJumi0zk,9181
 tests/server/test_http_output.py,sha256=AViMdeDEoSNfNtkftmtvyYG2A4DCP0ViGrmnZjYXuy4,4020
 tests/server/test_predictor.py,sha256=x7xpvWtJkY1N4lvk1SzhQpY57e_tNrk-atzTS2Lliog,2775
 tests/server/test_probes.py,sha256=L1ncJKDELevnxFq_Nr4hiZtNrLhkbClzbvAIGJ-RTzA,1334
 tests/server/test_response_throttler.py,sha256=5Dfslni4ioDrNbMJ2xNt-3La4K1SBm6LlV1UTosTlbg,1210
 tests/server/test_runner.py,sha256=dQymyMKrpYUpfifF_0R294520ZG7MdBDA9XlZHcKJ0s,10931
 tests/server/test_webhook.py,sha256=gt8XfJ-gizqKd__K2sCKTNkWJ1iYm29h1YDIYxxJo3Y,3225
 tests/server/test_worker.py,sha256=XH_B63JAmFniAQzYxO0Ee_2VKGa5S01NwVIq5iBo6Oo,16162
@@ -61,14 +61,15 @@
 tests/server/fixtures/input_ge_le.py,sha256=keijvUWbW6JBT4dKjE4tb_Y8vVXWjpb9w9hhjJ5AIIM,160
 tests/server/fixtures/input_integer.py,sha256=A-k1febjgFc48ILNvPLR6z5eN6S9bUhaTNXTgHypy9U,126
 tests/server/fixtures/input_integer_default.py,sha256=5xZBwBTlUGL_HsTIJWX4DnjGIEiynrBVNeQHPrqnPhs,152
 tests/server/fixtures/input_multiple.py,sha256=BdQYySj2JI05RFooHEscawfff3l765X789g2uCWegho,317
 tests/server/fixtures/input_none.py,sha256=ITfcOMD5kRImwcdSDAotFviaeTw-KyUmHH2ugTgvZp0,118
 tests/server/fixtures/input_path.py,sha256=FRUxE9PXEjftfvZYDBVWZNyhSOeD0DA_XwDq5lHGlNc,236
 tests/server/fixtures/input_path_2.py,sha256=bY9hD2a7jqkqPf5J7qePApkrc4DpzMxMnl0dNGeOHhw,137
+tests/server/fixtures/input_secret.py,sha256=SHIhR0jdr7xWK4dCtkIpcTnabAkbVRaFxW6tuadmSdo,159
 tests/server/fixtures/input_string.py,sha256=fNkMh9RT_Shzw3ouUSxKN8prsqLV_F1SOPx0-nzY2zk,125
 tests/server/fixtures/input_union_integer_or_list_of_integers.py,sha256=nqXMl1fUioSzR7te8c-py1kJSJvT0zZJcDLdAQmcGgc,262
 tests/server/fixtures/input_union_string_or_list_of_strings.py,sha256=RnGGRHJxAHDTsjMVJt6kxQSdnWojQlyYdeLecnAuIaQ,266
 tests/server/fixtures/input_unsupported_type.py,sha256=QSpeg7TfFYWz-e6HpQIlLBboZllgIJvdtXWQo4duAAY,205
 tests/server/fixtures/input_untyped.py,sha256=xbCojuqHGU0pyiSfQxpTYisKG3AdC2AfAiK-XEveG0M,122
 tests/server/fixtures/killed_in_predict.py,sha256=TsXUwj9aZtn0Y_Omw_u7QneeDW1LKaAi0EtCBu1_5UM,160
 tests/server/fixtures/logging.py,sha256=4W26YdMZR0MUN_CKuB-Yb3qf85GWr9bOCktqmVVTBFI,882
@@ -97,12 +98,12 @@
 tests/server/fixtures/slow_setup.py,sha256=vHIq6spLzpo-bLmgXlyazLWljQz53JamJDHcpTl_XJo,122
 tests/server/fixtures/steps.py,sha256=WbD27CUVQE8Zj_SVOtOqtleG3Y8meSJVAn-vkhpKst8,290
 tests/server/fixtures/train.py,sha256=5LmmIK9Cd7uSJIIjl-6zZkz4BRNbXCpMW5iBYRXLhKU,359
 tests/server/fixtures/yield_concatenate_iterator.py,sha256=2X582IGdiprIALwIs5e-EZO4i1eBUdM7CI4FCPf-CAo,263
 tests/server/fixtures/yield_files.py,sha256=QpIl1SOFsaakNZJlShl_XkjBGyB_MyuQgv5-J2Vm75U,506
 tests/server/fixtures/yield_strings.py,sha256=7Y9cTGZ7WE0iKlr-ZQmhkeg30mXt-fEpY9U0AQ0QMAQ,245
 tests/server/fixtures/yield_strings_file_input.py,sha256=rNxZHFXLhzqkNiG35JfcyihSA4Lx6s3bp86YRGPztX8,339
-cog-0.9.6.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
-cog-0.9.6.dist-info/METADATA,sha256=m4brIMf2CDYtMAqI68h4UTDeE-n5Nrw8e8Zxkapx1Cw,36704
-cog-0.9.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cog-0.9.6.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
-cog-0.9.6.dist-info/RECORD,,
+cog-0.9.7.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
+cog-0.9.7.dist-info/METADATA,sha256=5UWm__Kj3irEYVNfxvp5L86o5ZcdNdSpoYpW1gt56yU,36704
+cog-0.9.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cog-0.9.7.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
+cog-0.9.7.dist-info/RECORD,,
```

