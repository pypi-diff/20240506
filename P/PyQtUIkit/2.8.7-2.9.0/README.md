# Comparing `tmp/PyQtUIkit-2.8.7.tar.gz` & `tmp/PyQtUIkit-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.8.7.tar", last modified: Fri May  3 13:25:53 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.9.0.tar", last modified: Sun May  5 20:58:00 2024, max compression
```

## Comparing `PyQtUIkit-2.8.7.tar` & `PyQtUIkit-2.9.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.354953 PyQtUIkit-2.8.7/
--rw-rw-rw-   0        0        0     1090 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-05-03 13:25:53.354953 PyQtUIkit-2.8.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.308081 PyQtUIkit-2.8.7/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3417 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3271 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.323700 PyQtUIkit-2.8.7/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.323700 PyQtUIkit-2.8.7/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.339321 PyQtUIkit-2.8.7/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.339321 PyQtUIkit-2.8.7/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     4222 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1810582 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1830 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.354953 PyQtUIkit-2.8.7/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1734 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1367 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     8034 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2794 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11424 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5876 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     4350 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/grid_layout.py
--rw-rw-rw-   0        0        0     2280 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5436 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4948 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7471 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6805 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    14123 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1313 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/tabs_layout.py
--rw-rw-rw-   0        0        0     4538 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17878 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:25:53.308081 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 13:25:53.000000 PyQtUIkit-2.8.7/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 13:25:53.354953 PyQtUIkit-2.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-05-03 13:24:01.000000 PyQtUIkit-2.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3417 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.490498 PyQtUIkit-2.9.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.506125 PyQtUIkit-2.9.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.506125 PyQtUIkit-2.9.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4314 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     6433 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1810582 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0    10274 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/languages.py
+-rw-rw-rw-   0        0        0     1830 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1807 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1818 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1367 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_application.py
+-rw-rw-rw-   0        0        0     8034 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_button.py
+-rw-rw-rw-   0        0        0     2795 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_checkbox.py
+-rw-rw-rw-   0        0        0    11428 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_combo_box.py
+-rw-rw-rw-   0        0        0     8329 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_form.py
+-rw-rw-rw-   0        0        0     4350 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_group.py
+-rw-rw-rw-   0        0        0     1578 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_label.py
+-rw-rw-rw-   0        0        0     5436 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_layout.py
+-rw-rw-rw-   0        0        0     1697 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu.py
+-rw-rw-rw-   0        0        0     4948 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu_bar.py
+-rw-rw-rw-   0        0        0     7471 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_radio.py
+-rw-rw-rw-   0        0        0     4568 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scintilla.py
+-rw-rw-rw-   0        0        0     4021 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_separator.py
+-rw-rw-rw-   0        0        0     7515 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spinner.py
+-rw-rw-rw-   0        0        0    14128 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tab_bar.py
+-rw-rw-rw-   0        0        0     1313 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_text_edit.py
+-rw-rw-rw-   0        0        0     4466 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_toggle.py
+-rw-rw-rw-   0        0        0    17885 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tree_widget.py
+-rw-rw-rw-   0        0        0     3304 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2707 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/setup.py
```

### Comparing `PyQtUIkit-2.8.7/LICENSE` & `PyQtUIkit-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PKG-INFO` & `PyQtUIkit-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.7
+Version: 2.9.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/_icons.py` & `PyQtUIkit-2.9.0/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/_translate.py` & `PyQtUIkit-2.9.0/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.9.0/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/core/font.py` & `PyQtUIkit-2.9.0/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.9.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.9.0/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
     def _set_active(self):
         self.__active = KitTheme
 
     def palette(self, key: str):
         return self.__current_theme.palette(key)
 
+    def code_color(self, key: str):
+        return self.__current_theme.code_color(key)
+
     def font(self, font):
         return self.__current_theme.font(font)
 
     def border(self):
         return self.__current_theme.border()
 
     def pixmap(self, name, color, size=None):
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/builtin_themes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,56 @@
+from PyQt6.QtGui import QColor
+
 from PyQtUIkit.core.font import KitFont
 from PyQtUIkit.themes.theme import KitTheme, KitPalette
 
-basic_theme = KitTheme({
+basic_theme = KitTheme(palettes={
     'Transparent': KitPalette('#00000000', '#30000000', '#60000000', '#222222'),
 
     'Main': KitPalette('#FFFFFF', '#DFE1E5', '#CFDEFC', '#222222'),
     'Bg': KitPalette('#ECF5F9', '#CBCDCF', '#5283C9', '#222222'),
     'Menu': KitPalette('#C4CBCF', '#9DA3A6', '#3B81F0', '#222222'),
     'Border': KitPalette('#BFC0C2', '#A6A7A8', '#52AFDE', '#222222'),
     'Success': KitPalette('#B3D635', '#D0FA3E', '#41D431', '#222222', '#2A8018'),
     'Warning': KitPalette('#E3C920', '#CFB71D', '#C7891E', '#222222', '#AB8618'),
     'Danger': KitPalette('#E33838', '#FC3E3E', '#FC1414', '#222222', '#B51702'),
-}, {
+}, fonts={
     'default': KitFont('Roboto', 9, 10, 14, 20),
     'italic': KitFont('Roboto', 9, 10, 14, 20, italic=True),
     'bold': KitFont('Roboto', 9, 10, 14, 20, bold=True),
     'strike': KitFont('Roboto', 9, 10, 14, 20, strike=True),
     'mono': KitFont('Roboto Mono', 9, 10, 14, 20)
+}, code_colors={
+    'Identifier': QColor('#101010'),
+    'Preprocessor': QColor('#997509'),
+    'Comment': QColor('#B0B0B0'),
+    'Keyword': QColor('#0057D5'),
+    'Number': QColor('#0057D5'),
+    'String': QColor('#18822C'),
 },
     is_dark=False)
 
 builtin_themes = {
     'Light': basic_theme,
-    'Dark': KitTheme({
+    'Dark': KitTheme(palettes={
         'Transparent': KitPalette('#00FFFFFF', '#30FFFFFF', '#60FFFFFF', '#F0F0F0'),
         'Main': KitPalette('#2B2D30', '#3E4145', '#2E436E', '#F0F0F0'),
         'Bg': KitPalette('#141517', '#222345', '#323466', '#F0F0F0'),
         'Menu': KitPalette('#1F2024', '#4E5157', '#3573F0', '#F0F0F0'),
         'Border': KitPalette('#474747', '#595959', '#2D63CC', '#F0F0F0'),
         'Success': KitPalette('#214514', '#295419', '#397523', '#F0F0F0', '#2A8018'),
         'Warning': KitPalette('#B8901A', '#A17E17', '#8C6E14', '#F0F0F0', '#D9AA1F'),
         'Danger': KitPalette('#690B0B', '#7A0D0D', '#B31414', '#F0F0F0', '#FA2A08'),
+    }, code_colors={
+        'Identifier': QColor('#DFDFDF'),
+        'Preprocessor': QColor('#56A8F5'),
+        'Comment': QColor('#74797B'),
+        'Keyword': QColor('#CC7832'),
+        'Number': QColor('#5191A6'),
+        'String': QColor('#5F864C'),
     },
         inherit=basic_theme,
         is_dark=True),
 
     'Orange': KitTheme({
         'Transparent': KitPalette('#00FFFFFF', '#30FFFFFF', '#60FFFFFF', '#000000'),
         'Main': KitPalette('#F2D7AD', '#F2CE9C', '#FFCB99', '#000000'),
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.9.0/PyQtUIkit/themes/theme.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from PyQt6.QtGui import QColor
+
 from PyQtUIkit.core.font import KitFont
 
 
 class KitPalette:
     def __init__(self, main, hover=None, selected=None, text=None, text_only=None):
         self.main = main
         self.hover = hover or main
@@ -13,27 +15,36 @@
         return f"KitPalette({self.main}, {self.hover}, {self.selected}, {self.text}, {self.text_only})"
 
 
 class KitTheme:
     def __init__(self,
                  palettes: dict[str: KitPalette] = None,
                  fonts: dict[str: KitFont] = None,
+                 code_colors: dict[str, QColor] = None,
                  inherit: 'KitTheme' = None,
                  is_dark=False):
         self.is_dark = is_dark
         self._palettes = palettes
         self._fonts = fonts
+        self._code_colors = code_colors
         self._inherit = inherit
 
     def palette(self, key: str):
         if self._palettes and key in self._palettes:
             return self._palettes[key]
         if not self._inherit:
             raise KeyError(f"Key '{key}' not found")
         return self._inherit.palette(key)
 
+    def code_color(self, key: str):
+        if self._code_colors and key in self._code_colors:
+            return self._code_colors[key]
+        if not self._inherit:
+            raise KeyError(f"Key '{key}' not found")
+        return self._inherit.code_color(key)
+
     def font(self, key='default') -> KitFont:
         if self._fonts and key in self._fonts:
             return self._fonts[key]
         if not self._inherit:
             raise KeyError(f"Key '{key}' not found")
         return self._inherit.font(key)
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from PyQtUIkit.widgets.layout import KitHBoxLayout, KitVBoxLayout
-from PyQtUIkit.widgets.flow_layout import KitFlowLayout
-from PyQtUIkit.widgets.label import KitLabel
-from PyQtUIkit.widgets.icon_widget import KitIconWidget
-from PyQtUIkit.widgets.button import KitButton, KitIconButton, KitLayoutButton
-from PyQtUIkit.widgets.line_edit import KitLineEdit
-from PyQtUIkit.widgets.list_widget import KitListWidget, KitListWidgetItem
-from PyQtUIkit.widgets.main_window import KitMainWindow
-from PyQtUIkit.widgets.spin_box import KitSpinBox
-from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.combo_box import KitComboBox, KitComboBoxItem, KitLanguageBox
-from PyQtUIkit.widgets.checkbox import KitCheckBox
-from PyQtUIkit.widgets.toggle import KitToggle
-from PyQtUIkit.widgets.tab_bar import KitTabBar, KitTab
-from PyQtUIkit.widgets.spinner import KitSpinner
-from PyQtUIkit.widgets.progress_bar import KitProgressBar
-from PyQtUIkit.widgets.tree_widget import KitTreeWidget, KitTreeWidgetItem
-from PyQtUIkit.widgets.menu import KitMenu
-from PyQtUIkit.widgets.group import KitHGroup, KitVGroup
-from PyQtUIkit.widgets.navigation import KitNavigation
-from PyQtUIkit.widgets.radio import KitVRadio, KitHRadio
-from PyQtUIkit.widgets.tabs_layout import KitTabLayout
-from PyQtUIkit.widgets.text_edit import KitTextEdit, KitTextBrowser
-from PyQtUIkit.widgets.form import KitForm
-from PyQtUIkit.widgets.dialog import KitDialog, KitFormDialog
-from PyQtUIkit.widgets.application import KitApplication, KitAsyncApplication
-from PyQtUIkit.widgets.separator import KitHSeparator, KitVSeparator
-from PyQtUIkit.widgets.menu_bar import KitMenuBar
-from PyQtUIkit.widgets.grid_layout import KitGridLayout
+from PyQtUIkit.widgets._layout import KitHBoxLayout, KitVBoxLayout
+from PyQtUIkit.widgets._flow_layout import KitFlowLayout
+from PyQtUIkit.widgets._label import KitLabel
+from PyQtUIkit.widgets._icon_widget import KitIconWidget
+from PyQtUIkit.widgets._button import KitButton, KitIconButton, KitLayoutButton
+from PyQtUIkit.widgets._line_edit import KitLineEdit
+from PyQtUIkit.widgets._list_widget import KitListWidget, KitListWidgetItem
+from PyQtUIkit.widgets._main_window import KitMainWindow
+from PyQtUIkit.widgets._spin_box import KitSpinBox
+from PyQtUIkit.widgets._scroll_area import KitScrollArea
+from PyQtUIkit.widgets._combo_box import KitComboBox, KitComboBoxItem, KitLanguageBox
+from PyQtUIkit.widgets._checkbox import KitCheckBox
+from PyQtUIkit.widgets._toggle import KitToggle
+from PyQtUIkit.widgets._tab_bar import KitTabBar, KitTab
+from PyQtUIkit.widgets._spinner import KitSpinner
+from PyQtUIkit.widgets._progress_bar import KitProgressBar
+from PyQtUIkit.widgets._tree_widget import KitTreeWidget, KitTreeWidgetItem
+from PyQtUIkit.widgets._menu import KitMenu
+from PyQtUIkit.widgets._group import KitHGroup, KitVGroup
+from PyQtUIkit.widgets._navigation import KitNavigation
+from PyQtUIkit.widgets._radio import KitVRadio, KitHRadio
+from PyQtUIkit.widgets._tabs_layout import KitTabLayout
+from PyQtUIkit.widgets._text_edit import KitTextEdit, KitTextBrowser
+from PyQtUIkit.widgets._form import KitForm
+from PyQtUIkit.widgets._dialog import KitDialog, KitFormDialog
+from PyQtUIkit.widgets._application import KitApplication, KitAsyncApplication
+from PyQtUIkit.widgets._separator import KitHSeparator, KitVSeparator
+from PyQtUIkit.widgets._menu_bar import KitMenuBar
+from PyQtUIkit.widgets._grid_layout import KitGridLayout
+from PyQtUIkit.widgets._scintilla import KitScintilla
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_checkbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QPushButton, QSizePolicy
 
 from PyQtUIkit.core import *
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
-from PyQtUIkit.widgets.button import KitIconButton
+from PyQtUIkit.widgets._button import KitIconButton
 
 
 class KitCheckBox(QWidget, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     text = TextProperty('text')
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_combo_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from PyQt6.QtCore import pyqtSignal, Qt, QPoint, QPropertyAnimation, QEasingCurve, QSize, QParallelAnimationGroup
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QMenu, QHBoxLayout, QApplication
 
 from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, \
     MethodsProperty, TextProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
-from PyQtUIkit.widgets.icon_widget import KitIconWidget
-from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.layout import KitVBoxLayout
-from PyQtUIkit.widgets.button import KitLayoutButton
+from PyQtUIkit.widgets._icon_widget import KitIconWidget
+from PyQtUIkit.widgets._scroll_area import KitScrollArea
+from PyQtUIkit.widgets._layout import KitVBoxLayout
+from PyQtUIkit.widgets._button import KitLayoutButton
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
     selected = pyqtSignal(object)
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QDialog, QVBoxLayout, QLabel
 
 from PyQtUIkit.core.properties import PaletteProperty, BoolProperty, StringProperty, IconProperty, TextProperty
 from PyQtUIkit.widgets import KitIconButton, KitHBoxLayout, KitVBoxLayout, KitButton, KitIconWidget, KitLabel
-from PyQtUIkit.widgets.form import KitForm
+from PyQtUIkit.widgets._form import KitForm
 from PyQtUIkit.widgets._widget import _KitWidget
 
 
 class KitDialog(QDialog, _KitWidget):
     header_palette = PaletteProperty('header_palette', 'Menu')
     button_close = BoolProperty('button_close', True)
     name = TextProperty('name')
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/grid_layout.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_grid_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tab_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from PyQt6.QtWidgets import QPushButton, QHBoxLayout, QSizePolicy, QWidget
 from PyQt6.QtGui import QFontMetrics
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontProperty
 from PyQtUIkit.themes import KitPalette
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
-from PyQtUIkit.widgets.icon_widget import KitIconWidget
-from PyQtUIkit.widgets.button import KitIconButton, KitButton
-from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.layout import KitHBoxLayout
-from PyQtUIkit.widgets.label import KitLabel
+from PyQtUIkit.widgets._icon_widget import KitIconWidget
+from PyQtUIkit.widgets._button import KitIconButton, KitButton
+from PyQtUIkit.widgets._scroll_area import KitScrollArea
+from PyQtUIkit.widgets._layout import KitHBoxLayout
+from PyQtUIkit.widgets._label import KitLabel
 
 
 class KitTab(QPushButton, _KitWidget):
     radius_top = IntProperty('radius_top', 5)
     radius_bottom = IntProperty('radius_bottom', 0)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/tabs_layout.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tabs_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_toggle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint, QPropertyAnimation, QEasingCurve
 from PyQt6.QtWidgets import QWidget, QPushButton
 
 from PyQtUIkit.core import *
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
-from PyQtUIkit.widgets.button import KitButton
+from PyQtUIkit.widgets._button import KitButton
 
 
 class KitToggle(QWidget, _KitWidget):
     class Mode(Enum):
         SMALL = 0
         MEDIUM = 1
         LARGE = 2
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tree_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, StringProperty, IconProperty, BoolProperty, EnumProperty, \
     PaletteProperty, FontProperty, MethodsProperty
-from PyQtUIkit.widgets.dialog import KitDialog
-from PyQtUIkit.widgets.layout import KitVBoxLayout, KitHBoxLayout
-from PyQtUIkit.widgets.icon_widget import KitIconWidget
-from PyQtUIkit.widgets.label import KitLabel
-from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.button import KitLayoutButton, KitIconButton
-from PyQtUIkit.widgets.checkbox import KitCheckBox
+from PyQtUIkit.widgets._dialog import KitDialog
+from PyQtUIkit.widgets._layout import KitVBoxLayout, KitHBoxLayout
+from PyQtUIkit.widgets._icon_widget import KitIconWidget
+from PyQtUIkit.widgets._label import KitLabel
+from PyQtUIkit.widgets._scroll_area import KitScrollArea
+from PyQtUIkit.widgets._button import KitLayoutButton, KitIconButton
+from PyQtUIkit.widgets._checkbox import KitCheckBox
 
 
 class KitTreeWidgetItem(KitVBoxLayout):
     name = StringProperty('name', '')
     radius = IntProperty('radius', 4)
     icon = IconProperty('icon')
     text_palette = PaletteProperty('text_palette', 'Main')
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.9.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.7
+Version: 2.9.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.7/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.9.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,41 +42,43 @@
 PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
 PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
 PyQtUIkit/fonts/RobotoMono-Thin.ttf
 PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
 PyQtUIkit/themes/__init__.py
 PyQtUIkit/themes/builtin_themes.py
 PyQtUIkit/themes/icons.py
+PyQtUIkit/themes/languages.py
 PyQtUIkit/themes/locale.py
 PyQtUIkit/themes/svg.py
 PyQtUIkit/themes/theme.py
 PyQtUIkit/widgets/__init__.py
-PyQtUIkit/widgets/_widget.py
-PyQtUIkit/widgets/application.py
-PyQtUIkit/widgets/button.py
-PyQtUIkit/widgets/checkbox.py
-PyQtUIkit/widgets/combo_box.py
-PyQtUIkit/widgets/dialog.py
-PyQtUIkit/widgets/flow_layout.py
-PyQtUIkit/widgets/form.py
-PyQtUIkit/widgets/grid_layout.py
-PyQtUIkit/widgets/group.py
-PyQtUIkit/widgets/icon_widget.py
-PyQtUIkit/widgets/label.py
-PyQtUIkit/widgets/layout.py
-PyQtUIkit/widgets/line_edit.py
-PyQtUIkit/widgets/list_widget.py
-PyQtUIkit/widgets/main_window.py
-PyQtUIkit/widgets/menu.py
-PyQtUIkit/widgets/menu_bar.py
-PyQtUIkit/widgets/navigation.py
-PyQtUIkit/widgets/progress_bar.py
-PyQtUIkit/widgets/radio.py
-PyQtUIkit/widgets/scroll_area.py
-PyQtUIkit/widgets/separator.py
-PyQtUIkit/widgets/spin_box.py
-PyQtUIkit/widgets/spinner.py
-PyQtUIkit/widgets/tab_bar.py
-PyQtUIkit/widgets/tabs_layout.py
-PyQtUIkit/widgets/text_edit.py
-PyQtUIkit/widgets/toggle.py
-PyQtUIkit/widgets/tree_widget.py
+PyQtUIkit/widgets/_application.py
+PyQtUIkit/widgets/_button.py
+PyQtUIkit/widgets/_checkbox.py
+PyQtUIkit/widgets/_combo_box.py
+PyQtUIkit/widgets/_dialog.py
+PyQtUIkit/widgets/_flow_layout.py
+PyQtUIkit/widgets/_form.py
+PyQtUIkit/widgets/_grid_layout.py
+PyQtUIkit/widgets/_group.py
+PyQtUIkit/widgets/_icon_widget.py
+PyQtUIkit/widgets/_label.py
+PyQtUIkit/widgets/_layout.py
+PyQtUIkit/widgets/_line_edit.py
+PyQtUIkit/widgets/_list_widget.py
+PyQtUIkit/widgets/_main_window.py
+PyQtUIkit/widgets/_menu.py
+PyQtUIkit/widgets/_menu_bar.py
+PyQtUIkit/widgets/_navigation.py
+PyQtUIkit/widgets/_progress_bar.py
+PyQtUIkit/widgets/_radio.py
+PyQtUIkit/widgets/_scintilla.py
+PyQtUIkit/widgets/_scroll_area.py
+PyQtUIkit/widgets/_separator.py
+PyQtUIkit/widgets/_spin_box.py
+PyQtUIkit/widgets/_spinner.py
+PyQtUIkit/widgets/_tab_bar.py
+PyQtUIkit/widgets/_tabs_layout.py
+PyQtUIkit/widgets/_text_edit.py
+PyQtUIkit/widgets/_toggle.py
+PyQtUIkit/widgets/_tree_widget.py
+PyQtUIkit/widgets/_widget.py
```

### Comparing `PyQtUIkit-2.8.7/setup.py` & `PyQtUIkit-2.9.0/setup.py`

 * *Files identical despite different names*

