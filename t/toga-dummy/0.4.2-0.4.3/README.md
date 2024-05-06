# Comparing `tmp/toga-dummy-0.4.2.tar.gz` & `tmp/toga_dummy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-dummy-0.4.2.tar", last modified: Tue Feb  6 05:53:57 2024, max compression
+gzip compressed data, was "toga_dummy-0.4.3.tar", last modified: Mon May  6 06:43:33 2024, max compression
```

## Comparing `toga-dummy-0.4.2.tar` & `toga_dummy-0.4.3.tar`

### file list

```diff
@@ -1,63 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.530665 toga-dummy-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-02-06 05:53:57.530665 toga-dummy-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:53:57.530665 toga-dummy-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.518665 toga-dummy-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.522665 toga-dummy-0.4.2/src/toga_dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.526665 toga-dummy-0.4.2/src/toga_dummy/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.526665 toga-dummy-0.4.2/src/toga_dummy/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37825 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/resources/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.530665 toga-dummy-0.4.2/src/toga_dummy/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-06 05:53:23.000000 toga-dummy-0.4.2/src/toga_dummy/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:57.530665 toga-dummy-0.4.2/src/toga_dummy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-06 05:53:57.000000 toga-dummy-0.4.2/src/toga_dummy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.404354 toga_dummy-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.408354 toga_dummy-0.4.3/src/toga_dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.408354 toga_dummy-0.4.3/src/toga_dummy/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.412354 toga_dummy-0.4.3/src/toga_dummy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/plugins/image_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.412354 toga_dummy-0.4.3/src/toga_dummy/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/sample.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37825 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/src/toga_dummy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/src/toga_dummy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/top_level.txt
```

### Comparing `toga-dummy-0.4.2/LICENSE` & `toga_dummy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/PKG-INFO` & `toga_dummy-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: toga-dummy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A dummy testing backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-dummy
 ==========
 
 An Dummy backend for the `Toga widget toolkit`_. This doesn't actually display
 anything; it exists purely as a testing environment.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
 
 For platform requirements, see the `testing platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/testing.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/testing.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-dummy-0.4.2/README.rst` & `toga_dummy-0.4.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 An Dummy backend for the `Toga widget toolkit`_. This doesn't actually display
 anything; it exists purely as a testing environment.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
 
 For platform requirements, see the `testing platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/testing.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/testing.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-dummy-0.4.2/pyproject.toml` & `toga_dummy-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools==69.0.0",
+    "setuptools==69.5.1",
     "setuptools_scm==8.0.4",
     "setuptools_dynamic_dependencies @ git+https://github.com/beeware/setuptools_dynamic_dependencies",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version", "dependencies"]
@@ -33,30 +33,36 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 [project.urls]
 Homepage = "https://beeware.org/project/projects/libraries/toga/"
 Funding = "https://beeware.org/contributing/membership/"
-Documentation = "https://toga.readthedocs.io/en/latest/"
+Documentation = "https://toga.readthedocs.io/"
 Tracker = "https://github.com/beeware/toga/issues"
 Source = "https://github.com/beeware/toga"
+Changelog = "https://toga.readthedocs.io/en/stable/background/project/releases.html"
 
 [project.entry-points."toga.backends"]
 dummy = "toga_dummy"
 
+[project.entry-points."toga.image_formats"]
+dummy = "toga_dummy.plugins.image_formats.CustomImageConverter"
+disabled = "toga_dummy.plugins.image_formats.DisabledImageConverter"
+
 [tool.setuptools_scm]
 root = ".."
 
 [tool.setuptools_dynamic_dependencies]
 dependencies = [
     "toga-core == {version}",
 ]
```

### Comparing `toga-dummy-0.4.2/src/toga_dummy/dialogs.py` & `toga_dummy-0.4.3/src/toga_dummy/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/factory.py` & `toga_dummy-0.4.3/src/toga_dummy/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from toga import NotImplementedWarning
+
 from . import dialogs
 from .app import App, DocumentApp, MainWindow
 from .command import Command
 from .documents import Document
 from .fonts import Font
 from .hardware.camera import Camera
+from .hardware.location import Location
 from .icons import Icon
 from .images import Image
 from .paths import Paths
 from .widgets.activityindicator import ActivityIndicator
 from .widgets.base import Widget
 from .widgets.box import Box
 from .widgets.button import Button
 from .widgets.canvas import Canvas
 from .widgets.dateinput import DateInput
 from .widgets.detailedlist import DetailedList
 from .widgets.divider import Divider
 from .widgets.imageview import ImageView
 from .widgets.label import Label
+from .widgets.mapview import MapView
 from .widgets.multilinetextinput import MultilineTextInput
 from .widgets.numberinput import NumberInput
 from .widgets.optioncontainer import OptionContainer
 from .widgets.passwordinput import PasswordInput
 from .widgets.progressbar import ProgressBar
 from .widgets.scrollcontainer import ScrollContainer
 from .widgets.selection import Selection
@@ -32,15 +36,15 @@
 from .widgets.timeinput import TimeInput
 from .widgets.tree import Tree
 from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    raise NotImplementedError()
+    NotImplementedWarning.warn("Dummy", feature)
 
 
 __all__ = [
     "not_implemented",
     "App",
     "DocumentApp",
     "MainWindow",
@@ -49,24 +53,26 @@
     "Font",
     "Icon",
     "Image",
     "Paths",
     "dialogs",
     # Hardware
     "Camera",
+    "Location",
     # Widgets
     "ActivityIndicator",
     "Box",
     "Button",
     "Canvas",
     "DateInput",
     "DetailedList",
     "Divider",
     "ImageView",
     "Label",
+    "MapView",
     "MultilineTextInput",
     "NumberInput",
     "OptionContainer",
     "PasswordInput",
     "ProgressBar",
     "ScrollContainer",
     "Selection",
```

### Comparing `toga-dummy-0.4.2/src/toga_dummy/fonts.py` & `toga_dummy-0.4.3/src/toga_dummy/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/hardware/camera.py` & `toga_dummy-0.4.3/src/toga_dummy/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/images.py` & `toga_dummy-0.4.3/src/toga_dummy/images.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/resources/screenshot.png` & `toga_dummy-0.4.3/src/toga_dummy/resources/screenshot.png`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/resources/toga.png` & `toga_dummy-0.4.3/src/toga_dummy/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/utils.py` & `toga_dummy-0.4.3/src/toga_dummy/utils.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/base.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/canvas.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/dateinput.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/detailedlist.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/multilinetextinput.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/numberinput.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/optioncontainer.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/progressbar.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/scrollcontainer.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/selection.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/slider.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/splitcontainer.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/switch.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/table.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/textinput.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/timeinput.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/tree.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/widgets/webview.py` & `toga_dummy-0.4.3/src/toga_dummy/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga-dummy-0.4.2/src/toga_dummy/window.py` & `toga_dummy-0.4.3/src/toga_dummy/window.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 import toga_dummy
 
+from .screens import Screen as ScreenImpl
 from .utils import LoggedObject
 
 
 class Container:
     def __init__(self, content=None):
         self.baseline_dpi = 96
         self.dpi = 96
@@ -101,7 +102,11 @@
         return path.read_bytes()
 
     def set_full_screen(self, is_full_screen):
         self._action("set full screen", full_screen=is_full_screen)
 
     def simulate_close(self):
         self.interface.on_close()
+
+    def get_current_screen(self):
+        # `window.screen` will return `Secondary Screen`
+        return ScreenImpl(native=("Secondary Screen", (-1366, -768), (1366, 768)))
```

### Comparing `toga-dummy-0.4.2/src/toga_dummy.egg-info/PKG-INFO` & `toga_dummy-0.4.3/src/toga_dummy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: toga-dummy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A dummy testing backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-dummy
 ==========
 
 An Dummy backend for the `Toga widget toolkit`_. This doesn't actually display
 anything; it exists purely as a testing environment.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
 
 For platform requirements, see the `testing platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/testing.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/testing.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-dummy-0.4.2/src/toga_dummy.egg-info/SOURCES.txt` & `toga_dummy-0.4.3/src/toga_dummy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,44 @@
 src/toga_dummy/dialogs.py
 src/toga_dummy/documents.py
 src/toga_dummy/factory.py
 src/toga_dummy/fonts.py
 src/toga_dummy/icons.py
 src/toga_dummy/images.py
 src/toga_dummy/paths.py
+src/toga_dummy/screens.py
 src/toga_dummy/utils.py
 src/toga_dummy/window.py
 src/toga_dummy.egg-info/PKG-INFO
 src/toga_dummy.egg-info/SOURCES.txt
 src/toga_dummy.egg-info/dependency_links.txt
 src/toga_dummy.egg-info/entry_points.txt
 src/toga_dummy.egg-info/requires.txt
 src/toga_dummy.egg-info/top_level.txt
 src/toga_dummy/hardware/__init__.py
 src/toga_dummy/hardware/camera.py
+src/toga_dummy/hardware/location.py
+src/toga_dummy/plugins/__init__.py
+src/toga_dummy/plugins/image_formats.py
 src/toga_dummy/resources/__init__.py
+src/toga_dummy/resources/sample.png
 src/toga_dummy/resources/screenshot.png
 src/toga_dummy/resources/toga.png
 src/toga_dummy/widgets/__init__.py
 src/toga_dummy/widgets/activityindicator.py
 src/toga_dummy/widgets/base.py
 src/toga_dummy/widgets/box.py
 src/toga_dummy/widgets/button.py
 src/toga_dummy/widgets/canvas.py
 src/toga_dummy/widgets/dateinput.py
 src/toga_dummy/widgets/detailedlist.py
 src/toga_dummy/widgets/divider.py
 src/toga_dummy/widgets/imageview.py
 src/toga_dummy/widgets/label.py
+src/toga_dummy/widgets/mapview.py
 src/toga_dummy/widgets/multilinetextinput.py
 src/toga_dummy/widgets/numberinput.py
 src/toga_dummy/widgets/optioncontainer.py
 src/toga_dummy/widgets/passwordinput.py
 src/toga_dummy/widgets/progressbar.py
 src/toga_dummy/widgets/scrollcontainer.py
 src/toga_dummy/widgets/selection.py
```

