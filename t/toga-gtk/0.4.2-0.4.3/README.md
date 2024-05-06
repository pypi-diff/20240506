# Comparing `tmp/toga-gtk-0.4.2.tar.gz` & `tmp/toga_gtk-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-gtk-0.4.2.tar", last modified: Tue Feb  6 05:54:06 2024, max compression
+gzip compressed data, was "toga_gtk-0.4.3.tar", last modified: Mon May  6 06:43:35 2024, max compression
```

## Comparing `toga-gtk-0.4.2.tar` & `toga_gtk-0.4.3.tar`

### file list

```diff
@@ -1,99 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.908499 toga-gtk-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-06 05:54:06.908499 toga-gtk-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:54:06.908499 toga-gtk-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.892499 toga-gtk-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.896499 toga-gtk-0.4.2/src/toga_gtk/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.900499 toga-gtk-0.4.2/src/toga_gtk/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.900499 toga-gtk-0.4.2/src/toga_gtk/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/libs/fontconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/libs/gtk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/libs/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/libs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.900499 toga-gtk-0.4.2/src/toga_gtk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/resources/toga.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.904499 toga-gtk-0.4.2/src/toga_gtk/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/src/toga_gtk/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.908499 toga-gtk-0.4.2/src/toga_gtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-06 05:54:06.000000 toga-gtk-0.4.2/src/toga_gtk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.904499 toga-gtk-0.4.2/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:06.908499 toga-gtk-0.4.2/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-02-06 05:53:27.000000 toga-gtk-0.4.2/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.154737 toga_gtk-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.158737 toga_gtk-0.4.3/src/toga_gtk/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/fontconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/gtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.166737 toga_gtk-0.4.3/src/toga_gtk/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/src/toga_gtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.170737 toga_gtk-0.4.3/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/window.py
```

### Comparing `toga-gtk-0.4.2/LICENSE` & `toga_gtk-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/PKG-INFO` & `toga_gtk-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: toga-gtk
-Version: 0.4.2
+Version: 0.4.3
 Summary: A GTK backend for the Toga widget toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,linux,freeBSD,gtk
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
 Requires-Dist: gbulb>=0.5.3
 Requires-Dist: pycairo>=1.17.0
 Requires-Dist: pygobject>=3.46.0
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-gtk
 ========
 
 A GTK backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Linux platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/linux.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/linux.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-gtk-0.4.2/README.rst` & `toga_gtk-0.4.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ========
 
 A GTK backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Linux platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/linux.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/linux.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-gtk-0.4.2/pyproject.toml` & `toga_gtk-0.4.3/pyproject.toml`

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
@@ -36,26 +36,28 @@
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
 linux = "toga_gtk"
 freeBSD = "toga_gtk"
 
 [tool.setuptools_scm]
 root = ".."
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/app.py` & `toga_gtk-0.4.3/src/toga_gtk/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 import asyncio
+import os
 import signal
 import sys
 from pathlib import Path
 
 import gbulb
 
 import toga
 from toga import App as toga_App
 from toga.command import Command, Separator
 
 from .keys import gtk_accel
 from .libs import TOGA_DEFAULT_STYLES, Gdk, Gio, GLib, Gtk
+from .screens import Screen as ScreenImpl
 from .window import Window
 
 
 class MainWindow(Window):
     def create(self):
         self.native = Gtk.ApplicationWindow()
         self.native.set_role("MainWindow")
-        icon_impl = toga_App.app.icon._impl
-        self.native.set_icon(icon_impl.native_72)
 
     def gtk_delete_event(self, *args):
         # Return value of the GTK on_close handler indicates
         # whether the event has been fully handled. Returning
         # False indicates the event handling is *not* complete,
         # so further event processing (including actually
         # closing the window) should be performed; so
         # "should_exit == True" must be converted to a return
         # value of False.
         self.interface.app.on_exit()
         return True
 
 
 class App:
-    """
-    Todo:
-        * Creation of Menus is not working.
-        * Disabling of menu items is not working.
-        * App Icon is not showing up
-    """
-
     def __init__(self, interface):
         self.interface = interface
         self.interface._impl = self
 
         gbulb.install(gtk=True)
         self.loop = asyncio.new_event_loop()
 
@@ -60,33 +53,20 @@
 
         # Connect the GTK signal that will cause app startup to occur
         self.native.connect("startup", self.gtk_startup)
         self.native.connect("activate", self.gtk_activate)
 
         self.actions = None
 
+    def gtk_activate(self, data=None):
+        pass
+
     def gtk_startup(self, data=None):
         # Set up the default commands for the interface.
-        self.interface.commands.add(
-            Command(
-                self._menu_about,
-                "About " + self.interface.formal_name,
-                group=toga.Group.HELP,
-            ),
-            Command(None, "Preferences", group=toga.Group.APP),
-            # Quit should always be the last item, in a section on its own
-            Command(
-                self._menu_quit,
-                "Quit " + self.interface.formal_name,
-                shortcut=toga.Key.MOD_1 + "q",
-                group=toga.Group.APP,
-                section=sys.maxsize,
-            ),
-        )
-        self._create_app_commands()
+        self.create_app_commands()
 
         self.interface._startup()
 
         # Create the lookup table of menu items,
         # then force the creation of the menus.
         self.create_menus()
 
@@ -103,47 +83,81 @@
         css_provider.load_from_data(TOGA_DEFAULT_STYLES)
 
         context = Gtk.StyleContext()
         context.add_provider_for_screen(
             Gdk.Screen.get_default(), css_provider, Gtk.STYLE_PROVIDER_PRIORITY_USER
         )
 
-    def _create_app_commands(self):
-        # No extra menus
-        pass
-
-    def gtk_activate(self, data=None):
-        pass
+    ######################################################################
+    # Commands and menus
+    ######################################################################
 
     def _menu_about(self, command, **kwargs):
         self.interface.about()
 
     def _menu_quit(self, command, **kwargs):
         self.interface.on_exit()
 
+    def create_app_commands(self):
+        self.interface.commands.add(
+            Command(
+                self._menu_about,
+                "About " + self.interface.formal_name,
+                group=toga.Group.HELP,
+            ),
+            Command(None, "Preferences", group=toga.Group.APP),
+            # Quit should always be the last item, in a section on its own
+            Command(
+                self._menu_quit,
+                "Quit " + self.interface.formal_name,
+                shortcut=toga.Key.MOD_1 + "q",
+                group=toga.Group.APP,
+                section=sys.maxsize,
+            ),
+        )
+
+    def _submenu(self, group, menubar):
+        try:
+            submenu, section = self._menu_groups[group]
+        except KeyError:
+            # It's a new menu/group, so it must start a new section.
+            section = Gio.Menu()
+            if group is None:
+                # Menu is a top-level menu; so it's a child of the menu bar
+                submenu = menubar
+            else:
+                _, parent_section = self._submenu(group.parent, menubar)
+                submenu = Gio.Menu()
+
+                text = group.text
+                if text == "*":
+                    text = self.interface.formal_name
+                parent_section.append_submenu(text, submenu)
+
+            # Add the initial section to the submenu,
+            # and install the menu item in the group cache.
+            submenu.append_section(None, section)
+            self._menu_groups[group] = submenu, section
+
+        return submenu, section
+
     def create_menus(self):
         # Only create the menu if the menu item index has been created.
         self._menu_items = {}
         self._menu_groups = {}
 
         # Create the menu for the top level menubar.
         menubar = Gio.Menu()
-        section = None
         for cmd in self.interface.commands:
+            submenu, section = self._submenu(cmd.group, menubar)
             if isinstance(cmd, Separator):
-                section = None
+                section = Gio.Menu()
+                submenu.append_section(None, section)
+                self._menu_groups[cmd.group] = (submenu, section)
             else:
-                submenu, created = self._submenu(cmd.group, menubar)
-                if created:
-                    section = None
-
-                if section is None:
-                    section = Gio.Menu()
-                    submenu.append_section(None, section)
-
                 cmd_id = "command-%s" % id(cmd)
                 action = Gio.SimpleAction.new(cmd_id, None)
                 action.connect("activate", cmd._impl.gtk_activate)
 
                 cmd._impl.native.append(action)
                 cmd._impl.set_enabled(cmd.enabled)
                 self._menu_items[action] = cmd
@@ -156,99 +170,124 @@
                     )
 
                 section.append_item(item)
 
         # Set the menu for the app.
         self.native.set_menubar(menubar)
 
-    def _submenu(self, group, menubar):
-        try:
-            return self._menu_groups[group], False
-        except KeyError:
-            if group is None:
-                submenu = menubar
-            else:
-                parent_menu, _ = self._submenu(group.parent, menubar)
-                submenu = Gio.Menu()
-                self._menu_groups[group] = submenu
+    ######################################################################
+    # App lifecycle
+    ######################################################################
 
-                text = group.text
-                if text == "*":
-                    text = self.interface.formal_name
-                parent_menu.append_submenu(text, submenu)
-
-            # Install the item in the group cache.
-            self._menu_groups[group] = submenu
-
-            return submenu, True
+    # We can't call this under test conditions, because it would kill the test harness
+    def exit(self):  # pragma: no cover
+        self.native.quit()
 
     def main_loop(self):
         # Modify signal handlers to make sure Ctrl-C is caught and handled.
         signal.signal(signal.SIGINT, signal.SIG_DFL)
 
         self.loop.run_forever(application=self.native)
 
+    def set_icon(self, icon):
+        for window in self.interface.windows:
+            window._impl.native.set_icon(icon._impl.native(72))
+
     def set_main_window(self, window):
         pass
 
+    ######################################################################
+    # App resources
+    ######################################################################
+
+    def get_screens(self):
+        display = Gdk.Display.get_default()
+        if "WAYLAND_DISPLAY" in os.environ:  # pragma: no cover
+            # `get_primary_monitor()` doesn't work on wayland, so return as it is.
+            return [
+                ScreenImpl(native=display.get_monitor(i))
+                for i in range(display.get_n_monitors())
+            ]
+        else:
+            primary_screen = ScreenImpl(display.get_primary_monitor())
+            screen_list = [primary_screen] + [
+                ScreenImpl(native=display.get_monitor(i))
+                for i in range(display.get_n_monitors())
+                if display.get_monitor(i) != primary_screen.native
+            ]
+            return screen_list
+
+    ######################################################################
+    # App capabilities
+    ######################################################################
+
+    def beep(self):
+        Gdk.beep()
+
+    def _close_about(self, dialog):
+        self.native_about_dialog.destroy()
+        self.native_about_dialog = None
+
     def show_about_dialog(self):
         self.native_about_dialog = Gtk.AboutDialog()
         self.native_about_dialog.set_modal(True)
 
         icon_impl = toga_App.app.icon._impl
-        self.native_about_dialog.set_logo(icon_impl.native_72)
+        self.native_about_dialog.set_logo(icon_impl.native(72))
 
         self.native_about_dialog.set_program_name(self.interface.formal_name)
         if self.interface.version is not None:
             self.native_about_dialog.set_version(self.interface.version)
         if self.interface.author is not None:
             self.native_about_dialog.set_authors([self.interface.author])
         if self.interface.description is not None:
             self.native_about_dialog.set_comments(self.interface.description)
         if self.interface.home_page is not None:
             self.native_about_dialog.set_website(self.interface.home_page)
 
         self.native_about_dialog.show()
         self.native_about_dialog.connect("close", self._close_about)
 
-    def _close_about(self, dialog):
-        self.native_about_dialog.destroy()
-        self.native_about_dialog = None
+    ######################################################################
+    # Cursor control
+    ######################################################################
 
-    def beep(self):
-        Gdk.beep()
+    def hide_cursor(self):
+        self.interface.factory.not_implemented("App.hide_cursor()")
 
-    # We can't call this under test conditions, because it would kill the test harness
-    def exit(self):  # pragma: no cover
-        self.native.quit()
+    def show_cursor(self):
+        self.interface.factory.not_implemented("App.show_cursor()")
+
+    ######################################################################
+    # Window control
+    ######################################################################
 
     def get_current_window(self):
         current_window = self.native.get_active_window()._impl
         return current_window if current_window.interface.visible else None
 
     def set_current_window(self, window):
         window._impl.native.present()
 
+    ######################################################################
+    # Full screen control
+    ######################################################################
+
     def enter_full_screen(self, windows):
         for window in windows:
             window._impl.set_full_screen(True)
 
     def exit_full_screen(self, windows):
         for window in windows:
             window._impl.set_full_screen(False)
 
-    def show_cursor(self):
-        self.interface.factory.not_implemented("App.show_cursor()")
-
-    def hide_cursor(self):
-        self.interface.factory.not_implemented("App.hide_cursor()")
-
 
 class DocumentApp(App):  # pragma: no cover
-    def _create_app_commands(self):
+    def create_app_commands(self):
+        super().create_app_commands()
         self.interface.commands.add(
             toga.Command(
                 self.open_file,
                 text="Open...",
                 shortcut=toga.Key.MOD_1 + "o",
                 group=toga.Group.FILE,
                 section=0,
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/command.py` & `toga_gtk-0.4.3/src/toga_gtk/command.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/container.py` & `toga_gtk-0.4.3/src/toga_gtk/container.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/dialogs.py` & `toga_gtk-0.4.3/src/toga_gtk/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/factory.py` & `toga_gtk-0.4.3/src/toga_gtk/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from toga import NotImplementedWarning
+
 from . import dialogs
 from .app import App, DocumentApp, MainWindow
 from .command import Command
 from .documents import Document
 from .fonts import Font
 from .icons import Icon
 from .images import Image
@@ -10,14 +12,15 @@
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
@@ -28,15 +31,15 @@
 from .widgets.textinput import TextInput
 from .widgets.tree import Tree
 from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    print(f"[GTK+] Not implemented: {feature}")  # pragma: nocover
+    NotImplementedWarning.warn("GTK", feature)
 
 
 __all__ = [
     "not_implemented",
     "App",
     "DocumentApp",
     "MainWindow",
@@ -53,14 +56,15 @@
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

### Comparing `toga-gtk-0.4.2/src/toga_gtk/fonts.py` & `toga_gtk-0.4.3/src/toga_gtk/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/images.py` & `toga_gtk-0.4.3/src/toga_gtk/images.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/libs/fontconfig.py` & `toga_gtk-0.4.3/src/toga_gtk/libs/fontconfig.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/libs/gtk.py` & `toga_gtk-0.4.3/src/toga_gtk/libs/gtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,18 @@
         "Cannot identify an active display. Is the `DISPLAY` environment variable set correctly?"
     )
 
 # The following imports will fail if the underlying libraries or their API
 # wrappers aren't installed; handle failure gracefully (see
 # https://github.com/beeware/toga/issues/26)
 try:
-    gi.require_version("WebKit2", "4.0")
+    try:
+        gi.require_version("WebKit2", "4.1")
+    except ValueError:  # pragma: no cover
+        gi.require_version("WebKit2", "4.0")
     from gi.repository import WebKit2  # noqa: F401
 except (ImportError, ValueError):  # pragma: no cover
     WebKit2 = None
 
 try:
     gi.require_version("Pango", "1.0")
     from gi.repository import Pango  # noqa: F401
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/libs/styles.py` & `toga_gtk-0.4.3/src/toga_gtk/libs/styles.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/resources/toga.png` & `toga_gtk-0.4.3/src/toga_gtk/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/activityindicator.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/base.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/button.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def get_icon(self):
         return self._icon
 
     def set_icon(self, icon):
         self._icon = icon
         if icon:
-            self.native.set_image(Gtk.Image.new_from_pixbuf(icon._impl.native_32))
+            self.native.set_image(Gtk.Image.new_from_pixbuf(icon._impl.native(32)))
             self.native.set_always_show_image(True)
         else:
             self.native.set_image(None)
             self.native.set_always_show_image(False)
 
     def set_enabled(self, value):
         self.native.set_sensitive(value)
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/canvas.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/detailedlist.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/detailedlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.text.set_markup(markup)
 
         # Update the icon
         if self.icon:
             self.content.remove(self.icon)
 
         try:
-            pixbuf = getattr(self.row, dl.accessors[2])._impl.native_32
+            pixbuf = getattr(self.row, dl.accessors[2])._impl.native(32)
         except AttributeError:
             pixbuf = None
 
         if pixbuf is not None:
             self.icon = Gtk.Image.new_from_pixbuf(pixbuf)
             self.content.pack_start(self.icon, False, False, 6)
         else:
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/divider.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/imageview.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/label.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/multilinetextinput.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/numberinput.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/optioncontainer.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/progressbar.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/scrollcontainer.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/selection.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/slider.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/splitcontainer.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/switch.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/table.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         super().__init__()
         self.value = value
 
     def icon(self, attr):
         data = getattr(self.value, attr, None)
         if isinstance(data, tuple):
             if data[0] is not None:
-                return data[0]._impl.native_16
+                return data[0]._impl.native(16)
             return None
         else:
             try:
-                return data.icon._impl.native_16
+                return data.icon._impl.native(16)
             except AttributeError:
                 return None
 
     def text(self, attr, missing_value):
         data = getattr(self.value, attr, None)
         if isinstance(data, toga.Widget):
             warnings.warn("GTK does not support the use of widgets in cells")
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/textinput.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/tree.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/src/toga_gtk/widgets/webview.py` & `toga_gtk-0.4.3/src/toga_gtk/widgets/webview.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 class WebView(Widget):
     """GTK WebView implementation."""
 
     def create(self):
         if WebKit2 is None:  # pragma: no cover
             raise RuntimeError(
                 "Unable to import WebKit2. Ensure that the system package "
-                "providing Webkit2 and its GTK bindings have been installed."
+                "providing WebKit2 and its GTK bindings have been installed. "
+                "See https://toga.readthedocs.io/en/stable/reference/api/widgets/webview.html#system-requirements "
+                "for details."
             )
 
         self.native = WebKit2.WebView()
 
         settings = self.native.get_settings()
         settings.set_property("enable-developer-extras", True)
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk/window.py` & `toga_gtk-0.4.3/src/toga_gtk/window.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from toga.command import Separator
 
 from .container import TogaContainer
 from .libs import Gdk, Gtk
+from .screens import Screen as ScreenImpl
 
 
 class Window:
     def __init__(self, interface, title, position, size):
         self.interface = interface
         self.interface._impl = self
 
@@ -48,22 +49,48 @@
         self.layout.pack_end(self.container, expand=True, fill=True, padding=0)
 
         self.native.add(self.layout)
 
     def create(self):
         self.native = Gtk.Window()
 
+    ######################################################################
+    # Native event handlers
+    ######################################################################
+
+    def gtk_delete_event(self, widget, data):
+        if self._is_closing:
+            should_close = True
+        else:
+            should_close = self.interface.on_close()
+
+        # Return value of the GTK on_close handler indicates
+        # whether the event has been fully handled. Returning
+        # False indicates the event handling is *not* complete,
+        # so further event processing (including actually
+        # closing the window) should be performed.
+        return not should_close
+
+    ######################################################################
+    # Window properties
+    ######################################################################
+
     def get_title(self):
         return self.native.get_title()
 
     def set_title(self, title):
         self.native.set_title(title)
 
-    def set_app(self, app):
-        app.native.add_window(self.native)
+    ######################################################################
+    # Window lifecycle
+    ######################################################################
+
+    def close(self):
+        self._is_closing = True
+        self.native.close()
 
     def create_toolbar(self):
         # If there's an existing toolbar, hide it until we know we need it.
         if self.toolbar_items:
             self.native_toolbar.set_visible(False)
 
         # Deregister any toolbar buttons from their commands, and remove them from the toolbar
@@ -94,79 +121,95 @@
                     prev_group = None
                 else:
                     prev_group = cmd.group
 
                 item_impl = Gtk.ToolButton()
                 if cmd.icon:
                     item_impl.set_icon_widget(
-                        Gtk.Image.new_from_pixbuf(cmd.icon._impl.native_32)
+                        Gtk.Image.new_from_pixbuf(cmd.icon._impl.native(32))
                     )
                 item_impl.set_label(cmd.text)
                 if cmd.tooltip:
                     item_impl.set_tooltip_text(cmd.tooltip)
                 item_impl.connect("clicked", cmd._impl.gtk_clicked)
                 cmd._impl.native.append(item_impl)
                 self.toolbar_items[cmd] = item_impl
 
             self.native_toolbar.insert(item_impl, -1)
 
         if self.toolbar_items:
             self.native_toolbar.set_visible(True)
             self.native_toolbar.show_all()
 
-    def set_content(self, widget):
-        # Set the new widget to be the container's content
-        self.container.content = widget
+    def set_app(self, app):
+        app.native.add_window(self.native)
+        self.native.set_icon(app.interface.icon._impl.native(72))
 
     def show(self):
         self.native.show_all()
 
-    def hide(self):
-        self.native.hide()
+    ######################################################################
+    # Window content and resources
+    ######################################################################
 
-    def get_visible(self):
-        return self.native.get_property("visible")
+    def set_content(self, widget):
+        # Set the new widget to be the container's content
+        self.container.content = widget
 
-    def gtk_delete_event(self, widget, data):
-        if self._is_closing:
-            should_close = True
-        else:
-            should_close = self.interface.on_close()
+    ######################################################################
+    # Window size
+    ######################################################################
 
-        # Return value of the GTK on_close handler indicates
-        # whether the event has been fully handled. Returning
-        # False indicates the event handling is *not* complete,
-        # so further event processing (including actually
-        # closing the window) should be performed.
-        return not should_close
+    def get_size(self):
+        size = self.native.get_size()
+        return size.width, size.height
 
-    def close(self):
-        self._is_closing = True
-        self.native.close()
+    def set_size(self, size):
+        self.native.resize(size[0], size[1])
+
+    ######################################################################
+    # Window position
+    ######################################################################
+
+    def get_current_screen(self):
+        display = Gdk.Display.get_default()
+        monitor_native = display.get_monitor_at_window(self.native.get_window())
+        return ScreenImpl(monitor_native)
 
     def get_position(self):
         pos = self.native.get_position()
         return pos.root_x, pos.root_y
 
     def set_position(self, position):
         self.native.move(position[0], position[1])
 
-    def get_size(self):
-        size = self.native.get_size()
-        return size.width, size.height
+    ######################################################################
+    # Window visibility
+    ######################################################################
 
-    def set_size(self, size):
-        self.native.resize(size[0], size[1])
+    def get_visible(self):
+        return self.native.get_property("visible")
+
+    def hide(self):
+        self.native.hide()
+
+    ######################################################################
+    # Window state
+    ######################################################################
 
     def set_full_screen(self, is_full_screen):
         if is_full_screen:
             self.native.fullscreen()
         else:
             self.native.unfullscreen()
 
+    ######################################################################
+    # Window capabilities
+    ######################################################################
+
     def get_image_data(self):
         display = self.native.get_display()
         display.flush()
 
         # For some reason, converting the *window* to a pixbuf fails. But if you extract
         # a *part* of the overall screen, that works. So - work out the origin of the
         # window, then the allocation for the container relative to that window, and
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk.egg-info/PKG-INFO` & `toga_gtk-0.4.3/src/toga_gtk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: toga-gtk
-Version: 0.4.2
+Version: 0.4.3
 Summary: A GTK backend for the Toga widget toolkit.
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
 Keywords: gui,widget,cross-platform,toga,desktop,linux,freeBSD,gtk
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
 Requires-Dist: gbulb>=0.5.3
 Requires-Dist: pycairo>=1.17.0
 Requires-Dist: pygobject>=3.46.0
-Requires-Dist: toga-core==0.4.2
+Requires-Dist: toga-core==0.4.3
 
 toga-gtk
 ========
 
 A GTK backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For platform requirements, see the `Linux platform documentation
-<https://toga.readthedocs.io/en/stable/reference/platforms/linux.html#prerequisites>`__.
+<https://toga.readthedocs.io/en/latest/reference/platforms/linux.html#prerequisites>`__.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _the core Toga library: https://pypi.python.org/pypi/toga-core
 .. _Toga project on Github: https://github.com/beeware/toga
```

### Comparing `toga-gtk-0.4.2/src/toga_gtk.egg-info/SOURCES.txt` & `toga_gtk-0.4.3/src/toga_gtk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/toga_gtk/documents.py
 src/toga_gtk/factory.py
 src/toga_gtk/fonts.py
 src/toga_gtk/icons.py
 src/toga_gtk/images.py
 src/toga_gtk/keys.py
 src/toga_gtk/paths.py
+src/toga_gtk/screens.py
 src/toga_gtk/window.py
 src/toga_gtk.egg-info/PKG-INFO
 src/toga_gtk.egg-info/SOURCES.txt
 src/toga_gtk.egg-info/dependency_links.txt
 src/toga_gtk.egg-info/entry_points.txt
 src/toga_gtk.egg-info/requires.txt
 src/toga_gtk.egg-info/top_level.txt
@@ -35,14 +36,15 @@
 src/toga_gtk/widgets/box.py
 src/toga_gtk/widgets/button.py
 src/toga_gtk/widgets/canvas.py
 src/toga_gtk/widgets/detailedlist.py
 src/toga_gtk/widgets/divider.py
 src/toga_gtk/widgets/imageview.py
 src/toga_gtk/widgets/label.py
+src/toga_gtk/widgets/mapview.py
 src/toga_gtk/widgets/multilinetextinput.py
 src/toga_gtk/widgets/numberinput.py
 src/toga_gtk/widgets/optioncontainer.py
 src/toga_gtk/widgets/passwordinput.py
 src/toga_gtk/widgets/progressbar.py
 src/toga_gtk/widgets/scrollcontainer.py
 src/toga_gtk/widgets/selection.py
@@ -55,25 +57,27 @@
 src/toga_gtk/widgets/webview.py
 tests_backend/__init__.py
 tests_backend/app.py
 tests_backend/fonts.py
 tests_backend/icons.py
 tests_backend/images.py
 tests_backend/probe.py
+tests_backend/screens.py
 tests_backend/window.py
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

### Comparing `toga-gtk-0.4.2/tests_backend/fonts.py` & `toga_gtk-0.4.3/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/probe.py` & `toga_gtk-0.4.3/tests_backend/probe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
 
+import toga
 from toga_gtk.libs import Gtk
 
 
 class BaseProbe:
     def repaint_needed(self):
         return Gtk.events_pending()
 
-    async def redraw(self, message=None, delay=None):
+    async def redraw(self, message=None, delay=0):
         """Request a redraw of the app, waiting until that redraw has completed."""
         # Force a repaint
         while self.repaint_needed():
             Gtk.main_iteration_do(blocking=False)
 
         # If we're running slow, wait for a second
-        if self.app.run_slow:
-            print("Waiting for redraw" if message is None else message)
-            delay = 1
+        if toga.App.app.run_slow:
+            delay = max(1, delay)
 
         if delay:
+            print("Waiting for redraw" if message is None else message)
             await asyncio.sleep(delay)
 
-    def assert_image_size(self, image_size, size):
+    def assert_image_size(self, image_size, size, screen):
         assert image_size == size
```

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/base.py` & `toga_gtk-0.4.3/tests_backend/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/button.py` & `toga_gtk-0.4.3/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/canvas.py` & `toga_gtk-0.4.3/tests_backend/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/detailedlist.py` & `toga_gtk-0.4.3/tests_backend/widgets/detailedlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         assert (
             str(row.text.get_label())
             == f"{html.escape(title)}\n<small>{html.escape(subtitle)}</small>"
         )
 
         if icon:
-            assert row.icon.get_pixbuf() == icon._impl.native_32
+            assert row.icon.get_pixbuf() == icon._impl.native(32)
         else:
             assert row.icon is None
 
     @property
     def max_scroll_position(self):
         return int(self.native_vadj.get_upper() - self.native_vadj.get_page_size())
```

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/label.py` & `toga_gtk-0.4.3/tests_backend/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/multilinetextinput.py` & `toga_gtk-0.4.3/tests_backend/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/numberinput.py` & `toga_gtk-0.4.3/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/optioncontainer.py` & `toga_gtk-0.4.3/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/progressbar.py` & `toga_gtk-0.4.3/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/properties.py` & `toga_gtk-0.4.3/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/scrollcontainer.py` & `toga_gtk-0.4.3/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/selection.py` & `toga_gtk-0.4.3/tests_backend/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/slider.py` & `toga_gtk-0.4.3/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/splitcontainer.py` & `toga_gtk-0.4.3/tests_backend/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/switch.py` & `toga_gtk-0.4.3/tests_backend/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/table.py` & `toga_gtk-0.4.3/tests_backend/widgets/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if widget:
             pytest.skip("GTK doesn't support widgets in Tables")
         else:
             gtk_row = self.native_table.get_model()[row]
             assert gtk_row[col * 2 + 2]
 
             if icon:
-                assert gtk_row[col * 2 + 1] == icon._impl.native_16
+                assert gtk_row[col * 2 + 1] == icon._impl.native(16)
             else:
                 assert gtk_row[col * 2 + 1] is None
 
     @property
     def max_scroll_position(self):
         return int(
             self.native.get_vadjustment().get_upper()
```

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/textinput.py` & `toga_gtk-0.4.3/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga-gtk-0.4.2/tests_backend/widgets/tree.py` & `toga_gtk-0.4.3/tests_backend/widgets/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if widget:
             pytest.skip("GTK doesn't support widgets in Tables")
         else:
             gtk_row = self.native_tree.get_model()[row_path]
             assert gtk_row[col * 2 + 2]
 
             if icon:
-                assert gtk_row[col * 2 + 1] == icon._impl.native_16
+                assert gtk_row[col * 2 + 1] == icon._impl.native(16)
             else:
                 assert gtk_row[col * 2 + 1] is None
 
     @property
     def max_scroll_position(self):
         return int(
             self.native.get_vadjustment().get_upper()
```

### Comparing `toga-gtk-0.4.2/tests_backend/window.py` & `toga_gtk-0.4.3/tests_backend/window.py`

 * *Files identical despite different names*

