# Comparing `tmp/linktest-2.7.1.tar.gz` & `tmp/linktest-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.1.tar", last modified: Mon May  6 03:14:31 2024, max compression
+gzip compressed data, was "linktest-2.7.2.tar", last modified: Mon May  6 08:26:47 2024, max compression
```

## Comparing `linktest-2.7.1.tar` & `linktest-2.7.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.625067 linktest-2.7.1/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 03:14:31.624716 linktest-2.7.1/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.622396 linktest-2.7.1/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-06 03:04:06.000000 linktest-2.7.1/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33518 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103537 2024-05-05 06:17:36.000000 linktest-2.7.1/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8967 2024-05-06 03:07:54.000000 linktest-2.7.1/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 03:04:15.000000 linktest-2.7.1/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14080 2024-05-06 03:10:41.000000 linktest-2.7.1/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-06 03:10:25.000000 linktest-2.7.1/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-06 03:11:46.000000 linktest-2.7.1/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-06 03:12:43.000000 linktest-2.7.1/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-06 03:12:15.000000 linktest-2.7.1/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-03 09:39:48.000000 linktest-2.7.1/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 03:14:31.624331 linktest-2.7.1/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-06 03:14:31.000000 linktest-2.7.1/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-06 03:14:31.625122 linktest-2.7.1/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 03:14:26.000000 linktest-2.7.1/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:26:47.839064 linktest-2.7.2/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 08:26:47.837558 linktest-2.7.2/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:26:47.827211 linktest-2.7.2/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-06 08:11:41.000000 linktest-2.7.2/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33518 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103054 2024-05-06 08:14:33.000000 linktest-2.7.2/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9369 2024-05-06 08:11:05.000000 linktest-2.7.2/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 08:11:47.000000 linktest-2.7.2/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13936 2024-05-06 07:42:00.000000 linktest-2.7.2/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-06 05:48:02.000000 linktest-2.7.2/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:26:47.835977 linktest-2.7.2/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 08:26:47.000000 linktest-2.7.2/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-06 08:26:47.000000 linktest-2.7.2/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-06 08:26:47.000000 linktest-2.7.2/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-06 08:26:47.000000 linktest-2.7.2/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-06 08:26:47.000000 linktest-2.7.2/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-06 08:26:47.839141 linktest-2.7.2/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 08:26:31.000000 linktest-2.7.2/setup.py
```

### Comparing `linktest-2.7.1/linktest/appium_utils.py` & `linktest-2.7.2/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/auto_generate_testcase_list.py` & `linktest-2.7.2/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.2/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/base_testcase.py` & `linktest-2.7.2/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/clean_data.py` & `linktest-2.7.2/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/conver_xml_into_db.py` & `linktest-2.7.2/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/database_helper.py` & `linktest-2.7.2/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/date_utilities.py` & `linktest-2.7.2/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/doctor.py` & `linktest-2.7.2/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/framework_log.py` & `linktest-2.7.2/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/generate_html_log.py` & `linktest-2.7.2/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/get_adb_devices.py` & `linktest-2.7.2/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/get_ios_devices_list.py` & `linktest-2.7.2/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/get_platform_info.py` & `linktest-2.7.2/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/get_project_info.py` & `linktest-2.7.2/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/html_report.py` & `linktest-2.7.2/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/logged_requests.py` & `linktest-2.7.2/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/main.py` & `linktest-2.7.2/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,33 +395,14 @@
     settings.QUEUE_SIZE = 1
 
 try:
     from settings import LOG_FORMAT
 except ImportError:
     settings.LOG_FORMAT = '%(asctime)s %(levelname)s %(filename)s %(lineno)d: %(message)s'
 
-try:
-    from settings import AUTO_DOWNLOAD_CHROMEDRIVER
-except ImportError:
-    settings.AUTO_DOWNLOAD_CHROMEDRIVER = False
-
-try:
-    from settings import AUTO_SCREENSHOT_ON_ACTION
-except ImportError:
-    settings.AUTO_SCREENSHOT_ON_ACTION = False
-
-try:
-    from settings import SAVE_SCREENSHOT_FOR_PASSED_TESTS
-except ImportError:
-    settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS = False
-
-if settings.AUTO_SCREENSHOT_ON_ACTION:
-    settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS = False
-
-
 
 # set Default time_zone = 'Asia/Shanghai'
 if hasattr(settings, "TIME_ZONE"):
     if settings.TIME_ZONE:
         os.environ['TZ'] = '%s' % settings.TIME_ZONE
 else:
     os.environ['TZ'] = 'Asia/Shanghai'
```

### Comparing `linktest-2.7.1/linktest/memory_usage.py` & `linktest-2.7.2/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/re_func.py` & `linktest-2.7.2/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/run.py` & `linktest-2.7.2/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/run_testcase_thread.py` & `linktest-2.7.2/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/scp_report_to_specified_path.py` & `linktest-2.7.2/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/selenium_helper.py` & `linktest-2.7.2/linktest/selenium_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import os
 import platform
 import traceback
 import subprocess
 from selenium import webdriver
 
-from .webdriver_wrapper_firefox import WebDriverWrapperFireFox
-from .webdriver_wrapper_edge import WebDriverWrapperEdge
-from .webdriver_wrapper_chrome import WebDriverWrapperChrome
-from .webdriver_wrapper_safari import WebDriverWrapperSafari
-from .webdriver_wrapper_ie import WebDriverWrapperIE
 
 try:
     import settings
 except ImportError:
     traceback.print_exc()
 
 try:
@@ -70,29 +65,36 @@
 
                 return browser
 
         else:
             from selenium import webdriver
 
             if browser_name == 'ie':
-                    browser = WebDriverWrapperIE(ui_testcase)
+                from .webdriver_wrapper_ie import WebDriverWrapperIE
+                browser = WebDriverWrapperIE(ui_testcase)
             elif browser_name == 'edge':
+                from .webdriver_wrapper_edge import WebDriverWrapperEdge
+
                 if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
                     edge_options = webdriver.EdgeOptions()
                     edge_options.add_argument("--headless")
 
                     # 使用 WebDriverWrapperEdge 替换原来的 webdriver 实例
                     browser = WebDriverWrapperEdge(ui_testcase, options=edge_options)
                 else:
                     browser = WebDriverWrapperEdge(ui_testcase)
 
             elif browser_name == 'safari':
-                    browser = WebDriverWrapperSafari(ui_testcase)
+                from .webdriver_wrapper_safari import WebDriverWrapperSafari
+                browser = WebDriverWrapperSafari(ui_testcase)
 
             elif browser_name == 'chrome':
+                # 在运行时导入的原因是：用户启动脚本时可能会传入不同的参数。这些参数会直接影响 WebDriverWrapperChrome 中对 settings 模块配置项的读取。
+                # 因为在 main.py 中，框架会根据用户提供的配置动态地修改 settings 模块中的配置项。
+                from .webdriver_wrapper_chrome import WebDriverWrapperChrome
                 chrome_options = webdriver.ChromeOptions()
                 chrome_options.add_argument("--disable-infobars")
 
                 if hasattr(settings, "BROWSER_OPTION"):
                     for opt in settings.BROWSER_OPTION:
                         if type(opt) is str:
                             chrome_options.add_argument(opt)
@@ -121,14 +123,16 @@
                         browser = WebDriverWrapperChrome(ui_testcase, options=chrome_options)
                     else:
                         # browser = webdriver.Chrome()
                         # 使用 WebDriverWrapperChrome 替换原来的 webdriver 实例
                         browser = WebDriverWrapperChrome(ui_testcase)
 
             elif browser_name in ('firefox', 'ff'):
+                from .webdriver_wrapper_firefox import WebDriverWrapperFireFox
+
                 if hasattr(settings, "HEAD_LESS") and settings.HEAD_LESS:
                     firefox_options = webdriver.FirefoxOptions()
                     firefox_options.add_argument("--headless")
 
                     # 使用 WebDriverWrapperFireFox 替换原来的 webdriver 实例
                     browser = WebDriverWrapperFireFox(ui_testcase, options=firefox_options)
                 else:
```

### Comparing `linktest-2.7.1/linktest/timeout_thread.py` & `linktest-2.7.2/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/ui_testcase.py` & `linktest-2.7.2/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/update_config.py` & `linktest-2.7.2/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper.py` & `linktest-2.7.2/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.2/linktest/webdriver_wrapper_chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,20 @@
 
 from selenium.webdriver.chrome.webdriver import WebDriver as Chrome
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 from selenium.webdriver.remote.webelement import WebElement
 
-AUTO_SCREENSHOT_ON_ACTION = False
-
 try:
     import settings
 except BaseException:
     raise ("No settings module found ....")
 
-try:
-    from settings import AUTO_SCREENSHOT_ON_ACTION
-
-    AUTO_SCREENSHOT_ON_ACTION = settings.AUTO_SCREENSHOT_ON_ACTION
-except ImportError:
-    settings.AUTO_SCREENSHOT_ON_ACTION = False
+AUTO_SCREENSHOT_ON_ACTION = getattr(settings, "AUTO_SCREENSHOT_ON_ACTION", False)
 
 
 class WebElementWrapper:
     def __init__(self, element, logger, this):
         self.element = element
         self.logger = logger
         self.webdriver_wrapper = this
```

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.2/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.2/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.2/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.2/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest/xml_report.py` & `linktest-2.7.2/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.1/linktest.egg-info/SOURCES.txt` & `linktest-2.7.2/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

