# Comparing `tmp/PyQtUIkit-2.9.0.tar.gz` & `tmp/PyQtUIkit-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.9.0.tar", last modified: Sun May  5 20:58:00 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.9.1.tar", last modified: Mon May  6 10:03:56 2024, max compression
```

## Comparing `PyQtUIkit-2.9.0.tar` & `PyQtUIkit-2.9.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/
--rw-rw-rw-   0        0        0     1090 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3417 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3271 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.490498 PyQtUIkit-2.9.0/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.506125 PyQtUIkit-2.9.0/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.506125 PyQtUIkit-2.9.0/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     4314 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     6433 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1810582 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0    10274 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/languages.py
--rw-rw-rw-   0        0        0     1830 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1807 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1818 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     1367 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_application.py
--rw-rw-rw-   0        0        0     8034 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_button.py
--rw-rw-rw-   0        0        0     2795 2024-05-05 20:57:21.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_checkbox.py
--rw-rw-rw-   0        0        0    11428 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_combo_box.py
--rw-rw-rw-   0        0        0     8329 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_dialog.py
--rw-rw-rw-   0        0        0     5876 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_form.py
--rw-rw-rw-   0        0        0     4350 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_grid_layout.py
--rw-rw-rw-   0        0        0     2280 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_group.py
--rw-rw-rw-   0        0        0     1578 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_label.py
--rw-rw-rw-   0        0        0     5436 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_layout.py
--rw-rw-rw-   0        0        0     1697 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_main_window.py
--rw-rw-rw-   0        0        0     4253 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu.py
--rw-rw-rw-   0        0        0     4948 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu_bar.py
--rw-rw-rw-   0        0        0     7471 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_navigation.py
--rw-rw-rw-   0        0        0     2647 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_progress_bar.py
--rw-rw-rw-   0        0        0     6805 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_radio.py
--rw-rw-rw-   0        0        0     4568 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scintilla.py
--rw-rw-rw-   0        0        0     4021 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_separator.py
--rw-rw-rw-   0        0        0     7515 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spinner.py
--rw-rw-rw-   0        0        0    14128 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tab_bar.py
--rw-rw-rw-   0        0        0     1313 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tabs_layout.py
--rw-rw-rw-   0        0        0     4538 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_text_edit.py
--rw-rw-rw-   0        0        0     4466 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_toggle.py
--rw-rw-rw-   0        0        0    17885 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tree_widget.py
--rw-rw-rw-   0        0        0     3304 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/PyQtUIkit/widgets/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:58:00.474902 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2707 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 20:58:00.000000 PyQtUIkit-2.9.0/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 20:58:00.521750 PyQtUIkit-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-05-05 20:57:22.000000 PyQtUIkit-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:56.025178 PyQtUIkit-2.9.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-05-06 10:03:56.025178 PyQtUIkit-2.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:55.993920 PyQtUIkit-2.9.1/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3417 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:55.993920 PyQtUIkit-2.9.1/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:55.993920 PyQtUIkit-2.9.1/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:56.009554 PyQtUIkit-2.9.1/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:56.009554 PyQtUIkit-2.9.1/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4314 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     6433 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1810582 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0    10274 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/languages.py
+-rw-rw-rw-   0        0        0     1830 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1807 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:56.025178 PyQtUIkit-2.9.1/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1818 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1367 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_application.py
+-rw-rw-rw-   0        0        0     8034 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_button.py
+-rw-rw-rw-   0        0        0     2795 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_checkbox.py
+-rw-rw-rw-   0        0        0    11428 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_combo_box.py
+-rw-rw-rw-   0        0        0     8329 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_form.py
+-rw-rw-rw-   0        0        0     4350 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_group.py
+-rw-rw-rw-   0        0        0     1578 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_label.py
+-rw-rw-rw-   0        0        0     5436 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_layout.py
+-rw-rw-rw-   0        0        0     1697 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_menu.py
+-rw-rw-rw-   0        0        0     4948 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_menu_bar.py
+-rw-rw-rw-   0        0        0     7471 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_radio.py
+-rw-rw-rw-   0        0        0     4821 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_scintilla.py
+-rw-rw-rw-   0        0        0     4021 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_separator.py
+-rw-rw-rw-   0        0        0     7515 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_spinner.py
+-rw-rw-rw-   0        0        0    14128 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tab_bar.py
+-rw-rw-rw-   0        0        0     1313 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_text_edit.py
+-rw-rw-rw-   0        0        0     4466 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_toggle.py
+-rw-rw-rw-   0        0        0    17885 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tree_widget.py
+-rw-rw-rw-   0        0        0     3304 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/PyQtUIkit/widgets/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:03:55.993920 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2707 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 10:03:55.000000 PyQtUIkit-2.9.1/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 10:03:56.025178 PyQtUIkit-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-05-06 10:03:25.000000 PyQtUIkit-2.9.1/setup.py
```

### Comparing `PyQtUIkit-2.9.0/LICENSE` & `PyQtUIkit-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PKG-INFO` & `PyQtUIkit-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.9.0
+Version: 2.9.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/_icons.py` & `PyQtUIkit-2.9.1/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/_translate.py` & `PyQtUIkit-2.9.1/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.9.1/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.9.1/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.9.1/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/core/font.py` & `PyQtUIkit-2.9.1/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.9.1/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.9.1/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.9.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/languages.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/languages.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.9.1/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_application.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_button.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_checkbox.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_combo_box.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_dialog.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_flow_layout.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_form.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_grid_layout.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_grid_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_group.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_icon_widget.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_label.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_layout.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_line_edit.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_list_widget.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_main_window.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_menu_bar.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_navigation.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_progress_bar.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_radio.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scintilla.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_scintilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from PyQtUIkit.core.properties import PaletteProperty, IntProperty, FontProperty, EnumProperty
 
 from PyQtUIkit.widgets._widget import _KitWidget
 
 
 try:
     from PyQt6.Qsci import QsciScintilla, QsciLexer
-
-    from themes import languages
 except ImportError:
     class KitScintilla(QWidget, _KitWidget):
         def __init__(self, *args, **kwargs):
             super().__init__()
             raise ImportError("QScintilla is not installed. Please install by running 'pip install PyQt6-QScintilla'.")
 else:
+    from PyQtUIkit.themes import languages
+
     class KitScintilla(QsciScintilla, _KitWidget):
         main_palette = PaletteProperty('main_palette', 'Main')
         margins_palette = PaletteProperty('margins_palette', 'Bg')
         border = IntProperty('border', 0)
         radius = IntProperty('radius', 0)
         font = FontProperty('font', 'mono')
         font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
@@ -50,14 +50,24 @@
             self.setCallTipsVisible(0)
             self.setMarginWidth(0, 40)
 
             self.current_row = 0
 
             self._apply_lexer()
 
+        @property
+        def language(self):
+            return self._lang
+
+        @language.setter
+        def language(self, value):
+            self._lang = value
+            self._apply_lexer()
+            self._apply_theme()
+
         def _apply_lexer(self):
             if self._lang.lexer is not None:
                 self._lexer = self._lang.lexer(self)
                 self.setLexer(self._lexer)
             else:
                 self._lexer = None
```

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_scroll_area.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_separator.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spin_box.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_spinner.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tab_bar.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tabs_layout.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tabs_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_text_edit.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_toggle.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_tree_widget.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.9.1/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.9.1/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.9.0
+Version: 2.9.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.9.0/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.9.1/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.9.0/setup.py` & `PyQtUIkit-2.9.1/setup.py`

 * *Files identical despite different names*

