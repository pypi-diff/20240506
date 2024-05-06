# Comparing `tmp/glean_sdk-60.0.0.tar.gz` & `tmp/glean_sdk-60.1.0.tar.gz`

## Comparing `glean_sdk-60.0.0.tar` & `glean_sdk-60.1.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0     1001     1002     1893 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/Cargo.toml
--rw-r--r--   0     1001     1002    16725 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/LICENSE
--rw-r--r--   0     1001     1002     1699 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/README.md
--rw-r--r--   0     1001     1002       76 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/build.rs
--rw-r--r--   0     1001     1002     4699 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/common_metric_data.rs
--rw-r--r--   0     1001     1002    36926 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/core/mod.rs
--rw-r--r--   0     1001     1002     7409 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/core_metrics.rs
--rw-r--r--   0     1001     1002     1776 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/coverage.rs
--rw-r--r--   0     1001     1002    66424 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/database/mod.rs
--rw-r--r--   0     1001     1002    10907 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/debug.rs
--rw-r--r--   0     1001     1002     7202 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/dispatcher/global.rs
--rw-r--r--   0     1001     1002    19263 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/dispatcher/mod.rs
--rw-r--r--   0     1001     1002     4755 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/error.rs
--rw-r--r--   0     1001     1002     8335 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/error_recording.rs
--rw-r--r--   0     1001     1002    48888 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/event_database/mod.rs
--rw-r--r--   0     1001     1002     2603 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/fd_logger.rs
--rw-r--r--   0     1001     1002    18704 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/glean.udl
--rw-r--r--   0     1001     1002      899 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/glean_metrics.rs
--rw-r--r--   0     1001     1002     6962 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/histogram/exponential.rs
--rw-r--r--   0     1001     1002     5764 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/histogram/functional.rs
--rw-r--r--   0     1001     1002     5794 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/histogram/linear.rs
--rw-r--r--   0     1001     1002     3930 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/histogram/mod.rs
--rw-r--r--   0     1001     1002    10750 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/internal_metrics.rs
--rw-r--r--   0     1001     1002     2534 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/internal_pings.rs
--rw-r--r--   0     1001     1002    47569 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/lib.rs
--rw-r--r--   0     1001     1002    41835 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/lib_unit_tests.rs
--rw-r--r--   0     1001     1002     4061 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/boolean.rs
--rw-r--r--   0     1001     1002     5241 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/counter.rs
--rw-r--r--   0     1001     1002     8437 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/custom_distribution.rs
--rw-r--r--   0     1001     1002    10449 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/datetime.rs
--rw-r--r--   0     1001     1002     4572 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/denominator.rs
--rw-r--r--   0     1001     1002     7478 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/event.rs
--rw-r--r--   0     1001     1002     9850 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/experiment.rs
--rw-r--r--   0     1001     1002     9862 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/labeled.rs
--rw-r--r--   0     1001     1002     9793 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/memory_distribution.rs
--rw-r--r--   0     1001     1002     1809 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/memory_unit.rs
--rw-r--r--   0     1001     1002    12047 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/mod.rs
--rw-r--r--   0     1001     1002     2959 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/numerator.rs
--rw-r--r--   0     1001     1002     5239 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/object.rs
--rw-r--r--   0     1001     1002    10983 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/ping.rs
--rw-r--r--   0     1001     1002     3818 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/quantity.rs
--rw-r--r--   0     1001     1002     5963 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/rate.rs
--rw-r--r--   0     1001     1002     1573 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/recorded_experiment.rs
--rw-r--r--   0     1001     1002     1797 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/remote_settings_config.rs
--rw-r--r--   0     1001     1002     5363 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/string.rs
--rw-r--r--   0     1001     1002     6514 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/string_list.rs
--rw-r--r--   0     1001     1002     5544 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/text.rs
--rw-r--r--   0     1001     1002     3768 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/time_unit.rs
--rw-r--r--   0     1001     1002    10380 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/timespan.rs
--rw-r--r--   0     1001     1002    20000 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/timing_distribution.rs
--rw-r--r--   0     1001     1002    10222 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/url.rs
--rw-r--r--   0     1001     1002     5063 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/metrics/uuid.rs
--rw-r--r--   0     1001     1002    15471 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/ping/mod.rs
--rw-r--r--   0     1001     1002    23631 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/scheduler.rs
--rw-r--r--   0     1001     1002     9495 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/storage/mod.rs
--rw-r--r--   0     1001     1002     2856 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/system.rs
--rw-r--r--   0     1001     1002     1380 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/boolean.rs
--rw-r--r--   0     1001     1002     1497 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/counter.rs
--rw-r--r--   0     1001     1002     2615 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/custom_distribution.rs
--rw-r--r--   0     1001     1002     1759 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/datetime.rs
--rw-r--r--   0     1001     1002     3788 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/event.rs
--rw-r--r--   0     1001     1002     1519 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/labeled.rs
--rw-r--r--   0     1001     1002     1804 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/memory_distribution.rs
--rw-r--r--   0     1001     1002     1642 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/mod.rs
--rw-r--r--   0     1001     1002     1584 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/numerator.rs
--rw-r--r--   0     1001     1002     1730 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/object.rs
--rw-r--r--   0     1001     1002      665 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/ping.rs
--rw-r--r--   0     1001     1002     1481 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/quantity.rs
--rw-r--r--   0     1001     1002     1823 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/rate.rs
--rw-r--r--   0     1001     1002     1574 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/string.rs
--rw-r--r--   0     1001     1002     1971 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/string_list.rs
--rw-r--r--   0     1001     1002     1568 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/text.rs
--rw-r--r--   0     1001     1002     2403 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/timespan.rs
--rw-r--r--   0     1001     1002     5097 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/timing_distribution.rs
--rw-r--r--   0     1001     1002     1645 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/url.rs
--rw-r--r--   0     1001     1002     1528 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/traits/uuid.rs
--rw-r--r--   0     1001     1002    16472 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/upload/directory.rs
--rw-r--r--   0     1001     1002    68645 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/upload/mod.rs
--rw-r--r--   0     1001     1002     3830 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/upload/policy.rs
--rw-r--r--   0     1001     1002    10852 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/upload/request.rs
--rw-r--r--   0     1001     1002     3150 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/upload/result.rs
--rw-r--r--   0     1001     1002    10750 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/src/util.rs
--rw-r--r--   0     1001     1002     2829 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/boolean.rs
--rw-r--r--   0     1001     1002     5330 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/common/mod.rs
--rw-r--r--   0     1001     1002     5332 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/counter.rs
--rw-r--r--   0     1001     1002    13398 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/custom_distribution.rs
--rw-r--r--   0     1001     1002     5974 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/datetime.rs
--rw-r--r--   0     1001     1002    16332 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/event.rs
--rw-r--r--   0     1001     1002    14418 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/labeled.rs
--rw-r--r--   0     1001     1002     5865 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/memory_distribution.rs
--rw-r--r--   0     1001     1002     3195 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/object.rs
--rw-r--r--   0     1001     1002     8742 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/ping.rs
--rw-r--r--   0     1001     1002    10544 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/ping_maker.rs
--rw-r--r--   0     1001     1002     3611 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/quantity.rs
--rw-r--r--   0     1001     1002     4058 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/rate.rs
--rw-r--r--   0     1001     1002     3314 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/storage.rs
--rw-r--r--   0     1001     1002     3730 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/string.rs
--rw-r--r--   0     1001     1002     7423 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/string_list.rs
--rw-r--r--   0     1001     1002     3470 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/text.rs
--rw-r--r--   0     1001     1002    10155 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/timespan.rs
--rw-r--r--   0     1001     1002    12981 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/timing_distribution.rs
--rw-r--r--   0     1001     1002     3375 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/tests/uuid.rs
--rw-r--r--   0     1001     1002      205 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/uniffi.toml
--rw-r--r--   0     1001     1002      299 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/Cargo.toml
--rw-r--r--   0     1001     1002     1902 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/README.md
--rw-r--r--   0     1001     1002       67 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/src/lib.rs
--rw-r--r--   0     1001     1002     2571 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/src/main.rs
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.0.0/glean-core/bundle/Cargo.toml
--rw-r--r--   0     1001     1002    18704 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/bundle/src/glean.udl
--rw-r--r--   0     1001     1002      973 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/bundle/src/lib.rs
--rw-r--r--   0     1001     1002      205 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/bundle/uniffi.toml
--rw-r--r--   0     1001     1002    32669 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/Cargo.lock
--rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.0.0/Cargo.toml
--rw-r--r--   0     1001     1002     1209 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/pyproject.toml
--rw-r--r--   0     1001     1002     1502 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/__init__.py
--rw-r--r--   0     1001     1002      585 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_builtins.py
--rw-r--r--   0     1001     1002     1698 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_ffi.py
--rw-r--r--   0     1001     1002    12757 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_loader.py
--rw-r--r--   0     1001     1002     5161 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_process_dispatcher.py
--rw-r--r--   0     1001     1002      199 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_subprocess/__init__.py
--rw-r--r--   0     1001     1002     1336 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
--rw-r--r--   0     1001     1002     1502 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/_util.py
--rw-r--r--   0     1001     1002     4278 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/config.py
--rw-r--r--   0     1001     1002    15982 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/glean.py
--rw-r--r--   0     1001     1002    23717 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics.yaml
--rw-r--r--   0     1001     1002     2034 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/__init__.py
--rw-r--r--   0     1001     1002     3803 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/datetime.py
--rw-r--r--   0     1001     1002     3289 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/event.py
--rw-r--r--   0     1001     1002     3225 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/labeled.py
--rw-r--r--   0     1001     1002     3402 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/object.py
--rw-r--r--   0     1001     1002     2408 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/ping.py
--rw-r--r--   0     1001     1002     1576 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/string.py
--rw-r--r--   0     1001     1002     4395 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/timespan.py
--rw-r--r--   0     1001     1002     5030 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/timing_distribution.py
--rw-r--r--   0     1001     1002     1628 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/url.py
--rw-r--r--   0     1001     1002     1757 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/metrics/uuid.py
--rw-r--r--   0     1001     1002      522 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/net/__init__.py
--rw-r--r--   0     1001     1002     1569 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/net/base_uploader.py
--rw-r--r--   0     1001     1002     3211 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/net/http_client.py
--rw-r--r--   0     1001     1002     5200 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/net/ping_upload_worker.py
--rw-r--r--   0     1001     1002     1068 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/net/ping_uploader.py
--rw-r--r--   0     1001     1002     5383 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/pings.yaml
--rw-r--r--   0     1001     1002     2883 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/glean-core/python/glean/testing/__init__.py
--rw-r--r--   0     1001     1002     3773 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/README.md
--rw-r--r--   0     1001     1002    16725 2024-04-22 13:37:24.000000 glean_sdk-60.0.0/LICENSE
--rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.0.0/PKG-INFO
+-rw-r--r--   0     1001     1002     1893 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/Cargo.toml
+-rw-r--r--   0     1001     1002    16725 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/LICENSE
+-rw-r--r--   0     1001     1002     1699 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/README.md
+-rw-r--r--   0     1001     1002       76 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/build.rs
+-rw-r--r--   0     1001     1002     4699 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/common_metric_data.rs
+-rw-r--r--   0     1001     1002    36926 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/core/mod.rs
+-rw-r--r--   0     1001     1002     7409 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/core_metrics.rs
+-rw-r--r--   0     1001     1002     1776 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/coverage.rs
+-rw-r--r--   0     1001     1002    66424 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/database/mod.rs
+-rw-r--r--   0     1001     1002    10907 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/debug.rs
+-rw-r--r--   0     1001     1002     7202 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/dispatcher/global.rs
+-rw-r--r--   0     1001     1002    19263 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/dispatcher/mod.rs
+-rw-r--r--   0     1001     1002     4755 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/error.rs
+-rw-r--r--   0     1001     1002     8335 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/error_recording.rs
+-rw-r--r--   0     1001     1002    48891 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/event_database/mod.rs
+-rw-r--r--   0     1001     1002     2603 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/fd_logger.rs
+-rw-r--r--   0     1001     1002    18704 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/glean.udl
+-rw-r--r--   0     1001     1002      899 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/glean_metrics.rs
+-rw-r--r--   0     1001     1002     6938 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/exponential.rs
+-rw-r--r--   0     1001     1002     5764 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/functional.rs
+-rw-r--r--   0     1001     1002     5770 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/linear.rs
+-rw-r--r--   0     1001     1002     3930 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/mod.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/internal_metrics.rs
+-rw-r--r--   0     1001     1002     2534 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/internal_pings.rs
+-rw-r--r--   0     1001     1002    47569 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/lib.rs
+-rw-r--r--   0     1001     1002    41835 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/lib_unit_tests.rs
+-rw-r--r--   0     1001     1002     4061 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/boolean.rs
+-rw-r--r--   0     1001     1002     5241 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/counter.rs
+-rw-r--r--   0     1001     1002     8437 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/custom_distribution.rs
+-rw-r--r--   0     1001     1002    10449 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/datetime.rs
+-rw-r--r--   0     1001     1002     4572 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/denominator.rs
+-rw-r--r--   0     1001     1002     7478 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/event.rs
+-rw-r--r--   0     1001     1002     9850 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/experiment.rs
+-rw-r--r--   0     1001     1002     9862 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/labeled.rs
+-rw-r--r--   0     1001     1002     9793 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1809 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/memory_unit.rs
+-rw-r--r--   0     1001     1002    12047 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/mod.rs
+-rw-r--r--   0     1001     1002     2959 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/numerator.rs
+-rw-r--r--   0     1001     1002     5239 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/object.rs
+-rw-r--r--   0     1001     1002    10983 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/ping.rs
+-rw-r--r--   0     1001     1002     3818 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/quantity.rs
+-rw-r--r--   0     1001     1002     5963 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/rate.rs
+-rw-r--r--   0     1001     1002     1573 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/recorded_experiment.rs
+-rw-r--r--   0     1001     1002     1797 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/remote_settings_config.rs
+-rw-r--r--   0     1001     1002     5363 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/string.rs
+-rw-r--r--   0     1001     1002     6514 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/string_list.rs
+-rw-r--r--   0     1001     1002     5544 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/text.rs
+-rw-r--r--   0     1001     1002     3768 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/time_unit.rs
+-rw-r--r--   0     1001     1002    10380 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/timespan.rs
+-rw-r--r--   0     1001     1002    21230 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/timing_distribution.rs
+-rw-r--r--   0     1001     1002    10222 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/url.rs
+-rw-r--r--   0     1001     1002     5063 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/uuid.rs
+-rw-r--r--   0     1001     1002    15471 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/ping/mod.rs
+-rw-r--r--   0     1001     1002    23631 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/scheduler.rs
+-rw-r--r--   0     1001     1002     9495 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/storage/mod.rs
+-rw-r--r--   0     1001     1002     2856 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/system.rs
+-rw-r--r--   0     1001     1002     1380 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/boolean.rs
+-rw-r--r--   0     1001     1002     1497 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/counter.rs
+-rw-r--r--   0     1001     1002     2615 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/custom_distribution.rs
+-rw-r--r--   0     1001     1002     1759 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/datetime.rs
+-rw-r--r--   0     1001     1002     3788 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/event.rs
+-rw-r--r--   0     1001     1002     1519 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/labeled.rs
+-rw-r--r--   0     1001     1002     1804 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1642 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/mod.rs
+-rw-r--r--   0     1001     1002     1584 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/numerator.rs
+-rw-r--r--   0     1001     1002     1730 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/object.rs
+-rw-r--r--   0     1001     1002      665 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/ping.rs
+-rw-r--r--   0     1001     1002     1481 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/quantity.rs
+-rw-r--r--   0     1001     1002     1823 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/rate.rs
+-rw-r--r--   0     1001     1002     1574 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/string.rs
+-rw-r--r--   0     1001     1002     1971 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/string_list.rs
+-rw-r--r--   0     1001     1002     1568 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/text.rs
+-rw-r--r--   0     1001     1002     2403 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/timespan.rs
+-rw-r--r--   0     1001     1002     6069 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/timing_distribution.rs
+-rw-r--r--   0     1001     1002     1645 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/url.rs
+-rw-r--r--   0     1001     1002     1528 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/uuid.rs
+-rw-r--r--   0     1001     1002    16472 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/directory.rs
+-rw-r--r--   0     1001     1002    68645 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/mod.rs
+-rw-r--r--   0     1001     1002     3830 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/policy.rs
+-rw-r--r--   0     1001     1002    10852 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/request.rs
+-rw-r--r--   0     1001     1002     3150 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/result.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/util.rs
+-rw-r--r--   0     1001     1002     2829 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/boolean.rs
+-rw-r--r--   0     1001     1002     5330 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/common/mod.rs
+-rw-r--r--   0     1001     1002     5294 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/counter.rs
+-rw-r--r--   0     1001     1002    13398 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/custom_distribution.rs
+-rw-r--r--   0     1001     1002     5974 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/datetime.rs
+-rw-r--r--   0     1001     1002    16332 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/event.rs
+-rw-r--r--   0     1001     1002    14418 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/labeled.rs
+-rw-r--r--   0     1001     1002     5865 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/memory_distribution.rs
+-rw-r--r--   0     1001     1002     3195 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/object.rs
+-rw-r--r--   0     1001     1002     8742 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/ping.rs
+-rw-r--r--   0     1001     1002    10544 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/ping_maker.rs
+-rw-r--r--   0     1001     1002     3611 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/quantity.rs
+-rw-r--r--   0     1001     1002     4058 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/rate.rs
+-rw-r--r--   0     1001     1002     3314 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/storage.rs
+-rw-r--r--   0     1001     1002     3730 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/string.rs
+-rw-r--r--   0     1001     1002     7423 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/string_list.rs
+-rw-r--r--   0     1001     1002     3470 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/text.rs
+-rw-r--r--   0     1001     1002    10155 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/timespan.rs
+-rw-r--r--   0     1001     1002    12973 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/timing_distribution.rs
+-rw-r--r--   0     1001     1002     3375 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/uuid.rs
+-rw-r--r--   0     1001     1002      205 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/uniffi.toml
+-rw-r--r--   0     1001     1002      299 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/Cargo.toml
+-rw-r--r--   0     1001     1002     1902 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/README.md
+-rw-r--r--   0     1001     1002       67 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/lib.rs
+-rw-r--r--   0     1001     1002     2571 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/main.rs
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/glean-core/bundle/Cargo.toml
+-rw-r--r--   0     1001     1002    18704 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/src/glean.udl
+-rw-r--r--   0     1001     1002      973 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/src/lib.rs
+-rw-r--r--   0     1001     1002      205 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/uniffi.toml
+-rw-r--r--   0     1001     1002    32669 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/Cargo.lock
+-rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/Cargo.toml
+-rw-r--r--   0     1001     1002     1209 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/pyproject.toml
+-rw-r--r--   0     1001     1002     1479 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/__init__.py
+-rw-r--r--   0     1001     1002      585 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_builtins.py
+-rw-r--r--   0     1001     1002     1698 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_ffi.py
+-rw-r--r--   0     1001     1002    12757 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_loader.py
+-rw-r--r--   0     1001     1002     5161 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_process_dispatcher.py
+-rw-r--r--   0     1001     1002      199 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_subprocess/__init__.py
+-rw-r--r--   0     1001     1002     1336 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
+-rw-r--r--   0     1001     1002     1502 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_util.py
+-rw-r--r--   0     1001     1002     4278 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/config.py
+-rw-r--r--   0     1001     1002    15982 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/glean.py
+-rw-r--r--   0     1001     1002    23717 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics.yaml
+-rw-r--r--   0     1001     1002     2034 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/__init__.py
+-rw-r--r--   0     1001     1002     3803 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/datetime.py
+-rw-r--r--   0     1001     1002     3289 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/event.py
+-rw-r--r--   0     1001     1002     3225 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/labeled.py
+-rw-r--r--   0     1001     1002     3402 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/object.py
+-rw-r--r--   0     1001     1002     2408 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/ping.py
+-rw-r--r--   0     1001     1002     1576 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/string.py
+-rw-r--r--   0     1001     1002     4395 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/timespan.py
+-rw-r--r--   0     1001     1002     5030 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/timing_distribution.py
+-rw-r--r--   0     1001     1002     1628 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/url.py
+-rw-r--r--   0     1001     1002     1757 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/uuid.py
+-rw-r--r--   0     1001     1002      522 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/__init__.py
+-rw-r--r--   0     1001     1002     1569 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/base_uploader.py
+-rw-r--r--   0     1001     1002     3211 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/http_client.py
+-rw-r--r--   0     1001     1002     5200 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/ping_upload_worker.py
+-rw-r--r--   0     1001     1002     1068 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/ping_uploader.py
+-rw-r--r--   0     1001     1002     5383 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/pings.yaml
+-rw-r--r--   0     1001     1002     2883 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/testing/__init__.py
+-rw-r--r--   0     1001     1002     3773 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/README.md
+-rw-r--r--   0     1001     1002    16725 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/LICENSE
+-rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/PKG-INFO
```

### Comparing `glean_sdk-60.0.0/glean-core/Cargo.toml` & `glean_sdk-60.1.0/glean-core/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "glean-core"
-version = "60.0.0"
+version = "60.1.0"
 authors = ["Jan-Erik Rediger <jrediger@mozilla.com>", "The Glean Team <glean-team@mozilla.com>"]
 description = "A modern Telemetry library"
 repository = "https://github.com/mozilla/glean"
 readme = "README.md"
 license = "MPL-2.0"
 edition = "2021"
 keywords = ["telemetry"]
```

### Comparing `glean_sdk-60.0.0/glean-core/LICENSE` & `glean_sdk-60.1.0/glean-core/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/README.md` & `glean_sdk-60.1.0/glean-core/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/common_metric_data.rs` & `glean_sdk-60.1.0/glean-core/src/common_metric_data.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/core/mod.rs` & `glean_sdk-60.1.0/glean-core/src/core/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/core_metrics.rs` & `glean_sdk-60.1.0/glean-core/src/core_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/coverage.rs` & `glean_sdk-60.1.0/glean-core/src/coverage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/database/mod.rs` & `glean_sdk-60.1.0/glean-core/src/database/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/debug.rs` & `glean_sdk-60.1.0/glean-core/src/debug.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/dispatcher/global.rs` & `glean_sdk-60.1.0/glean-core/src/dispatcher/global.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/dispatcher/mod.rs` & `glean_sdk-60.1.0/glean-core/src/dispatcher/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/error.rs` & `glean_sdk-60.1.0/glean-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/error_recording.rs` & `glean_sdk-60.1.0/glean-core/src/error_recording.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/event_database/mod.rs` & `glean_sdk-60.1.0/glean-core/src/event_database/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use std::collections::HashMap;
 use std::fs;
 use std::fs::{create_dir_all, File, OpenOptions};
 use std::io::BufRead;
 use std::io::BufReader;
 use std::io::Write;
 use std::path::{Path, PathBuf};
-use std::sync::RwLock;
+use std::sync::{Mutex, RwLock};
 
 use chrono::{DateTime, FixedOffset, Utc};
 
 use serde::{Deserialize, Serialize};
 use serde_json::{json, Value as JsonValue};
 
 use crate::common_metric_data::CommonMetricDataInternal;
@@ -92,15 +92,15 @@
 #[derive(Debug)]
 pub struct EventDatabase {
     /// Path to directory of on-disk event files
     pub path: PathBuf,
     /// The in-memory list of events
     event_stores: RwLock<HashMap<String, Vec<StoredEvent>>>,
     /// A lock to be held when doing operations on the filesystem
-    file_lock: RwLock<()>,
+    file_lock: Mutex<()>,
 }
 
 impl EventDatabase {
     /// Creates a new event database.
     ///
     /// # Arguments
     ///
@@ -109,15 +109,15 @@
     pub fn new(data_path: &Path) -> Result<Self> {
         let path = data_path.join("events");
         create_dir_all(&path)?;
 
         Ok(Self {
             path,
             event_stores: RwLock::new(HashMap::new()),
-            file_lock: RwLock::new(()),
+            file_lock: Mutex::new(()),
         })
     }
 
     /// Initializes events storage after Glean is fully initialized and ready to send pings.
     ///
     /// This must be called once on application startup, e.g. from
     /// [Glean.initialize], but after we are ready to send pings, since this
@@ -216,15 +216,15 @@
         trim_data_to_registered_pings: bool,
     ) -> Result<()> {
         // NOTE: The order of locks here is important.
         // In other code parts we might acquire the `file_lock` when we already have acquired
         // a lock on `event_stores`.
         // This is a potential lock-order-inversion.
         let mut db = self.event_stores.write().unwrap(); // safe unwrap, only error case is poisoning
-        let _lock = self.file_lock.write().unwrap(); // safe unwrap, only error case is poisoning
+        let _lock = self.file_lock.lock().unwrap(); // safe unwrap, only error case is poisoning
 
         for entry in fs::read_dir(&self.path)? {
             let entry = entry?;
             if entry.file_type()?.is_file() {
                 let store_name = entry.file_name().into_string()?;
                 log::info!("Loading events for {}", store_name);
                 if trim_data_to_registered_pings && glean.get_ping_by_name(&store_name).is_none() {
@@ -322,15 +322,15 @@
     /// Writes an event to a single store on disk.
     ///
     /// # Arguments
     ///
     /// * `store_name` - The name of the store.
     /// * `event_json` - The event content, as a single-line JSON-encoded string.
     fn write_event_to_disk(&self, store_name: &str, event_json: &str) {
-        let _lock = self.file_lock.write().unwrap(); // safe unwrap, only error case is poisoning
+        let _lock = self.file_lock.lock().unwrap(); // safe unwrap, only error case is poisoning
         if let Err(err) = OpenOptions::new()
             .create(true)
             .append(true)
             .open(self.path.join(store_name))
             .and_then(|mut file| writeln!(file, "{}", event_json))
         {
             log::warn!("IO error writing event to store '{}': {}", store_name, err);
@@ -572,15 +572,15 @@
 
         if clear_store {
             self.event_stores
                 .write()
                 .unwrap() // safe unwrap, only error case is poisoning
                 .remove(&store_name.to_string());
 
-            let _lock = self.file_lock.write().unwrap(); // safe unwrap, only error case is poisoning
+            let _lock = self.file_lock.lock().unwrap(); // safe unwrap, only error case is poisoning
             if let Err(err) = fs::remove_file(self.path.join(store_name)) {
                 match err.kind() {
                     std::io::ErrorKind::NotFound => {
                         // silently drop this error, the file was already non-existing
                     }
                     _ => log::warn!("Error removing events queue file '{}': {}", store_name, err),
                 }
@@ -592,15 +592,15 @@
 
     /// Clears all stored events, both in memory and on-disk.
     pub fn clear_all(&self) -> Result<()> {
         // safe unwrap, only error case is poisoning
         self.event_stores.write().unwrap().clear();
 
         // safe unwrap, only error case is poisoning
-        let _lock = self.file_lock.write().unwrap();
+        let _lock = self.file_lock.lock().unwrap();
         std::fs::remove_dir_all(&self.path)?;
         create_dir_all(&self.path)?;
 
         Ok(())
     }
 
     /// **Test-only API (exported for FFI purposes).**
```

### Comparing `glean_sdk-60.0.0/glean-core/src/fd_logger.rs` & `glean_sdk-60.1.0/glean-core/src/fd_logger.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/glean.udl` & `glean_sdk-60.1.0/glean-core/src/glean.udl`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/glean_metrics.rs` & `glean_sdk-60.1.0/glean-core/src/glean_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/histogram/exponential.rs` & `glean_sdk-60.1.0/glean-core/src/histogram/exponential.rs`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,16 @@
         assert_eq!(1, hist.values[&9262]); // bucket_ranges[80] = 9262
     }
 
     #[test]
     fn accumulate_large_numbers() {
         let mut hist = Histogram::exponential(1, 500, 10);
 
-        hist.accumulate(u64::max_value());
-        hist.accumulate(u64::max_value());
+        hist.accumulate(u64::MAX);
+        hist.accumulate(u64::MAX);
 
         assert_eq!(2, hist.count());
         // Saturate before overflowing
-        assert_eq!(u64::max_value(), hist.sum());
+        assert_eq!(u64::MAX, hist.sum());
         assert_eq!(2, hist.values[&500]);
     }
 }
```

### Comparing `glean_sdk-60.0.0/glean-core/src/histogram/functional.rs` & `glean_sdk-60.1.0/glean-core/src/histogram/functional.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/histogram/linear.rs` & `glean_sdk-60.1.0/glean-core/src/histogram/linear.rs`

 * *Files 5% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         assert_eq!(3, hist.values[&100]);
     }
 
     #[test]
     fn accumulate_large_numbers() {
         let mut hist = Histogram::linear(1, 500, 10);
 
-        hist.accumulate(u64::max_value());
-        hist.accumulate(u64::max_value());
+        hist.accumulate(u64::MAX);
+        hist.accumulate(u64::MAX);
 
         assert_eq!(2, hist.count());
         // Saturate before overflowing
-        assert_eq!(u64::max_value(), hist.sum());
+        assert_eq!(u64::MAX, hist.sum());
         assert_eq!(2, hist.values[&500]);
     }
 }
```

### Comparing `glean_sdk-60.0.0/glean-core/src/histogram/mod.rs` & `glean_sdk-60.1.0/glean-core/src/histogram/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/internal_metrics.rs` & `glean_sdk-60.1.0/glean-core/src/internal_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/internal_pings.rs` & `glean_sdk-60.1.0/glean-core/src/internal_pings.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/lib.rs` & `glean_sdk-60.1.0/glean-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/lib_unit_tests.rs` & `glean_sdk-60.1.0/glean-core/src/lib_unit_tests.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/boolean.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/counter.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/custom_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/datetime.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/denominator.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/denominator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/event.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/experiment.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/labeled.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/memory_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/memory_unit.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/memory_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/mod.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/numerator.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/object.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/ping.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/quantity.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/rate.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/recorded_experiment.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/recorded_experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/remote_settings_config.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/remote_settings_config.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/string.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/string_list.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/text.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/time_unit.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/time_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/timespan.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/timing_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/timing_distribution.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 use std::collections::HashMap;
 use std::sync::atomic::{AtomicUsize, Ordering};
 use std::sync::{Arc, Mutex};
+use std::time::Duration;
 
 use crate::common_metric_data::CommonMetricDataInternal;
 use crate::error_recording::{record_error, test_get_num_recorded_errors, ErrorType};
 use crate::histogram::{Functional, Histogram};
 use crate::metrics::time_unit::TimeUnit;
 use crate::metrics::{DistributionData, Metric, MetricType};
 use crate::storage::StorageManager;
@@ -408,14 +409,43 @@
     pub fn accumulate_raw_samples_nanos(&self, samples: Vec<u64>) {
         let metric = self.clone();
         crate::launch_with_glean(move |glean| {
             metric.accumulate_raw_samples_nanos_sync(glean, &samples)
         })
     }
 
+    /// Accumulates precisely one duration to the metric.
+    ///
+    /// Like `TimingDistribution::accumulate_single_sample`, but for use when the
+    /// duration is:
+    ///
+    ///  * measured externally, or
+    ///  * is in a unit different from the timing_distribution's internal TimeUnit.
+    ///
+    /// # Arguments
+    ///
+    /// * `duration` - The single duration to be recorded in the metric.
+    ///
+    /// ## Notes
+    ///
+    /// Reports an [`ErrorType::InvalidOverflow`] error if `duration` is longer than
+    /// `MAX_SAMPLE_TIME`.
+    ///
+    /// The API client is responsible for ensuring that `duration` is derived from a
+    /// monotonic clock source that behaves consistently over computer sleep across
+    /// the application's platforms. Otherwise the resulting data may not share the same
+    /// guarantees that other `timing_distribution` metrics' data do.
+    pub fn accumulate_raw_duration(&self, duration: Duration) {
+        let duration_ns = duration.as_nanos().try_into().unwrap_or(u64::MAX);
+        let metric = self.clone();
+        crate::launch_with_glean(move |glean| {
+            metric.accumulate_raw_samples_nanos_sync(glean, &[duration_ns])
+        })
+    }
+
     /// **Test-only API (exported for testing purposes).**
     ///
     /// Accumulates the provided samples in the metric.
     ///
     /// Use [`accumulate_raw_samples_nanos`](Self::accumulate_raw_samples_nanos) instead.
     #[doc(hidden)]
     pub fn accumulate_raw_samples_nanos_sync(&self, glean: &Glean, samples: &[u64]) {
```

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/url.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/metrics/uuid.rs` & `glean_sdk-60.1.0/glean-core/src/metrics/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/ping/mod.rs` & `glean_sdk-60.1.0/glean-core/src/ping/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/scheduler.rs` & `glean_sdk-60.1.0/glean-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/storage/mod.rs` & `glean_sdk-60.1.0/glean-core/src/storage/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/system.rs` & `glean_sdk-60.1.0/glean-core/src/system.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/boolean.rs` & `glean_sdk-60.1.0/glean-core/src/traits/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/counter.rs` & `glean_sdk-60.1.0/glean-core/src/traits/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/custom_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/traits/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/datetime.rs` & `glean_sdk-60.1.0/glean-core/src/traits/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/event.rs` & `glean_sdk-60.1.0/glean-core/src/traits/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/labeled.rs` & `glean_sdk-60.1.0/glean-core/src/traits/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/memory_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/traits/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/mod.rs` & `glean_sdk-60.1.0/glean-core/src/traits/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/numerator.rs` & `glean_sdk-60.1.0/glean-core/src/traits/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/object.rs` & `glean_sdk-60.1.0/glean-core/src/traits/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/ping.rs` & `glean_sdk-60.1.0/glean-core/src/traits/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/quantity.rs` & `glean_sdk-60.1.0/glean-core/src/traits/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/rate.rs` & `glean_sdk-60.1.0/glean-core/src/traits/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/string.rs` & `glean_sdk-60.1.0/glean-core/src/traits/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/string_list.rs` & `glean_sdk-60.1.0/glean-core/src/traits/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/text.rs` & `glean_sdk-60.1.0/glean-core/src/traits/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/timespan.rs` & `glean_sdk-60.1.0/glean-core/src/traits/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/timing_distribution.rs` & `glean_sdk-60.1.0/glean-core/src/traits/timing_distribution.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 use crate::metrics::DistributionData;
 use crate::metrics::TimerId;
 use crate::ErrorType;
 
+use std::time::Duration;
+
 /// A description for the [`TimingDistributionMetric`](crate::metrics::TimingDistributionMetric) type.
 ///
 /// When changing this trait, make sure all the operations are
 /// implemented in the related type in `../metrics/`.
 pub trait TimingDistribution {
     /// Start tracking time for the provided metric.
     /// Multiple timers can run simultaneously.
@@ -99,14 +101,37 @@
     ///               Samples must be in nanoseconds.
     /// ## Notes
     ///
     /// Reports an [`ErrorType::InvalidOverflow`] error for samples that
     /// are longer than `MAX_SAMPLE_TIME`.
     fn accumulate_raw_samples_nanos(&self, samples: Vec<u64>);
 
+    /// Accumulates precisely one duration to the metric.
+    ///
+    /// Like `TimingDistribution::accumulate_single_sample`, but for use when the
+    /// duration is:
+    ///
+    ///  * measured externally, or
+    ///  * is in a unit different from the timing_distribution's internal TimeUnit.
+    ///
+    /// # Arguments
+    ///
+    /// * `duration` - The single duration to be recorded in the metric.
+    ///
+    /// ## Notes
+    ///
+    /// Reports an [`ErrorType::InvalidOverflow`] error if `duration` is longer than
+    /// `MAX_SAMPLE_TIME`.
+    ///
+    /// The API client is responsible for ensuring that `duration` is derived from a
+    /// monotonic clock source that behaves consistently over computer sleep across
+    /// the application's platforms. Otherwise the resulting data may not share the same
+    /// guarantees that other `timing_distribution` metrics' data do.
+    fn accumulate_raw_duration(&self, duration: Duration);
+
     /// **Exported for test purposes.**
     ///
     /// Gets the currently stored value of the metric.
     ///
     /// This doesn't clear the stored value.
     ///
     /// # Arguments
```

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/url.rs` & `glean_sdk-60.1.0/glean-core/src/traits/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/traits/uuid.rs` & `glean_sdk-60.1.0/glean-core/src/traits/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/upload/directory.rs` & `glean_sdk-60.1.0/glean-core/src/upload/directory.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/upload/mod.rs` & `glean_sdk-60.1.0/glean-core/src/upload/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/upload/policy.rs` & `glean_sdk-60.1.0/glean-core/src/upload/policy.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/upload/request.rs` & `glean_sdk-60.1.0/glean-core/src/upload/request.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/upload/result.rs` & `glean_sdk-60.1.0/glean-core/src/upload/result.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/src/util.rs` & `glean_sdk-60.1.0/glean-core/src/util.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/boolean.rs` & `glean_sdk-60.1.0/glean-core/tests/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/common/mod.rs` & `glean_sdk-60.1.0/glean-core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/counter.rs` & `glean_sdk-60.1.0/glean-core/tests/counter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,11 @@
         name: "transformation".into(),
         category: "local".into(),
         send_in_pings: vec!["store1".into()],
         ..Default::default()
     });
 
     counter.add_sync(&glean, 2);
-    counter.add_sync(&glean, i32::max_value());
+    counter.add_sync(&glean, i32::MAX);
 
-    assert_eq!(
-        i32::max_value(),
-        counter.get_value(&glean, Some("store1")).unwrap()
-    );
+    assert_eq!(i32::MAX, counter.get_value(&glean, Some("store1")).unwrap());
 }
```

### Comparing `glean_sdk-60.0.0/glean-core/tests/custom_distribution.rs` & `glean_sdk-60.1.0/glean-core/tests/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/datetime.rs` & `glean_sdk-60.1.0/glean-core/tests/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/event.rs` & `glean_sdk-60.1.0/glean-core/tests/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/labeled.rs` & `glean_sdk-60.1.0/glean-core/tests/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/memory_distribution.rs` & `glean_sdk-60.1.0/glean-core/tests/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/object.rs` & `glean_sdk-60.1.0/glean-core/tests/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/ping.rs` & `glean_sdk-60.1.0/glean-core/tests/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/ping_maker.rs` & `glean_sdk-60.1.0/glean-core/tests/ping_maker.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/quantity.rs` & `glean_sdk-60.1.0/glean-core/tests/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/rate.rs` & `glean_sdk-60.1.0/glean-core/tests/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/storage.rs` & `glean_sdk-60.1.0/glean-core/tests/storage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/string.rs` & `glean_sdk-60.1.0/glean-core/tests/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/string_list.rs` & `glean_sdk-60.1.0/glean-core/tests/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/text.rs` & `glean_sdk-60.1.0/glean-core/tests/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/timespan.rs` & `glean_sdk-60.1.0/glean-core/tests/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/tests/timing_distribution.rs` & `glean_sdk-60.1.0/glean-core/tests/timing_distribution.rs`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             lifetime: Lifetime::Ping,
             ..Default::default()
         },
         TimeUnit::Nanosecond,
     );
 
     let time = Duration::from_secs(10).as_nanos() as u64;
-    assert!(time > u64::from(u32::max_value()));
+    assert!(time > u64::from(u32::MAX));
 
     let id = 4u64.into();
     metric.set_start(id, 0);
     metric.set_stop_and_accumulate(&glean, id, time);
 
     let val = metric
         .get_value(&glean, "store1")
```

### Comparing `glean_sdk-60.0.0/glean-core/tests/uuid.rs` & `glean_sdk-60.1.0/glean-core/tests/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/README.md` & `glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/tools/embedded-uniffi-bindgen/src/main.rs` & `glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/main.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/bundle/Cargo.toml` & `glean_sdk-60.1.0/glean-core/bundle/Cargo.toml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/bundle/src/glean.udl` & `glean_sdk-60.1.0/glean-core/bundle/src/glean.udl`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/bundle/src/lib.rs` & `glean_sdk-60.1.0/glean-core/bundle/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/Cargo.lock` & `glean_sdk-60.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "glean"
-version = "60.0.0"
+version = "60.1.0"
 dependencies = [
  "crossbeam-channel",
  "env_logger",
  "flate2",
  "glean-core",
  "inherent",
  "jsonschema-valid",
@@ -355,15 +355,15 @@
 version = "1.0.0"
 dependencies = [
  "glean-core",
 ]
 
 [[package]]
 name = "glean-core"
-version = "60.0.0"
+version = "60.1.0"
 dependencies = [
  "android_logger",
  "bincode",
  "chrono",
  "crossbeam-channel",
  "ctor",
  "env_logger",
```

### Comparing `glean_sdk-60.0.0/pyproject.toml` & `glean_sdk-60.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "glean-sdk"
-version = "60.0.0"
+version = "60.1.0"
 requires-python = ">=3.8"
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
```

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/__init__.py` & `glean_sdk-60.1.0/glean-core/python/glean/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """Top-level package for Glean SDK."""
 
 import warnings
 
 
-from pkg_resources import get_distribution, DistributionNotFound
+import importlib.metadata
 from semver import VersionInfo  # type: ignore
 
 
 import glean_parser  # type: ignore
 
 
 from .glean import Glean
 from .config import Configuration
 from ._loader import load_metrics, load_pings
 
 
 __version__: str = "unknown"
 try:
-    __version__ = str(get_distribution("glean-sdk").version)
-except DistributionNotFound:  # pragma: no cover
+    __version__ = importlib.metadata.version("glean-sdk")
+except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     pass
 
 
 __author__ = "The Glean Team"
 __email__ = "glean-team@mozilla.com"
```

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_builtins.py` & `glean_sdk-60.1.0/glean-core/python/glean/_builtins.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_ffi.py` & `glean_sdk-60.1.0/glean-core/python/glean/_ffi.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_loader.py` & `glean_sdk-60.1.0/glean-core/python/glean/_loader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_process_dispatcher.py` & `glean_sdk-60.1.0/glean-core/python/glean/_process_dispatcher.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py` & `glean_sdk-60.1.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/_util.py` & `glean_sdk-60.1.0/glean-core/python/glean/_util.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/config.py` & `glean_sdk-60.1.0/glean-core/python/glean/config.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/glean.py` & `glean_sdk-60.1.0/glean-core/python/glean/glean.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics.yaml` & `glean_sdk-60.1.0/glean-core/python/glean/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/__init__.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/datetime.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/datetime.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/event.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/event.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/labeled.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/labeled.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/object.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/object.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/ping.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/ping.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/string.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/string.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/timespan.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/timespan.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/timing_distribution.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/timing_distribution.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/url.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/url.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/metrics/uuid.py` & `glean_sdk-60.1.0/glean-core/python/glean/metrics/uuid.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/net/__init__.py` & `glean_sdk-60.1.0/glean-core/python/glean/net/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/net/base_uploader.py` & `glean_sdk-60.1.0/glean-core/python/glean/net/base_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/net/http_client.py` & `glean_sdk-60.1.0/glean-core/python/glean/net/http_client.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/net/ping_upload_worker.py` & `glean_sdk-60.1.0/glean-core/python/glean/net/ping_upload_worker.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/net/ping_uploader.py` & `glean_sdk-60.1.0/glean-core/python/glean/net/ping_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/pings.yaml` & `glean_sdk-60.1.0/glean-core/python/glean/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/glean-core/python/glean/testing/__init__.py` & `glean_sdk-60.1.0/glean-core/python/glean/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/README.md` & `glean_sdk-60.1.0/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/LICENSE` & `glean_sdk-60.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.0.0/PKG-INFO` & `glean_sdk-60.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: glean-sdk
-Version: 60.0.0
+Version: 60.1.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: semver >=2.13.0
 Requires-Dist: glean-parser ~=14.0
```

