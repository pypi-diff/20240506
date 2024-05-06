# Comparing `tmp/jetson-stats-4.2.7.tar.gz` & `tmp/jetson-stats-4.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson-stats-4.2.7.tar", last modified: Mon Mar 18 10:47:57 2024, max compression
+gzip compressed data, was "jetson-stats-4.2.8.tar", last modified: Mon May  6 19:08:21 2024, max compression
```

## Comparing `jetson-stats-4.2.7.tar` & `jetson-stats-4.2.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/
--rw-r--r--   0 root         (0) root         (0)     5210 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)    34522 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1195 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7240 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5013 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.635470 jetson-stats-4.2.7/jetson_stats.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7240 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1391 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-18 10:47:57.000000 jetson-stats-4.2.7/jetson_stats.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.635470 jetson-stats-4.2.7/jtop/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7442 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/jtop/core/
--rw-r--r--   0 root         (0) root         (0)      857 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/command.py
--rw-r--r--   0 root         (0) root         (0)     8186 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/common.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/config.py
--rw-r--r--   0 root         (0) root         (0)    10295 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5202 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/engine.py
--rw-r--r--   0 root         (0) root         (0)     1273 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    26135 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/fan.py
--rw-r--r--   0 root         (0) root         (0)    13306 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/gpu.py
--rw-r--r--   0 root         (0) root         (0)     3248 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/hardware.py
--rw-r--r--   0 root         (0) root         (0)    21131 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/jetson_clocks.py
--rw-r--r--   0 root         (0) root         (0)     5116 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/jetson_libraries.py
--rw-r--r--   0 root         (0) root         (0)    16315 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/jetson_variables.py
--rw-r--r--   0 root         (0) root         (0)    17572 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/memory.py
--rw-r--r--   0 root         (0) root         (0)    19721 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/nvpmodel.py
--rw-r--r--   0 root         (0) root         (0)    13576 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/power.py
--rw-r--r--   0 root         (0) root         (0)     5405 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/processes.py
--rw-r--r--   0 root         (0) root         (0)     7997 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/tegra_parse.py
--rw-r--r--   0 root         (0) root         (0)     4476 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/tegrastats.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/temperature.py
--rw-r--r--   0 root         (0) root         (0)     3173 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/core/timer_reader.py
--rw-r--r--   0 root         (0) root         (0)     6862 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/jtop/gui/
--rw-r--r--   0 root         (0) root         (0)     1111 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12426 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/jtopgui.py
--rw-r--r--   0 root         (0) root         (0)     9679 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/jtopguiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/jtop/gui/lib/
--rw-r--r--   0 root         (0) root         (0)      850 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11124 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/chart.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/colors.py
--rw-r--r--   0 root         (0) root         (0)     5806 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/common.py
--rw-r--r--   0 root         (0) root         (0)     6148 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/linear_gauge.py
--rw-r--r--   0 root         (0) root         (0)     3701 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/process_table.py
--rw-r--r--   0 root         (0) root         (0)     6182 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/lib/smallbutton.py
--rw-r--r--   0 root         (0) root         (0)     8976 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pall.py
--rw-r--r--   0 root         (0) root         (0)    19822 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pcontrol.py
--rw-r--r--   0 root         (0) root         (0)     5662 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pcpu.py
--rw-r--r--   0 root         (0) root         (0)     6481 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pengine.py
--rw-r--r--   0 root         (0) root         (0)    10067 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pgpu.py
--rw-r--r--   0 root         (0) root         (0)     5946 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pinfo.py
--rw-r--r--   0 root         (0) root         (0)    17935 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/gui/pmem.py
--rw-r--r--   0 root         (0) root         (0)     9788 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/jetson_config.py
--rw-r--r--   0 root         (0) root         (0)     6001 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/jetson_release.py
--rw-r--r--   0 root         (0) root         (0)     3547 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/jetson_swap.py
--rw-r--r--   0 root         (0) root         (0)    58685 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/jtop.py
--rw-r--r--   0 root         (0) root         (0)    25463 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/service.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/jtop/terminal_colors.py
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/scripts/
--rw-r--r--   0 root         (0) root         (0)     1563 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/scripts/jtop_env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/services/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/services/jtop.service
--rw-r--r--   0 root         (0) root         (0)       89 2024-03-18 10:47:57.639469 jetson-stats-4.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11340 2024-03-18 10:47:50.000000 jetson-stats-4.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/
+-rw-r--r--   0 root         (0) root         (0)     5210 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)    34522 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7240 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5013 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.398952 jetson-stats-4.2.8/jetson_stats.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7240 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-06 19:08:21.000000 jetson-stats-4.2.8/jetson_stats.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.402952 jetson-stats-4.2.8/jtop/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/jtop/core/
+-rw-r--r--   0 root         (0) root         (0)      857 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/command.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/common.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    10295 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/engine.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    26135 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/fan.py
+-rw-r--r--   0 root         (0) root         (0)    13306 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/hardware.py
+-rw-r--r--   0 root         (0) root         (0)    21131 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/jetson_clocks.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/jetson_libraries.py
+-rw-r--r--   0 root         (0) root         (0)    16336 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/jetson_variables.py
+-rw-r--r--   0 root         (0) root         (0)    17572 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/memory.py
+-rw-r--r--   0 root         (0) root         (0)    19721 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/nvpmodel.py
+-rw-r--r--   0 root         (0) root         (0)    13576 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/power.py
+-rw-r--r--   0 root         (0) root         (0)     5405 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/processes.py
+-rw-r--r--   0 root         (0) root         (0)     7997 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/tegra_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/tegrastats.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/temperature.py
+-rw-r--r--   0 root         (0) root         (0)     3173 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/core/timer_reader.py
+-rw-r--r--   0 root         (0) root         (0)     6862 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/jtop/gui/
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12426 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/jtopgui.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/jtopguiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/jtop/gui/lib/
+-rw-r--r--   0 root         (0) root         (0)      850 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/chart.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/colors.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/common.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/linear_gauge.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/process_table.py
+-rw-r--r--   0 root         (0) root         (0)     6182 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/lib/smallbutton.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pall.py
+-rw-r--r--   0 root         (0) root         (0)    19822 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pcontrol.py
+-rw-r--r--   0 root         (0) root         (0)     5662 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pcpu.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pengine.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pgpu.py
+-rw-r--r--   0 root         (0) root         (0)     5946 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pinfo.py
+-rw-r--r--   0 root         (0) root         (0)    17935 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/gui/pmem.py
+-rw-r--r--   0 root         (0) root         (0)     9788 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/jetson_config.py
+-rw-r--r--   0 root         (0) root         (0)     6001 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/jetson_release.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/jetson_swap.py
+-rw-r--r--   0 root         (0) root         (0)    58685 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/jtop.py
+-rw-r--r--   0 root         (0) root         (0)    25463 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/service.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/jtop/terminal_colors.py
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/scripts/
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/scripts/jtop_env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/services/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/services/jtop.service
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-06 19:08:21.406952 jetson-stats-4.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    11340 2024-05-06 19:08:16.000000 jetson-stats-4.2.8/setup.py
```

### Comparing `jetson-stats-4.2.7/CODE_OF_CONDUCT.md` & `jetson-stats-4.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/LICENSE` & `jetson-stats-4.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/MANIFEST.in` & `jetson-stats-4.2.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/PKG-INFO` & `jetson-stats-4.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-stats
-Version: 4.2.7
+Version: 4.2.8
 Summary: Interactive system-monitor and process viewer for all NVIDIA Jetson [Orin, Xavier, Nano, TX] series
 Home-page: https://rnext.it/jetson_stats
 Author: Raffaello Bonghi
 Author-email: raffaello@rnext.it
 License: AGPL-3.0
 Project-URL: Documentation, https://rnext.it/jetson_stats
 Project-URL: Funding, https://github.com/sponsors/rbonghi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jetson-stats Version: 4.2.7 Summary: Interactive
+Metadata-Version: 2.1 Name: jetson-stats Version: 4.2.8 Summary: Interactive
 system-monitor and process viewer for all NVIDIA Jetson [Orin, Xavier, Nano,
 TX] series Home-page: https://rnext.it/jetson_stats Author: Raffaello Bonghi
 Author-email: raffaello@rnext.it License: AGPL-3.0 Project-URL: Documentation,
 https://rnext.it/jetson_stats Project-URL: Funding, https://github.com/
 sponsors/rbonghi Project-URL: Say Thanks!, https://discord.gg/BFbuJNhYzS
 Project-URL: Source, https://github.com/rbonghi/jetson_stats Project-URL:
 Tracker, https://github.com/rbonghi/jetson_stats/issues Project-URL: Examples,
```

### Comparing `jetson-stats-4.2.7/README.md` & `jetson-stats-4.2.8/README.md`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jetson_stats.egg-info/PKG-INFO` & `jetson-stats-4.2.8/jetson_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-stats
-Version: 4.2.7
+Version: 4.2.8
 Summary: Interactive system-monitor and process viewer for all NVIDIA Jetson [Orin, Xavier, Nano, TX] series
 Home-page: https://rnext.it/jetson_stats
 Author: Raffaello Bonghi
 Author-email: raffaello@rnext.it
 License: AGPL-3.0
 Project-URL: Documentation, https://rnext.it/jetson_stats
 Project-URL: Funding, https://github.com/sponsors/rbonghi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jetson-stats Version: 4.2.7 Summary: Interactive
+Metadata-Version: 2.1 Name: jetson-stats Version: 4.2.8 Summary: Interactive
 system-monitor and process viewer for all NVIDIA Jetson [Orin, Xavier, Nano,
 TX] series Home-page: https://rnext.it/jetson_stats Author: Raffaello Bonghi
 Author-email: raffaello@rnext.it License: AGPL-3.0 Project-URL: Documentation,
 https://rnext.it/jetson_stats Project-URL: Funding, https://github.com/
 sponsors/rbonghi Project-URL: Say Thanks!, https://discord.gg/BFbuJNhYzS
 Project-URL: Source, https://github.com/rbonghi/jetson_stats Project-URL:
 Tracker, https://github.com/rbonghi/jetson_stats/issues Project-URL: Examples,
```

### Comparing `jetson-stats-4.2.7/jetson_stats.egg-info/SOURCES.txt` & `jetson-stats-4.2.8/jetson_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/__init__.py` & `jetson-stats-4.2.8/jtop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 __author__ = "Raffaello Bonghi"
 __email__ = "raffaello@rnext.it"
 __cr__ = "(c) 2024, RB"
 __copyright__ = "(c) 2024, Raffaello Bonghi"
 # Version package
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#choosing-a-versioning-scheme
-__version__ = "4.2.7"
+__version__ = "4.2.8"
 # EOF
```

### Comparing `jetson-stats-4.2.7/jtop/__main__.py` & `jetson-stats-4.2.8/jtop/__main__.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/__init__.py` & `jetson-stats-4.2.8/jtop/core/__init__.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/command.py` & `jetson-stats-4.2.8/jtop/core/command.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/common.py` & `jetson-stats-4.2.8/jtop/core/common.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/config.py` & `jetson-stats-4.2.8/jtop/core/config.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/cpu.py` & `jetson-stats-4.2.8/jtop/core/cpu.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/engine.py` & `jetson-stats-4.2.8/jtop/core/engine.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/exceptions.py` & `jetson-stats-4.2.8/jtop/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/fan.py` & `jetson-stats-4.2.8/jtop/core/fan.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/gpu.py` & `jetson-stats-4.2.8/jtop/core/gpu.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/hardware.py` & `jetson-stats-4.2.8/jtop/core/hardware.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/jetson_clocks.py` & `jetson-stats-4.2.8/jtop/core/jetson_clocks.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/jetson_libraries.py` & `jetson-stats-4.2.8/jtop/core/jetson_libraries.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/jetson_variables.py` & `jetson-stats-4.2.8/jtop/core/jetson_variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # ---------------------
 # JETPACK DETECTION
 # ---------------------
 # Write version of jetpack installed
 # https://developer.nvidia.com/embedded/jetpack-archive
 NVIDIA_JETPACK = {
     # -------- JP6 --------
+    "36.3.0": "6.0",
     "36.2.0": "6.0 DP",
     "36.0.0": "6.0 EA",
     # -------- JP5 --------
     "35.5.0": "5.1.3",
     "35.4.1": "5.1.2",
     "35.3.1": "5.1.1",
     "35.3.0": "5.1.1 PRE",
```

### Comparing `jetson-stats-4.2.7/jtop/core/memory.py` & `jetson-stats-4.2.8/jtop/core/memory.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/nvpmodel.py` & `jetson-stats-4.2.8/jtop/core/nvpmodel.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/power.py` & `jetson-stats-4.2.8/jtop/core/power.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/processes.py` & `jetson-stats-4.2.8/jtop/core/processes.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/tegra_parse.py` & `jetson-stats-4.2.8/jtop/core/tegra_parse.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/tegrastats.py` & `jetson-stats-4.2.8/jtop/core/tegrastats.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/temperature.py` & `jetson-stats-4.2.8/jtop/core/temperature.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/core/timer_reader.py` & `jetson-stats-4.2.8/jtop/core/timer_reader.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/github.py` & `jetson-stats-4.2.8/jtop/github.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/__init__.py` & `jetson-stats-4.2.8/jtop/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/jtopgui.py` & `jetson-stats-4.2.8/jtop/gui/jtopgui.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/jtopguiconfig.py` & `jetson-stats-4.2.8/jtop/gui/jtopguiconfig.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/__init__.py` & `jetson-stats-4.2.8/jtop/gui/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/chart.py` & `jetson-stats-4.2.8/jtop/gui/lib/chart.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/colors.py` & `jetson-stats-4.2.8/jtop/gui/lib/colors.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/common.py` & `jetson-stats-4.2.8/jtop/gui/lib/common.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/linear_gauge.py` & `jetson-stats-4.2.8/jtop/gui/lib/linear_gauge.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/process_table.py` & `jetson-stats-4.2.8/jtop/gui/lib/process_table.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/lib/smallbutton.py` & `jetson-stats-4.2.8/jtop/gui/lib/smallbutton.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pall.py` & `jetson-stats-4.2.8/jtop/gui/pall.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pcontrol.py` & `jetson-stats-4.2.8/jtop/gui/pcontrol.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pcpu.py` & `jetson-stats-4.2.8/jtop/gui/pcpu.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pengine.py` & `jetson-stats-4.2.8/jtop/gui/pengine.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pgpu.py` & `jetson-stats-4.2.8/jtop/gui/pgpu.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pinfo.py` & `jetson-stats-4.2.8/jtop/gui/pinfo.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/gui/pmem.py` & `jetson-stats-4.2.8/jtop/gui/pmem.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/jetson_config.py` & `jetson-stats-4.2.8/jtop/jetson_config.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/jetson_release.py` & `jetson-stats-4.2.8/jtop/jetson_release.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/jetson_swap.py` & `jetson-stats-4.2.8/jtop/jetson_swap.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/jtop.py` & `jetson-stats-4.2.8/jtop/jtop.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/service.py` & `jetson-stats-4.2.8/jtop/service.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/jtop/terminal_colors.py` & `jetson-stats-4.2.8/jtop/terminal_colors.py`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/scripts/jtop_env.sh` & `jetson-stats-4.2.8/scripts/jtop_env.sh`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/services/jtop.service` & `jetson-stats-4.2.8/services/jtop.service`

 * *Files identical despite different names*

### Comparing `jetson-stats-4.2.7/setup.py` & `jetson-stats-4.2.8/setup.py`

 * *Files identical despite different names*

