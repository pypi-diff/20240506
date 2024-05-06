# Comparing `tmp/libsrg-5.0.0.tar.gz` & `tmp/libsrg-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg-5.0.0.tar", max compression
+gzip compressed data, was "libsrg-5.1.0.tar", max compression
```

## Comparing `libsrg-5.0.0.tar` & `libsrg-5.1.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
--rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.0.0/README.md
--rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.0.0/libsrg/AppTemplate.py
--rw-r--r--   0        0        0    11392 2024-05-04 13:48:11.572363 libsrg-5.0.0/libsrg/Config.py
--rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.0.0/libsrg/ElapsedTime.py
--rwxr-xr-x   0        0        0     8002 2024-05-03 23:47:01.863721 libsrg-5.0.0/libsrg/Info.py
--rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.0.0/libsrg/LevelBanner.py
--rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.0.0/libsrg/LoggerGUIProxy.py
--rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.0.0/libsrg/LoggingAppBase.py
--rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.0.0/libsrg/LoggingCounter.py
--rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.0.0/libsrg/LoggingUtils.py
--rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.0.0/libsrg/LoggingWatcher.py
--rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.0.0/libsrg/NagiosBase.py
--rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.0.0/libsrg/Runner.py
--rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.0.0/libsrg/Runner2.py
--rw-r--r--   0        0        0     4508 2024-04-21 12:42:50.283800 libsrg-5.0.0/libsrg/Statistics/ADStatsBase.py
--rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.0.0/libsrg/Statistics/AnalogStatsBase.py
--rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.0.0/libsrg/Statistics/AnalogStatsCumulative.py
--rw-r--r--   0        0        0     2300 2024-04-08 17:02:20.939118 libsrg-5.0.0/libsrg/Statistics/AnalogStatsFading.py
--rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.0.0/libsrg/Statistics/AnalogStatsSlidingWindow.py
--rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsBase.py
--rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsCumulative.py
--rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py
--rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.0.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py
--rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
--rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
--rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
--rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
--rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
--rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.0.0/libsrg/Statistics/UnitTests/__init__.py
--rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
--rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
--rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.0.0/libsrg/Statistics/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.0.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
--rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.0.0/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.0.0/libsrg/TKGUI/GuiBase.py
--rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.0.0/libsrg/TKGUI/GuiRequest.py
--rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.0.0/libsrg/TKGUI/GuiRequestQueue.py
--rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.0.0/libsrg/TKGUI/LoggerGUI.py
--rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.0.0/libsrg/TKGUI/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
--rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
--rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.0.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
--rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.0.0/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.0.0/libsrg/UnitTests/Config_test.py
--rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.0.0/libsrg/UnitTests/RolloverTest_filename.py
--rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.0.0/libsrg/UnitTests/RolloverTest_logfile.py
--rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.0.0/libsrg/UnitTests/Sample.env
--rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.0.0/libsrg/UnitTests/Sample.ini
--rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.0.0/libsrg/UnitTests/Sample.json
--rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.0.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
--rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.0.0/libsrg/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-04 14:33:28.588647 libsrg-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.1.0/README.md
+-rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.1.0/libsrg/AppTemplate.py
+-rw-r--r--   0        0        0    11933 2024-05-06 15:12:41.996241 libsrg-5.1.0/libsrg/Config.py
+-rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.1.0/libsrg/ElapsedTime.py
+-rwxr-xr-x   0        0        0     8847 2024-05-06 15:00:11.302960 libsrg-5.1.0/libsrg/Info.py
+-rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.1.0/libsrg/LevelBanner.py
+-rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.1.0/libsrg/LoggerGUIProxy.py
+-rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.1.0/libsrg/LoggingAppBase.py
+-rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.1.0/libsrg/LoggingCounter.py
+-rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.1.0/libsrg/LoggingUtils.py
+-rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.1.0/libsrg/LoggingWatcher.py
+-rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.1.0/libsrg/NagiosBase.py
+-rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.1.0/libsrg/Runner.py
+-rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.1.0/libsrg/Runner2.py
+-rw-r--r--   0        0        0     4523 2024-05-06 14:42:50.143127 libsrg-5.1.0/libsrg/Statistics/ADStatsBase.py
+-rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.1.0/libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.1.0/libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--   0        0        0     2302 2024-05-06 14:43:05.792050 libsrg-5.1.0/libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.1.0/libsrg/Statistics/AnalogStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.1.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.1.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py
+-rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.1.0/libsrg/Statistics/UnitTests/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
+-rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.1.0/libsrg/Statistics/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.1.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
+-rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.1.0/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.1.0/libsrg/TKGUI/GuiBase.py
+-rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.1.0/libsrg/TKGUI/GuiRequest.py
+-rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.1.0/libsrg/TKGUI/GuiRequestQueue.py
+-rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.1.0/libsrg/TKGUI/LoggerGUI.py
+-rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.1.0/libsrg/TKGUI/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
+-rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
+-rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.1.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.1.0/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.1.0/libsrg/UnitTests/Config_test.py
+-rw-r--r--   0        0        0      470 2024-05-06 14:29:21.184142 libsrg-5.1.0/libsrg/UnitTests/Info_test.py
+-rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.1.0/libsrg/UnitTests/RolloverTest_filename.py
+-rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.1.0/libsrg/UnitTests/RolloverTest_logfile.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.1.0/libsrg/UnitTests/Sample.env
+-rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.1.0/libsrg/UnitTests/Sample.ini
+-rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.1.0/libsrg/UnitTests/Sample.json
+-rw-r--r--   0        0        0        0 2024-05-06 14:46:32.169025 libsrg-5.1.0/libsrg/UnitTests/__init__.py
+-rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.1.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
+-rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.1.0/libsrg/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-06 15:13:06.778118 libsrg-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.1.0/PKG-INFO
```

### Comparing `libsrg-5.0.0/LICENSE.txt` & `libsrg-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/README.md` & `libsrg-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/AppTemplate.py` & `libsrg-5.1.0/libsrg/AppTemplate.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Config.py` & `libsrg-5.1.0/libsrg/Config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import configparser
 import json
 import os
 import re
 from collections import ChainMap
 from pathlib import Path
-from typing import Any, Self, Optional, Tuple, TypeAlias
+from typing import Any, Optional, Tuple, Union
 
 from jinja2 import Template
 
-FileName: TypeAlias = str | bytes | os.PathLike
+# FileName: TypeAlias = str | bytes | os.PathLike
+FileName = Union[str, bytes, os.PathLike]
 """FileName can be a str, bytes or a pathlib.Path."""
 
-ConfigSource: TypeAlias = ChainMap[str, Any] | dict[str, Any] | FileName
+# ConfigSource: TypeAlias = ChainMap[str, Any] | dict[str, Any] | FileName
+ConfigSource = Union[ChainMap[str, Any], dict[str, Any], FileName]
 """ConfigSource can be a ChainMap, a dict, or a FileName as defined above."""
 
 
 class Config(ChainMap):
     """
     The Config class extends the ChainMap class to provide access to config files.
 
     From outside, a Config looks like a series of python dictionaries which get searched in
-    order for a given configuation item,
+    order for a given configuration item,
 
     Jinja argument processing can be applied on a per item basis using the get_item function,
     Jinja processing is NOT applied as files are read in from the config file. Other items in the config
     can be referenced in jinja templates.
 
     The Config class maintains one special Config instance which contains secrets. These can be usernames,
     passwords, api keys, or anything else that should not normally be kept in publicly accessible
     configuration files. One file of secrets can be read from a secure location and referenced by items
     in the normal config files.
 
     """
 
-    _secret_config: Self | None = None
+    _secret_config: Optional["Config"] = None
     """Holds a secret config instance for usernames, passwords, api keys, etc."""
 
     def __init__(self, *args: ConfigSource):
         """
         Constructs a new Config object.
         :param args: zero or more Config, ChainMap, dict[str, Any], Path
         """
         args2 = self.process_args(*args)
         super().__init__(*args2)
 
-    def apply_templates_to_strings(self, data: Any, config: Optional[Self] = None,
+    def apply_templates_to_strings(self, data: Any, config: Optional["Config"] = None,
                                    secrets: bool = False) -> Any:
         """
         apply templates to strings in data (applies to str or list of str, else return unchanged
           * if data is a str, apply templates
           * if data is a list containing ONLY str, apply recursively for one level only
           * anything else returns unmodified
         :param data: data to be processed
@@ -67,15 +69,15 @@
         if isinstance(data, list):
             # only apply to list of str, not list of Any
             if all([isinstance(x, str) for x in data]):
                 return [self.apply_templates_to_strings(x, config=config, secrets=False) for x in data]
         return data
 
     @classmethod
-    def config_to_list(cls, config: Self) -> list[tuple[str, Any, int]]:
+    def config_to_list(cls, config: "Config") -> list[tuple[str, Any, int]]:
         """Finds and alphabetizes all config items in config
         :param config: Config instance
         :return: Ordered list of tuples (name, value, depth)
         """
         names = list(config.keys())
         names.sort()
         lst = []
@@ -216,15 +218,15 @@
         if markers is None:
             markers = ("#", ";", "//")
         lines = text.split("\n")
         new_lines = [line for line in lines if not line.strip(" \t").startswith(markers)]
         return "\n".join(new_lines)
 
     @classmethod
-    def text_to_config(cls, text: str) -> Self:
+    def text_to_config(cls, text: str) -> "Config":
         """Create a Config instance from a string (see text_to_dict)."""
         return cls(cls.text_to_dict(text))
 
     @classmethod
     def text_to_dict(cls, text: str) -> dict[str, Any]:
         """
         Converts a string into a dict. Content type is determined using a few heuristics.
@@ -244,15 +246,15 @@
         ini_pat = re.compile(r"^\s*\[", re.MULTILINE)
         if ini_pat.match(text):
             cp = configparser.ConfigParser()
             cp.read_string(text)
             # reformat ini data as native dict of dicts
             out = {name: {k: v for k, v in cp[name].items()} for name in cp.sections()}
             return out
-        # fallback to flat env like file w/o [inisection]
+        # fallback to flat env like file w/o [ini_section]
         cp = configparser.ConfigParser()
         cp.read_string("[qqq]\n" + text)
         out = {k: v for k, v in cp["qqq"].items()}
         return out
 
     def to_flat_dict(self, ) -> dict[str, Any]:
         """
@@ -261,27 +263,38 @@
         """
         return dict(self)
 
     def to_json_file(self, file: FileName, **kwargs):
         """
         Produces a flat dict from a Config and converts to JSON file.
         :param file: str or Path instance
-        :param kwargs: keyword arguments pased to json.dump
+        :param kwargs: keyword arguments passed to "json.dumps"
         :return: None
         """
         txt = self.to_json_str(**kwargs)
         with open(file, 'w') as f:
             f.write(txt)
 
     def to_json_str(self, **kwargs) -> str:
         """
         Produces a flat dict from a Config and converts to JSON string.
-        :param kwargs: Keyword arguments pased to json.dump
+        :param kwargs: Keyword arguments passed to "json.dumps"
         :return: JSON string of Config
         """
         return json.dumps(self.to_flat_dict(), **kwargs)
 
     def to_list(self) -> list[tuple[str, Any, int]]:
         """Finds and alphabetizes all config items in config
         :return: Ordered list of tuples (name, value, depth)
         """
         return self.config_to_list(self)
+
+    def new_child(self, m=None, **kwargs)->"Config":      # like Django's Context.push()
+        """New Config with a new map followed by all previous maps.
+        If no map is provided, an empty dict is used.
+        Keyword arguments update the map or new empty dict.
+        """
+        if m is None:
+            m = kwargs
+        elif kwargs:
+            m.update(kwargs)
+        return Config(m, self)
```

### Comparing `libsrg-5.0.0/libsrg/ElapsedTime.py` & `libsrg-5.1.0/libsrg/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Info.py` & `libsrg-5.1.0/libsrg/Info.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import configparser
 import logging
 import os
 import platform
 import sys
 from importlib.metadata import version
 
+from libsrg.Config import Config
 from libsrg.LoggingCounter import LoggingCounter
 from libsrg.Runner import ElapsedTime
 from libsrg.Runner import Runner
 
 
 class Info:
     """
@@ -18,14 +19,15 @@
     * uname
     * hostname
     * host
     * /etc/os-release
 
     To work on a host other than localhost, ssh keys to the other host are required.
     """
+
     def __init__(self, hostname: str = None, timeout: int = 10, retries: int = 0):
         """
         All available information is fetched from the constructor.
         :param hostname: ssh to this remote host, localhost if None
         :param timeout: max time to wait on ssh calls
         :param retries: max number of retries before giving up
 
@@ -74,17 +76,18 @@
         """
         Internal function that fetches information from the remote host.
         :param timeout:
         :param retries:
         :return: None
         """
         # return
-        rh = Runner(f"host {self.hostname}")
-        if not rh.success:
-            raise Exception(f"Failed name lookup for host {self.hostname}")
+        if self.userat:
+            rh = Runner(f"host {self.hostname}")
+            if not rh.success:
+                raise Exception(f"Failed name lookup for remote host {self.hostname}")
 
         rm = Runner("uname -m", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.machine = rm.so_lines[-1]
 
         rk = Runner("uname -r", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.kernel = rk.so_lines[-1]
 
@@ -197,24 +200,44 @@
             if k not in ["logger", "config", "osrelease"]:
                 print(f"{k}={v}")
         if "osrelease" in self.__dict__ and self.__dict__["osrelease"]:
             for k, v in self.osrelease.items():
                 print(f"osrelease.{k}={v}")
         print("-----------------------------------------------")
 
+    def to_config(self, prefix: str = None) -> Config:
+        """
+        Load discovered info into a Config object.
+        :param prefix:  string top be prepended at the start of field names
+        """
+        config = Config()
+        if prefix is None:
+            prefix = ""
+        for k, v in self.__dict__.items():
+            if k not in ["logger", "config", "osrelease"]:
+                config.set_item(f"{prefix}{k.lower()}", v)
+
+        if "osrelease" in self.__dict__ and self.__dict__["osrelease"]:
+            for k, v in self.osrelease.items():
+                config.set_item(f"{prefix}osrelease.{k}", v)
+                config.set_item(f"{prefix}osrelease.{k.lower()}", v)
+        return config
+
 
 if __name__ == '__main__':
+    import pprint
+
     # info = Info("nas0")
     LoggingCounter.config_and_attach()
-    argv= sys.argv[1:]
+    argv = sys.argv[1:]
     if len(argv) == 0:
-        argv=["localhost"]
+        argv = ["localhost"]
     for arg in argv:
-        i=Info(arg)
-        i.dump()
+        i = Info(arg)
+        pprint.pp(i.to_config(arg + "__"))
     # for name in [None, "nas1", "web", "nowhere"]:
     #     logging.info(f"start {name}")
     #     t1 = ElapsedTime(f"Outer {name}")
     #     print(name, "*" * 80)
     #     with t1:
     #         info = Info(name)
     #     logging.info(f"returned {name} {info} {t1}")
```

### Comparing `libsrg-5.0.0/libsrg/LevelBanner.py` & `libsrg-5.1.0/libsrg/LevelBanner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/LoggerGUIProxy.py` & `libsrg-5.1.0/libsrg/LoggerGUIProxy.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/LoggingAppBase.py` & `libsrg-5.1.0/libsrg/LoggingAppBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/LoggingCounter.py` & `libsrg-5.1.0/libsrg/LoggingCounter.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/LoggingUtils.py` & `libsrg-5.1.0/libsrg/LoggingUtils.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/LoggingWatcher.py` & `libsrg-5.1.0/libsrg/LoggingWatcher.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/NagiosBase.py` & `libsrg-5.1.0/libsrg/NagiosBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Runner.py` & `libsrg-5.1.0/libsrg/Runner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Runner2.py` & `libsrg-5.1.0/libsrg/Runner2.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/ADStatsBase.py` & `libsrg-5.1.0/libsrg/Statistics/ADStatsBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from time import time
-from typing import Optional, Callable, Self, Any
+from typing import Optional, Callable, Any
 
 
 @dataclass
 class ADStatsRecord:
     name: str
     count: int
     time: float
@@ -85,15 +85,15 @@
         return self._name
 
     def count(self) -> int:
         return self._sample_count
 
     @classmethod
     def find_in_object(cls, obj: Any, tgt_class=None, nosort: bool = False,
-                       prop_name: str = "statistics_dict") -> list[Self]:
+                       prop_name: str = "statistics_dict") -> list["ADStatsBase"]:
         """
         Given obj, find all instances variables which are an instance of tgt_class
 
         Note that even though this classmethod is defined on the base class, it can be
         called on any subclass, and will (by default) find instances of that subclass
 
         If the obj has the property named  by prop_name, it will also be considered as s dictionary
@@ -114,15 +114,15 @@
                 for k, v in dct.items():
                     if isinstance(v, tgt_class):
                         stats.append(v)
         if not nosort:
             stats.sort()
         return stats
 
-    def __lt__(self, other: Self | None) -> bool:
+    def __lt__(self, other: Optional["ADStatsBase"]) -> bool:
         """Allow sorting by name"""
         return self._name < other._name
 
     def register_callback(self, callback: Callable):
         self.instance_callbacks.append(callback)
 
     def unregister_callback(self, callback: Callable):
```

### Comparing `libsrg-5.0.0/libsrg/Statistics/AnalogStatsBase.py` & `libsrg-5.1.0/libsrg/Statistics/AnalogStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/AnalogStatsCumulative.py` & `libsrg-5.1.0/libsrg/Statistics/AnalogStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/AnalogStatsFading.py` & `libsrg-5.1.0/libsrg/Statistics/AnalogStatsFading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import math
-from typing import Optional, Callable, Self
+from typing import Optional, Callable
 
 from libsrg.Statistics.AnalogStatsBase import AnalogStatsBase
 
 
 class AnalogStatsFading(AnalogStatsBase):
     """
     RunningStatistics class calculates running mean and standard deviation for data accumulated one sample at a time
     It also produces fading window statistics based on alpha/beta filtering the data.
     Normally beta will be set to (1-alpha) but if alpha and beta are set to one, the windowed statistics should
     match the non-fading.
 
 
     """
 
-    def __lt__(self, other: Self | None) -> bool:
+    def __lt__(self, other: "AnalogStatsFading") -> bool:
         """Allow sorting by name"""
         return self._name < other._name
 
     def __init__(self, name: str, callbacks: Optional[list[Callable]] = None, alpha: float = 0.99, beta: float = 0):
         super().__init__(name=name, callbacks=callbacks)
         self._alpha: float = alpha
         self._beta: float = beta if beta > 0 else 1 - self._alpha
```

### Comparing `libsrg-5.0.0/libsrg/Statistics/AnalogStatsSlidingWindow.py` & `libsrg-5.1.0/libsrg/Statistics/AnalogStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsBase.py` & `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsCumulative.py` & `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py` & `libsrg-5.1.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.1.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/GuiBase.py` & `libsrg-5.1.0/libsrg/TKGUI/GuiBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/GuiRequestQueue.py` & `libsrg-5.1.0/libsrg/TKGUI/GuiRequestQueue.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/LoggerGUI.py` & `libsrg-5.1.0/libsrg/TKGUI/LoggerGUI.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc` & `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc` & `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc` & `libsrg-5.1.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc` & `libsrg-5.1.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/UnitTests/Config_test.py` & `libsrg-5.1.0/libsrg/UnitTests/Config_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/UnitTests/RolloverTest_filename.py` & `libsrg-5.1.0/libsrg/UnitTests/RolloverTest_filename.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/UnitTests/RolloverTest_logfile.py` & `libsrg-5.1.0/libsrg/UnitTests/RolloverTest_logfile.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.1.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.0.0/pyproject.toml` & `libsrg-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg"
-version = "5.0.0"
+version = "5.1.0"
 description = "Utility lib logging, statistics, subprocesses"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `libsrg-5.0.0/PKG-INFO` & `libsrg-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 5.0.0
+Version: 5.1.0
 Summary: Utility lib logging, statistics, subprocesses
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

