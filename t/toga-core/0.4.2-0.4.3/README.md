# Comparing `tmp/toga-core-0.4.2.tar.gz` & `tmp/toga_core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-core-0.4.2.tar", last modified: Tue Feb  6 05:53:56 2024, max compression
+gzip compressed data, was "toga_core-0.4.3.tar", last modified: Mon May  6 06:43:32 2024, max compression
```

## Comparing `toga-core-0.4.2.tar` & `toga_core-0.4.3.tar`

### file list

```diff
@@ -1,191 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.743252 toga-core-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:53:20.000000 toga-core-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:53:20.000000 toga-core-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-06 05:53:56.743252 toga-core-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-06 05:53:20.000000 toga-core-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-06 05:53:20.000000 toga-core-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:53:56.743252 toga-core-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.707252 toga-core-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.711252 toga-core-0.4.2/src/toga/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31692 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.711252 toga-core-0.4.2/src/toga/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.711252 toga-core-0.4.2/src/toga/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.711252 toga-core-0.4.2/src/toga/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.715252 toga-core-0.4.2/src/toga/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/list_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/tree_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/sources/value_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.715252 toga-core-0.4.2/src/toga/style/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/style/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    40879 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/style/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.719251 toga-core-0.4.2/src/toga/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    59824 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    16553 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)    29667 2024-02-06 05:53:20.000000 toga-core-0.4.2/src/toga/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.743252 toga-core-0.4.2/src/toga_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-06 05:53:56.000000 toga-core-0.4.2/src/toga_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-06 05:53:56.000000 toga-core-0.4.2/src/toga_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:53:56.000000 toga-core-0.4.2/src/toga_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-06 05:53:56.000000 toga-core-0.4.2/src/toga_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-06 05:53:56.000000 toga-core-0.4.2/src/toga_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.723252 toga-core-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.723252 toga-core-0.4.2/tests/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/test_documentapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/test_mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/test_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/app/test_windowset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.723252 toga-core-0.4.2/tests/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/command/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/command/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/command/test_commandset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/command/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.723252 toga-core-0.4.2/tests/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/hardware/test_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.727252 toga-core-0.4.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/orange.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/orange.png
--rw-r--r--   0 runner    (1001) docker     (127)   772491 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/photo.png
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/red-16.png
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/red-32.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/red-72.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/red.png
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/sample-dummy.png
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/sample.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/resources/toga.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.731252 toga-core-0.4.2/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10103 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_list_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_tree_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/sources/test_value_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.731252 toga-core-0.4.2/tests/style/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.731252 toga-core-0.4.2/tests/style/pack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.731252 toga-core-0.4.2/tests/style/pack/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_beeliza.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_column_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_flex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_row_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_rtl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_tutorial0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_tutorial1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/layout/test_tutorial3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/test_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/pack/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/style/test_applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)    19995 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    20075 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/test_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.735252 toga-core-0.4.2/tests/testbed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.735252 toga-core-0.4.2/tests/testbed/customize/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/customize/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.735252 toga-core-0.4.2/tests/testbed/simple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/simple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/simple/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.735252 toga-core-0.4.2/tests/testbed/subclassed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/subclassed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/subclassed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/testbed/subclassed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.739252 toga-core-0.4.2/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.739252 toga-core-0.4.2/tests/widgets/canvas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/test_context_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/test_draw_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/canvas/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    34443 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16361 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/widgets/test_webview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:56.743252 toga-core-0.4.2/tests/window/
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-02-06 05:53:20.000000 toga-core-0.4.2/tests/window/test_filtered_widget_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.847061 toga_core-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_core-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_core-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-06 06:43:32.847061 toga_core-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 06:43:02.000000 toga_core-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 06:43:02.000000 toga_core-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:32.847061 toga_core-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.807061 toga_core-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33715 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/plugins/image_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/list_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.819061 toga_core-0.4.3/src/toga/style/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40828 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.823061 toga_core-0.4.3/src/toga/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59957 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/src/toga_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_documentapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_windowset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_commandset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/test_location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.831061 toga_core-0.4.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/orange.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)   772491 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/photo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-72.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/sample-dummy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/sample.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/toga.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.831061 toga_core-0.4.3/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/pack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/pack/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_beeliza.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_column_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_flex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_row_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_rtl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/test_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/test_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20019 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20080 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/customize/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/customize/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.839061 toga_core-0.4.3/tests/testbed/subclassed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/widgets/canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_context_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_draw_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34610 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_webview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/window/
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/window/test_filtered_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/window/test_window.py
```

### Comparing `toga-core-0.4.2/LICENSE` & `toga_core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/PKG-INFO` & `toga_core-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 Metadata-Version: 2.1
 Name: toga-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python native, OS native GUI toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,mobile,web,macOS,cocoa,iOS,android,windows,winforms,linux,freeBSD,gtk,console,web
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
 Requires-Dist: travertino>=0.3.0
 Requires-Dist: importlib_metadata>=4.4.0; python_version <= "3.9"
 Provides-Extra: dev
-Requires-Dist: coverage[toml]==7.4.1; extra == "dev"
-Requires-Dist: Pillow==10.2.0; extra == "dev"
+Requires-Dist: coverage[toml]==7.5.1; extra == "dev"
+Requires-Dist: Pillow==10.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
-Requires-Dist: pre-commit==3.6.0; python_version >= "3.9" and extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.4; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 Requires-Dist: pytest-freezer==0.4.8; extra == "dev"
 Requires-Dist: setuptools-scm==8.0.4; extra == "dev"
-Requires-Dist: tox==4.12.1; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 Requires-Dist: typing-extensions==4.9.0; python_version < "3.10" and extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
-Requires-Dist: Pillow==10.2.0; extra == "docs"
+Requires-Dist: furo==2024.4.27; extra == "docs"
+Requires-Dist: Pillow==10.3.0; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx==7.3.7; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
-Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints==1.25.3; extra == "docs"
+Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.4.16; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints==2.1.0; extra == "docs"
 Requires-Dist: sphinx-csv-filter==0.4.1; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
 Toga
 ====
@@ -72,15 +75,15 @@
 
 Minimum requirements
 --------------------
 
 Toga requires **Python 3.8** or newer. Python 2 is not supported.
 
 Each backend also has specific requirements and pre-requisites. See the `platform
-documentation <https://toga.readthedocs.io/en/stable/reference/platforms.html>`__ for
+documentation <https://toga.readthedocs.io/en/latest/reference/platforms.html>`__ for
 details.
 
 Quickstart
 ----------
 
 To get a demonstration of the capabilities of Toga, run the following::
```

### Comparing `toga-core-0.4.2/README.rst` & `toga_core-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Minimum requirements
 --------------------
 
 Toga requires **Python 3.8** or newer. Python 2 is not supported.
 
 Each backend also has specific requirements and pre-requisites. See the `platform
-documentation <https://toga.readthedocs.io/en/stable/reference/platforms.html>`__ for
+documentation <https://toga.readthedocs.io/en/latest/reference/platforms.html>`__ for
 details.
 
 Quickstart
 ----------
 
 To get a demonstration of the capabilities of Toga, run the following::
```

### Comparing `toga-core-0.4.2/pyproject.toml` & `toga_core-0.4.3/pyproject.toml`

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
 dynamic = ["version"]
@@ -46,64 +46,71 @@
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
 dependencies = [
     "travertino >= 0.3.0",
     # limited to <=3.9 for the `group` argument for `entry_points()`
     "importlib_metadata >= 4.4.0; python_version <= '3.9'",
 ]
 
 [project.optional-dependencies]
-# Extras used by developers *of* briefcase are pinned to specific versions to
+# Extras used by developers *of* Toga are pinned to specific versions to
 # ensure environment consistency.
 dev = [
-    "coverage[toml] == 7.4.1",
-    "Pillow == 10.2.0",
+    "coverage[toml] == 7.5.1",
+    "Pillow == 10.3.0",
     # Pre-commit 3.6.0 deprecated support for Python 3.8
     "pre-commit == 3.5.0 ; python_version < '3.9'",
-    "pre-commit == 3.6.0 ; python_version >= '3.9'",
-    "pytest == 7.4.4",
-    "pytest-asyncio == 0.23.4",
+    "pre-commit == 3.7.0 ; python_version >= '3.9'",
+    "pytest == 8.2.0",
+    "pytest-asyncio == 0.23.6",
     "pytest-freezer == 0.4.8",
     "setuptools-scm == 8.0.4",
-    "tox == 4.12.1",
+    "tox == 4.15.0",
     # typing-extensions needed for TypeAlias added in Py 3.10
-    "typing-extensions == 4.9.0 ; python_version < '3.10'"
+    "typing-extensions == 4.9.0 ; python_version < '3.10'",
 ]
 docs = [
-    "furo == 2024.1.29",
-    "Pillow == 10.2.0",
+    "furo == 2024.4.27",
+    "Pillow == 10.3.0",
     "pyenchant == 3.2.2",
     # Sphinx 7.2 deprecated support for Python 3.8
     "sphinx == 7.1.2 ; python_version < '3.9'",
-    "sphinx == 7.2.6 ; python_version >= '3.9'",
+    "sphinx == 7.3.7 ; python_version >= '3.9'",
     "sphinx_tabs == 3.4.5",
-    "sphinx-autobuild == 2024.2.4",
-    "sphinx-autodoc-typehints == 1.25.3",
+    # Sphinx 2024.2.4 deprecated support for Python 3.8
+    "sphinx-autobuild == 2021.3.14 ; python_version < '3.9'",
+    "sphinx-autobuild == 2024.4.16 ; python_version >= '3.9'",
+    "sphinx-autodoc-typehints == 2.1.0",
     "sphinx-csv-filter == 0.4.1",
     "sphinx-copybutton == 0.5.2",
     "sphinx-toolbox == 3.5.0",
     "sphinxcontrib-spelling == 8.0.0",
 ]
 
 [project.urls]
 Homepage = "https://beeware.org/project/projects/libraries/toga/"
 Funding = "https://beeware.org/contributing/membership/"
-Documentation = "https://toga.readthedocs.io/en/latest/"
+Documentation = "https://toga.readthedocs.io/"
 Tracker = "https://github.com/beeware/toga/issues"
 Source = "https://github.com/beeware/toga"
+Changelog = "https://toga.readthedocs.io/en/stable/background/project/releases.html"
+
+[project.entry-points."toga.image_formats"]
+pil = "toga.plugins.image_formats.PILConverter"
 
 [tool.setuptools_scm]
 root = ".."
 
 [tool.coverage.run]
 parallel = true
 branch = true
@@ -117,7 +124,10 @@
 source = [
     "src/toga",
     "**/toga",
 ]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+filterwarnings = [
+    "error",
+]
```

### Comparing `toga-core-0.4.2/src/toga/__init__.py` & `toga_core-0.4.3/src/toga/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+import warnings
+
 from .app import App, DocumentApp, DocumentMainWindow, MainWindow
 
 # Resources
 from .colors import hsl, hsla, rgb, rgba
 from .command import Command, Group
 from .documents import Document
 from .fonts import Font
 from .icons import Icon
 from .images import Image
 from .keys import Key
-from .widgets.activityindicator import ActivityIndicator
+
+# Types
+from .types import LatLng
 
 # Widgets
+from .widgets.activityindicator import ActivityIndicator
 from .widgets.base import Widget
 from .widgets.box import Box
 from .widgets.button import Button
 from .widgets.canvas import Canvas
 from .widgets.dateinput import DateInput, DatePicker
 from .widgets.detailedlist import DetailedList
 from .widgets.divider import Divider
 from .widgets.imageview import ImageView
 from .widgets.label import Label
+from .widgets.mapview import MapPin, MapView
 from .widgets.multilinetextinput import MultilineTextInput
 from .widgets.numberinput import NumberInput
 from .widgets.optioncontainer import OptionContainer, OptionItem
 from .widgets.passwordinput import PasswordInput
 from .widgets.progressbar import ProgressBar
 from .widgets.scrollcontainer import ScrollContainer
 from .widgets.selection import Selection
@@ -33,15 +39,27 @@
 from .widgets.table import Table
 from .widgets.textinput import TextInput
 from .widgets.timeinput import TimeInput, TimePicker
 from .widgets.tree import Tree
 from .widgets.webview import WebView
 from .window import Window
 
+
+class NotImplementedWarning(RuntimeWarning):
+    # pytest.warns() requires that Warning() subclasses are constructed by passing a
+    # single argument (the warning message). Use a factory method to avoid reproducing
+    # the message format and the warn invocation.
+    @classmethod
+    def warn(self, platform, feature):
+        """Raise a warning that a feature isn't implemented on a platform."""
+        warnings.warn(NotImplementedWarning(f"[{platform}] Not implemented: {feature}"))
+
+
 __all__ = [
+    "NotImplementedWarning",
     # Applications
     "App",
     "DocumentApp",
     "MainWindow",
     "DocumentMainWindow",
     # Commands
     "Command",
@@ -50,28 +68,32 @@
     "Document",
     # Keys
     "Key",
     # Resources
     "hsl",
     "hsla",
     "rgb",
-    "rgba",  # Colors
+    "rgba",
     "Font",
     "Icon",
     "Image",
+    # Types
+    "LatLng",
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
+    "MapPin",
+    "MapView",
     "MultilineTextInput",
     "NumberInput",
     "OptionContainer",
     "OptionItem",
     "PasswordInput",
     "ProgressBar",
     "ScrollContainer",
```

### Comparing `toga-core-0.4.2/src/toga/app.py` & `toga_core-0.4.3/src/toga/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 from warnings import warn
 from weakref import WeakValueDictionary
 
 from toga.command import Command, CommandSet
 from toga.documents import Document
 from toga.handlers import wrapped_handler
 from toga.hardware.camera import Camera
+from toga.hardware.location import Location
 from toga.icons import Icon
 from toga.paths import Paths
 from toga.platform import get_platform_factory
+from toga.screens import Screen
 from toga.widgets.base import Widget
 from toga.window import Window
 
 if TYPE_CHECKING:
     from toga.icons import IconContent
 
 # Make sure deprecation warnings are shown by default
@@ -143,15 +145,15 @@
 
 class WidgetRegistry:
     # WidgetRegistry is implemented as a wrapper around a WeakValueDictionary, because
     # it provides a mapping from ID to widget. The mapping is weak so the registry
     # doesn't retain a strong reference to the widget, preventing memory cleanup.
     #
     # The lookup methods (__getitem__(), __iter__(), __len()__, keys(), items(), and
-    # values()) are all proxied to to underlying data store. Private methods exist for
+    # values()) are all proxied to underlying data store. Private methods exist for
     # internal use, but those methods shouldn't be used by end-users.
 
     def __init__(self, *args, **kwargs):
         self._registry = WeakValueDictionary(*args, **kwargs)
 
     def __len__(self) -> int:
         return len(self._registry)
@@ -302,15 +304,17 @@
 
     @property
     def _default_title(self) -> str:
         return self.doc.path.name
 
 
 class App:
-    app = None
+    #: The currently running :class:`~toga.App`. Since there can only be one running
+    #: Toga app in a process, this is available as a class property via ``toga.App.app``.
+    app: App = None
 
     def __init__(
         self,
         formal_name: str | None = None,
         app_id: str | None = None,
         app_name: str | None = None,
         *,
@@ -341,18 +345,16 @@
 
             #. If the ``__main__`` module is contained in a package, that package's name
                will be used.
             #. If the ``app_id`` argument was provided, its last segment will be used.
                For example, an ``app_id`` of ``com.example.my-app`` would yield a
                distribution name of ``my-app``.
             #. As a last resort, the name ``toga``.
-        :param icon: The :any:`icon <IconContent>` for the app. If not provided, Toga
-            will attempt to load an icon from ``resources/app_name``, where ``app_name``
-            is defined above. If no resource matching this name can be found, a warning
-            will be printed, and the app will fall back to a default icon.
+        :param icon: The :any:`icon <IconContent>` for the app. Defaults to
+            :attr:`toga.Icon.APP_ICON`.
         :param author: The person or organization to be credited as the author of the
             app. If not provided, the metadata key ``Author`` will be used.
         :param version: The version number of the app.  If not provided, the metadata
             key ``Version`` will be used.
         :param home_page: The URL of a web page for the app. Used in auto-generated help
             menu items. If not provided, the metadata key ``Home-page`` will be used.
         :param description: A brief (one line) description of the app. If not provided,
@@ -464,20 +466,18 @@
 
         # Get a platform factory.
         self.factory = get_platform_factory()
 
         # Instantiate the paths instance for this app.
         self._paths = Paths()
 
-        # If an icon (or icon name) has been explicitly provided, use it;
-        # otherwise, the icon will be based on the distribution name.
-        if icon:
-            self.icon = icon
+        if icon is None:
+            self.icon = Icon.APP_ICON
         else:
-            self.icon = f"resources/{app_name}"
+            self.icon = icon
 
         self.on_exit = on_exit
 
         # We need the command set to exist so that startup et al can add commands;
         # but we don't have an impl yet, so we can't set the on_change handler
         self._commands = CommandSet()
 
@@ -490,52 +490,19 @@
 
         self._create_impl()
 
         # Now that we have an impl, set the on_change handler for commands
         self.commands.on_change = self._impl.create_menus
 
     def _create_impl(self):
-        self.factory.App(interface=self)
-
-    @property
-    def paths(self) -> Paths:
-        """Paths for platform-appropriate locations on the user's file system.
-
-        Some platforms do not allow access to any file system location other than these
-        paths. Even when arbitrary file access is allowed, there are preferred locations
-        for each type of content.
-        """
-        return self._paths
-
-    @property
-    def camera(self) -> Camera:
-        """A representation of the device's camera (or cameras)."""
-        try:
-            return self._camera
-        except AttributeError:
-            # Instantiate the camera instance for this app on first access
-            # This will raise a exception if the platform doesn't implement
-            # the Camera API.
-            self._camera = Camera(self)
-        return self._camera
+        return self.factory.App(interface=self)
 
-    @property
-    def name(self) -> str:
-        """**DEPRECATED** – Use :any:`formal_name`."""
-        warn(
-            "App.name is deprecated. Use formal_name instead",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self._formal_name
-
-    @property
-    def formal_name(self) -> str:
-        """The human-readable name of the app (read-only)."""
-        return self._formal_name
+    ######################################################################
+    # App properties
+    ######################################################################
 
     @property
     def app_name(self) -> str:
         """The name of the distribution used to load metadata with
         :any:`importlib.metadata` (read-only)."""
         return self._app_name
 
@@ -549,54 +516,191 @@
     @property
     def author(self) -> str | None:
         """The person or organization to be credited as the author of the app
         (read-only)."""
         return self._author
 
     @property
-    def version(self) -> str | None:
-        """The version number of the app (read-only)."""
-        return self._version
+    def description(self) -> str | None:
+        """A brief (one line) description of the app (read-only)."""
+        return self._description
+
+    @property
+    def formal_name(self) -> str:
+        """The human-readable name of the app (read-only)."""
+        return self._formal_name
 
     @property
     def home_page(self) -> str | None:
         """The URL of a web page for the app (read-only). Used in auto-generated help
         menu items."""
         return self._home_page
 
     @property
-    def description(self) -> str | None:
-        """A brief (one line) description of the app (read-only)."""
-        return self._description
+    def icon(self) -> Icon:
+        """The Icon for the app.
+
+        Can be specified as any valid :any:`icon content <IconContent>`.
+        """
+        return self._icon
+
+    @icon.setter
+    def icon(self, icon_or_name: IconContent) -> None:
+        if isinstance(icon_or_name, Icon):
+            self._icon = icon_or_name
+        else:
+            self._icon = Icon(icon_or_name)
+
+        try:
+            self._impl.set_icon(self._icon)
+        except AttributeError:
+            # The first time the icon is set, it is *before* the impl has been created,
+            # so that the app instance can be instantiated with the correct icon.
+            pass
 
     @property
     def id(self) -> str:
         """**DEPRECATED** – Use :any:`app_id`."""
         warn(
             "App.id is deprecated. Use app_id instead", DeprecationWarning, stacklevel=2
         )
         return self._app_id
 
     @property
-    def icon(self) -> Icon:
-        """The Icon for the app.
+    def version(self) -> str | None:
+        """The version number of the app (read-only)."""
+        return self._version
 
-        Can be specified as any valid :any:`icon content <IconContent>`.
+    ######################################################################
+    # App lifecycle
+    ######################################################################
+
+    def add_background_task(self, handler: BackgroundTask) -> None:
+        """Schedule a task to run in the background.
+
+        Schedules a coroutine or a generator to run in the background. Control
+        will be returned to the event loop during await or yield statements,
+        respectively. Use this to run background tasks without blocking the
+        GUI. If a regular callable is passed, it will be called as is and will
+        block the GUI until the call returns.
 
-        When setting the icon, you can provide either an :any:`Icon` instance, or a
-        path that will be passed to the ``Icon`` constructor.
+        :param handler: A coroutine, generator or callable.
         """
-        return self._icon
+        self.loop.call_soon_threadsafe(wrapped_handler(self, handler))
 
-    @icon.setter
-    def icon(self, icon_or_name: IconContent | None) -> None:
-        if isinstance(icon_or_name, Icon):
-            self._icon = icon_or_name
-        else:
-            self._icon = Icon(icon_or_name)
+    def exit(self) -> None:
+        """Exit the application gracefully.
+
+        This *does not* invoke the ``on_exit`` handler; the app will be immediately
+        and unconditionally closed.
+        """
+        self._impl.exit()
+
+    @property
+    def loop(self) -> asyncio.AbstractEventLoop:
+        """The `event loop
+        <https://docs.python.org/3/library/asyncio-eventloop.html>`__ of the app's main
+        thread (read-only)."""
+        return self._impl.loop
+
+    def main_loop(self) -> None:
+        """Start the application.
+
+        On desktop platforms, this method will block until the application has exited.
+        On mobile and web platforms, it returns immediately.
+        """
+        # Modify signal handlers to make sure Ctrl-C is caught and handled.
+        signal.signal(signal.SIGINT, signal.SIG_DFL)
+
+        self._impl.main_loop()
+
+    @property
+    def main_window(self) -> MainWindow:
+        """The main window for the app."""
+        return self._main_window
+
+    @main_window.setter
+    def main_window(self, window: MainWindow) -> None:
+        self._main_window = window
+        self._impl.set_main_window(window)
+
+    def _verify_startup(self):
+        if not isinstance(self.main_window, MainWindow):
+            raise ValueError(
+                "Application does not have a main window. "
+                "Does your startup() method assign a value to self.main_window?"
+            )
+
+    def _startup(self):
+        # This is a wrapper around the user's startup method that performs any
+        # post-setup validation.
+        self.startup()
+        self._verify_startup()
+
+    def startup(self) -> None:
+        """Create and show the main window for the application.
+
+        Subclasses can override this method to define customized startup behavior;
+        however, any override *must* ensure the :any:`main_window` has been assigned
+        before it returns.
+        """
+        self.main_window = MainWindow(title=self.formal_name, id="main")
+
+        if self._startup_method:
+            self.main_window.content = self._startup_method(self)
+
+        self.main_window.show()
+
+    ######################################################################
+    # App resources
+    ######################################################################
+
+    @property
+    def camera(self) -> Camera:
+        """A representation of the device's camera (or cameras)."""
+        try:
+            return self._camera
+        except AttributeError:
+            # Instantiate the camera instance for this app on first access
+            # This will raise an exception if the platform doesn't implement
+            # the Camera API.
+            self._camera = Camera(self)
+        return self._camera
+
+    @property
+    def commands(self) -> MutableSet[Command]:
+        """The commands available in the app."""
+        return self._commands
+
+    @property
+    def location(self) -> Location:
+        """A representation of the device's location service."""
+        try:
+            return self._location
+        except AttributeError:
+            # Instantiate the location service for this app on first access
+            # This will raise an exception if the platform doesn't implement
+            # the Location API.
+            self._location = Location(self)
+        return self._location
+
+    @property
+    def paths(self) -> Paths:
+        """Paths for platform-appropriate locations on the user's file system.
+
+        Some platforms do not allow access to any file system location other than these
+        paths. Even when arbitrary file access is allowed, there are preferred locations
+        for each type of content.
+        """
+        return self._paths
+
+    @property
+    def screens(self) -> list[Screen]:
+        """Returns a list of available screens."""
+        return [screen.interface for screen in self._impl.get_screens()]
 
     @property
     def widgets(self) -> Mapping[str, Widget]:
         """The widgets managed by the app, over all windows.
 
         Can be used to look up widgets by ID over the entire app (e.g.,
         ``app.widgets["my_id"]``).
@@ -610,55 +714,76 @@
     @property
     def windows(self) -> Collection[Window]:
         """The windows managed by the app. Windows are automatically added to the app
         when they are created, and removed when they are closed."""
         return self._windows
 
     ######################################################################
-    # 2023-10: Backwards compatibility
+    # App capabilities
     ######################################################################
 
-    # Support WindowSet __iadd__ and __isub__
-    @windows.setter
-    def windows(self, windows):
-        if windows is not self._windows:
-            raise AttributeError("can't set attribute 'windows'")
+    def about(self) -> None:
+        """Display the About dialog for the app.
+
+        Default implementation shows a platform-appropriate about dialog using app
+        metadata. Override if you want to display a custom About dialog.
+        """
+        self._impl.show_about_dialog()
+
+    def beep(self) -> None:
+        """Play the default system notification sound."""
+        self._impl.beep()
+
+    def visit_homepage(self) -> None:
+        """Open the application's :any:`home_page` in the default browser.
+
+        If the :any:`home_page` is ``None``, this is a no-op.
+        """
+        if self.home_page is not None:
+            webbrowser.open(self.home_page)
 
     ######################################################################
-    # End backwards compatibility
+    # Cursor control
     ######################################################################
 
-    @property
-    def commands(self) -> MutableSet[Command]:
-        """The commands available in the app."""
-        return self._commands
+    def hide_cursor(self) -> None:
+        """Hide cursor from view."""
+        self._impl.hide_cursor()
 
-    @property
-    def main_window(self) -> MainWindow:
-        """The main window for the app."""
-        return self._main_window
+    def show_cursor(self) -> None:
+        """Make the cursor visible."""
+        self._impl.show_cursor()
 
-    @main_window.setter
-    def main_window(self, window: MainWindow) -> None:
-        self._main_window = window
-        self._impl.set_main_window(window)
+    ######################################################################
+    # Window control
+    ######################################################################
 
     @property
     def current_window(self) -> Window | None:
         """Return the currently active window."""
         window = self._impl.get_current_window()
         if window is None:
             return None
         return window.interface
 
     @current_window.setter
     def current_window(self, window: Window):
         """Set a window into current active focus."""
         self._impl.set_current_window(window)
 
+    ######################################################################
+    # Full screen control
+    ######################################################################
+
+    def exit_full_screen(self) -> None:
+        """Exit full screen mode."""
+        if self.is_full_screen:
+            self._impl.exit_full_screen(self._full_screen_windows)
+            self._full_screen_windows = None
+
     @property
     def is_full_screen(self) -> bool:
         """Is the app currently in full screen mode?"""
         return self._full_screen_windows is not None
 
     def set_full_screen(self, *windows: Window) -> None:
         """Make one or more windows full screen.
@@ -672,126 +797,54 @@
             exit full screen mode.
         """
         self.exit_full_screen()
         if windows:
             self._impl.enter_full_screen(windows)
             self._full_screen_windows = windows
 
-    def exit_full_screen(self) -> None:
-        """Exit full screen mode."""
-        if self.is_full_screen:
-            self._impl.exit_full_screen(self._full_screen_windows)
-            self._full_screen_windows = None
-
-    def show_cursor(self) -> None:
-        """Make the cursor visible."""
-        self._impl.show_cursor()
-
-    def hide_cursor(self) -> None:
-        """Hide cursor from view."""
-        self._impl.hide_cursor()
-
-    def startup(self) -> None:
-        """Create and show the main window for the application.
-
-        Subclasses can override this method to define customized startup behavior;
-        however, any override *must* ensure the :any:`main_window` has been assigned
-        before it returns.
-        """
-        self.main_window = MainWindow(title=self.formal_name, id="main")
-
-        if self._startup_method:
-            self.main_window.content = self._startup_method(self)
-
-        self.main_window.show()
-
-    def _startup(self):
-        # This is a wrapper around the user's startup method that performs any
-        # post-setup validation.
-        self.startup()
-        self._verify_startup()
-
-    def _verify_startup(self):
-        if not isinstance(self.main_window, MainWindow):
-            raise ValueError(
-                "Application does not have a main window. "
-                "Does your startup() method assign a value to self.main_window?"
-            )
-
-    def about(self) -> None:
-        """Display the About dialog for the app.
-
-        Default implementation shows a platform-appropriate about dialog using app
-        metadata. Override if you want to display a custom About dialog.
-        """
-        self._impl.show_about_dialog()
-
-    def visit_homepage(self) -> None:
-        """Open the application's :any:`home_page` in the default browser.
-
-        If the :any:`home_page` is ``None``, this is a no-op.
-        """
-        if self.home_page is not None:
-            webbrowser.open(self.home_page)
-
-    def beep(self) -> None:
-        """Play the default system notification sound."""
-        self._impl.beep()
-
-    def main_loop(self) -> None:
-        """Start the application.
-
-        On desktop platforms, this method will block until the application has exited.
-        On mobile and web platforms, it returns immediately.
-        """
-        # Modify signal handlers to make sure Ctrl-C is caught and handled.
-        signal.signal(signal.SIGINT, signal.SIG_DFL)
-
-        self._impl.main_loop()
-
-    def exit(self) -> None:
-        """Exit the application gracefully.
-
-        This *does not* invoke the ``on_exit`` handler; the app will be immediately
-        and unconditionally closed.
-        """
-        self._impl.exit()
+    ######################################################################
+    # App events
+    ######################################################################
 
     @property
     def on_exit(self) -> OnExitHandler:
         """The handler to invoke if the user attempts to exit the app."""
         return self._on_exit
 
     @on_exit.setter
     def on_exit(self, handler: OnExitHandler | None) -> None:
         def cleanup(app, should_exit):
             if should_exit or handler is None:
                 app.exit()
 
         self._on_exit = wrapped_handler(self, handler, cleanup=cleanup)
 
-    @property
-    def loop(self) -> asyncio.AbstractEventLoop:
-        """The `event loop
-        <https://docs.python.org/3/library/asyncio-eventloop.html>`__ of the app's main
-        thread (read-only)."""
-        return self._impl.loop
+    ######################################################################
+    # 2023-10: Backwards compatibility
+    ######################################################################
 
-    def add_background_task(self, handler: BackgroundTask) -> None:
-        """Schedule a task to run in the background.
+    @property
+    def name(self) -> str:
+        """**DEPRECATED** – Use :any:`formal_name`."""
+        warn(
+            "App.name is deprecated. Use formal_name instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._formal_name
 
-        Schedules a coroutine or a generator to run in the background. Control
-        will be returned to the event loop during await or yield statements,
-        respectively. Use this to run background tasks without blocking the
-        GUI. If a regular callable is passed, it will be called as is and will
-        block the GUI until the call returns.
+    # Support WindowSet __iadd__ and __isub__
+    @windows.setter
+    def windows(self, windows):
+        if windows is not self._windows:
+            raise AttributeError("can't set attribute 'windows'")
 
-        :param handler: A coroutine, generator or callable.
-        """
-        self.loop.call_soon_threadsafe(wrapped_handler(self, handler))
+    ######################################################################
+    # End backwards compatibility
+    ######################################################################
 
 
 class DocumentApp(App):
     def __init__(
         self,
         formal_name: str | None = None,
         app_id: str | None = None,
@@ -807,15 +860,15 @@
         on_exit: OnExitHandler | None = None,
         id=None,  # DEPRECATED
     ):
         """Create a document-based application.
 
         A document-based application is the same as a normal application, with the
         exception that there is no main window. Instead, each document managed by the
-        app will create and manage it's own window (or windows).
+        app will create and manage its own window (or windows).
 
         :param document_types: Initial :any:`document_types` mapping.
         """
         if document_types is None:
             raise ValueError("A document must manage at least one document type.")
 
         self._document_types = document_types
@@ -865,15 +918,15 @@
         """
 
     def _open(self, path):
         """Internal utility method; open a new document in this app, and shows the document.
 
         :param path: The path to the document to be opened.
         :raises ValueError: If the document is of a type that can't be opened. Backends can
-            suppress this exception if necessary to presere platform-native behavior.
+            suppress this exception if necessary to preserve platform-native behavior.
         """
         try:
             DocType = self.document_types[path.suffix[1:]]
         except KeyError:
             raise ValueError(f"Don't know how to open documents of type {path.suffix}")
         else:
             document = DocType(path, app=self)
```

### Comparing `toga-core-0.4.2/src/toga/command.py` & `toga_core-0.4.3/src/toga/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         text: str,
         *,
         parent: Group | None = None,
         section: int = 0,
         order: int = 0,
     ):
         """
-        An collection of commands to display together.
+        A collection of commands to display together.
 
         :param text: A label for the group.
         :param parent: The parent of this group; use ``None`` to make a root group.
         :param section: The section where the group should appear within its parent. A
             section cannot be specified unless a parent is also specified.
         :param order: The position where the group should appear within its section.
             If multiple items have the same group, section and order, they will be
@@ -199,15 +199,15 @@
         self.tooltip = tooltip
         self.icon = icon
 
         self.group = group
         self.section = section
         self.order = order
 
-        self.action = wrapped_handler(self, action)
+        self.action = action
 
         self.factory = get_platform_factory()
         self._impl = self.factory.Command(interface=self)
 
         self.enabled = enabled
 
     @property
@@ -240,14 +240,27 @@
     @icon.setter
     def icon(self, icon_or_name: IconContent | None):
         if isinstance(icon_or_name, Icon) or icon_or_name is None:
             self._icon = icon_or_name
         else:
             self._icon = Icon(icon_or_name)
 
+    @property
+    def action(self) -> ActionHandler | None:
+        """The Action attached to the command."""
+        return self._action
+
+    @action.setter
+    def action(self, action: ActionHandler | None):
+        """Set the action attached to the command
+
+        Needs to be a valid ActionHandler or ``None``
+        """
+        self._action = wrapped_handler(self, action)
+
     def __lt__(self, other: Any) -> bool:
         if not isinstance(other, (Group, Command)):
             return False
         return self.key < other.key
 
     def __gt__(self, other: Any) -> bool:
         if not isinstance(other, (Group, Command)):
@@ -278,22 +291,15 @@
         if isinstance(other, Separator):
             return self.group == other.group
         return False
 
 
 class CommandSetChangeHandler(Protocol):
     def __call__(self) -> None:
-        """A handler that will be invoked when a Command or Group is added to the CommandSet.
-
-        .. note::
-            ``**kwargs`` ensures compatibility with additional arguments
-            introduced in future versions.
-
-        :return: Nothing
-        """
+        """A handler that will be invoked when a Command or Group is added to the CommandSet."""
         ...
 
 
 class CommandSet:
     def __init__(
         self,
         on_change: CommandSetChangeHandler = None,
```

### Comparing `toga-core-0.4.2/src/toga/constants/__init__.py` & `toga_core-0.4.3/src/toga/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/documents.py` & `toga_core-0.4.3/src/toga/documents.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/fonts.py` & `toga_core-0.4.3/src/toga/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/handlers.py` & `toga_core-0.4.3/src/toga/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,7 +159,11 @@
 
     __lt__ = __bool__
     __le__ = __bool__
     __eq__ = __bool__
     __ne__ = __bool__
     __gt__ = __bool__
     __ge__ = __bool__
+
+
+class PermissionResult(AsyncResult):
+    RESULT_TYPE = "permission"
```

### Comparing `toga-core-0.4.2/src/toga/hardware/camera.py` & `toga_core-0.4.3/src/toga/hardware/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from toga.constants import FlashMode
-from toga.handlers import AsyncResult
+from toga.handlers import AsyncResult, PermissionResult
 from toga.platform import get_platform_factory
 
 if TYPE_CHECKING:
     from toga.app import App
 
 
-class PermissionResult(AsyncResult):
-    RESULT_TYPE = "permission"
-
-
 class PhotoResult(AsyncResult):
     RESULT_TYPE = "photo"
 
 
 class CameraDevice:
     def __init__(self, impl):
         self._impl = impl
@@ -72,15 +68,15 @@
 
         If permission has already been granted, this will return without prompting the
         user.
 
         **This is an asynchronous method**. If you invoke this method in synchronous
         context, it will start the process of requesting permissions, but will return
         *immediately*. The return value can be awaited in an asynchronous context, but
-        cannot be compared directly.
+        cannot be used directly.
 
         :returns: An asynchronous result; when awaited, returns True if the app has
             permission to take a photo; False otherwise.
         """
         result = PermissionResult(None)
 
         if has_permission := self.has_permission:
@@ -104,20 +100,21 @@
 
         If the platform requires permission to access the camera, and the user hasn't
         previously provided that permission, this will cause permission to be requested.
 
         **This is an asynchronous method**. If you invoke this method in synchronous
         context, it will start the process of taking a photo, but will return
         *immediately*. The return value can be awaited in an asynchronous context, but
-        cannot be compared directly.
+        cannot be used directly.
 
         :param device: The initial camera device to use. If a device is *not* specified,
             a default camera will be used. Depending on the hardware available, the user
             may be able to change the camera used to capture the image at runtime.
         :param flash: The initial flash mode to use; defaults to "auto". Depending on
             the hardware available, this may be modified by the user at runtime.
         :returns: An asynchronous result; when awaited, returns the :any:`toga.Image`
             captured by the camera, or ``None`` if the photo was  cancelled.
+        :raises PermissionError: if the app does not have permission to use the camera.
         """
         photo = PhotoResult(None)
         self._impl.take_photo(photo, device=device, flash=flash)
         return photo
```

### Comparing `toga-core-0.4.2/src/toga/keys.py` & `toga_core-0.4.3/src/toga/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,25 @@
     F18 = "<f18>"
     F19 = "<f19>"
 
     EJECT = "<eject>"
 
     HOME = "<home>"
     END = "<end>"
+    INSERT = "<insert>"
     DELETE = "<delete>"
     PAGE_UP = "<pg up>"
     PAGE_DOWN = "<pg dn>"
 
     UP = "<up>"
     DOWN = "<down>"
     LEFT = "<left>"
     RIGHT = "<right>"
 
+    NUMLOCK = "<num lock>"
     NUMPAD_0 = "numpad:0"
     NUMPAD_1 = "numpad:1"
     NUMPAD_2 = "numpad:2"
     NUMPAD_3 = "numpad:3"
     NUMPAD_4 = "numpad:4"
     NUMPAD_5 = "numpad:5"
     NUMPAD_6 = "numpad:6"
@@ -143,14 +145,19 @@
     NUMPAD_DIVIDE = "numpad:/"
     NUMPAD_ENTER = "numpad:enter"
     NUMPAD_EQUAL = "numpad:="
     NUMPAD_MINUS = "numpad:-"
     NUMPAD_MULTIPLY = "numpad:*"
     NUMPAD_PLUS = "numpad:+"
 
+    SCROLLLOCK = "<scroll lock>"
+    BEGIN = "<begin>"
+    MENU = "<menu>"
+    PAUSE = "<pause>"
+
     def is_printable(self) -> bool:
         """Does pressing the key result in a printable character?"""
         return not (self.value.startswith("<") and self.value.endswith(">"))
 
     def __add__(self, other):
         """Allow two Keys to be concatenated, or a string to be concatenated to a Key.
```

### Comparing `toga-core-0.4.2/src/toga/paths.py` & `toga_core-0.4.3/src/toga/paths.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/platform.py` & `toga_core-0.4.3/src/toga/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,53 +36,54 @@
     else:
         return _TOGA_PLATFORMS.get(sys.platform)
 
 
 current_platform = get_current_platform()
 
 
+def find_backends():
+    # As of Setuptools 65.5, entry points are returned duplicated if the
+    # package is installed editable. Use a set to ensure that each entry point
+    # is only returned once.
+    # See https://github.com/pypa/setuptools/issues/3649
+    return sorted(set(entry_points(group="toga.backends")))
+
+
 @lru_cache(maxsize=1)
 def get_platform_factory():
     """Determine the current host platform and import the platform factory.
 
     If the ``TOGA_BACKEND`` environment variable is set, the factory will be loaded
     from that module.
 
     Raises :any:`RuntimeError` if an appropriate host platform cannot be identified.
 
     :returns: The factory for the host platform.
     """
-    toga_backends = entry_points(group="toga.backends")
-    if not toga_backends:
-        raise RuntimeError("No Toga backend could be loaded.")
-
     backend_value = os.environ.get("TOGA_BACKEND")
     if backend_value:
         try:
             factory = importlib.import_module(f"{backend_value}.factory")
         except ModuleNotFoundError as e:
             toga_backends_values = ", ".join(
-                [f"{backend.value!r}" for backend in toga_backends]
+                [f"{backend.value!r}" for backend in find_backends()]
             )
             # Android doesn't report Python exception chains in crashes
             # (https://github.com/chaquo/chaquopy/issues/890), so include the original
             # exception message in case the backend does exist but throws a
             # ModuleNotFoundError from one of its internal imports.
             raise RuntimeError(
                 f"The backend specified by TOGA_BACKEND ({backend_value!r}) could "
                 f"not be loaded ({e}). It should be one of: {toga_backends_values}."
             )
     else:
-        # As of Setuptools 65.5, entry points are returned duplicated if the
-        # package is installed editable. Use a set to ensure that each entry point
-        # is only returned once.
-        # See https://github.com/pypa/setuptools/issues/3649
-        toga_backends = sorted(set(toga_backends))
-
-        if len(toga_backends) == 1:
+        toga_backends = find_backends()
+        if len(toga_backends) == 0:
+            raise RuntimeError("No Toga backend could be loaded.")
+        elif len(toga_backends) == 1:
             backend = toga_backends[0]
         else:
             # multiple backends are installed: choose the one that matches the host platform
             matching_backends = [
                 backend for backend in toga_backends if backend.name == current_platform
             ]
             if len(matching_backends) == 0:
```

### Comparing `toga-core-0.4.2/src/toga/sources/accessors.py` & `toga_core-0.4.3/src/toga/sources/accessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ) -> list[str]:
     """Convert a list of headings (with accessor overrides) to a finalised list of
     accessors.
 
     :param headings: The list of headings.
     :param accessors: The list of accessor overrides. Can be specified as:
 
-        * A list the same length as headings. Each entry in the list is a a string that
+        * A list the same length as headings. Each entry in the list is a string that
           is the override name for the accessor, or :any:`None` if the default accessor
           for the heading at that index should be used.
         * A dictionary mapping heading names to accessor names. If a heading name isn't
           present in the dictionary, the default accessor will be used.
 
     :returns: The final list of accessors.
     """
```

### Comparing `toga-core-0.4.2/src/toga/sources/base.py` & `toga_core-0.4.3/src/toga/sources/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,19 +25,15 @@
         """An item has been removed from the data source.
 
         :param index: The 0-index position in the data.
         :param item: The data object that was added.
         """
 
     def clear(self):
-        """All items have been removed from the data source.
-
-        :param index: The 0-index position in the data.
-        :param item: The data object that was added.
-        """
+        """All items have been removed from the data source."""
 
 
 class Source:
     """A base class for data sources, providing an implementation of data notifications."""
 
     def __init__(self):
         self._listeners = []
```

### Comparing `toga-core-0.4.2/src/toga/sources/list_source.py` & `toga_core-0.4.3/src/toga/sources/list_source.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/sources/tree_source.py` & `toga_core-0.4.3/src/toga/sources/tree_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def __delitem__(self, index: int):
         if self._children is None:
             raise ValueError(f"{self} is a leaf node")
 
         child = self._children[index]
         del self._children[index]
 
-        # Child isn't part of this source, or a child of this node any more.
+        # Child isn't part of this source, or a child of this node anymore.
         child._parent = None
         child._source = None
 
         self._source.notify("remove", parent=self, index=index, item=child)
 
     def __len__(self) -> int:
         if self.can_have_children():
```

### Comparing `toga-core-0.4.2/src/toga/style/applicator.py` & `toga_core-0.4.3/src/toga/style/applicator.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/style/pack.py` & `toga_core-0.4.3/src/toga/style/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,26 +47,26 @@
 ######################################################################
 # Declaration choices
 ######################################################################
 
 DISPLAY_CHOICES = Choices(PACK, NONE)
 VISIBILITY_CHOICES = Choices(VISIBLE, HIDDEN)
 DIRECTION_CHOICES = Choices(ROW, COLUMN)
-ALIGNMENT_CHOICES = Choices(LEFT, RIGHT, TOP, BOTTOM, CENTER, default=True)
+ALIGNMENT_CHOICES = Choices(LEFT, RIGHT, TOP, BOTTOM, CENTER)
 
 SIZE_CHOICES = Choices(NONE, integer=True)
 FLEX_CHOICES = Choices(number=True)
 
 PADDING_CHOICES = Choices(integer=True)
 
-TEXT_ALIGN_CHOICES = Choices(LEFT, RIGHT, CENTER, JUSTIFY, default=True)
+TEXT_ALIGN_CHOICES = Choices(LEFT, RIGHT, CENTER, JUSTIFY)
 TEXT_DIRECTION_CHOICES = Choices(RTL, LTR)
 
-COLOR_CHOICES = Choices(color=True, default=True)
-BACKGROUND_COLOR_CHOICES = Choices(TRANSPARENT, color=True, default=True)
+COLOR_CHOICES = Choices(color=True)
+BACKGROUND_COLOR_CHOICES = Choices(TRANSPARENT, color=True)
 
 FONT_FAMILY_CHOICES = Choices(*SYSTEM_DEFAULT_FONTS, string=True)
 FONT_STYLE_CHOICES = Choices(*FONT_STYLES)
 FONT_VARIANT_CHOICES = Choices(*FONT_VARIANTS)
 FONT_WEIGHT_CHOICES = Choices(*FONT_WEIGHTS)
 FONT_SIZE_CHOICES = Choices(integer=True)
 
@@ -81,15 +81,15 @@
     _depth = -1
 
     def _debug(self, *args):  # pragma: no cover
         print("    " * self.__class__._depth, *args)
 
     @property
     def _hidden(self):
-        "Does this style declaration define a object that should be hidden"
+        """Does this style declaration define an object that should be hidden"""
         return self.visibility == HIDDEN
 
     def apply(self, prop, value):
         if self._applicator:
             if prop == "text_align":
                 if value is None:
                     if self.text_direction == RTL:
```

### Comparing `toga-core-0.4.2/src/toga/validators.py` & `toga_core-0.4.3/src/toga/validators.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/activityindicator.py` & `toga_core-0.4.3/src/toga/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/base.py` & `toga_core-0.4.3/src/toga/widgets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     @property
     def tab_index(self) -> int | None:
         """The position of the widget in the focus chain for the window.
 
         .. note::
 
             This is a beta feature. The ``tab_index`` API may change in
-            future.
+            the future.
         """
         return self._impl.get_tab_index()
 
     @tab_index.setter
     def tab_index(self, tab_index: int) -> None:
         self._impl.set_tab_index(tab_index)
```

### Comparing `toga-core-0.4.2/src/toga/widgets/box.py` & `toga_core-0.4.3/src/toga/widgets/box.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/button.py` & `toga_core-0.4.3/src/toga/widgets/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,16 @@
     from toga.icons import IconContent
 
 
 class OnPressHandler(Protocol):
     def __call__(self, widget: Button, **kwargs: Any) -> None:
         """A handler that will be invoked when a button is pressed.
 
-        .. note::
-            ``**kwargs`` ensures compatibility with additional arguments
-            introduced in future versions.
-
         :param widget: The button that was pressed.
+        :param kwargs: Ensures compatibility with arguments added in future versions.
         """
         ...
 
 
 class Button(Widget):
     def __init__(
         self,
```

### Comparing `toga-core-0.4.2/src/toga/widgets/canvas.py` & `toga_core-0.4.3/src/toga/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     def line_dash(self, value: list[float] | None):
         self._line_dash = value
 
     ###########################################################################
     # 2023-07 Backwards incompatibility
     ###########################################################################
 
-    # `context.stroke()` used to be a context managger, but is now a primitive.
+    # `context.stroke()` used to be a context manager, but is now a primitive.
     # If you try to use the Stroke drawing object as a context, raise an exception.
     def __enter__(self):
         raise RuntimeError("Context.stroke() has been renamed Context.Stroke().")
 
     def __exit__(self):  # pragma: no cover
         # This method is required to make the object a context manager, but as the
         # __enter__ method raises an exception, the __exit__ can't be called.
@@ -1449,15 +1449,17 @@
     # As image
     ###########################################################################
 
     def as_image(self, format: type[ImageT] = toga.Image) -> ImageT:
         """Render the canvas as an image.
 
         :param format: Format to provide. Defaults to :class:`~toga.images.Image`; also
-            supports :class:`PIL.Image.Image` if Pillow is installed
+            supports :any:`PIL.Image.Image` if Pillow is installed, as well as any image
+            types defined by installed :doc:`image format plugins
+            </reference/plugins/image_formats>`
         :returns: The canvas as an image of the specified type.
         """
         return toga.Image(self._impl.get_image_data()).as_format(format)
 
     ###########################################################################
     # 2023-07 Backwards compatibility
     ###########################################################################
```

### Comparing `toga-core-0.4.2/src/toga/widgets/dateinput.py` & `toga_core-0.4.3/src/toga/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/detailedlist.py` & `toga_core-0.4.3/src/toga/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/divider.py` & `toga_core-0.4.3/src/toga/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/imageview.py` & `toga_core-0.4.3/src/toga/widgets/imageview.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,11 +125,13 @@
         self._impl.set_image(self._image)
         self.refresh()
 
     def as_image(self, format: type[ImageT] = toga.Image) -> ImageT:
         """Return the image in the specified format.
 
         :param format: Format to provide. Defaults to :class:`~toga.images.Image`; also
-            supports :any:`PIL.Image.Image` if Pillow is installed.
+            supports :any:`PIL.Image.Image` if Pillow is installed, as well as any image
+            types defined by installed :doc:`image format plugins
+            </reference/plugins/image_formats>`.
         :returns: The image in the specified format.
         """
         return self.image.as_format(format)
```

### Comparing `toga-core-0.4.2/src/toga/widgets/label.py` & `toga_core-0.4.3/src/toga/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/multilinetextinput.py` & `toga_core-0.4.3/src/toga/widgets/multilinetextinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         :param id: The ID for the widget.
         :param style: A style object. If no style is provided, a default style
             will be applied to the widget.
         :param value: The initial content to display in the widget.
         :param readonly: Can the value of the widget be modified by the user?
         :param placeholder: The content to display as a placeholder when
             there is no user content to display.
-        :param on_change: A handler that will be invoked when the the value of
+        :param on_change: A handler that will be invoked when the value of
             the widget changes.
         """
 
         super().__init__(id=id, style=style)
 
         # Create a platform specific implementation of a MultilineTextInput
         self._impl = self.factory.MultilineTextInput(interface=self)
```

### Comparing `toga-core-0.4.2/src/toga/widgets/numberinput.py` & `toga_core-0.4.3/src/toga/widgets/numberinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             the widget's current value.
         :param min: If provided, :any:`value` will be guaranteed to be greater than or
             equal to this minimum.
         :param max: If provided, :any:`value` will be guaranteed to be less than or
             equal to this maximum.
         :param value: The initial value for the widget.
         :param readonly: Can the value of the widget be modified by the user?
-        :param on_change: A handler that will be invoked when the the value of the
+        :param on_change: A handler that will be invoked when the value of the
             widget changes.
         :param min_value: **DEPRECATED**; alias of ``min``.
         :param max_value: **DEPRECATED**; alias of ``max``.
         """
         super().__init__(id=id, style=style)
 
         ######################################################################
```

### Comparing `toga-core-0.4.2/src/toga/widgets/optioncontainer.py` & `toga_core-0.4.3/src/toga/widgets/optioncontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,16 @@
     )
 
 
 class OnSelectHandler(Protocol):
     def __call__(self, widget: OptionContainer, **kwargs: Any) -> None:
         """A handler that will be invoked when a new tab is selected in the OptionContainer.
 
-        .. note::
-            ``**kwargs`` ensures compatibility with additional arguments
-            introduced in future versions.
-
         :param widget: The OptionContainer that had a selection change.
+        :param kwargs: Ensures compatibility with arguments added in future versions.
         """
         ...
 
 
 class OptionItem:
     def __init__(
         self,
@@ -82,15 +79,15 @@
 
         Returns ``None`` if the tab isn't currently part of an OptionContainer.
         """
         return self._interface
 
     @property
     def enabled(self) -> bool:
-        "Is the panel of content available for selection?"
+        """Is the panel of content available for selection?"""
         try:
             return self._enabled
         except AttributeError:
             return self._interface._impl.is_option_enabled(self.index)
 
     @enabled.setter
     def enabled(self, value):
@@ -104,15 +101,15 @@
             ):
                 raise ValueError("The currently selected tab cannot be disabled.")
 
             self._interface._impl.set_option_enabled(self.index, enable)
 
     @property
     def text(self) -> str:
-        "The label for the tab of content."
+        """The label for the tab of content."""
         try:
             return self._text
         except AttributeError:
             return self._interface._impl.get_option_text(self.index)
 
     @text.setter
     def text(self, value):
@@ -381,15 +378,15 @@
 
 class OptionContainer(Widget):
     def __init__(
         self,
         id=None,
         style=None,
         content: list[OptionContainerContent] | None = None,
-        on_select: OnSelectHandler | None = None,
+        on_select: toga.widgets.optioncontainer.OnSelectHandler | None = None,
     ):
         """Create a new OptionContainer.
 
         :param id: The ID for the widget.
         :param style: A style object. If no style is provided, a default style will be
             applied to the widget.
         :param content: The initial :any:`OptionContainer content
@@ -437,15 +434,15 @@
         return True
 
     @enabled.setter
     def enabled(self, value):
         pass
 
     def focus(self):
-        "No-op; OptionContainer cannot accept input focus"
+        """No-op; OptionContainer cannot accept input focus"""
         pass
 
     @property
     def content(self) -> OptionList:
         """The tabs of content currently managed by the OptionContainer."""
         return self._content
 
@@ -484,14 +481,14 @@
         Widget.window.fset(self, window)
 
         # Also assign the window to the content in the container
         for item in self._content:
             item._content.window = window
 
     @property
-    def on_select(self) -> OnSelectHandler:
+    def on_select(self) -> toga.widgets.optioncontainer.OnSelectHandler:
         """The callback to invoke when a new tab of content is selected."""
         return self._on_select
 
     @on_select.setter
     def on_select(self, handler):
         self._on_select = wrapped_handler(self, handler)
```

### Comparing `toga-core-0.4.2/src/toga/widgets/progressbar.py` & `toga_core-0.4.3/src/toga/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/scrollcontainer.py` & `toga_core-0.4.3/src/toga/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/selection.py` & `toga_core-0.4.3/src/toga/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/slider.py` & `toga_core-0.4.3/src/toga/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/splitcontainer.py` & `toga_core-0.4.3/src/toga/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/switch.py` & `toga_core-0.4.3/src/toga/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/src/toga/widgets/table.py` & `toga_core-0.4.3/src/toga/widgets/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     @property
     def accessors(self) -> list[str]:
         """The accessors used to populate the table (read-only)"""
         return self._accessors
 
     @property
     def missing_value(self) -> str:
-        """The value that will be used when a data row doesn't provide an value for an
+        """The value that will be used when a data row doesn't provide a value for an
         attribute.
         """
         return self._missing_value
 
     ######################################################################
     # 2023-06: Backwards compatibility
     ######################################################################
```

### Comparing `toga-core-0.4.2/src/toga/widgets/textinput.py` & `toga_core-0.4.3/src/toga/widgets/textinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :param id: The ID for the widget.
         :param style: A style object. If no style is provided, a default style
             will be applied to the widget.
         :param value: The initial content to display in the widget.
         :param readonly: Can the value of the widget be modified by the user?
         :param placeholder: The content to display as a placeholder when there
             is no user content to display.
-        :param on_change: A handler that will be invoked when the the value of
+        :param on_change: A handler that will be invoked when the value of
             the widget changes.
         :param on_confirm: A handler that will be invoked when the user accepts
             the value of the input (usually by pressing Return on the keyboard).
         :param on_gain_focus: A handler that will be invoked when the widget
             gains input focus.
         :param on_lose_focus: A handler that will be invoked when the widget
             loses input focus.
@@ -115,15 +115,15 @@
         else:
             v = str(value).replace("\n", " ")
         self._impl.set_value(v)
         self.refresh()
 
     @property
     def is_valid(self) -> bool:
-        "Does the value of the widget currently pass all validators without error?"
+        """Does the value of the widget currently pass all validators without error?"""
         return self._impl.is_valid()
 
     @property
     def on_change(self) -> callable:
         """The handler to invoke when the value of the widget changes."""
         return self._on_change
```

### Comparing `toga-core-0.4.2/src/toga/widgets/timeinput.py` & `toga_core-0.4.3/src/toga/widgets/timeinput.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -138,19 +138,19 @@
         warnings.warn("TimePicker has been renamed TimeInput", DeprecationWarning)
 
         for old_name, new_name in [
             ("min_time", "min"),
             ("max_time", "max"),
         ]:
             try:
+                value = kwargs.pop(old_name)
                 warnings.warn(
                     f"TimePicker.{old_name} has been renamed TimeInput.{new_name}",
                     DeprecationWarning,
                 )
-                value = kwargs.pop(old_name)
             except KeyError:
                 pass
             else:
                 kwargs[new_name] = value
 
         super().__init__(*args, **kwargs)
```

### Comparing `toga-core-0.4.2/src/toga/widgets/tree.py` & `toga_core-0.4.3/src/toga/widgets/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         When setting this property:
 
         * A :any:`Source` will be used as-is. It must either be a :any:`TreeSource`, or
           a custom class that provides the same methods.
 
         * A value of None is turned into an empty TreeSource.
 
-        * Otherwise, the value must be an dictionary or an iterable, which is copied
+        * Otherwise, the value must be a dictionary or an iterable, which is copied
           into a new TreeSource as shown :ref:`here <treesource-item>`.
         """
         return self._data
 
     @data.setter
     def data(self, data: Any):
         if data is None:
@@ -268,15 +268,15 @@
     @property
     def accessors(self) -> list[str]:
         """The accessors used to populate the tree (read-only)"""
         return self._accessors
 
     @property
     def missing_value(self) -> str:
-        """The value that will be used when a data row doesn't provide an value for an
+        """The value that will be used when a data row doesn't provide a value for an
         attribute.
         """
         return self._missing_value
 
     @property
     def on_select(self) -> callable:
         """The callback function that is invoked when a row of the tree is selected."""
```

### Comparing `toga-core-0.4.2/src/toga/widgets/webview.py` & `toga_core-0.4.3/src/toga/widgets/webview.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 
         **Note:** This is not currently supported on Android.
         """
         return self._on_webview_load
 
     @on_webview_load.setter
     def on_webview_load(self, handler):
+        if handler and not getattr(self._impl, "SUPPORTS_ON_WEBVIEW_LOAD", True):
+            self.factory.not_implemented("WebView.on_webview_load")
+
         self._on_webview_load = wrapped_handler(self, handler)
 
     @property
     def user_agent(self) -> str:
         """The user agent to use for web requests.
 
         **Note:** On Windows, this property will return an empty string until the widget
```

### Comparing `toga-core-0.4.2/src/toga/window.py` & `toga_core-0.4.3/src/toga/window.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from toga.handlers import AsyncResult, wrapped_handler
 from toga.images import Image
 from toga.platform import get_platform_factory
 
 if TYPE_CHECKING:
     from toga.app import App
     from toga.images import ImageT
+    from toga.screens import Screen
     from toga.widgets.base import Widget
 
 
 class FilteredWidgetRegistry:
     # A class that exposes a mapping lookup interface, filtered to widgets from a single
     # window. The underlying data store is on the app.
 
@@ -193,22 +194,21 @@
         App.app.windows.add(self)
 
         # Create a toolbar that is linked to the app
         self._toolbar = CommandSet(on_change=self._impl.create_toolbar, app=self._app)
 
         self.on_close = on_close
 
-    @property
-    def id(self) -> str:
-        """A unique identifier for the window."""
-        return self._id
-
     def __lt__(self, other) -> bool:
         return self.id < other.id
 
+    ######################################################################
+    # Window properties
+    ######################################################################
+
     @property
     def app(self) -> App:
         """The :any:`App` that this window belongs to (read-only).
 
         New windows are automatically associated with the currently active app."""
         return self._app
 
@@ -217,17 +217,32 @@
         if self._app:
             raise ValueError("Window is already associated with an App")
 
         self._app = app
         self._impl.set_app(app._impl)
 
     @property
-    def closed(self) -> bool:
-        """Whether the window was closed."""
-        return self._closed
+    def closable(self) -> bool:
+        """Can the window be closed by the user?"""
+        return self._closable
+
+    @property
+    def id(self) -> str:
+        """A unique identifier for the window."""
+        return self._id
+
+    @property
+    def minimizable(self) -> bool:
+        """Can the window be minimized by the user?"""
+        return self._minimizable
+
+    @property
+    def resizable(self) -> bool:
+        """Can the window be resized by the user?"""
+        return self._resizable
 
     @property
     def _default_title(self) -> str:
         return "Toga"
 
     @property
     def title(self) -> str:
@@ -238,33 +253,48 @@
     @title.setter
     def title(self, title: str) -> None:
         if not title:
             title = self._default_title
 
         self._impl.set_title(str(title).split("\n")[0])
 
-    @property
-    def resizable(self) -> bool:
-        """Can the window be resized by the user?"""
-        return self._resizable
+    ######################################################################
+    # Window lifecycle
+    ######################################################################
 
-    @property
-    def closable(self) -> bool:
-        """Can the window be closed by the user?"""
-        return self._closable
+    def close(self) -> None:
+        """Close the window.
 
-    @property
-    def minimizable(self) -> bool:
-        """Can the window be minimized by the user?"""
-        return self._minimizable
+        This *does not* invoke the ``on_close`` handler; the window will be immediately
+        and unconditionally closed.
+
+        Once a window has been closed, it *cannot* be reused. The behavior of any method
+        or property on a :class:`~toga.Window` instance after it has been closed is
+        undefined, except for :attr:`closed` which can be used to check if the window
+        was closed.
+        """
+        if self.content:
+            self.content.window = None
+        self.app.windows.discard(self)
+        self._impl.close()
+        self._closed = True
 
     @property
-    def toolbar(self) -> MutableSet[Command]:
-        """Toolbar for the window."""
-        return self._toolbar
+    def closed(self) -> bool:
+        """Whether the window was closed."""
+        return self._closed
+
+    def show(self) -> None:
+        """Show the window. If the window is already visible, this method has no
+        effect."""
+        self._impl.show()
+
+    ######################################################################
+    # Window content and resources
+    ######################################################################
 
     @property
     def content(self) -> Widget | None:
         """Content of the window. On setting, the content is added to the same app as
         the window."""
         return self._content
 
@@ -286,54 +316,129 @@
         # Manifest the widget
         self._impl.set_content(widget._impl)
 
         # Update the geometry of the widget
         widget.refresh()
 
     @property
+    def toolbar(self) -> MutableSet[Command]:
+        """Toolbar for the window."""
+        return self._toolbar
+
+    @property
     def widgets(self) -> Mapping[str, Widget]:
         """The widgets contained in the window.
 
         Can be used to look up widgets by ID (e.g., ``window.widgets["my_id"]``).
         """
         return FilteredWidgetRegistry(self)
 
+    ######################################################################
+    # Window size
+    ######################################################################
+
     @property
     def size(self) -> tuple[int, int]:
         """Size of the window, as a tuple of ``(width, height)``, in
         :ref:`CSS pixels <css-units>`."""
         return self._impl.get_size()
 
     @size.setter
     def size(self, size: tuple[int, int]) -> None:
         self._impl.set_size(size)
         if self.content:
             self.content.refresh()
 
+    ######################################################################
+    # Window position
+    ######################################################################
+
     @property
     def position(self) -> tuple[int, int]:
-        """Position of the window, as a tuple of ``(x, y)`` coordinates, in
-        :ref:`CSS pixels <css-units>`."""
-        return self._impl.get_position()
+        """Absolute position of the window, as a ``(x, y)`` tuple coordinates, in
+        :ref:`CSS pixels <css-units>`.
+
+        The origin is the top left corner of the primary screen.
+        """
+        absolute_origin = self._app.screens[0].origin
+        absolute_window_position = self._impl.get_position()
+
+        window_position = (
+            absolute_window_position[0] - absolute_origin[0],
+            absolute_window_position[1] - absolute_origin[1],
+        )
+        return window_position
 
     @position.setter
     def position(self, position: tuple[int, int]) -> None:
-        self._impl.set_position(position)
+        absolute_origin = self._app.screens[0].origin
+        absolute_new_position = (
+            position[0] + absolute_origin[0],
+            position[1] + absolute_origin[1],
+        )
+        self._impl.set_position(absolute_new_position)
 
-    def show(self) -> None:
-        """Show the window. If the window is already visible, this method has no
-        effect."""
-        self._impl.show()
+    @property
+    def screen(self) -> Screen:
+        """Instance of the :class:`toga.Screen` on which this window is present."""
+        return self._impl.get_current_screen().interface
+
+    @screen.setter
+    def screen(self, app_screen: Screen) -> None:
+        original_window_location = self.position
+        original_origin = self.screen.origin
+        new_origin = app_screen.origin
+        x = original_window_location[0] - original_origin[0] + new_origin[0]
+        y = original_window_location[1] - original_origin[1] + new_origin[1]
+
+        self._impl.set_position((x, y))
+
+    @property
+    def screen_position(self) -> tuple[int, int]:
+        """Position of the window with respect to current screen, as a ``(x, y)`` tuple."""
+        current_relative_position = (
+            self.position[0] - self.screen.origin[0],
+            self.position[1] - self.screen.origin[1],
+        )
+        return current_relative_position
+
+    @screen_position.setter
+    def screen_position(self, position: tuple[int, int]) -> None:
+        new_relative_position = (
+            position[0] + self.screen.origin[0],
+            position[1] + self.screen.origin[1],
+        )
+        self._impl.set_position(new_relative_position)
+
+    ######################################################################
+    # Window visibility
+    ######################################################################
 
     def hide(self) -> None:
         """Hide the window. If the window is already hidden, this method has no
         effect."""
         self._impl.hide()
 
     @property
+    def visible(self) -> bool:
+        """Is the window visible?"""
+        return self._impl.get_visible()
+
+    @visible.setter
+    def visible(self, visible: bool) -> None:
+        if visible:
+            self.show()
+        else:
+            self.hide()
+
+    ######################################################################
+    # Window state
+    ######################################################################
+
+    @property
     def full_screen(self) -> bool:
         """Is the window in full screen mode?
 
         Full screen mode is *not* the same as "maximized". A full screen window
         has no title bar, toolbar or window controls; some or all of these
         items may be visible on a maximized window. A good example of "full screen"
         mode is a slideshow app in presentation mode - the only visible content is
@@ -342,66 +447,49 @@
         return self._is_full_screen
 
     @full_screen.setter
     def full_screen(self, is_full_screen: bool) -> None:
         self._is_full_screen = is_full_screen
         self._impl.set_full_screen(is_full_screen)
 
-    @property
-    def visible(self) -> bool:
-        "Is the window visible?"
-        return self._impl.get_visible()
+    ######################################################################
+    # Window capabilities
+    ######################################################################
 
-    @visible.setter
-    def visible(self, visible: bool) -> None:
-        if visible:
-            self.show()
-        else:
-            self.hide()
+    def as_image(self, format: type[ImageT] = Image) -> ImageT:
+        """Render the current contents of the window as an image.
+
+        :param format: Format to provide. Defaults to :class:`~toga.images.Image`; also
+            supports :any:`PIL.Image.Image` if Pillow is installed, as well as any image
+            types defined by installed :doc:`image format plugins
+            </reference/plugins/image_formats>`.
+        :returns: An image containing the window content, in the format requested.
+        """
+        return Image(self._impl.get_image_data()).as_format(format)
+
+    ######################################################################
+    # Window events
+    ######################################################################
 
     @property
     def on_close(self) -> OnCloseHandler:
         """The handler to invoke if the user attempts to close the window."""
         return self._on_close
 
     @on_close.setter
     def on_close(self, handler: OnCloseHandler | None) -> None:
         def cleanup(window: Window, should_close: bool) -> None:
             if should_close or handler is None:
                 window.close()
 
         self._on_close = wrapped_handler(self, handler, cleanup=cleanup)
 
-    def close(self) -> None:
-        """Close the window.
-
-        This *does not* invoke the ``on_close`` handler; the window will be immediately
-        and unconditionally closed.
-
-        Once a window has been closed, it *cannot* be reused. The behavior of any method
-        or property on a :class:`~toga.Window` instance after it has been closed is
-        undefined, except for :attr:`closed` which can be used to check if the window
-        was closed.
-        """
-        self.app.windows.discard(self)
-        self._impl.close()
-        self._closed = True
-
-    def as_image(self, format: type[ImageT] = Image) -> ImageT:
-        """Render the current contents of the window as an image.
-
-        :param format: Format to provide. Defaults to :class:`~toga.images.Image`; also
-            supports :any:`PIL.Image.Image` if Pillow is installed
-        :returns: An image containing the window content, in the format requested.
-        """
-        return Image(self._impl.get_image_data()).as_format(format)
-
-    ############################################################
+    ######################################################################
     # Dialogs
-    ############################################################
+    ######################################################################
 
     def info_dialog(
         self,
         title: str,
         message: str,
         on_result: DialogResultHandler[None] | None = None,
     ) -> Dialog:
@@ -485,15 +573,15 @@
         self,
         title: str,
         message: str,
         on_result: DialogResultHandler[None] | None = None,
     ) -> Dialog:
         """Ask the user to acknowledge an error state.
 
-        Presents as an error dialog with a "OK" button to close the dialog.
+        Presents as an error dialog with an "OK" button to close the dialog.
 
         **This is an asynchronous method**. If you invoke this method in synchronous
         context, it will show the dialog, but will return *immediately*. The object
         returned by this method can be awaited to obtain the result of the dialog.
 
         :param title: The title of the dialog window.
         :param message: The error message to display.
```

### Comparing `toga-core-0.4.2/src/toga_core.egg-info/PKG-INFO` & `toga_core-0.4.3/src/toga_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 Metadata-Version: 2.1
 Name: toga-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python native, OS native GUI toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,mobile,web,macOS,cocoa,iOS,android,windows,winforms,linux,freeBSD,gtk,console,web
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
 Requires-Dist: travertino>=0.3.0
 Requires-Dist: importlib_metadata>=4.4.0; python_version <= "3.9"
 Provides-Extra: dev
-Requires-Dist: coverage[toml]==7.4.1; extra == "dev"
-Requires-Dist: Pillow==10.2.0; extra == "dev"
+Requires-Dist: coverage[toml]==7.5.1; extra == "dev"
+Requires-Dist: Pillow==10.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; python_version < "3.9" and extra == "dev"
-Requires-Dist: pre-commit==3.6.0; python_version >= "3.9" and extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.4; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 Requires-Dist: pytest-freezer==0.4.8; extra == "dev"
 Requires-Dist: setuptools-scm==8.0.4; extra == "dev"
-Requires-Dist: tox==4.12.1; extra == "dev"
+Requires-Dist: tox==4.15.0; extra == "dev"
 Requires-Dist: typing-extensions==4.9.0; python_version < "3.10" and extra == "dev"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
-Requires-Dist: Pillow==10.2.0; extra == "docs"
+Requires-Dist: furo==2024.4.27; extra == "docs"
+Requires-Dist: Pillow==10.3.0; extra == "docs"
 Requires-Dist: pyenchant==3.2.2; extra == "docs"
 Requires-Dist: sphinx==7.1.2; python_version < "3.9" and extra == "docs"
-Requires-Dist: sphinx==7.2.6; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx==7.3.7; python_version >= "3.9" and extra == "docs"
 Requires-Dist: sphinx_tabs==3.4.5; extra == "docs"
-Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints==1.25.3; extra == "docs"
+Requires-Dist: sphinx-autobuild==2021.3.14; python_version < "3.9" and extra == "docs"
+Requires-Dist: sphinx-autobuild==2024.4.16; python_version >= "3.9" and extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints==2.1.0; extra == "docs"
 Requires-Dist: sphinx-csv-filter==0.4.1; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling==8.0.0; extra == "docs"
 
 Toga
 ====
@@ -72,15 +75,15 @@
 
 Minimum requirements
 --------------------
 
 Toga requires **Python 3.8** or newer. Python 2 is not supported.
 
 Each backend also has specific requirements and pre-requisites. See the `platform
-documentation <https://toga.readthedocs.io/en/stable/reference/platforms.html>`__ for
+documentation <https://toga.readthedocs.io/en/latest/reference/platforms.html>`__ for
 details.
 
 Quickstart
 ----------
 
 To get a demonstration of the capabilities of Toga, run the following::
```

### Comparing `toga-core-0.4.2/src/toga_core.egg-info/SOURCES.txt` & `toga_core-0.4.3/src/toga_core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 src/toga/handlers.py
 src/toga/icons.py
 src/toga/images.py
 src/toga/keys.py
 src/toga/paths.py
 src/toga/platform.py
 src/toga/py.typed
+src/toga/screens.py
+src/toga/types.py
 src/toga/validators.py
 src/toga/window.py
 src/toga/constants/__init__.py
 src/toga/hardware/__init__.py
 src/toga/hardware/camera.py
+src/toga/hardware/location.py
+src/toga/plugins/__init__.py
+src/toga/plugins/image_formats.py
 src/toga/resources/__init__.py
 src/toga/sources/__init__.py
 src/toga/sources/accessors.py
 src/toga/sources/base.py
 src/toga/sources/list_source.py
 src/toga/sources/tree_source.py
 src/toga/sources/value_source.py
@@ -37,14 +42,15 @@
 src/toga/widgets/button.py
 src/toga/widgets/canvas.py
 src/toga/widgets/dateinput.py
 src/toga/widgets/detailedlist.py
 src/toga/widgets/divider.py
 src/toga/widgets/imageview.py
 src/toga/widgets/label.py
+src/toga/widgets/mapview.py
 src/toga/widgets/multilinetextinput.py
 src/toga/widgets/numberinput.py
 src/toga/widgets/optioncontainer.py
 src/toga/widgets/passwordinput.py
 src/toga/widgets/progressbar.py
 src/toga/widgets/scrollcontainer.py
 src/toga/widgets/selection.py
@@ -55,41 +61,43 @@
 src/toga/widgets/textinput.py
 src/toga/widgets/timeinput.py
 src/toga/widgets/tree.py
 src/toga/widgets/webview.py
 src/toga_core.egg-info/PKG-INFO
 src/toga_core.egg-info/SOURCES.txt
 src/toga_core.egg-info/dependency_links.txt
+src/toga_core.egg-info/entry_points.txt
 src/toga_core.egg-info/requires.txt
 src/toga_core.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_documents.py
 tests/test_fonts.py
 tests/test_handlers.py
 tests/test_icons.py
 tests/test_images.py
 tests/test_keys.py
 tests/test_paths.py
 tests/test_platform.py
 tests/test_validators.py
-tests/test_window.py
 tests/app/__init__.py
 tests/app/test_app.py
 tests/app/test_documentapp.py
 tests/app/test_mainwindow.py
+tests/app/test_screens.py
 tests/app/test_widget_registry.py
 tests/app/test_windowset.py
 tests/command/__init__.py
 tests/command/conftest.py
 tests/command/test_command.py
 tests/command/test_commandset.py
 tests/command/test_group.py
 tests/hardware/__init__.py
 tests/hardware/test_camera.py
+tests/hardware/test_location.py
 tests/resources/blue.png
 tests/resources/orange.bmp
 tests/resources/orange.png
 tests/resources/photo.png
 tests/resources/red-16.png
 tests/resources/red-32.png
 tests/resources/red-72.png
@@ -135,14 +143,15 @@
 tests/widgets/test_box.py
 tests/widgets/test_button.py
 tests/widgets/test_dateinput.py
 tests/widgets/test_detailedlist.py
 tests/widgets/test_divider.py
 tests/widgets/test_imageview.py
 tests/widgets/test_label.py
+tests/widgets/test_mapview.py
 tests/widgets/test_multilinetextinput.py
 tests/widgets/test_numberinput.py
 tests/widgets/test_optioncontainer.py
 tests/widgets/test_passwordinput.py
 tests/widgets/test_progressbar.py
 tests/widgets/test_scrollcontainer.py
 tests/widgets/test_selection.py
@@ -156,8 +165,9 @@
 tests/widgets/test_webview.py
 tests/widgets/canvas/__init__.py
 tests/widgets/canvas/conftest.py
 tests/widgets/canvas/test_canvas.py
 tests/widgets/canvas/test_context_objects.py
 tests/widgets/canvas/test_draw_operations.py
 tests/widgets/canvas/test_helpers.py
-tests/window/test_filtered_widget_registry.py
+tests/window/test_filtered_widget_registry.py
+tests/window/test_window.py
```

### Comparing `toga-core-0.4.2/src/toga_core.egg-info/requires.txt` & `toga_core-0.4.3/src/toga_core.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 travertino>=0.3.0
 
 [:python_version <= "3.9"]
 importlib_metadata>=4.4.0
 
 [dev]
-coverage[toml]==7.4.1
-Pillow==10.2.0
-pytest==7.4.4
-pytest-asyncio==0.23.4
+coverage[toml]==7.5.1
+Pillow==10.3.0
+pytest==8.2.0
+pytest-asyncio==0.23.6
 pytest-freezer==0.4.8
 setuptools-scm==8.0.4
-tox==4.12.1
+tox==4.15.0
 
 [dev:python_version < "3.10"]
 typing-extensions==4.9.0
 
 [dev:python_version < "3.9"]
 pre-commit==3.5.0
 
 [dev:python_version >= "3.9"]
-pre-commit==3.6.0
+pre-commit==3.7.0
 
 [docs]
-furo==2024.1.29
-Pillow==10.2.0
+furo==2024.4.27
+Pillow==10.3.0
 pyenchant==3.2.2
 sphinx_tabs==3.4.5
-sphinx-autobuild==2024.2.4
-sphinx-autodoc-typehints==1.25.3
+sphinx-autodoc-typehints==2.1.0
 sphinx-csv-filter==0.4.1
 sphinx-copybutton==0.5.2
 sphinx-toolbox==3.5.0
 sphinxcontrib-spelling==8.0.0
 
 [docs:python_version < "3.9"]
 sphinx==7.1.2
+sphinx-autobuild==2021.3.14
 
 [docs:python_version >= "3.9"]
-sphinx==7.2.6
+sphinx==7.3.7
+sphinx-autobuild==2024.4.16
```

### Comparing `toga-core-0.4.2/tests/app/test_app.py` & `toga_core-0.4.3/tests/app/test_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,22 +197,23 @@
             "org.beeware.explicit-app",
             "override-app",
         ),
     ],
 )
 def test_create(
     monkeypatch,
+    event_loop,
     kwargs,
     metadata,
     main_module,
     expected_formal_name,
     expected_app_id,
     expected_app_name,
 ):
-    """A simple app can be created"""
+    """A simple app can be created."""
     # Monkeypatch the metadata retrieval function
     if metadata:
         metadata_mock = Mock(return_value=metadata)
     else:
         metadata_mock = Mock(
             side_effect=importlib.metadata.PackageNotFoundError(expected_app_name)
         )
@@ -250,21 +251,21 @@
             dict(windows=()),
             ValueError,
             "The `windows` constructor argument of toga.App has been removed",
         ),
     ],
 )
 def test_bad_app_creation(kwargs, exc_type, message):
-    """Errors are raised"""
+    """Errors are raised."""
     with pytest.raises(exc_type, match=message):
         toga.App(**kwargs)
 
 
-def test_app_metadata(monkeypatch):
-    """An app can load metadata from the .dist-info file"""
+def test_app_metadata(monkeypatch, event_loop):
+    """An app can load metadata from the .dist-info file."""
     monkeypatch.setattr(
         importlib.metadata,
         "metadata",
         Mock(
             return_value={
                 "Formal-Name": "Metadata Name",
                 "Name": "metadata",
@@ -286,16 +287,16 @@
 
     assert app.author == "Jane Developer"
     assert app.version == "1.2.3"
     assert app.home_page == "https://example.com/test-app"
     assert app.description == "A test app"
 
 
-def test_explicit_app_metadata(monkeypatch):
-    """App metadata can be provided explicitly, overriding module-level metadata"""
+def test_explicit_app_metadata(monkeypatch, event_loop):
+    """App metadata can be provided explicitly, overriding module-level metadata."""
     monkeypatch.setattr(
         importlib.metadata,
         "metadata",
         Mock(
             return_value={
                 "Formal-Name": "Metadata Name",
                 "Name": "metadata",
@@ -325,16 +326,16 @@
     assert app.home_page == "https://example.com/test-app"
     assert app.description == "A test app"
 
     assert app.on_exit._raw == on_exit_handler
 
 
 @pytest.mark.parametrize("construct", [True, False])
-def test_icon_construction(construct):
-    """The app icon can be set during construction"""
+def test_icon_construction(construct, event_loop):
+    """The app icon can be set during construction."""
     if construct:
         icon = toga.Icon("path/to/icon")
     else:
         icon = "path/to/icon"
 
     app = toga.App(
         formal_name="Test App",
@@ -343,28 +344,31 @@
     )
     assert isinstance(app.icon, toga.Icon)
     assert app.icon.path == Path("path/to/icon")
 
 
 @pytest.mark.parametrize("construct", [True, False])
 def test_icon(app, construct):
-    """The app icon can be changed"""
+    """The app icon can be changed."""
     if construct:
         icon = toga.Icon("path/to/icon")
     else:
         icon = "path/to/icon"
 
     # Default icon matches distribution name
     assert isinstance(app.icon, toga.Icon)
     assert app.icon.path == Path("resources/test-app")
+    # During initial setup, the icon isn't explicitly set.
+    assert_action_not_performed(app, "set_icon")
 
     # Change icon
     app.icon = icon
     assert isinstance(app.icon, toga.Icon)
     assert app.icon.path == Path("path/to/icon")
+    assert_action_performed_with(app, "set_icon", icon=toga.Icon("path/to/icon"))
 
 
 def test_current_window(app):
     """The current window can be set and changed."""
     other_window = toga.Window()
 
     # There are two windows - the main window, plus "other"
@@ -377,24 +381,24 @@
     # Change the current window
     app.current_window = other_window
     assert app.current_window == other_window
     assert_action_performed_with(app, "set_current_window", window=other_window)
 
 
 def test_no_current_window(app):
-    """If there's no current window, current_window reflects this"""
+    """If there's no current window, current_window reflects this."""
     # If all the windows are deleted, and there's no main window (e.g., if it's a document app)
     # there might be no current window.
     app._main_window = None
 
     # The current window evaluates as None
     assert app.current_window is None
 
 
-def test_full_screen():
+def test_full_screen(event_loop):
     """The app can be put into full screen mode."""
     window1 = toga.Window()
     window2 = toga.Window()
     app = toga.App(formal_name="Test App", app_id="org.example.test")
 
     assert not app.is_full_screen
 
@@ -420,16 +424,16 @@
     app.exit_full_screen()
     assert not app.is_full_screen
     assert_action_performed_with(
         app, "exit_full_screen", windows=(app.main_window, window1)
     )
 
 
-def test_set_empty_full_screen_window_list():
-    """Setting the full screen window list to [] is an explicit exit"""
+def test_set_empty_full_screen_window_list(event_loop):
+    """Setting the full screen window list to [] is an explicit exit."""
     app = toga.App(formal_name="Test App", app_id="org.example.test")
     window1 = toga.Window()
     window2 = toga.Window()
 
     assert not app.is_full_screen
 
     # Change the screens that are full screen
@@ -440,66 +444,66 @@
     # Exit full screen mode by setting no windows full screen
     app.set_full_screen()
     assert not app.is_full_screen
     assert_action_performed_with(app, "exit_full_screen", windows=(window1, window2))
 
 
 def test_show_hide_cursor(app):
-    """The app cursor can be shown and hidden"""
+    """The app cursor can be shown and hidden."""
     app.hide_cursor()
     assert_action_performed(app, "hide_cursor")
 
     app.show_cursor()
     assert_action_performed(app, "show_cursor")
 
 
-def test_startup_method():
-    """If an app provides a startup method, it will be invoked during startup"""
+def test_startup_method(event_loop):
+    """If an app provides a startup method, it will be invoked during startup."""
     startup = Mock()
     app = toga.App(
         formal_name="Test App",
         app_id="org.example.test",
         startup=startup,
     )
 
     startup.assert_called_once_with(app)
 
 
-def test_startup_subclass():
-    """App can be subclassed"""
+def test_startup_subclass(event_loop):
+    """App can be subclassed."""
 
     class SubclassedApp(toga.App):
         def startup(self):
             self.main_window = toga.MainWindow()
 
     app = SubclassedApp(formal_name="Test App", app_id="org.example.test")
 
     # The main window will exist, and will have the app's formal name.
     assert app.main_window.title == "Test App"
 
 
-def test_startup_subclass_no_main_window():
-    """If a subclassed app doesn't define a main window, an error is raised"""
+def test_startup_subclass_no_main_window(event_loop):
+    """If a subclassed app doesn't define a main window, an error is raised."""
 
     class SubclassedApp(toga.App):
         def startup(self):
             pass
 
     with pytest.raises(ValueError, match=r"Application does not have a main window."):
         SubclassedApp(formal_name="Test App", app_id="org.example.test")
 
 
 def test_about(app):
-    """The about dialog for the app can be shown"""
+    """The about dialog for the app can be shown."""
     app.about()
     assert_action_performed(app, "show_about_dialog")
 
 
-def test_visit_homepage(monkeypatch):
-    """The app's homepage can be opened"""
+def test_visit_homepage(monkeypatch, event_loop):
+    """The app's homepage can be opened."""
     app = toga.App(
         formal_name="Test App",
         app_id="org.example.test",
         home_page="https://example.com/test-app",
     )
     open_webbrowser = Mock()
     monkeypatch.setattr(webbrowser, "open", open_webbrowser)
@@ -507,15 +511,15 @@
     # The app has no homepage by default, so visit is a no-op
     app.visit_homepage()
 
     open_webbrowser.assert_called_once_with("https://example.com/test-app")
 
 
 def test_no_homepage(monkeypatch, app):
-    """If the app doesn't have a home page, visit_homepage is a no-op"""
+    """If the app doesn't have a home page, visit_homepage is a no-op."""
     open_webbrowser = Mock()
     monkeypatch.setattr(webbrowser, "open", open_webbrowser)
 
     # The app has no homepage by default, so visit is a no-op
     app.visit_homepage()
 
     open_webbrowser.assert_not_called()
@@ -524,69 +528,69 @@
 def test_beep(app):
     """The machine can go Bing!"""
     app.beep()
     assert_action_performed(app, "beep")
 
 
 def test_exit_direct(app):
-    """An app can be exited directly"""
+    """An app can be exited directly."""
     on_exit_handler = Mock(return_value=True)
     app.on_exit = on_exit_handler
 
     # Exit the app directly
     app.exit()
 
     # App has been exited, but the exit handler has *not* been invoked.
     assert_action_performed(app, "exit")
     on_exit_handler.assert_not_called()
 
 
 def test_exit_no_handler(app):
-    """A app without a exit handler can be exited"""
+    """An app without an exit handler can be exited."""
     # Exit the app
     app._impl.simulate_exit()
 
-    # Window has been exitd, and is no longer in the app's list of windows.
+    # Window has been exited, and is no longer in the app's list of windows.
     assert_action_performed(app, "exit")
 
 
-def test_exit_sucessful_handler(app):
-    """An app with a successful exit handler can be exited"""
+def test_exit_successful_handler(app):
+    """An app with a successful exit handler can be exited."""
     on_exit_handler = Mock(return_value=True)
     app.on_exit = on_exit_handler
 
     # Close the app
     app._impl.simulate_exit()
 
     # App has been exited
     assert_action_performed(app, "exit")
     on_exit_handler.assert_called_once_with(app)
 
 
 def test_exit_rejected_handler(app):
-    """An app can have a exit handler that rejects the exit"""
+    """An app can have a exit handler that rejects the exit."""
     on_exit_handler = Mock(return_value=False)
     app.on_exit = on_exit_handler
 
     # Close the window
     app._impl.simulate_exit()
 
     # App has been *not* exited
     assert_action_not_performed(app, "exit")
     on_exit_handler.assert_called_once_with(app)
 
 
 def test_loop(app, event_loop):
-    """The main thread's event loop can be accessed"""
+    """The main thread's event loop can be accessed."""
     assert isinstance(app.loop, asyncio.AbstractEventLoop)
     assert app.loop is event_loop
 
 
 def test_background_task(app):
-    """A background task can be queued"""
+    """A background task can be queued."""
     canary = Mock()
 
     async def background(app, **kwargs):
         canary()
 
     app.add_background_task(background)
 
@@ -596,28 +600,27 @@
 
     app.loop.run_until_complete(waiter())
 
     # Once the loop has executed, the background task should have executed as well.
     canary.assert_called_once()
 
 
-def test_deprecated_id():
+def test_deprecated_id(event_loop):
     """The deprecated `id` constructor argument is ignored, and the property of the same
-    name is redirected to `app_id`
-    """
+    name is redirected to `app_id`"""
     id_warning = r"App.id is deprecated.* Use app_id instead"
     with pytest.warns(DeprecationWarning, match=id_warning):
         app = toga.App("Test App", "org.example.test", id="test_app_id")
 
     assert app.app_id == "org.example.test"
     with pytest.warns(DeprecationWarning, match=id_warning):
         assert app.id == "org.example.test"
 
 
-def test_deprecated_name():
+def test_deprecated_name(event_loop):
     """The deprecated `name` property is redirected to `formal_name`"""
     name_warning = r"App.name is deprecated. Use formal_name instead"
     app = toga.App("Test App", "org.example.test")
 
     assert app.formal_name == "Test App"
     with pytest.warns(DeprecationWarning, match=name_warning):
         assert app.name == "Test App"
```

### Comparing `toga-core-0.4.2/tests/app/test_documentapp.py` & `toga_core-0.4.3/tests/app/test_documentapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
     # Document window has been created and shown
     assert_action_performed(app.documents[0].main_window, "create Window")
     assert_action_performed(app.documents[0].main_window, "show")
 
 
 def test_create_with_unknown_document_type(monkeypatch):
-    """If the document specified at the command line is an unknown type, an exception is raised"""
+    """If the document specified at the command line is an unknown type, an exception is
+    raised."""
     monkeypatch.setattr(sys, "argv", ["app-exe", "/path/to/filename.unknown"])
 
     with pytest.raises(
         ValueError,
         match=r"Don't know how to open documents of type .unknown",
     ):
         toga.DocumentApp(
@@ -87,15 +88,15 @@
         ValueError,
         match=r"A document must manage at least one document type.",
     ):
         toga.DocumentApp("Test App", "org.beeware.document-app")
 
 
 def test_close_single_document_app():
-    """An app in single document mode closes the app when the window is closed"""
+    """An app in single document mode closes the app when the window is closed."""
     # Monkeypatch the dummy impl to use single document mode
     DummyDocument.SINGLE_DOCUMENT_APP = True
 
     # Mock the app, but preserve the factory
     app = Mock()
     app.factory = get_platform_factory()
 
@@ -107,15 +108,15 @@
         return await doc.handle_close(Mock())
 
     assert not asyncio.get_event_loop().run_until_complete(_do_close())
     app.exit.assert_called_once_with()
 
 
 def test_close_multiple_document_app():
-    """An app in multiple document mode doesn't close when the window is closed"""
+    """An app in multiple document mode doesn't close when the window is closed."""
     # Monkeypatch the dummy impl to use single document mode
     DummyDocument.SINGLE_DOCUMENT_APP = False
 
     # Mock the app, but preserve the factory
     app = Mock()
     app.factory = get_platform_factory()
```

### Comparing `toga-core-0.4.2/tests/app/test_mainwindow.py` & `toga_core-0.4.3/tests/app/test_mainwindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 import toga
 from toga_dummy.utils import assert_action_performed
 
 
 def test_create(app):
-    "A MainWindow can be created with minimal arguments"
+    """A MainWindow can be created with minimal arguments."""
     window = toga.MainWindow()
 
     assert window.app == app
     assert window.content is None
 
     assert window._impl.interface == window
     assert_action_performed(window, "create Window")
@@ -27,15 +27,15 @@
     assert window.minimizable
     assert len(window.toolbar) == 0
     # No on-close handler
     assert window.on_close is None
 
 
 def test_no_close():
-    "An on_close handler cannot be set on MainWindow"
+    """An on_close handler cannot be set on MainWindow."""
     window = toga.MainWindow()
 
     with pytest.raises(
         ValueError,
         match=r"Cannot set on_close handler for the main window. Use the app on_exit handler instead.",
     ):
         window.on_close = Mock()
```

### Comparing `toga-core-0.4.2/tests/app/test_widget_registry.py` & `toga_core-0.4.3/tests/app/test_widget_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def test_empty_registry(widget_registry):
     assert len(widget_registry) == 0
     assert list(widget_registry) == []
     assert str(widget_registry) == "{}"
 
 
 def test_add_widget(widget_registry):
-    "Widgets can be added to the registry"
+    """Widgets can be added to the registry."""
     # Add a widget to the registry
     widget1 = ExampleWidget(id="widget-1")
     widget_registry._add(widget1)
 
     assert len(widget_registry) == 1
     assert list(widget_registry) == [widget1]
     assert str(widget_registry) == "{'widget-1': Widget(id='widget-1')}"
@@ -42,15 +42,15 @@
 
     assert len(widget_registry) == 2
     assert widget_registry["widget-1"] == widget1
     assert widget_registry["widget-2"] == widget2
 
 
 def test_update_widgets(widget_registry):
-    "The registry can be bulk updated"
+    """The registry can be bulk updated."""
     # Add a widget to the registry
     widget1 = ExampleWidget(id="widget-1")
     widget_registry._add(widget1)
 
     widget2 = ExampleWidget(id="widget-2")
     widget3 = ExampleWidget(id="widget-3")
     widget4 = ExampleWidget(id="widget-4")
@@ -60,15 +60,15 @@
     assert widget_registry["widget-1"] == widget1
     assert widget_registry["widget-2"] == widget2
     assert widget_registry["widget-3"] == widget3
     assert widget_registry["widget-4"] == widget4
 
 
 def test_remove_widget(widget_registry):
-    "A widget can be removed from the repository"
+    """A widget can be removed from the repository."""
     "Widgets can be added to the registry"
     # Add a widget to the registry
     widget1 = ExampleWidget(id="widget-1")
     widget2 = ExampleWidget(id="widget-2")
     widget_registry._update({widget1, widget2})
 
     assert len(widget_registry) == 2
@@ -76,15 +76,15 @@
     widget_registry._remove("widget-2")
 
     assert widget_registry["widget-1"] == widget1
     assert "widget-2" not in widget_registry
 
 
 def test_add_same_widget_twice(widget_registry):
-    "A widget cannot be added to the same registry twice"
+    """A widget cannot be added to the same registry twice."""
     # Add a widget to the registry
     widget1 = ExampleWidget(id="widget-1")
     widget_registry._add(widget1)
 
     assert len(widget_registry) == 1
 
     # Add the widget again; this raises an error
@@ -96,15 +96,15 @@
 
     # Widget is still there
     assert len(widget_registry) == 1
     assert widget_registry["widget-1"] == widget1
 
 
 def test_add_duplicate_id(widget_registry):
-    "A widget cannot be added to the same registry twice"
+    """A widget cannot be added to the same registry twice."""
     # Add a widget to the registry
     widget1 = ExampleWidget(id="widget-1")
     widget_registry._add(widget1)
 
     assert len(widget_registry) == 1
 
     new_widget = ExampleWidget(id="widget-1")
@@ -118,15 +118,15 @@
 
     # Widget is still there
     assert len(widget_registry) == 1
     assert widget_registry["widget-1"] == widget1
 
 
 def test_setitem(widget_registry):
-    "Widgets cannot be directly assigned to the registry"
+    """Widgets cannot be directly assigned to the registry."""
     widget1 = ExampleWidget(id="widget-1")
 
     with pytest.raises(
         TypeError,
         match=r"'WidgetRegistry' object does not support item assignment",
     ):
         widget_registry["new is"] = widget1
```

### Comparing `toga-core-0.4.2/tests/app/test_windowset.py` & `toga_core-0.4.3/tests/app/test_windowset.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     windowset = WindowSet(app)
 
     assert windowset.app == app
     assert len(windowset) == 0
 
 
 def test_add_discard(app, window1, window2):
-    """An item can be added to a windowset"""
+    """An item can be added to a windowset."""
     # The windowset has 3 windows - the main window, plus 2 extras
     assert len(app.windows) == 3
 
     # Check the iterator and sorting works
     assert sorted(iter(app.windows)) == [window1, app.main_window, window2]
 
     with pytest.raises(
@@ -57,15 +57,15 @@
         TypeError,
         match=r"Can only discard objects of type toga.Window",
     ):
         app.windows.discard(object())
 
 
 def test_iadd_isub(app, window1, window2):
-    """The deprecated += and -= operators are no-ops"""
+    """The deprecated += and -= operators are no-ops."""
     # The windowset has 3 windows - the main window, plus 2 extras
     assert window2 in app.windows
     assert len(app.windows) == 3
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Windows are automatically associated with the app; \+= is not required",
```

### Comparing `toga-core-0.4.2/tests/command/conftest.py` & `toga_core-0.4.3/tests/command/conftest.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/command/test_command.py` & `toga_core-0.4.3/tests/command/test_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,22 @@
             assert not items[i] < None
             assert not items[i] < 42
             assert not items[i] > None
             assert not items[i] > 42
 
 
 def test_separator(parent_group_1):
-    """A separator can be created"""
+    """A separator can be created."""
 
     separator = Separator(group=parent_group_1)
     assert repr(separator) == "<Separator group=P1>"
 
 
 def test_separator_eq(parent_group_1, parent_group_2):
-    """Separator objects can be compared for equality"""
+    """Separator objects can be compared for equality."""
 
     separator_1a = Separator(parent_group_1)
     separator_1b = Separator(parent_group_1)
     separator_2 = Separator(parent_group_2)
 
     # Separators are equal to breaks in the same section, but not to other
     # sections
@@ -42,15 +42,15 @@
     assert separator_1a != separator_2
 
     # Separators aren't equal to non-separator objects
     assert separator_1a != 3
 
 
 def test_create():
-    """A command can be created with defaults"""
+    """A command can be created with defaults."""
     cmd = toga.Command(None, "Test command")
 
     assert cmd.text == "Test command"
     assert cmd.shortcut is None
     assert cmd.tooltip is None
     assert cmd.group == toga.Group.COMMANDS
     assert cmd.section == 0
@@ -59,16 +59,41 @@
 
     assert (
         repr(cmd)
         == "<Command text='Test command' group=<Group text='Commands' order=30> section=0 order=0>"
     )
 
 
+def test_change_action():
+    """A command's action can be changed to another handler."""
+    action1 = Mock()
+
+    cmd = toga.Command(action1, "Test command")
+
+    assert cmd.text == "Test command"
+    assert cmd.shortcut is None
+    assert cmd.tooltip is None
+    assert cmd.group == toga.Group.COMMANDS
+    assert cmd.section == 0
+    assert cmd.order == 0
+    assert cmd.action._raw == action1
+
+    # Change the action to a something new
+    action2 = Mock()
+    cmd.action = action2
+
+    assert cmd.action._raw == action2
+
+    # Clear the action
+    cmd.action = None
+    assert cmd.action._raw is None
+
+
 def test_create_explicit(app):
-    """A command can be created with explicit arguments"""
+    """A command can be created with explicit arguments."""
     grp = toga.Group("Test group", order=10)
 
     handler = Mock()
     cmd = toga.Command(
         handler,
         text="Test command",
         tooltip="This is a test command",
@@ -91,28 +116,28 @@
         repr(cmd)
         == "<Command text='Test command' group=<Group text='Test group' order=10> section=3 order=4>"
     )
 
 
 @pytest.mark.parametrize("construct", [True, False])
 def test_icon_construction(app, construct):
-    """The command icon can be set during construction"""
+    """The command icon can be set during construction."""
     if construct:
         icon = toga.Icon("path/to/icon")
     else:
         icon = "path/to/icon"
 
     cmd = toga.Command(None, "Test command", icon=icon)
     assert isinstance(cmd.icon, toga.Icon)
     assert cmd.icon.path == Path("path/to/icon")
 
 
 @pytest.mark.parametrize("construct", [True, False])
 def test_icon(app, construct):
-    """The command icon can be changed"""
+    """The command icon can be changed."""
     if construct:
         icon = toga.Icon("path/to/icon")
     else:
         icon = "path/to/icon"
 
     cmd = toga.Command(None, "Test command")
 
@@ -155,39 +180,39 @@
 
     # Set enabled; triggers an implementation response
     cmd.enabled = True
     assert_action_performed_with(cmd, "set enabled", value=True)
 
 
 def test_order_by_text():
-    """Commands are ordered by text when group, section and order match"""
+    """Commands are ordered by text when group, section and order match."""
     assert_order(
         toga.Command(None, "A"),
         toga.Command(None, "B"),
     )
 
 
 def test_order_by_number():
-    """Commands are ordered by number when group and section match"""
+    """Commands are ordered by number when group and section match."""
     assert_order(
         toga.Command(None, "B", order=1),
         toga.Command(None, "A", order=2),
     )
 
 
 def test_order_by_section(parent_group_1):
-    """Section ordering takes priority over order and text"""
+    """Section ordering takes priority over order and text."""
     assert_order(
         toga.Command(None, "B", group=parent_group_1, section=1, order=2),
         toga.Command(None, "A", group=parent_group_1, section=2, order=1),
     )
 
 
 def test_order_by_groups(parent_group_1, parent_group_2, child_group_1, child_group_2):
-    """Commands are ordered by group over"""
+    """Commands are ordered by group over."""
 
     command_z = toga.Command(None, "Z", group=parent_group_1, order=1)
     command_y = toga.Command(None, "Y", group=child_group_1, order=1)
     command_x = toga.Command(None, "X", group=child_group_1, order=2)
     command_w = toga.Command(None, "W", group=child_group_1, order=4)
     command_b = toga.Command(None, "B", group=child_group_1, section=2, order=1)
     command_v = toga.Command(None, "V", group=parent_group_1, order=3)
```

### Comparing `toga-core-0.4.2/tests/command/test_commandset.py` & `toga_core-0.4.3/tests/command/test_commandset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import pytest
 
 import toga
 from toga.command import CommandSet, Separator
 
 
 def test_create():
-    """A CommandSet can be created with defaults"""
+    """A CommandSet can be created with defaults."""
     cs = CommandSet()
 
     assert list(cs) == []
     assert cs.on_change is None
 
 
 def test_create_with_values():
-    """A CommandSet can be created with values"""
+    """A CommandSet can be created with values."""
     change_handler = Mock()
     cs = CommandSet(on_change=change_handler)
 
     assert list(cs) == []
     assert cs.on_change == change_handler
 
 
 @pytest.mark.parametrize("change_handler", [(None), (Mock())])
 def test_add_clear(app, change_handler):
-    """Commands can be added and removed from a commandset"""
+    """Commands can be added and removed from a commandset."""
     # Put some commands into the app
     cmd_a = toga.Command(None, text="App command a")
     cmd_b = toga.Command(None, text="App command b", order=10)
     app.commands.add(cmd_a, cmd_b)
     assert list(app.commands) == [cmd_a, cmd_b]
 
     # Create a standalone command set and add some commands
@@ -63,15 +63,15 @@
 
     # App command set hasn't changed.
     assert list(app.commands) == [cmd_a, cmd_b]
 
 
 @pytest.mark.parametrize("change_handler", [(None), (Mock())])
 def test_add_clear_with_app(app, change_handler):
-    """Commands can be added and removed from a commandset that is linked to an app"""
+    """Commands can be added and removed from a commandset that is linked to an app."""
     # Put some commands into the app
     cmd_a = toga.Command(None, text="App command a")
     cmd_b = toga.Command(None, text="App command b", order=10)
     app.commands.add(cmd_a, cmd_b)
     assert list(app.commands) == [cmd_a, cmd_b]
 
     # Create a command set that is linked to the app and add some commands
@@ -126,15 +126,15 @@
     parent_group_2,
     child_group_1,
     child_group_2,
     child_group_3,
     child_group_4,
     child_group_5,
 ):
-    """Ordering of groups, separators and commands is preserved"""
+    """Ordering of groups, separators and commands is preserved."""
 
     # Menu structure is:
     # - parent group 1
     #   - Z                 - a group that starts with a command
     #   - child group 1
     #     - Y
     #     - X
```

### Comparing `toga-core-0.4.2/tests/command/test_group.py` & `toga_core-0.4.3/tests/command/test_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import toga
 
 from .test_command import assert_order
 
 
 def test_create():
-    """A group can be created with defaults"""
+    """A group can be created with defaults."""
     grp = toga.Group("Group name")
     assert grp.text == "Group name"
     assert grp.order == 0
 
     assert repr(grp) == "<Group text='Group name' order=0>"
 
 
 def test_create_with_params():
-    """A fully specified group can be created"""
+    """A fully specified group can be created."""
     parent = toga.Group("Parent name")
     grp = toga.Group("Group name", order=2, section=3, parent=parent)
 
     assert grp.text == "Group name"
     assert grp.order == 2
     assert grp.section == 3
     assert grp.parent == parent
@@ -88,15 +88,15 @@
     # Partially same values are not equal
     assert group_a1 != group_a
     assert group_a1 != toga.Group("B", order=1)
     assert group_a1 != toga.Group("A", order=2)
 
 
 def test_parent_creation():
-    """Parents can be assigned at creation"""
+    """Parents can be assigned at creation."""
     group_a = toga.Group("A")
     group_b = toga.Group("B", parent=group_a)
     group_c = toga.Group("C", parent=group_b)
 
     # None checks
     assert not group_a.is_parent_of(None)
     assert not group_a.is_child_of(None)
@@ -127,15 +127,15 @@
     assert group_b.root == group_a
 
     assert group_c.parent == group_b
     assert group_c.root == group_a
 
 
 def test_parent_assignment():
-    """Parents can be assigned at runtime"""
+    """Parents can be assigned at runtime."""
     # Eventually, we'll end up with A->B->C, D.
     group_a = toga.Group("A")
     group_b = toga.Group("B")
     group_c = toga.Group("C")
     group_d = toga.Group("D")
 
     assert not group_a.is_parent_of(group_b)
@@ -214,15 +214,15 @@
     assert group_c.root == group_a
 
     assert group_d.parent == group_b
     assert group_d.root == group_a
 
 
 def test_parent_loops():
-    """Parent loops are prevented can be assigned at runtime"""
+    """Parent loops are prevented can be assigned at runtime."""
     group_a = toga.Group("A")
     group_b = toga.Group("B", parent=group_a)
     group_c = toga.Group("C", parent=group_b)
 
     #
     with pytest.raises(
         ValueError,
@@ -240,20 +240,20 @@
         ValueError,
         match=r"Cannot set parent; 'A' is an ancestor of 'C'.",
     ):
         group_a.parent = group_c
 
 
 def test_order_by_text():
-    """Groups are ordered by text if order and section are equivalent"""
+    """Groups are ordered by text if order and section are equivalent."""
     assert_order(toga.Group("A"), toga.Group("B"))
 
 
 def test_order_by_number():
-    """Groups are ordered by number"""
+    """Groups are ordered by number."""
     assert_order(toga.Group("B", order=1), toga.Group("A", order=2))
 
 
 def test_order_by_groups(parent_group_1, parent_group_2):
     """Groups are ordered by parent, then section, then order."""
     assert_order(
         parent_group_1,
```

### Comparing `toga-core-0.4.2/tests/conftest.py` & `toga_core-0.4.3/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,14 @@
 
 class TestApp(toga.App):
     pass
 
 
 @pytest.fixture
 def app(event_loop):
+    # The app icon is cached; purge the app icon cache if it exists
+    try:
+        del toga.Icon.__APP_ICON
+    except AttributeError:
+        pass
+
     return TestApp(formal_name="Test App", app_id="org.beeware.toga.test-app")
```

### Comparing `toga-core-0.4.2/tests/hardware/test_camera.py` & `toga_core-0.4.3/tests/hardware/test_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 @pytest.fixture
 def photo(app):
     return toga.Image("resources/photo.png")
 
 
 def test_no_camera(monkeypatch, app):
-    """If there's no camera, and no factory implementation, accessing camera raises an exception"""
+    """If there's no camera, and no factory implementation, accessing camera raises an
+    exception."""
     try:
         monkeypatch.delattr(app, "_camera")
     except AttributeError:
         pass
     monkeypatch.delattr(factory, "Camera")
 
     # Accessing the camera object should raise NotImplementedError
@@ -38,15 +39,15 @@
     [
         (-1, True, True),
         (0, True, False),
         (1, False, True),
     ],
 )
 def test_request_permission(app, initial, should_request, has_permission):
-    """An app can request permission to use the camera"""
+    """An app can request permission to use the camera."""
     # The camera instance round-trips the app instance
     assert app.camera.app == app
 
     # Set initial permission
     app.camera._impl._has_permission = initial
 
     assert (
@@ -59,15 +60,15 @@
         assert_action_not_performed(app.camera, "request permission")
 
     # As a result of requesting, photo permission is as expected
     assert app.camera.has_permission == has_permission
 
 
 def test_request_permission_sync(app):
-    """An app can synchronously request permission to use the camera"""
+    """An app can synchronously request permission to use the camera."""
     # Set initial permission
     app.camera._impl._has_permission = -1
 
     result = app.camera.request_permission()
 
     # This will cause a permission request to occur...
     assert_action_performed(app.camera, "request permission")
@@ -75,15 +76,15 @@
     # ... but the result won't be directly comparable
     with pytest.raises(RuntimeError):
         # == True isn't good python, but it's going to raise an exception anyway.
         result == True  # noqa: E712
 
 
 def test_device_properties(app):
-    """Device properties can be checked"""
+    """Device properties can be checked."""
 
     assert [
         {
             "device": device,
             "__repr__": repr(device),
             "__str__": str(device),
             "name": device.name,
@@ -126,15 +127,16 @@
     [None, CameraDevice(DummyCamera.CAMERA_1), CameraDevice(DummyCamera.CAMERA_2)],
 )
 @pytest.mark.parametrize(
     "flash",
     [FlashMode.AUTO, FlashMode.ON, FlashMode.OFF],
 )
 def test_take_photo_with_permission(app, device, flash, photo):
-    """If permission has not been previously requested, it is requested before a photo is taken."""
+    """If permission has not been previously requested, it is requested before a photo
+    is taken."""
     # Set permission to potentially allowed
     app.camera._impl._has_permission = -1
 
     app.camera._impl.simulate_photo(photo)
 
     result = app.loop.run_until_complete(
         app.camera.take_photo(device=device, flash=flash)
@@ -173,15 +175,15 @@
         permission_requested=False,
         device=None,
         flash=FlashMode.AUTO,
     )
 
 
 def test_take_photo_no_permission(app, photo):
-    """If permission has been denied, an exception is raised"""
+    """If permission has been denied, an exception is raised."""
     # Deny permission
     app.camera._impl._has_permission = 0
 
     with pytest.raises(
         PermissionError,
         match=r"App does not have permission to take photos",
     ):
```

### Comparing `toga-core-0.4.2/tests/resources/blue.png` & `toga_core-0.4.3/tests/resources/blue.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/orange.bmp` & `toga_core-0.4.3/tests/resources/orange.bmp`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/orange.png` & `toga_core-0.4.3/tests/resources/orange.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/photo.png` & `toga_core-0.4.3/tests/resources/photo.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/red-32.png` & `toga_core-0.4.3/tests/resources/red-32.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/red-72.png` & `toga_core-0.4.3/tests/resources/red-72.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/red.png` & `toga_core-0.4.3/tests/resources/red.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/sample-dummy.png` & `toga_core-0.4.3/tests/resources/sample-dummy.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/sample.png` & `toga_core-0.4.3/tests/resources/sample.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/resources/toga.png` & `toga_core-0.4.3/tests/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/sources/test_accessors.py` & `toga_core-0.4.3/tests/sources/test_accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         (" ", "_"),
         # Multiple whitespace characters are collapsed
         ("Hello - World", "hello_world"),
         ("  ", "_"),
     ],
 )
 def test_to_accessor(heading, accessor):
-    "Headings can be converted into accessors"
+    """Headings can be converted into accessors."""
 
     assert to_accessor(heading) == accessor
 
 
 @pytest.mark.parametrize("heading", ["$*(!&*@&^*&^!", ""])
 def test_to_accessor_failures(heading):
     with pytest.raises(
@@ -66,15 +66,15 @@
             ["First Col", "Second Col", "Third Col"],
             {"First Col": "first", "Second Col": "second"},
             ["first", "second", "third_col"],
         ),
     ],
 )
 def test_build_accessors(headings, overrides, accessors):
-    "Accessors can be constructed from headings with overrides"
+    """Accessors can be constructed from headings with overrides."""
     assert build_accessors(headings, overrides) == accessors
 
 
 @pytest.mark.parametrize(
     "headings, overrides, error",
     [
         (
@@ -86,10 +86,10 @@
             ["!!", "Second Col", "Third Col"],
             None,
             r"Unable to automatically generate accessor from heading '!!'",
         ),
     ],
 )
 def test_build_accessor_failure(headings, overrides, error):
-    "If an accessor list can't be build, an error is raised"
+    """If an accessor list can't be built, an error is raised."""
     with pytest.raises(ValueError, match=error):
         build_accessors(headings, overrides)
```

### Comparing `toga-core-0.4.2/tests/sources/test_list_source.py` & `toga_core-0.4.3/tests/sources/test_list_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,52 +22,52 @@
     [
         None,
         42,
         "not a list",
     ],
 )
 def test_invalid_accessors(value):
-    "Accessors for a list source must be a list of attribute names"
+    """Accessors for a list source must be a list of attribute names."""
     with pytest.raises(
         ValueError,
         match=r"accessors should be a list of attribute names",
     ):
         ListSource(accessors=value)
 
 
 def test_accessors_required():
-    "A list source must specify *some* accessors"
+    """A list source must specify *some* accessors."""
     with pytest.raises(
         ValueError,
         match=r"ListSource must be provided a list of accessors",
     ):
         ListSource(accessors=[], data=[1, 2, 3])
 
 
 def test_accessors_copied():
-    "A list source must specify *some* accessors"
+    """A list source must specify *some* accessors."""
     accessors = ["foo", "bar"]
     source = ListSource(accessors)
 
     assert source._accessors == ["foo", "bar"]
 
     # The accessors have been copied.
     accessors.append("whiz")
     assert source._accessors == ["foo", "bar"]
 
 
 def test_empty_source():
-    "A list source can be constructed with no data"
+    """A list source can be constructed with no data."""
     source = ListSource(accessors=["foo", "bar"])
 
     assert len(source) == 0
 
 
 def test_tuples():
-    "A ListSource can be instantiated with tuples"
+    """A ListSource can be instantiated with tuples."""
     source = ListSource(
         data=[
             ("first", 111),
             ("second", 222),
             ("third", 333),
         ],
         accessors=["val1", "val2"],
@@ -92,15 +92,15 @@
     assert source[1].val1 == "new element"
     assert source[1].val2 == 999
 
     listener.insert.assert_called_once_with(index=1, item=source[1])
 
 
 def test_list():
-    "A ListSource can be instantiated with lists"
+    """A ListSource can be instantiated with lists."""
     source = ListSource(
         data=[
             ["first", 111],
             ["second", 222],
             ["third", 333],
         ],
         accessors=["val1", "val2"],
@@ -125,15 +125,15 @@
     assert source[1].val1 == "new element"
     assert source[1].val2 == 999
 
     listener.insert.assert_called_once_with(index=1, item=source[1])
 
 
 def test_dict():
-    "A ListSource can be instantiated with dictionaries"
+    """A ListSource can be instantiated with dictionaries."""
     source = ListSource(
         data=[
             {"val1": "first", "val2": 111},
             {"val1": "second", "val2": 222},
             {"val1": "third", "val2": 333},
         ],
         accessors=["val1", "val2"],
@@ -158,15 +158,15 @@
     assert source[1].val1 == "new element"
     assert source[1].val2 == 999
 
     listener.insert.assert_called_once_with(index=1, item=source[1])
 
 
 def test_flat_list():
-    "A list source can be created from a flat list of objects"
+    """A list source can be created from a flat list of objects."""
 
     class MyObject:
         def __init__(self, info):
             self.info = info
 
         def __str__(self):
             return "string value %s" % self.info
@@ -183,15 +183,15 @@
     )
 
     for i, row in enumerate(source):
         assert row.col1 == data[i]
 
 
 def test_flat_list_numbers():
-    "A list source can be created from a flat list of numbers"
+    """A list source can be created from a flat list of numbers."""
 
     data = [
         100,
         200.0,
         -3.14,
     ]
 
@@ -201,15 +201,15 @@
     )
 
     for i, row in enumerate(source):
         assert row.col1 == data[i]
 
 
 def test_flat_list_strings():
-    "A list source can be created from a flat list of numbers"
+    """A list source can be created from a flat list of numbers."""
 
     data = [
         "xxx",
         "yyy",
         "zzz",
     ]
 
@@ -219,24 +219,24 @@
     )
 
     for i, row in enumerate(source):
         assert row.col1 == data[i]
 
 
 def test_iter(source):
-    "A list source can be iterated over"
+    """A list source can be iterated over."""
     result = 0
     for row in source:
         result += row.val2
 
     assert result == 666
 
 
 def test_clear(source):
-    "A list source can be cleared"
+    """A list source can be cleared."""
 
     assert len(source) == 3
 
     listener = Mock()
     source.add_listener(listener)
 
     # Clear the list
@@ -246,15 +246,15 @@
     assert len(source) == 0
 
     # A notification was sent
     listener.clear.assert_called_once_with()
 
 
 def test_insert_kwarg(source):
-    "You can insert into a list source using kwargs"
+    """You can insert into a list source using kwargs."""
 
     listener = Mock()
     source.add_listener(listener)
 
     # Insert the new element
     row = source.insert(1, dict(val1="new element", val2=999))
 
@@ -263,15 +263,15 @@
     assert row.val1 == "new element"
     assert row.val2 == 999
 
     listener.insert.assert_called_once_with(index=1, item=row)
 
 
 def test_insert_positional(source):
-    "You can insert into a list source using positional args"
+    """You can insert into a list source using positional args."""
     listener = Mock()
     source.add_listener(listener)
 
     # Insert the new element using positional args.
     # The values are mapped to the accessors in order.
     row = source.insert(1, ("new element", 999))
 
@@ -280,15 +280,15 @@
     assert row.val1 == "new element"
     assert row.val2 == 999
 
     listener.insert.assert_called_once_with(index=1, item=row)
 
 
 def test_append_dict(source):
-    "You can append onto a list source using a dictionary"
+    """You can append onto a list source using a dictionary."""
 
     listener = Mock()
     source.add_listener(listener)
 
     # Append the new element
     row = source.append(dict(val1="new element", val2=999))
 
@@ -297,15 +297,15 @@
     assert row.val1 == "new element"
     assert row.val2 == 999
 
     listener.insert.assert_called_once_with(index=3, item=row)
 
 
 def test_append_positional(source):
-    "You can append onto a list source using positional args"
+    """You can append onto a list source using positional args."""
     listener = Mock()
     source.add_listener(listener)
 
     # Append the new element using positional args.
     # The values are mapped to the accessors in order.
     row = source.append(("new element", 999))
 
@@ -314,15 +314,15 @@
     assert row.val1 == "new element"
     assert row.val2 == 999
 
     listener.insert.assert_called_once_with(index=3, item=row)
 
 
 def test_del(source):
-    "You can delete an item from a list source by index"
+    """You can delete an item from a list source by index."""
     listener = Mock()
     source.add_listener(listener)
 
     # Delete the second element
     row = source[1]
     del source[1]
 
@@ -333,15 +333,15 @@
     assert source[1].val1 == "third"
     assert source[1].val2 == 333
 
     listener.remove.assert_called_once_with(item=row, index=1)
 
 
 def test_remove(source):
-    "You can remove an item from a list source"
+    """You can remove an item from a list source."""
     listener = Mock()
     source.add_listener(listener)
 
     # Remove the second element
     row = source[1]
     source.remove(row)
 
@@ -352,15 +352,15 @@
     assert source[1].val1 == "third"
     assert source[1].val2 == 333
 
     listener.remove.assert_called_once_with(item=row, index=1)
 
 
 def test_index(source):
-    "You can get the index of any row within a list source"
+    """You can get the index of any row within a list source."""
     for i, row in enumerate(source):
         assert i == source.index(row)
 
     # look-alike rows are not equal, so index lookup should fail
     lookalike_row = Row(val1="second", val2=222)
     with pytest.raises(
         ValueError,
@@ -378,15 +378,15 @@
         ValueError,
         match=r"<Row .* \(no attributes\)> is not in list",
     ):
         source.index(Row())
 
 
 def test_find(source):
-    "You can find the index of any matching row within a list source"
+    """You can find the index of any matching row within a list source."""
 
     # Duplicate row 1 of the data.
     source.append(dict(val1="second", val2=222))
 
     # A unique row can be found
     assert source.find(dict(val1="third", val2=333)) == source[2]
```

### Comparing `toga-core-0.4.2/tests/sources/test_node.py` & `toga_core-0.4.3/tests/sources/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 
 from toga.sources import Node
 
 
 def _create_node(source, parent, data, children=None):
-    "A very simplified _create_node for mock purposes"
+    """A very simplified _create_node for mock purposes."""
     node = Node(**data)
     node._source = source
     node._parent = parent
     if children:
         node._children = [
             _create_node(source, parent=node, data=item[0], children=item[1])
             for item in children
@@ -64,48 +64,48 @@
 def node(leaf_node, child_a, child_b):
     leaf_node._children = [child_a, child_b]
 
     return leaf_node
 
 
 def test_node_properties(node):
-    "An node with children can be created and modified"
+    """A node with children can be created and modified."""
     assert node.val1 == "value 1"
     assert node.val2 == 42
     assert node.can_have_children()
     assert len(node) == 2
     assert (
         re.match(r"<Node .* val1='value 1' val2=42; 2 children>", repr(node))
         is not None
     )
 
 
 def test_empty_node_properties(empty_node):
-    "An empty Node can be created"
+    """An empty Node can be created."""
     assert empty_node.can_have_children()
     assert len(empty_node) == 0
     assert (
         re.match(r"<Node .* \(no attributes\); 0 children>", repr(empty_node))
         is not None
     )
 
 
 def test_leaf_node_properties(leaf_node):
-    "A Leaf Node can be created"
+    """A Leaf Node can be created."""
     assert leaf_node.val1 == "value 1"
     assert leaf_node.val2 == 42
     assert not leaf_node.can_have_children()
     assert len(leaf_node) == 0
     assert (
         re.match(r"<Leaf Node .* val1='value 1' val2=42>", repr(leaf_node)) is not None
     )
 
 
 def test_modify_attributes(source, node):
-    """If node attributes are modified, a change notification is sent"""
+    """If node attributes are modified, a change notification is sent."""
     node.val1 = "new value"
     assert node.val1 == "new value"
     source.notify.assert_called_once_with("change", item=node)
     source.notify.reset_mock()
 
     # Deleting an attribute causes a change notification
     del node.val1
@@ -135,15 +135,15 @@
     del node.val3
     assert not hasattr(node, "val3")
     source.notify.assert_called_once_with("change", item=node)
     source.notify.reset_mock()
 
 
 def test_modify_attributes_no_source(node):
-    """Node attributes can be modified on a node with no source"""
+    """Node attributes can be modified on a node with no source."""
     node.source = None
 
     node.val1 = "new value"
     assert node.val1 == "new value"
 
     # Deleting an attribute causes a change notification
     del node.val1
@@ -165,15 +165,15 @@
     # Deleting an attribute that wasn't in the original attribute set
     # still causes a change notification
     del node.val3
     assert not hasattr(node, "val3")
 
 
 def test_modify_children(source, node):
-    """Node children can be retrieved and modified"""
+    """Node children can be retrieved and modified."""
     child = node[1]
     assert node[1].val1 == "value b"
 
     # Delete the child
     del node[1]
 
     # Removal notification was sent
@@ -206,15 +206,15 @@
     source.notify.assert_called_once_with("change", item=node[0])
 
     # Node child count hasn't changed
     assert len(node) == 1
 
 
 def test_modify_leaf_children(leaf_node):
-    """Attempts to modifying Leaf Node children raise an error"""
+    """Attempts to modifying Leaf Node children raise an error."""
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .*> is a leaf node",
     ):
         leaf_node[1]
 
     with pytest.raises(
@@ -227,34 +227,34 @@
         ValueError,
         match=r"<Leaf Node .*> is a leaf node",
     ):
         leaf_node[1] = {"val1": "new"}
 
 
 def test_iterate(node):
-    """Node can be iterated"""
+    """Node can be iterated."""
     assert "|".join(child.val1 for child in node) == "value a|value b"
 
 
 def test_iterate_leaf(leaf_node):
-    """Node can be iterated"""
+    """Node can be iterated."""
     assert "|".join(child.val1 for child in leaf_node) == ""
 
 
 @pytest.mark.parametrize(
     "index, actual_index",
     [
         (1, 1),  # Positive, in range
         (10, 2),  # Positive, past positive limit
         (-1, 1),  # Negative, in range
         (-10, 0),  # Negative, past negative limit
     ],
 )
 def test_insert(source, node, index, actual_index):
-    """A child can be inserted into a node"""
+    """A child can be inserted into a node."""
     new_child = node.insert(index, {"val1": "new"})
 
     # Node has one more child.
     assert len(node) == 3
     assert node[actual_index] == new_child
 
     # A child node was created using the source's factory
@@ -268,15 +268,15 @@
         parent=node,
         index=actual_index,
         item=new_child,
     )
 
 
 def test_insert_with_children(source, node):
-    """A child with children can be inserted into a node"""
+    """A child with children can be inserted into a node."""
     new_child = node.insert(
         1,
         {"val1": "new"},
         children=[
             ({"val1": "new child 1"}, None),
             ({"val1": "new child 2"}, None),
         ],
@@ -308,15 +308,15 @@
         parent=node,
         index=1,
         item=new_child,
     )
 
 
 def test_insert_leaf(leaf_node, source):
-    """Inserting a child into a leaf makes the node not a leaf any more"""
+    """Inserting a child into a leaf makes the node not a leaf any more."""
     new_child = leaf_node.insert(0, {"val1": "new"})
 
     # Leaf node isn't a leaf any more
     assert leaf_node.can_have_children()
     assert len(leaf_node) == 1
     assert leaf_node[0] == new_child
 
@@ -328,15 +328,15 @@
     # insert notification was sent, the change is associated with the new item
     source.notify.assert_called_once_with(
         "insert", parent=leaf_node, index=0, item=leaf_node[0]
     )
 
 
 def test_append(source, node):
-    """A child can be appended onto a node"""
+    """A child can be appended onto a node."""
     new_child = node.append({"val1": "new"})
 
     # Node has one more child.
     assert len(node) == 3
     assert node[2] == new_child
 
     # A child node was created using the source's factory
@@ -350,15 +350,15 @@
         parent=node,
         index=2,
         item=new_child,
     )
 
 
 def test_append_with_children(source, node):
-    """A child with children can be appended onto a node"""
+    """A child with children can be appended onto a node."""
     new_child = node.append(
         {"val1": "new"},
         children=[
             ({"val1": "new child 1"}, None),
             ({"val1": "new child 2"}, None),
         ],
     )
@@ -384,15 +384,15 @@
         parent=node,
         index=2,
         item=new_child,
     )
 
 
 def test_append_leaf(leaf_node, source):
-    """Appending to a leaf makes the node not a leaf any more"""
+    """Appending to a leaf makes the node not a leaf any more."""
     new_child = leaf_node.append({"val1": "new"})
 
     # Leaf node isn't a leaf any more
     assert leaf_node.can_have_children()
     assert len(leaf_node) == 1
     assert leaf_node[0] == new_child
 
@@ -404,40 +404,40 @@
     # insert notification was sent, the change is associated with the new item
     source.notify.assert_called_once_with(
         "insert", parent=leaf_node, index=0, item=leaf_node[0]
     )
 
 
 def test_index(node, child_b):
-    """A child can be found it it's parent"""
+    """A child can be found it it's parent."""
     assert node.index(child_b) == 1
 
 
 def test_index_not_child(node):
-    """If a node isn't a child of this node, it can't be found by index"""
+    """If a node isn't a child of this node, it can't be found by index."""
     other = Node(val1="other")
 
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .* val1='other'> is not in list",
     ):
         node.index(other)
 
 
 def test_index_leaf(leaf_node, child_b):
-    """A child cannot be found in a leaf node"""
+    """A child cannot be found in a leaf node."""
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .* val1='value 1' val2=42> is a leaf node",
     ):
         leaf_node.index(child_b)
 
 
 def test_remove(source, node, child_b):
-    """A node can be removed from it's parent"""
+    """A node can be removed from it's parent."""
     # Child is initially associated with the node
     assert child_b._parent == node
     assert child_b._source == node._source
 
     # Remove the child
     node.remove(child_b)
 
@@ -449,24 +449,24 @@
     assert len(node) == 1
 
     # The source was notified
     source.notify.assert_called_once_with("remove", parent=node, index=1, item=child_b)
 
 
 def test_remove_leaf(leaf_node, child_b):
-    """A child cannot be removed from a leaf node"""
+    """A child cannot be removed from a leaf node."""
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .* val1='value 1' val2=42> is a leaf node",
     ):
         leaf_node.index(child_b)
 
 
 def test_find(node, child_b):
-    """A node can be found by value in it's parent's list of children"""
+    """A node can be found by value in it's parent's list of children."""
     # Append some additional children
     child_c = node.append({"val1": "value a", "val2": 333})
     child_d = node.append({"val1": "value b", "val2": 444})
 
     # Find the child by a partial match of values.
     assert node.find({"val1": "value b"}) == child_b
 
@@ -474,13 +474,13 @@
     assert node.find({"val1": "value b"}, start=child_b) == child_d
 
     # Find the child by a full match of values, starting at the first match
     assert node.find({"val1": "value a", "val2": 333}) == child_c
 
 
 def test_found_leaf(leaf_node):
-    """A child cannot be foundd from a leaf node"""
+    """A child cannot be found from a leaf node."""
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .* val1='value 1' val2=42> is a leaf node",
     ):
         leaf_node.find({"val1": "value 1"})
```

### Comparing `toga-core-0.4.2/tests/sources/test_row.py` & `toga_core-0.4.3/tests/sources/test_row.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import Mock
 
 from toga.sources import Row
 
 
 def test_row():
-    "A row can be created and modified"
+    """A row can be created and modified."""
     source = Mock()
     row = Row(val1="value 1", val2=42)
     # Set a source.
     row._source = source
 
     # initial values are as expected
     assert row.val1 == "value 1"
@@ -43,30 +43,30 @@
     del row.val3
     assert not hasattr(row, "val")
     source.notify.assert_called_once_with("change", item=row)
     source.notify.reset_mock()
 
 
 def test_row_without_source():
-    "A row with no source can be created and modified"
+    """A row with no source can be created and modified."""
     row = Row(val1="value 1", val2=42)
 
     # initial values are as expected
     assert row.val1 == "value 1"
     assert row.val2 == 42
 
     # An existing attribute can be updated.
     row.val1 = "new value"
     assert row.val1 == "new value"
 
     # Deleting an attribute causes a change notification
     del row.val1
     assert not hasattr(row, "val1")
 
-    # Setting an attribute starting with with an underscore isn't a notifiable event
+    # Setting an attribute starting with an underscore isn't a notifiable event
     row._secret = "secret value"
     assert row._secret == "secret value"
 
     # An attribute that wasn't in the original attribute set
     # still causes a change notification
     row.val3 = "other value"
     assert row.val3 == "other value"
```

### Comparing `toga-core-0.4.2/tests/sources/test_source.py` & `toga_core-0.4.3/tests/sources/test_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     # Activate listeners; listener2 not notified.
     source.notify("message5")
     listener1.message5.assert_called_once_with()
     listener2.message5.assert_not_called()
 
 
 def test_missing_listener_method():
-    """If a listener doesn't implement a notification method, the notification is ignored"""
+    """If a listener doesn't implement a notification method, the notification is
+    ignored."""
     full_listener = Mock()
     partial_listener = object()
     source = Source()
 
     source.add_listener(full_listener)
     source.add_listener(partial_listener)
     assert source.listeners == [full_listener, partial_listener]
```

### Comparing `toga-core-0.4.2/tests/sources/test_tree_source.py` & `toga_core-0.4.3/tests/sources/test_tree_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,33 +61,33 @@
     [
         None,
         42,
         "not a list",
     ],
 )
 def test_invalid_accessors(value):
-    "Accessors for a list source must be a list of attribute names"
+    """Accessors for a list source must be a list of attribute names."""
     with pytest.raises(
         ValueError,
         match=r"accessors should be a list of attribute names",
     ):
         TreeSource(accessors=value)
 
 
 def test_accessors_required():
-    "A list source must specify *some* accessors"
+    """A list source must specify *some* accessors."""
     with pytest.raises(
         ValueError,
         match=r"TreeSource must be provided a list of accessors",
     ):
         TreeSource(accessors=[], data=[1, 2, 3])
 
 
 def test_accessors_copied():
-    "A list source must specify *some* accessors"
+    """A list source must specify *some* accessors."""
     accessors = ["foo", "bar"]
     source = TreeSource(accessors)
 
     assert source._accessors == ["foo", "bar"]
 
     # The accessors have been copied.
     accessors.append("whiz")
@@ -98,15 +98,15 @@
     "data",
     [
         {},
         [],
     ],
 )
 def test_create_empty(data):
-    """An empty TreeSource can be created"""
+    """An empty TreeSource can be created."""
     source = TreeSource(data=data, accessors=["val1", "val2"])
 
     assert len(source) == 0
 
 
 @pytest.mark.parametrize(
     "data, all_accessor_levels",
@@ -266,15 +266,15 @@
                 ),
             ],
             {0, 2},  # all accessors at first and last level
         ),
     ],
 )
 def test_create(data, all_accessor_levels):
-    """A tree source can be created from data in different formats"""
+    """A tree source can be created from data in different formats."""
     source = TreeSource(data=data, accessors=["val1", "val2"])
 
     # Source has 2 roots
     assert len(source) == 2
 
     # Root0 has 2 children
     assert source[0].val1 == "root0"
@@ -351,23 +351,23 @@
         assert source[0][2][1].val2 == 132
 
         assert source[1][2][0].val2 == 231
         assert source[1][2][1].val2 == 232
 
 
 def test_source_single_object():
-    """A single object can be passed as root data"""
+    """A single object can be passed as root data."""
     source = TreeSource(accessors=["val1", "val2"], data="A string")
 
     assert len(source) == 1
     assert source[0].val1 == "A string"
 
 
 def test_single_object_child():
-    """A single object can be passed as child data"""
+    """A single object can be passed as child data."""
     source = TreeSource(
         accessors=["val1", "val2"],
         data={("root1", 1): "A string"},
     )
 
     assert len(source) == 1
     assert source[0].val1 == "root1"
@@ -415,20 +415,20 @@
     listener.change.assert_called_once_with(item=source[0])
 
     # Source's root count hasn't changed
     assert len(source) == 1
 
 
 def test_iter_root(source):
-    """The roots of a source can be iterated over"""
+    """The roots of a source can be iterated over."""
     assert "|".join(root.val1 for root in source) == "group1|group2"
 
 
 def test_clear(source, listener):
-    """A TreeSource can be cleared"""
+    """A TreeSource can be cleared."""
     source.clear()
 
     assert len(source) == 0
 
     # Clear notification was sent
     listener.clear.assert_called_once_with()
 
@@ -439,15 +439,15 @@
         (1, 1),  # Positive, in range
         (10, 2),  # Positive, past positive limit
         (-1, 1),  # Negative, in range
         (-10, 0),  # Negative, past negative limit
     ],
 )
 def test_insert(source, listener, index, actual_index):
-    """A new root node can be inserted"""
+    """A new root node can be inserted."""
     new_child = source.insert(index, {"val1": "new"})
 
     # Source has one more root.
     assert len(source) == 3
     assert source[actual_index] == new_child
 
     # Root data is as expected
@@ -458,15 +458,15 @@
         parent=None,
         index=actual_index,
         item=new_child,
     )
 
 
 def test_insert_with_children(source, listener):
-    """A new root node can be inserted with children"""
+    """A new root node can be inserted with children."""
     new_child = source.insert(
         1,
         {"val1": "new"},
         children=[
             ({"val1": "new child 1"}, None),
             ({"val1": "new child 2"}, None),
         ],
@@ -491,15 +491,15 @@
         parent=None,
         index=1,
         item=new_child,
     )
 
 
 def test_append(source, listener):
-    """A new root node can be appended"""
+    """A new root node can be appended."""
     new_child = source.append({"val1": "new"})
 
     # Source has one more root.
     assert len(source) == 3
     assert source[2] == new_child
 
     # Root data is as expected
@@ -510,15 +510,15 @@
         parent=None,
         index=2,
         item=new_child,
     )
 
 
 def test_append_with_children(source, listener):
-    """A new root node can be inserted with children"""
+    """A new root node can be inserted with children."""
     new_child = source.append(
         {"val1": "new"},
         children=[
             ({"val1": "new child 1"}, None),
             ({"val1": "new child 2"}, None),
         ],
     )
@@ -542,66 +542,66 @@
         parent=None,
         index=2,
         item=new_child,
     )
 
 
 def test_remove_root(source, listener):
-    """A root node can be removed"""
+    """A root node can be removed."""
     root = source[1]
     source.remove(root)
 
     # One less item in the source
     assert len(source) == 1
 
     # The root is no longer associated with the source
     assert root._source is None
 
     # Removal notification was sent
     listener.remove.assert_called_once_with(parent=None, index=1, item=root)
 
 
 def test_remove_child(source, listener):
-    """A child node can be removed from a source"""
+    """A child node can be removed from a source."""
     node = source[1][1]
     source.remove(node)
 
     # The source still has 2 roots
     assert len(source) == 2
     # ... but there's 1 less child
     assert len(source[1]) == 2
 
     # The child is no longer associated with the source,
-    # and the child isn't associated with it's parent.
+    # and the child isn't associated with its parent.
     assert node._source is None
     assert node._parent is None
 
     # Removal notification was sent
     listener.remove.assert_called_once_with(parent=source[1], index=1, item=node)
 
 
 def test_remove_non_root(source, listener):
-    """If a node isn't associated with this source, remove raises an error"""
+    """If a node isn't associated with this source, remove raises an error."""
     other = Node(val="other")
 
     with pytest.raises(
         ValueError,
         match=r"<Leaf Node .*> is not managed by this data source",
     ):
         source.remove(other)
 
 
 def test_index(source):
-    """A root can be found in a TreeSource"""
+    """A root can be found in a TreeSource."""
     root = source[1]
     assert source.index(root) == 1
 
 
 def test_find(source):
-    """A node can be found by value"""
+    """A node can be found by value."""
     root1 = source[1]
 
     # Append some additional roots
     root2 = source.append({"val1": "group1", "val2": 333})
     root3 = source.append({"val1": "group2", "val2": 444})
 
     # Find the child by a partial match of values.
```

### Comparing `toga-core-0.4.2/tests/sources/test_value_source.py` & `toga_core-0.4.3/tests/sources/test_value_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from unittest.mock import Mock
 
 from toga.sources.value_source import ValueSource
 
 
 def test_empty():
-    """An empty ValueSource can be created"""
+    """An empty ValueSource can be created."""
     source = ValueSource()
 
     assert source.accessor == "value"
     assert source.value is None
     assert str(source) == "None"
 
 
 def test_value():
-    """A ValueSource can be created with a value"""
+    """A ValueSource can be created with a value."""
     source = ValueSource(42)
 
     assert source.accessor == "value"
     assert source.value == 42
     assert str(source) == "42"
 
 
 def test_value_with_accessor():
-    """A ValueSource can be created with a custom accessro"""
+    """A ValueSource can be created with a custom accessor."""
     source = ValueSource(42, accessor="something")
 
     assert source.accessor == "something"
     assert source.something == 42
     assert str(source) == "42"
 
 
 def test_listener():
-    """A listener will be notified of ValueSource changes"""
+    """A listener will be notified of ValueSource changes."""
     source = ValueSource(42)
     listener = Mock()
 
     source.add_listener(listener)
 
     source.value = 37
```

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_beeliza.py` & `toga_core-0.4.3/tests/style/pack/layout/test_beeliza.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_column_alignment.py` & `toga_core-0.4.3/tests/style/pack/layout/test_column_alignment.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_fixed.py` & `toga_core-0.4.3/tests/style/pack/layout/test_fixed.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from toga.style.pack import COLUMN, ROW, Pack
 
 from ..utils import ExampleNode, ExampleViewport, assert_layout
 
 
 def test_row_expanding_intrinsic():
-    "Children in a row layout with fixed size don't expand, even if their hints allow it"
+    """Children in a row layout with fixed size don't expand, even if their hints allow
+    it."""
     root = ExampleNode(
         "app",
         style=Pack(direction=ROW),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(width=100, height=100),
@@ -62,15 +63,16 @@
                 },
             ],
         },
     )
 
 
 def test_row_fixed_intrinsic():
-    "Children in a row layout without an explicit size, but a fixed intrinsic width, don't expand"
+    """Children in a row layout without an explicit size, but a fixed intrinsic width,
+    don't expand."""
     root = ExampleNode(
         "app",
         style=Pack(direction=ROW),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(),
@@ -121,15 +123,16 @@
                 },
             ],
         },
     )
 
 
 def test_column_expanding_intrinsic():
-    "Children in a column layout with fixed size don't expand, even if their hints allow it"
+    """Children in a column layout with fixed size don't expand, even if their hints
+    allow it."""
     root = ExampleNode(
         "app",
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(width=100, height=100),
@@ -179,15 +182,16 @@
                 },
             ],
         },
     )
 
 
 def test_column_fixed_intrinsic():
-    "Children in a column layout without an explicit size, but a fixed intrinsic width, don't expand"
+    """Children in a column layout without an explicit size, but a fixed intrinsic
+    width, don't expand."""
     root = ExampleNode(
         "app",
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(),
```

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_flex.py` & `toga_core-0.4.3/tests/style/pack/layout/test_flex.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,15 @@
         },
     )
 
 
 def test_row_flex_insufficient_space_no_flex():
     """Children in a row layout with flexible containers, but insufficient_space for any
     of the flexible content, and an explicit intrinsic width, doesn't collapse row
-    height.
-    """
+    height."""
     root = ExampleNode(
         "app",
         style=Pack(direction=ROW),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(flex=1),
@@ -273,15 +272,15 @@
                 },
             ],
         },
     )
 
 
 def test_row_flex_grandchild_min_size():
-    """The minimum intrinsic sizes of grandchild of flex row containers are honored"""
+    """The minimum intrinsic sizes of grandchild of flex row containers are honored."""
     root = ExampleNode(
         "app",
         size=(at_least(0), at_least(0)),
         style=Pack(direction=ROW),
         children=[
             ExampleNode(
                 "inner",
@@ -325,16 +324,16 @@
                 },
             ],
         },
     )
 
 
 def test_column_flex_no_hints():
-    """Children in a column layout with flexible containers, but no flex hints,
-    doesn't collapse column width."""
+    """Children in a column layout with flexible containers, but no flex hints, doesn't
+    collapse column width."""
     root = ExampleNode(
         "app",
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "first",
                 style=Pack(flex=1),
@@ -455,16 +454,15 @@
             ],
         },
     )
 
 
 def test_column_flex_insufficient_space():
     """Children in a column layout with flexible containers, but insufficient space to
-    accommodate them, and an explicit intrinsic width, doesn't collapse column width.
-    """
+    accommodate them, and an explicit intrinsic width, doesn't collapse column width."""
 
     root = ExampleNode(
         "app",
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "first",
@@ -538,16 +536,15 @@
         },
     )
 
 
 def test_column_flex_insufficient_space_no_flex():
     """Children in a column layout with flexible containers, but insufficient space for
     any of the flexible content, and an explicit intrinsic width, doesn't collapse
-    column width.
-    """
+    column width."""
 
     root = ExampleNode(
         "app",
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "first",
@@ -599,15 +596,16 @@
                 },
             ],
         },
     )
 
 
 def test_column_flex_grandchild_min_size():
-    """The minimum intrinsic sizes of grandchild of flex column containers are honored"""
+    """The minimum intrinsic sizes of grandchild of flex column containers are
+    honored."""
     root = ExampleNode(
         "app",
         size=(at_least(0), at_least(0)),
         style=Pack(direction=COLUMN),
         children=[
             ExampleNode(
                 "inner",
```

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_row_alignment.py` & `toga_core-0.4.3/tests/style/pack/layout/test_row_alignment.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_rtl.py` & `toga_core-0.4.3/tests/style/pack/layout/test_rtl.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_tutorial0.py` & `toga_core-0.4.3/tests/style/pack/layout/test_tutorial0.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_tutorial1.py` & `toga_core-0.4.3/tests/style/pack/layout/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/layout/test_tutorial3.py` & `toga_core-0.4.3/tests/style/pack/layout/test_tutorial3.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/test_apply.py` & `toga_core-0.4.3/tests/style/pack/test_apply.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/style/pack/test_css.py` & `toga_core-0.4.3/tests/style/pack/test_css.py`

 * *Files identical despite different names*

```diff
@@ -471,9 +471,9 @@
                 "font-variant: small-caps;"
             ),
             id="font-full",
         ),
     ],
 )
 def test_rendering(style, expected_css):
-    """An empty style node can be rendered"""
+    """An empty style node can be rendered."""
     assert style.__css__() == expected_css
```

### Comparing `toga-core-0.4.2/tests/style/pack/utils.py` & `toga_core-0.4.3/tests/style/pack/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         self.refresh = Mock()
 
     def __repr__(self):
         return f"<{self.name}>"
 
     def __html__(self, depth=0):
-        "Debugging helper - output the HTML interpretation of this layout"
+        """Debugging helper - output the HTML interpretation of this layout"""
         if depth:
             tag = "div"
         else:
             tag = "body"
         lines = []
 
         # Add an interpretation of intrinsic width
```

### Comparing `toga-core-0.4.2/tests/style/test_applicator.py` & `toga_core-0.4.3/tests/style/test_applicator.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     widget = ExampleWidget(id="widget_id")
     widget.add(child)
 
     return widget
 
 
 def test_refresh(widget):
-    "Refresh requests are passed to the widget"
+    """Refresh requests are passed to the widget."""
     widget.applicator.refresh()
 
     assert_action_performed_with(widget, "refresh")
 
 
 def test_set_bounds(widget, child, grandchild):
-    "Bounds changes are passed to all widgets in the tree"
+    """Bounds changes are passed to all widgets in the tree."""
     # Manually set location of the parent
     widget.layout._origin_left = 100
     widget.layout._origin_top = 200
     widget.layout.content_width = 300
     widget.layout.content_height = 400
 
     # Manually set location of the child
@@ -68,26 +68,26 @@
 
     # Manually set location of the grandchild
     grandchild.layout._origin_left = 1
     grandchild.layout._origin_top = 2
     grandchild.layout.content_width = 3
     grandchild.layout.content_height = 4
 
-    # Propegate the boundsq
+    # Propagate the bounds
     widget.applicator.set_bounds()
 
     assert_action_performed_with(
         widget, "set bounds", x=100, y=200, width=300, height=400
     )
     assert_action_performed_with(child, "set bounds", x=10, y=20, width=30, height=40)
     assert_action_performed_with(grandchild, "set bounds", x=1, y=2, width=3, height=4)
 
 
 def test_text_alignment(widget):
-    "Text alignment can be set on a widget"
+    """Text alignment can be set on a widget."""
     widget.applicator.set_text_alignment(RIGHT)
 
     assert_action_performed_with(widget, "set alignment", alignment=RIGHT)
 
 
 @pytest.mark.parametrize(
     "child_visibility, grandchild_visibility, value, "
@@ -132,25 +132,25 @@
 
     # The style property of the child and grandchild hasn't changed.
     assert child.style.visibility == child_visibility
     assert grandchild.style.visibility == grandchild_visibility
 
 
 def test_set_font(widget):
-    "A font change can be applied to a widget"
+    """A font change can be applied to a widget."""
     widget.applicator.set_font(FANTASY)
 
     assert_action_performed_with(widget, "set font", font=FANTASY)
 
 
 def test_set_color(widget):
-    "A color change can be applied to a widget"
+    """A color change can be applied to a widget."""
     widget.applicator.set_color(REBECCAPURPLE)
 
     assert_action_performed_with(widget, "set color", color=REBECCAPURPLE)
 
 
 def test_set_background_color(child, widget):
-    "A background color change can be applied to a widget"
+    """A background color change can be applied to a widget."""
     widget.applicator.set_background_color(REBECCAPURPLE)
 
     assert_action_performed_with(widget, "set background color", color=REBECCAPURPLE)
```

### Comparing `toga-core-0.4.2/tests/test_documents.py` & `toga_core-0.4.3/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/test_fonts.py` & `toga_core-0.4.3/tests/test_fonts.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             NORMAL,
             NORMAL,
             "system default size",
         ),
     ],
 )
 def test_builtin_font(family, size, weight, style, variant, as_str):
-    "A builtin font can be constructed"
+    """A builtin font can be constructed."""
     font = toga.Font(
         family=family,
         size=size,
         style=style,
         weight=weight,
         variant=variant,
     )
@@ -129,15 +129,15 @@
         # Unknown style/weight/variants are normalized to "NORMAL"
         ("Wonky", "unknown", ITALIC, SMALL_CAPS, ("Wonky", NORMAL, ITALIC, SMALL_CAPS)),
         ("Wonky", BOLD, "unknown", SMALL_CAPS, ("Wonky", BOLD, NORMAL, SMALL_CAPS)),
         ("Wonky", BOLD, ITALIC, "unknown", ("Wonky", BOLD, ITALIC, NORMAL)),
     ],
 )
 def test_registered_font_key(app, family, style, weight, variant, key):
-    "Registered font keys can be generarted"
+    """Registered font keys can be generated."""
     assert (
         toga.Font._registered_font_key(
             family, style=style, weight=weight, variant=variant
         )
         == key
     )
 
@@ -156,15 +156,15 @@
         (
             "path/to/custom/font.otf",
             Path(toga.__file__).parent / "path/to/custom/font.otf",
         ),
     ],
 )
 def test_register_font(app, path, registered):
-    "A custom font can be registered"
+    """A custom font can be registered."""
     toga.Font.register("Custom Font", path)
 
     # Test fixture has paths in Path format; fully resolve for test comparison. This
     # gets around Windows path separator and absolute path discrepancies.
     assert (
         Path(_REGISTERED_FONT_CACHE[("Custom Font", NORMAL, NORMAL, NORMAL)]).resolve()
         == registered.resolve()
@@ -185,15 +185,15 @@
         (
             str(Path("path/to/custom/font.otf")),
             Path(toga.__file__).parent / "path/to/custom/font.otf",
         ),
     ],
 )
 def test_register_font_variant(app, path, registered):
-    "A custom font can be registered as a variant"
+    """A custom font can be registered as a variant."""
     toga.Font.register("Custom Font", path, weight=BOLD)
 
     # Test fixture has paths in Path format; fully resolve for test comparison. This
     # gets around Windows path separator and absolute path discrepancies.
     assert (
         Path(_REGISTERED_FONT_CACHE[("Custom Font", BOLD, NORMAL, NORMAL)]).resolve()
         == registered.resolve()
```

### Comparing `toga-core-0.4.2/tests/test_handlers.py` & `toga_core-0.4.3/tests/test_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 
 class ExampleAsyncResult(AsyncResult):
     RESULT_TYPE = "Test"
 
 
 def test_noop_handler():
-    """None can be wrapped as a valid handler"""
+    """None can be wrapped as a valid handler."""
     obj = Mock()
 
     wrapped = wrapped_handler(obj, None)
 
     assert wrapped._raw is None
 
     # This does nothing, but doesn't raise an error.
     wrapped("arg1", "arg2", kwarg1=3, kwarg2=4)
 
 
 def test_noop_handler_with_cleanup():
-    """cleanup is still performed when a no-op handler is used"""
+    """Cleanup is still performed when a no-op handler is used."""
     obj = Mock()
     cleanup = Mock()
 
     wrapped = wrapped_handler(obj, None, cleanup=cleanup)
 
     assert wrapped._raw is None
 
@@ -35,15 +35,15 @@
     wrapped("arg1", "arg2", kwarg1=3, kwarg2=4)
 
     # Cleanup method was invoked
     cleanup.assert_called_once_with(obj, None)
 
 
 def test_noop_handler_with_cleanup_error(capsys):
-    """If cleanup on a no-op handler raises an error, it is logged"""
+    """If cleanup on a no-op handler raises an error, it is logged."""
     obj = Mock()
     cleanup = Mock(side_effect=Exception("Problem in cleanup"))
 
     wrapped = wrapped_handler(obj, None, cleanup=cleanup)
 
     assert wrapped._raw is None
 
@@ -57,15 +57,15 @@
     assert (
         "Error in handler cleanup: Problem in cleanup\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_function_handler():
-    """A function can be used as a handler"""
+    """A function can be used as a handler."""
     obj = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
 
@@ -81,15 +81,15 @@
     assert handler_call == {
         "args": (obj, "arg1", "arg2"),
         "kwargs": {"kwarg1": 3, "kwarg2": 4},
     }
 
 
 def test_function_handler_error(capsys):
-    """A function handler can raise an error"""
+    """A function handler can raise an error."""
     obj = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
         raise Exception("Problem in handler")
@@ -111,15 +111,15 @@
     assert (
         "Error in handler: Problem in handler\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_function_handler_with_cleanup():
-    """A function handler can have a cleanup method"""
+    """A function handler can have a cleanup method."""
     obj = Mock()
     cleanup = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
@@ -175,15 +175,15 @@
     assert (
         "Error in handler cleanup: Problem in cleanup\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_generator_handler(event_loop):
-    """A generator can be used as a handler"""
+    """A generator can be used as a handler."""
     obj = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
         yield 0.01  # A short sleep
@@ -212,15 +212,15 @@
         "kwargs": {"kwarg1": 3, "kwarg2": 4},
         "slept": True,
         "done": True,
     }
 
 
 def test_generator_handler_error(event_loop, capsys):
-    """A generator can raise an error"""
+    """A generator can raise an error."""
     obj = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
         yield 0.01  # A short sleep
@@ -251,15 +251,15 @@
     assert (
         "Error in long running handler: Problem in handler\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_generator_handler_with_cleanup(event_loop):
-    """A generator can have cleanup"""
+    """A generator can have cleanup."""
     obj = Mock()
     cleanup = Mock()
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
@@ -293,15 +293,15 @@
     }
 
     # Cleanup method was invoked
     cleanup.assert_called_once_with(obj, 42)
 
 
 def test_generator_handler_with_cleanup_error(event_loop, capsys):
-    """A generator can raise an error during cleanup"""
+    """A generator can raise an error during cleanup."""
     obj = Mock()
     cleanup = Mock(side_effect=Exception("Problem in cleanup"))
     handler_call = {}
 
     def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
@@ -341,15 +341,15 @@
     assert (
         "Error in long running handler cleanup: Problem in cleanup\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_coroutine_handler(event_loop):
-    """A coroutine can be used as a handler"""
+    """A coroutine can be used as a handler."""
     obj = Mock()
     handler_call = {}
 
     async def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
         await asyncio.sleep(0.01)  # A short sleep
@@ -375,15 +375,15 @@
         "args": (obj, "arg1", "arg2"),
         "kwargs": {"kwarg1": 3, "kwarg2": 4},
         "done": True,
     }
 
 
 def test_coroutine_handler_error(event_loop, capsys):
-    """A coroutine can raise an error"""
+    """A coroutine can raise an error."""
     obj = Mock()
     handler_call = {}
 
     async def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
         await asyncio.sleep(0.01)  # A short sleep
@@ -414,15 +414,15 @@
     assert (
         "Error in async handler: Problem in handler\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_coroutine_handler_with_cleanup(event_loop):
-    """A coroutine can have cleanup"""
+    """A coroutine can have cleanup."""
     obj = Mock()
     cleanup = Mock()
     handler_call = {}
 
     async def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
@@ -453,15 +453,15 @@
     }
 
     # Cleanup method was invoked
     cleanup.assert_called_once_with(obj, 42)
 
 
 def test_coroutine_handler_with_cleanup_error(event_loop, capsys):
-    """A coroutine can raise an error during cleanup"""
+    """A coroutine can raise an error during cleanup."""
     obj = Mock()
     cleanup = Mock(side_effect=Exception("Problem in cleanup"))
     handler_call = {}
 
     async def handler(*args, **kwargs):
         handler_call["args"] = args
         handler_call["kwargs"] = kwargs
@@ -498,28 +498,28 @@
     assert (
         "Error in async handler cleanup: Problem in cleanup\nTraceback (most recent call last):\n"
         in capsys.readouterr().err
     )
 
 
 def test_native_handler():
-    """A native function can be used as a handler"""
+    """A native function can be used as a handler."""
     obj = Mock()
     native_method = Mock()
 
     handler = NativeHandler(native_method)
 
     wrapped = wrapped_handler(obj, handler)
 
     # Native method is returned as the handler.
     assert wrapped == native_method
 
 
 def test_async_result_non_comparable(event_loop):
-    """An async result can't be compared or evaluated"""
+    """An async result can't be compared or evaluated."""
     result = ExampleAsyncResult(None)
 
     # repr for the result is useful
     assert repr(result) == "<Async Test result; future=<Future pending>>"
 
     # Result cannot be compared.
 
@@ -557,53 +557,53 @@
         RuntimeError,
         match=r"Can't check Test result directly; use await or an on_result handler",
     ):
         result != 42
 
 
 def test_async_result(event_loop):
-    """An async result can be set"""
+    """An async result can be set."""
     result = ExampleAsyncResult()
 
     result.set_result(42)
 
     # Evaluate the future
     async_answer = event_loop.run_until_complete(result.future)
 
     # The answer was returned, and passed to the callback
     assert async_answer == 42
 
 
 def test_async_result_cancelled(event_loop):
-    """An async result can be set even if the future is cancelled"""
+    """An async result can be set even if the future is cancelled."""
     result = ExampleAsyncResult()
 
     # cancel the future.
     result.future.cancel()
 
     result.set_result(42)
 
     # Evaluate the future. This will raise an error
     with pytest.raises(asyncio.CancelledError):
         event_loop.run_until_complete(result.future)
 
 
 def test_async_exception(event_loop):
-    """An async result can raise an exception"""
+    """An async result can raise an exception."""
     result = ExampleAsyncResult()
 
     result.set_exception(ValueError("Bad stuff"))
 
     # Evaluate the future; this will raise an exception
     with pytest.raises(ValueError, match=r"Bad stuff"):
         event_loop.run_until_complete(result.future)
 
 
 def test_async_exception_cancelled(event_loop):
-    """An async result can raise an exception even if the future is cancelled"""
+    """An async result can raise an exception even if the future is cancelled."""
     result = ExampleAsyncResult()
 
     # Cancel the future
     result.future.cancel()
 
     result.set_exception(ValueError("Bad stuff"))
 
@@ -614,15 +614,15 @@
 
 ######################################################################
 # 2023-12: Backwards compatibility
 ######################################################################
 
 
 def test_async_result_sync(event_loop):
-    """The deprecated behavior of using a synchronous result handler is supported"""
+    """The deprecated behavior of using a synchronous result handler is supported."""
     on_result = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         result = ExampleAsyncResult(on_result)
@@ -634,15 +634,15 @@
 
     # The answer was returned, and passed to the callback
     assert async_answer == 42
     on_result.assert_called_once_with(42)
 
 
 def test_async_result_cancelled_sync(event_loop):
-    """A deprecated on_result handler won't be fired on a cancelled future"""
+    """A deprecated on_result handler won't be fired on a cancelled future."""
     on_result = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         result = ExampleAsyncResult(on_result)
@@ -657,15 +657,15 @@
         event_loop.run_until_complete(result.future)
 
     # The callback wasn't called
     on_result.assert_not_called()
 
 
 def test_async_exception_sync(event_loop):
-    """A deprecated on_result handler can raise an exception"""
+    """A deprecated on_result handler can raise an exception."""
     on_result = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         result = ExampleAsyncResult(on_result)
@@ -679,15 +679,15 @@
     # The answer was returned, and passed to the callback
     on_result.assert_called_once()
     assert on_result.call_args[0] == (None,)
     assert isinstance(on_result.call_args[1]["exception"], ValueError)
 
 
 def test_async_exception_cancelled_sync(event_loop):
-    """An async result can raise an exception even if the future is cancelled"""
+    """An async result can raise an exception even if the future is cancelled."""
     on_result = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         result = ExampleAsyncResult(on_result)
```

### Comparing `toga-core-0.4.2/tests/test_images.py` & `toga_core-0.4.3/tests/test_images.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from pathlib import Path
 
 import PIL.Image
 import pytest
 
 import toga
+from toga_dummy.plugins.image_formats import (
+    CustomImage,
+    CustomImageSubclass,
+    DisabledImageConverter,
+)
 from toga_dummy.utils import assert_action_performed_with
 
 RELATIVE_FILE_PATH = Path("resources/sample.png")
 ABSOLUTE_FILE_PATH = Path(__file__).parent / "resources/sample.png"
 
 
 @pytest.mark.filterwarnings("ignore::DeprecationWarning")
@@ -29,15 +34,15 @@
         # Relative string
         ((f"{RELATIVE_FILE_PATH}",), {}),
         ((), {"src": f"{RELATIVE_FILE_PATH}"}),
         ((), {"path": f"{RELATIVE_FILE_PATH}"}),
     ],
 )
 def test_create_from_file(app, args, kwargs):
-    """An image can be constructed from a file"""
+    """An image can be constructed from a file."""
     image = toga.Image(*args, **kwargs)
 
     # Image is bound
     assert image._impl is not None
     # impl/interface round trips
     assert image._impl.interface == image
 
@@ -71,15 +76,15 @@
         # Relative string
         ((f"{MISSING_RELATIVE_PATH}",), {}),
         ((), {"src": f"{MISSING_RELATIVE_PATH}"}),
         ((), {"path": f"{MISSING_RELATIVE_PATH}"}),
     ],
 )
 def test_create_with_nonexistent_file(app, args, kwargs):
-    """If a file image source doesn't exist, an error is raised"""
+    """If a file image source doesn't exist, an error is raised."""
     with pytest.raises(FileNotFoundError):
         toga.Image(*args, **kwargs)
 
 
 BYTES = ABSOLUTE_FILE_PATH.read_bytes()
 
 
@@ -92,88 +97,88 @@
         ((), {"data": BYTES}),
         # Other "lump of bytes" data types
         ((bytearray(BYTES),), {}),
         ((memoryview(BYTES),), {}),
     ],
 )
 def test_create_from_bytes(args, kwargs):
-    """An image can be constructed from data"""
+    """An image can be constructed from data."""
     image = toga.Image(*args, **kwargs)
 
     # Image is bound
     assert image._impl is not None
     # impl/interface round trips
     assert image._impl.interface == image
 
     # Image was constructed with data
     assert_action_performed_with(image, "load image data", data=BYTES)
 
 
 def test_create_from_raw():
-    """An image can be created from a raw data source"""
+    """An image can be created from a raw data source."""
     orig = toga.Image(BYTES)
 
     copy = toga.Image(orig._impl.native)
     # Image is bound
     assert copy._impl is not None
     # impl/interface round trips
     assert copy._impl.interface == copy
 
     # Image was constructed from raw data
     assert_action_performed_with(copy, "load image from raw")
 
 
 def test_no_source():
-    """If no source is provided, an error is raised"""
+    """If no source is provided, an error is raised."""
     with pytest.raises(
         TypeError,
         match=r"Image.__init__\(\) missing 1 required positional argument: 'src'",
     ):
         toga.Image()
 
 
 def test_empty_image():
-    """If the image source is provided as None, an error is raised"""
+    """If the image source is provided as None, an error is raised."""
     with pytest.raises(
         TypeError,
         match=r"Unsupported source type for Image",
     ):
         toga.Image(None)
 
 
 def test_empty_image_explicit():
-    """If src is explicitly provided as None, an error is raised"""
+    """If src is explicitly provided as None, an error is raised."""
     with pytest.raises(
         TypeError,
         match=r"Unsupported source type for Image",
     ):
         toga.Image(src=None)
 
 
 def test_invalid_input_format():
-    """Trying to create an image with an invalid input should raise an error"""
+    """Trying to create an image with an invalid input should raise an error."""
     with pytest.raises(
         TypeError,
         match=r"Unsupported source type for Image",
     ):
         toga.Image(42)
 
 
 def test_create_from_pil(app):
-    """An image can be created from a PIL image"""
+    """An image can be created from a PIL image."""
     with PIL.Image.open(ABSOLUTE_FILE_PATH) as pil_image:
         pil_image.load()
     toga_image = toga.Image(pil_image)
 
     assert isinstance(toga_image, toga.Image)
     assert toga_image.size == (144, 72)
 
 
 def test_create_from_toga_image(app):
-    """An image can be create from another Toga image"""
+    """An image can be created from another Toga image."""
     toga_image = toga.Image(ABSOLUTE_FILE_PATH)
     toga_image_2 = toga.Image(toga_image)
 
     assert isinstance(toga_image_2, toga.Image)
     assert toga_image_2.size == (144, 72)
 
 
@@ -193,24 +198,24 @@
         # Two keywords
         ((), {"data": BYTES, "path": ABSOLUTE_FILE_PATH}),
         # All three
         ((ABSOLUTE_FILE_PATH,), {"data": BYTES, "path": ABSOLUTE_FILE_PATH}),
     ],
 )
 def test_too_many_arguments(args, kwargs):
-    """If multiple arguments are supplied, an error is raised"""
+    """If multiple arguments are supplied, an error is raised."""
     with pytest.raises(
-        ValueError,
+        TypeError,
         match=r"Received multiple arguments to constructor.",
     ):
         toga.Image(*args, **kwargs)
 
 
 def test_dimensions(app):
-    """The dimensions of the image can be retrieved"""
+    """The dimensions of the image can be retrieved."""
     image = toga.Image(RELATIVE_FILE_PATH)
 
     assert image.size == (144, 72)
     assert image.width == 144
     assert image.height == 72
 
 
@@ -225,15 +230,15 @@
     # If we build a new image from the data, it has the same properties.
     from_data = toga.Image(image.data)
     assert from_data.width == image.width
     assert from_data.height == image.height
 
 
 def test_image_save(tmp_path):
-    """An image can be saved"""
+    """An image can be saved."""
     save_path = tmp_path / "save.png"
     image = toga.Image(BYTES)
     image.save(save_path)
 
     assert_action_performed_with(image, "save", path=save_path)
 
 
@@ -247,31 +252,55 @@
         (toga.Image, toga.Image),
         (toga.Image, ImageSubclass),
         (ImageSubclass, toga.Image),
         (ImageSubclass, ImageSubclass),
     ],
 )
 def test_as_format_toga(app, Class_1, Class_2):
-    """as_format can successfully return a "copy" Image, with support for subclassing"""
+    """as_format can successfully return a "copy" Image, with support for
+    subclassing."""
     image_1 = Class_1(ABSOLUTE_FILE_PATH)
     image_2 = image_1.as_format(Class_2)
 
     assert isinstance(image_2, Class_2)
     assert image_2.size == (144, 72)
 
 
 def test_as_format_pil(app):
-    """as_format can successfully return a PIL image"""
+    """as_format can successfully return a PIL image."""
     toga_image = toga.Image(ABSOLUTE_FILE_PATH)
     pil_image = toga_image.as_format(PIL.Image.Image)
     assert isinstance(pil_image, PIL.Image.Image)
     assert pil_image.size == (144, 72)
 
 
+@pytest.mark.parametrize("ImageClass", [CustomImage, CustomImageSubclass])
+def test_create_from_custom_class(app, ImageClass):
+    """toga.Image can be created from custom type."""
+    custom_image = ImageClass()
+    toga_image = toga.Image(custom_image)
+    assert isinstance(toga_image, toga.Image)
+    assert toga_image.size == (144, 72)
+
+
+@pytest.mark.parametrize("ImageClass", [CustomImage, CustomImageSubclass])
+def test_as_format_custom_class(app, ImageClass):
+    """as_format can successfully return a registered custom image type."""
+    toga_image = toga.Image(ABSOLUTE_FILE_PATH)
+    custom_image = toga_image.as_format(ImageClass)
+    assert isinstance(custom_image, ImageClass)
+    assert custom_image.size == (144, 72)
+
+
+def test_disabled_image_plugin(app):
+    """Disabled image plugin shouldn't be available."""
+    assert DisabledImageConverter not in toga.Image._converters()
+
+
 # None is same as supplying nothing; also test a random unrecognized class
 @pytest.mark.parametrize("arg", [None, toga.Button])
 def test_as_format_invalid_input(app, arg):
-    """An unsupported format raises an error"""
+    """An unsupported format raises an error."""
     toga_image = toga.Image(ABSOLUTE_FILE_PATH)
 
     with pytest.raises(TypeError, match=r"Unknown conversion format for Image:"):
         toga_image.as_format(arg)
```

### Comparing `toga-core-0.4.2/tests/test_keys.py` & `toga_core-0.4.3/tests/test_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from toga.keys import Key
 
 
 def test_is_printable():
-    "Key printability can be checked"
+    """Key printability can be checked."""
     assert not Key.is_printable(Key.SHIFT)
     assert Key.is_printable(Key.LESS_THAN)
     assert Key.is_printable(Key.GREATER_THAN)
     assert Key.is_printable(Key.NUMPAD_0)
 
 
 def test_modifiers():
-    "Keys can be added with modifiers"
+    """Keys can be added with modifiers."""
     # Mod + Key
     assert Key.MOD_1 + Key.A == "<mod 1>a"
 
     # Multiple modifiers can be used
     assert Key.MOD_1 + Key.SHIFT + Key.A == "<mod 1><shift>a"
 
     # Bare characters can be used
```

### Comparing `toga-core-0.4.2/tests/test_paths.py` & `toga_core-0.4.3/tests/test_paths.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import sys
 from pathlib import Path
 
 import toga
 
 
 def run_app(args, cwd):
-    "Run a Toga app as a subprocess with coverage enabled and the Toga Dummy backend"
+    """Run a Toga app as a subprocess with coverage enabled and the Toga Dummy
+    backend."""
     # We need to do a full copy of the environment, then add our extra bits;
     # if we don't the Windows interpreter won't inherit SYSTEMROOT
     env = os.environ.copy()
     env.update(
         {
             "COVERAGE_PROCESS_START": str(
                 Path(__file__).parent.parent / "pyproject.toml"
@@ -22,23 +23,23 @@
     )
     output = subprocess.check_output(
         [sys.executable] + args,
         cwd=cwd,
         env=env,
         text=True,
     )
-    # When called as a subprocess, coverage drops it's coverage report in CWD.
+    # When called as a subprocess, coverage drops its coverage report in CWD.
     # Move it to the project root for combination with the main test report.
     for file in cwd.glob(".coverage*"):
         os.rename(file, Path(__file__).parent.parent / file.name)
     return output
 
 
 def assert_paths(output, app_path, app_name):
-    "Assert the paths for the standalone app are consistent"
+    """Assert the paths for the standalone app are consistent."""
     results = output.splitlines()
     assert f"app.paths.app={app_path.resolve()}" in results
     assert (
         f"app.paths.config={(Path.home() / 'config' / f'org.testbed.{app_name}').resolve()}"
         in results
     )
     assert (
@@ -53,49 +54,51 @@
         f"app.paths.logs={(Path.home() / 'logs' / f'org.testbed.{app_name}').resolve()}"
         in results
     )
     assert f"app.paths.toga={Path(toga.__file__).parent.resolve()}" in results
 
 
 def test_as_interactive():
-    "At an interactive prompt, the app path is the current working directory"
+    """At an interactive prompt, the app path is the current working directory."""
     # Spawn the interactive-mode mocking entry point
     cwd = Path(__file__).parent / "testbed"
     output = run_app(["interactive.py"], cwd=cwd)
     assert_paths(output, app_path=cwd, app_name="interactive-app")
 
 
 def test_simple_as_file_in_module():
-    """When a simple app is started as `python app.py` inside a runnable module, the
-    app path is the folder holding app.py."""
+    """When a simple app is started as `python app.py` inside a runnable module, the app
+    path is the folder holding app.py."""
     # Spawn the simple testbed app using `app.py`
     cwd = Path(__file__).parent / "testbed/simple"
     output = run_app(["app.py"], cwd=cwd)
     assert_paths(output, app_path=Path(toga.__file__).parent, app_name="simple-app")
 
 
 def test_simple_as_module():
-    """When a simple apps is started as `python -m app` inside a runnable module,
-    the app path is the folder holding app.py."""
+    """When a simple apps is started as `python -m app` inside a runnable module, the
+    app path is the folder holding app.py."""
     # Spawn the simple testbed app using `-m app`
     cwd = Path(__file__).parent / "testbed/simple"
     output = run_app(["-m", "app"], cwd=cwd)
     assert_paths(output, app_path=Path(toga.__file__).parent, app_name="simple-app")
 
 
 def test_simple_as_deep_file():
-    "When a simple app is started as `python simple/app.py`, the app path is the folder holding app.py"
+    """When a simple app is started as `python simple/app.py`, the app path is the
+    folder holding app.py."""
     # Spawn the simple testbed app using `simple/app.py`
     cwd = Path(__file__).parent / "testbed"
     output = run_app(["simple/app.py"], cwd=cwd)
     assert_paths(output, app_path=Path(toga.__file__).parent, app_name="simple-app")
 
 
 def test_simple_as_deep_module():
-    "When a simple app is started as `python -m simple`, the app path is the folder holding app.py"
+    """When a simple app is started as `python -m simple`, the app path is the folder
+    holding app.py."""
     # Spawn the simple testbed app using `-m simple`
     cwd = Path(__file__).parent / "testbed"
     output = run_app(["-m", "simple"], cwd=cwd)
     assert_paths(output, app_path=Path(toga.__file__).parent, app_name="simple-app")
 
 
 def test_subclassed_as_file_in_module():
@@ -104,29 +107,31 @@
     # Spawn the simple testbed app using `app.py`
     cwd = Path(__file__).parent / "testbed/subclassed"
     output = run_app(["app.py"], cwd=cwd)
     assert_paths(output, app_path=cwd, app_name="subclassed-app")
 
 
 def test_subclassed_as_module():
-    """When a subclassed app is started as `python -m app` inside a runnable module,
-    the app path is the folder holding app.py."""
+    """When a subclassed app is started as `python -m app` inside a runnable module, the
+    app path is the folder holding app.py."""
     # Spawn the subclassed testbed app using `-m app`
     cwd = Path(__file__).parent / "testbed/subclassed"
     output = run_app(["-m", "app"], cwd=cwd)
     assert_paths(output, app_path=cwd, app_name="subclassed-app")
 
 
 def test_subclassed_as_deep_file():
-    "When a subclassed app is started as `python simple/app.py`, the app path is the folder holding app.py"
+    """When a subclassed app is started as `python simple/app.py`, the app path is the
+    folder holding app.py."""
     # Spawn the subclassed testbed app using `subclassed/app.py`
     cwd = Path(__file__).parent / "testbed"
     output = run_app(["subclassed/app.py"], cwd=cwd)
     assert_paths(output, app_path=cwd / "subclassed", app_name="subclassed-app")
 
 
 def test_subclassed_as_deep_module():
-    "When a subclassed app is started as `python -m simple`, the app path is the folder holding app.py"
+    """When a subclassed app is started as `python -m simple`, the app path is the
+    folder holding app.py."""
     # Spawn the subclassed testbed app using `-m subclassed`
     cwd = Path(__file__).parent / "testbed"
     output = run_app(["-m", "subclassed"], cwd=cwd)
     assert_paths(output, app_path=cwd / "subclassed", app_name="subclassed-app")
```

### Comparing `toga-core-0.4.2/tests/test_platform.py` & `toga_core-0.4.3/tests/test_platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,50 +62,50 @@
             "linux": "linux",
             "win32": "windows",
         }[sys.platform]
     )
 
 
 def test_get_current_platform_android_inferred(monkeypatch):
-    "Android platform can be inferred from existence of sys.getandroidapilevel"
+    """Android platform can be inferred from existence of sys.getandroidapilevel."""
     monkeypatch.setattr(sys, "platform", "linux")
     try:
         # since there isn't an existing attribute of this name, it can't be patched.
         sys.getandroidapilevel = Mock(return_value=42)
         assert get_current_platform() == "android"
     finally:
         del sys.getandroidapilevel
 
 
 def test_get_current_platform_android(monkeypatch):
-    "Android platform can be obtained directly from sys.platform"
+    """Android platform can be obtained directly from sys.platform."""
     monkeypatch.setattr(sys, "platform", "android")
     try:
         # since there isn't an existing attribute of this name, it can't be patched.
         sys.getandroidapilevel = Mock(return_value=42)
         assert get_current_platform() == "android"
     finally:
         del sys.getandroidapilevel
 
 
 def test_get_current_platform_iOS(monkeypatch):
-    "iOS platform can be obtained directly from sys.platform"
+    """IOS platform can be obtained directly from sys.platform."""
     monkeypatch.setattr(sys, "platform", "ios")
     assert get_current_platform() == "iOS"
 
 
 def test_get_current_platform_web(monkeypatch):
-    "Web platform can be obtained directly from sys.platform"
+    """Web platform can be obtained directly from sys.platform."""
     monkeypatch.setattr(sys, "platform", "emscripten")
     assert get_current_platform() == "web"
 
 
 @pytest.mark.parametrize("value", ["freebsd12", "freebsd13", "freebsd14"])
 def test_get_current_platform_freebsd(monkeypatch, value):
-    "FreeBSD platform can be obtained directly from sys.platform"
+    """FreeBSD platform can be obtained directly from sys.platform."""
     monkeypatch.setattr(sys, "platform", value)
     assert get_current_platform() == "freeBSD"
 
 
 def _get_platform_factory():
     get_platform_factory.cache_clear()
     factory = get_platform_factory()
```

### Comparing `toga-core-0.4.2/tests/test_validators.py` & `toga_core-0.4.3/tests/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 def test_length_between(value, kwargs, error):
     validator = validators.LengthBetween(**kwargs)
 
     assert validator(value) == error
 
 
 def test_invalid_range():
-    "Minimum value must be less than maximum value"
+    """Minimum value must be less than maximum value."""
     with pytest.raises(
         ValueError,
         match=r"Minimum length cannot be less than maximum length",
     ):
         validators.LengthBetween(min_length=10, max_length=5)
 
 
@@ -636,15 +636,15 @@
         (".1234", dict(), None),
         # Negative Float, no leading 0
         ("-.1234", dict(), None),
         # Exponential
         ("1.23e+4", dict(), None),
         # Negative Exponential
         ("-1.23e-4", dict(), None),
-        # Exponential (captialized)
+        # Exponential (capitalized)
         ("1.23E+4", dict(), None),
         # Negative (capitalized)
         ("-1.23E-4", dict(), None),
         # Allow empty strings
         ("", dict(), None),
         # Doesn't match
         (
```

### Comparing `toga-core-0.4.2/tests/test_window.py` & `toga_core-0.4.3/tests/window/test_window.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @pytest.fixture
 def window(app):
     return toga.Window()
 
 
 def test_window_created(app):
-    "A Window can be created with minimal arguments"
+    """A Window can be created with minimal arguments."""
     window = toga.Window()
 
     assert window.app == app
     assert window.content is None
 
     assert window._impl.interface == window
     assert_action_performed(window, "create Window")
@@ -35,15 +35,15 @@
     assert window.closable
     assert window.minimizable
     assert len(window.toolbar) == 0
     assert window.on_close._raw is None
 
 
 def test_window_created_explicit(app):
-    "Explicit arguments at construction are stored"
+    """Explicit arguments at construction are stored."""
     on_close_handler = Mock()
 
     window = toga.Window(
         id="my-window",
         title="My Window",
         position=(10, 20),
         size=(200, 300),
@@ -67,33 +67,33 @@
     assert not window.closable
     assert not window.minimizable
     assert len(window.toolbar) == 0
     assert window.on_close._raw == on_close_handler
 
 
 def test_window_created_without_app():
-    "A window cannot be created without an active app"
+    """A window cannot be created without an active app."""
     toga.App.app = None
     with pytest.raises(
         RuntimeError, match="Cannot create a Window before creating an App"
     ):
         toga.Window()
 
 
 def test_set_app(window, app):
-    """A window's app cannot be reassigned"""
+    """A window's app cannot be reassigned."""
     assert window.app == app
 
     app2 = toga.App("Test App 2", "org.beeware.toga.test-app-2")
     with pytest.raises(ValueError, match=r"Window is already associated with an App"):
         window.app = app2
 
 
 def test_set_app_with_content(window, app):
-    """If a window has content, the content is assigned to the app"""
+    """If a window has content, the content is assigned to the app."""
     assert window.app == app
 
     content = toga.Box()
     assert content.app is None
 
     window.content = content
     assert content.app == app
@@ -106,21 +106,21 @@
         ("", "Toga"),
         (None, "Toga"),
         (12345, "12345"),
         ("Contains\nnewline", "Contains"),
     ],
 )
 def test_title(window, value, expected):
-    """The title of the window can be changed"""
+    """The title of the window can be changed."""
     window.title = value
     assert window.title == expected
 
 
 def test_toolbar_implicit_add(window, app):
-    """Adding an item to to a toolbar implicitly adds it to the app."""
+    """Adding an item to a toolbar implicitly adds it to the app."""
     cmd1 = toga.Command(None, "Command 1")
     cmd2 = toga.Command(None, "Command 2")
 
     toolbar = window.toolbar
     assert list(toolbar) == []
     assert list(app.commands) == []
 
@@ -137,15 +137,15 @@
     # Adding a command to both places does not cause a duplicate
     app.commands.add(cmd1)
     assert list(toolbar) == [cmd1]
     assert list(app.commands) == [cmd1, cmd2]
 
 
 def test_change_content(window, app):
-    """The content of a window can be changed"""
+    """The content of a window can be changed."""
     assert window.content is None
     assert window.app == app
 
     # Set the content of the window
     content1 = toga.Box()
     window.content = content1
 
@@ -267,15 +267,15 @@
 
     window.full_screen = False
     assert not window.full_screen
     assert_action_performed_with(window, "set full screen", full_screen=False)
 
 
 def test_close_direct(window, app):
-    """A window can be closed directly"""
+    """A window can be closed directly."""
     on_close_handler = Mock(return_value=True)
     window.on_close = on_close_handler
 
     window.show()
     assert window.app == app
     assert window in app.windows
 
@@ -287,31 +287,31 @@
     assert window.app == app
     assert window not in app.windows
     assert_action_performed(window, "close")
     on_close_handler.assert_not_called()
 
 
 def test_close_no_handler(window, app):
-    """A window without a close handler can be closed"""
+    """A window without a close handler can be closed."""
     window.show()
     assert window.app == app
     assert window in app.windows
 
     # Close the window
     window._impl.simulate_close()
 
     # Window has been closed, and is no longer in the app's list of windows.
     assert window.closed
     assert window.app == app
     assert window not in app.windows
     assert_action_performed(window, "close")
 
 
-def test_close_sucessful_handler(window, app):
-    """A window with a successful close handler can be closed"""
+def test_close_successful_handler(window, app):
+    """A window with a successful close handler can be closed."""
     on_close_handler = Mock(return_value=True)
     window.on_close = on_close_handler
 
     window.show()
     assert window.app == app
     assert window in app.windows
 
@@ -323,15 +323,15 @@
     assert window.app == app
     assert window not in app.windows
     assert_action_performed(window, "close")
     on_close_handler.assert_called_once_with(window)
 
 
 def test_close_rejected_handler(window, app):
-    """A window can have a close handler that rejects closing"""
+    """A window can have a close handler that rejects closing."""
     on_close_handler = Mock(return_value=False)
     window.on_close = on_close_handler
 
     window.show()
     assert window.app == app
     assert window in app.windows
 
@@ -343,23 +343,134 @@
     assert window.app == app
     assert window in app.windows
     assert_action_not_performed(window, "close")
     on_close_handler.assert_called_once_with(window)
 
 
 def test_as_image(window):
-    """A window can be captured as an image"""
+    """A window can be captured as an image."""
     image = window.as_image()
     assert_action_performed(window, "get image data")
     # Don't need to check the raw data; just check it's the right size.
     assert image.size == (318, 346)
 
 
+def test_screen(window, app):
+    """A window can be moved to a different screen."""
+    # Cannot actually change window.screen, so just check
+    # the window positions as a substitute for moving the
+    # window between the screens.
+    # `window.screen` will return `Secondary Screen`
+    assert window.screen == app.screens[1]
+    assert window.position == (100, 100)
+    window.screen = app.screens[0]
+    assert window.position == (1466, 868)
+
+
+def test_screen_position(window, app):
+    """The window can be relocated using absolute and relative screen positions."""
+    # Details about screen layout are in toga_dummy=>app.py=>get_screens()
+    initial_position = window.position
+    window.position = (-100, -100)
+    assert window.position != initial_position
+    assert window.position == (-100, -100)
+    assert window.screen_position == (1266, 668)
+
+    # Move the window to a new position.
+    window.screen_position = (100, 100)
+    assert window.position == (-1266, -668)
+    assert window.screen_position == (100, 100)
+
+
+def test_widget_id_reusablity(window, app):
+    """Widget IDs can be reused after the associated widget's window is closed."""
+    # Common IDs
+    CONTENT_WIDGET_ID = "sample_window_content"
+    LABEL_WIDGET_ID = "sample_label"
+
+    label_widget = toga.Label(text="Sample Label", id=LABEL_WIDGET_ID)
+    second_window_content = toga.Box(id=CONTENT_WIDGET_ID, children=[label_widget])
+
+    third_window_content = toga.Box(children=[])
+
+    # A widget ID is only "used" when it is part of a visible layout;
+    # creating a widget and *not* putting it in a layout isn't an problem.
+    try:
+        new_label_widget = toga.Label(text="New Label", id=LABEL_WIDGET_ID)
+    except KeyError:
+        pytest.fail("Widget IDs that aren't part of a layout can be re-used.")
+
+    # Create 2 new visible windows
+    second_window = toga.Window()
+    second_window.show()
+
+    third_window = toga.Window()
+    third_window.show()
+
+    # Assign the window content widget to the second window
+    second_window.content = second_window_content
+    assert CONTENT_WIDGET_ID in app.widgets
+    assert LABEL_WIDGET_ID in app.widgets
+
+    # CONTENT_WIDGET_ID is in use, so a widget with that ID can't be assigned to a window.
+    with pytest.raises(
+        KeyError,
+        match=r"There is already a widget with the id 'sample_label'",
+    ):
+        third_window.content = new_label_widget
+    assert CONTENT_WIDGET_ID not in third_window.widgets
+    assert LABEL_WIDGET_ID not in third_window.widgets
+
+    # Adding content that has a child with a re-used ID should raise an error
+    with pytest.raises(
+        KeyError,
+        match=r"There is already a widget with the id 'sample_label'",
+    ):
+        third_window.content = toga.Box(children=[new_label_widget])
+    assert CONTENT_WIDGET_ID not in third_window.widgets
+    assert LABEL_WIDGET_ID not in third_window.widgets
+
+    # Adding a child with a re-used ID should raise an error.
+    third_window.content = third_window_content
+    with pytest.raises(
+        KeyError,
+        match=r"There is already a widget with the id 'sample_label'",
+    ):
+        third_window_content.add(new_label_widget)
+    assert CONTENT_WIDGET_ID not in third_window.widgets
+    assert LABEL_WIDGET_ID not in third_window.widgets
+
+    # Creating a new widget with same widget ID should not raise KeyError
+    try:
+        another_label_widget = toga.Label(text="Another Label", id=LABEL_WIDGET_ID)
+    except KeyError:
+        pytest.fail("Widget IDs that aren't part of a layout can be re-used.")
+
+    # If a widget using an ID is being *replaced*, the ID can be re-used.
+    try:
+        second_window.content = another_label_widget
+    except KeyError:
+        pytest.fail("Widget IDs that are replaced can be re-used.")
+
+    # Close Window 2
+    second_window.close()
+    assert CONTENT_WIDGET_ID not in app.widgets
+    assert LABEL_WIDGET_ID not in app.widgets
+
+    # Now that second_window has been closed, the duplicate ID can be used
+    try:
+        third_window_content.add(new_label_widget)
+    except KeyError:
+        pytest.fail("Widget IDs that are replaced can be re-used.")
+
+    third_window.close()
+
+
 def test_info_dialog(window, app):
-    """An info dialog can be shown"""
+    """An info dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.info_dialog("Title", "Body", on_result=on_result_handler)
@@ -386,15 +497,15 @@
         title="Title",
         message="Body",
     )
     on_result_handler.assert_called_once_with(window, None)
 
 
 def test_question_dialog(window, app):
-    """A question dialog can be shown"""
+    """A question dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.question_dialog("Title", "Body", on_result=on_result_handler)
@@ -421,15 +532,15 @@
         title="Title",
         message="Body",
     )
     on_result_handler.assert_called_once_with(window, True)
 
 
 def test_confirm_dialog(window, app):
-    """A confirm dialog can be shown"""
+    """A confirm dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.confirm_dialog("Title", "Body", on_result=on_result_handler)
@@ -456,15 +567,15 @@
         title="Title",
         message="Body",
     )
     on_result_handler.assert_called_once_with(window, True)
 
 
 def test_error_dialog(window, app):
-    """An error dialog can be shown"""
+    """An error dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.error_dialog("Title", "Body", on_result=on_result_handler)
@@ -491,15 +602,15 @@
         title="Title",
         message="Body",
     )
     on_result_handler.assert_called_once_with(window, None)
 
 
 def test_stack_trace_dialog(window, app):
-    """A stack trace dialog can be shown"""
+    """A stack trace dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.stack_trace_dialog(
@@ -533,15 +644,15 @@
         content="The error",
         retry=False,
     )
     on_result_handler.assert_called_once_with(window, None)
 
 
 def test_save_file_dialog(window, app):
-    """A save file dialog can be shown"""
+    """A save file dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.save_file_dialog(
@@ -576,15 +687,15 @@
         initial_directory=Path("/path/to"),
         file_types=None,
     )
     on_result_handler.assert_called_once_with(window, saved_file)
 
 
 def test_save_file_dialog_default_directory(window, app):
-    """If no path is provided, a save file dialog will use the default directory"""
+    """If no path is provided, a save file dialog will use the default directory."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.save_file_dialog(
@@ -620,15 +731,15 @@
         initial_directory=None,
         file_types=[".txt", ".pdf"],
     )
     on_result_handler.assert_called_once_with(window, saved_file)
 
 
 def test_open_file_dialog(window, app):
-    """A open file dialog can be shown"""
+    """A open file dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.open_file_dialog(
@@ -663,15 +774,15 @@
         file_types=None,
         multiple_select=False,
     )
     on_result_handler.assert_called_once_with(window, opened_file)
 
 
 def test_open_file_dialog_default_directory(window, app):
-    """If no path is provided, a open file dialog will use the default directory"""
+    """If no path is provided, a open file dialog will use the default directory."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.open_file_dialog(
@@ -710,15 +821,15 @@
         file_types=[".txt", ".pdf"],
         multiple_select=True,
     )
     on_result_handler.assert_called_once_with(window, opened_files)
 
 
 def test_select_folder_dialog(window, app):
-    """A select folder dialog can be shown"""
+    """A select folder dialog can be shown."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.select_folder_dialog(
@@ -752,15 +863,15 @@
         initial_directory=Path("/path/to/folder"),
         multiple_select=False,
     )
     on_result_handler.assert_called_once_with(window, opened_file)
 
 
 def test_select_folder_dialog_default_directory(window, app):
-    """If no path is provided, a select folder dialog will use the default directory"""
+    """If no path is provided, a select folder dialog will use the default directory."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Synchronous `on_result` handlers have been deprecated;",
     ):
         dialog = window.select_folder_dialog(
@@ -803,14 +914,17 @@
 def test_deprecated_names_open_file_dialog(window, app):
     """Deprecated names still work on open file dialogs."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"open_file_dialog\(multiselect\) has been renamed multiple_select",
+    ), pytest.warns(
+        DeprecationWarning,
+        match=r"Synchronous `on_result` handlers have been deprecated; use `await` on the asynchronous result",
     ):
         dialog = window.open_file_dialog(
             "Title",
             "/path/to/folder",
             multiselect=True,
             on_result=on_result_handler,
         )
@@ -837,14 +951,17 @@
 def test_deprecated_names_select_folder_dialog(window, app):
     """Deprecated names still work on open file dialogs."""
     on_result_handler = Mock()
 
     with pytest.warns(
         DeprecationWarning,
         match=r"select_folder_dialog\(multiselect\) has been renamed multiple_select",
+    ), pytest.warns(
+        DeprecationWarning,
+        match=r"Synchronous `on_result` handlers have been deprecated; use `await` on the asynchronous result",
     ):
         dialog = window.select_folder_dialog(
             "Title",
             "/path/to/folder",
             multiselect=True,
             on_result=on_result_handler,
         )
@@ -864,30 +981,30 @@
         initial_directory=Path("/path/to/folder"),
         multiple_select=True,
     )
     on_result_handler.assert_called_once_with(window, opened_files)
 
 
 def test_deprecated_names_resizeable():
-    """Deprecated spelling of resizable still works"""
+    """Deprecated spelling of resizable still works."""
     with pytest.warns(
         DeprecationWarning,
         match=r"Window.resizeable has been renamed Window.resizable",
     ):
         window = toga.Window(title="Deprecated", resizeable=True)
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Window.resizeable has been renamed Window.resizable",
     ):
         assert window.resizeable
 
 
 def test_deprecated_names_closeable():
-    """Deprecated spelling of closable still works"""
+    """Deprecated spelling of closable still works."""
     with pytest.warns(
         DeprecationWarning,
         match=r"Window.closeable has been renamed Window.closable",
     ):
         window = toga.Window(title="Deprecated", closeable=True)
 
     with pytest.warns(
```

### Comparing `toga-core-0.4.2/tests/testbed/interactive.py` & `toga_core-0.4.3/tests/testbed/interactive.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/testbed/subclassed/app.py` & `toga_core-0.4.3/tests/testbed/subclassed/app.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/widgets/canvas/conftest.py` & `toga_core-0.4.3/tests/widgets/canvas/conftest.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/widgets/canvas/test_canvas.py` & `toga_core-0.4.3/tests/widgets/canvas/test_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from toga.widgets.canvas import ClosedPathContext, Context, FillContext, StrokeContext
 from toga_dummy.utils import assert_action_not_performed, assert_action_performed
 
 REBECCA_PURPLE_COLOR = rgb(102, 51, 153)
 
 
 def test_widget_created():
-    "An empty canvas can be created"
+    """An empty canvas can be created."""
     widget = toga.Canvas()
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create Canvas")
 
     assert widget.on_resize._raw is None
     assert widget.on_press._raw is None
     assert widget.on_activate._raw is None
@@ -36,15 +36,15 @@
     on_activate_handler,
     on_release_handler,
     on_drag_handler,
     on_alt_press_handler,
     on_alt_release_handler,
     on_alt_drag_handler,
 ):
-    "A Canvas can be created with initial values"
+    """A Canvas can be created with initial values."""
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create Canvas")
 
     assert widget.on_resize._raw == on_resize_handler
     assert widget.on_press._raw == on_press_handler
     assert widget.on_activate._raw == on_activate_handler
     assert widget.on_release._raw == on_release_handler
@@ -54,15 +54,15 @@
     assert widget.on_alt_drag._raw == on_alt_drag_handler
 
     # Canvas has a root context
     assert isinstance(widget.context, Context)
 
 
 def test_disable_no_op(widget):
-    """Canvas doesn't have a disabled state"""
+    """Canvas doesn't have a disabled state."""
     # Enabled by default
     assert widget.enabled
 
     # Try to disable the widget
     widget.enabled = False
 
     # Still enabled.
@@ -73,61 +73,61 @@
     """Focus is a no-op."""
 
     widget.focus()
     assert_action_not_performed(widget, "focus")
 
 
 def test_redraw(widget):
-    """The canvas can be redrawn"""
+    """The canvas can be redrawn."""
     widget.redraw()
 
     assert_action_performed(widget, "redraw")
 
     # An empty canvas has 2 draw operations - pushing and popping the root context.
     assert widget._impl.draw_instructions == [
         ("push context", {}),
         ("pop context", {}),
     ]
 
 
 def test_subcontext(widget):
-    "A canvas can produce a subcontext"
+    """A canvas can produce a subcontext."""
     with widget.Context() as subcontext:
         # A fresh context has been created as a subcontext of the canvas.
         assert isinstance(subcontext, Context)
         assert subcontext != widget.context
 
 
 def test_closed_path(widget):
-    "A canvas can produce a ClosedPath subcontext"
+    """A canvas can produce a ClosedPath subcontext."""
     with widget.ClosedPath(x=10, y=20) as closed_path:
         # A fresh context has been created as a subcontext of the canvas.
         assert isinstance(closed_path, ClosedPathContext)
         assert closed_path != widget.context
         assert closed_path.x == 10
         assert closed_path.y == 20
 
 
 def test_fill(widget):
-    "A canvas can produce a Fill subcontext"
+    """A canvas can produce a Fill subcontext."""
     with widget.Fill(
         x=10, y=20, color="rebeccapurple", fill_rule=FillRule.EVENODD
     ) as fill:
         # A fresh context has been created as a subcontext of the canvas.
         assert isinstance(fill, FillContext)
         assert fill != widget.context
 
         assert fill.x == 10
         assert fill.y == 20
         assert fill.color == REBECCA_PURPLE_COLOR
         assert fill.fill_rule == FillRule.EVENODD
 
 
 def test_stroke(widget):
-    "A canvas can produce a Stroke subcontext"
+    """A canvas can produce a Stroke subcontext."""
     with widget.Stroke(
         x=10, y=20, color="rebeccapurple", line_width=5, line_dash=[2, 7]
     ) as stroke:
         # A fresh context has been created as a subcontext of the canvas.
         assert isinstance(stroke, StrokeContext)
         assert stroke != widget.context
 
@@ -145,27 +145,27 @@
         (Font(family=SYSTEM, size=SYSTEM_DEFAULT_FONT_SIZE), (132, 12)),
         (Font(family=SYSTEM, size=20), (220, 20)),
         (Font(family="Cutive", size=SYSTEM_DEFAULT_FONT_SIZE), (198, 18)),
         (Font(family="Cutive", size=20), (330, 30)),
     ],
 )
 def test_measure_text(widget, font, expected):
-    "Canvas can measure rendered text size"
+    """Canvas can measure rendered text size."""
     assert widget.measure_text("Hello world", font=font) == expected
 
 
 def test_as_image(widget):
-    """A rendered canvas can be retrieved as an image"""
+    """A rendered canvas can be retrieved as an image."""
     image = widget.as_image()
     assert image is not None
     assert_action_performed(widget, "get image data")
 
 
 def test_deprecated_drawing_operations(widget):
-    """Deprecated simple drawing operations raise a warning"""
+    """Deprecated simple drawing operations raise a warning."""
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Direct canvas operations have been deprecated; use context.begin_path()",
     ):
         widget.new_path()
 
@@ -378,25 +378,28 @@
         ),
         ("pop context", {}),
         ("pop context", {}),
     ]
 
 
 def test_deprecated_args(widget):
-    "Deprecated arguments to canvas functions raise warnings."
+    """Deprecated arguments to canvas functions raise warnings."""
     with pytest.warns(
         DeprecationWarning,
         match=r"The `tight` argument on Canvas.measure_text\(\) has been deprecated.",
     ):
         assert widget.measure_text(
             "Hello world", font=Font(family="Cutive", size=42), tight=True
         ) == (693, 63)
 
     with pytest.warns(
         DeprecationWarning,
+        match=r"Canvas.fill\(\) has been renamed Canvas.Fill\(\)",
+    ), pytest.warns(
+        DeprecationWarning,
         match=r"The `preserve` argument on fill\(\) has been deprecated.",
     ):
         with widget.fill("rebeccapurple", FillRule.EVENODD, preserve=False) as fill:
             fill.line_to(20, 30)
             fill.line_to(30, 20)
 
     widget._impl.draw_instructions == [
```

### Comparing `toga-core-0.4.2/tests/widgets/canvas/test_context_objects.py` & `toga_core-0.4.3/tests/widgets/canvas/test_context_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from toga_dummy.utils import assert_action_performed
 
 REBECCA_PURPLE_COLOR = rgb(102, 51, 153)
 
 
 def test_subcontext(widget):
-    "A context can produce a subcontext"
+    """A context can produce a subcontext."""
     with widget.context.Context() as subcontext:
         subcontext.line_to(30, 40)
     # A fresh context has been created as a subcontext of the canvas.
     assert isinstance(subcontext, Context)
     assert subcontext != widget.context
 
     assert_action_performed(widget, "redraw")
@@ -63,15 +63,15 @@
             "x=10, y=20",
             True,
             {"x": 10, "y": 20},
         ),
     ],
 )
 def test_closed_path(widget, kwargs, args_repr, has_move, properties):
-    "A context can produce a ClosedPath subcontext"
+    """A context can produce a ClosedPath subcontext."""
     with widget.context.ClosedPath(**kwargs) as closed_path:
         closed_path.line_to(30, 40)
 
     # A fresh context has been created as a subcontext of the canvas.
     assert isinstance(closed_path, ClosedPathContext)
     assert repr(closed_path) == f"ClosedPathContext({args_repr})"
 
@@ -175,15 +175,15 @@
                 "color": REBECCA_PURPLE_COLOR,
                 "fill_rule": FillRule.EVENODD,
             },
         ),
     ],
 )
 def test_fill(widget, kwargs, args_repr, has_move, properties):
-    "A context can produce a Fill subcontext"
+    """A context can produce a Fill subcontext."""
     with widget.context.Fill(**kwargs) as fill:
         fill.line_to(30, 40)
 
     # A fresh context has been created as a subcontext of the canvas.
     assert isinstance(fill, FillContext)
     assert repr(fill) == f"FillContext({args_repr})"
 
@@ -339,15 +339,15 @@
                 "line_width": 4.5,
                 "line_dash": [2, 7],
             },
         ),
     ],
 )
 def test_stroke(widget, kwargs, args_repr, has_move, properties):
-    "A context can produce a Stroke subcontext"
+    """A context can produce a Stroke subcontext."""
     with widget.context.Stroke(**kwargs) as stroke:
         stroke.line_to(30, 40)
 
     # A fresh context has been created as a subcontext of the canvas.
     assert isinstance(stroke, StrokeContext)
     assert repr(stroke) == f"StrokeContext({args_repr})"
 
@@ -376,15 +376,15 @@
         ),
         ("stroke", properties),
         ("pop context", {}),
     ]
 
 
 def test_deprecated_drawing_operations(widget):
-    """Deprecated simple drawing operations raise a warning"""
+    """Deprecated simple drawing operations raise a warning."""
 
     with pytest.warns(
         DeprecationWarning,
         match=r"Context.new_path\(\) has been renamed Context.begin_path\(\)",
     ):
         widget.context.new_path()
 
@@ -422,15 +422,15 @@
         ("close path", {}),
         ("pop context", {}),
         ("pop context", {}),
     ]
 
 
 def test_order_change(widget):
-    """The order of context objects can be changed"""
+    """The order of context objects can be changed."""
     # Initially nothing on the context.
     assert len(widget.context) == 0
 
     # Set up an inner context that has contained operations, including a subcontext
     widget.context.line_to(0, 0)
     with widget.Context() as context:
         context.line_to(10, 20)
@@ -621,15 +621,15 @@
         ("pop context", {}),
         ("line to", {"x": 99, "y": 99}),
         ("pop context", {}),
     ]
 
 
 def test_stacked_kwargs(widget):
-    "If contexts are stacked, kwargs for sub operations don't leak"
+    """If contexts are stacked, kwargs for sub operations don't leak."""
     widget.context.line_to(0, 0)
     with widget.Fill(color=rgb(255, 0, 0)) as fill1:
         fill1.line_to(10, 20)
         with fill1.Stroke(color=rgb(0, 255, 0)) as stroke1:
             stroke1.line_to(20, 30)
             with stroke1.Fill(color=rgb(0, 0, 255)) as fill2:
                 fill2.line_to(100, 200)
@@ -830,15 +830,15 @@
         # end fill 1
         ("line to", {"x": 99, "y": 99}),
         ("pop context", {}),
     ]
 
 
 def test_deprecated_args(widget):
-    "Deprecated arguments to canvas functions raise warnings."
+    """Deprecated arguments to canvas functions raise warnings."""
 
     # fill() raises a warning about preserve being deprecated, then raises an error when
     # it's used as a context manager.
     with pytest.raises(
         RuntimeError,
         match=r"Context\.fill\(\) has been renamed Context\.Fill\(\)\.",
     ):
```

### Comparing `toga-core-0.4.2/tests/widgets/canvas/test_draw_operations.py` & `toga_core-0.4.3/tests/widgets/canvas/test_draw_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from toga.fonts import SYSTEM, SYSTEM_DEFAULT_FONT_SIZE, Font
 from toga_dummy.utils import assert_action_performed
 
 REBECCA_PURPLE_COLOR = rgb(102, 51, 153)
 
 
 def test_begin_path(widget):
-    """A begin path operation can be added"""
+    """A begin path operation can be added."""
     draw_op = widget.context.begin_path()
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "BeginPath()"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
         ("begin path", {}),
     ]
 
 
 def test_close_path(widget):
-    """A close path operation can be added"""
+    """A close path operation can be added."""
     draw_op = widget.context.close_path()
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "ClosePath()"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -84,15 +84,15 @@
             {"color": REBECCAPURPLE, "fill_rule": FillRule.EVENODD},
             f"color={REBECCA_PURPLE_COLOR}, fill_rule=FillRule.EVENODD",
             {"color": REBECCA_PURPLE_COLOR, "fill_rule": FillRule.EVENODD},
         ),
     ],
 )
 def test_fill(widget, kwargs, args_repr, draw_kwargs):
-    """A primitive fill operation can be added"""
+    """A primitive fill operation can be added."""
     draw_op = widget.context.fill(**kwargs)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == f"Fill({args_repr})"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -154,15 +154,15 @@
             {"color": REBECCAPURPLE, "line_width": 4.5, "line_dash": [2, 7]},
             f"color={REBECCA_PURPLE_COLOR}, line_width=4.5, line_dash=[2, 7]",
             {"color": REBECCA_PURPLE_COLOR, "line_width": 4.5, "line_dash": [2, 7]},
         ),
     ],
 )
 def test_stroke(widget, kwargs, args_repr, draw_kwargs):
-    """A primitive stroke operation can be added"""
+    """A primitive stroke operation can be added."""
     draw_op = widget.context.stroke(**kwargs)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == f"Stroke({args_repr})"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -171,15 +171,15 @@
 
     # All the attributes can be retrieved.
     for attr, value in draw_kwargs.items():
         assert getattr(draw_op, attr) == value
 
 
 def test_move_to(widget):
-    """A move to operation can be added"""
+    """A move to operation can be added."""
     draw_op = widget.context.move_to(10, 20)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "MoveTo(x=10, y=20)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -188,15 +188,15 @@
 
     # All the attributes can be retrieved.
     assert draw_op.x == 10
     assert draw_op.y == 20
 
 
 def test_line_to(widget):
-    """A line to operation can be added"""
+    """A line to operation can be added."""
     draw_op = widget.context.line_to(10, 20)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "LineTo(x=10, y=20)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -205,15 +205,15 @@
 
     # All the attributes can be retrieved.
     assert draw_op.x == 10
     assert draw_op.y == 20
 
 
 def test_bezier_curve_to(widget):
-    """A Bézier curve to operation can be added"""
+    """A Bézier curve to operation can be added."""
     draw_op = widget.context.bezier_curve_to(10, 20, 30, 40, 50, 60)
 
     assert_action_performed(widget, "redraw")
     assert (
         repr(draw_op) == "BezierCurveTo(cp1x=10, cp1y=20, cp2x=30, cp2y=40, x=50, y=60)"
     )
 
@@ -231,15 +231,15 @@
     assert draw_op.cp2x == 30
     assert draw_op.cp2y == 40
     assert draw_op.x == 50
     assert draw_op.y == 60
 
 
 def test_quadratic_curve_to(widget):
-    """A Quadratic curve to operation can be added"""
+    """A Quadratic curve to operation can be added."""
     draw_op = widget.context.quadratic_curve_to(10, 20, 30, 40)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "QuadraticCurveTo(cpx=10, cpy=20, x=30, y=40)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -358,15 +358,15 @@
                 "endangle": pytest.approx(2.345),
                 "anticlockwise": True,
             },
         ),
     ],
 )
 def test_arc(widget, kwargs, args_repr, draw_kwargs):
-    """An arc operation can be added"""
+    """An arc operation can be added."""
     draw_op = widget.context.arc(**kwargs)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == f"Arc({args_repr})"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -515,15 +515,15 @@
                 "endangle": pytest.approx(3.456),
                 "anticlockwise": True,
             },
         ),
     ],
 )
 def test_ellipse(widget, kwargs, args_repr, draw_kwargs):
-    """An ellipse operation can be added"""
+    """An ellipse operation can be added."""
     draw_op = widget.context.ellipse(**kwargs)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == f"Ellipse({args_repr})"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -532,15 +532,15 @@
 
     # All the attributes can be retrieved.
     for attr, value in draw_kwargs.items():
         assert getattr(draw_op, attr) == value
 
 
 def test_rect(widget):
-    """A rect operation can be added"""
+    """A rect operation can be added."""
     draw_op = widget.context.rect(10, 20, 30, 40)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "Rect(x=10, y=20, width=30, height=40)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -595,15 +595,15 @@
                 "font": Font("Cutive", 42)._impl,
                 "baseline": Baseline.ALPHABETIC,
             },
         ),
     ],
 )
 def test_write_text(widget, kwargs, args_repr, draw_kwargs):
-    """A write text operation can be added"""
+    """A write text operation can be added."""
     draw_op = widget.context.write_text(**kwargs)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == f"WriteText({args_repr})"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -615,15 +615,15 @@
     assert draw_op.x == draw_kwargs["x"]
     assert draw_op.y == draw_kwargs["y"]
     assert draw_op.font == draw_kwargs["font"].interface
     assert draw_op.baseline == draw_kwargs["baseline"]
 
 
 def test_rotate(widget):
-    """A rotate operation can be added"""
+    """A rotate operation can be added."""
     draw_op = widget.context.rotate(1.234)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "Rotate(radians=1.234)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -631,15 +631,15 @@
     ]
 
     # All the attributes can be retrieved.
     assert draw_op.radians == pytest.approx(1.234)
 
 
 def test_scale(widget):
-    """A scale operation can be added"""
+    """A scale operation can be added."""
     draw_op = widget.context.scale(1.234, 2.345)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "Scale(sx=1.234, sy=2.345)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -648,15 +648,15 @@
 
     # All the attributes can be retrieved.
     assert draw_op.sx == pytest.approx(1.234)
     assert draw_op.sy == pytest.approx(2.345)
 
 
 def test_translate(widget):
-    """A translate operation can be added"""
+    """A translate operation can be added."""
     draw_op = widget.context.translate(10, 20)
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "Translate(tx=10, ty=20)"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
@@ -665,28 +665,28 @@
 
     # All the attributes can be retrieved.
     assert draw_op.tx == 10
     assert draw_op.ty == 20
 
 
 def test_reset_transform(widget):
-    """A reset transform operation can be added"""
+    """A reset transform operation can be added."""
     draw_op = widget.context.reset_transform()
 
     assert_action_performed(widget, "redraw")
     assert repr(draw_op) == "ResetTransform()"
 
     # The first and last instructions can be ignored as they are the
     assert widget._impl.draw_instructions[1:-1] == [
         ("reset transform", {}),
     ]
 
 
 def test_deprecated_usage(widget):
-    """Test that deprecated usage of operations raise errors"""
+    """Test that deprecated usage of operations raise errors."""
     with pytest.raises(
         RuntimeError,
         match=r"Context\.fill\(\) has been renamed Context\.Fill\(\)\.",
     ):
         with widget.context.fill() as fill:
             fill.line_to(10, 20)
```

### Comparing `toga-core-0.4.2/tests/widgets/canvas/test_helpers.py` & `toga_core-0.4.3/tests/widgets/canvas/test_helpers.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/widgets/test_activityindicator.py` & `toga_core-0.4.3/tests/widgets/test_activityindicator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 @pytest.fixture
 def activity_indicator():
     return toga.ActivityIndicator()
 
 
 def test_widget_created(activity_indicator):
-    "An activity indicator can be created."
+    """An activity indicator can be created."""
     # Round trip the impl/interface
     assert activity_indicator._impl.interface == activity_indicator
     assert_action_performed(activity_indicator, "create ActivityIndicator")
 
 
 def test_disable_no_op(activity_indicator):
-    "ActivityIndicator doesn't have a disabled state"
+    """ActivityIndicator doesn't have a disabled state."""
     # Enabled by default
     assert activity_indicator.enabled
 
     # Try to disable the widget
     activity_indicator.enabled = False
 
     # Still enabled.
     assert activity_indicator.enabled
 
 
 def test_start(activity_indicator):
-    "An activity indicator can be started"
+    """An activity indicator can be started."""
     # Not running initially
     assert not activity_indicator.is_running
 
     # Assert that start was not invoked on the impl as part of creation.
     assert_action_not_performed(activity_indicator, "start ActivityIndicator")
 
     # Start spinning
@@ -47,15 +47,15 @@
     assert activity_indicator.is_running
 
     # The impl was triggered.
     assert_action_performed(activity_indicator, "start ActivityIndicator")
 
 
 def test_already_started(activity_indicator):
-    "If an activity indicator is already started, starting again is a no-op"
+    """If an activity indicator is already started, starting again is a no-op."""
     # Start the activity indicator
     activity_indicator.start()
 
     # Reset the event log so we can detect new events
     EventLog.reset()
 
     # Start the indicator again
@@ -65,15 +65,15 @@
     assert activity_indicator.is_running
 
     # No action was performed.
     assert_action_not_performed(activity_indicator, "start ActivityIndicator")
 
 
 def test_stop(activity_indicator):
-    "An indicator can be stopped"
+    """An indicator can be stopped."""
     # Start spinning
     activity_indicator.start()
 
     # The indicator is running
     assert activity_indicator.is_running
 
     # Stop spinning
@@ -83,38 +83,38 @@
     assert not activity_indicator.is_running
 
     # The impl has been stopped
     assert_action_performed(activity_indicator, "stop ActivityIndicator")
 
 
 def test_already_stopped(activity_indicator):
-    "If an indicator is already stopped, stopping again is a no-op"
+    """If an indicator is already stopped, stopping again is a no-op."""
     # The indicator is not running initially
     assert not activity_indicator.is_running
 
     # Stop spinning
     activity_indicator.stop()
 
     # The indicator is still not running
     assert not activity_indicator.is_running
 
     # No stop action was performed.
     assert_action_not_performed(activity_indicator, "stop ActivityIndicator")
 
 
 def test_initially_running():
-    "An activity indicator can be created in a started state"
+    """An activity indicator can be created in a started state."""
     # Creating a new progress bar with running=True so it is already running
     activity_indicator = toga.ActivityIndicator(running=True)
 
     # Indicator is running
     assert activity_indicator.is_running
 
     # Assert that start was invoked on the impl as part of creation.
     assert_action_performed(activity_indicator, "start ActivityIndicator")
 
 
 def test_focus_noop(activity_indicator):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     activity_indicator.focus()
     assert_action_not_performed(activity_indicator, "focus")
```

### Comparing `toga-core-0.4.2/tests/widgets/test_base.py` & `toga_core-0.4.3/tests/widgets/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     assert widget.enabled
     assert widget.id == "widget_id"
     assert isinstance(widget.style, Pack)
     assert widget.style.padding == (666, 666, 666, 666)
 
 
 def test_add_child_to_leaf():
-    "A child cannot be added to a leaf node"
+    """A child cannot be added to a leaf node."""
     leaf = ExampleLeafWidget()
 
     # Widget doesn't have an app or window
     assert leaf.app is None
     assert leaf.window is None
 
     # Leaf nodes report an empty child list
@@ -78,15 +78,15 @@
 
     # Add the child.
     with pytest.raises(ValueError, match=r"ExampleLeafWidget cannot have children"):
         leaf.add(child)
 
 
 def test_add_child_without_app(widget):
-    "A child can be added to a node when there's no underlying app"
+    """A child can be added to a node when there's no underlying app."""
     # Widget doesn't have an app or window
     assert widget.app is None
     assert widget.window is None
 
     # Child list is empty
     assert widget.children == []
 
@@ -108,15 +108,15 @@
     assert_action_performed_with(widget, "add child", child=child._impl)
 
     # The widget's layout has been refreshed
     assert_action_performed_with(widget, "refresh")
 
 
 def test_add_child(app, widget):
-    "A child can be added to a node when there's an app & window"
+    """A child can be added to a node when there's an app & window."""
     # Set the app and window for the widget.
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     # Widget has an app and window
@@ -160,15 +160,15 @@
     # App's widget index has been updated
     assert len(app.widgets) == 2
     assert app.widgets["widget_id"] == widget
     assert app.widgets["child_id"] == child
 
 
 def test_add_multiple_children(app, widget):
-    "Multiple children can be added in one call"
+    """Multiple children can be added in one call."""
     # Set the app and window for the widget.
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     # Widget has an app and window
@@ -231,15 +231,15 @@
         "child1_id": child1,
         "child2_id": child2,
         "child3_id": child3,
     }
 
 
 def test_reparent_child(widget):
-    "A widget can be reparented"
+    """A widget can be reparented."""
     # Create a second parent widget, and add a child to it
     other = ExampleWidget(id="other")
     child = ExampleLeafWidget(id="child_id")
     other.add(child)
 
     assert other.children == [child]
     assert child.parent == other
@@ -261,15 +261,15 @@
     assert_action_performed_with(widget, "refresh")
 
     # The layout of the old parent has been refreshed
     assert_action_performed_with(other, "refresh")
 
 
 def test_reparent_child_to_self(widget):
-    "Reparenting a widget to the same parent is a no-op"
+    """Reparenting a widget to the same parent is a no-op."""
     # Add a child to the widget
     child = ExampleLeafWidget(id="child_id")
     widget.add(child)
 
     assert widget.children == [child]
     assert child.parent == widget
 
@@ -288,15 +288,15 @@
     assert_action_not_performed(widget, "add child")
 
     # The widget's layout has been refreshed
     assert_action_performed_with(widget, "refresh")
 
 
 def test_insert_child_into_leaf():
-    "A child cannot be inserted into a leaf node"
+    """A child cannot be inserted into a leaf node."""
     leaf = ExampleLeafWidget()
 
     # Widget doesn't have an app or window
     assert leaf.app is None
     assert leaf.window is None
 
     # Leaf nodes report an empty child list
@@ -307,15 +307,15 @@
 
     # insert the child.
     with pytest.raises(ValueError, match=r"ExampleLeafWidget cannot have children"):
         leaf.insert(0, child)
 
 
 def test_insert_child_without_app(widget):
-    "A child can be inserted into a node when there's no underlying app"
+    """A child can be inserted into a node when there's no underlying app."""
     # Widget doesn't have an app or window
     assert widget.app is None
     assert widget.window is None
 
     # Child list is empty
     assert widget.children == []
 
@@ -337,15 +337,15 @@
     assert_action_performed_with(widget, "insert child", child=child._impl)
 
     # The widget's layout has been refreshed
     assert_action_performed_with(widget, "refresh")
 
 
 def test_insert_child(app, widget):
-    "A child can be inserted into a node when there's an app & window"
+    """A child can be inserted into a node when there's an app & window."""
     # Set the app and window for the widget.
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     # Widget has an app and window
@@ -392,15 +392,15 @@
     assert dict(window.widgets) == {
         "widget_id": widget,
         "child_id": child,
     }
 
 
 def test_insert_position(app, widget):
-    "Insert can put a child into a specific position"
+    """Insert can put a child into a specific position."""
     # Set the app and window for the widget.
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     # Widget has an app and window
@@ -467,15 +467,15 @@
         "child1_id": child1,
         "child2_id": child2,
         "child3_id": child3,
     }
 
 
 def test_insert_bad_position(app, widget):
-    "If the position is invalid, an error is raised"
+    """If the position is invalid, an error is raised."""
     # Set the app and window for the widget.
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     # Widget has an app and window
@@ -525,15 +525,15 @@
     assert dict(window.widgets) == {
         "widget_id": widget,
         "child_id": child,
     }
 
 
 def test_insert_reparent_child(widget):
-    "A widget can be reparented by insertion"
+    """A widget can be reparented by insertion."""
     # Create a second parent widget, and add a child to it
     other = ExampleWidget(id="other")
     child = ExampleLeafWidget(id="child_id")
     other.add(child)
 
     assert other.children == [child]
     assert child.parent == other
@@ -555,15 +555,15 @@
     assert_action_performed_with(widget, "refresh")
 
     # The original parent's layout has been refreshed
     assert_action_performed_with(other, "refresh")
 
 
 def test_insert_reparent_child_to_self(widget):
-    "Reparenting a widget to the same parent by insertion is a no-op"
+    """Reparenting a widget to the same parent by insertion is a no-op."""
     # Add a child to the widget
     child = ExampleLeafWidget(id="child_id")
     widget.add(child)
 
     assert widget.children == [child]
     assert child.parent == widget
 
@@ -582,15 +582,15 @@
     assert_action_not_performed(widget, "insert child")
 
     # The widget's layout has been refreshed
     assert_action_performed_with(widget, "refresh")
 
 
 def test_remove_child_from_leaf():
-    "A child cannot be removed from a leaf node"
+    """A child cannot be removed from a leaf node."""
     leaf = ExampleLeafWidget()
 
     # Widget doesn't have an app or window
     assert leaf.app is None
     assert leaf.window is None
 
     # Leaf nodes report an empty child list
@@ -601,15 +601,15 @@
 
     # Remove the child.
     with pytest.raises(ValueError, match=r"ExampleLeafWidget cannot have children"):
         leaf.remove(child)
 
 
 def test_remove_child_without_app(widget):
-    "A child without an app or window can be removed from a widget"
+    """A child without an app or window can be removed from a widget."""
     # Add a child to the widget
     child = ExampleLeafWidget(id="child_id")
     widget.add(child)
 
     assert widget.children == [child]
     assert child.parent == widget
     assert child.app is None
@@ -630,15 +630,15 @@
     assert_action_performed_with(widget, "remove child", child=child._impl)
 
     # The widget's layout has been refreshed
     assert_action_performed_with(widget, "refresh")
 
 
 def test_remove_child(app, widget):
-    "A child associated with an app & window can be removed from a widget"
+    """A child associated with an app & window can be removed from a widget."""
     # Add a child to the widget
     child = ExampleLeafWidget(id="child_id")
     widget.add(child)
 
     window = toga.Window()
     window.content = widget
     # Clear the event log
@@ -676,15 +676,15 @@
     assert_action_performed_with(window.content, "refresh")
 
     # App's widget index does not contain the widget
     assert "child_id" not in app.widgets
 
 
 def test_remove_multiple_children(app, widget):
-    "Multiple children can be removed from a widget"
+    """Multiple children can be removed from a widget."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     window = toga.Window()
@@ -735,15 +735,15 @@
 
     # Windows's widget index does not contain the widget
     assert "child1_id" not in window.widgets
     assert "child3_id" not in window.widgets
 
 
 def test_clear_all_children(app, widget):
-    "All children can be simultaneously removed from a widget"
+    """All children can be simultaneously removed from a widget."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     window = toga.Window()
@@ -797,15 +797,15 @@
     # Window's widget index does not contain the widget
     assert "child1_id" not in window.widgets
     assert "child2_id" not in window.widgets
     assert "child3_id" not in window.widgets
 
 
 def test_clear_no_children(app, widget):
-    "No changes are made (no-op) if widget has no children"
+    """No changes are made (no-op) if widget has no children."""
     window = toga.Window()
     window.content = widget
     # Clear the event log
     EventLog.reset()
 
     assert widget.children == []
 
@@ -819,15 +819,15 @@
     assert_action_not_performed(widget, "refresh")
 
     # The window's content doesn't get a refresh notification
     assert_action_not_performed(window.content, "refresh")
 
 
 def test_clear_leaf(app):
-    "`clear` cannot be called on a leaf node"
+    """`clear` cannot be called on a leaf node."""
     leaf = ExampleLeafWidget()
     window = toga.Window()
     window.content = leaf
     # Clear the event log
     EventLog.reset()
 
     assert leaf.children == []
@@ -843,15 +843,15 @@
     assert_action_not_performed(leaf, "refresh")
 
     # The window's content doesn't get a refresh notification
     assert_action_not_performed(window.content, "refresh")
 
 
 def test_remove_from_non_parent(widget):
-    "Trying to remove a child from a widget other than it's parent is a no-op"
+    """Trying to remove a child from a widget other than it's parent is a no-op."""
     # Create a second parent widget, and add a child to it
     other = ExampleWidget(id="other")
     child = ExampleLeafWidget(id="child_id")
     other.add(child)
 
     assert widget.children == []
     assert other.children == [child]
@@ -869,15 +869,15 @@
     assert_action_not_performed(widget, "remove child")
 
     # The widget's layout has *not* been refreshed
     assert_action_not_performed(widget, "refresh")
 
 
 def test_set_app(app, widget):
-    "A widget can be assigned to an app"
+    """A widget can be assigned to an app."""
     assert len(app.widgets) == 0
 
     # Assign the widget to an app
     widget.app = app
 
     # The app has been assigned
     assert widget.app == app
@@ -895,15 +895,15 @@
 
     # The widget is now in the app index.
     assert len(app.widgets) == 1
     assert app.widgets["widget_id"] == widget
 
 
 def test_set_app_with_children(app, widget):
-    "If a widget has children, the children get the app assignment"
+    """If a widget has children, the children get the app assignment."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     assert len(app.widgets) == 0
@@ -931,32 +931,32 @@
     assert attribute_value(widget, "app") == app
     assert attribute_value(child1, "app") == app
     assert attribute_value(child2, "app") == app
     assert attribute_value(child3, "app") == app
 
 
 def test_set_same_app(app, widget):
-    "A widget can be re-assigned to the same app"
+    """A widget can be re-assigned to the same app."""
     assert len(app.widgets) == 0
 
     # Assign the widget to an app
     widget.app = app
 
     # Reset the event log so we know the new events
     EventLog.reset()
 
     # Assign the widget to the same app
     widget.app = app
 
-    # The impl has not had it's app property set as a result of the update
+    # The impl has not had its app property set as a result of the update
     assert_attribute_not_set(widget, "app")
 
 
 def test_reset_app(app, widget):
-    "A widget can be re-assigned to no app"
+    """A widget can be re-assigned to no app."""
     assert len(app.widgets) == 0
 
     # Assign the widget to an app
     widget.app = app
 
     # Reset the event log so we know the new events
     EventLog.reset()
@@ -966,20 +966,20 @@
 
     # The app has been assigned
     assert widget.app is None
 
     # The widget index has been updated
     assert len(app.widgets) == 0
 
-    # The impl has had it's app property set.
+    # The impl has had its app property set.
     assert attribute_value(widget, "app") is None
 
 
 def test_set_new_app(app, widget):
-    "A widget can be assigned to a different app"
+    """A widget can be assigned to a different app."""
     # Assign the widget to an app. It won't appear in the registry, as
     # it hasn't been assigned to a window
     widget.app = app
     assert len(app.widgets) == 0
 
     # Reset the event log so we know the new events
     EventLog.reset()
@@ -996,20 +996,20 @@
 
     # The widget still doesn't appear in a widget index.
     assert len(app.widgets) == 0
     assert "widget_id" not in app.widgets
     assert len(new_app.widgets) == 0
     assert "widget_id" not in new_app.widgets
 
-    # The impl has had it's app property set.
+    # The impl has had its app property set.
     assert attribute_value(widget, "app") == new_app
 
 
 def test_set_window(widget):
-    "A widget can be assigned to a window."
+    """A widget can be assigned to a window."""
     window = toga.Window()
     assert len(window.widgets) == 0
     assert widget.window is None
 
     # Assign the widget to a window
     widget.window = window
 
@@ -1018,15 +1018,15 @@
 
     # Window Widget registry has been updated
     assert len(window.widgets) == 1
     assert window.widgets["widget_id"] == widget
 
 
 def test_set_window_with_children(app, widget):
-    "A widget can be assigned to a window."
+    """A widget can be assigned to a window."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     window = toga.Window()
@@ -1052,15 +1052,15 @@
     assert window.widgets["widget_id"] == widget
     assert window.widgets["child1_id"] == child1
     assert window.widgets["child2_id"] == child2
     assert window.widgets["child3_id"] == child3
 
 
 def test_reset_window(widget):
-    "A widget can be assigned to a different window."
+    """A widget can be assigned to a different window."""
     window = toga.Window()
     assert len(window.widgets) == 0
     assert widget.window is None
 
     # Assign the widget to a window
     widget.window = window
     assert len(window.widgets) == 1
@@ -1077,15 +1077,15 @@
     # Window Widget registry has been updated
     assert len(window.widgets) == 0
     assert len(new_window.widgets) == 1
     assert new_window.widgets["widget_id"] == widget
 
 
 def test_unset_window(widget):
-    "A widget can be assigned to no window."
+    """A widget can be assigned to no window."""
     window = toga.Window()
     assert len(window.widgets) == 0
     assert widget.window is None
 
     # Assign the widget to a window
     widget.window = window
     assert len(window.widgets) == 1
@@ -1108,15 +1108,15 @@
         ("true", True),
         ("false", True),  # Evaluated as a string, this value is true.
         (0, False),
         (1234, True),
     ],
 )
 def test_enabled(widget, value, expected):
-    "The enabled status of the widget can be changed."
+    """The enabled status of the widget can be changed."""
     # Widget is initially enabled by default.
     assert widget.enabled
 
     # Set the enabled status
     widget.enabled = value
     assert widget.enabled == expected
 
@@ -1126,30 +1126,30 @@
 
     # Set the enabled status again
     widget.enabled = value
     assert widget.enabled == expected
 
 
 def test_refresh_root(widget):
-    "Refresh can be invoked on the root node"
+    """Refresh can be invoked on the root node."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     # Refresh the root node
     widget.refresh()
 
     # Root widget was refreshed
     assert_action_performed(widget, "refresh")
 
 
 def test_refresh_child(widget):
-    "Refresh can be invoked on child"
+    """Refresh can be invoked on child."""
     # Add children to the widget
     child1 = ExampleLeafWidget(id="child1_id")
     child2 = ExampleLeafWidget(id="child2_id")
     child3 = ExampleLeafWidget(id="child3_id")
     widget.add(child1, child2, child3)
 
     # Refresh a child
@@ -1159,21 +1159,21 @@
     assert_action_performed(child2, "refresh")
 
     # Root widget was refreshed
     assert_action_performed(widget, "refresh")
 
 
 def test_focus(widget):
-    "A widget can be given focus"
+    """A widget can be given focus."""
     widget.focus()
     assert_action_performed(widget, "focus")
 
 
 def test_tab_index(widget):
-    "The tab index of a widget can be set and retrieved"
+    """The tab index of a widget can be set and retrieved."""
     # The initial tab index is None
     assert widget.tab_index is None
 
     tab_index = 8
     widget.tab_index = tab_index
 
     assert widget.tab_index == 8
```

### Comparing `toga-core-0.4.2/tests/widgets/test_box.py` & `toga_core-0.4.3/tests/widgets/test_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     assert_action_not_performed,
     assert_action_performed,
     assert_action_performed_with,
 )
 
 
 def test_create_box():
-    "A Box can be created."
+    """A Box can be created."""
     box = toga.Box()
     # Round trip the impl/interface
     assert box._impl.interface == box
 
     assert_action_performed(box, "create Box")
     assert_action_not_performed(box, "add child")
 
 
 def test_create_box_with_children():
-    "A Box can be created with children."
+    """A Box can be created with children."""
     child1 = toga.Box()
     child2 = toga.Box()
     box = toga.Box(children=[child1, child2])
 
     # Round trip the impl/interface
     assert box._impl.interface == box
 
@@ -30,26 +30,26 @@
     assert_action_performed_with(box, "add child", child=child2._impl)
 
     # But the box will have children.
     assert box.children == [child1, child2]
 
 
 def test_disable_no_op():
-    "Box doesn't have a disabled state"
+    """Box doesn't have a disabled state."""
     box = toga.Box()
 
     # Enabled by default
     assert box.enabled
 
     # Try to disable the widget
     box.enabled = False
 
     # Still enabled.
     assert box.enabled
 
 
 def test_focus_noop():
-    "Focus is a no-op."
+    """Focus is a no-op."""
     box = toga.Box()
 
     box.focus()
     assert_action_not_performed(box, "focus")
```

### Comparing `toga-core-0.4.2/tests/widgets/test_button.py` & `toga_core-0.4.3/tests/widgets/test_button.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.4.2/tests/widgets/test_dateinput.py` & `toga_core-0.4.3/tests/widgets/test_dateinput.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     assert widget.value == date(2023, 5, 25)
     assert widget.min == date(1800, 1, 1)
     assert widget.max == date(8999, 12, 31)
     assert widget.on_change._raw is None
 
 
 def test_widget_created_with_values(on_change_handler):
-    """A DateInput can be created with initial values"""
+    """A DateInput can be created with initial values."""
     # Round trip the impl/interface
     widget = toga.DateInput(
         value=date(2015, 6, 15),
         min=date(2013, 5, 14),
         max=date(2017, 7, 16),
         on_change=on_change_handler,
     )
@@ -60,15 +60,15 @@
         (date(2023, 1, 11), date(2023, 1, 11)),
         (datetime(2023, 2, 11, 10, 42, 37), date(2023, 2, 11)),
         ("2023-03-11", date(2023, 3, 11)),
         (None, date(2023, 5, 25)),
     ],
 )
 def test_value(widget, value, expected, on_change_handler):
-    "The value of the datepicker can be set"
+    """The value of the datepicker can be set."""
     widget.value = value
 
     assert widget.value == expected
 
     on_change_handler.assert_called_once_with(widget)
 
 
@@ -78,15 +78,15 @@
     (time(10, 42, 37), TypeError, "Not a valid date value"),
     ("not a date", ValueError, "Invalid isoformat string: 'not a date'"),
 ]
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_VALUES)
 def test_invalid_value(widget, value, exc, message):
-    "Invalid date values raise an exception"
+    """Invalid date values raise an exception."""
     with pytest.raises(exc, match=message):
         widget.value = value
 
 
 @pytest.mark.parametrize(
     "value, clipped",
     [
@@ -100,15 +100,15 @@
         # Unlike `min` and `max`, `value` accepts and clips dates outside of the
         # supported range.
         (date(1700, 1, 1), date(2010, 1, 1)),
         (date(9999, 12, 31), date(2020, 1, 1)),
     ],
 )
 def test_value_clipping(widget, value, clipped, on_change_handler):
-    "It the value is inconsistent with min/max, it is clipped."
+    """It the value is inconsistent with min/max, it is clipped."""
     # Set min/max dates, and clear the on_change mock
     widget.min = date(2010, 1, 1)
     widget.max = date(2020, 1, 1)
     on_change_handler.reset_mock()
 
     # Set the new value
     widget.value = value
@@ -126,29 +126,29 @@
         (None, date(1800, 1, 1)),
         (date(2023, 1, 11), date(2023, 1, 11)),
         (datetime(2023, 2, 11, 10, 42, 37), date(2023, 2, 11)),
         ("2023-03-11", date(2023, 3, 11)),
     ],
 )
 def test_min(widget, value, expected):
-    "The min of the datepicker can be set"
+    """The min of the datepicker can be set."""
     widget.min = value
 
     assert widget.min == expected
 
 
 INVALID_LIMITS = INVALID_VALUES + [
     (date(1799, 12, 31), ValueError, "The lowest supported date is 1800-01-01"),
     (date(9000, 1, 1), ValueError, "The highest supported date is 8999-12-31"),
 ]
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_LIMITS)
 def test_invalid_min(widget, value, exc, message):
-    "Invalid min values raise an exception"
+    """Invalid min values raise an exception."""
     widget.max = date(2025, 6, 12)
 
     with pytest.raises(exc, match=message):
         widget.min = value
 
 
 @pytest.mark.parametrize(
@@ -160,15 +160,15 @@
         (date(2005, 7, 4), True, False),
         (date(2005, 12, 31), True, False),
         (date(2006, 1, 1), True, True),
         (date(2006, 7, 4), True, True),
     ],
 )
 def test_min_clip(widget, on_change_handler, min, clip_value, clip_max):
-    "If the current value or max is before a new min date, it is clipped"
+    """If the current value or max is before a new min date, it is clipped."""
     widget.value = date(2005, 6, 25)
     widget.max = date(2005, 12, 31)
     on_change_handler.reset_mock()
 
     widget.min = min
     assert widget.min == min
 
@@ -191,23 +191,23 @@
         (None, date(8999, 12, 31)),
         (date(2023, 1, 11), date(2023, 1, 11)),
         (datetime(2023, 2, 11, 10, 42, 37), date(2023, 2, 11)),
         ("2023-03-11", date(2023, 3, 11)),
     ],
 )
 def test_max(widget, value, expected):
-    "The max of the datepicker can be set"
+    """The max of the datepicker can be set."""
     widget.max = value
 
     assert widget.max == expected
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_LIMITS)
 def test_invalid_max(widget, value, exc, message):
-    "Invalid max values raise an exception"
+    """Invalid max values raise an exception."""
     widget.min = date(2015, 6, 12)
 
     with pytest.raises(exc, match=message):
         widget.max = value
 
 
 @pytest.mark.parametrize(
@@ -219,15 +219,15 @@
         (date(2005, 7, 4), True, False),
         (date(2005, 12, 30), True, False),
         (date(2005, 12, 31), False, False),
         (date(2006, 7, 4), False, False),
     ],
 )
 def test_max_clip(widget, on_change_handler, max, clip_value, clip_min):
-    "If the current value or min is after a new max date, it is clipped"
+    """If the current value or min is after a new max date, it is clipped."""
     widget.min = date(2005, 6, 25)
     widget.value = date(2005, 12, 31)
     on_change_handler.reset_mock()
 
     widget.max = max
     assert widget.max == max
 
@@ -246,16 +246,21 @@
 
 def test_deprecated_names():
     MIN = date(2012, 8, 3)
     MAX = date(2016, 11, 15)
 
     with pytest.warns(
         DeprecationWarning, match="DatePicker has been renamed DateInput"
+    ), pytest.warns(
+        DeprecationWarning, match="DatePicker.min_date has been renamed DateInput.min"
+    ), pytest.warns(
+        DeprecationWarning, match="DatePicker.max_date has been renamed DateInput.max"
     ):
         widget = toga.DatePicker(min_date=MIN, max_date=MAX)
+
     assert widget.min == MIN
     assert widget.max == MAX
     widget.min = widget.max = None
 
     with pytest.warns(
         DeprecationWarning, match="DatePicker.min_date has been renamed DateInput.min"
     ):
```

### Comparing `toga-core-0.4.2/tests/widgets/test_detailedlist.py` & `toga_core-0.4.3/tests/widgets/test_detailedlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         on_refresh=on_refresh_handler,
         on_primary_action=on_primary_action_handler,
         on_secondary_action=on_secondary_action_handler,
     )
 
 
 def test_detailedlist_created():
-    "An minimal DetailedList can be created"
+    """A minimal DetailedList can be created."""
     detailedlist = toga.DetailedList()
     assert detailedlist._impl.interface == detailedlist
     assert_action_performed(detailedlist, "create DetailedList")
 
     assert len(detailedlist.data) == 0
     assert detailedlist.accessors == ("title", "subtitle", "icon")
     assert detailedlist.missing_value == ""
@@ -87,15 +87,15 @@
 def test_create_with_values(
     source,
     on_select_handler,
     on_refresh_handler,
     on_primary_action_handler,
     on_secondary_action_handler,
 ):
-    "A DetailedList can be created with initial values"
+    """A DetailedList can be created with initial values."""
     detailedlist = toga.DetailedList(
         data=source,
         accessors=("key", "value", "icon"),
         missing_value="Boo!",
         on_select=on_select_handler,
         on_refresh=on_refresh_handler,
         primary_action="Primary",
@@ -118,27 +118,27 @@
 
     assert_action_performed_with(detailedlist, "refresh enabled", enabled=True)
     assert_action_performed_with(detailedlist, "primary action enabled", enabled=True)
     assert_action_performed_with(detailedlist, "secondary action enabled", enabled=True)
 
 
 def test_disable_no_op(detailedlist):
-    "DetailedList doesn't have a disabled state"
+    """DetailedList doesn't have a disabled state."""
     # Enabled by default
     assert detailedlist.enabled
 
     # Try to disable the widget
     detailedlist.enabled = False
 
     # Still enabled.
     assert detailedlist.enabled
 
 
 def test_focus_noop(detailedlist):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     detailedlist.focus()
     assert_action_not_performed(detailedlist, "focus")
 
 
 @pytest.mark.parametrize(
     "data, all_attributes, extra_attributes",
@@ -188,15 +188,15 @@
 def test_set_data(
     detailedlist,
     on_select_handler,
     data,
     all_attributes,
     extra_attributes,
 ):
-    "Data can be set from a variety of sources"
+    """Data can be set from a variety of sources."""
 
     # The selection hasn't changed yet.
     on_select_handler.assert_not_called()
 
     # Change the data
     detailedlist.data = data
 
@@ -227,15 +227,15 @@
     if extra_attributes:
         assert detailedlist.data[0].extra == "extra1"
         assert detailedlist.data[1].extra == "extra2"
         assert detailedlist.data[2].extra == "extra3"
 
 
 def test_selection(detailedlist, on_select_handler):
-    "The current selection can be retrieved"
+    """The current selection can be retrieved."""
     # Selection is initially empty
     assert detailedlist.selection is None
     on_select_handler.assert_not_called()
 
     # Select an item
     detailedlist._impl.simulate_selection(1)
 
@@ -243,15 +243,15 @@
     assert detailedlist.selection == detailedlist.data[1]
 
     # Selection handler was triggered
     on_select_handler.assert_called_once_with(detailedlist)
 
 
 def test_refresh(detailedlist, on_refresh_handler):
-    "Completion of a refresh event triggers the cleanup handler"
+    """Completion of a refresh event triggers the cleanup handler."""
     # Stimulate a refresh.
     detailedlist._impl.stimulate_refresh()
 
     # refresh handler was invoked
     on_refresh_handler.assert_called_once_with(detailedlist)
 
     # The post-refresh handler was invoked on the backend
@@ -260,15 +260,15 @@
         "after on refresh",
         widget=detailedlist,
         result=None,
     )
 
 
 def test_scroll_to_top(detailedlist):
-    "A DetailedList can be scrolled to the top"
+    """A DetailedList can be scrolled to the top."""
     detailedlist.scroll_to_top()
 
     assert_action_performed_with(detailedlist, "scroll to row", row=0)
 
 
 @pytest.mark.parametrize(
     "row, effective",
@@ -282,41 +282,41 @@
         (-1, 2),
         (-3, 0),
         # Greater negative index than available rows
         (-10, 0),
     ],
 )
 def test_scroll_to_row(detailedlist, row, effective):
-    "A DetailedList can be scrolled to a specific row"
+    """A DetailedList can be scrolled to a specific row."""
     detailedlist.scroll_to_row(row)
 
     assert_action_performed_with(detailedlist, "scroll to row", row=effective)
 
 
 def test_scroll_to_row_no_data(detailedlist):
-    "If there's no data, scrolling is a no-op"
+    """If there's no data, scrolling is a no-op."""
     detailedlist.data.clear()
 
     detailedlist.scroll_to_row(5)
 
     assert_action_not_performed(detailedlist, "scroll to row")
 
 
 def test_scroll_to_bottom(detailedlist):
-    "A DetailedList can be scrolled to the top"
+    """A DetailedList can be scrolled to the top."""
     detailedlist.scroll_to_bottom()
 
     assert_action_performed_with(detailedlist, "scroll to row", row=2)
 
 
 ######################################################################
 # 2023-07: Backwards compatibility
 ######################################################################
 def test_deprecated_names(on_primary_action_handler):
-    "Deprecated names still work"
+    """Deprecated names still work."""
 
     # Can't specify both on_delete and on_primary_action
     with pytest.raises(
         ValueError,
         match=r"Cannot specify both on_delete and on_primary_action",
     ):
         toga.DetailedList(on_delete=Mock(), on_primary_action=Mock())
```

### Comparing `toga-core-0.4.2/tests/widgets/test_divider.py` & `toga_core-0.4.3/tests/widgets/test_divider.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,54 +5,54 @@
     EventLog,
     assert_action_not_performed,
     assert_action_performed,
 )
 
 
 def test_divider_created():
-    "A divider can be created."
+    """A divider can be created."""
     divider = toga.Divider()
 
     # Round trip the impl/interface
     assert divider._impl.interface == divider
     assert_action_performed(divider, "create Divider")
 
     # Default direction is honored
     assert divider.direction == toga.Divider.HORIZONTAL
 
 
 @pytest.mark.parametrize("direction", [toga.Divider.HORIZONTAL, toga.Divider.VERTICAL])
 def test_divider_created_explicit(direction):
-    "A divider can be created."
+    """A divider can be created."""
     divider = toga.Divider(direction=direction)
 
     # Round trip the impl/interface
     assert divider._impl.interface == divider
     assert_action_performed(divider, "create Divider")
 
     # Default direction is honored
     assert divider.direction == direction
 
 
 def test_disable_no_op():
-    "Divider doesn't have a disabled state"
+    """Divider doesn't have a disabled state."""
     divider = toga.Divider()
 
     # Enabled by default
     assert divider.enabled
 
     # Try to disable the widget
     divider.enabled = False
 
     # Still enabled.
     assert divider.enabled
 
 
 def test_update_direction():
-    "The direction of the divider can be altered."
+    """The direction of the divider can be altered."""
     divider = toga.Divider(direction=toga.Divider.HORIZONTAL)
 
     # Initial direction is as expected
     assert divider.direction == toga.Divider.HORIZONTAL
 
     # Reset the event log.
     EventLog.reset()
@@ -62,12 +62,12 @@
 
     # The direction has been changed, and a refresh requested
     assert divider.direction == toga.Divider.VERTICAL
     assert_action_performed(divider, "refresh")
 
 
 def test_focus_noop():
-    "Focus is a no-op."
+    """Focus is a no-op."""
     divider = toga.Divider(direction=toga.Divider.HORIZONTAL)
 
     divider.focus()
     assert_action_not_performed(divider, "focus")
```

### Comparing `toga-core-0.4.2/tests/widgets/test_imageview.py` & `toga_core-0.4.3/tests/widgets/test_imageview.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,54 +17,54 @@
 
 @pytest.fixture
 def widget(app):
     return toga.ImageView()
 
 
 def test_create_empty(widget):
-    """A empty ImageView can be created"""
+    """An empty ImageView can be created."""
     # interface/impl round trips
     assert widget._impl.interface is widget
     assert_action_performed(widget, "create ImageView")
     assert_action_performed_with(widget, "set image", image=None)
     assert_action_performed(widget, "refresh")
 
     assert widget.image is None
 
 
 ABSOLUTE_FILE_PATH = Path(__file__).parent.parent / "resources/toga.png"
 
 
 def test_create_from_toga_image(app):
-    """An ImageView can be created from a Toga image"""
+    """An ImageView can be created from a Toga image."""
     image = toga.Image(ABSOLUTE_FILE_PATH)
     widget = toga.ImageView(image=image)
 
     # Interface/impl round trips
     assert widget._impl.interface is widget
     assert_action_performed(widget, "create ImageView")
     assert_action_performed_with(widget, "set image", image=image)
     assert_action_performed(widget, "refresh")
 
     # Image attribute is set
     assert widget.image == image
 
 
 def test_create_from_pil():
-    """An ImageView can be created from a PIL image"""
+    """An ImageView can be created from a PIL image."""
     with PIL.Image.open(ABSOLUTE_FILE_PATH) as pil_img:
         pil_img.load()
 
     imageview = toga.ImageView(pil_img)
     assert isinstance(imageview.image, toga.Image)
     assert imageview.image.size == (32, 32)
 
 
 def test_disable_no_op(widget):
-    """ImageView doesn't have a disabled state"""
+    """ImageView doesn't have a disabled state."""
 
     # Enabled by default
     assert widget.enabled
 
     # Try to disable the widget
     widget.enabled = False
 
@@ -75,47 +75,47 @@
 def test_focus_noop(widget):
     """Focus is a no-op."""
     widget.focus()
     assert_action_not_performed(widget, "focus")
 
 
 def test_set_image_str(widget):
-    """The image can be set with a string"""
+    """The image can be set with a string."""
     widget.image = ABSOLUTE_FILE_PATH
 
     assert_action_performed_with(widget, "set image", image=ANY)
     assert_action_performed(widget, "refresh")
 
     assert isinstance(widget.image, toga.Image)
     assert widget.image.path == ABSOLUTE_FILE_PATH
 
 
 def test_set_image_path(widget):
-    """The image can be set with a Path"""
+    """The image can be set with a Path."""
     widget.image = Path(ABSOLUTE_FILE_PATH)
 
     assert_action_performed_with(widget, "set image", image=ANY)
     assert_action_performed(widget, "refresh")
 
     assert isinstance(widget.image, toga.Image)
     assert widget.image.path == ABSOLUTE_FILE_PATH
 
 
 def test_set_image(widget):
-    "The image can be set with an Image instance"
+    """The image can be set with an Image instance."""
     image = toga.Image(Path(ABSOLUTE_FILE_PATH))
     widget.image = image
     assert_action_performed_with(widget, "set image", image=image)
     assert_action_performed(widget, "refresh")
 
     assert widget.image == image
 
 
 def test_set_image_none(app):
-    "The image can be cleared"
+    """The image can be cleared."""
     widget = toga.ImageView(image=ABSOLUTE_FILE_PATH)
     assert widget.image is not None
 
     widget.image = None
     assert_action_performed_with(widget, "set image", image=None)
     assert_action_performed(widget, "refresh")
```

### Comparing `toga-core-0.4.2/tests/widgets/test_label.py` & `toga_core-0.4.3/tests/widgets/test_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.fixture
 def label():
     return toga.Label("Test Label")
 
 
 def test_label_created(label):
-    "A label can be created."
+    """A label can be created."""
     # Round trip the impl/interface
     assert label._impl.interface == label
     assert_action_performed(label, "create Label")
 
 
 @pytest.mark.parametrize(
     "value, expected",
@@ -44,11 +44,11 @@
     assert attribute_value(label, "text") == expected
 
     # A rehint was performed
     assert_action_performed(label, "refresh")
 
 
 def test_focus_noop(label):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     label.focus()
     assert_action_not_performed(label, "focus")
```

### Comparing `toga-core-0.4.2/tests/widgets/test_multilinetextinput.py` & `toga_core-0.4.3/tests/widgets/test_multilinetextinput.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 @pytest.fixture
 def widget():
     return toga.MultilineTextInput()
 
 
 def test_widget_created(widget):
-    "A multiline text input"
+    """A multiline text input."""
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create MultilineTextInput")
 
     assert not widget.readonly
     assert widget.placeholder == ""
     assert widget.value == ""
     assert widget._on_change._raw is None
 
 
 def test_create_with_values():
-    "A multiline text input can be created with initial values"
+    """A multiline text input can be created with initial values."""
     on_change = Mock()
     widget = toga.MultilineTextInput(
         value="Some text",
         placeholder="A placeholder",
         readonly=True,
         on_change=on_change,
     )
@@ -83,15 +83,15 @@
         ("true", True),
         ("false", True),  # Evaluated as a string, this value is true.
         (0, False),
         (1234, True),
     ],
 )
 def test_readonly(widget, value, expected):
-    "The readonly status of the widget can be changed."
+    """The readonly status of the widget can be changed."""
     # Widget is initially not readonly by default.
     assert not widget.readonly
 
     # Set the readonly status
     widget.readonly = value
     assert widget.readonly == expected
```

### Comparing `toga-core-0.4.2/tests/widgets/test_numberinput.py` & `toga_core-0.4.3/tests/widgets/test_numberinput.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 @pytest.fixture
 def widget():
     return toga.NumberInput(step="0.01")
 
 
 def test_widget_created():
-    "A NumberInput can be created with minimal arguments"
+    """A NumberInput can be created with minimal arguments."""
     widget = toga.NumberInput()
 
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create NumberInput")
 
     assert not widget.readonly
     assert widget.value is None
     assert widget.step == Decimal("1")
     assert widget.min is None
     assert widget.max is None
     assert widget._on_change._raw is None
 
 
 def test_create_with_values():
-    "A NumberInput can be created with initial values"
+    """A NumberInput can be created with initial values."""
     on_change = Mock()
 
     widget = toga.NumberInput(
         value=Decimal("2.71828"),
         step=0.001,
         min=-42,
         max=420,
@@ -79,15 +79,15 @@
         # Empty string
         ("", None),
         # None
         (None, None),
     ],
 )
 def test_value(widget, value, expected):
-    "The value of the widget can be set"
+    """The value of the widget can be set."""
     # Clear the event log and validator mock
     EventLog.reset()
 
     # Define and set a new change callback
     on_change_handler = Mock()
     widget.on_change = on_change_handler
 
@@ -108,15 +108,15 @@
     "value",
     [
         object(),  # Not convertible
         "Not a number",  # Non-numerical string
     ],
 )
 def test_bad_value(widget, value):
-    "If a value can't be converted into a decimal, an error is raised"
+    """If a value can't be converted into a decimal, an error is raised."""
     with pytest.raises(ValueError, match=r"value must be a number or None"):
         widget.value = value
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
@@ -130,15 +130,15 @@
         ("123", Decimal("123")),
         ("1.23e+4", Decimal("1.23e+4")),
         # Decimal
         (Decimal("1.23"), Decimal("1.23")),
     ],
 )
 def test_step(widget, value, expected):
-    "The step of the widget can be set"
+    """The step of the widget can be set."""
     widget.step = value
     assert widget.step == expected
 
     # test backend has the right value
     assert attribute_value(widget, "step") == expected
 
 
@@ -155,25 +155,25 @@
         ("10", Decimal("12")),
     ],
 )
 
 
 @pytest.mark.parametrize(*QUANTIZE_PARAMS)
 def test_quantization(widget, step, expected):
-    "The value is quantized to the precision of the step"
+    """The value is quantized to the precision of the step."""
     widget.step = step
     widget.value = 12.3456
 
     # The value has been quantized to the step
     assert widget.value == expected
 
 
 @pytest.mark.parametrize(*QUANTIZE_PARAMS)
 def test_quantize_on_retrieval(widget, step, expected):
-    "A widget's value will be quantized on retrieval."
+    """A widget's value will be quantized on retrieval."""
     widget.step = step
 
     # Inject a raw attribute value.
     widget._impl._set_value("value", 12.3456)
     assert widget.value == expected
 
 
@@ -183,15 +183,15 @@
         object(),  # Not convertible
         "Not a number",  # Non-numerical string
         "",  # Empty string
         None,
     ],
 )
 def test_bad_step(widget, value):
-    "If a step can't be converted into a decimal, an error is raised"
+    """If a step can't be converted into a decimal, an error is raised."""
     with pytest.raises(ValueError, match=r"step must be a number"):
         widget.step = "not a number"
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
@@ -213,15 +213,15 @@
         # Empty string
         ("", None),
         # None
         (None, None),
     ],
 )
 def test_min(widget, value, expected):
-    "The min of the widget can be set"
+    """The min of the widget can be set."""
     widget.min = value
     assert widget.min == expected
 
     # test backend has the right value
     assert attribute_value(widget, "min") == expected
 
 
@@ -229,31 +229,31 @@
     "value",
     [
         object(),  # Not convertible
         "Not a number",  # Non-numerical string
     ],
 )
 def test_bad_min(widget, value):
-    "If a min can't be converted into a decimal, an error is raised"
+    """If a min can't be converted into a decimal, an error is raised."""
     with pytest.raises(ValueError, match=r"min must be a number or None"):
         widget.min = value
 
 
 def test_min_greater_than_max(widget):
-    "If the new min value exceeds the max value, the max value is clipped"
+    """If the new min value exceeds the max value, the max value is clipped."""
     widget.max = 10
     widget.min = 100
 
     assert widget.max == 100
     assert widget.min == 100
 
 
 @pytest.mark.parametrize(*QUANTIZE_PARAMS)
 def test_min_quantized(widget, step, expected):
-    "An existing min value is re-quantized after a change in step"
+    """An existing min value is re-quantized after a change in step."""
     # Set a small step so that the min value isn't quantized
     widget.step = 0.00000001
     widget.min = 12.3456
 
     # Set a new minimum
     widget.step = step
 
@@ -282,15 +282,15 @@
         # Empty string
         ("", None),
         # None
         (None, None),
     ],
 )
 def test_max(widget, value, expected):
-    "The max of the widget can be set"
+    """The max of the widget can be set."""
     widget.max = value
     assert widget.max == expected
 
     # test backend has the right value
     assert attribute_value(widget, "max") == expected
 
 
@@ -298,31 +298,31 @@
     "value",
     [
         object(),  # Not convertible
         "Not a number",  # Non-numerical string
     ],
 )
 def test_bad_max(widget, value):
-    "If a max can't be converted into a decimal, an error is raised"
+    """If a max can't be converted into a decimal, an error is raised."""
     with pytest.raises(ValueError, match=r"max must be a number or None"):
         widget.max = value
 
 
 def test_max_less_than_min(widget):
-    "If the new max value is less than the min value, the min value is clipped"
+    """If the new max value is less than the min value, the min value is clipped."""
     widget.min = 100
     widget.max = 10
 
     assert widget.max == 10
     assert widget.min == 10
 
 
 @pytest.mark.parametrize(*QUANTIZE_PARAMS)
 def test_max_quantized(widget, step, expected):
-    "An existing max value is re-quantized after a change in step"
+    """An existing max value is re-quantized after a change in step."""
     # Set a small step so that the max value isn't quantized
     widget.step = 0.00000001
     widget.max = 12.3456
 
     # Set a new maximum
     widget.step = step
 
@@ -339,15 +339,15 @@
         (10, 20, None, None),
         # Check min/max values of 0
         (0, 20, -15, Decimal(0)),
         (-10, 0, 25, Decimal(0)),
     ],
 )
 def test_clip_on_value_change(widget, min, max, provided, clipped):
-    "A widget's value will be clipped inside the min/max range."
+    """A widget's value will be clipped inside the min/max range."""
     widget.min = min
     widget.max = max
 
     widget.value = provided
     assert widget.value == clipped
 
 
@@ -363,15 +363,16 @@
         (-10, 0, 25, Decimal(0)),
         # Check a "raw" value of 0
         (10, 20, 0, Decimal(10)),
         (-20, -10, 0, Decimal(-10)),
     ],
 )
 def test_clip_on_retrieval(widget, min, max, provided, clipped):
-    "A widget's value will be clipped if the widget has a value outside the min/max range."
+    """A widget's value will be clipped if the widget has a value outside the min/max
+    range."""
     widget.min = min
     widget.max = max
 
     # Inject a raw attribute value.
     widget._impl._set_value("value", provided)
     assert widget.value == clipped
 
@@ -383,15 +384,15 @@
         (10, 5, Decimal(5)),
         (10, None, Decimal(10)),
         (None, None, None),
         (None, 5, None),
     ],
 )
 def test_clip_on_max_change(widget, value, new_max, clipped):
-    "A widget's value will be clipped if the max value changes"
+    """A widget's value will be clipped if the max value changes."""
     # Set an initial max, and a value that is less than it.
     widget.max = 20
     widget.value = value
 
     # Set a new max
     widget.max = new_max
     # Value might be clipped
@@ -405,15 +406,15 @@
         (20, 25, Decimal(25)),
         (20, None, Decimal(20)),
         (None, None, None),
         (None, 25, None),
     ],
 )
 def test_clip_on_min_change(widget, value, new_min, clipped):
-    "A widget's value will be clipped if the min value changes"
+    """A widget's value will be clipped if the min value changes."""
     # Set an initial max, and a value that is less than it.
     widget.min = 10
     widget.value = value
 
     # Set a new max
     widget.min = new_min
     # Value might be clipped
@@ -445,15 +446,15 @@
         # Valid values
         ("", ""),
         ("123", "123"),
         ("-123", "-123"),
         ("1.23", "1.23"),
         ("-1.23", "-1.23"),
         (".123", ".123"),
-        # Non alphanumeric
+        # Non-alphanumeric
         ("12a3b", "123"),
         ("12!3@", "123"),
         # - not at the start
         ("1-23", "123"),
         ("123-", "123"),
         ("1.2-3", "1.23"),
         # Multiple . characters
@@ -493,15 +494,15 @@
     ],
 )
 def test_clean_decimal(value, step, clean):
     assert _clean_decimal(value, Decimal(step) if step else step) == Decimal(clean)
 
 
 def test_deprecated_names():
-    """The deprecated min_value/max_value names still work"""
+    """The deprecated min_value/max_value names still work."""
     # Can't specify min and min_value
     with pytest.raises(
         ValueError,
         match=r"Cannot specify both min and min_value",
     ):
         toga.NumberInput(min=2, min_value=4)
```

### Comparing `toga-core-0.4.2/tests/widgets/test_optioncontainer.py` & `toga_core-0.4.3/tests/widgets/test_optioncontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             toga.OptionItem("Item 4", content4),
         ],
         on_select=on_select_handler,
     )
 
 
 def test_widget_create():
-    "An option container can be created with no arguments"
+    """An option container can be created with no arguments."""
     optioncontainer = toga.OptionContainer()
     assert_action_performed(optioncontainer, "create OptionContainer")
 
     assert len(optioncontainer.content) == 0
     assert optioncontainer.current_tab is None
     assert optioncontainer.on_select._raw is None
 
@@ -82,15 +82,15 @@
     content1,
     content2,
     content3,
     content4,
     on_select_handler,
     tab_icon,
 ):
-    "An option container can be created with arguments"
+    """An option container can be created with arguments."""
     assert optioncontainer._impl.interface == optioncontainer
     assert_action_performed(optioncontainer, "create OptionContainer")
 
     assert len(optioncontainer.content) == 4
     assert optioncontainer.current_tab.text == "Item 1"
     assert optioncontainer.current_tab.icon is None
     assert optioncontainer.current_tab.enabled
@@ -117,27 +117,28 @@
     "value",
     [
         ("label",),
         ("label", toga.Box(), None, True, "extra"),
     ],
 )
 def test_widget_create_invalid_content(value):
-    """If the content provided at construction isn't 2- or 3-tuples, an error is raised."""
+    """If the content provided at construction isn't 2- or 3-tuples, an error is
+    raised."""
     with pytest.raises(
         ValueError,
         match=(
             r"Content items must be an OptionItem instance, or tuples of \(title, widget\), "
             r"\(title, widget, icon\), or \(title, widget, icon, enabled\)"
         ),
     ):
         toga.OptionContainer(content=value)
 
 
 def test_item_create(content1):
-    """An OptionItem can be created"""
+    """An OptionItem can be created."""
     item = toga.OptionItem("label", content1)
 
     assert item.text == "label"
     assert item.content == content1
     assert item.index is None
     assert item.interface is None
 
@@ -155,27 +156,27 @@
     has_content,
     has_icon,
     enabled,
     message,
     content1,
     tab_icon,
 ):
-    """If item details are invalid, an exception is raised"""
+    """If item details are invalid, an exception is raised."""
 
     with pytest.raises(ValueError, match=message):
         toga.OptionItem(
             title,
             content1 if has_content else None,
             icon=tab_icon if has_icon else None,
             enabled=enabled,
         )
 
 
 def test_assign_to_app(app, optioncontainer, content1, content2, content3):
-    """If the widget is assigned to an app, the content is also assigned"""
+    """If the widget is assigned to an app, the content is also assigned."""
     # Option container is initially unassigned
     assert optioncontainer.app is None
 
     # Assign the option container to the app
     optioncontainer.app = app
 
     # option container is on the app
@@ -184,29 +185,30 @@
     # Content is also on the app
     assert content1.app == app
     assert content2.app == app
     assert content3.app == app
 
 
 def test_assign_to_app_no_content(app):
-    """If the widget is assigned to an app, and there is no content, there's no error"""
+    """If the widget is assigned to an app, and there is no content, there's no
+    error."""
     optioncontainer = toga.OptionContainer()
 
     # Option container is initially unassigned
     assert optioncontainer.app is None
 
     # Assign the Option container to the app
     optioncontainer.app = app
 
     # Option container is on the app
     assert optioncontainer.app == app
 
 
 def test_assign_to_window(window, optioncontainer, content1, content2, content3):
-    """If the widget is assigned to a window, the content is also assigned"""
+    """If the widget is assigned to a window, the content is also assigned."""
     # Option container is initially unassigned
     assert optioncontainer.window is None
 
     # Assign the Option container to the window
     optioncontainer.window = window
 
     # Option container is on the window
@@ -214,29 +216,30 @@
     # Content is also on the window
     assert content1.window == window
     assert content2.window == window
     assert content3.window == window
 
 
 def test_assign_to_window_no_content(window):
-    """If the widget is assigned to a window, and there is no content, there's no error"""
+    """If the widget is assigned to a window, and there is no content, there's no
+    error."""
     optioncontainer = toga.OptionContainer()
 
     # Option container is initially unassigned
     assert optioncontainer.window is None
 
     # Assign the Option container to the window
     optioncontainer.window = window
 
     # Option container is on the window
     assert optioncontainer.window == window
 
 
 def test_disable_no_op(optioncontainer):
-    """OptionContainer doesn't have a disabled state"""
+    """OptionContainer doesn't have a disabled state."""
     # Enabled by default
     assert optioncontainer.enabled
 
     # Try to disable the widget
     optioncontainer.enabled = False
 
     # Still enabled.
@@ -282,15 +285,15 @@
 
     # Set the enabled status again
     item.enabled = value
     assert item.enabled == expected
 
 
 def test_disable_current_item(optioncontainer):
-    """The currently selected item cannot be disabled"""
+    """The currently selected item cannot be disabled."""
     # Item 0 is selected by default
     item = optioncontainer.content[0]
     with pytest.raises(
         ValueError,
         match=r"The currently selected tab cannot be disabled.",
     ):
         item.enabled = False
@@ -338,15 +341,15 @@
     [
         (None, r"Item text cannot be None"),
         ("", r"Item text cannot be blank"),
         (MyTitle(""), r"Item text cannot be blank"),
     ],
 )
 def test_invalid_item_text(optioncontainer, value, error, bare_item):
-    """Invalid item titles are prevented"""
+    """Invalid item titles are prevented."""
     if bare_item:
         item = toga.OptionItem("title", toga.Box())
     else:
         item = optioncontainer.content[1]
 
     # Using invalid text raises an error
     with pytest.raises(ValueError, match=error):
@@ -434,39 +437,39 @@
     optioncontainer.content.append("New content", toga.Box(), icon="new-icon")
 
     # Icon is still none
     assert optioncontainer.content["New content"].icon is None
 
 
 def test_optionlist_repr(optioncontainer):
-    """OptionContainer content has a helpful repr"""
+    """OptionContainer content has a helpful repr."""
     assert (
         repr(optioncontainer.content)
         == "<OptionList 'Item 1', 'Item 2', 'Item 3', 'Item 4'>"
     )
 
 
 def test_optionlist_iter(optioncontainer):
-    """OptionContainer content can be iterated"""
+    """OptionContainer content can be iterated."""
     assert [item.text for item in optioncontainer.content] == [
         "Item 1",
         "Item 2",
         "Item 3",
         "Item 4",
     ]
 
 
 def test_optionlist_len(optioncontainer):
-    """OptionContainer content has length"""
+    """OptionContainer content has length."""
     assert len(optioncontainer.content) == 4
 
 
 @pytest.mark.parametrize("index", [1, "Item 2", None])
 def test_getitem(optioncontainer, content2, index):
-    """An item can be retrieved"""
+    """An item can be retrieved."""
     if index is None:
         index = optioncontainer.content[1]
 
     # get item
     item = optioncontainer.content[index]
     assert item.text == "Item 2"
     assert item.index == 1
@@ -498,27 +501,27 @@
 
     # Widget has been refreshed
     assert_action_performed(optioncontainer, "refresh")
 
 
 @pytest.mark.parametrize("index", [0, "Item 1", None])
 def test_delitem_current(optioncontainer, index):
-    """The current item can't be deleted"""
+    """The current item can't be deleted."""
     if index is None:
         index = optioncontainer.content[0]
 
     with pytest.raises(
         ValueError, match=r"The currently selected tab cannot be deleted."
     ):
         del optioncontainer.content[index]
 
 
 @pytest.mark.parametrize("index", [1, "Item 2", None])
 def test_item_remove(optioncontainer, index):
-    """An item can be removed with remove"""
+    """An item can be removed with remove."""
     if index is None:
         index = optioncontainer.content[1]
 
     # get a reference to items 1 and 3
     item1 = optioncontainer.content[0]
     item3 = optioncontainer.content[2]
 
@@ -537,26 +540,26 @@
 
     # Widget has been refreshed
     assert_action_performed(optioncontainer, "refresh")
 
 
 @pytest.mark.parametrize("index", [0, "Item 1", None])
 def test_item_remove_current(optioncontainer, index):
-    """The current item can't be removed"""
+    """The current item can't be removed."""
     if index is None:
         index = optioncontainer.content[0]
 
     with pytest.raises(
         ValueError, match=r"The currently selected tab cannot be deleted."
     ):
         optioncontainer.content.remove(index)
 
 
 def test_item_insert_item(optioncontainer):
-    """The text of an inserted item can be set"""
+    """The text of an inserted item can be set."""
     new_content = toga.Box()
     item = toga.OptionItem("New Tab", new_content)
 
     optioncontainer.content.insert(1, item)
 
     # Backend added an item and set enabled
     assert_action_performed_with(
@@ -597,29 +600,29 @@
             (toga.OptionItem("New Tab", toga.Box()),),
             {"enabled": False},
             r"Cannot specify enabled if using an OptionItem instance.",
         ),
     ],
 )
 def test_item_insert_item_invalid(optioncontainer, args, kwargs, message):
-    """If both an item and specific details are provided, an error is raised"""
+    """If both an item and specific details are provided, an error is raised."""
     with pytest.raises(ValueError, match=message):
         optioncontainer.content.insert(1, *args, **kwargs)
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
         ("New Title", "New Title"),
         (42, "42"),  # Evaluated as a string
         (MyTitle("Custom Title"), "Custom Title"),  # Evaluated as a string
     ],
 )
 def test_item_insert_text(optioncontainer, value, expected):
-    """The text of an inserted item can be set"""
+    """The text of an inserted item can be set."""
     new_content = toga.Box()
 
     optioncontainer.content.insert(1, value, new_content, enabled=True)
 
     # Backend added an item and set enabled
     assert_action_performed_with(
         optioncontainer,
@@ -642,23 +645,23 @@
     [
         (None, r"Item text cannot be None"),
         ("", r"Item text cannot be blank"),
         (MyTitle(""), r"Item text cannot be blank"),
     ],
 )
 def test_item_insert_invalid_text(optioncontainer, value, error):
-    """The item text must be valid"""
+    """The item text must be valid."""
     new_content = toga.Box()
     with pytest.raises(ValueError, match=error):
         optioncontainer.content.insert(1, value, new_content, enabled=True)
 
 
 @pytest.mark.parametrize("enabled", [True, False])
 def test_item_insert_enabled(optioncontainer, enabled):
-    """The enabled status of content can be set on insert"""
+    """The enabled status of content can be set on insert."""
     new_content = toga.Box()
 
     optioncontainer.content.insert(1, "New content", new_content, enabled=enabled)
 
     # Backend added an item and set enabled
     assert_action_performed_with(
         optioncontainer,
@@ -674,15 +677,15 @@
         value=enabled,
     )
     assert_action_performed_with(optioncontainer, "refresh")
 
 
 @pytest.mark.parametrize("enabled", [True, False])
 def test_item_append(optioncontainer, enabled):
-    """An item can be appended to the content list"""
+    """An item can be appended to the content list."""
     # append is implemented using insert;
     # the bulk of the functionality is tested there.
     new_content = toga.Box()
 
     optioncontainer.content.append("New content", new_content, enabled=enabled)
     assert_action_performed_with(
         optioncontainer, "add option", index=4, widget=new_content._impl
```

### Comparing `toga-core-0.4.2/tests/widgets/test_passwordinput.py` & `toga_core-0.4.3/tests/widgets/test_passwordinput.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest.mock import Mock
 
 import toga
 from toga_dummy.utils import assert_action_performed
 
 
 def test_widget_created():
-    "A text input can be created"
+    """A text input can be created."""
     widget = toga.PasswordInput()
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create PasswordInput")
 
     assert not widget.readonly
     assert widget.placeholder == ""
     assert widget.value == ""
@@ -17,15 +17,15 @@
     assert widget._on_confirm._raw is None
     assert widget._on_gain_focus._raw is None
     assert widget._on_lose_focus._raw is None
     assert widget.validators == []
 
 
 def test_create_with_values():
-    "A multiline text input can be created with initial values"
+    """A multiline text input can be created with initial values."""
     on_change = Mock()
     on_confirm = Mock()
     on_gain_focus = Mock()
     on_lose_focus = Mock()
     validator1 = Mock(return_value=None)
     validator2 = Mock(return_value=None)
```

### Comparing `toga-core-0.4.2/tests/widgets/test_progressbar.py` & `toga_core-0.4.3/tests/widgets/test_progressbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @pytest.fixture
 def progressbar():
     return toga.ProgressBar()
 
 
 def test_progressbar_created(progressbar):
-    "A progressbar can be created."
+    """A progressbar can be created."""
     # Round trip the impl/interface
     assert progressbar._impl.interface == progressbar
     assert_action_performed(progressbar, "create ProgressBar")
 
     # Assert the default state of the progress bar.
     assert progressbar.max == pytest.approx(1.0)
     assert progressbar.value == pytest.approx(0.0)
@@ -37,30 +37,30 @@
         (15, 10.0),  # Integer, above max
         (-1, 0.0),  # Integer, below min
         (12.0, 10.0),  # Float, above max
         (-42.0, 0.0),  # Float, below min
     ],
 )
 def test_set_value_determinate(progressbar, value, actual):
-    "The value of a determinite progressbar can be set"
+    """The value of a determinate progressbar can be set."""
     # Set the max value
     progressbar.max = 10
 
     # Confirm this makes the progress bar determinate
     assert progressbar.is_determinate
 
     # Set the value of the
     progressbar.value = value
 
     # Value is clipped and converted to float
     assert progressbar.value == pytest.approx(actual)
 
 
 def test_set_value_indeterminate(progressbar):
-    "Setting the value of an indeterminate progressbar is a no-op"
+    """Setting the value of an indeterminate progressbar is a no-op."""
 
     # Make the progressbar indeterminate
     progressbar.max = None
 
     # Confirm this makes the progress bar indeterminate
     assert not progressbar.is_determinate
 
@@ -80,15 +80,15 @@
         (None, None, False),  # Non-determinate
         (42, 42.0, True),  # Integer
         (12.345, 12.345, True),  # Float
         ("37.42", 37.42, True),  # Float, but specified as a string.
     ],
 )
 def test_set_max(progressbar, value, actual, determinate):
-    "The max value can be set."
+    """The max value can be set."""
     progressbar.max = value
 
     # The maximum value has been applied, and has altered the determinate state.
     assert progressbar.max == pytest.approx(actual)
     assert progressbar.is_determinate == determinate
 
 
@@ -128,21 +128,21 @@
             0.0,
             ValueError,
             r"max value must be None, or a numerical value > 0",
         ),  # Non-positive float
     ],
 )
 def test_invalid_max(progressbar, value, error, msg):
-    "A max value that isn't positive raises an error"
+    """A max value that isn't positive raises an error."""
     with pytest.raises(error, match=msg):
         progressbar.max = value
 
 
 def test_start(progressbar):
-    "An activity indicator can be started"
+    """An activity indicator can be started."""
     # Not running initially
     assert not progressbar.is_running
 
     # Assert that start was not invoked on the impl as part of creation.
     assert_action_not_performed(progressbar, "start ProgressBar")
 
     # Start running
@@ -152,15 +152,15 @@
     assert progressbar.is_running
 
     # The impl was triggered.
     assert_action_performed(progressbar, "start ProgressBar")
 
 
 def test_already_started(progressbar):
-    "If an activity indicator is already started, starting again is a no-op"
+    """If an activity indicator is already started, starting again is a no-op."""
     # Start the activity indicator
     progressbar.start()
 
     # Reset the event log so we can detect new events
     EventLog.reset()
 
     # Start the indicator again
@@ -170,15 +170,15 @@
     assert progressbar.is_running
 
     # No action was performed.
     assert_action_not_performed(progressbar, "start ProgressBar")
 
 
 def test_stop(progressbar):
-    "An indicator can be stopped"
+    """An indicator can be stopped."""
     # Start running
     progressbar.start()
 
     # The indicator is running
     assert progressbar.is_running
 
     # Stop running
@@ -188,42 +188,42 @@
     assert not progressbar.is_running
 
     # The impl has been stopped
     assert_action_performed(progressbar, "stop ProgressBar")
 
 
 def test_already_stopped(progressbar):
-    "If an indicator is already stopped, stopping again is a no-op"
+    """If an indicator is already stopped, stopping again is a no-op."""
     # The indicator is not running initially
     assert not progressbar.is_running
 
     # Stop running
     progressbar.stop()
 
     # The indicator is still not running
     assert not progressbar.is_running
 
     # No stop action was performed.
     assert_action_not_performed(progressbar, "stop ProgressBar")
 
 
 def test_initially_running():
-    "An activity indicator can be created in a started state"
+    """An activity indicator can be created in a started state."""
     # Creating a new progress bar with running=True so it is already running
     progressbar = toga.ProgressBar(running=True)
 
     # Indicator is running
     assert progressbar.is_running
 
     # Assert that start was invoked on the impl as part of creation.
     assert_action_performed(progressbar, "start ProgressBar")
 
 
 def test_determinate_switch(progressbar):
-    "A progressbar can switch between determinate and indeterminate"
+    """A progressbar can switch between determinate and indeterminate."""
     # Set initial max and value
     progressbar.max = 10
     progressbar.value = 5
 
     # State of progress bar is determinate
     assert progressbar.is_determinate
     assert progressbar.value == pytest.approx(5.0)
```

### Comparing `toga-core-0.4.2/tests/widgets/test_scrollcontainer.py` & `toga_core-0.4.3/tests/widgets/test_scrollcontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 
 @pytest.fixture
 def scroll_container(content, on_scroll_handler):
     return toga.ScrollContainer(content=content, on_scroll=on_scroll_handler)
 
 
 def test_widget_created():
-    "A scroll container can be created with no arguments"
+    """A scroll container can be created with no arguments."""
     scroll_container = toga.ScrollContainer()
     assert scroll_container._impl.interface == scroll_container
     assert_action_performed(scroll_container, "create ScrollContainer")
 
     assert scroll_container.content is None
     assert scroll_container.vertical
     assert scroll_container.horizontal
     assert scroll_container.on_scroll._raw is None
 
 
 def test_widget_created_with_values(content, on_scroll_handler):
-    "A scroll container can be created with arguments"
+    """A scroll container can be created with arguments."""
     scroll_container = toga.ScrollContainer(
         content=content,
         on_scroll=on_scroll_handler,
         vertical=False,
         horizontal=False,
     )
     assert scroll_container._impl.interface == scroll_container
@@ -70,90 +70,92 @@
     assert_action_performed(content, "refresh")
 
     # The scroll handler hasn't been invoked
     on_scroll_handler.assert_not_called()
 
 
 def test_assign_to_app(app, scroll_container, content):
-    """If the widget is assigned to an app, the content is also assigned"""
+    """If the widget is assigned to an app, the content is also assigned."""
     # Scroll container is initially unassigned
     assert scroll_container.app is None
 
     # Assign the scroll container to the app
     scroll_container.app = app
 
     # Scroll container is on the app
     assert scroll_container.app == app
     # Content is also on the app
     assert content.app == app
 
 
 def test_assign_to_app_no_content(app):
-    """If the widget is assigned to an app, and there is no content, there's no error"""
+    """If the widget is assigned to an app, and there is no content, there's no
+    error."""
     scroll_container = toga.ScrollContainer()
 
     # Scroll container is initially unassigned
     assert scroll_container.app is None
 
     # Assign the scroll container to the app
     scroll_container.app = app
 
     # Scroll container is on the app
     assert scroll_container.app == app
 
 
 def test_assign_to_window(window, scroll_container, content):
-    """If the widget is assigned to a window, the content is also assigned"""
+    """If the widget is assigned to a window, the content is also assigned."""
     # Scroll container is initially unassigned
     assert scroll_container.window is None
 
     # Assign the scroll container to the window
     scroll_container.window = window
 
     # Scroll container is on the window
     assert scroll_container.window == window
     # Content is also on the window
     assert content.window == window
 
 
 def test_assign_to_window_no_content(window):
-    """If the widget is assigned to an app, and there is no content, there's no error"""
+    """If the widget is assigned to an app, and there is no content, there's no
+    error."""
     scroll_container = toga.ScrollContainer()
 
     # Scroll container is initially unassigned
     assert scroll_container.window is None
 
     # Assign the scroll container to the window
     scroll_container.window = window
 
     # Scroll container is on the window
     assert scroll_container.window == window
 
 
 def test_disable_no_op(scroll_container):
-    "ScrollContainer doesn't have a disabled state"
+    """ScrollContainer doesn't have a disabled state."""
     # Enabled by default
     assert scroll_container.enabled
 
     # Try to disable the widget
     scroll_container.enabled = False
 
     # Still enabled.
     assert scroll_container.enabled
 
 
 def test_focus_noop(scroll_container):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     scroll_container.focus()
     assert_action_not_performed(scroll_container, "focus")
 
 
 def test_set_content(app, window, scroll_container, content):
-    """The content of the scroll container can be changed"""
+    """The content of the scroll container can be changed."""
     # Assign the scroll container to an app and window
     scroll_container.app = app
     scroll_container.window = window
 
     # The content is also assigned
     assert content.app == app
     assert content.window == window
@@ -184,15 +186,15 @@
 
     # The old content isn't
     assert content.app is None
     assert content.window is None
 
 
 def test_clear_content(app, window, scroll_container, content):
-    """The content of the scroll container can be cleared"""
+    """The content of the scroll container can be cleared."""
     # Assign the scroll container to an app and window
     scroll_container.app = app
     scroll_container.window = window
 
     # The content is also assigned
     assert content.app == app
     assert content.window == window
@@ -205,15 +207,15 @@
 
     # The content has been assigned to the widget
     assert_action_performed_with(scroll_container, "set content", widget=None)
 
     # The content has been cleared
     assert scroll_container.content is None
 
-    # The old content isn't assigned any more
+    # The old content isn't assigned anymore
     assert content.app is None
     assert content.window is None
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
@@ -224,15 +226,15 @@
         ("True", True),
         ("False", True),  # non-empty string is truthy
         ("", False),
         (object(), True),
     ],
 )
 def test_horizontal(scroll_container, on_scroll_handler, content, value, expected):
-    "Horizontal scrolling can be enabled/disabled."
+    """Horizontal scrolling can be enabled/disabled."""
     scroll_container.horizontal = value
     scroll_container.horizontal == expected
 
     if not expected:
         on_scroll_handler.assert_called_with(scroll_container)
     else:
         on_scroll_handler.assert_not_called()
@@ -251,15 +253,15 @@
         ("True", True),
         ("False", True),  # non-empty string is truthy
         ("", False),
         (object(), True),
     ],
 )
 def test_vertical(scroll_container, on_scroll_handler, content, value, expected):
-    "Vertical scrolling can be enabled/disabled."
+    """Vertical scrolling can be enabled/disabled."""
     scroll_container.vertical = value
     scroll_container.vertical == expected
 
     if not expected:
         on_scroll_handler.assert_called_with(scroll_container)
     else:
         on_scroll_handler.assert_not_called()
@@ -275,26 +277,26 @@
         (-100, 0),  # Clipped to minimum value
         (1500, 1000),  # Clipped to maximum value
         ("10", 10),  # String, converted to int
         (10.1, 10),  # Float, converted to int
     ],
 )
 def test_horizontal_position(scroll_container, on_scroll_handler, position, expected):
-    "The horizontal position can be set (clipped if necessary) and retrieved"
+    """The horizontal position can be set (clipped if necessary) and retrieved."""
     scroll_container.horizontal_position = position
 
     # scroll handler fired
     on_scroll_handler.assert_called_with(scroll_container)
 
     assert scroll_container.horizontal_position == expected
     assert scroll_container.max_horizontal_position == 1000
 
 
 def test_disable_horizontal_scrolling(scroll_container, on_scroll_handler):
-    "When disabling horizontal scrolling, horizontal position resets"
+    """When disabling horizontal scrolling, horizontal position resets."""
     scroll_container.horizontal_position = 100
     on_scroll_handler.reset_mock()
 
     scroll_container.horizontal = False
 
     # scroll handler fired as a result of reset
     on_scroll_handler.assert_called_with(scroll_container)
@@ -309,15 +311,16 @@
 
     # scroll handler fired
     on_scroll_handler.assert_called_with(scroll_container)
     on_scroll_handler.reset_mock()
 
 
 def test_horizontal_position_when_not_horizontal(scroll_container):
-    "If horizontal scrolling isn't enabled, setting the horizontal position raises an error"
+    """If horizontal scrolling isn't enabled, setting the horizontal position raises an
+    error."""
     scroll_container.horizontal = False
     with pytest.raises(
         ValueError,
         match=r"Cannot set horizontal position when horizontal scrolling is not enabled.",
     ):
         scroll_container.horizontal_position = 37
 
@@ -335,26 +338,26 @@
         (-100, 0),  # Clipped to minimum value
         (2500, 2000),  # Clipped to maximum value
         ("10", 10),  # String, converted to int
         (10.1, 10),  # Float, converted to int
     ],
 )
 def test_vertical_position(scroll_container, on_scroll_handler, position, expected):
-    "The vertical position can be set (clipped if necessary) and retrieved"
+    """The vertical position can be set (clipped if necessary) and retrieved."""
     scroll_container.vertical_position = position
 
     # scroll handler fired
     on_scroll_handler.assert_called_with(scroll_container)
 
     assert scroll_container.vertical_position == expected
     assert scroll_container.max_vertical_position == 2000
 
 
 def test_disable_vertical_scrolling(scroll_container, on_scroll_handler):
-    "When vertical scrolling is disabled, vertical position resets"
+    """When vertical scrolling is disabled, vertical position resets."""
     scroll_container.vertical_position = 100
 
     scroll_container.vertical = False
 
     # scroll handler fired as a result of reset
     on_scroll_handler.assert_called_with(scroll_container)
     on_scroll_handler.reset_mock()
@@ -369,15 +372,16 @@
 
     # scroll handler fired
     on_scroll_handler.assert_called_with(scroll_container)
     on_scroll_handler.reset_mock()
 
 
 def test_set_vertical_position_when_not_vertical(scroll_container):
-    "If vertical scrolling isn't enabled, setting the vertical position raises an error"
+    """If vertical scrolling isn't enabled, setting the vertical position raises an
+    error."""
     scroll_container.vertical = False
     with pytest.raises(
         ValueError,
         match=r"Cannot set vertical position when vertical scrolling is not enabled.",
     ):
         scroll_container.vertical_position = 42
 
@@ -397,14 +401,14 @@
         ((-100, -100), (0, 0)),  # Clipped to minimum
         ((1500, 42), (1000, 42)),  # Clipped to maximum horizontal value
         ((37, 2500), (37, 2000)),  # Clipped to maximum vertical value
         ((1500, 2500), (1000, 2000)),  # Clipped to maximum
     ],
 )
 def test_position(scroll_container, on_scroll_handler, position, expected):
-    "The scroll position can be set (clipped if necessary) and retrieved"
+    """The scroll position can be set (clipped if necessary) and retrieved."""
     scroll_container.position = position
 
     assert scroll_container.position == expected
 
     # scroll handler fired
     on_scroll_handler.assert_called_with(scroll_container)
```

### Comparing `toga-core-0.4.2/tests/widgets/test_selection.py` & `toga_core-0.4.3/tests/widgets/test_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,28 @@
         items=source,
         value=source[1],
         on_change=on_change_handler,
     )
 
 
 def test_widget_created():
-    "An empty selection can be created"
+    """An empty selection can be created."""
     widget = toga.Selection()
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create Selection")
 
     assert len(widget.items) == 0
     assert widget._accessor is None
     assert widget.value is None
     assert widget.on_change._raw is None
     assert widget.enabled
 
 
 def test_create_with_value():
-    "A Selection can be created with initial values"
+    """A Selection can be created with initial values."""
     on_change = Mock()
 
     widget = toga.Selection(
         items=["first", "second", "third"],
         value="second",
         on_change=on_change,
         enabled=False,
@@ -102,15 +102,15 @@
         # List of strings with a newline in value
         (["first", "second\nitem", "third"], "second", "second\nitem"),
         # List of strings with a duplicate entry
         (["first", "second", "third", "first", "second"], "second", "second"),
     ],
 )
 def test_value_no_accessor(items, title, value):
-    "If there's no accessor, the items can be set and values will be dereferenced"
+    """If there's no accessor, the items can be set and values will be dereferenced."""
     on_change_handler = Mock()
     widget = toga.Selection(on_change=on_change_handler)
 
     # There haven't been any changes
     on_change_handler.assert_not_called()
 
     # Change the items. This changes the selection, triggering the handler
@@ -179,15 +179,15 @@
         # List of strings with a newline in a title
         ("key", ["first", "second\nitem", "third"], "second", "second\nitem"),
         # List of strings with a duplicate entry
         ("key", ["first", "second", "third", "first", "second"], "second", "second"),
     ],
 )
 def test_value_with_accessor(accessor, items, title, value):
-    "If an accessor is used, item lookup semantics are different"
+    """If an accessor is used, item lookup semantics are different."""
     on_change_handler = Mock()
     widget = toga.Selection(accessor=accessor, on_change=on_change_handler)
 
     # There haven't been any changes
     on_change_handler.assert_not_called()
 
     # Change the items. This changes the selection, triggering the handler
@@ -220,26 +220,26 @@
         ValueError,
         match=r"Must specify an accessor to use a data source",
     ):
         toga.Selection(items=ListSource(accessors=["foo", "bar"]))
 
 
 def test_bad_item_no_accessor():
-    """The value for the selection must exist in accessor-less data"""
+    """The value for the selection must exist in accessor-less data."""
     selection = toga.Selection(items=["first", "second", "third"])
 
     with pytest.raises(
         ValueError,
         match=r"'bad' is not a current item in the selection",
     ):
         selection.value = "bad"
 
 
 def test_bad_item_with_accessor():
-    """The value for the selection must exist in accessor-based data"""
+    """The value for the selection must exist in accessor-based data."""
     # Create a selection with an extra item and an explicit accessor
     selection = toga.Selection(
         accessor="value", items=["first", "bad", "second", "third"]
     )
 
     # Store the bad item
     item = selection.items.find(dict(value="bad"))
@@ -267,30 +267,30 @@
 
     # This doesn't change the widget.
     on_change_handler.assert_not_called()
     assert widget.value == selection
 
 
 def test_insert_item(widget, source, on_change_handler):
-    """A row can be inserted into the source"""
+    """A row can be inserted into the source."""
     # Store the original selection
     selection = widget.value
 
     source.insert(1, dict(key="new", value=999))
 
     # The widget adds the item
     assert_action_performed_with(widget, "insert item", index=1)
 
     # This doesn't change the widget
     on_change_handler.assert_not_called()
     assert widget.value == selection
 
 
 def test_remove(widget, source, on_change_handler):
-    """If you remove an item that isn't selected, no change is generated"""
+    """If you remove an item that isn't selected, no change is generated."""
     # Store the original selection
     selection = widget.value
 
     # Remove a non-selected item
     item = source[0]
     source.remove(item)
 
@@ -299,84 +299,84 @@
 
     # This changes the selection
     on_change_handler.assert_not_called()
     assert widget.value == selection
 
 
 def test_remove_selected(widget, source, on_change_handler):
-    """If you remove the currently selected item, a change is generated"""
+    """If you remove the currently selected item, a change is generated."""
     # Store the original selection
     selection = widget.value
 
     source.remove(selection)
 
     # The widget adds the item
     assert_action_performed_with(widget, "remove item", index=1, item=selection)
 
     # This changes the selection
     on_change_handler.assert_called_with(widget)
     assert widget.value == source[0]
 
 
 def test_clear_source(widget, source, on_change_handler):
-    "If the source is cleared, the selection is cleared"
+    """If the source is cleared, the selection is cleared."""
     # Clear the source
     source.clear()
 
     # The widget has been cleared
     assert_action_performed(widget, "clear")
 
-    # The widget must have cleared it's selection
+    # The widget must have cleared its selection
     on_change_handler.assert_called_with(widget)
     assert widget.value is None
 
 
 def test_change_source_empty(widget, on_change_handler):
-    """If the source is changed to an empty source, the selection is reset"""
+    """If the source is changed to an empty source, the selection is reset."""
     # Clear the event history
     EventLog.reset()
 
     widget.items = []
 
     # The widget data has been cleared and refreshed
     assert_action_performed(widget, "clear")
     assert_action_not_performed(widget, "insert item")
     assert_action_performed(widget, "refresh")
 
-    # The widget must have cleared it's selection
+    # The widget must have cleared its selection
     on_change_handler.assert_called_once_with(widget)
     assert widget.value is None
 
 
 def test_change_source(widget, on_change_handler):
-    """If the source is changed, the selection is set to the first item"""
+    """If the source is changed, the selection is set to the first item."""
     # Clear the event history
     EventLog.reset()
 
     # Change the source of the data
     widget.items = ["new 1", "new 2"]
 
     # The widget source has changed
     assert_action_performed(widget, "clear")
     assert_action_performed_with(widget, "insert item", item=widget.items[0])
     assert_action_performed_with(widget, "insert item", item=widget.items[1])
     assert_action_performed(widget, "refresh")
 
-    # The widget must have cleared it's selection
+    # The widget must have cleared its selection
     on_change_handler.assert_called_once_with(widget)
     assert widget.value.key == "new 1"
 
 
 ######################################################################
 # 2023-05: Backwards compatibility
 ######################################################################
 
 
 def test_deprecated_names(on_change_handler):
-    "Deprecated names still work"
+    """Deprecated names still work."""
 
     # Can't specify both on_select and on_change
     with pytest.raises(
         ValueError,
         match=r"Cannot specify both on_select and on_change",
     ):
         toga.Selection(on_select=Mock(), on_change=Mock())
```

### Comparing `toga-core-0.4.2/tests/widgets/test_slider.py` & `toga_core-0.4.3/tests/widgets/test_slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         value=INITIAL_MAX,
         tick_value=INITIAL_TICK_COUNT,
         change_count=1,
     )
 
 
 def test_set_value_to_be_too_small(slider, on_change):
-    "Setting the value below the minimum results in clipping"
+    """Setting the value below the minimum results in clipping."""
     slider.value = INITIAL_MIN - 1
     assert_value(slider, on_change, tick_value=1, value=INITIAL_MIN, change_count=1)
 
 
 def test_set_value_to_be_too_big(slider, on_change):
-    "Setting the value above the maximum results in clipping"
+    """Setting the value above the maximum results in clipping."""
     slider.value = INITIAL_MAX + 1
     assert_value(slider, on_change, tick_value=11, value=INITIAL_MAX, change_count=1)
 
 
 def test_set_tick_value_between_min_and_max(slider, on_change):
     value = 30
     tick_value = 4
@@ -109,21 +109,21 @@
         value=INITIAL_MAX,
         tick_value=INITIAL_TICK_COUNT,
         change_count=1,
     )
 
 
 def test_set_tick_value_to_be_too_small(slider, on_change):
-    "Setting the tick value to less than the min results in clipping"
+    """Setting the tick value to less than the min results in clipping."""
     slider.tick_value = 0
     assert_value(slider, on_change, tick_value=1, value=INITIAL_MIN, change_count=1)
 
 
 def test_set_tick_value_to_be_too_big(slider, on_change):
-    "Setting the tick value to greater than the max results in clipping"
+    """Setting the tick value to greater than the max results in clipping."""
     slider.tick_value = INITIAL_TICK_COUNT + 1
     assert_value(slider, on_change, tick_value=11, value=INITIAL_MAX, change_count=1)
 
 
 def test_tick_value_without_tick_count(slider, on_change):
     slider.tick_count = None
     with raises(ValueError, match="cannot set tick value when tick count is None"):
@@ -543,15 +543,15 @@
         impl.int_value = int_value
         impl.on_change()
         assert impl.get_value() == approx(value)
         impl.interface.on_change.assert_called_once_with()
 
 
 def test_deprecated():
-    "Check the deprecated min/max naming"
+    """Check the deprecated min/max naming."""
     # Can't specify min and range
     with pytest.raises(
         ValueError,
         match=r"range cannot be specified if min and max are specified",
     ):
         toga.Slider(min=2, range=(2, 4))
```

### Comparing `toga-core-0.4.2/tests/widgets/test_splitcontainer.py` & `toga_core-0.4.3/tests/widgets/test_splitcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 
 @pytest.fixture
 def splitcontainer(content1, content2):
     return toga.SplitContainer(content=[content1, content2])
 
 
 def test_widget_created():
-    "A scroll container can be created with no arguments"
+    """A scroll container can be created with no arguments."""
     splitcontainer = toga.SplitContainer()
     assert splitcontainer._impl.interface == splitcontainer
     assert_action_performed(splitcontainer, "create SplitContainer")
 
     assert splitcontainer.content == (None, None)
     assert splitcontainer.direction == toga.SplitContainer.VERTICAL
 
 
 def test_widget_created_with_values(content1, content2):
-    "A split container can be created with arguments"
+    """A split container can be created with arguments."""
     splitcontainer = toga.SplitContainer(
         content=[content1, content2],
         direction=toga.SplitContainer.HORIZONTAL,
     )
     assert splitcontainer._impl.interface == splitcontainer
     assert_action_performed(splitcontainer, "create SplitContainer")
 
@@ -73,15 +73,15 @@
         (False, False),
         (False, True),
         (True, False),
         (True, True),
     ],
 )
 def test_assign_to_app(app, content1, content2, include_left, include_right):
-    """If the widget is assigned to an app, the content is also assigned"""
+    """If the widget is assigned to an app, the content is also assigned."""
     splitcontainer = toga.SplitContainer(
         content=[
             content1 if include_left else None,
             content2 if include_right else None,
         ]
     )
 
@@ -99,15 +99,16 @@
         assert content1.app == app
 
     if include_right:
         assert content2.app == app
 
 
 def test_assign_to_app_no_content(app):
-    """If the widget is assigned to an app, and there is no content, there's no error"""
+    """If the widget is assigned to an app, and there is no content, there's no
+    error."""
     splitcontainer = toga.SplitContainer()
 
     # Scroll container is initially unassigned
     assert splitcontainer.app is None
 
     # Assign the scroll container to the app
     splitcontainer.app = app
@@ -122,15 +123,15 @@
         (False, False),
         (False, True),
         (True, False),
         (True, True),
     ],
 )
 def test_assign_to_window(window, content1, content2, include_left, include_right):
-    """If the widget is assigned to a window, the content is also assigned"""
+    """If the widget is assigned to a window, the content is also assigned."""
     splitcontainer = toga.SplitContainer(
         content=[
             content1 if include_left else None,
             content2 if include_right else None,
         ]
     )
 
@@ -148,41 +149,42 @@
         assert content1.window == window
 
     if include_right:
         assert content2.window == window
 
 
 def test_assign_to_window_no_content(window):
-    """If the widget is assigned to an app, and there is no content, there's no error"""
+    """If the widget is assigned to an app, and there is no content, there's no
+    error."""
     splitcontainer = toga.SplitContainer()
 
     # Scroll container is initially unassigned
     assert splitcontainer.window is None
 
     # Assign the scroll container to the window
     splitcontainer.window = window
 
     # Scroll container is on the window
     assert splitcontainer.window == window
 
 
 def test_disable_no_op(splitcontainer):
-    "SplitContainer doesn't have a disabled state"
+    """SplitContainer doesn't have a disabled state."""
     # Enabled by default
     assert splitcontainer.enabled
 
     # Try to disable the widget
     splitcontainer.enabled = False
 
     # Still enabled.
     assert splitcontainer.enabled
 
 
 def test_focus_noop(splitcontainer):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     splitcontainer.focus()
     assert_action_not_performed(splitcontainer, "focus")
 
 
 @pytest.mark.parametrize(
     "include_left, include_right",
@@ -197,15 +199,15 @@
     splitcontainer,
     content1,
     content2,
     content3,
     include_left,
     include_right,
 ):
-    """Widget content can be set to a list of widgets"""
+    """Widget content can be set to a list of widgets."""
     splitcontainer.content = [
         content2 if include_left else None,
         content3 if include_right else None,
     ]
 
     assert_action_performed_with(
         splitcontainer,
@@ -233,15 +235,15 @@
 def test_set_content_flex(
     splitcontainer,
     content2,
     content3,
     include_left,
     include_right,
 ):
-    """Widget content can be set to a list of widgets with flex values"""
+    """Widget content can be set to a list of widgets with flex values."""
     splitcontainer.content = [
         (content2 if include_left else None, 2),
         (content3 if include_right else None, 3),
     ]
 
     assert_action_performed_with(
         splitcontainer,
@@ -269,15 +271,15 @@
 def test_set_content_flex_mixed(
     splitcontainer,
     content2,
     content3,
     include_left,
     include_right,
 ):
-    """Flex values will be defaulted if missing"""
+    """Flex values will be defaulted if missing."""
     splitcontainer.content = [
         content2 if include_left else None,
         (content3 if include_right else None, 3),
     ]
 
     assert_action_performed_with(
         splitcontainer,
@@ -329,22 +331,22 @@
         (
             [toga.Box(), (toga.Box(), -1)],
             r"The flex value for an item in a SplitContainer must be >0",
         ),
     ],
 )
 def test_set_content_invalid(splitcontainer, content, message):
-    """Widget content can only be set to valid values"""
+    """Widget content can only be set to valid values."""
 
     with pytest.raises(ValueError, match=message):
         splitcontainer.content = content
 
 
 def test_direction(splitcontainer):
-    """The direction of the splitcontainer can be changed"""
+    """The direction of the splitcontainer can be changed."""
 
     splitcontainer.direction = toga.SplitContainer.HORIZONTAL
 
     # The direction has been set
     assert splitcontainer.direction == toga.SplitContainer.HORIZONTAL
 
     # The split container has been refreshed
```

### Comparing `toga-core-0.4.2/tests/widgets/test_switch.py` & `toga_core-0.4.3/tests/widgets/test_switch.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         (None, ""),
         ("\u200B", ""),
         (12345, "12345"),
         ("Contains\nnewline", "Contains"),
     ],
 )
 def test_label_text(switch, value, expected):
-    "The switch's label can be modified."
+    """The switch's label can be modified."""
     assert switch.text == "Test Switch"
 
     # Clear the event log
     EventLog.reset()
 
     switch.text = value
     assert switch.text == expected
@@ -81,32 +81,32 @@
         ("", False),
         (None, False),
         (1234, True),
         (0, False),
     ],
 )
 def test_value_change(switch, value, expected):
-    "The value of the switch can be set from almost any value."
+    """The value of the switch can be set from almost any value."""
     switch.value = value
     assert switch.value == expected
 
 
 def test_toggle(switch):
-    "Toggle can be used to change the value"
+    """Toggle can be used to change the value."""
     assert not switch.value
 
     switch.toggle()
     assert switch.value
 
     switch.toggle()
     assert not switch.value
 
 
 def test_on_change(switch):
-    "The on_change handler is invoked whenever the value is changed."
+    """The on_change handler is invoked whenever the value is changed."""
     handler = MagicMock()
     switch.on_change = handler
 
     # Reset the mock; installing the mock causes it to be evaluated as a bool()
     handler.reset_mock()
 
     # Set the value explicitly using a non-bool value
```

### Comparing `toga-core-0.4.2/tests/widgets/test_table.py` & `toga_core-0.4.3/tests/widgets/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,30 @@
         data=source,
         on_select=on_select_handler,
         on_activate=on_activate_handler,
     )
 
 
 def test_table_created():
-    "An minimal Table can be created"
+    """A minimal Table can be created."""
     table = toga.Table(["First", "Second"])
     assert table._impl.interface == table
     assert_action_performed(table, "create Table")
 
     assert len(table.data) == 0
     assert table.headings == ["First", "Second"]
     assert table.accessors == ["first", "second"]
     assert not table.multiple_select
     assert table.missing_value == ""
     assert table.on_select._raw is None
     assert table.on_activate._raw is None
 
 
 def test_create_with_values(source, on_select_handler, on_activate_handler):
-    "A Table can be created with initial values"
+    """A Table can be created with initial values."""
     table = toga.Table(
         ["First", "Second"],
         data=source,
         accessors=["primus", "secondus"],
         multiple_select=True,
         on_select=on_select_handler,
         on_activate=on_activate_handler,
@@ -79,64 +79,64 @@
     assert table.multiple_select
     assert table.missing_value == "Boo!"
     assert table.on_select._raw == on_select_handler
     assert table.on_activate._raw == on_activate_handler
 
 
 def test_create_with_accessor_overrides():
-    "A Table can partially override accessors"
+    """A Table can partially override accessors."""
     table = toga.Table(
         ["First", "Second"],
         accessors={"First": "override"},
     )
     assert table._impl.interface == table
     assert_action_performed(table, "create Table")
 
     assert len(table.data) == 0
     assert table.headings == ["First", "Second"]
     assert table.accessors == ["override", "second"]
 
 
 def test_create_no_headings():
-    "A Table can be created with no headings"
+    """A Table can be created with no headings."""
     table = toga.Table(
         headings=None,
         accessors=["primus", "secondus"],
     )
     assert table._impl.interface == table
     assert_action_performed(table, "create Table")
 
     assert len(table.data) == 0
     assert table.headings is None
     assert table.accessors == ["primus", "secondus"]
 
 
 def test_create_headings_required():
-    "A Table requires either headingscan be created with no headings"
+    """A Table requires either headings can be created with no headings."""
     with pytest.raises(
         ValueError,
         match=r"Cannot create a table without either headings or accessors",
     ):
         toga.Table()
 
 
 def test_disable_no_op(table):
-    "Table doesn't have a disabled state"
+    """Table doesn't have a disabled state."""
     # Enabled by default
     assert table.enabled
 
     # Try to disable the widget
     table.enabled = False
 
     # Still enabled.
     assert table.enabled
 
 
 def test_focus_noop(table):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     table.focus()
     assert_action_not_performed(table, "focus")
 
 
 @pytest.mark.parametrize(
     "data, all_attributes, extra_attributes",
@@ -180,15 +180,15 @@
             ],
             False,
             False,
         ),
     ],
 )
 def test_set_data(table, on_select_handler, data, all_attributes, extra_attributes):
-    "Data can be set from a variety of sources"
+    """Data can be set from a variety of sources."""
 
     # The selection hasn't changed yet.
     on_select_handler.assert_not_called()
 
     # Change the data
     table.data = data
 
@@ -214,15 +214,15 @@
     if extra_attributes:
         assert table.data[0].extra == "extra1"
         assert table.data[1].extra == "extra2"
         assert table.data[2].extra == "extra3"
 
 
 def test_single_selection(table, on_select_handler):
-    "The current selection can be retrieved"
+    """The current selection can be retrieved."""
     # Selection is initially empty
     assert table.selection is None
     on_select_handler.assert_not_called()
 
     # Select an item
     table._impl.simulate_selection(1)
 
@@ -230,15 +230,15 @@
     assert table.selection == table.data[1]
 
     # Selection handler was triggered
     on_select_handler.assert_called_once_with(table)
 
 
 def test_multiple_selection(source, on_select_handler):
-    "A multi-select table can have the selection retrieved"
+    """A multi-select table can have the selection retrieved."""
     table = toga.Table(
         ["Title", "Value"],
         data=source,
         multiple_select=True,
         on_select=on_select_handler,
     )
     # Selection is initially empty
@@ -252,25 +252,25 @@
     assert table.selection == [table.data[0], table.data[2]]
 
     # Selection handler was triggered
     on_select_handler.assert_called_once_with(table)
 
 
 def test_activation(table, on_activate_handler):
-    "A row can be activated"
+    """A row can be activated."""
 
     # Activate an item
     table._impl.simulate_activate(1)
 
     # Activate handler was triggered; the activated row is provided
     on_activate_handler.assert_called_once_with(table, row=table.data[1])
 
 
 def test_scroll_to_top(table):
-    "A table can be scrolled to the top"
+    """A table can be scrolled to the top."""
     table.scroll_to_top()
 
     assert_action_performed_with(table, "scroll to row", row=0)
 
 
 @pytest.mark.parametrize(
     "row, effective",
@@ -284,38 +284,38 @@
         (-1, 2),
         (-3, 0),
         # Greater negative index than available rows
         (-10, 0),
     ],
 )
 def test_scroll_to_row(table, row, effective):
-    "A table can be scrolled to a specific row"
+    """A table can be scrolled to a specific row."""
     table.scroll_to_row(row)
 
     assert_action_performed_with(table, "scroll to row", row=effective)
 
 
 def test_scroll_to_row_no_data(table):
-    "If there's no data, scrolling is a no-op"
+    """If there's no data, scrolling is a no-op."""
     table.data.clear()
 
     table.scroll_to_row(5)
 
     assert_action_not_performed(table, "scroll to row")
 
 
 def test_scroll_to_bottom(table):
-    "A table can be scrolled to the top"
+    """A table can be scrolled to the top."""
     table.scroll_to_bottom()
 
     assert_action_performed_with(table, "scroll to row", row=2)
 
 
 def test_insert_column_accessor(table):
-    """A column can be inserted at an accessor"""
+    """A column can be inserted at an accessor."""
     table.insert_column("value", "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
         index=1,
@@ -323,21 +323,21 @@
         accessor="extra",
     )
     assert table.headings == ["Title", "New Column", "Value"]
     assert table.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_unknown_accessor(table):
-    """If the insertion index accessor is unknown, an error is raised"""
+    """If the insertion index accessor is unknown, an error is raised."""
     with pytest.raises(ValueError, match=r"'unknown' is not in list"):
         table.insert_column("unknown", "New Column", accessor="extra")
 
 
 def test_insert_column_index(table):
-    """A column can be inserted"""
+    """A column can be inserted."""
 
     table.insert_column(1, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
@@ -346,15 +346,15 @@
         accessor="extra",
     )
     assert table.headings == ["Title", "New Column", "Value"]
     assert table.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_big_index(table):
-    """A column can be inserted at an index bigger than the number of columns"""
+    """A column can be inserted at an index bigger than the number of columns."""
 
     table.insert_column(100, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
@@ -363,15 +363,15 @@
         accessor="extra",
     )
     assert table.headings == ["Title", "Value", "New Column"]
     assert table.accessors == ["key", "value", "extra"]
 
 
 def test_insert_column_negative_index(table):
-    """A column can be inserted at a negative index"""
+    """A column can be inserted at a negative index."""
 
     table.insert_column(-2, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
@@ -380,15 +380,16 @@
         accessor="extra",
     )
     assert table.headings == ["New Column", "Title", "Value"]
     assert table.accessors == ["extra", "key", "value"]
 
 
 def test_insert_column_big_negative_index(table):
-    """A column can be inserted at a negative index larger than the number of columns"""
+    """A column can be inserted at a negative index larger than the number of
+    columns."""
 
     table.insert_column(-100, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
@@ -397,15 +398,15 @@
         accessor="extra",
     )
     assert table.headings == ["New Column", "Title", "Value"]
     assert table.accessors == ["extra", "key", "value"]
 
 
 def test_insert_column_no_accessor(table):
-    """A column can be inserted with a default accessor"""
+    """A column can be inserted with a default accessor."""
 
     table.insert_column(1, "New Column")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
@@ -414,15 +415,15 @@
         accessor="new_column",
     )
     assert table.headings == ["Title", "New Column", "Value"]
     assert table.accessors == ["key", "new_column", "value"]
 
 
 def test_insert_column_no_headings(source):
-    """A column can be inserted into a table with no headings"""
+    """A column can be inserted into a table with no headings."""
     table = toga.Table(headings=None, accessors=["key", "value"], data=source)
 
     table.insert_column(1, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
@@ -432,26 +433,26 @@
         accessor="extra",
     )
     assert table.headings is None
     assert table.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_no_headings_missing_accessor(source):
-    """An accessor is mandatory when adding a column to a table with no headings"""
+    """An accessor is mandatory when adding a column to a table with no headings."""
     table = toga.Table(headings=None, accessors=["key", "value"], data=source)
 
     with pytest.raises(
         ValueError,
         match=r"Must specify an accessor on a table without headings",
     ):
         table.insert_column(1, "New Column")
 
 
 def test_append_column(table):
-    """A column can be appended"""
+    """A column can be appended."""
     table.append_column("New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         table,
         "insert column",
         index=2,
@@ -459,72 +460,72 @@
         accessor="extra",
     )
     assert table.headings == ["Title", "Value", "New Column"]
     assert table.accessors == ["key", "value", "extra"]
 
 
 def test_remove_column_accessor(table):
-    "A column can be removed by accessor"
+    """A column can be removed by accessor."""
 
     table.remove_column("value")
 
     # The column was removed
     assert_action_performed_with(
         table,
         "remove column",
         index=1,
     )
     assert table.headings == ["Title"]
     assert table.accessors == ["key"]
 
 
 def test_remove_column_unknown_accessor(table):
-    "If the column named for removal doesn't exist, an error is raised"
+    """If the column named for removal doesn't exist, an error is raised."""
     with pytest.raises(ValueError, match=r"'unknown' is not in list"):
         table.remove_column("unknown")
 
 
 def test_remove_column_invalid_index(table):
-    "If the index specified doesn't exist, an error is raised"
+    """If the index specified doesn't exist, an error is raised."""
     with pytest.raises(IndexError, match=r"list assignment index out of range"):
         table.remove_column(100)
 
 
 def test_remove_column_index(table):
-    "A column can be removed by index"
+    """A column can be removed by index."""
 
     table.remove_column(1)
 
     # The column was removed
     assert_action_performed_with(
         table,
         "remove column",
         index=1,
     )
     assert table.headings == ["Title"]
     assert table.accessors == ["key"]
 
 
 def test_remove_column_negative_index(table):
-    "A column can be removed by index"
+    """A column can be removed by index."""
 
     table.remove_column(-2)
 
     # The column was removed
     assert_action_performed_with(
         table,
         "remove column",
         index=0,
     )
     assert table.headings == ["Value"]
     assert table.accessors == ["value"]
 
 
 def test_remove_column_no_headings(table):
-    "A column can be removed when there are no headings"
+    """A column can be removed when there are no headings."""
     table = toga.Table(
         headings=None,
         accessors=["primus", "secondus"],
     )
 
     table.remove_column(1)
 
@@ -535,15 +536,15 @@
         index=1,
     )
     assert table.headings is None
     assert table.accessors == ["primus"]
 
 
 def test_deprecated_names(on_activate_handler):
-    "Deprecated names still work"
+    """Deprecated names still work."""
 
     # Can't specify both on_double_click and on_activate
     with pytest.raises(
         ValueError,
         match=r"Cannot specify both on_double_click and on_activate",
     ):
         toga.Table(["First", "Second"], on_double_click=Mock(), on_activate=Mock())
```

### Comparing `toga-core-0.4.2/tests/widgets/test_textinput.py` & `toga_core-0.4.3/tests/widgets/test_textinput.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 @pytest.fixture
 def widget(validator):
     return toga.TextInput(validators=[validator])
 
 
 def test_widget_created():
-    "A text input can be created"
+    """A text input can be created."""
     widget = toga.TextInput()
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create TextInput")
 
     assert not widget.readonly
     assert widget.placeholder == ""
     assert widget.value == ""
@@ -35,15 +35,15 @@
     assert widget._on_confirm._raw is None
     assert widget._on_gain_focus._raw is None
     assert widget._on_lose_focus._raw is None
     assert widget.validators == []
 
 
 def test_create_with_values():
-    "A multiline text input can be created with initial values"
+    """A multiline text input can be created with initial values."""
     on_change = Mock()
     on_confirm = Mock()
     on_gain_focus = Mock()
     on_lose_focus = Mock()
     validator1 = Mock(return_value=None)
     validator2 = Mock(return_value=None)
 
@@ -121,15 +121,15 @@
         ("true", True),
         ("false", True),  # Evaluated as a string, this value is true.
         (0, False),
         (1234, True),
     ],
 )
 def test_readonly(widget, value, expected):
-    "The readonly status of the widget can be changed."
+    """The readonly status of the widget can be changed."""
     # Widget is initially not readonly by default.
     assert not widget.readonly
 
     # Set the readonly status
     widget.readonly = value
     assert widget.readonly == expected
 
@@ -239,15 +239,15 @@
     widget._impl.simulate_lose_focus()
 
     # Callback was invoked
     handler.assert_called_once_with(widget)
 
 
 def test_change_validators(widget, validator):
-    "If the validator list is changed, the new validators are invoked"
+    """If the validator list is changed, the new validators are invoked."""
     new_validator1 = Mock(return_value=None)
     new_validator2 = Mock(return_value=None)
 
     widget.value = "Some text"
 
     # Clear the validator mock
     validator.reset_mock()
@@ -259,30 +259,30 @@
 
     # Validators have been invoked with the initial text
     new_validator1.assert_called_once_with("Some text")
     new_validator2.assert_called_once_with("Some text")
 
 
 def test_remove_validators(widget, validator):
-    "The validator list can be cleared"
+    """The validator list can be cleared."""
     widget.value = "Some text"
 
     # Clear the event log and validator mock
     EventLog.reset()
     validator.reset_mock()
 
     # Clear the validators
     widget.validators = None
 
     # Old validator hasn't been invoked
     validator.assert_not_called()
 
 
 def test_is_valid(widget):
-    "Widget validity can be evaluated"
+    """Widget validity can be evaluated."""
     validator1 = Mock(return_value=None)
     validator2 = Mock(return_value=None)
 
     widget.validators = [validator1, validator2]
 
     # Widget is initially valid
     assert widget.is_valid
```

### Comparing `toga-core-0.4.2/tests/widgets/test_timeinput.py` & `toga_core-0.4.3/tests/widgets/test_timeinput.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     assert_action_performed(widget, "create TimeInput")
 
     assert widget.value == time(10, 42, 37)
     assert widget.on_change._raw is None
 
 
 def test_widget_created_with_values(on_change_handler):
-    """A TimeInput can be created with initial values"""
+    """A TimeInput can be created with initial values."""
     # Round trip the impl/interface
     widget = toga.TimeInput(
         value=time(13, 37, 42),
         min=time(6, 1, 2),
         max=time(18, 58, 59),
         on_change=on_change_handler,
     )
@@ -58,15 +58,15 @@
         (time(14, 37, 42, 123456), time(14, 37, 42)),
         (datetime(2023, 2, 11, 14, 37, 42, 123456), time(14, 37, 42)),
         ("14:37:42.123456", time(14, 37, 42)),
         (None, time(10, 42, 37)),
     ],
 )
 def test_value(widget, value, expected, on_change_handler):
-    "The value of the datepicker can be set"
+    """The value of the datepicker can be set."""
     widget.value = value
 
     assert widget.value == expected
 
     on_change_handler.assert_called_once_with(widget)
 
 
@@ -76,15 +76,15 @@
     (date(2023, 5, 25), TypeError, "Not a valid time value"),
     ("not a time", ValueError, "Invalid isoformat string: 'not a time'"),
 ]
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_VALUES)
 def test_invalid_value(widget, value, exc, message):
-    "Invalid time values raise an exception"
+    """Invalid time values raise an exception."""
     with pytest.raises(exc, match=message):
         widget.value = value
 
 
 @pytest.mark.parametrize(
     "value, clipped",
     [
@@ -94,15 +94,15 @@
         (time(10, 37, 42), time(10, 37, 42)),
         (time(18, 0, 0), time(18, 0, 0)),
         (time(18, 0, 1), time(18, 0, 0)),
         (time(22, 37, 42), time(18, 0, 0)),
     ],
 )
 def test_value_clipping(widget, value, clipped, on_change_handler):
-    "It the value is inconsistent with min/max, it is clipped."
+    """It the value is inconsistent with min/max, it is clipped."""
     # Set min/max dates, and clear the on_change mock
     widget.min = time(6, 0, 0)
     widget.max = time(18, 0, 0)
     on_change_handler.reset_mock()
 
     # Set the new value
     widget.value = value
@@ -120,23 +120,23 @@
         (None, time(0, 0, 0)),
         (time(6, 1, 11), time(6, 1, 11)),
         (datetime(2023, 6, 16, 6, 2, 11), time(6, 2, 11)),
         ("06:03:11", time(6, 3, 11)),
     ],
 )
 def test_min(widget, value, expected):
-    "The min of the datepicker can be set"
+    """The min of the datepicker can be set."""
     widget.min = value
 
     assert widget.min == expected
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_VALUES)
 def test_invalid_min(widget, value, exc, message):
-    "Invalid min values raise an exception"
+    """Invalid min values raise an exception."""
     widget.max = time(18, 0, 0)
 
     with pytest.raises(exc, match=message):
         widget.min = value
 
 
 @pytest.mark.parametrize(
@@ -148,15 +148,15 @@
         (time(6, 0, 0), True, False),
         (time(12, 0, 0), True, False),
         (time(12, 0, 1), True, True),
         (time(13, 14, 15), True, True),
     ],
 )
 def test_min_clip(widget, on_change_handler, min, clip_value, clip_max):
-    "If the current value or max is before a new min time, it is clipped"
+    """If the current value or max is before a new min time, it is clipped."""
     widget.value = time(3, 42, 37)
     widget.max = time(12, 0, 0)
     on_change_handler.reset_mock()
 
     widget.min = min
     assert widget.min == min
 
@@ -179,23 +179,23 @@
         (None, time(23, 59, 59)),
         (time(18, 1, 11), time(18, 1, 11)),
         (datetime(2023, 5, 25, 18, 2, 11), time(18, 2, 11)),
         ("18:03:11", time(18, 3, 11)),
     ],
 )
 def test_max(widget, value, expected):
-    "The max of the datepicker can be set"
+    """The max of the datepicker can be set."""
     widget.max = value
 
     assert widget.max == expected
 
 
 @pytest.mark.parametrize("value, exc, message", INVALID_VALUES)
 def test_invalid_max(widget, value, exc, message):
-    "Invalid max values raise an exception"
+    """Invalid max values raise an exception."""
     widget.min = time(18, 0, 0)
 
     with pytest.raises(exc, match=message):
         widget.max = value
 
 
 @pytest.mark.parametrize(
@@ -207,15 +207,15 @@
         (time(6, 0, 0), True, False),
         (time(11, 59, 0), True, False),
         (time(12, 0, 0), False, False),
         (time(13, 14, 15), False, False),
     ],
 )
 def test_max_clip(widget, on_change_handler, max, clip_value, clip_min):
-    "If the current value is after a new max date, the value is clipped"
+    """If the current value is after a new max date, the value is clipped."""
     widget.min = time(3, 42, 37)
     widget.value = time(12, 0, 0)
     on_change_handler.reset_mock()
 
     widget.max = max
     assert widget.max == max
 
@@ -234,16 +234,21 @@
 
 def test_deprecated_names():
     MIN = time(8, 30, 59)
     MAX = time(10, 0, 0)
 
     with pytest.warns(
         DeprecationWarning, match="TimePicker has been renamed TimeInput"
+    ), pytest.warns(
+        DeprecationWarning, match="TimePicker.min_time has been renamed TimeInput.min"
+    ), pytest.warns(
+        DeprecationWarning, match="TimePicker.max_time has been renamed TimeInput.max"
     ):
         widget = toga.TimePicker(min_time=MIN, max_time=MAX)
+
     assert widget.min == MIN
     assert widget.max == MAX
     widget.min = widget.max = None
 
     with pytest.warns(
         DeprecationWarning, match="TimePicker.min_time has been renamed TimeInput.min"
     ):
```

### Comparing `toga-core-0.4.2/tests/widgets/test_tree.py` & `toga_core-0.4.3/tests/widgets/test_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,30 +73,30 @@
         data=source,
         on_select=on_select_handler,
         on_activate=on_activate_handler,
     )
 
 
 def test_tree_created():
-    "An minimal Tree can be created"
+    """A minimal Tree can be created."""
     tree = toga.Tree(["First", "Second"])
     assert tree._impl.interface is tree
     assert_action_performed(tree, "create Tree")
 
     assert len(tree.data) == 0
     assert tree.headings == ["First", "Second"]
     assert tree.accessors == ["first", "second"]
     assert not tree.multiple_select
     assert tree.missing_value == ""
     assert tree.on_select._raw is None
     assert tree.on_activate._raw is None
 
 
 def test_create_with_values(source, on_select_handler, on_activate_handler):
-    "A Tree can be created with initial values"
+    """A Tree can be created with initial values."""
     tree = toga.Tree(
         ["First", "Second"],
         data=source,
         accessors=["primus", "secondus"],
         multiple_select=True,
         on_select=on_select_handler,
         on_activate=on_activate_handler,
@@ -110,65 +110,65 @@
     assert tree.accessors == ["primus", "secondus"]
     assert tree.multiple_select
     assert tree.missing_value == "Boo!"
     assert tree.on_select._raw == on_select_handler
     assert tree.on_activate._raw == on_activate_handler
 
 
-def test_create_with_acessor_overrides():
-    "A Tree can partially override accessors"
+def test_create_with_accessor_overrides():
+    """A Tree can partially override accessors."""
     tree = toga.Tree(
         ["First", "Second"],
         accessors={"First": "override"},
     )
     assert tree._impl.interface == tree
     assert_action_performed(tree, "create Tree")
 
     assert len(tree.data) == 0
     assert tree.headings == ["First", "Second"]
     assert tree.accessors == ["override", "second"]
 
 
 def test_create_no_headings():
-    "A Tree can be created with no headings"
+    """A Tree can be created with no headings."""
     tree = toga.Tree(
         headings=None,
         accessors=["primus", "secondus"],
     )
     assert tree._impl.interface == tree
     assert_action_performed(tree, "create Tree")
 
     assert len(tree.data) == 0
     assert tree.headings is None
     assert tree.accessors == ["primus", "secondus"]
 
 
 def test_create_headings_required():
-    "A Tree requires either headingscan be created with no headings"
+    """A Tree requires either headings can be created with no headings."""
     with pytest.raises(
         ValueError,
         match=r"Cannot create a tree without either headings or accessors",
     ):
         toga.Tree()
 
 
 def test_disable_no_op(tree):
-    "Tree doesn't have a disabled state"
+    """Tree doesn't have a disabled state."""
     # Enabled by default
     assert tree.enabled
 
     # Try to disable the widget
     tree.enabled = False
 
     # Still enabled.
     assert tree.enabled
 
 
 def test_focus_noop(tree):
-    "Focus is a no-op."
+    """Focus is a no-op."""
 
     tree.focus()
     assert_action_not_performed(tree, "focus")
 
 
 @pytest.mark.parametrize(
     "data, all_attributes, extra_attributes",
@@ -226,15 +226,15 @@
             ],
             True,
             True,
         ),
     ],
 )
 def test_set_data(tree, on_select_handler, data, all_attributes, extra_attributes):
-    "Data can be set from a variety of sources"
+    """Data can be set from a variety of sources."""
 
     # The selection hasn't changed yet.
     on_select_handler.assert_not_called()
 
     # Change the data
     tree.data = data
 
@@ -261,15 +261,15 @@
     if extra_attributes:
         assert tree.data[0][0].other == "extra1"
         assert tree.data[0][1].other == "extra2"
         assert tree.data[0][2].other == "extra3"
 
 
 def test_single_selection(tree, on_select_handler):
-    "The current selection can be retrieved"
+    """The current selection can be retrieved."""
     # Selection is initially empty
     assert tree.selection is None
     on_select_handler.assert_not_called()
 
     # Select an item
     tree._impl.simulate_selection((0, 1))
 
@@ -277,15 +277,15 @@
     assert tree.selection == tree.data[0][1]
 
     # Selection handler was triggered
     on_select_handler.assert_called_once_with(tree)
 
 
 def test_multiple_selection(source, on_select_handler):
-    "A multi-select tree can have the selection retrieved"
+    """A multi-select tree can have the selection retrieved."""
     tree = toga.Tree(
         ["Title", "Value"],
         data=source,
         multiple_select=True,
         on_select=on_select_handler,
     )
     # Selection is initially empty
@@ -299,15 +299,15 @@
     assert tree.selection == [tree.data[0][1], tree.data[1][2][1]]
 
     # Selection handler was triggered
     on_select_handler.assert_called_once_with(tree)
 
 
 def test_expand_collapse(tree):
-    """The rows on a tree can be expanded and collapsed"""
+    """The rows on a tree can be expanded and collapsed."""
 
     # Expand the full tree
     tree.expand()
     assert_action_performed_with(tree, "expand all")
 
     # Collapse a single node
     tree.collapse(tree.data[1][2])
@@ -327,25 +327,25 @@
 
     # Collapse the full tree
     tree.collapse()
     assert_action_performed_with(tree, "collapse all")
 
 
 def test_activation(tree, on_activate_handler):
-    """A row can be activated"""
+    """A row can be activated."""
 
     # Activate an item
     tree._impl.simulate_activate((0, 1))
 
     # Activate handler was triggered; the activated node is provided
     on_activate_handler.assert_called_once_with(tree, node=tree.data[0][1])
 
 
 def test_insert_column_accessor(tree):
-    """A column can be inserted at an accessor"""
+    """A column can be inserted at an accessor."""
     tree.insert_column("value", "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
         index=1,
@@ -353,21 +353,21 @@
         accessor="extra",
     )
     assert tree.headings == ["Title", "New Column", "Value"]
     assert tree.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_unknown_accessor(tree):
-    """If the insertion index accessor is unknown, an error is raised"""
+    """If the insertion index accessor is unknown, an error is raised."""
     with pytest.raises(ValueError, match=r"'unknown' is not in list"):
         tree.insert_column("unknown", "New Column", accessor="extra")
 
 
 def test_insert_column_index(tree):
-    """A column can be inserted"""
+    """A column can be inserted."""
 
     tree.insert_column(1, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
@@ -376,15 +376,15 @@
         accessor="extra",
     )
     assert tree.headings == ["Title", "New Column", "Value"]
     assert tree.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_big_index(tree):
-    """A column can be inserted at an index bigger than the number of columns"""
+    """A column can be inserted at an index bigger than the number of columns."""
 
     tree.insert_column(100, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
@@ -393,15 +393,15 @@
         accessor="extra",
     )
     assert tree.headings == ["Title", "Value", "New Column"]
     assert tree.accessors == ["key", "value", "extra"]
 
 
 def test_insert_column_negative_index(tree):
-    """A column can be inserted at a negative index"""
+    """A column can be inserted at a negative index."""
 
     tree.insert_column(-2, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
@@ -410,15 +410,16 @@
         accessor="extra",
     )
     assert tree.headings == ["New Column", "Title", "Value"]
     assert tree.accessors == ["extra", "key", "value"]
 
 
 def test_insert_column_big_negative_index(tree):
-    """A column can be inserted at a negative index larger than the number of columns"""
+    """A column can be inserted at a negative index larger than the number of
+    columns."""
 
     tree.insert_column(-100, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
@@ -427,15 +428,15 @@
         accessor="extra",
     )
     assert tree.headings == ["New Column", "Title", "Value"]
     assert tree.accessors == ["extra", "key", "value"]
 
 
 def test_insert_column_no_accessor(tree):
-    """A column can be inserted with a default accessor"""
+    """A column can be inserted with a default accessor."""
 
     tree.insert_column(1, "New Column")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
@@ -444,15 +445,15 @@
         accessor="new_column",
     )
     assert tree.headings == ["Title", "New Column", "Value"]
     assert tree.accessors == ["key", "new_column", "value"]
 
 
 def test_insert_column_no_headings(source):
-    """A column can be inserted into a tree with no headings"""
+    """A column can be inserted into a tree with no headings."""
     tree = toga.Tree(headings=None, accessors=["key", "value"], data=source)
 
     tree.insert_column(1, "New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
@@ -462,26 +463,26 @@
         accessor="extra",
     )
     assert tree.headings is None
     assert tree.accessors == ["key", "extra", "value"]
 
 
 def test_insert_column_no_headings_missing_accessor(source):
-    """An accessor is mandatory when adding a column to a tree with no headings"""
+    """An accessor is mandatory when adding a column to a tree with no headings."""
     tree = toga.Tree(headings=None, accessors=["key", "value"], data=source)
 
     with pytest.raises(
         ValueError,
         match=r"Must specify an accessor on a tree without headings",
     ):
         tree.insert_column(1, "New Column")
 
 
 def test_append_column(tree):
-    """A column can be appended"""
+    """A column can be appended."""
     tree.append_column("New Column", accessor="extra")
 
     # The column was added
     assert_action_performed_with(
         tree,
         "insert column",
         index=2,
@@ -489,72 +490,72 @@
         accessor="extra",
     )
     assert tree.headings == ["Title", "Value", "New Column"]
     assert tree.accessors == ["key", "value", "extra"]
 
 
 def test_remove_column_accessor(tree):
-    "A column can be removed by accessor"
+    """A column can be removed by accessor."""
 
     tree.remove_column("value")
 
     # The column was removed
     assert_action_performed_with(
         tree,
         "remove column",
         index=1,
     )
     assert tree.headings == ["Title"]
     assert tree.accessors == ["key"]
 
 
 def test_remove_column_unknown_accessor(tree):
-    "If the column named for removal doesn't exist, an error is raised"
+    """If the column named for removal doesn't exist, an error is raised."""
     with pytest.raises(ValueError, match=r"'unknown' is not in list"):
         tree.remove_column("unknown")
 
 
 def test_remove_column_invalid_index(tree):
-    "If the index specified doesn't exist, an error is raised"
+    """If the index specified doesn't exist, an error is raised."""
     with pytest.raises(IndexError, match=r"list assignment index out of range"):
         tree.remove_column(100)
 
 
 def test_remove_column_index(tree):
-    "A column can be removed by index"
+    """A column can be removed by index."""
 
     tree.remove_column(1)
 
     # The column was removed
     assert_action_performed_with(
         tree,
         "remove column",
         index=1,
     )
     assert tree.headings == ["Title"]
     assert tree.accessors == ["key"]
 
 
 def test_remove_column_negative_index(tree):
-    "A column can be removed by index"
+    """A column can be removed by index."""
 
     tree.remove_column(-2)
 
     # The column was removed
     assert_action_performed_with(
         tree,
         "remove column",
         index=0,
     )
     assert tree.headings == ["Value"]
     assert tree.accessors == ["value"]
 
 
 def test_remove_column_no_headings(tree):
-    "A column can be removed when there are no headings"
+    """A column can be removed when there are no headings."""
     tree = toga.Tree(
         headings=None,
         accessors=["primus", "secondus"],
     )
 
     tree.remove_column(1)
 
@@ -565,15 +566,15 @@
         index=1,
     )
     assert tree.headings is None
     assert tree.accessors == ["primus"]
 
 
 def test_deprecated_names(on_activate_handler):
-    "Deprecated names still work"
+    """Deprecated names still work."""
 
     # Can't specify both on_double_click and on_activate
     with pytest.raises(
         ValueError,
         match=r"Cannot specify both on_double_click and on_activate",
     ):
         toga.Tree(["First", "Second"], on_double_click=Mock(), on_activate=Mock())
```

### Comparing `toga-core-0.4.2/tests/widgets/test_webview.py` & `toga_core-0.4.3/tests/widgets/test_webview.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 import toga
 from toga.widgets.webview import JavaScriptResult
 from toga_dummy.utils import (
     assert_action_performed,
     assert_action_performed_with,
     attribute_value,
 )
+from toga_dummy.widgets.webview import WebView as DummyWebView
 
 
 @pytest.fixture
 def widget():
     return toga.WebView()
 
 
 def test_widget_created():
-    "A WebView can be created with minimal arguments"
+    """A WebView can be created with minimal arguments."""
     widget = toga.WebView()
 
     assert widget._impl.interface == widget
     assert_action_performed(widget, "create WebView")
 
     assert widget.url is None
     assert widget.user_agent == "Toga dummy backend"
     assert widget._on_webview_load._raw is None
 
 
 def test_create_with_values():
-    "A WebView can be created with initial values"
+    """A WebView can be created with initial values."""
     on_webview_load = Mock()
 
     widget = toga.WebView(
         url="https://beeware.org",
         user_agent="Custom agent",
         on_webview_load=on_webview_load,
     )
@@ -42,24 +43,48 @@
     assert_action_performed(widget, "create WebView")
 
     assert widget.url == "https://beeware.org"
     assert widget.user_agent == "Custom agent"
     assert widget.on_webview_load._raw == on_webview_load
 
 
+def test_webview_load_disabled(monkeypatch):
+    """If the backend doesn't support on_webview_load, a warning is raised."""
+    try:
+        # Temporarily set the feature attribute on the backend
+        DummyWebView.SUPPORTS_ON_WEBVIEW_LOAD = False
+
+        # Instantiate a new widget with a hobbled backend.
+        widget = toga.WebView()
+        handler = Mock()
+
+        # Setting the handler raises a warning
+        with pytest.warns(
+            toga.NotImplementedWarning,
+            match=r"\[Dummy\] Not implemented: WebView\.on_webview_load",
+        ):
+            widget.on_webview_load = handler
+
+        # But the handler is still installed
+        assert widget.on_webview_load._raw == handler
+    finally:
+        # Clear the feature attribute.
+        del DummyWebView.SUPPORTS_ON_WEBVIEW_LOAD
+
+
 @pytest.mark.parametrize(
     "url",
     [
         "http://example.com",
         "https://example.com",
         None,
     ],
 )
 def test_url(widget, url):
-    "The URL of a webview can be set"
+    """The URL of a webview can be set."""
     # Set up a load handler
     on_webview_load_handler = Mock()
     widget.on_webview_load = on_webview_load_handler
 
     widget.url = url
     assert widget.url == url
 
@@ -81,15 +106,15 @@
     [
         "http://example.com",
         "https://example.com",
         None,
     ],
 )
 async def test_load_url(widget, url):
-    "The URL of a webview can be loaded asynchronously"
+    """The URL of a webview can be loaded asynchronously."""
     # Set up a load handler
     on_webview_load_handler = Mock()
     widget.on_webview_load = on_webview_load_handler
 
     # An async task that simulates a page load after a delay
     async def delayed_page_load():
         await asyncio.sleep(0.1)
@@ -123,62 +148,63 @@
     "url",
     [
         "file:///Path/to/file",
         "gopher://example.com",
     ],
 )
 async def test_invalid_url(widget, url):
-    "URLs must start with https:// or http://"
+    """URLs must start with https:// or http://"""
     with pytest.raises(
         ValueError,
         match=r"WebView can only display http:// and https:// URLs",
     ):
         widget.url = url
 
     with pytest.raises(
         ValueError,
         match=r"WebView can only display http:// and https:// URLs",
     ):
         await widget.load_url(url)
 
 
 def test_set_content(widget):
-    "Static HTML content can be loaded into the page"
+    """Static HTML content can be loaded into the page."""
     widget.set_content("https://example.com", "<h1>Fancy page</h1>")
     assert_action_performed_with(
         widget,
         "set content",
         root_url="https://example.com",
         content="<h1>Fancy page</h1>",
     )
 
 
 def test_user_agent(widget):
-    "The user agent can be customized"
+    """The user agent can be customized."""
     widget.user_agent = "New user agent"
     assert widget.user_agent == "New user agent"
 
 
 def test_evaluate_javascript(widget):
-    "Javascript can be evaluated"
+    """Javascript can be evaluated."""
     result = widget.evaluate_javascript("test(1);")
     assert_action_performed(widget, "evaluate_javascript")
 
     assert isinstance(result, JavaScriptResult)
 
     # Attempting to use or compare the result raises an error
     with pytest.raises(
         RuntimeError,
         match=r"Can't check JavaScript result directly; use await or an on_result handler",
     ):
         result == 42
 
 
 async def test_evaluate_javascript_async(widget):
-    "Javascript can be evaluated asynchronously, and an asynchronous result returned"
+    """Javascript can be evaluated asynchronously, and an asynchronous result
+    returned."""
 
     # An async task that simulates evaluation of Javascript after a delay
     async def delayed_page_load():
         await asyncio.sleep(0.1)
 
         # Complete the Javascript
         widget._impl.simulate_javascript_result(42)
@@ -188,15 +214,15 @@
     result = await widget.evaluate_javascript("test(1);")
     assert_action_performed(widget, "evaluate_javascript")
 
     assert result == 42
 
 
 async def test_evaluate_javascript_sync(widget):
-    """Deprecated sync handlers can be used for Javascript evaluation"""
+    """Deprecated sync handlers can be used for Javascript evaluation."""
 
     # An async task that simulates evaluation of Javascript after a delay
     async def delayed_page_load():
         await asyncio.sleep(0.1)
 
         # Complete the Javascript
         widget._impl.simulate_javascript_result(42)
```

### Comparing `toga-core-0.4.2/tests/window/test_filtered_widget_registry.py` & `toga_core-0.4.3/tests/window/test_filtered_widget_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     win_2 = make_window("2")
 
     # the `magic` ID doesn't exist initially
     assert "magic" not in app.widgets
     assert "magic" not in win_1.widgets
     assert "magic" not in win_2.widgets
 
-    # Create a widget with the magic ID. The wiget still isn't in the registry, because
+    # Create a widget with the magic ID. The widget still isn't in the registry, because
     # it's not part of a window
     first = ExampleWidget(id="magic")
 
     assert "magic" not in app.widgets
     assert "magic" not in win_1.widgets
     assert "magic" not in win_2.widgets
```

