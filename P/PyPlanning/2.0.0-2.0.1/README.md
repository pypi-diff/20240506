# Comparing `tmp/PyPlanning-2.0.0.tar.gz` & `tmp/pyplanning-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlanning-2.0.0.tar", last modified: Wed Mar 27 16:01:50 2024, max compression
+gzip compressed data, was "pyplanning-2.0.1.tar", last modified: Mon May  6 07:55:36 2024, max compression
```

## Comparing `PyPlanning-2.0.0.tar` & `pyplanning-2.0.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.308186 PyPlanning-2.0.0/
--rw-rw-rw-   0        0        0    35821 2023-12-06 13:22:03.000000 PyPlanning-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    45067 2024-03-27 16:01:50.306755 PyPlanning-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.304381 PyPlanning-2.0.0/PyPlanning.egg-info/
--rw-rw-rw-   0        0        0    45067 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2307 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 16:01:50.000000 PyPlanning-2.0.0/PyPlanning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2280 2024-03-27 15:50:31.000000 PyPlanning-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.194190 PyPlanning-2.0.0/planning/
--rw-rw-rw-   0        0        0       84 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/__init__.py
--rw-rw-rw-   0        0        0      934 2024-03-14 14:22:32.000000 PyPlanning-2.0.0/planning/app.py
--rw-rw-rw-   0        0        0     2900 2023-03-07 16:16:22.000000 PyPlanning-2.0.0/planning/config.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.262632 PyPlanning-2.0.0/planning/data/
--rw-rw-rw-   0        0        0     1790 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/chart.svg
--rw-rw-rw-   0        0        0     2229 2022-02-12 15:43:29.000000 PyPlanning-2.0.0/planning/data/collapse.svg
--rw-rw-rw-   0        0        0     2938 2024-03-15 09:44:22.000000 PyPlanning-2.0.0/planning/data/duplicate_task.svg
--rw-rw-rw-   0        0        0     1610 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/edit.svg
--rw-rw-rw-   0        0        0     4195 2022-02-12 15:43:55.000000 PyPlanning-2.0.0/planning/data/expand.svg
--rw-rw-rw-   0        0        0     2386 2022-02-17 10:27:24.000000 PyPlanning-2.0.0/planning/data/invalid.svg
--rw-rw-rw-   0        0        0     1760 2022-02-12 15:34:26.000000 PyPlanning-2.0.0/planning/data/leave.svg
--rw-rw-rw-   0        0        0      353 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-about.svg
--rw-rw-rw-   0        0        0     2094 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-calendar-leave.svg
--rw-rw-rw-   0        0        0      708 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-close.svg
--rw-rw-rw-   0        0        0      436 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-contacts.svg
--rw-rw-rw-   0        0        0      881 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-expired.svg
--rw-rw-rw-   0        0        0      279 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-file.svg
--rw-rw-rw-   0        0        0      737 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-folder-open.svg
--rw-rw-rw-   0        0        0      358 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-folder.svg
--rw-rw-rw-   0        0        0     1265 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-help.svg
--rw-rw-rw-   0        0        0      346 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-import.svg
--rw-rw-rw-   0        0        0      345 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-redo.svg
--rw-rw-rw-   0        0        0     1237 2024-03-15 09:44:22.000000 PyPlanning-2.0.0/planning/data/libre-gui-refresh.svg
--rw-rw-rw-   0        0        0     1102 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-save.svg
--rw-rw-rw-   0        0        0      607 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-trash.svg
--rw-rw-rw-   0        0        0      513 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/libre-gui-undo.svg
--rw-rw-rw-   0        0        0      801 2023-02-12 10:55:32.000000 PyPlanning-2.0.0/planning/data/logs.svg
--rw-rw-rw-   0        0        0     1409 2022-02-17 10:28:59.000000 PyPlanning-2.0.0/planning/data/milestone.svg
--rw-rw-rw-   0        0        0     2458 2022-02-22 21:17:56.000000 PyPlanning-2.0.0/planning/data/move_down.svg
--rw-rw-rw-   0        0        0     2100 2022-02-22 21:18:02.000000 PyPlanning-2.0.0/planning/data/move_up.svg
--rw-rw-rw-   0        0        0     3842 2022-02-13 16:51:50.000000 PyPlanning-2.0.0/planning/data/new_chart.svg
--rw-rw-rw-   0        0        0     2229 2022-02-12 15:34:04.000000 PyPlanning-2.0.0/planning/data/new_leave.svg
--rw-rw-rw-   0        0        0     2085 2022-02-17 10:32:07.000000 PyPlanning-2.0.0/planning/data/new_milestone.svg
--rw-rw-rw-   0        0        0     2377 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/data/new_project.svg
--rw-rw-rw-   0        0        0     2749 2022-02-12 15:30:40.000000 PyPlanning-2.0.0/planning/data/new_resource.svg
--rw-rw-rw-   0        0        0     2297 2022-02-12 15:35:55.000000 PyPlanning-2.0.0/planning/data/new_task.svg
--rw-rw-rw-   0        0        0     4755 2023-10-25 07:14:22.000000 PyPlanning-2.0.0/planning/data/planning-banner.svg
--rw-rw-rw-   0        0        0     8266 2023-10-25 07:12:05.000000 PyPlanning-2.0.0/planning/data/planning-title.png
--rw-rw-rw-   0        0        0     4361 2023-10-25 07:14:19.000000 PyPlanning-2.0.0/planning/data/planning-title.svg
--rw-rw-rw-   0        0        0     8294 2023-10-25 07:07:15.000000 PyPlanning-2.0.0/planning/data/planning.png
--rw-rw-rw-   0        0        0     3482 2022-02-14 18:04:17.000000 PyPlanning-2.0.0/planning/data/planning.svg
--rw-rw-rw-   0        0        0      582 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/project.svg
--rw-rw-rw-   0        0        0     2250 2022-02-12 15:30:16.000000 PyPlanning-2.0.0/planning/data/resource.svg
--rw-rw-rw-   0        0        0      434 2019-01-11 22:20:42.000000 PyPlanning-2.0.0/planning/data/task.svg
--rw-rw-rw-   0        0        0     2896 2022-02-24 13:22:20.000000 PyPlanning-2.0.0/planning/data/today.svg
--rw-rw-rw-   0        0        0   111316 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/gantt.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.275638 PyPlanning-2.0.0/planning/gui/
--rw-rw-rw-   0        0        0        0 2022-01-16 07:40:28.000000 PyPlanning-2.0.0/planning/gui/__init__.py
--rw-rw-rw-   0        0        0    12129 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/gui/centralwidget.py
--rw-rw-rw-   0        0        0     2941 2023-12-01 16:59:55.000000 PyPlanning-2.0.0/planning/gui/logviewer.py
--rw-rw-rw-   0        0        0     1062 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/gui/long_text_editor.py
--rw-rw-rw-   0        0        0    18227 2024-03-27 15:48:44.000000 PyPlanning-2.0.0/planning/gui/mainwindow.py
--rw-rw-rw-   0        0        0     4915 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/gui/multi_selection_combobox.py
--rw-rw-rw-   0        0        0     2644 2023-02-05 14:25:25.000000 PyPlanning-2.0.0/planning/gui/svgviewer.py
--rw-rw-rw-   0        0        0    50221 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/gui/treewidgets.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.168347 PyPlanning-2.0.0/planning/locale/
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.168347 PyPlanning-2.0.0/planning/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.278399 PyPlanning-2.0.0/planning/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4973 2024-03-27 15:57:16.000000 PyPlanning-2.0.0/planning/locale/fr/LC_MESSAGES/planning.mo
--rw-rw-rw-   0        0        0    67512 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/model.py
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.294579 PyPlanning-2.0.0/planning/tests/
--rw-rw-rw-   0        0        0        0 2022-01-16 07:40:28.000000 PyPlanning-2.0.0/planning/tests/__init__.py
--rw-rw-rw-   0        0        0      882 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_central_widget.py
--rw-rw-rw-   0        0        0     4645 2024-03-15 09:44:22.000000 PyPlanning-2.0.0/planning/tests/test_gantt.py
--rw-rw-rw-   0        0        0      400 2023-11-13 13:47:51.000000 PyPlanning-2.0.0/planning/tests/test_logviewer.py
--rw-rw-rw-   0        0        0     1617 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_model.py
--rw-rw-rw-   0        0        0      479 2023-02-05 14:54:04.000000 PyPlanning-2.0.0/planning/tests/test_svgviewer.py
--rw-rw-rw-   0        0        0     1370 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_treewidgets.py
--rw-rw-rw-   0        0        0    27490 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_v1_02.svg
--rw-rw-rw-   0        0        0    39805 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_v1_03.svg
--rw-rw-rw-   0        0        0    26198 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_v2_01.svg
--rw-rw-rw-   0        0        0    27490 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_v2_02.svg
--rw-rw-rw-   0        0        0    39805 2024-03-27 15:42:59.000000 PyPlanning-2.0.0/planning/tests/test_v2_03.svg
-drwxrwxrwx   0        0        0        0 2024-03-27 16:01:50.303383 PyPlanning-2.0.0/planning/utils/
--rw-rw-rw-   0        0        0        0 2023-02-12 10:55:32.000000 PyPlanning-2.0.0/planning/utils/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-10-25 06:32:51.000000 PyPlanning-2.0.0/planning/utils/conf.py
--rw-rw-rw-   0        0        0     5748 2023-11-13 15:20:30.000000 PyPlanning-2.0.0/planning/utils/qthelpers.py
--rw-rw-rw-   0        0        0     1848 2024-03-27 15:44:41.000000 PyPlanning-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 16:01:50.308186 PyPlanning-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.703822 pyplanning-2.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-12-06 13:22:03.000000 pyplanning-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0    45067 2024-05-06 07:55:36.703822 pyplanning-2.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.703822 pyplanning-2.0.1/PyPlanning.egg-info/
+-rw-rw-rw-   0        0        0    45067 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 07:55:36.000000 pyplanning-2.0.1/PyPlanning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2280 2024-04-29 06:43:38.000000 pyplanning-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.586493 pyplanning-2.0.1/planning/
+-rw-rw-rw-   0        0        0       84 2024-04-30 07:29:50.000000 pyplanning-2.0.1/planning/__init__.py
+-rw-rw-rw-   0        0        0      934 2024-03-14 14:22:32.000000 pyplanning-2.0.1/planning/app.py
+-rw-rw-rw-   0        0        0     2900 2023-03-07 16:16:22.000000 pyplanning-2.0.1/planning/config.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.660438 pyplanning-2.0.1/planning/data/
+-rw-rw-rw-   0        0        0     1790 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/chart.svg
+-rw-rw-rw-   0        0        0     2229 2022-02-12 15:43:29.000000 pyplanning-2.0.1/planning/data/collapse.svg
+-rw-rw-rw-   0        0        0     2938 2024-03-15 09:44:22.000000 pyplanning-2.0.1/planning/data/duplicate_task.svg
+-rw-rw-rw-   0        0        0     1610 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/edit.svg
+-rw-rw-rw-   0        0        0     4195 2022-02-12 15:43:55.000000 pyplanning-2.0.1/planning/data/expand.svg
+-rw-rw-rw-   0        0        0     2386 2022-02-17 10:27:24.000000 pyplanning-2.0.1/planning/data/invalid.svg
+-rw-rw-rw-   0        0        0     1760 2022-02-12 15:34:26.000000 pyplanning-2.0.1/planning/data/leave.svg
+-rw-rw-rw-   0        0        0      353 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-about.svg
+-rw-rw-rw-   0        0        0     2094 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-calendar-leave.svg
+-rw-rw-rw-   0        0        0      708 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-close.svg
+-rw-rw-rw-   0        0        0      436 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-contacts.svg
+-rw-rw-rw-   0        0        0      881 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-expired.svg
+-rw-rw-rw-   0        0        0      279 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-file.svg
+-rw-rw-rw-   0        0        0      737 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-folder-open.svg
+-rw-rw-rw-   0        0        0      358 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-folder.svg
+-rw-rw-rw-   0        0        0     1265 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-help.svg
+-rw-rw-rw-   0        0        0      346 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-import.svg
+-rw-rw-rw-   0        0        0      345 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-redo.svg
+-rw-rw-rw-   0        0        0     1237 2024-03-15 09:44:22.000000 pyplanning-2.0.1/planning/data/libre-gui-refresh.svg
+-rw-rw-rw-   0        0        0     1102 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-save.svg
+-rw-rw-rw-   0        0        0      607 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-trash.svg
+-rw-rw-rw-   0        0        0      513 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/libre-gui-undo.svg
+-rw-rw-rw-   0        0        0      801 2023-02-12 10:55:32.000000 pyplanning-2.0.1/planning/data/logs.svg
+-rw-rw-rw-   0        0        0     1409 2022-02-17 10:28:59.000000 pyplanning-2.0.1/planning/data/milestone.svg
+-rw-rw-rw-   0        0        0     2458 2022-02-22 21:17:56.000000 pyplanning-2.0.1/planning/data/move_down.svg
+-rw-rw-rw-   0        0        0     2100 2022-02-22 21:18:02.000000 pyplanning-2.0.1/planning/data/move_up.svg
+-rw-rw-rw-   0        0        0     3842 2022-02-13 16:51:50.000000 pyplanning-2.0.1/planning/data/new_chart.svg
+-rw-rw-rw-   0        0        0     2229 2022-02-12 15:34:04.000000 pyplanning-2.0.1/planning/data/new_leave.svg
+-rw-rw-rw-   0        0        0     2085 2022-02-17 10:32:07.000000 pyplanning-2.0.1/planning/data/new_milestone.svg
+-rw-rw-rw-   0        0        0     2377 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/data/new_project.svg
+-rw-rw-rw-   0        0        0     2749 2022-02-12 15:30:40.000000 pyplanning-2.0.1/planning/data/new_resource.svg
+-rw-rw-rw-   0        0        0     2297 2022-02-12 15:35:55.000000 pyplanning-2.0.1/planning/data/new_task.svg
+-rw-rw-rw-   0        0        0     4755 2023-10-25 07:14:22.000000 pyplanning-2.0.1/planning/data/planning-banner.svg
+-rw-rw-rw-   0        0        0     8266 2023-10-25 07:12:05.000000 pyplanning-2.0.1/planning/data/planning-title.png
+-rw-rw-rw-   0        0        0     4361 2023-10-25 07:14:19.000000 pyplanning-2.0.1/planning/data/planning-title.svg
+-rw-rw-rw-   0        0        0     8294 2023-10-25 07:07:15.000000 pyplanning-2.0.1/planning/data/planning.png
+-rw-rw-rw-   0        0        0     3482 2022-02-14 18:04:17.000000 pyplanning-2.0.1/planning/data/planning.svg
+-rw-rw-rw-   0        0        0      582 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/project.svg
+-rw-rw-rw-   0        0        0     2250 2022-02-12 15:30:16.000000 pyplanning-2.0.1/planning/data/resource.svg
+-rw-rw-rw-   0        0        0      434 2019-01-11 22:20:42.000000 pyplanning-2.0.1/planning/data/task.svg
+-rw-rw-rw-   0        0        0     2896 2022-02-24 13:22:20.000000 pyplanning-2.0.1/planning/data/today.svg
+-rw-rw-rw-   0        0        0   111458 2024-04-30 07:29:50.000000 pyplanning-2.0.1/planning/gantt.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.674977 pyplanning-2.0.1/planning/gui/
+-rw-rw-rw-   0        0        0        0 2022-01-16 07:40:28.000000 pyplanning-2.0.1/planning/gui/__init__.py
+-rw-rw-rw-   0        0        0    12129 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/gui/centralwidget.py
+-rw-rw-rw-   0        0        0     2941 2023-12-01 16:59:55.000000 pyplanning-2.0.1/planning/gui/logviewer.py
+-rw-rw-rw-   0        0        0     1062 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/gui/long_text_editor.py
+-rw-rw-rw-   0        0        0    18455 2024-04-30 07:29:50.000000 pyplanning-2.0.1/planning/gui/mainwindow.py
+-rw-rw-rw-   0        0        0     4915 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/gui/multi_selection_combobox.py
+-rw-rw-rw-   0        0        0     2644 2023-02-05 14:25:25.000000 pyplanning-2.0.1/planning/gui/svgviewer.py
+-rw-rw-rw-   0        0        0    50441 2024-04-30 07:29:50.000000 pyplanning-2.0.1/planning/gui/treewidgets.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.561538 pyplanning-2.0.1/planning/locale/
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.561538 pyplanning-2.0.1/planning/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.678194 pyplanning-2.0.1/planning/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4969 2024-05-06 07:49:29.000000 pyplanning-2.0.1/planning/locale/fr/LC_MESSAGES/planning.mo
+-rw-rw-rw-   0        0        0    68248 2024-05-06 07:43:21.000000 pyplanning-2.0.1/planning/model.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.697264 pyplanning-2.0.1/planning/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-16 07:40:28.000000 pyplanning-2.0.1/planning/tests/__init__.py
+-rw-rw-rw-   0        0        0      882 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_central_widget.py
+-rw-rw-rw-   0        0        0     4645 2024-03-15 09:44:22.000000 pyplanning-2.0.1/planning/tests/test_gantt.py
+-rw-rw-rw-   0        0        0      400 2023-11-13 13:47:51.000000 pyplanning-2.0.1/planning/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0     1617 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_model.py
+-rw-rw-rw-   0        0        0      479 2023-02-05 14:54:04.000000 pyplanning-2.0.1/planning/tests/test_svgviewer.py
+-rw-rw-rw-   0        0        0     1370 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_treewidgets.py
+-rw-rw-rw-   0        0        0    27490 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_v1_02.svg
+-rw-rw-rw-   0        0        0    39805 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_v1_03.svg
+-rw-rw-rw-   0        0        0    26198 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_v2_01.svg
+-rw-rw-rw-   0        0        0    27490 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_v2_02.svg
+-rw-rw-rw-   0        0        0    39805 2024-03-27 15:42:59.000000 pyplanning-2.0.1/planning/tests/test_v2_03.svg
+drwxrwxrwx   0        0        0        0 2024-05-06 07:55:36.701248 pyplanning-2.0.1/planning/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-12 10:55:32.000000 pyplanning-2.0.1/planning/utils/__init__.py
+-rw-rw-rw-   0        0        0     5144 2023-10-25 06:32:51.000000 pyplanning-2.0.1/planning/utils/conf.py
+-rw-rw-rw-   0        0        0     5748 2023-11-13 15:20:30.000000 pyplanning-2.0.1/planning/utils/qthelpers.py
+-rw-rw-rw-   0        0        0     1848 2024-04-29 06:43:38.000000 pyplanning-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:55:36.703822 pyplanning-2.0.1/setup.cfg
```

### Comparing `PyPlanning-2.0.0/LICENSE` & `pyplanning-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/PKG-INFO` & `pyplanning-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlanning
-Version: 2.0.0
+Version: 2.0.1
 Summary: Manage team schedules and quickly create simple project plannings
 Author-email: Pierre Raybaut <p.raybaut@codra.fr>
 Maintainer-email: PyPlanning Developers <p.raybaut@codra.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `PyPlanning-2.0.0/PyPlanning.egg-info/PKG-INFO` & `pyplanning-2.0.1/PyPlanning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlanning
-Version: 2.0.0
+Version: 2.0.1
 Summary: Manage team schedules and quickly create simple project plannings
 Author-email: Pierre Raybaut <p.raybaut@codra.fr>
 Maintainer-email: PyPlanning Developers <p.raybaut@codra.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `PyPlanning-2.0.0/PyPlanning.egg-info/SOURCES.txt` & `pyplanning-2.0.1/PyPlanning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/README.md` & `pyplanning-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/app.py` & `pyplanning-2.0.1/planning/app.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/config.py` & `pyplanning-2.0.1/planning/config.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/chart.svg` & `pyplanning-2.0.1/planning/data/chart.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/collapse.svg` & `pyplanning-2.0.1/planning/data/collapse.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/duplicate_task.svg` & `pyplanning-2.0.1/planning/data/duplicate_task.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/edit.svg` & `pyplanning-2.0.1/planning/data/edit.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/expand.svg` & `pyplanning-2.0.1/planning/data/expand.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/invalid.svg` & `pyplanning-2.0.1/planning/data/invalid.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/leave.svg` & `pyplanning-2.0.1/planning/data/leave.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-calendar-leave.svg` & `pyplanning-2.0.1/planning/data/libre-gui-calendar-leave.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-close.svg` & `pyplanning-2.0.1/planning/data/libre-gui-close.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-expired.svg` & `pyplanning-2.0.1/planning/data/libre-gui-expired.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-folder-open.svg` & `pyplanning-2.0.1/planning/data/libre-gui-folder-open.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-help.svg` & `pyplanning-2.0.1/planning/data/libre-gui-help.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-refresh.svg` & `pyplanning-2.0.1/planning/data/libre-gui-refresh.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-save.svg` & `pyplanning-2.0.1/planning/data/libre-gui-save.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-trash.svg` & `pyplanning-2.0.1/planning/data/libre-gui-trash.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/libre-gui-undo.svg` & `pyplanning-2.0.1/planning/data/libre-gui-undo.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/logs.svg` & `pyplanning-2.0.1/planning/data/logs.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/milestone.svg` & `pyplanning-2.0.1/planning/data/milestone.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/move_down.svg` & `pyplanning-2.0.1/planning/data/move_down.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/move_up.svg` & `pyplanning-2.0.1/planning/data/move_up.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_chart.svg` & `pyplanning-2.0.1/planning/data/new_chart.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_leave.svg` & `pyplanning-2.0.1/planning/data/new_leave.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_milestone.svg` & `pyplanning-2.0.1/planning/data/new_milestone.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_project.svg` & `pyplanning-2.0.1/planning/data/new_project.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_resource.svg` & `pyplanning-2.0.1/planning/data/new_resource.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/new_task.svg` & `pyplanning-2.0.1/planning/data/new_task.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/planning-banner.svg` & `pyplanning-2.0.1/planning/data/planning-banner.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/planning-title.png` & `pyplanning-2.0.1/planning/data/planning-title.png`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/planning-title.svg` & `pyplanning-2.0.1/planning/data/planning-title.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/planning.png` & `pyplanning-2.0.1/planning/data/planning.png`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/planning.svg` & `pyplanning-2.0.1/planning/data/planning.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/project.svg` & `pyplanning-2.0.1/planning/data/project.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/resource.svg` & `pyplanning-2.0.1/planning/data/resource.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/data/today.svg` & `pyplanning-2.0.1/planning/data/today.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gantt.py` & `pyplanning-2.0.1/planning/gantt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1283,15 +1283,15 @@
                 stroke_width=2,
                 opacity=0.85,
             )
         )
         svg.add(
             svgwrite.shapes.Rect(
                 insert=((x + 1 + offset) * mm, (y + 6) * mm),
-                size=(((d - 2)) * mm, 3 * mm),
+                size=((d - 2) * mm, 3 * mm),
                 fill="#909090",
                 stroke=color,
                 stroke_width=1,
                 opacity=0.2,
             )
         )
 
@@ -2517,23 +2517,17 @@
 
         if len(self.tasks) == 0:
             LOG.warning("** Empty project : {0}".format(self.name))
             return
 
         self._reset_coord()
 
-        if start is None:
-            start_date = self.start_date()
-        else:
-            start_date = start
+        start_date = self.start_date() if start is None else start
 
-        if end is None:
-            end_date = self.end_date()
-        else:
-            end_date = end
+        end_date = self.end_date() if end is None else end
 
         if start_date > end_date:
             message = "start date {0} > end_date {1}".format(start_date, end_date)
             LOG.critical(message)
             raise ValueError(message)
 
         if resources is None:
@@ -2597,18 +2591,15 @@
                     font_family=_font_attributes()["font_family"],
                     font_size=15 + 3,
                 )
             )
 
             overcharged_days = r.search_for_task_conflicts()
 
-            if resource_on_left:
-                conflict_display_line = nline + 1
-            else:
-                conflict_display_line = nline
+            conflict_display_line = nline + 1 if resource_on_left else nline
             nline += 1
 
             vac = svgwrite.container.Group()
             conflicts = svgwrite.container.Group()
             cday = start_date
             while cday <= end_date:
                 # Vacations
@@ -2717,14 +2708,23 @@
                 size=((maxx + 1 + offset / 10) * cm, (nline + 1) * cm),
                 fill="white",
                 stroke_width=0,
                 opacity=1,
             )
         )
         dwg.add(
+            svgwrite.shapes.Line(
+                start=((0) * cm, (nline + 1) * cm),
+                end=((maxx + 1 + offset / 10) * cm, (nline + 1) * cm),
+                stroke="black",
+                stroke_width=2,
+            )
+        )
+
+        dwg.add(
             self._svg_calendar(
                 maxx, nline - 1, start_date, today, scale, offset=offset, t0mode=t0mode
             )
         )
         dwg.add(ldwg)
         dwg.save(width=(maxx + 1 + offset / 10) * cm, height=(nline + 1) * cm)
         return {
@@ -2765,15 +2765,14 @@
         avail_width: int,
         color: str,
         x: float,
         prev_y: int,
         margin: int = 5,
         font_size: int = 18,
     ) -> tuple[Optional[svgwrite.container.Group], float]:
-
         line_char_count = int(avail_width / (font_size / 2))
 
         text_lines = self.description.split("\n")
         text_lines = sum(
             (textwrap.wrap(line, width=line_char_count) for line in text_lines),
             [self.name],
         )
@@ -2785,15 +2784,15 @@
         title_capital_chars = sum(1 for char in self.name if char.isupper())
         title_lower_chars = len(self.name) - title_capital_chars
         title_width = (
             title_capital_chars * font_size / 1.5 + title_lower_chars * font_size / 2
         )
         max_line_char_count = max(len(line) for line in text_lines)
         width = int(max(title_width, max_line_char_count * font_size / 2) + 2 * margin)
-
+        width = min(avail_width, width)
         height = line_count * font_size + 2 * margin
 
         x_top_left = x * mm - width
         y_top_left = (prev_y + 0.5) * cm
         desc_box = svgwrite.container.Group()
 
         desc_box.add(
@@ -2817,29 +2816,29 @@
             )
         )
 
         desc_box.add(
             svgwrite.text.Text(
                 text_lines[0],
                 insert=(
-                    x_top_left + margin,
+                    x_top_left + 2 * margin,
                     y_top_left + margin / 2 + font_size,
                 ),  # * px_to_mm),
                 font_size=font_size,
                 font_family=_font_attributes()["font_family"],
                 font_weight="bold",
             )
         )
 
         for i, line in enumerate(text_lines[1:], start=1):
             desc_box.add(
                 svgwrite.text.Text(
                     line,
                     insert=(
-                        x_top_left + margin,
+                        x_top_left + 2 * margin,
                         y_top_left + margin / 2 + (i + 1) * font_size,
                     ),
                     font_size=font_size,
                     font_family=_font_attributes()["font_family"],
                     font_weight="normal",
                 )
             )
@@ -2954,15 +2953,14 @@
                 )
                 prj_bar = True
 
             else:
                 cy -= 1
 
             if is_project_in_interval and level >= 1 and self.show_description:
-
                 x = _time_diff(scale, start, end, False) * 10
                 desc_box, px_desc_height = self.desc_svg(
                     400, color, x, prev_y, font_size=font_size
                 )
                 if desc_box is not None:
                     prj.add(desc_box)
```

### Comparing `PyPlanning-2.0.0/planning/gui/centralwidget.py` & `pyplanning-2.0.1/planning/gui/centralwidget.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gui/logviewer.py` & `pyplanning-2.0.1/planning/gui/logviewer.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gui/long_text_editor.py` & `pyplanning-2.0.1/planning/gui/long_text_editor.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gui/mainwindow.py` & `pyplanning-2.0.1/planning/gui/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from guidata import __version__ as GUIDATA_VERSION_STR
 from guidata.configtools import get_icon
 from guidata.qthelpers import add_actions, create_action, win32_fix_title_bar_background
 from guidata.userconfig import get_config_basedir
 from guidata.widgets.console import DockableConsole
 from qtpy import QtCore as QC
+from qtpy import QtGui as QG
 from qtpy import QtWidgets as QW
 from qtpy.compat import getopenfilename, getsavefilename
 
 #  Local imports
 from planning import __version__
 from planning.config import APP_DESC, APP_NAME, DEBUG, DEBUG_VAR_STR, Conf, _
 from planning.gantt import LOG
@@ -94,14 +95,19 @@
         self.tasks_menu = None
         self.projects_menu = None
         self.help_menu = None
 
         self.create_actions()
         self.create_menus()
         self.create_toolbars()
+
+        # This is necessary when the application is opened in xml mode
+        if self.central_widget.editor.xml_mode:
+            self.central_widget.editor.trees.hideEvent(QG.QHideEvent())
+
         self.statusBar().showMessage(_("Welcome to %s!") % APP_NAME, 5000)
 
         self.check_recent_files()
         if fname is None and self.recent_files:
             fname = self.recent_files[0]
         ok = False
         if fname is not None:
```

### Comparing `PyPlanning-2.0.0/planning/gui/multi_selection_combobox.py` & `pyplanning-2.0.1/planning/gui/multi_selection_combobox.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gui/svgviewer.py` & `pyplanning-2.0.1/planning/gui/svgviewer.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/gui/treewidgets.py` & `pyplanning-2.0.1/planning/gui/treewidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """PyPlanning task tree widget"""
 
 # pylint: disable=no-name-in-module
 # pylint: disable=no-member
 
-
 import datetime
 import os
 import re
 import xml.etree.ElementTree as ET
 from typing import Any, Callable, Generic, Optional, TypeVar, Union
 
 from guidata import qthelpers
@@ -148,17 +147,15 @@
     def commitAndCloseEditor(self):  # pylint: disable=invalid-name
         """Reimplement Qt method"""
         self.editor_opened = False
         editor = self.sender()
         self.commitData.emit(editor)
         self.closeEditor.emit(editor)
 
-    def setEditorData(
-        self, editor: ItemEditor, index: QC.QModelIndex
-    ):  # pylint: disable=invalid-name
+    def setEditorData(self, editor: ItemEditor, index: QC.QModelIndex):  # pylint: disable=invalid-name
         """Reimplement Qt method"""
         ditem = self.dataitem_from_index(index)
         value = ditem.to_widget_value()
         if ditem.datatype == DTypes.DAYS:
             editor.setValue(value)
         elif ditem.datatype == DTypes.DATE:
             editor.setDate(value)
@@ -428,14 +425,15 @@
             # down_action should be disabled if the next data is "LeaveData"
             self.down_action.setEnabled(item.row() < parent.rowCount() - 1)
 
     def update_menu(self):
         """Update context menu"""
         self.menu.clear()
         indexes = self.selectedIndexes()
+        self.set_specific_actions_state(bool(indexes))
         actions = self.get_actions_from_indexes(indexes)
         if actions:
             actions.append(None)
         actions += self.specific_actions
         add_actions(self.menu, actions)
 
     def contextMenuEvent(self, event):  # pylint: disable=C0103
@@ -569,17 +567,18 @@
             text: str = "" if ditem is None else ditem.to_display()
 
             if update:
                 item = items[column]
                 item.setText(text)
                 if ditem is not None:
                     self.update_item_icon(item, ditem)
-                    if ditem.datatype == DTypes.COLOR and ditem.value is not None:
-                        color = ditem.get_html_color(ditem.value)
-                        item.setBackground(QG.QBrush(QG.QColor(color)))
+                    if ditem.datatype == DTypes.COLOR:
+                        color = ditem.get_html_color(ditem.value or "")
+                        qcolor = QG.QBrush(QG.QColor(color)) if color else QG.QBrush()
+                        item.setBackground(qcolor)
             else:
                 item = QG.QStandardItem(text)
                 self.item_data[id(item)] = ditem
                 if column == 0 and group:
                     font = item.font()
                     font.setBold(True)
                     item.setFont(font)
@@ -881,15 +880,15 @@
         self.set_current_id(data.id.value)
         self.repopulate()
         self.edit(self.currentIndex())
 
     def duplicate_task(self):
         """Duplicates the selected task."""
         current_data: AbstractData | None = self.get_current_data()
-        if isinstance(current_data, AbstractTaskData):
+        if isinstance(current_data, AbstractTaskData) and self.planning is not None:
             data = current_data.duplicate()
             self.planning.add_task(data, after_data=current_data)
             self.__add_taskitem(data)
             self.set_current_id(data_id=data.id.value)
             self.repopulate()
             self.edit(self.currentIndex())
 
@@ -918,15 +917,15 @@
             item_row = self.get_item_row_from_id(data.id.value)
             self.edit(item_row[1].index())
 
     def __add_resourceitem(self, data: ResourceData):
         """Add resource item to tree"""
         self.add_or_update_item_row(data, group=True)
 
-    def __add_taskitem(self, data: MilestoneData | TaskData):
+    def __add_taskitem(self, data: AbstractTaskData):
         """Add task/milestone item to tree"""
         if isinstance(data, MilestoneData):
             self.add_or_update_item_row(data)
         else:
             for resid in data.iterate_resource_ids():
                 parent_row = self.get_item_row_from_id(resid)[0]
                 self.add_or_update_item_row(data, parent_row)
@@ -1219,15 +1218,19 @@
         self.__snapshots = []
         self.__snapshots_lock = False
         self.planning: Optional[PlanningData] = None
 
         self.project_tree = ProjectTreeWidget(self, debug=debug)
         self.chart_tree = ChartTreeWidget(self, debug=debug)
         self.task_tree = TaskTreeWidget(self, debug=debug)
-        self.forest = [self.chart_tree, self.task_tree, self.project_tree]
+        self.forest: list[BaseTreeWidget] = [
+            self.chart_tree,
+            self.task_tree,
+            self.project_tree,
+        ]
         for tree in self.forest:
             tree.SIG_MODEL_CHANGED.connect(self.model_has_changed)
             tree.pressed.connect(self.tree_pressed)
             self.addWidget(tree)
 
         self.undo_action = None
         self.redo_action = None
@@ -1237,14 +1240,15 @@
 
         self.toolbars = self.create_toolbars()
 
         # Task tree is default
         self.task_tree.setFocus()
         self.chart_tree.set_specific_actions_state(False)
         self.chart_tree.toolbar.hide()
+        self.project_tree.toolbar.hide()
 
         self.setCollapsible(0, False)
         self.setCollapsible(1, False)
         self.setStretchFactor(0, 1)
         self.setStretchFactor(1, 4)
 
         # self.task_tree.FIELD_CHANGE_SIGNALS["project"] = self.SIG_MODEL_CHANGED
```

### Comparing `PyPlanning-2.0.0/planning/locale/fr/LC_MESSAGES/planning.mo` & `pyplanning-2.0.1/planning/locale/fr/LC_MESSAGES/planning.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -227,15 +227,15 @@
 msgstr "Mettre à jour à la date d'aujourd'hui"
 
 msgid "Set the %s environment variable to 1, 2 or 3"
 msgstr ""
 "Définir la variable d'environnement %s et lui affecter la valeur 1, 2 ou 3"
 
 msgid "Show description"
-msgstr "Afficher la des description"
+msgstr "Afficher la description"
 
 msgid "Show log files..."
 msgstr "Afficher les journaux de bords..."
 
 msgid "Start"
 msgstr "Début"
```

### Comparing `PyPlanning-2.0.0/planning/model.py` & `pyplanning-2.0.1/planning/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from enum import Enum, IntEnum, StrEnum
 from io import StringIO
 from typing import Any, Generator, Generic, Optional, TypeVar, Union
 
 from planning import __version__, gantt
 from planning.config import MAIN_FONT_FAMILY, _
 
+locale.setlocale(locale.LC_TIME, "")
+
 VERSION = ".".join(__version__.split(".", 2)[0:2])
 
 gantt.define_font_attributes(
     fill="black", stroke="black", stroke_width=0, font_family=MAIN_FONT_FAMILY
 )
 
 _T = TypeVar("_T")
@@ -65,15 +67,16 @@
 class NoDefault:
     """No default value"""
 
 
 class DataItem(Generic[_T]):
     """Data elementary item"""
 
-    COLORS = {
+    COLORS: dict[str, str | None] = {
+        "": None,
         "orange": "#fab978",
         "red": "#e47172",
         "blue": "#53ccff",
         "yellow": "#ffd966",
         "cyan": "#c6eeff",
         "silver": "#9c9ea0",
         "green": "#b0d184",
@@ -303,15 +306,15 @@
         raise NotImplementedError(f"Unsupported datatype {self.datatype}")
 
     def from_text(self, text: str):
         """Set data item value from text"""
         if self.datatype == DTypes.COLOR:
             self.value = self.get_html_color(text)
         elif self.datatype == DTypes.TEXT or self.datatype == DTypes.LONG_TEXT:
-            self.value = None if len(text) == 0 else text
+            self.value = None if len(text) == 0 else text.strip()
         elif self.datatype == DTypes.INTEGER:
             self.value = None if text == "" else int(text)
         elif self.datatype == DTypes.LIST:
             if text == "":
                 self.value = []
             else:
                 values = text.split(",")
@@ -348,15 +351,15 @@
     """Abstract data set (associated with an XML element)"""
 
     TAG = None
     DEFAULT_ICON_NAME = None
     DEFAULT_NAME = None
     DEFAULT_COLOR = None
     READ_ONLY_ITEMS = ()
-    NO_COPY: tuple[str, ...] = ("pdata",)
+    __NO_COPY: tuple[str, ...] = ("pdata",)
     DEFAULT_ID_PREFIX = "default"
 
     def __init__(self, pdata: "PlanningData", name=None, fullname=None):
         self.pdata = pdata
         self.element = None
         if name is None:
             name = self.DEFAULT_NAME
@@ -380,29 +383,37 @@
     def default_id(self) -> str:
         if self._default_id == "" and self.pdata is not None:
             self._default_id = self.create_id()
         return self._default_id
 
     def duplicate(self):
         """Duplicate data set"""
-        new_item = deepcopy(self)
-        new_item.pdata = self.pdata
-        new_item.id.value = new_item.default_id
-        return new_item
-
-    def __deepcopy__(self, memo):
-        """Deepcopy method"""
         cls = self.__class__
-        obj = cls.__new__(cls)
-        memo[id(self)] = obj
-        for k, v in self.__dict__.items():
-            if k in self.NO_COPY:
-                v = dict()
-            setattr(obj, k, deepcopy(v, memo))
-        return obj
+        new_data = cls.__new__(cls)
+        for name, value in self.__dict__.items():
+            if name in self.__NO_COPY and value:
+                setattr(new_data, name, value)
+                continue
+            copied_value = deepcopy(value)
+            if isinstance(copied_value, DataItem):
+                copied_value.parent = new_data
+            setattr(new_data, name, copied_value)
+
+        copy_pattern = re.compile(r"\((\d+)\)$")
+        if re.search(copy_pattern, str(new_data.name.value)):
+            new_data.name.value = re.sub(
+                copy_pattern,
+                lambda m: f"({int(m.group(1)) + 1})",
+                str(new_data.name.value),
+            )
+        else:
+            new_data.name.value = f"{new_data.name.value} (1)"
+
+        new_data.id.value = new_data.create_id()
+        return new_data
 
     @property
     def gantt_object(
         self,
     ) -> gantt.Resource | gantt.Task | gantt.Milestone | gantt.Project | None:
         """Return associated gantt object"""
         return self.__gantt_object
@@ -839,14 +850,15 @@
             # choices=[(self.task_number.value, self.name.value)],
             # default_choice_mode=DefaultChoiceMode.NONE,
         )
         self.update_project_choice()
 
     def duplicate(self):
         new_item = super().duplicate()
+        new_item.task_number.value = None
         return new_item
 
     def _init_from_element(self, element):
         """Init instance from XML element"""
         super()._init_from_element(element)
         self.depends_on: DataItem[list[str]] = self.get_list("depends_on")
         # self.percent_done: DataItem[int] = self.get_int("percent_done")
@@ -1367,28 +1379,31 @@
             self.add_chart(chtdata)
         tasks_elt = self.element.find(tasks_tag)
         for elem in tasks_elt.findall(ResourceData.TAG):
             resdata = ResourceData.from_element(self, elem)
             resid = resdata.id.value
             self.add_resource(resdata)
             for telem in resdata.element:
+                # Tasks attributed to a resource (direct children to RESOURCE)
                 if telem.tag == TaskData.TAG:
                     data = TaskData.from_element(self, telem)
                     data.set_resource_ids([resid])
                     self.add_task(data)
                 elif telem.tag == LeaveData.TAG:
                     data = LeaveData.from_element(self, telem)
                     data.set_resource_id(resid)
                     self.add_leave(data)
-        for elem in tasks_elt.findall(TaskData.TAG):
-            data = TaskData.from_element(self, elem)
-            self.add_task(data)
-        for elem in tasks_elt.findall(MilestoneData.TAG):
-            data = MilestoneData.from_element(self, elem)
-            self.add_task(data)
+        # Tasks not attributed to a resource (direct children to TASKS)
+        for elem in tasks_elt:
+            if elem.tag == TaskData.TAG:
+                data = TaskData.from_element(self, elem)
+                self.add_task(data)
+            elif elem.tag == MilestoneData.TAG:
+                data = MilestoneData.from_element(self, elem)
+                self.add_task(data)
         cdays_elt = self.element.find("CLOSINGDAYS")
         if cdays_elt is not None:
             for elem in cdays_elt.findall(ClosingDayData.TAG):
                 data = ClosingDayData.from_element(self, elem)
                 self.add_closing_day(data)
         for data in self.iterate_task_data():
             data.update_task_choices()
@@ -1592,15 +1607,15 @@
 
     def add_task(
         self, data: AbstractTaskData, after_data: Optional[AbstractData] = None
     ):
         """Add task/milestone to planning"""
         index = None
         task_number_index = None
-        if isinstance(after_data, TaskData):
+        if isinstance(after_data, AbstractTaskData):
             index = task_number_index = self.tsklist.index(after_data)
         elif isinstance(after_data, ResourceData):
             # Sum all task indexes for all resources before:
             resids = []
             for res in self.reslist:
                 if res is after_data:
                     break
```

### Comparing `PyPlanning-2.0.0/planning/tests/test_central_widget.py` & `pyplanning-2.0.1/planning/tests/test_central_widget.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_gantt.py` & `pyplanning-2.0.1/planning/tests/test_gantt.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_model.py` & `pyplanning-2.0.1/planning/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_treewidgets.py` & `pyplanning-2.0.1/planning/tests/test_treewidgets.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_v1_02.svg` & `pyplanning-2.0.1/planning/tests/test_v1_02.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_v1_03.svg` & `pyplanning-2.0.1/planning/tests/test_v1_03.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_v2_01.svg` & `pyplanning-2.0.1/planning/tests/test_v2_01.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_v2_02.svg` & `pyplanning-2.0.1/planning/tests/test_v2_02.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/tests/test_v2_03.svg` & `pyplanning-2.0.1/planning/tests/test_v2_03.svg`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/utils/conf.py` & `pyplanning-2.0.1/planning/utils/conf.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/planning/utils/qthelpers.py` & `pyplanning-2.0.1/planning/utils/qthelpers.py`

 * *Files identical despite different names*

### Comparing `PyPlanning-2.0.0/pyproject.toml` & `pyplanning-2.0.1/pyproject.toml`

 * *Files identical despite different names*

