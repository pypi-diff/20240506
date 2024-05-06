# Comparing `tmp/toga-cocoa-0.4.2.tar.gz` & `tmp/toga_cocoa-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-cocoa-0.4.2.tar", last modified: Tue Feb  6 05:54:02 2024, max compression
+gzip compressed data, was "toga_cocoa-0.4.3.tar", last modified: Mon May  6 06:43:37 2024, max compression
```

## Comparing `toga-cocoa-0.4.2.tar` & `toga_cocoa-0.4.3.tar`

### file list

```diff
@@ -1,112 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.565874 toga-cocoa-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-06 05:54:02.565874 toga-cocoa-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:54:02.565874 toga-cocoa-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.545874 toga-cocoa-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.549874 toga-cocoa-0.4.2/src/toga_cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17968 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.553874 toga-cocoa-0.4.2/src/toga_cocoa/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.553874 toga-cocoa-0.4.2/src/toga_cocoa/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/appkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/av_foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/core_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/libs/webkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.553874 toga-cocoa-0.4.2/src/toga_cocoa/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/resources/camera.png
--rw-r--r--   0 runner    (1001) docker     (127)   396417 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/resources/toga.icns
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.557874 toga-cocoa-0.4.2/src/toga_cocoa/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/imageview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.561874 toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/src/toga_cocoa/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.565874 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-06 05:54:02.000000 toga-cocoa-0.4.2/src/toga_cocoa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.561874 toga-cocoa-0.4.2/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.561874 toga-cocoa-0.4.2/tests_backend/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:02.565874 toga-cocoa-0.4.2/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-02-06 05:53:25.000000 toga-cocoa-0.4.2/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.805608 toga_cocoa-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.809608 toga_cocoa-0.4.3/src/toga_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/appkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/av_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/mapkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/resources/camera.png
+-rw-r--r--   0 runner    (1001) docker     (127)   396417 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/resources/toga.icns
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.817608 toga_cocoa-0.4.3/src/toga_cocoa/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/tests_backend/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/window.py
```

### Comparing `toga-cocoa-0.4.2/LICENSE` & `toga_cocoa-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/PKG-INFO` & `toga_cocoa-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: toga-cocoa
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Cocoa (macOS) backend for the Toga widget toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,macOS,cocoa
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
 Requires-Dist: fonttools<5.0.0,>=4.42.1
 Requires-Dist: rubicon-objc<0.5.0,>=0.4.7
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-cocoa
 ==========
 
 A Cocoa backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `macOS platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/macOS.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/macOS.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-cocoa-0.4.2/README.rst` & `toga_cocoa-0.4.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========
 
 A Cocoa backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `macOS platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/macOS.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/macOS.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-cocoa-0.4.2/pyproject.toml` & `toga_cocoa-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

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
@@ -35,26 +35,28 @@
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
 macOS = "toga_cocoa"
 
 [tool.setuptools_scm]
 root = ".."
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/app.py` & `toga_cocoa-0.4.3/src/toga_cocoa/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     NSObject,
     NSOpenPanel,
     NSScreen,
     NSString,
     objc_method,
     objc_property,
 )
+from .screens import Screen as ScreenImpl
 from .window import Window
 
 
 class MainWindow(Window):
     def cocoa_windowShouldClose(self):
         # Main Window close is a proxy for "Exit app".
         # Defer all handling to the app's on_exit handler.
@@ -56,14 +57,20 @@
     impl = objc_property(object, weak=True)
 
     @objc_method
     def applicationDidFinishLaunching_(self, notification):
         self.native.activateIgnoringOtherApps(True)
 
     @objc_method
+    def applicationSupportsSecureRestorableState_(
+        self, app
+    ) -> bool:  # pragma: no cover
+        return True
+
+    @objc_method
     def applicationOpenUntitledFile_(self, sender) -> bool:  # pragma: no cover
         self.impl.select_file()
         return True
 
     @objc_method
     def addDocument_(self, document) -> None:  # pragma: no cover
         # print("Add Document", document)
@@ -124,38 +131,68 @@
         # Stimulate the build of the app
         self.create()
 
     def create(self):
         self.native = NSApplication.sharedApplication
         self.native.setActivationPolicy(NSApplicationActivationPolicyRegular)
 
-        self.native.setApplicationIconImage_(self.interface.icon._impl.native)
+        # The app icon been set *before* the app instance is created. However, we only
+        # need to set the icon on the app if it has been explicitly defined; the default
+        # icon is... the default. We can't test this branch in the testbed.
+        if self.interface.icon._impl.path:
+            self.set_icon(self.interface.icon)  # pragma: no cover
 
         self.resource_path = os.path.dirname(
             os.path.dirname(NSBundle.mainBundle.bundlePath)
         )
 
         self.appDelegate = AppDelegate.alloc().init()
         self.appDelegate.impl = self
         self.appDelegate.interface = self.interface
         self.appDelegate.native = self.native
         self.native.setDelegate_(self.appDelegate)
 
-        self._create_app_commands()
+        self.create_app_commands()
 
         # Call user code to populate the main window
         self.interface._startup()
 
         # Create the lookup table of menu items,
         # then force the creation of the menus.
         self._menu_groups = {}
         self._menu_items = {}
         self.create_menus()
 
-    def _create_app_commands(self):
+    ######################################################################
+    # Commands and menus
+    ######################################################################
+
+    def _menu_about(self, command, **kwargs):
+        self.interface.about()
+
+    def _menu_close_all_windows(self, command, **kwargs):
+        # Convert to a list to so that we're not altering a set while iterating
+        for window in list(self.interface.windows):
+            window._impl.native.performClose(None)
+
+    def _menu_close_window(self, command, **kwargs):
+        if self.interface.current_window:
+            self.interface.current_window._impl.native.performClose(None)
+
+    def _menu_minimize(self, command, **kwargs):
+        if self.interface.current_window:
+            self.interface.current_window._impl.native.miniaturize(None)
+
+    def _menu_quit(self, command, **kwargs):
+        self.interface.on_exit()
+
+    def _menu_visit_homepage(self, command, **kwargs):
+        self.interface.visit_homepage()
+
+    def create_app_commands(self):
         formal_name = self.interface.formal_name
         self.interface.commands.add(
             # ---- App menu -----------------------------------
             toga.Command(
                 self._menu_about,
                 "About " + formal_name,
                 group=toga.Group.APP,
@@ -294,35 +331,39 @@
                 self._menu_visit_homepage,
                 "Visit homepage",
                 enabled=self.interface.home_page is not None,
                 group=toga.Group.HELP,
             ),
         )
 
-    def _menu_about(self, command, **kwargs):
-        self.interface.about()
-
-    def _menu_quit(self, command, **kwargs):
-        self.interface.on_exit()
-
-    def _menu_close_window(self, command, **kwargs):
-        if self.interface.current_window:
-            self.interface.current_window._impl.native.performClose(None)
+    def _submenu(self, group, menubar):
+        """Obtain the submenu representing the command group.
 
-    def _menu_close_all_windows(self, command, **kwargs):
-        # Convert to a list to so that we're not altering a set while iterating
-        for window in list(self.interface.windows):
-            window._impl.native.performClose(None)
+        This will create the submenu if it doesn't exist. It will call itself
+        recursively to build the full path to menus inside submenus, returning the
+        "leaf" node in the submenu path. Once created, it caches the menu that has been
+        created for future lookup.
+        """
+        try:
+            return self._menu_groups[group]
+        except KeyError:
+            if group is None:
+                submenu = menubar
+            else:
+                parent_menu = self._submenu(group.parent, menubar)
 
-    def _menu_minimize(self, command, **kwargs):
-        if self.interface.current_window:
-            self.interface.current_window._impl.native.miniaturize(None)
+                menu_item = parent_menu.addItemWithTitle(
+                    group.text, action=None, keyEquivalent=""
+                )
+                submenu = NSMenu.alloc().initWithTitle(group.text)
+                parent_menu.setSubmenu(submenu, forItem=menu_item)
 
-    def _menu_visit_homepage(self, command, **kwargs):
-        self.interface.visit_homepage()
+            # Install the item in the group cache.
+            self._menu_groups[group] = submenu
+            return submenu
 
     def create_menus(self):
         # Recreate the menu.
         # Remove any native references to the existing menu
         for menu_item, cmd in self._menu_items.items():
             cmd._impl.native.remove(menu_item)
 
@@ -369,46 +410,55 @@
 
                 self._menu_items[item] = cmd
                 submenu.addItem(item)
 
         # Set the menu for the app.
         self.native.mainMenu = menubar
 
-    def _submenu(self, group, menubar):
-        """Obtain the submenu representing the command group.
+    ######################################################################
+    # App lifecycle
+    ######################################################################
 
-        This will create the submenu if it doesn't exist. It will call itself
-        recursively to build the full path to menus inside submenus, returning the
-        "leaf" node in the submenu path. Once created, it caches the menu that has been
-        created for future lookup.
-        """
-        try:
-            return self._menu_groups[group]
-        except KeyError:
-            if group is None:
-                submenu = menubar
-            else:
-                parent_menu = self._submenu(group.parent, menubar)
-
-                menu_item = parent_menu.addItemWithTitle(
-                    group.text, action=None, keyEquivalent=""
-                )
-                submenu = NSMenu.alloc().initWithTitle(group.text)
-                parent_menu.setSubmenu(submenu, forItem=menu_item)
-
-            # Install the item in the group cache.
-            self._menu_groups[group] = submenu
-            return submenu
+    # We can't call this under test conditions, because it would kill the test harness
+    def exit(self):  # pragma: no cover
+        self.loop.stop()
 
     def main_loop(self):
         self.loop.run_forever(lifecycle=CocoaLifecycle(self.native))
 
+    def set_icon(self, icon):
+        # If the icon is a path, it's an explicit icon; otherwise its the default icon
+        if icon._impl.path:
+            self.native.setApplicationIconImage(icon._impl.native)
+        else:
+            self.native.setApplicationIconImage(None)
+
     def set_main_window(self, window):
         pass
 
+    ######################################################################
+    # App resources
+    ######################################################################
+
+    def get_screens(self):
+        return [ScreenImpl(native=screen) for screen in NSScreen.screens]
+
+    ######################################################################
+    # App capabilities
+    ######################################################################
+
+    def beep(self):
+        NSBeep()
+
+    def open_document(self, fileURL):
+        """No-op when the app is not a ``DocumentApp``."""
+
+    def select_file(self, **kwargs):
+        """No-op when the app is not a ``DocumentApp``."""
+
     def show_about_dialog(self):
         options = NSMutableDictionary.alloc().init()
 
         options[NSAboutPanelOptionApplicationIcon] = self.interface.icon._impl.native
         options[NSAboutPanelOptionApplicationName] = self.interface.formal_name
 
         if self.interface.version is None:
@@ -422,27 +472,44 @@
         if self.interface.author is None:
             options["Copyright"] = ""
         else:
             options["Copyright"] = f"Copyright © {self.interface.author}"
 
         self.native.orderFrontStandardAboutPanelWithOptions(options)
 
-    def beep(self):
-        NSBeep()
+    ######################################################################
+    # Cursor control
+    ######################################################################
 
-    # We can't call this under test conditions, because it would kill the test harness
-    def exit(self):  # pragma: no cover
-        self.loop.stop()
+    def hide_cursor(self):
+        if self._cursor_visible:
+            NSCursor.hide()
+
+        self._cursor_visible = False
+
+    def show_cursor(self):
+        if not self._cursor_visible:
+            NSCursor.unhide()
+
+        self._cursor_visible = True
+
+    ######################################################################
+    # Window control
+    ######################################################################
 
     def get_current_window(self):
         return self.native.keyWindow
 
     def set_current_window(self, window):
         window._impl.native.makeKeyAndOrderFront(window._impl.native)
 
+    ######################################################################
+    # Full screen control
+    ######################################################################
+
     def enter_full_screen(self, windows):
         opts = NSMutableDictionary.alloc().init()
         opts.setObject(
             NSNumber.numberWithBool(True), forKey="NSFullScreenModeAllScreens"
         )
 
         for window, screen in zip(windows, NSScreen.screens):
@@ -460,36 +527,18 @@
             NSNumber.numberWithBool(True), forKey="NSFullScreenModeAllScreens"
         )
 
         for window in windows:
             window.content._impl.native.exitFullScreenModeWithOptions(opts)
             window.content.refresh()
 
-    def show_cursor(self):
-        if not self._cursor_visible:
-            NSCursor.unhide()
-
-        self._cursor_visible = True
-
-    def hide_cursor(self):
-        if self._cursor_visible:
-            NSCursor.hide()
-
-        self._cursor_visible = False
-
-    def open_document(self, fileURL):
-        """No-op when the app is not a ``DocumentApp``."""
-
-    def select_file(self, **kwargs):
-        """No-op when the app is not a ``DocumentApp``."""
-
 
 class DocumentApp(App):  # pragma: no cover
-    def _create_app_commands(self):
-        super()._create_app_commands()
+    def create_app_commands(self):
+        super().create_app_commands()
         self.interface.commands.add(
             toga.Command(
                 self._menu_open_file,
                 text="Open\u2026",
                 shortcut=toga.Key.MOD_1 + "o",
                 group=toga.Group.FILE,
                 section=0,
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/command.py` & `toga_cocoa-0.4.3/src/toga_cocoa/command.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/constraints.py` & `toga_cocoa-0.4.3/src/toga_cocoa/constraints.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/container.py` & `toga_cocoa-0.4.3/src/toga_cocoa/container.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/dialogs.py` & `toga_cocoa-0.4.3/src/toga_cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/documents.py` & `toga_cocoa-0.4.3/src/toga_cocoa/documents.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/factory.py` & `toga_cocoa-0.4.3/src/toga_cocoa/factory.py`

 * *Files 2% similar despite different names*

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
 
 # Widgets
 from .widgets.activityindicator import ActivityIndicator
 from .widgets.box import Box
 from .widgets.button import Button
 from .widgets.canvas import Canvas
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
@@ -31,15 +35,15 @@
 from .widgets.textinput import TextInput
 from .widgets.tree import Tree
 from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    print(f"[Cocoa] Not implemented: {feature}")  # pragma: nocover
+    NotImplementedWarning.warn("Cocoa", feature)
 
 
 __all__ = [
     "not_implemented",
     "App",
     "DocumentApp",
     "MainWindow",
@@ -49,23 +53,25 @@
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

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/fonts.py` & `toga_cocoa-0.4.3/src/toga_cocoa/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/hardware/camera.py` & `toga_cocoa-0.4.3/src/toga_cocoa/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/images.py` & `toga_cocoa-0.4.3/src/toga_cocoa/images.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,39 +19,52 @@
 
 
 class Image:
     RAW_TYPE = NSImage
 
     def __init__(self, interface, path=None, data=None, raw=None):
         self.interface = interface
+        self._needs_release = False
 
         try:
             # We *should* be able to do a direct NSImage.alloc.init...(), but if the
-            # image file is invalid, the init fails, and returns NULL - but we've
-            # created an ObjC instance, so when the object passes out of scope, Rubicon
-            # tries to free it, which segfaults. To avoid this, we retain result of the
-            # alloc() (overriding the default Rubicon behavior of alloc), then release
-            # that reference once we're done. If the image was created successfully, we
-            # temporarily have a reference count that is 1 higher than it needs to be;
-            # if it fails, we don't end up with a stray release.
+            # image file is invalid, the init fails, returns NULL, and releases the
+            # Objective-C object. Since we've created an ObjC instance, when the object
+            # passes out of scope, Rubicon tries to free it, which segfaults.
+            # To avoid this, we retain result of the alloc() (overriding the default
+            # Rubicon behavior of alloc), then release that reference once we're done.
+            # If the image was created successfully, we temporarily have a reference
+            # count that is 1 higher than it needs to be; if it fails, we don't end up
+            # with a stray release.
             image = NSImage.alloc().retain()
             if path:
                 self.native = image.initWithContentsOfFile(str(path))
                 if self.native is None:
                     raise ValueError(f"Unable to load image from {path}")
+                else:
+                    self._needs_release = True
             elif data:
                 nsdata = NSData.dataWithBytes(data, length=len(data))
                 self.native = image.initWithData(nsdata)
                 if self.native is None:
                     raise ValueError("Unable to load image from data")
+                else:
+                    self._needs_release = True
             else:
                 self.native = raw
         finally:
+            # Calling `release` here disabled Rubicon's "release on delete" automation.
+            # We therefore add an explicit `release` call in __del__ if the NSImage was
+            # initialized successfully.
             image.release()
 
+    def __del__(self):
+        if self._needs_release:
+            self.native.release()
+
     def get_width(self):
         return self.native.size.width
 
     def get_height(self):
         return self.native.size.height
 
     def get_data(self):
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/keys.py` & `toga_cocoa-0.4.3/src/toga_cocoa/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     34: Key.I,
     35: Key.P,
     36: Key.ENTER,
     37: Key.L,
     38: Key.J,
     39: Key.QUOTE,
     40: Key.K,
-    41: Key.COLON,
+    41: Key.SEMICOLON,
     42: Key.BACKSLASH,
     43: Key.COMMA,
     44: Key.SLASH,
     45: Key.N,
     46: Key.M,
     47: Key.FULL_STOP,
     48: Key.TAB,
@@ -99,35 +99,35 @@
     124: Key.RIGHT,
     125: Key.DOWN,
     126: Key.UP,
 }
 
 # Keys that have a different Toga key when Shift is pressed.
 TOGA_SHIFT_MODIFIED = {
+    Key.BACK_QUOTE: Key.TILDE,
     Key._1: Key.EXCLAMATION,
     Key._2: Key.AT,
     Key._3: Key.HASH,
     Key._4: Key.DOLLAR,
-    Key._6: Key.CARET,
     Key._5: Key.PERCENT,
-    Key.PLUS: Key.EQUAL,
-    Key._9: Key.OPEN_PARENTHESIS,
+    Key._6: Key.CARET,
     Key._7: Key.AMPERSAND,
-    Key.MINUS: Key.UNDERSCORE,
     Key._8: Key.ASTERISK,
+    Key._9: Key.OPEN_PARENTHESIS,
     Key._0: Key.CLOSE_PARENTHESIS,
-    Key.CLOSE_BRACKET: Key.CLOSE_BRACKET,
-    Key.OPEN_BRACKET: Key.OPEN_BRACKET,
-    Key.ENTER: Key.ENTER,
+    Key.MINUS: Key.UNDERSCORE,
+    Key.EQUAL: Key.PLUS,
+    Key.CLOSE_BRACKET: Key.CLOSE_BRACE,
+    Key.OPEN_BRACKET: Key.OPEN_BRACE,
+    Key.BACKSLASH: Key.PIPE,
     Key.QUOTE: Key.DOUBLE_QUOTE,
-    Key.COLON: Key.SEMICOLON,
+    Key.SEMICOLON: Key.COLON,
     Key.COMMA: Key.LESS_THAN,
-    Key.SLASH: Key.QUESTION,
     Key.FULL_STOP: Key.GREATER_THAN,
-    Key.BACK_QUOTE: Key.TILDE,
+    Key.SLASH: Key.QUESTION,
 }
 
 
 def toga_key(event):
     """Convert a Cocoa NSKeyEvent into a Toga event."""
     natural_key = TOGA_KEYS.get(event.keyCode, None)
     if event.modifierFlags & NSEventModifierFlagShift:
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/__init__.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,10 +19,12 @@
     objc_property,
     send_super,
 )
 
 from .appkit import *  # noqa: F401, F403
 from .av_foundation import *  # noqa: F401, F403
 from .core_graphics import *  # noqa: F401, F403
+from .core_location import *  # noqa: F401, F403
 from .core_text import *  # noqa: F401, F403
 from .foundation import *  # noqa: F401, F403
+from .mapkit import *  # noqa: F401, F403
 from .webkit import *  # noqa: F401, F403
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/appkit.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/appkit.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/av_foundation.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/av_foundation.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/core_graphics.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/core_graphics.py`

 * *Files 10% similar despite different names*

```diff
@@ -198,14 +198,24 @@
 ######################################################################
 # CGEventTypes.h
 kCGScrollEventUnitPixel = 0
 kCGScrollEventUnitLine = 1
 
 ######################################################################
 # CGImage.h
+
+CGImageRef = c_void_p
+register_preferred_encoding(b"^{CGImage=}", CGImageRef)
+
+core_graphics.CGImageGetWidth.argtypes = [CGImageRef]
+core_graphics.CGImageGetWidth.restype = c_size_t
+
+core_graphics.CGImageGetHeight.argtypes = [CGImageRef]
+core_graphics.CGImageGetHeight.restype = c_size_t
+
 kCGImageAlphaNone = 0
 kCGImageAlphaPremultipliedLast = 1
 kCGImageAlphaPremultipliedFirst = 2
 kCGImageAlphaLast = 3
 kCGImageAlphaFirst = 4
 kCGImageAlphaNoneSkipLast = 5
 kCGImageAlphaNoneSkipFirst = 6
@@ -216,7 +226,20 @@
 
 kCGBitmapByteOrderMask = 0x7000
 kCGBitmapByteOrderDefault = 0 << 12
 kCGBitmapByteOrder16Little = 1 << 12
 kCGBitmapByteOrder32Little = 2 << 12
 kCGBitmapByteOrder16Big = 3 << 12
 kCGBitmapByteOrder32Big = 4 << 12
+
+######################################################################
+# CGDirectDisplay.h
+
+CGDirectDisplayID = c_uint32
+
+# CGDirectDisplayID CGMainDisplayID(void);
+core_graphics.CGMainDisplayID.restype = CGDirectDisplayID
+core_graphics.CGMainDisplayID.argtypes = None
+
+# CGImageRef CGDisplayCreateImage(CGDirectDisplayID displayID, CGRect rect);
+core_graphics.CGDisplayCreateImage.restype = CGImageRef
+core_graphics.CGDisplayCreateImage.argtypes = [CGDirectDisplayID, CGRect]
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/core_text.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/core_text.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/foundation.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/foundation.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/libs/webkit.py` & `toga_cocoa-0.4.3/src/toga_cocoa/libs/webkit.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/paths.py` & `toga_cocoa-0.4.3/src/toga_cocoa/paths.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/resources/camera.png` & `toga_cocoa-0.4.3/src/toga_cocoa/resources/camera.png`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/resources/toga.icns` & `toga_cocoa-0.4.3/src/toga_cocoa/resources/toga.icns`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/activityindicator.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/base.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/box.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/box.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/button.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/canvas.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from math import ceil
 
-from rubicon.objc import objc_method, objc_property
+from rubicon.objc import CGSize, objc_method, objc_property
 from travertino.size import at_least
 
 from toga.colors import BLACK, TRANSPARENT, color
 from toga.widgets.canvas import Baseline, FillRule
 from toga_cocoa.colors import native_color
-from toga_cocoa.images import nsdata_to_bytes
 from toga_cocoa.libs import (
     CGFloat,
     CGPathDrawingMode,
     CGRectMake,
     NSAttributedString,
-    NSBitmapImageFileType,
     NSFontAttributeName,
     NSForegroundColorAttributeName,
     NSGraphicsContext,
+    NSImage,
     NSMutableDictionary,
     NSPoint,
     NSRect,
     NSSize,
     NSStrokeColorAttributeName,
     NSStrokeWidthAttributeName,
     NSView,
@@ -317,23 +316,26 @@
             # (https://www.sketch.com/blog/typesetting-in-sketch/), but it would be
             # unwise to rely on that.
             rs.drawWithRect(
                 NSRect(origin, NSSize(2**31 - 1, 0)), options=0, context=None
             )
 
     def get_image_data(self):
+
         bitmap = self.native.bitmapImageRepForCachingDisplayInRect(self.native.bounds)
-        bitmap.setSize(self.native.bounds.size)
         self.native.cacheDisplayInRect(self.native.bounds, toBitmapImageRep=bitmap)
 
-        return nsdata_to_bytes(
-            bitmap.representationUsingType(
-                NSBitmapImageFileType.PNG,
-                properties=None,
-            )
+        # Get a reference to the CGImage from the bitmap
+        cg_image = bitmap.CGImage
+
+        target_size = CGSize(
+            core_graphics.CGImageGetWidth(cg_image),
+            core_graphics.CGImageGetHeight(cg_image),
         )
+        ns_image = NSImage.alloc().initWithCGImage(cg_image, size=target_size)
+        return ns_image
 
     # Rehint
     def rehint(self):
         fitting_size = self.native.fittingSize()
         self.interface.intrinsic.height = at_least(fitting_size.height)
         self.interface.intrinsic.width = at_least(fitting_size.width)
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/detailedlist.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/detailedlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 
 class TogaList(NSTableView):
     interface = objc_property(object, weak=True)
     impl = objc_property(object, weak=True)
 
     @objc_method
+    def didCloseMenu_withEvent_(self, menu, event) -> None:
+        # When the menu closes, drop the reference to the menu object.
+        self.impl._popup = None
+
+    @objc_method
     def menuForEvent_(self, event):
         if self.impl.primary_action_enabled or self.impl.secondary_action_enabled:
             # Find the row under the mouse click
             mousePoint = self.convertPoint(event.locationInWindow, fromView=None)
             row = self.rowAtPoint(mousePoint)
 
             # Ensure the row is selected.
@@ -45,17 +50,20 @@
                 secondary_action_item = popup.addItemWithTitle(
                     self.interface._secondary_action,
                     action=SEL("secondaryActionOnRow:"),
                     keyEquivalent="",
                 )
                 secondary_action_item.tag = row
 
-            return popup
         else:
-            return None
+            popup = None
+
+        # Preserve a Python reference to the popup for testing purposes.
+        self.impl._popup = popup
+        return popup
 
     @objc_method
     def primaryActionOnRow_(self, menuitem):
         row = self.interface.data[menuitem.tag]
         self.interface.on_primary_action(row=row)
 
     @objc_method
@@ -71,15 +79,14 @@
     @objc_method
     def tableView_objectValueForTableColumn_row_(self, table, column, row: int):
         value = self.interface.data[row]
         try:
             data = value._impl
         except AttributeError:
             data = TogaData.alloc().init()
-            data.retain()
             value._impl = data
 
         try:
             title = getattr(value, self.interface.accessors[0])
             if title is not None:
                 title = str(title)
             else:
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/divider.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/imageview.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/cells.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/cells.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/internal/refresh.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/refresh.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,20 @@
             self,
             "constrainScrollPoint:",
             proposedNewOrigin,
             restype=NSPoint,
             argtypes=[NSPoint],
         )
 
-        if self.superview and self.superview.is_refreshing:
+        # FIXME: This has been marked no-cover so that ARM64 testing can be enabled;
+        # ARM64 CI can only run on Sonoma, and it looks like Sonoma has turned off
+        # scroll elasticity by default, which prevents pull-to-refresh from working.
+        # See Toga#2412 for details. If that ticket is closed, it should be possible
+        # to remove this this no-cover.
+        if self.superview and self.superview.is_refreshing:  # pragma: no cover
             return NSMakePoint(
                 constrained.x,
                 max(
                     proposedNewOrigin.y, -self.superview.refresh_view.frame.size.height
                 ),
             )
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/label.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/multilinetextinput.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/numberinput.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/optioncontainer.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/passwordinput.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/passwordinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/progressbar.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/scrollcontainer.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/selection.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/slider.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/splitcontainer.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/switch.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/table.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
         if not tcv:  # there is no existing view to reuse so create a new one
             tcv = TogaIconView.alloc().init()
             tcv.identifier = identifier
 
             # Prevent tcv from being deallocated prematurely when no Python references
             # are left
-            tcv.retain()
             tcv.autorelease()
 
         tcv.setText(str(value))
         if icon:
             tcv.setImage(icon._impl.native)
         else:
             tcv.setImage(None)
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/textinput.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/tree.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     NSTableViewColumnAutoresizingStyle,
 )
 from toga_cocoa.widgets.base import Widget
 from toga_cocoa.widgets.internal.cells import TogaIconView
 from toga_cocoa.widgets.internal.data import TogaData
 
 
+def node_impl(node):
+    try:
+        return node._impl
+    except AttributeError:
+        node._impl = TogaData.alloc().init()
+        node._impl.attrs = {"node": node}
+        return node._impl
+
+
 class TogaTree(NSOutlineView):
     interface = objc_property(object, weak=True)
     impl = objc_property(object, weak=True)
 
     # OutlineViewDataSource methods
     @objc_method
     def outlineView_child_ofItem_(self, tree, child: int, item):
@@ -28,22 +37,16 @@
             node = self.interface.data[child]
         else:
             node = item.attrs["node"][child]
 
         # Get the Cocoa implementation for the row. If an _impl
         # doesn't exist, create a data object for it, and
         # populate it with initial values for each column.
-        try:
-            node_impl = node._impl
-        except AttributeError:
-            node_impl = TogaData.alloc().init()
-            node_impl.attrs = {"node": node}
-            node._impl = node_impl
 
-        return node_impl
+        return node_impl(node)
 
     @objc_method
     def outlineView_isItemExpandable_(self, tree, item) -> bool:
         return item.attrs["node"].can_have_children()
 
     @objc_method
     def outlineView_numberOfChildrenOfItem_(self, tree, item) -> int:
@@ -94,15 +97,14 @@
         if not tcv:  # there is no existing view to reuse so create a new one
             # tcv = TogaIconView.alloc().initWithFrame(CGRectMake(0, 0, column.width, 16))
             tcv = TogaIconView.alloc().init()
             tcv.identifier = identifier
 
             # Prevent tcv from being deallocated prematurely when no Python references
             # are left
-            tcv.retain()
             tcv.autorelease()
 
         tcv.setText(str(value))
         if icon:
             tcv.setImage(icon._impl.native)
         else:
             tcv.setImage(None)
@@ -216,30 +218,33 @@
     def change_source(self, source):
         self.native_tree.reloadData()
 
     def insert(self, parent, index, item):
         index_set = NSIndexSet.indexSetWithIndex(index)
         self.native_tree.insertItemsAtIndexes(
             index_set,
-            inParent=parent._impl if parent else None,
+            inParent=node_impl(parent) if parent else None,
             withAnimation=NSTableViewAnimation.SlideDown.value,
         )
 
     def change(self, item):
-        self.native_tree.reloadItem(item._impl)
+        self.native_tree.reloadItem(node_impl(item))
 
     def remove(self, parent, index, item):
-        index = self.native_tree.childIndexForItem(item._impl)
-        index_set = NSIndexSet.indexSetWithIndex(index)
-        parent = self.native_tree.parentForItem(item._impl)
-        self.native_tree.removeItemsAtIndexes(
-            index_set,
-            inParent=parent,
-            withAnimation=NSTableViewAnimation.SlideUp.value,
-        )
+        try:
+            index = self.native_tree.childIndexForItem(item._impl)
+            index_set = NSIndexSet.indexSetWithIndex(index)
+            parent = self.native_tree.parentForItem(item._impl)
+            self.native_tree.removeItemsAtIndexes(
+                index_set,
+                inParent=parent,
+                withAnimation=NSTableViewAnimation.SlideUp.value,
+            )
+        except AttributeError:
+            pass
 
     def clear(self):
         self.native_tree.reloadData()
 
     def get_selection(self):
         if self.interface.multiple_select:
             selection = []
@@ -260,21 +265,21 @@
             index = self.native_tree.selectedRow
             if index != -1:
                 return self.native_tree.itemAtRow(index).attrs["node"]
             else:
                 return None
 
     def expand_node(self, node):
-        self.native_tree.expandItem(node._impl, expandChildren=True)
+        self.native_tree.expandItem(node_impl(node), expandChildren=True)
 
     def expand_all(self):
         self.native_tree.expandItem(None, expandChildren=True)
 
     def collapse_node(self, node):
-        self.native_tree.collapseItem(node._impl, collapseChildren=True)
+        self.native_tree.collapseItem(node_impl(node), collapseChildren=True)
 
     def collapse_all(self):
         self.native_tree.collapseItem(None, collapseChildren=True)
 
     def _insert_column(self, index, heading, accessor):
         column = NSTableColumn.alloc().initWithIdentifier(accessor)
         column.minWidth = 16
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/widgets/webview.py` & `toga_cocoa-0.4.3/src/toga_cocoa/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa/window.py` & `toga_cocoa-0.4.3/src/toga_cocoa/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+from rubicon.objc import CGSize
+
 from toga.command import Command, Separator
 from toga_cocoa.container import Container
-from toga_cocoa.images import nsdata_to_bytes
 from toga_cocoa.libs import (
     SEL,
     NSBackingStoreBuffered,
-    NSBitmapImageFileType,
+    NSImage,
     NSMakeRect,
     NSMutableArray,
     NSPoint,
     NSScreen,
     NSSize,
     NSToolbar,
     NSToolbarItem,
     NSWindow,
     NSWindowStyleMask,
+    core_graphics,
     objc_method,
     objc_property,
 )
 
+from .screens import Screen as ScreenImpl
+
 
 def toolbar_identifier(cmd):
     return f"Toolbar-{type(cmd).__name__}-{id(cmd)}"
 
 
 class TogaWindow(NSWindow):
     interface = objc_property(object, weak=True)
@@ -171,33 +175,41 @@
         self._toolbar_items = {}
         self.native_toolbar = None
 
     def __del__(self):
         self.purge_toolbar()
         self.native.release()
 
-    def purge_toolbar(self):
-        while self._toolbar_items:
-            dead_items = []
-            _, cmd = self._toolbar_items.popitem()
-            # The command might have toolbar representations on multiple window
-            # toolbars, and may have other representations (at the very least, a menu
-            # item). Only clean up the representation pointing at *this* window. Do this
-            # in 2 passes so that we're not modifying the set of native objects while
-            # iterating over it.
-            for item_native in cmd._impl.native:
-                if (
-                    isinstance(item_native, NSToolbarItem)
-                    and item_native.target == self.native
-                ):
-                    dead_items.append(item_native)
+    ######################################################################
+    # Native event handlers
+    ######################################################################
 
-            for item_native in dead_items:
-                cmd._impl.native.remove(item_native)
-                item_native.release()
+    def cocoa_windowShouldClose(self):
+        # The on_close handler has a cleanup method that will enforce
+        # the close if the on_close handler requests it; this initial
+        # "should close" request can always return False.
+        self.interface.on_close()
+        return False
+
+    ######################################################################
+    # Window properties
+    ######################################################################
+
+    def get_title(self):
+        return str(self.native.title)
+
+    def set_title(self, title):
+        self.native.title = title
+
+    ######################################################################
+    # Window lifecycle
+    ######################################################################
+
+    def close(self):
+        self.native.close()
 
     def create_toolbar(self):
         # Purge any existing toolbar items
         self.purge_toolbar()
 
         # Create the new toolbar items.
         if self.interface.toolbar:
@@ -214,17 +226,43 @@
 
         self.native.setToolbar(self.native_toolbar)
 
         # Adding/removing a toolbar changes the size of the content window.
         if self.interface.content:
             self.interface.content.refresh()
 
-    def set_content(self, widget):
-        # Set the content of the window's container
-        self.container.content = widget
+    def purge_toolbar(self):
+        while self._toolbar_items:
+            dead_items = []
+            _, cmd = self._toolbar_items.popitem()
+            # The command might have toolbar representations on multiple window
+            # toolbars, and may have other representations (at the very least, a menu
+            # item). Only clean up the representation pointing at *this* window. Do this
+            # in 2 passes so that we're not modifying the set of native objects while
+            # iterating over it.
+            for item_native in cmd._impl.native:
+                if (
+                    isinstance(item_native, NSToolbarItem)
+                    and item_native.target == self.native
+                ):
+                    dead_items.append(item_native)
+
+            for item_native in dead_items:
+                cmd._impl.native.remove(item_native)
+                item_native.release()
+
+    def set_app(self, app):
+        pass
+
+    def show(self):
+        self.native.makeKeyAndOrderFront(None)
+
+    ######################################################################
+    # Window content and resources
+    ######################################################################
 
     def content_refreshed(self, container):
         min_width = self.interface.content.layout.min_width
         min_height = self.interface.content.layout.min_height
 
         # If the minimum layout is bigger than the current window,
         # increase the size of the window.
@@ -235,19 +273,37 @@
             self.set_size((min_width, frame.size.height))
         elif frame.size.height < min_height:
             self.set_size((frame.size.width, min_height))
 
         self.container.min_width = min_width
         self.container.min_height = min_height
 
-    def get_title(self):
-        return str(self.native.title)
+    def set_content(self, widget):
+        # Set the content of the window's container
+        self.container.content = widget
 
-    def set_title(self, title):
-        self.native.title = title
+    ######################################################################
+    # Window size
+    ######################################################################
+
+    def get_size(self):
+        frame = self.native.frame
+        return frame.size.width, frame.size.height
+
+    def set_size(self, size):
+        frame = self.native.frame
+        frame.size = NSSize(size[0], size[1])
+        self.native.setFrame(frame, display=True, animate=True)
+
+    ######################################################################
+    # Window position
+    ######################################################################
+
+    def get_current_screen(self):
+        return ScreenImpl(self.native.screen)
 
     def get_position(self):
         # The "primary" screen has index 0 and origin (0, 0).
         primary_screen = NSScreen.screens[0].frame
         window_frame = self.native.frame
 
         # macOS origin is bottom left of screen, and the screen might be
@@ -265,56 +321,47 @@
         # macOS origin is bottom left of screen, and the screen might be
         # offset relative to other screens. Adjust for this.
         x = position[0]
         y = primary_screen.size.height - position[1]
 
         self.native.setFrameTopLeftPoint(NSPoint(x, y))
 
-    def get_size(self):
-        frame = self.native.frame
-        return frame.size.width, frame.size.height
-
-    def set_size(self, size):
-        frame = self.native.frame
-        frame.size = NSSize(size[0], size[1])
-        self.native.setFrame(frame, display=True, animate=True)
-
-    def set_app(self, app):
-        pass
-
-    def show(self):
-        self.native.makeKeyAndOrderFront(None)
+    ######################################################################
+    # Window visibility
+    ######################################################################
 
     def hide(self):
         self.native.orderOut(self.native)
 
     def get_visible(self):
         return bool(self.native.isVisible)
 
+    ######################################################################
+    # Window state
+    ######################################################################
+
     def set_full_screen(self, is_full_screen):
         current_state = bool(self.native.styleMask & NSWindowStyleMask.FullScreen)
         if is_full_screen != current_state:
             self.native.toggleFullScreen(self.native)
 
-    def cocoa_windowShouldClose(self):
-        # The on_close handler has a cleanup method that will enforce
-        # the close if the on_close handler requests it; this initial
-        # "should close" request can always return False.
-        self.interface.on_close()
-        return False
-
-    def close(self):
-        self.native.close()
+    ######################################################################
+    # Window capabilities
+    ######################################################################
 
     def get_image_data(self):
         bitmap = self.container.native.bitmapImageRepForCachingDisplayInRect(
             self.container.native.bounds
         )
-        bitmap.setSize(self.container.native.bounds.size)
         self.container.native.cacheDisplayInRect(
             self.container.native.bounds, toBitmapImageRep=bitmap
         )
-        data = bitmap.representationUsingType(
-            NSBitmapImageFileType.PNG,
-            properties=None,
+
+        # Get a reference to the CGImage from the bitmap
+        cg_image = bitmap.CGImage
+
+        target_size = CGSize(
+            core_graphics.CGImageGetWidth(cg_image),
+            core_graphics.CGImageGetHeight(cg_image),
         )
-        return nsdata_to_bytes(data)
+        ns_image = NSImage.alloc().initWithCGImage(cg_image, size=target_size)
+        return ns_image
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa.egg-info/PKG-INFO` & `toga_cocoa-0.4.3/src/toga_cocoa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: toga-cocoa
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Cocoa (macOS) backend for the Toga widget toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,macOS,cocoa
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
 Requires-Dist: fonttools<5.0.0,>=4.42.1
 Requires-Dist: rubicon-objc<0.5.0,>=0.4.7
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-cocoa
 ==========
 
 A Cocoa backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `macOS platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/macOS.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/macOS.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-cocoa-0.4.2/src/toga_cocoa.egg-info/SOURCES.txt` & `toga_cocoa-0.4.3/src/toga_cocoa.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,42 +12,47 @@
 src/toga_cocoa/documents.py
 src/toga_cocoa/factory.py
 src/toga_cocoa/fonts.py
 src/toga_cocoa/icons.py
 src/toga_cocoa/images.py
 src/toga_cocoa/keys.py
 src/toga_cocoa/paths.py
+src/toga_cocoa/screens.py
 src/toga_cocoa/window.py
 src/toga_cocoa.egg-info/PKG-INFO
 src/toga_cocoa.egg-info/SOURCES.txt
 src/toga_cocoa.egg-info/dependency_links.txt
 src/toga_cocoa.egg-info/entry_points.txt
 src/toga_cocoa.egg-info/requires.txt
 src/toga_cocoa.egg-info/top_level.txt
 src/toga_cocoa/hardware/__init__.py
 src/toga_cocoa/hardware/camera.py
+src/toga_cocoa/hardware/location.py
 src/toga_cocoa/libs/__init__.py
 src/toga_cocoa/libs/appkit.py
 src/toga_cocoa/libs/av_foundation.py
 src/toga_cocoa/libs/core_graphics.py
+src/toga_cocoa/libs/core_location.py
 src/toga_cocoa/libs/core_text.py
 src/toga_cocoa/libs/foundation.py
+src/toga_cocoa/libs/mapkit.py
 src/toga_cocoa/libs/webkit.py
 src/toga_cocoa/resources/camera.png
 src/toga_cocoa/resources/toga.icns
 src/toga_cocoa/widgets/__init__.py
 src/toga_cocoa/widgets/activityindicator.py
 src/toga_cocoa/widgets/base.py
 src/toga_cocoa/widgets/box.py
 src/toga_cocoa/widgets/button.py
 src/toga_cocoa/widgets/canvas.py
 src/toga_cocoa/widgets/detailedlist.py
 src/toga_cocoa/widgets/divider.py
 src/toga_cocoa/widgets/imageview.py
 src/toga_cocoa/widgets/label.py
+src/toga_cocoa/widgets/mapview.py
 src/toga_cocoa/widgets/multilinetextinput.py
 src/toga_cocoa/widgets/numberinput.py
 src/toga_cocoa/widgets/optioncontainer.py
 src/toga_cocoa/widgets/passwordinput.py
 src/toga_cocoa/widgets/progressbar.py
 src/toga_cocoa/widgets/scrollcontainer.py
 src/toga_cocoa/widgets/selection.py
@@ -64,27 +69,30 @@
 src/toga_cocoa/widgets/internal/refresh.py
 tests_backend/__init__.py
 tests_backend/app.py
 tests_backend/fonts.py
 tests_backend/icons.py
 tests_backend/images.py
 tests_backend/probe.py
+tests_backend/screens.py
 tests_backend/window.py
 tests_backend/hardware/__init__.py
 tests_backend/hardware/camera.py
+tests_backend/hardware/location.py
 tests_backend/widgets/__init__.py
 tests_backend/widgets/activityindicator.py
 tests_backend/widgets/base.py
 tests_backend/widgets/box.py
 tests_backend/widgets/button.py
 tests_backend/widgets/canvas.py
 tests_backend/widgets/detailedlist.py
 tests_backend/widgets/divider.py
 tests_backend/widgets/imageview.py
 tests_backend/widgets/label.py
+tests_backend/widgets/mapview.py
 tests_backend/widgets/multilinetextinput.py
 tests_backend/widgets/numberinput.py
 tests_backend/widgets/optioncontainer.py
 tests_backend/widgets/passwordinput.py
 tests_backend/widgets/progressbar.py
 tests_backend/widgets/properties.py
 tests_backend/widgets/scrollcontainer.py
```

### Comparing `toga-cocoa-0.4.2/tests_backend/app.py` & `toga_cocoa-0.4.3/tests_backend/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
 
+import PIL.Image
 from rubicon.objc import NSPoint, ObjCClass, objc_id, send_message
 
+import toga
 from toga_cocoa.keys import cocoa_key, toga_key
 from toga_cocoa.libs import (
     NSApplication,
     NSEvent,
     NSEventModifierFlagShift,
     NSEventType,
     NSWindow,
@@ -54,14 +56,50 @@
 
     def content_size(self, window):
         return (
             window.content._impl.native.frame.size.width,
             window.content._impl.native.frame.size.height,
         )
 
+    def assert_app_icon(self, icon):
+        # We have no real way to check we've got the right icon; use pixel peeping as a
+        # guess. Construct a PIL image from the current icon.
+        img = toga.Image(
+            NSApplication.sharedApplication.applicationIconImage
+        ).as_format(PIL.Image.Image)
+
+        # Due to icon resizing and colorspace issues, the exact pixel colors are
+        # inconsistent, so multiple values must be provided for test purposes.
+        if icon:
+            # The explicit alt icon has blue background, with green at a point 1/3 into
+            # the image
+            assert img.getpixel((5, 5)) in {
+                (205, 226, 243, 255),
+                (211, 226, 243, 255),
+                (211, 230, 245, 255),
+            }
+            mid_color = img.getpixel((img.size[0] // 3, img.size[1] // 3))
+            assert mid_color in {
+                (0, 204, 9, 255),
+                (6, 204, 8, 255),
+                (14, 197, 8, 255),
+                (105, 192, 32, 255),
+            }
+        else:
+            # The default icon is transparent background, and brown in the center.
+            assert img.getpixel((5, 5))[3] == 0
+            mid_color = img.getpixel((img.size[0] // 2, img.size[1] // 2))
+            assert mid_color in {
+                (130, 100, 57, 255),
+                (130, 109, 66, 255),
+                (138, 107, 64, 255),
+                (138, 108, 64, 255),
+                (149, 119, 73, 255),
+            }
+
     def _menu_item(self, path):
         main_menu = self.app._impl.native.mainMenu
 
         menu = main_menu
         orig_path = path.copy()
         while True:
             label, path = path[0], path[1:]
@@ -143,27 +181,43 @@
     def activate_menu_minimize(self):
         self._activate_menu_item(["Window", "Minimize"])
 
     def assert_menu_item(self, path, enabled):
         item = self._menu_item(path)
         assert item.isEnabled() == enabled
 
+    def assert_menu_order(self, path, expected):
+        menu = self._menu_item(path).submenu
+
+        assert menu.numberOfItems == len(expected)
+        for item, title in zip(menu.itemArray, expected):
+            if title == "---":
+                assert item.isSeparatorItem
+            else:
+                assert item.title == title
+
     def keystroke(self, combination):
         key, modifiers = cocoa_key(combination)
         key_code = {
             "a": 0,
             "A": 0,
             "1": 18,
             "!": 18,
+            "'": 39,
+            ";": 41,
+            "|": 42,
+            " ": 49,
             chr(0xF708): 96,  # F5
             chr(0x2196): 115,  # Home
+            # This only works because we're *not* testing the numeric 5
+            "5": 87,
         }[key]
 
-        # Add the shift modifier to disambiguate 1 from !
-        if key in {"!"}:
+        # Add the shift modifier to disambiguate shifted keys from non-shifted
+        if key in {"!", "|"}:
             modifiers |= NSEventModifierFlagShift
 
         event = NSEvent.keyEventWithType(
             NSEventType.KeyDown,
             location=NSPoint(0, 0),  # key presses don't have a location.
             modifierFlags=modifiers,
             timestamp=0,
```

### Comparing `toga-cocoa-0.4.2/tests_backend/fonts.py` & `toga_cocoa-0.4.3/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/hardware/camera.py` & `toga_cocoa-0.4.3/tests_backend/hardware/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
                 return AVAuthorizationStatus.NotDetermined.value
 
         self._mock_AVCaptureDevice.authorizationStatusForMediaType = _mock_auth_status
 
         def _mock_request_access(media_type, completionHandler):
             # Fire completion handler
             try:
+                self._mock_permissions[str(media_type)] = abs(
+                    self._mock_permissions[str(media_type)]
+                )
                 result = bool(self._mock_permissions[str(media_type)])
             except KeyError:
                 # If there's no explicit permission, it's a denial
                 self._mock_permissions[str(media_type)] = 0
                 result = False
             completionHandler.func(result)
 
@@ -130,18 +133,18 @@
     def disconnect_cameras(self):
         self._mock_AVCaptureDevice.devicesWithMediaType.return_value = []
 
     def reset_permission(self):
         self._mock_permissions = {}
 
     def grant_permission(self):
-        self._mock_permissions[str(AVMediaTypeVideo)] = -1
+        self._mock_permissions[str(AVMediaTypeVideo)] = 1
 
     def allow_permission(self):
-        self._mock_permissions[str(AVMediaTypeVideo)] = 1
+        self._mock_permissions[str(AVMediaTypeVideo)] = -1
 
     def reject_permission(self):
         self._mock_permissions[str(AVMediaTypeVideo)] = 0
 
     async def wait_for_camera(self, device_count=2):
         # A short delay is needed to ensure that the window fully creates.
         await self.redraw("Camera view displayed", delay=0.1)
```

### Comparing `toga-cocoa-0.4.2/tests_backend/probe.py` & `toga_cocoa-0.4.3/tests_backend/probe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from ctypes import c_void_p
 
 from rubicon.objc import SEL, NSArray, NSObject, ObjCClass, objc_method
 from rubicon.objc.api import NSString
 
+import toga
 from toga_cocoa.libs.appkit import appkit
 
 NSRunLoop = ObjCClass("NSRunLoop")
 NSRunLoop.declare_class_property("currentRunLoop")
 NSDefaultRunLoopMode = NSString(c_void_p.in_dll(appkit, "NSDefaultRunLoopMode"))
 
 
@@ -42,25 +43,25 @@
                 target=self.event_listener,
                 argument=None,
                 order=0,
                 modes=NSArray.arrayWithObject(NSDefaultRunLoopMode),
             )
             await self.event_listener.event.wait()
 
-    async def redraw(self, message=None, delay=None):
+    async def redraw(self, message=None, delay=0):
         """Request a redraw of the app, waiting until that redraw has completed."""
-        if self.app.run_slow:
-            # If we're running slow, wait for a second
-            print("Waiting for redraw" if message is None else message)
-            delay = 1
+        if toga.App.app.run_slow:
+            # If we're running slow, wait for at least a second
+            delay = max(1, delay)
 
         if delay:
+            print("Waiting for redraw" if message is None else message)
             await asyncio.sleep(delay)
         else:
             # Running at "normal" speed, we need to release to the event loop
             # for at least one iteration. `runUntilDate:None` does this.
             NSRunLoop.currentRunLoop.runUntilDate(None)
 
-    def assert_image_size(self, image_size, size):
-        # Cocoa reports image sizing in the natural screen coordinates, not the size of
-        # the backing store.
-        assert image_size == size
+    def assert_image_size(self, image_size, size, screen):
+        # Screenshots are captured in native device resolution, not in CSS pixels.
+        scale = int(screen._impl.native.backingScaleFactor)
+        assert image_size == (size[0] * scale, size[1] * scale)
```

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/base.py` & `toga_cocoa-0.4.3/tests_backend/widgets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         assert self.widget._impl.container is None
         assert self.native.superview is None
         assert self.native.window is None
 
     def assert_alignment(self, expected):
         assert self.alignment == expected
 
-    async def redraw(self, message=None, delay=None):
+    async def redraw(self, message=None, delay=0):
         """Request a redraw of the app, waiting until that redraw has completed."""
         # Force a widget repaint
         self.widget.window.content._impl.native.displayIfNeeded()
 
         await super().redraw(message=message, delay=delay)
 
     @property
```

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/button.py` & `toga_cocoa-0.4.3/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/canvas.py` & `toga_cocoa-0.4.3/tests_backend/widgets/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from io import BytesIO
 
 from PIL import Image, ImageCms
 from rubicon.objc import NSPoint
 
 from toga.colors import TRANSPARENT
+from toga.images import Image as TogaImage
 from toga_cocoa.libs import NSEventType, NSView
 
 from .base import SimpleProbe
 from .properties import toga_color
 
 
 class CanvasProbe(SimpleProbe):
@@ -23,15 +24,15 @@
     def reference_variant(self, reference):
         if reference in {"multiline_text", "write_text"}:
             # System font and default size is platform dependent.
             return f"{reference}-macOS"
         return reference
 
     def get_image(self):
-        image = Image.open(BytesIO(self.impl.get_image_data()))
+        image = Image.open(BytesIO(TogaImage(self.impl.get_image_data()).data))
 
         try:
             # If the image has an ICC profile, convert it into sRGB colorspace.
             # This is needed when attached to an laptop display; otherwise the RGB
             # values in colors in the image won't *quite* match.
             icc = image.info["icc_profile"]
             src_profile = ImageCms.ImageCmsProfile(BytesIO(icc))
```

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/detailedlist.py` & `toga_cocoa-0.4.3/tests_backend/widgets/detailedlist.py`

 * *Files 8% similar despite different names*

```diff
@@ -175,43 +175,32 @@
             self.scroll_to_top()
         else:
             assert not self.native.refresh_indicator.isHidden()
             # Wait for the scroll to relax after reload completion
             while self.scroll_position < 0:
                 await asyncio.sleep(0.01)
 
-    async def _perform_action(self, row, offset):
+    async def _perform_action(self, row, index):
         point = self.row_position(row)
-        # First click to show menu
+
+        # Click to show menu
         await self.mouse_event(
             NSEventType.RightMouseDown,
             point,
             delay=0.1,
         )
         await self.redraw("Action menu has been displayed")
 
-        # Pick a point a little to the right of the point where the menu was displayed,
-        # and slightly lower (in reversed y coordinates) to select a menu item.
-        point2 = NSPoint(point.x + 10, point.y - offset)
-        await self.mouse_event(
-            NSEventType.LeftMouseDown,
-            point2,
-            delay=0.1,
-        )
-        await self.mouse_event(
-            NSEventType.LeftMouseUp,
-            point2,
-            delay=0.1,
-        )
+        popup = self.impl._popup
+        if popup:
+            popup.performActionForItemAtIndex(index)
+            popup.cancelTracking()
+
+            # Wait until the popup menu is fully disposed.
+            while self.impl._popup is not None:
+                await self.redraw("Action has been selected", delay=0.1)
 
     async def perform_primary_action(self, row, active=True):
-        # 10px is enough to select the first menu item. It doesn't matter whether the
-        # action is active or not; if the action is inactive, it will either press the
-        # wrong action, or press empty space.
-        await self._perform_action(row, 10)
+        await self._perform_action(row, 0)
 
     async def perform_secondary_action(self, row, active=True):
-        # 30px is enough to select the second menu item. However the secondary action
-        # will be in position 1 on the menu if the primary action is disabled. It
-        # doesn't matter whether the action is active or not; if the action is inactive,
-        # it will either press the wrong action, or press empty space.
-        await self._perform_action(row, 30 if self.impl.primary_action_enabled else 10)
+        await self._perform_action(row, 1 if self.impl.primary_action_enabled else 0)
```

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/label.py` & `toga_cocoa-0.4.3/tests_backend/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/multilinetextinput.py` & `toga_cocoa-0.4.3/tests_backend/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/numberinput.py` & `toga_cocoa-0.4.3/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/optioncontainer.py` & `toga_cocoa-0.4.3/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/progressbar.py` & `toga_cocoa-0.4.3/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/properties.py` & `toga_cocoa-0.4.3/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/scrollcontainer.py` & `toga_cocoa-0.4.3/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/selection.py` & `toga_cocoa-0.4.3/tests_backend/widgets/selection.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,12 +42,9 @@
             NSPoint(self.width / 2, self.height / 2), toView=None
         )
         # Selection maintains an inner mouse event loop, so we can't
         # use the "wait for another event" approach for the mouse events.
         # Use a short delaly instead.
         await self.mouse_event(NSEventType.LeftMouseDown, point, delay=0.1)
 
-        # macOS coordinate systems are backwards, so to select the item *above*
-        # the current selection, you need to *add* height.
-        point.y = point.y + self.height
-        await self.mouse_event(NSEventType.LeftMouseDown, point, delay=0.1)
-        await self.mouse_event(NSEventType.LeftMouseUp, point, delay=0.1)
+        self.native.menu.performActionForItemAtIndex(1)
+        self.native.menu.cancelTracking()
```

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/slider.py` & `toga_cocoa-0.4.3/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/splitcontainer.py` & `toga_cocoa-0.4.3/tests_backend/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/table.py` & `toga_cocoa-0.4.3/tests_backend/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/textinput.py` & `toga_cocoa-0.4.3/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/widgets/tree.py` & `toga_cocoa-0.4.3/tests_backend/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga-cocoa-0.4.2/tests_backend/window.py` & `toga_cocoa-0.4.3/tests_backend/window.py`

 * *Files identical despite different names*

