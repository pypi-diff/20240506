# Comparing `tmp/linktest-2.7.0.tar.gz` & `tmp/linktest-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.0.tar", last modified: Fri May  3 09:36:22 2024, max compression
+gzip compressed data, was "linktest-2.7.1.tar", last modified: Mon May  6 03:14:31 2024, max compression
```

## Comparing `linktest-2.7.0.tar` & `linktest-2.7.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 09:36:22.809125 linktest-2.7.0/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-03 09:36:22.808777 linktest-2.7.0/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 09:36:22.805643 linktest-2.7.0/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-03 09:33:05.000000 linktest-2.7.0/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33518 2024-05-03 09:28:58.000000 linktest-2.7.0/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103498 2024-05-03 09:27:36.000000 linktest-2.7.0/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-03 09:33:12.000000 linktest-2.7.0/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-03 08:13:13.000000 linktest-2.7.0/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 09:36:22.808403 linktest-2.7.0/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-03 09:36:22.000000 linktest-2.7.0/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-03 09:36:22.000000 linktest-2.7.0/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-03 09:36:22.000000 linktest-2.7.0/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-03 09:36:22.000000 linktest-2.7.0/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-03 09:36:22.000000 linktest-2.7.0/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-03 09:36:22.809191 linktest-2.7.0/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-03 09:36:15.000000 linktest-2.7.0/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.625067 linktest-2.7.1/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 03:14:31.624716 linktest-2.7.1/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.622396 linktest-2.7.1/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-06 03:04:06.000000 linktest-2.7.1/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33518 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103537 2024-05-05 06:17:36.000000 linktest-2.7.1/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8967 2024-05-06 03:07:54.000000 linktest-2.7.1/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 03:04:15.000000 linktest-2.7.1/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14080 2024-05-06 03:10:41.000000 linktest-2.7.1/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-06 03:10:25.000000 linktest-2.7.1/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-06 03:11:46.000000 linktest-2.7.1/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-06 03:12:43.000000 linktest-2.7.1/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-06 03:12:15.000000 linktest-2.7.1/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.624331 linktest-2.7.1/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-06 03:14:31.625122 linktest-2.7.1/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 03:14:26.000000 linktest-2.7.1/setup.py
```

### Comparing `linktest-2.7.0/linktest/appium_utils.py` & `linktest-2.7.1/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/auto_generate_testcase_list.py` & `linktest-2.7.1/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.1/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/base_testcase.py` & `linktest-2.7.1/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/clean_data.py` & `linktest-2.7.1/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/conver_xml_into_db.py` & `linktest-2.7.1/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/database_helper.py` & `linktest-2.7.1/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/date_utilities.py` & `linktest-2.7.1/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/doctor.py` & `linktest-2.7.1/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/framework_log.py` & `linktest-2.7.1/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/generate_html_log.py` & `linktest-2.7.1/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/get_adb_devices.py` & `linktest-2.7.1/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/get_ios_devices_list.py` & `linktest-2.7.1/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/get_platform_info.py` & `linktest-2.7.1/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/get_project_info.py` & `linktest-2.7.1/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/html_report.py` & `linktest-2.7.1/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/logged_requests.py` & `linktest-2.7.1/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/main.py` & `linktest-2.7.1/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2067,15 +2067,15 @@
                                          PLATFORM_INFO,
                                          len(BaseTestCase.GlobalDataList) > 0,
                                          True)
                 except BaseException:
                     traceback.print_exc()
 
             print(
-                "=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
+                "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
 
             # save the execution summary into DB (environment, total_execution_time,
             try:
                 import linktest
                 from . import database_helper
                 if hasattr(settings, "SAVE_LOG_TO_DB"):
                     if settings.SAVE_LOG_TO_DB is True:
```

### Comparing `linktest-2.7.0/linktest/memory_usage.py` & `linktest-2.7.1/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/re_func.py` & `linktest-2.7.1/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/run.py` & `linktest-2.7.1/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/run_testcase_thread.py` & `linktest-2.7.1/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/scp_report_to_specified_path.py` & `linktest-2.7.1/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/selenium_helper.py` & `linktest-2.7.1/linktest/selenium_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,18 @@
 try:
     import settings
 except ImportError:
     traceback.print_exc()
 
 try:
     if hasattr(settings, "run_by_github_action") and settings.run_by_github_action is True:
+        # todo 此次逻辑需要再优化一下
         pass
     else:
-        try:
-            from settings import auto_download_chromedriver
-        except ImportError:
-            auto_download_chromedriver = False
-
-        if auto_download_chromedriver is True:
+        if getattr(settings, "AUTO_DOWNLOAD_CHROMEDRIVER", False):
             import chromedriver_autoinstaller
 
             chromedriver_autoinstaller.install()
 except BaseException:
     traceback.print_exc()
```

### Comparing `linktest-2.7.0/linktest/timeout_thread.py` & `linktest-2.7.1/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/ui_testcase.py` & `linktest-2.7.1/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/update_config.py` & `linktest-2.7.1/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper.py` & `linktest-2.7.1/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.1/linktest/webdriver_wrapper_safari.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 
-from selenium.webdriver.chrome.webdriver import WebDriver as Chrome
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.safari.webdriver import WebDriver as Safari
+from selenium.webdriver.safari.options import Options
+from selenium.webdriver.safari.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
@@ -225,15 +225,15 @@
         return_value = self.element.__hash__()
         self._log_action("__hash__")
         return return_value
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
-class WebDriverWrapperChrome(Chrome):
+class WebDriverWrapperSafari(Safari):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
         # Default options and service for Chrome, if not provided in kwargs
         options = kwargs.pop('options', Options())
         service = None # todo macOS VS windows
@@ -284,50 +284,51 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         return_value = super().execute_async_script(script, *args)
         self._log_action("execute_async_script", script, *args)
         return return_value
 
+    @property
     def title(self) -> str:
         return_value = super().title
         self._log_action("title")
         return return_value
 
-    # def create_web_element(self, element_id: str) -> WebElement:
-    #     self._log_action("create_web_element", element_id)
-    #     return super().create_web_element(element_id)
-
     def start_session(self, capabilities: dict) -> None:
         super().start_session(capabilities)
         self._log_action("start_session", capabilities)
 
+    @property
     def current_url(self) -> str:
         return_value = super().current_url
         self._log_action("current_url")
         return return_value
 
+    @property
     def page_source(self) -> str:
         return_value = super().page_source
         self._log_action("page_source")
         return return_value
 
     def close(self) -> None:
         super().close()
         self._log_action("close")
 
     def quit(self) -> None:
         super().quit()
         self._log_action("quit")
 
+    @property
     def current_window_handle(self) -> str:
         return_value = super().current_window_handle
         self._log_action("current_window_handle")
         return return_value
 
+    @property
     def window_handles(self) -> List[str]:
         return_value = super().window_handles
         self._log_action("window_handles")
         return return_value
 
     def maximize_window(self) -> None:
         super().maximize_window()
```

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.1/linktest/webdriver_wrapper_chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 
-from selenium.webdriver.edge.webdriver import WebDriver as Edge
-from selenium.webdriver.edge.options import Options
-from selenium.webdriver.edge.service import Service
+from selenium.webdriver.chrome.webdriver import WebDriver as Chrome
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.chrome.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
@@ -225,23 +225,25 @@
         return_value = self.element.__hash__()
         self._log_action("__hash__")
         return return_value
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
-class WebDriverWrapperEdge(Edge):
+class WebDriverWrapperChrome(Chrome):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
+        # Default options and service for Chrome, if not provided in kwargs
         options = kwargs.pop('options', Options())
-        service = None
+        service = None # todo macOS VS windows
         keep_alive = kwargs.pop('keep_alive', True)
 
+        # Initialization of the Chrome WebDriver with the correct parameters
         super().__init__(options=options, service=service, keep_alive=keep_alive, *args, **kwargs)
 
     def _log_action(self, action, *args):
         if args:
             msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
         else:
             msg = f"- WebDriver Action: '{action}'"
@@ -250,15 +252,14 @@
 
     def get(self, url):
         super().get(url)
         self._log_action("get", url)
         if AUTO_SCREENSHOT_ON_ACTION:
             self.save_screenshot()
 
-
     def find_element(self, by=By.ID, value=None):
         element = super().find_element(by, value)
         this = self
         return_value = WebElementWrapper(element, self.logger, this)
         self._log_action("find_element", by, value)
         return return_value
 
@@ -277,50 +278,55 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         return_value = super().execute_async_script(script, *args)
         self._log_action("execute_async_script", script, *args)
         return return_value
 
+    @property
     def title(self) -> str:
         return_value = super().title
         self._log_action("title")
         return return_value
 
     # def create_web_element(self, element_id: str) -> WebElement:
     #     self._log_action("create_web_element", element_id)
     #     return super().create_web_element(element_id)
 
     def start_session(self, capabilities: dict) -> None:
         super().start_session(capabilities)
         self._log_action("start_session", capabilities)
 
+    @property
     def current_url(self) -> str:
         return_value = super().current_url
         self._log_action("current_url")
         return return_value
 
+    @property
     def page_source(self) -> str:
         return_value = super().page_source
         self._log_action("page_source")
         return return_value
 
     def close(self) -> None:
         super().close()
         self._log_action("close")
 
     def quit(self) -> None:
         super().quit()
         self._log_action("quit")
 
+    @property
     def current_window_handle(self) -> str:
         return_value = super().current_window_handle
         self._log_action("current_window_handle")
         return return_value
 
+    @property
     def window_handles(self) -> List[str]:
         return_value = super().window_handles
         self._log_action("window_handles")
         return return_value
 
     def maximize_window(self) -> None:
         super().maximize_window()
```

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.1/linktest/webdriver_wrapper_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 
-from selenium.webdriver.firefox.webdriver import WebDriver as FireFox
-from selenium.webdriver.firefox.options import Options
-from selenium.webdriver.firefox.service import Service
+from selenium.webdriver.edge.webdriver import WebDriver as Edge
+from selenium.webdriver.edge.options import Options
+from selenium.webdriver.edge.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
@@ -225,15 +225,15 @@
         return_value = self.element.__hash__()
         self._log_action("__hash__")
         return return_value
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
-class WebDriverWrapperFireFox(FireFox):
+class WebDriverWrapperEdge(Edge):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
         options = kwargs.pop('options', Options())
         service = None
         keep_alive = kwargs.pop('keep_alive', True)
@@ -277,50 +277,51 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         return_value = super().execute_async_script(script, *args)
         self._log_action("execute_async_script", script, *args)
         return return_value
 
+    @property
     def title(self) -> str:
         return_value = super().title
         self._log_action("title")
         return return_value
 
-    # def create_web_element(self, element_id: str) -> WebElement:
-    #     self._log_action("create_web_element", element_id)
-    #     return super().create_web_element(element_id)
-
     def start_session(self, capabilities: dict) -> None:
         super().start_session(capabilities)
         self._log_action("start_session", capabilities)
 
+    @property
     def current_url(self) -> str:
         return_value = super().current_url
         self._log_action("current_url")
         return return_value
 
+    @property
     def page_source(self) -> str:
         return_value = super().page_source
         self._log_action("page_source")
         return return_value
 
     def close(self) -> None:
         super().close()
         self._log_action("close")
 
     def quit(self) -> None:
         super().quit()
         self._log_action("quit")
 
+    @property
     def current_window_handle(self) -> str:
         return_value = super().current_window_handle
         self._log_action("current_window_handle")
         return return_value
 
+    @property
     def window_handles(self) -> List[str]:
         return_value = super().window_handles
         self._log_action("window_handles")
         return return_value
 
     def maximize_window(self) -> None:
         super().maximize_window()
```

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.1/linktest/webdriver_wrapper_firefox.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 
-from selenium.webdriver.ie.webdriver import WebDriver as IE
-from selenium.webdriver.ie.options import Options
-from selenium.webdriver.ie.service import Service
+from selenium.webdriver.firefox.webdriver import WebDriver as FireFox
+from selenium.webdriver.firefox.options import Options
+from selenium.webdriver.firefox.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
@@ -225,15 +225,15 @@
         return_value = self.element.__hash__()
         self._log_action("__hash__")
         return return_value
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
-class WebDriverWrapperIE(IE):
+class WebDriverWrapperFireFox(FireFox):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
         options = kwargs.pop('options', Options())
         service = None
         keep_alive = kwargs.pop('keep_alive', True)
@@ -277,50 +277,51 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         return_value = super().execute_async_script(script, *args)
         self._log_action("execute_async_script", script, *args)
         return return_value
 
+    @property
     def title(self) -> str:
         return_value = super().title
         self._log_action("title")
         return return_value
 
-    # def create_web_element(self, element_id: str) -> WebElement:
-    #     self._log_action("create_web_element", element_id)
-    #     return super().create_web_element(element_id)
-
     def start_session(self, capabilities: dict) -> None:
         super().start_session(capabilities)
         self._log_action("start_session", capabilities)
 
+    @property
     def current_url(self) -> str:
         return_value = super().current_url
         self._log_action("current_url")
         return return_value
 
+    @property
     def page_source(self) -> str:
         return_value = super().page_source
         self._log_action("page_source")
         return return_value
 
     def close(self) -> None:
         super().close()
         self._log_action("close")
 
     def quit(self) -> None:
         super().quit()
         self._log_action("quit")
 
+    @property
     def current_window_handle(self) -> str:
         return_value = super().current_window_handle
         self._log_action("current_window_handle")
         return return_value
 
+    @property
     def window_handles(self) -> List[str]:
         return_value = super().window_handles
         self._log_action("window_handles")
         return return_value
 
     def maximize_window(self) -> None:
         super().maximize_window()
```

### Comparing `linktest-2.7.0/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.1/linktest/webdriver_wrapper_ie.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
 
-from selenium.webdriver.safari.webdriver import WebDriver as Safari
-from selenium.webdriver.safari.options import Options
-from selenium.webdriver.safari.service import Service
+from selenium.webdriver.ie.webdriver import WebDriver as IE
+from selenium.webdriver.ie.options import Options
+from selenium.webdriver.ie.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
@@ -225,25 +225,23 @@
         return_value = self.element.__hash__()
         self._log_action("__hash__")
         return return_value
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
-class WebDriverWrapperSafari(Safari):
+class WebDriverWrapperIE(IE):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
-        # Default options and service for Chrome, if not provided in kwargs
         options = kwargs.pop('options', Options())
-        service = None # todo macOS VS windows
+        service = None
         keep_alive = kwargs.pop('keep_alive', True)
 
-        # Initialization of the Chrome WebDriver with the correct parameters
         super().__init__(options=options, service=service, keep_alive=keep_alive, *args, **kwargs)
 
     def _log_action(self, action, *args):
         if args:
             msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
         else:
             msg = f"- WebDriver Action: '{action}'"
@@ -252,19 +250,14 @@
 
     def get(self, url):
         super().get(url)
         self._log_action("get", url)
         if AUTO_SCREENSHOT_ON_ACTION:
             self.save_screenshot()
 
-    # def find_element(self, by=By.ID, value=None):
-    #     self._log_action("find_element", by, value)
-    #     element = super().find_element(by, value)
-    #     this = self
-    #     return WebElementWrapper(element, self.logger, this)
 
     def find_element(self, by=By.ID, value=None):
         element = super().find_element(by, value)
         this = self
         return_value = WebElementWrapper(element, self.logger, this)
         self._log_action("find_element", by, value)
         return return_value
@@ -284,50 +277,51 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         return_value = super().execute_async_script(script, *args)
         self._log_action("execute_async_script", script, *args)
         return return_value
 
+    @property
     def title(self) -> str:
         return_value = super().title
         self._log_action("title")
         return return_value
 
-    # def create_web_element(self, element_id: str) -> WebElement:
-    #     self._log_action("create_web_element", element_id)
-    #     return super().create_web_element(element_id)
-
     def start_session(self, capabilities: dict) -> None:
         super().start_session(capabilities)
         self._log_action("start_session", capabilities)
 
+    @property
     def current_url(self) -> str:
         return_value = super().current_url
         self._log_action("current_url")
         return return_value
 
+    @property
     def page_source(self) -> str:
         return_value = super().page_source
         self._log_action("page_source")
         return return_value
 
     def close(self) -> None:
         super().close()
         self._log_action("close")
 
     def quit(self) -> None:
         super().quit()
         self._log_action("quit")
 
+    @property
     def current_window_handle(self) -> str:
         return_value = super().current_window_handle
         self._log_action("current_window_handle")
         return return_value
 
+    @property
     def window_handles(self) -> List[str]:
         return_value = super().window_handles
         self._log_action("window_handles")
         return return_value
 
     def maximize_window(self) -> None:
         super().maximize_window()
```

### Comparing `linktest-2.7.0/linktest/xml_report.py` & `linktest-2.7.1/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.0/linktest.egg-info/SOURCES.txt` & `linktest-2.7.1/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

