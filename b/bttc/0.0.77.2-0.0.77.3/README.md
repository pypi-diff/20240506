# Comparing `tmp/bttc-0.0.77.2.tar.gz` & `tmp/bttc-0.0.77.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.77.2.tar", last modified: Sun May  5 01:41:46 2024, max compression
+gzip compressed data, was "bttc-0.0.77.3.tar", last modified: Mon May  6 14:51:46 2024, max compression
```

## Comparing `bttc-0.0.77.2.tar` & `bttc-0.0.77.3.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.074468 bttc-0.0.77.2/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.2/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-05 01:41:46.074468 bttc-0.0.77.2/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-05 01:26:33.000000 bttc-0.0.77.2/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.066468 bttc-0.0.77.2/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-05 01:41:37.000000 bttc-0.0.77.2/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.2/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.2/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.066468 bttc-0.0.77.2/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.2/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.2/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77.2/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    35298 2024-05-05 01:21:12.000000 bttc-0.0.77.2/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.062468 bttc-0.0.77.2/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.2/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.2/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77.2/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.070468 bttc-0.0.77.2/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-05 01:33:18.000000 bttc-0.0.77.2/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.074468 bttc-0.0.77.2/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.2/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    17093 2024-05-05 01:41:20.000000 bttc-0.0.77.2/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.2/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.2/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-05 01:41:46.066468 bttc-0.0.77.2/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-05 01:41:46.000000 bttc-0.0.77.2/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1587 2024-05-05 01:41:46.000000 bttc-0.0.77.2/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-05 01:41:46.000000 bttc-0.0.77.2/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-05 01:41:46.000000 bttc-0.0.77.2/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-05 01:41:46.000000 bttc-0.0.77.2/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-05 01:41:46.074468 bttc-0.0.77.2/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.2/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.3/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-06 14:51:46.257136 bttc-0.0.77.3/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-06 13:58:19.000000 bttc-0.0.77.3/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.249136 bttc-0.0.77.3/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-06 14:51:31.000000 bttc-0.0.77.3/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.3/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.3/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.3/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.3/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    36150 2024-05-06 14:42:05.000000 bttc-0.0.77.3/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.249136 bttc-0.0.77.3/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.3/bttc/utils/device_factory.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2336 2024-05-06 07:32:12.000000 bttc-0.0.77.3/bttc/utils/dialer_simulator.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.77.3/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.3/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    17093 2024-05-06 13:58:19.000000 bttc-0.0.77.3/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-06 14:51:46.257136 bttc-0.0.77.3/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.3/setup.py
```

### Comparing `bttc-0.0.77.2/LICENSE` & `bttc-0.0.77.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/PKG-INFO` & `bttc-0.0.77.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77.2
+Version: 0.0.77.3
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77.2/README.md` & `bttc-0.0.77.3/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/__init__.py` & `bttc-0.0.77.3/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.77.2'
+__version__ = '0.0.77.3'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.77.2/bttc/apk_utils.py` & `bttc-0.0.77.3/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/ble_data.py` & `bttc-0.0.77.3/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/ble_utils.py` & `bttc-0.0.77.3/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/bt_data.py` & `bttc-0.0.77.3/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/bt_utils.py` & `bttc-0.0.77.3/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/cli/__init__.py` & `bttc-0.0.77.3/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/cli/constants.py` & `bttc-0.0.77.3/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/cli/main.py` & `bttc-0.0.77.3/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/common_data.py` & `bttc-0.0.77.3/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/constants.py` & `bttc-0.0.77.3/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/core.py` & `bttc-0.0.77.3/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/errors.py` & `bttc-0.0.77.3/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/general_data.py` & `bttc-0.0.77.3/bttc/general_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/general_utils.py` & `bttc-0.0.77.3/bttc/general_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -363,14 +363,15 @@
     self._bind(get_ui_xml)
     self._bind(get_all_volume)
     self._bind(get_volume)
     self._bind(is_apk_installed)
     self._bind(logcat_filter)
     self.props = Props(self._ad)
     self._bind(push_file)
+    self._bind(push_non_persistent_property)
     self._bind(set_volume)
     self.shell = bt_utils.safe_adb_shell(ad)
     self._bind(take_screenshot)
 
   @property
   def airplane_mode(self) -> bool:
     """Gets the current airplane mode status of the device.
@@ -1171,14 +1172,43 @@
         "Failed to copy %s to %s: %s", src_file_path, dst_file_path, out
     )
     return False
 
   return True
 
 
+def push_non_persistent_property(
+    ad: typing_utils.AdbDevice,
+    property_name: str, property_value: str) -> None:
+  """Pushes non persistent property.
+
+  Args:
+    ad: An Adb-like device object representing the DUT.
+    property_name: Name of property.
+    property_value: Value of property.
+
+  Raises:
+    adb.AdbError: Failed in pushing the desired property.
+  """
+  if ad.gm.props[property_name] == property_value:
+    logging.info('Property="%s" is already set!', property_name)
+    return
+
+  ad.adb.shell(
+      f"'echo {property_name}={property_value} >> /data/local.prop'",
+      shell=True)
+
+  try:
+    ad.adb.shell("'chmod 644 /data/local.prop'", shell=True)
+  except adb.AdbError as ex:
+    ad.log.error(
+        f'Failed to push persistent property="{property_name}": {ex}')
+    raise ex
+
+
 def set_volume(
     ad: typing_utils.AdbDevice,
     volume_type: general_data.VolumeType,
     level: int,
     sync_wait_sec: int = 2) -> str:
   """Sets the level of a certain volume type.
```

### Comparing `bttc-0.0.77.2/bttc/mc_data.py` & `bttc-0.0.77.3/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/mc_utils.py` & `bttc-0.0.77.3/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.77.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.77.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.77.3/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/avrcp/errors.py` & `bttc-0.0.77.3/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/__init__.py` & `bttc-0.0.77.3/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/constants.py` & `bttc-0.0.77.3/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/errors.py` & `bttc-0.0.77.3/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.77.3/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.77.3/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.77.3/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.77.3/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/strategy.py` & `bttc-0.0.77.3/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ad_checker.py` & `bttc-0.0.77.3/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/device_factory.py` & `bttc-0.0.77.3/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/iperf/__init__.py` & `bttc-0.0.77.3/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/iperf/errors.py` & `bttc-0.0.77.3/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/key_events_handler.py` & `bttc-0.0.77.3/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/log_parser.py` & `bttc-0.0.77.3/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/logcat.py` & `bttc-0.0.77.3/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.77.3/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.77.3/bttc/utils/media_player/yt_player_agent.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/retry.py` & `bttc-0.0.77.3/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/typing_utils.py` & `bttc-0.0.77.3/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.77.3/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ui_pages/errors.py` & `bttc-0.0.77.3/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.77.3/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.77.3/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils/ui_pages/utils.py` & `bttc-0.0.77.3/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/utils_loader.py` & `bttc-0.0.77.3/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc/wifi_utils.py` & `bttc-0.0.77.3/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.2/bttc.egg-info/PKG-INFO` & `bttc-0.0.77.3/bttc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77.2
+Version: 0.0.77.3
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77.2/bttc.egg-info/SOURCES.txt` & `bttc-0.0.77.3/bttc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 bttc/profiles/hfp/errors.py
 bttc/profiles/hfp/hfp_data.py
 bttc/profiles/hfp/hfp_devices.py
 bttc/profiles/hfp/hfp_facade.py
 bttc/profiles/hfp/hfp_strategy.py
 bttc/utils/ad_checker.py
 bttc/utils/device_factory.py
+bttc/utils/dialer_simulator.py
 bttc/utils/key_events_handler.py
 bttc/utils/log_parser.py
 bttc/utils/logcat.py
 bttc/utils/retry.py
 bttc/utils/typing_utils.py
 bttc/utils/iperf/__init__.py
 bttc/utils/iperf/errors.py
```

### Comparing `bttc-0.0.77.2/setup.py` & `bttc-0.0.77.3/setup.py`

 * *Files identical despite different names*

