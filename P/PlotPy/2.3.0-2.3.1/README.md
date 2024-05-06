# Comparing `tmp/PlotPy-2.3.0.tar.gz` & `tmp/plotpy-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlotPy-2.3.0.tar", last modified: Mon Mar 11 08:19:18 2024, max compression
+gzip compressed data, was "plotpy-2.3.1.tar", last modified: Mon May  6 16:41:15 2024, max compression
```

## Comparing `PlotPy-2.3.0.tar` & `plotpy-2.3.1.tar`

### file list

```diff
@@ -1,565 +1,577 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.977071 PlotPy-2.3.0/
--rw-rw-rw-   0        0        0     1563 2023-11-23 17:46:00.000000 PlotPy-2.3.0/LICENSE
--rw-rw-rw-   0        0        0       57 2023-11-23 17:46:00.000000 PlotPy-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8168 2024-03-11 08:19:18.977071 PlotPy-2.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.977071 PlotPy-2.3.0/PlotPy.egg-info/
--rw-rw-rw-   0        0        0     8168 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16572 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      231 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-11 08:19:16.000000 PlotPy-2.3.0/PlotPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4379 2023-11-23 17:46:00.000000 PlotPy-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.258324 PlotPy-2.3.0/doc/
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.273943 PlotPy-2.3.0/doc/_static/
--rw-rw-rw-   0        0        0   110568 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0       79 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/changelog.rst
--rw-rw-rw-   0        0        0     2273 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.320825 PlotPy-2.3.0/doc/dev/
--rw-rw-rw-   0        0        0     1083 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/dev/build.rst
--rw-rw-rw-   0        0        0     4381 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0     3108 2024-02-09 17:39:23.000000 PlotPy-2.3.0/doc/dev/guiqwt_to_plotpy.csv
--rw-rw-rw-   0        0        0     9868 2024-02-16 08:53:28.000000 PlotPy-2.3.0/doc/dev/guiqwt_to_plotpy.rst
--rw-rw-rw-   0        0        0      158 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/dev/index.rst
--rw-rw-rw-   0        0        0     5053 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/dev/platforms.rst
--rw-rw-rw-   0        0        0      389 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/dev/v1_to_guidata_v3.csv
--rw-rw-rw-   0        0        0     2489 2024-02-09 17:39:23.000000 PlotPy-2.3.0/doc/dev/v1_to_v2.csv
--rw-rw-rw-   0        0        0     3374 2024-02-16 08:53:28.000000 PlotPy-2.3.0/doc/dev/v1_to_v2.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.367698 PlotPy-2.3.0/doc/features/
--rw-rw-rw-   0        0        0       41 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/colormapmanager.rst
--rw-rw-rw-   0        0        0       31 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/events.rst
--rw-rw-rw-   0        0        0       36 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/fit.rst
--rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/fliprotate.rst
--rw-rw-rw-   0        0        0       42 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/imagefile.rst
--rw-rw-rw-   0        0        0      327 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/index.rst
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/io.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.398948 PlotPy-2.3.0/doc/features/items/
--rw-rw-rw-   0        0        0      784 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/items/builder.rst
--rw-rw-rw-   0        0        0     4830 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/items/examples.rst
--rw-rw-rw-   0        0        0      149 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/items/index.rst
--rw-rw-rw-   0        0        0     2311 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/items/overview.rst
--rw-rw-rw-   0        0        0     3319 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/items/reference.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.414578 PlotPy-2.3.0/doc/features/mathutils/
--rw-rw-rw-   0        0        0       41 2024-02-09 17:39:23.000000 PlotPy-2.3.0/doc/features/mathutils/colormaps.rst
--rw-rw-rw-   0        0        0       41 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/mathutils/geometry.rst
--rw-rw-rw-   0        0        0      119 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/mathutils/index.rst
--rw-rw-rw-   0        0        0       39 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/mathutils/scaler.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.430193 PlotPy-2.3.0/doc/features/panels/
--rw-rw-rw-   0        0        0      127 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/panels/index.rst
--rw-rw-rw-   0        0        0      891 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/panels/overview.rst
--rw-rw-rw-   0        0        0      212 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/panels/reference.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.445819 PlotPy-2.3.0/doc/features/plot/
--rw-rw-rw-   0        0        0     1012 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/plot/examples.rst
--rw-rw-rw-   0        0        0     1560 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/plot/index.rst
--rw-rw-rw-   0        0        0     1150 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/plot/overview.rst
--rw-rw-rw-   0        0        0      625 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/plot/reference.rst
--rw-rw-rw-   0        0        0       51 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/pyplot.rst
--rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/resizedialog.rst
--rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/rotatecrop.rst
--rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/selectdialog.rst
--rw-rw-rw-   0        0        0     1754 2024-03-04 12:33:14.000000 PlotPy-2.3.0/doc/features/signals.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.461446 PlotPy-2.3.0/doc/features/styles/
--rw-rw-rw-   0        0        0      157 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/styles/index.rst
--rw-rw-rw-   0        0        0      540 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/styles/overview.rst
--rw-rw-rw-   0        0        0     1921 2024-02-08 10:33:36.000000 PlotPy-2.3.0/doc/features/styles/reference.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.492688 PlotPy-2.3.0/doc/features/tools/
--rw-rw-rw-   0        0        0      289 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/tools/examples.rst
--rw-rw-rw-   0        0        0      137 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/features/tools/index.rst
--rw-rw-rw-   0        0        0     2747 2024-03-11 08:11:54.000000 PlotPy-2.3.0/doc/features/tools/overview.rst
--rw-rw-rw-   0        0        0     3717 2024-03-11 08:11:54.000000 PlotPy-2.3.0/doc/features/tools/reference.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.570814 PlotPy-2.3.0/doc/images/
--rw-rw-rw-   0        0        0    42675 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/my_plot_manager.png
--rw-rw-rw-   0        0        0    31164 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/my_plot_manager.svg
--rw-rw-rw-   0        0        0   240381 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/panorama.png
--rw-rw-rw-   0        0        0  1914412 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/panorama.svg
--rw-rw-rw-   0        0        0    55886 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/plot_widgets.png
--rw-rw-rw-   0        0        0    30549 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/plot_widgets.svg
--rw-rw-rw-   0        0        0     9809 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/plotpy-banner.png
--rw-rw-rw-   0        0        0     7460 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/plotpy-vertical.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.602064 PlotPy-2.3.0/doc/images/screenshots/
--rw-rw-rw-   0        0        0    64597 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0    37530 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/computations.png
--rw-rw-rw-   0        0        0   179050 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/contrast.png
--rw-rw-rw-   0        0        0   210107 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/cross_section.png
--rw-rw-rw-   0        0        0   210494 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/cross_section2.png
--rw-rw-rw-   0        0        0    81254 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/dotarraydemo.png
--rw-rw-rw-   0        0        0    41879 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/filtertest1.png
--rw-rw-rw-   0        0        0    49232 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/filtertest2.png
--rw-rw-rw-   0        0        0    44646 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/fit.png
--rw-rw-rw-   0        0        0    32653 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/get_point.png
--rw-rw-rw-   0        0        0    77053 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/hist2d.png
--rw-rw-rw-   0        0        0   269545 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/image_plot_tools.png
--rw-rw-rw-   0        0        0   230644 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/imagefilter.png
--rw-rw-rw-   0        0        0   163887 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/imagesuperp.png
--rw-rw-rw-   0        0        0   143730 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/imagexy.png
--rw-rw-rw-   0        0        0   168112 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/manager.png
--rw-rw-rw-   0        0        0   231418 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/mandelbrot.png
--rw-rw-rw-   0        0        0   172858 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/pcolor.png
--rw-rw-rw-   0        0        0    76448 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/plot.png
--rw-rw-rw-   0        0        0   173690 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/simple_dialog.png
--rw-rw-rw-   0        0        0    59433 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/simple_window.png
--rw-rw-rw-   0        0        0   456556 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/images/screenshots/transform.png
--rw-rw-rw-   0        0        0     1651 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/index.rst
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.633316 PlotPy-2.3.0/doc/intro/
--rw-rw-rw-   0        0        0     2862 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/examples.rst
--rw-rw-rw-   0        0        0      164 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/index.rst
--rw-rw-rw-   0        0        0      675 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/installation.rst
--rw-rw-rw-   0        0        0   107599 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/licenses.rst
--rw-rw-rw-   0        0        0     2309 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/motivation.rst
--rw-rw-rw-   0        0        0     4815 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/intro/overview.rst
--rw-rw-rw-   0        0        0     2429 2024-03-11 08:11:54.000000 PlotPy-2.3.0/doc/requirements.rst
--rw-rw-rw-   0        0        0      721 2023-11-23 17:46:00.000000 PlotPy-2.3.0/doc/update_requirements.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.711442 PlotPy-2.3.0/plotpy/
--rw-rw-rw-   0        0        0     1053 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.789568 PlotPy-2.3.0/plotpy/builder/
--rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/builder/__init__.py
--rw-rw-rw-   0        0        0    13033 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/builder/annotation.py
--rw-rw-rw-   0        0        0    31776 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/builder/curvemarker.py
--rw-rw-rw-   0        0        0    33708 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/builder/image.py
--rw-rw-rw-   0        0        0    10062 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/builder/label.py
--rw-rw-rw-   0        0        0    17119 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/builder/plot.py
--rw-rw-rw-   0        0        0     5886 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/builder/shape.py
--rw-rw-rw-   0        0        0    34344 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/config.py
--rw-rw-rw-   0        0        0     4756 2024-02-16 08:53:28.000000 PlotPy-2.3.0/plotpy/constants.py
--rw-rw-rw-   0        0        0     2385 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/coords.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.820820 PlotPy-2.3.0/plotpy/data/
--rw-rw-rw-   0        0        0   328300 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/colormaps_default.json
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.992694 PlotPy-2.3.0/plotpy/data/icons/
--rw-rw-rw-   0        0        0      595 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/apply.png
--rw-rw-rw-   0        0        0      897 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/arredit.png
--rw-rw-rw-   0        0        0      637 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/arrow_down.png
--rw-rw-rw-   0        0        0      638 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/arrow_up.png
--rw-rw-rw-   0        0        0      868 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/autorefresh.png
--rw-rw-rw-   0        0        0     1012 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/autoscale.png
--rw-rw-rw-   0        0        0      513 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/axes.png
--rw-rw-rw-   0        0        0      474 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/busy.png
--rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/cell_edit.png
--rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/center.png
--rw-rw-rw-   0        0        0      495 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/cmap_edit.png
--rw-rw-rw-   0        0        0      316 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/contrast.png
--rw-rw-rw-   0        0        0      620 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/copy.png
--rw-rw-rw-   0        0        0      979 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/copytoclipboard.png
--rw-rw-rw-   0        0        0      705 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csapplylut.png
--rw-rw-rw-   0        0        0      178 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csautoscale.png
--rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csection.png
--rw-rw-rw-   0        0        0      310 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csection_a.png
--rw-rw-rw-   0        0        0      375 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csection_line.png
--rw-rw-rw-   0        0        0      711 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csection_oblique.png
--rw-rw-rw-   0        0        0      160 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/csperimage.png
--rw-rw-rw-   0        0        0      758 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curve_downsample.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.008314 PlotPy-2.3.0/plotpy/data/icons/curvestyles/
--rw-rw-rw-   0        0        0      121 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvestyles/dots.png
--rw-rw-rw-   0        0        0      164 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvestyles/lines.png
--rw-rw-rw-   0        0        0      136 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvestyles/steps.png
--rw-rw-rw-   0        0        0      187 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvestyles/sticks.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.008314 PlotPy-2.3.0/plotpy/data/icons/curvetypes/
--rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvetypes/xfy.png
--rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/curvetypes/yfx.png
--rw-rw-rw-   0        0        0      496 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/delete.png
--rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/edit.png
--rw-rw-rw-   0        0        0      793 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/edit_point_selection.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.039566 PlotPy-2.3.0/plotpy/data/icons/editors/
--rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/edit.png
--rw-rw-rw-   0        0        0      790 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/edit_add.png
--rw-rw-rw-   0        0        0      837 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/editcopy.png
--rw-rw-rw-   0        0        0     1242 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/editdelete.png
--rw-rw-rw-   0        0        0     1084 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/editpaste.png
--rw-rw-rw-   0        0        0     2065 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/fileimport.png
--rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/filesave.png
--rw-rw-rw-   0        0        0      516 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/imshow.png
--rw-rw-rw-   0        0        0      314 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/insert.png
--rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/plot.png
--rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/editors/rename.png
--rw-rw-rw-   0        0        0      183 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/eliminate_outliers.png
--rw-rw-rw-   0        0        0      671 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/eraser.png
--rw-rw-rw-   0        0        0      974 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/exit.png
--rw-rw-rw-   0        0        0      191 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/expander_down.png
--rw-rw-rw-   0        0        0      184 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/expander_right.png
--rw-rw-rw-   0        0        0      861 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/export.png
--rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/file.png
--rw-rw-rw-   0        0        0     1213 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/fileclose.png
--rw-rw-rw-   0        0        0     1383 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/fileimport.png
--rw-rw-rw-   0        0        0      271 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filenew.png
--rw-rw-rw-   0        0        0     1349 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/fileopen.png
--rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filesave.png
--rw-rw-rw-   0        0        0     1264 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filesaveas.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.148937 PlotPy-2.3.0/plotpy/data/icons/filetypes/
--rw-rw-rw-   0        0        0     1389 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/doc.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/gif.png
--rw-rw-rw-   0        0        0     1658 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/html.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1352 2024-03-04 13:28:35.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/png.png
--rw-rw-rw-   0        0        0     1226 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/pps.png
--rw-rw-rw-   0        0        0     1217 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/ps.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/tar.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/tif.png
--rw-rw-rw-   0        0        0     1609 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/txt.png
--rw-rw-rw-   0        0        0     1026 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/xls.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/filetypes/zip.png
--rw-rw-rw-   0        0        0      244 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/font.png
--rw-rw-rw-   0        0        0      185 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/full_range.png
--rw-rw-rw-   0        0        0      922 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/funct.png
--rw-rw-rw-   0        0        0      151 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/hcursor.png
--rw-rw-rw-   0        0        0      433 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/hflip.png
--rw-rw-rw-   0        0        0      793 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/imagestats.png
--rw-rw-rw-   0        0        0      437 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/item_list.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.148937 PlotPy-2.3.0/plotpy/data/icons/items/
--rw-rw-rw-   0        0        0      687 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/annotation.png
--rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/curve.png
--rw-rw-rw-   0        0        0      172 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/errorbar.png
--rw-rw-rw-   0        0        0      120 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/grid.png
--rw-rw-rw-   0        0        0      140 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/histogram.png
--rw-rw-rw-   0        0        0      857 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/histogram2d.png
--rw-rw-rw-   0        0        0      852 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/image.png
--rw-rw-rw-   0        0        0      531 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/label.png
--rw-rw-rw-   0        0        0      317 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/legend.png
--rw-rw-rw-   0        0        0      448 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/items/polygonmap.png
--rw-rw-rw-   0        0        0      673 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/magnifier.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.164563 PlotPy-2.3.0/plotpy/data/icons/markers/
--rw-rw-rw-   0        0        0      123 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/cross.png
--rw-rw-rw-   0        0        0      194 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/diamond.png
--rw-rw-rw-   0        0        0      241 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/ellipse.png
--rw-rw-rw-   0        0        0      260 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/hexagon.png
--rw-rw-rw-   0        0        0      105 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/point.png
--rw-rw-rw-   0        0        0      137 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/square.png
--rw-rw-rw-   0        0        0      160 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/star.png
--rw-rw-rw-   0        0        0      223 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/triangle_d.png
--rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/triangle_l.png
--rw-rw-rw-   0        0        0      212 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/triangle_r.png
--rw-rw-rw-   0        0        0      224 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/triangle_u.png
--rw-rw-rw-   0        0        0      145 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markers/xcross.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.164563 PlotPy-2.3.0/plotpy/data/icons/markerstyles/
--rw-rw-rw-   0        0        0       96 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markerstyles/cross_marker.png
--rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markerstyles/horiz_marker.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/markerstyles/vert_marker.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.164563 PlotPy-2.3.0/plotpy/data/icons/mask/
--rw-rw-rw-   0        0        0      368 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/mask/mask_circle.png
--rw-rw-rw-   0        0        0      374 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/mask/mask_circle_outside.png
--rw-rw-rw-   0        0        0      199 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/mask/mask_rectangle.png
--rw-rw-rw-   0        0        0      200 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/mask/mask_rectangle_outside.png
--rw-rw-rw-   0        0        0      164 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/mask/mask_tool.png
--rw-rw-rw-   0        0        0      130 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/max.png
--rw-rw-rw-   0        0        0      125 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/min.png
--rw-rw-rw-   0        0        0      132 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/move.png
--rw-rw-rw-   0        0        0      729 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/multipoint_selection.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/none.png
--rw-rw-rw-   0        0        0      284 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/not_found.png
--rw-rw-rw-   0        0        0      397 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/on_curve.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.180187 PlotPy-2.3.0/plotpy/data/icons/patterns/
--rw-rw-rw-   0        0        0      104 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/bdiagpattern.png
--rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/crosspattern.png
--rw-rw-rw-   0        0        0       76 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense1pattern.png
--rw-rw-rw-   0        0        0       78 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense2pattern.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense3pattern.png
--rw-rw-rw-   0        0        0       73 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense4pattern.png
--rw-rw-rw-   0        0        0       88 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense5pattern.png
--rw-rw-rw-   0        0        0       87 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense6pattern.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/dense7pattern.png
--rw-rw-rw-   0        0        0      114 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/diagcrosspattern.png
--rw-rw-rw-   0        0        0      112 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/fdiagpattern.png
--rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/horpattern.png
--rw-rw-rw-   0        0        0       74 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/nobrush.png
--rw-rw-rw-   0        0        0       69 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/solidpattern.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/patterns/verpattern.png
--rw-rw-rw-   0        0        0    17636 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/plotpy-banner.svg
--rw-rw-rw-   0        0        0    17614 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/plotpy-vertical.svg
--rw-rw-rw-   0        0        0    16339 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/plotpy.svg
--rw-rw-rw-   0        0        0      216 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/point_selection.png
--rw-rw-rw-   0        0        0      723 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/print.png
--rw-rw-rw-   0        0        0      697 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/python.png
--rw-rw-rw-   0        0        0      677 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/quickview.png
--rw-rw-rw-   0        0        0      823 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/rectangular_select.png
--rw-rw-rw-   0        0        0      740 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/refresh.png
--rw-rw-rw-   0        0        0     1428 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/save_all.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.180187 PlotPy-2.3.0/plotpy/data/icons/scales/
--rw-rw-rw-   0        0        0      203 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/scales/lin_lin.png
--rw-rw-rw-   0        0        0      208 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/scales/lin_log.png
--rw-rw-rw-   0        0        0      219 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/scales/log_lin.png
--rw-rw-rw-   0        0        0      222 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/scales/log_log.png
--rw-rw-rw-   0        0        0      518 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/selection.png
--rw-rw-rw-   0        0        0      851 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/settings.png
--rw-rw-rw-   0        0        0      135 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shape.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.195813 PlotPy-2.3.0/plotpy/data/icons/shapes/
--rw-rw-rw-   0        0        0      530 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/circle.png
--rw-rw-rw-   0        0        0      622 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/contour.png
--rw-rw-rw-   0        0        0      547 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/ellipse_shape.png
--rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/freeform.png
--rw-rw-rw-   0        0        0      321 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/gtaxes.png
--rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/marker.png
--rw-rw-rw-   0        0        0      650 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/oblique_rectangle.png
--rw-rw-rw-   0        0        0      118 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/point_shape.png
--rw-rw-rw-   0        0        0      232 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/polyline.png
--rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/rectangle.png
--rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/shapes/segment.png
--rw-rw-rw-   0        0        0     1150 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/snapshot.png
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.195813 PlotPy-2.3.0/plotpy/data/icons/styles/
--rw-rw-rw-   0        0        0       85 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/styles/dash.png
--rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/styles/dashdot.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/styles/dashdotdot.png
--rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/styles/dot.png
--rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/styles/solid.png
--rw-rw-rw-   0        0        0      236 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/trash.png
--rw-rw-rw-   0        0        0      932 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/trimage_lock.png
--rw-rw-rw-   0        0        0      958 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/trimage_unlock.png
--rw-rw-rw-   0        0        0      159 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/vcursor.png
--rw-rw-rw-   0        0        0      432 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/vflip.png
--rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/xcursor.png
--rw-rw-rw-   0        0        0      128 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/xmax.png
--rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/xmin.png
--rw-rw-rw-   0        0        0      170 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/data/icons/xrange.png
--rw-rw-rw-   0        0        0    46755 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/events.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.211440 PlotPy-2.3.0/plotpy/external/
--rw-rw-rw-   0        0        0      399 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.242699 PlotPy-2.3.0/plotpy/external/sliders/
--rw-rw-rw-   0        0        0     2108 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/sliders/__init__.py
--rw-rw-rw-   0        0        0    14101 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/sliders/_generic_range_slider.py
--rw-rw-rw-   0        0        0    20447 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/sliders/_generic_slider.py
--rw-rw-rw-   0        0        0    24034 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/sliders/_labeled.py
--rw-rw-rw-   0        0        0      758 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/external/sliders/_misc.py
--rw-rw-rw-   0        0        0     9829 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/external/sliders/_range_style.py
--rw-rw-rw-   0        0        0     1126 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/external/sliders/_sliders.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.273943 PlotPy-2.3.0/plotpy/interfaces/
--rw-rw-rw-   0        0        0      517 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/interfaces/__init__.py
--rw-rw-rw-   0        0        0    14685 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/interfaces/items.py
--rw-rw-rw-   0        0        0      461 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/interfaces/panel.py
--rw-rw-rw-   0        0        0     1049 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/interfaces/plotmanager.py
--rw-rw-rw-   0        0        0    24064 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/io.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.320823 PlotPy-2.3.0/plotpy/items/
--rw-rw-rw-   0        0        0     1517 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/items/__init__.py
--rw-rw-rw-   0        0        0    30198 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/annotation.py
--rw-rw-rw-   0        0        0     6355 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/items/contour.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.336448 PlotPy-2.3.0/plotpy/items/curve/
--rw-rw-rw-   0        0        0      176 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/items/curve/__init__.py
--rw-rw-rw-   0        0        0    18860 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/curve/base.py
--rw-rw-rw-   0        0        0    12987 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/curve/errorbar.py
--rw-rw-rw-   0        0        0     7632 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/grid.py
--rw-rw-rw-   0        0        0     7118 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/histogram.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.398953 PlotPy-2.3.0/plotpy/items/image/
--rw-rw-rw-   0        0        0      608 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/items/image/__init__.py
--rw-rw-rw-   0        0        0    44532 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/base.py
--rw-rw-rw-   0        0        0    11447 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/filter.py
--rw-rw-rw-   0        0        0    28332 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/image_items.py
--rw-rw-rw-   0        0        0    24911 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/masked.py
--rw-rw-rw-   0        0        0    25205 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/misc.py
--rw-rw-rw-   0        0        0    23529 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/image/transform.py
--rw-rw-rw-   0        0        0    32674 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/label.py
--rw-rw-rw-   0        0        0    13551 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/polygonmap.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.539569 PlotPy-2.3.0/plotpy/items/shape/
--rw-rw-rw-   0        0        0      457 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/items/shape/__init__.py
--rw-rw-rw-   0        0        0     9972 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/axis.py
--rw-rw-rw-   0        0        0     8592 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/base.py
--rw-rw-rw-   0        0        0    11893 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/ellipse.py
--rw-rw-rw-   0        0        0    16554 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/marker.py
--rw-rw-rw-   0        0        0     2611 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/point.py
--rw-rw-rw-   0        0        0    14718 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/polygon.py
--rw-rw-rw-   0        0        0     9701 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/range.py
--rw-rw-rw-   0        0        0    11459 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/rectangle.py
--rw-rw-rw-   0        0        0     4581 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/items/shape/segment.py
--rw-rw-rw-   0        0        0     4619 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/items/shape/svg.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.164563 PlotPy-2.3.0/plotpy/locale/
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:16.164563 PlotPy-2.3.0/plotpy/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.539569 PlotPy-2.3.0/plotpy/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    32854 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/locale/fr/LC_MESSAGES/plotpy.mo
--rw-rw-rw-   0        0        0     1918 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/lutrange.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.570819 PlotPy-2.3.0/plotpy/mathutils/
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/mathutils/__init__.py
--rw-rw-rw-   0        0        0     1739 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/mathutils/arrayfuncs.py
--rw-rw-rw-   0        0        0    10325 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/mathutils/colormap.py
--rw-rw-rw-   0        0        0     6803 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/mathutils/geometry.py
--rw-rw-rw-   0        0        0     1892 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/mathutils/scaler.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.617706 PlotPy-2.3.0/plotpy/panels/
--rw-rw-rw-   0        0        0      270 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/panels/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/panels/base.py
--rw-rw-rw-   0        0        0    19745 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/panels/contrastadjustment.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.648940 PlotPy-2.3.0/plotpy/panels/csection/
--rw-rw-rw-   0        0        0      480 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/panels/csection/__init__.py
--rw-rw-rw-   0        0        0    16970 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/panels/csection/csitem.py
--rw-rw-rw-   0        0        0    16887 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/panels/csection/csplot.py
--rw-rw-rw-   0        0        0    12868 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/panels/csection/cswidget.py
--rw-rw-rw-   0        0        0     9425 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/panels/itemlist.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.695819 PlotPy-2.3.0/plotpy/plot/
--rw-rw-rw-   0        0        0      325 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/plot/__init__.py
--rw-rw-rw-   0        0        0    85106 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/plot/base.py
--rw-rw-rw-   0        0        0    22002 2024-02-09 17:39:23.000000 PlotPy-2.3.0/plotpy/plot/interactive.py
--rw-rw-rw-   0        0        0    25295 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/plot/manager.py
--rw-rw-rw-   0        0        0    34516 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/plot/plotwidget.py
--rw-rw-rw-   0        0        0     2762 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/pyplot.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.758340 PlotPy-2.3.0/plotpy/styles/
--rw-rw-rw-   0        0        0     1738 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/styles/__init__.py
--rw-rw-rw-   0        0        0     4155 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/styles/axes.py
--rw-rw-rw-   0        0        0    19338 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/base.py
--rw-rw-rw-   0        0        0     3172 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/curve.py
--rw-rw-rw-   0        0        0     1552 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/styles/errorbar.py
--rw-rw-rw-   0        0        0     3896 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/histogram.py
--rw-rw-rw-   0        0        0    18053 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/image.py
--rw-rw-rw-   0        0        0     8365 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/styles/label.py
--rw-rw-rw-   0        0        0     1631 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/polygonmap.py
--rw-rw-rw-   0        0        0    13088 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/styles/shape.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.852069 PlotPy-2.3.0/plotpy/tests/
--rw-rw-rw-   0        0        0      698 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:17.883332 PlotPy-2.3.0/plotpy/tests/benchmarks/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/benchmarks/__init__.py
--rw-rw-rw-   0        0        0     4226 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/benchmarks/test_benchmarks.py
--rw-rw-rw-   0        0        0      836 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/benchmarks/test_bigimages.py
--rw-rw-rw-   0        0        0     2847 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/benchmarks/test_loadtest.py
--rw-rw-rw-   0        0        0      189 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.008319 PlotPy-2.3.0/plotpy/tests/data/
--rw-rw-rw-   0        0        0    39666 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data/brain.png
--rw-rw-rw-   0        0        0    35354 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data/brain_cylinder.png
--rw-rw-rw-   0        0        0   525620 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data/mr-brain.dcm
--rw-rw-rw-   0        0        0     1991 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data/svg_target.svg
--rw-rw-rw-   0        0        0     1765 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data/svg_tool.svg
--rw-rw-rw-   0        0        0     4363 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/data.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.148941 PlotPy-2.3.0/plotpy/tests/features/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/__init__.py
--rw-rw-rw-   0        0        0      906 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_auto_curve_image.py
--rw-rw-rw-   0        0        0     2619 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_autoscale_shapes.py
--rw-rw-rw-   0        0        0     1660 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_builder.py
--rw-rw-rw-   0        0        0     3014 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/features/test_colormap_editor.py
--rw-rw-rw-   0        0        0     1501 2024-02-09 17:39:23.000000 PlotPy-2.3.0/plotpy/tests/features/test_colormap_manager.py
--rw-rw-rw-   0        0        0     1381 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_computations.py
--rw-rw-rw-   0        0        0     1275 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_contrast.py
--rw-rw-rw-   0        0        0     1064 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_cursors.py
--rw-rw-rw-   0        0        0     1164 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_dicom_image.py
--rw-rw-rw-   0        0        0      798 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_fit.py
--rw-rw-rw-   0        0        0     1483 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_image_coords.py
--rw-rw-rw-   0        0        0     1587 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_imagefilter.py
--rw-rw-rw-   0        0        0     1576 2024-02-16 08:53:28.000000 PlotPy-2.3.0/plotpy/tests/features/test_imagesuperp.py
--rw-rw-rw-   0        0        0     1116 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_hdf5.py
--rw-rw-rw-   0        0        0     1453 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_json.py
--rw-rw-rw-   0        0        0     6395 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_pickle.py
--rw-rw-rw-   0        0        0     3123 2023-12-14 19:00:47.000000 PlotPy-2.3.0/plotpy/tests/features/test_manager.py
--rw-rw-rw-   0        0        0      718 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_no_auto_tools.py
--rw-rw-rw-   0        0        0      927 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_plot_log.py
--rw-rw-rw-   0        0        0     1214 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_plot_types.py
--rw-rw-rw-   0        0        0      846 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_plot_yreverse.py
--rw-rw-rw-   0        0        0     2114 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_pyplot.py
--rw-rw-rw-   0        0        0      694 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/features/test_resize.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.227077 PlotPy-2.3.0/plotpy/tests/items/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/__init__.py
--rw-rw-rw-   0        0        0     1159 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_annotations.py
--rw-rw-rw-   0        0        0     1493 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_curves.py
--rw-rw-rw-   0        0        0     2298 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_hist2d.py
--rw-rw-rw-   0        0        0      710 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_histogram.py
--rw-rw-rw-   0        0        0      840 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image.py
--rw-rw-rw-   0        0        0      989 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image_contour.py
--rw-rw-rw-   0        0        0     1231 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image_masked.py
--rw-rw-rw-   0        0        0     1336 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image_masked_xy.py
--rw-rw-rw-   0        0        0      759 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image_rgb.py
--rw-rw-rw-   0        0        0      758 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_image_xy.py
--rw-rw-rw-   0        0        0     2763 2023-12-14 19:00:47.000000 PlotPy-2.3.0/plotpy/tests/items/test_mandelbrot.py
--rw-rw-rw-   0        0        0     2340 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_pcolor.py
--rw-rw-rw-   0        0        0     2363 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/tests/items/test_polygons.py
--rw-rw-rw-   0        0        0      906 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_svgshapes.py
--rw-rw-rw-   0        0        0     6217 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/items/test_transform.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.336453 PlotPy-2.3.0/plotpy/tests/tools/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/test_actiontool.py
--rw-rw-rw-   0        0        0     1151 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/test_cross_section.py
--rw-rw-rw-   0        0        0     2466 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_cross_section_line.py
--rw-rw-rw-   0        0        0     1097 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_cross_section_oblique.py
--rw-rw-rw-   0        0        0     1804 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/test_customize_shape_tool.py
--rw-rw-rw-   0        0        0     1692 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_downsample_curve.py
--rw-rw-rw-   0        0        0     2865 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_edit_point.py
--rw-rw-rw-   0        0        0     1757 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_get_point.py
--rw-rw-rw-   0        0        0     2215 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_get_points.py
--rw-rw-rw-   0        0        0     1118 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/test_get_rectangle.py
--rw-rw-rw-   0        0        0     1741 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/tools/test_get_rectangle_with_svg.py
--rw-rw-rw-   0        0        0     1983 2024-02-08 12:52:10.000000 PlotPy-2.3.0/plotpy/tests/tools/test_get_segment.py
--rw-rw-rw-   0        0        0     2155 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/tools/test_image_plot_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.508317 PlotPy-2.3.0/plotpy/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1151 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_aspect_ratio_tool.py
--rw-rw-rw-   0        0        0     2183 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_baseplot.py
--rw-rw-rw-   0        0        0     2728 2024-02-08 11:53:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_builder_annotation.py
--rw-rw-rw-   0        0        0     6112 2024-02-08 11:53:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_builder_curve.py
--rw-rw-rw-   0        0        0     3291 2024-02-16 08:53:28.000000 PlotPy-2.3.0/plotpy/tests/unit/test_builder_image.py
--rw-rw-rw-   0        0        0     1700 2024-02-08 11:53:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_builder_shape.py
--rw-rw-rw-   0        0        0     2352 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_contour.py
--rw-rw-rw-   0        0        0     1111 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_display_coords_tool.py
--rw-rw-rw-   0        0        0      415 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_fontparam.py
--rw-rw-rw-   0        0        0     2840 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_geometry.py
--rw-rw-rw-   0        0        0      937 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_highprecisionxy.py
--rw-rw-rw-   0        0        0     3234 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_io.py
--rw-rw-rw-   0        0        0     1702 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_line.py
--rw-rw-rw-   0        0        0      888 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_line_cross_section_tool.py
--rw-rw-rw-   0        0        0     1783 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_multiline_tools.py
--rw-rw-rw-   0        0        0      909 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_oblique_cross_section_tool.py
--rw-rw-rw-   0        0        0     2368 2024-02-08 11:53:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_plot_curve.py
--rw-rw-rw-   0        0        0     4735 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_plot_image.py
--rw-rw-rw-   0        0        0     5692 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_point_tools.py
--rw-rw-rw-   0        0        0     2165 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tests/unit/test_rect_zoom.py
--rw-rw-rw-   0        0        0      839 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_seg_dist.py
--rw-rw-rw-   0        0        0     4861 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/unit/test_shape_tools.py
--rw-rw-rw-   0        0        0     3032 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_styles.py
--rw-rw-rw-   0        0        0      854 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/unit/test_tools_export.py
--rw-rw-rw-   0        0        0     5307 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/unit/utils.py
--rw-rw-rw-   0        0        0     1320 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/vistools.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.617705 PlotPy-2.3.0/plotpy/tests/widgets/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/__init__.py
--rw-rw-rw-   0        0        0     6919 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_dotarraydemo.py
--rw-rw-rw-   0        0        0     2711 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_filtertest1.py
--rw-rw-rw-   0        0        0     3517 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_filtertest2.py
--rw-rw-rw-   0        0        0     2220 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_fliprotate.py
--rw-rw-rw-   0        0        0    14422 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_plot_timecurve.py
--rw-rw-rw-   0        0        0     1185 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_qtdesigner.py
--rw-rw-rw-   0        0        0      763 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_qtdesigner.ui
--rw-rw-rw-   0        0        0     2201 2024-02-08 11:53:54.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_resize_dialog.py
--rw-rw-rw-   0        0        0     2906 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_rotatecrop.py
--rw-rw-rw-   0        0        0     3740 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_simple_dialog.py
--rw-rw-rw-   0        0        0    10267 2023-12-14 19:00:47.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_simple_window.py
--rw-rw-rw-   0        0        0     2875 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tests/widgets/test_syncplot.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.805190 PlotPy-2.3.0/plotpy/tools/
--rw-rw-rw-   0        0        0     1993 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tools/__init__.py
--rw-rw-rw-   0        0        0     1945 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/annotation.py
--rw-rw-rw-   0        0        0     3382 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/axes.py
--rw-rw-rw-   0        0        0    13497 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/tools/base.py
--rw-rw-rw-   0        0        0     4654 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tools/cross_section.py
--rw-rw-rw-   0        0        0     3447 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/cursor.py
--rw-rw-rw-   0        0        0    42211 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tools/curve.py
--rw-rw-rw-   0        0        0    42395 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/tools/image.py
--rw-rw-rw-   0        0        0     6460 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/item.py
--rw-rw-rw-   0        0        0     3054 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/label.py
--rw-rw-rw-   0        0        0    11324 2023-12-14 19:00:47.000000 PlotPy-2.3.0/plotpy/tools/misc.py
--rw-rw-rw-   0        0        0     6115 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/plot.py
--rw-rw-rw-   0        0        0     5730 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/selection.py
--rw-rw-rw-   0        0        0     9273 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/tools/shape.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.867697 PlotPy-2.3.0/plotpy/widgets/
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/widgets/__init__.py
--rw-rw-rw-   0        0        0     1777 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/widgets/about.py
--rw-rw-rw-   0        0        0    10076 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/basetransform.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.914567 PlotPy-2.3.0/plotpy/widgets/colormap/
--rw-rw-rw-   0        0        0      358 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/widgets/colormap/__init__.py
--rw-rw-rw-   0        0        0     2221 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/widgets/colormap/_slider.py
--rw-rw-rw-   0        0        0    10513 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/widgets/colormap/editor.py
--rw-rw-rw-   0        0        0    15330 2024-03-04 13:28:36.000000 PlotPy-2.3.0/plotpy/widgets/colormap/manager.py
--rw-rw-rw-   0        0        0    25006 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/colormap/widget.py
--rw-rw-rw-   0        0        0    30889 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/fit.py
--rw-rw-rw-   0        0        0     8439 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/fliprotate.py
--rw-rw-rw-   0        0        0     6375 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/widgets/imagefile.py
--rw-rw-rw-   0        0        0     4120 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy/widgets/qtdesigner.py
--rw-rw-rw-   0        0        0     4988 2024-02-08 10:33:36.000000 PlotPy-2.3.0/plotpy/widgets/resizedialog.py
--rw-rw-rw-   0        0        0     7980 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/rotatecrop.py
--rw-rw-rw-   0        0        0     5841 2024-03-11 08:11:54.000000 PlotPy-2.3.0/plotpy/widgets/selectdialog.py
--rw-rw-rw-   0        0        0      276 2023-11-23 17:46:00.000000 PlotPy-2.3.0/plotpy-tests.desktop
--rw-rw-rw-   0        0        0     2035 2024-03-11 08:11:54.000000 PlotPy-2.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.914567 PlotPy-2.3.0/qtdesigner/
--rw-rw-rw-   0        0        0      361 2023-11-23 17:46:00.000000 PlotPy-2.3.0/qtdesigner/plotplugin.py
--rw-rw-rw-   0        0        0       42 2024-03-11 08:19:18.977071 PlotPy-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3257 2023-12-22 08:06:28.000000 PlotPy-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 08:19:18.977071 PlotPy-2.3.0/src/
--rw-rw-rw-   0        0        0     5676 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/arrays.hpp
--rw-rw-rw-   0        0        0  1210847 2024-03-11 08:19:15.000000 PlotPy-2.3.0/src/contour2d.c
--rw-rw-rw-   0        0        0    12546 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/contour2d.pyx
--rw-rw-rw-   0        0        0     1162 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/debug.hpp
--rw-rw-rw-   0        0        0   302415 2024-03-11 08:19:15.000000 PlotPy-2.3.0/src/histogram2d.c
--rw-rw-rw-   0        0        0     3407 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/histogram2d.pyx
--rw-rw-rw-   0        0        0   240674 2024-03-11 08:19:15.000000 PlotPy-2.3.0/src/mandelbrot.c
--rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/mandelbrot.pyx
--rw-rw-rw-   0        0        0    15123 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/pcolor.cpp
--rw-rw-rw-   0        0        0     7785 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/points.hpp
--rw-rw-rw-   0        0        0    26596 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/scaler.cpp
--rw-rw-rw-   0        0        0     2555 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/scaler.hpp
--rw-rw-rw-   0        0        0     4105 2023-11-23 17:46:00.000000 PlotPy-2.3.0/src/traits.hpp
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.583426 plotpy-2.3.1/
+-rw-rw-rw-   0        0        0    15956 2024-05-06 16:40:26.000000 plotpy-2.3.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1563 2023-11-23 17:46:00.000000 plotpy-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      143 2024-04-10 16:39:34.000000 plotpy-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8668 2024-05-06 16:41:15.583426 plotpy-2.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.583426 plotpy-2.3.1/PlotPy.egg-info/
+-rw-rw-rw-   0        0        0     8668 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16880 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      224 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4379 2023-11-23 17:46:00.000000 plotpy-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.114675 plotpy-2.3.1/colormaps/
+-rw-rw-rw-   0        0        0      170 2024-02-08 10:33:36.000000 plotpy-2.3.1/colormaps/README.md
+-rw-rw-rw-   0        0        0   421433 2024-02-08 10:33:36.000000 plotpy-2.3.1/colormaps/_cm.py
+-rw-rw-rw-   0        0        0     3083 2024-02-09 17:39:23.000000 plotpy-2.3.1/colormaps/colormap.py
+-rw-rw-rw-   0        0        0     9391 2024-03-04 13:28:35.000000 plotpy-2.3.1/colormaps/matplotlib_cmaps.py
+-rw-rw-rw-   0        0        0      189 2024-04-10 16:39:34.000000 plotpy-2.3.1/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.161549 plotpy-2.3.1/doc/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.177175 plotpy-2.3.1/doc/_static/
+-rw-rw-rw-   0        0        0   110568 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0       79 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/changelog.rst
+-rw-rw-rw-   0        0        0     2273 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.270926 plotpy-2.3.1/doc/dev/
+-rw-rw-rw-   0        0        0     1003 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/build.rst
+-rw-rw-rw-   0        0        0     4374 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0     3108 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.csv
+-rw-rw-rw-   0        0        0     9868 2024-02-16 08:53:28.000000 plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.rst
+-rw-rw-rw-   0        0        0      158 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     5039 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/platforms.rst
+-rw-rw-rw-   0        0        0      389 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/dev/v1_to_guidata_v3.csv
+-rw-rw-rw-   0        0        0     2489 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/dev/v1_to_v2.csv
+-rw-rw-rw-   0        0        0     3374 2024-02-16 08:53:28.000000 plotpy-2.3.1/doc/dev/v1_to_v2.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.333428 plotpy-2.3.1/doc/features/
+-rw-rw-rw-   0        0        0       41 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/colormapmanager.rst
+-rw-rw-rw-   0        0        0       31 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/events.rst
+-rw-rw-rw-   0        0        0       36 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/fit.rst
+-rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/fliprotate.rst
+-rw-rw-rw-   0        0        0       42 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/imagefile.rst
+-rw-rw-rw-   0        0        0      327 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/index.rst
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/io.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.364677 plotpy-2.3.1/doc/features/items/
+-rw-rw-rw-   0        0        0      784 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/builder.rst
+-rw-rw-rw-   0        0        0     4830 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/examples.rst
+-rw-rw-rw-   0        0        0      149 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/index.rst
+-rw-rw-rw-   0        0        0     2311 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/overview.rst
+-rw-rw-rw-   0        0        0     3319 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/items/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.380298 plotpy-2.3.1/doc/features/mathutils/
+-rw-rw-rw-   0        0        0       41 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/features/mathutils/colormaps.rst
+-rw-rw-rw-   0        0        0       41 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/mathutils/geometry.rst
+-rw-rw-rw-   0        0        0      119 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/mathutils/index.rst
+-rw-rw-rw-   0        0        0       39 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/mathutils/scaler.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.395923 plotpy-2.3.1/doc/features/panels/
+-rw-rw-rw-   0        0        0      127 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/panels/index.rst
+-rw-rw-rw-   0        0        0      891 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/panels/overview.rst
+-rw-rw-rw-   0        0        0      212 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/panels/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.411548 plotpy-2.3.1/doc/features/plot/
+-rw-rw-rw-   0        0        0     1012 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/plot/examples.rst
+-rw-rw-rw-   0        0        0     1560 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/plot/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/plot/overview.rst
+-rw-rw-rw-   0        0        0      625 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/plot/reference.rst
+-rw-rw-rw-   0        0        0       51 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/pyplot.rst
+-rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/resizedialog.rst
+-rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/rotatecrop.rst
+-rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/selectdialog.rst
+-rw-rw-rw-   0        0        0     1754 2024-03-04 12:33:14.000000 plotpy-2.3.1/doc/features/signals.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.442798 plotpy-2.3.1/doc/features/styles/
+-rw-rw-rw-   0        0        0      157 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/styles/index.rst
+-rw-rw-rw-   0        0        0      540 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/styles/overview.rst
+-rw-rw-rw-   0        0        0     1921 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/styles/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.474049 plotpy-2.3.1/doc/features/tools/
+-rw-rw-rw-   0        0        0      289 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/tools/examples.rst
+-rw-rw-rw-   0        0        0      137 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/tools/index.rst
+-rw-rw-rw-   0        0        0     2747 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/features/tools/overview.rst
+-rw-rw-rw-   0        0        0     3717 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/features/tools/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.599052 plotpy-2.3.1/doc/images/
+-rw-rw-rw-   0        0        0    42675 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/my_plot_manager.png
+-rw-rw-rw-   0        0        0    31164 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/my_plot_manager.svg
+-rw-rw-rw-   0        0        0   240381 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/panorama.png
+-rw-rw-rw-   0        0        0  1914412 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/panorama.svg
+-rw-rw-rw-   0        0        0    55886 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plot_widgets.png
+-rw-rw-rw-   0        0        0    30549 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plot_widgets.svg
+-rw-rw-rw-   0        0        0     9809 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plotpy-banner.png
+-rw-rw-rw-   0        0        0     7460 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plotpy-vertical.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.817797 plotpy-2.3.1/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    64597 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0    37530 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/computations.png
+-rw-rw-rw-   0        0        0   179050 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/contrast.png
+-rw-rw-rw-   0        0        0   210107 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/cross_section.png
+-rw-rw-rw-   0        0        0   210494 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/cross_section2.png
+-rw-rw-rw-   0        0        0    81254 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/dotarraydemo.png
+-rw-rw-rw-   0        0        0    41879 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/filtertest1.png
+-rw-rw-rw-   0        0        0    49232 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/filtertest2.png
+-rw-rw-rw-   0        0        0    44646 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/fit.png
+-rw-rw-rw-   0        0        0    32653 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/get_point.png
+-rw-rw-rw-   0        0        0    77053 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/hist2d.png
+-rw-rw-rw-   0        0        0   269545 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/image_plot_tools.png
+-rw-rw-rw-   0        0        0   230644 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagefilter.png
+-rw-rw-rw-   0        0        0   163887 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagesuperp.png
+-rw-rw-rw-   0        0        0   143730 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagexy.png
+-rw-rw-rw-   0        0        0   168112 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/manager.png
+-rw-rw-rw-   0        0        0   231418 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/mandelbrot.png
+-rw-rw-rw-   0        0        0   172858 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/pcolor.png
+-rw-rw-rw-   0        0        0    76448 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/plot.png
+-rw-rw-rw-   0        0        0   173690 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/simple_dialog.png
+-rw-rw-rw-   0        0        0    59433 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/simple_window.png
+-rw-rw-rw-   0        0        0   456556 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/transform.png
+-rw-rw-rw-   0        0        0     1651 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.911550 plotpy-2.3.1/doc/intro/
+-rw-rw-rw-   0        0        0     2862 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/examples.rst
+-rw-rw-rw-   0        0        0      164 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/index.rst
+-rw-rw-rw-   0        0        0      675 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/installation.rst
+-rw-rw-rw-   0        0        0   107599 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/licenses.rst
+-rw-rw-rw-   0        0        0     2299 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/intro/motivation.rst
+-rw-rw-rw-   0        0        0     4815 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/overview.rst
+-rw-rw-rw-   0        0        0     2429 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/requirements.rst
+-rw-rw-rw-   0        0        0      721 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/update_requirements.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.005302 plotpy-2.3.1/plotpy/
+-rw-rw-rw-   0        0        0     1053 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.114675 plotpy-2.3.1/plotpy/builder/
+-rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/__init__.py
+-rw-rw-rw-   0        0        0    13033 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/builder/annotation.py
+-rw-rw-rw-   0        0        0    31776 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/curvemarker.py
+-rw-rw-rw-   0        0        0    33708 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/image.py
+-rw-rw-rw-   0        0        0    10062 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/label.py
+-rw-rw-rw-   0        0        0    17119 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/plot.py
+-rw-rw-rw-   0        0        0     5886 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/shape.py
+-rw-rw-rw-   0        0        0    34344 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/config.py
+-rw-rw-rw-   0        0        0     4756 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/constants.py
+-rw-rw-rw-   0        0        0     2385 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/coords.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.130299 plotpy-2.3.1/plotpy/data/
+-rw-rw-rw-   0        0        0   328300 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/colormaps_default.json
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.458424 plotpy-2.3.1/plotpy/data/icons/
+-rw-rw-rw-   0        0        0      595 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/apply.png
+-rw-rw-rw-   0        0        0      897 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arredit.png
+-rw-rw-rw-   0        0        0      637 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arrow_down.png
+-rw-rw-rw-   0        0        0      638 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arrow_up.png
+-rw-rw-rw-   0        0        0      868 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/autorefresh.png
+-rw-rw-rw-   0        0        0     1012 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/autoscale.png
+-rw-rw-rw-   0        0        0      513 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/axes.png
+-rw-rw-rw-   0        0        0      474 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/busy.png
+-rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/cell_edit.png
+-rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/center.png
+-rw-rw-rw-   0        0        0      495 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/cmap_edit.png
+-rw-rw-rw-   0        0        0      316 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/contrast.png
+-rw-rw-rw-   0        0        0      620 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/copy.png
+-rw-rw-rw-   0        0        0      979 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/copytoclipboard.png
+-rw-rw-rw-   0        0        0      705 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csapplylut.png
+-rw-rw-rw-   0        0        0      178 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csautoscale.png
+-rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection.png
+-rw-rw-rw-   0        0        0      310 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_a.png
+-rw-rw-rw-   0        0        0      375 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_line.png
+-rw-rw-rw-   0        0        0      711 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_oblique.png
+-rw-rw-rw-   0        0        0      160 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csperimage.png
+-rw-rw-rw-   0        0        0      758 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curve_downsample.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.505301 plotpy-2.3.1/plotpy/data/icons/curvestyles/
+-rw-rw-rw-   0        0        0      121 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/dots.png
+-rw-rw-rw-   0        0        0      164 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/lines.png
+-rw-rw-rw-   0        0        0      136 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/steps.png
+-rw-rw-rw-   0        0        0      187 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/sticks.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.505301 plotpy-2.3.1/plotpy/data/icons/curvetypes/
+-rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvetypes/xfy.png
+-rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvetypes/yfx.png
+-rw-rw-rw-   0        0        0      496 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/delete.png
+-rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/edit.png
+-rw-rw-rw-   0        0        0      793 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/edit_point_selection.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.614680 plotpy-2.3.1/plotpy/data/icons/editors/
+-rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/edit.png
+-rw-rw-rw-   0        0        0      790 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/edit_add.png
+-rw-rw-rw-   0        0        0      837 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editcopy.png
+-rw-rw-rw-   0        0        0     1242 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1084 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2065 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/fileimport.png
+-rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/filesave.png
+-rw-rw-rw-   0        0        0      516 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/imshow.png
+-rw-rw-rw-   0        0        0      314 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/insert.png
+-rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/plot.png
+-rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/rename.png
+-rw-rw-rw-   0        0        0      183 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/eliminate_outliers.png
+-rw-rw-rw-   0        0        0      671 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/eraser.png
+-rw-rw-rw-   0        0        0      974 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/exit.png
+-rw-rw-rw-   0        0        0      191 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/expander_down.png
+-rw-rw-rw-   0        0        0      184 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/expander_right.png
+-rw-rw-rw-   0        0        0      861 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/export.png
+-rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/file.png
+-rw-rw-rw-   0        0        0     1213 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileclose.png
+-rw-rw-rw-   0        0        0     1383 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileimport.png
+-rw-rw-rw-   0        0        0      271 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filenew.png
+-rw-rw-rw-   0        0        0     1349 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileopen.png
+-rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filesave.png
+-rw-rw-rw-   0        0        0     1264 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filesaveas.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.724050 plotpy-2.3.1/plotpy/data/icons/filetypes/
+-rw-rw-rw-   0        0        0     1389 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1658 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/html.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1352 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/png.png
+-rw-rw-rw-   0        0        0     1226 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1217 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1609 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1026 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/zip.png
+-rw-rw-rw-   0        0        0      244 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/font.png
+-rw-rw-rw-   0        0        0      185 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/full_range.png
+-rw-rw-rw-   0        0        0      922 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/funct.png
+-rw-rw-rw-   0        0        0      151 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/hcursor.png
+-rw-rw-rw-   0        0        0      433 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/hflip.png
+-rw-rw-rw-   0        0        0      793 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/imagestats.png
+-rw-rw-rw-   0        0        0      437 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/item_list.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.770923 plotpy-2.3.1/plotpy/data/icons/items/
+-rw-rw-rw-   0        0        0      687 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/annotation.png
+-rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/curve.png
+-rw-rw-rw-   0        0        0      172 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/errorbar.png
+-rw-rw-rw-   0        0        0      120 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/grid.png
+-rw-rw-rw-   0        0        0      140 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/histogram.png
+-rw-rw-rw-   0        0        0      857 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/histogram2d.png
+-rw-rw-rw-   0        0        0      852 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/image.png
+-rw-rw-rw-   0        0        0      531 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/label.png
+-rw-rw-rw-   0        0        0      317 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/legend.png
+-rw-rw-rw-   0        0        0      448 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/polygonmap.png
+-rw-rw-rw-   0        0        0      673 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/magnifier.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.849049 plotpy-2.3.1/plotpy/data/icons/markers/
+-rw-rw-rw-   0        0        0      123 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/cross.png
+-rw-rw-rw-   0        0        0      194 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/diamond.png
+-rw-rw-rw-   0        0        0      241 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/ellipse.png
+-rw-rw-rw-   0        0        0      260 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/hexagon.png
+-rw-rw-rw-   0        0        0      105 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/point.png
+-rw-rw-rw-   0        0        0      137 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/square.png
+-rw-rw-rw-   0        0        0      160 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/star.png
+-rw-rw-rw-   0        0        0      223 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_d.png
+-rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_l.png
+-rw-rw-rw-   0        0        0      212 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_r.png
+-rw-rw-rw-   0        0        0      224 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_u.png
+-rw-rw-rw-   0        0        0      145 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/xcross.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.849049 plotpy-2.3.1/plotpy/data/icons/markerstyles/
+-rw-rw-rw-   0        0        0       96 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/cross_marker.png
+-rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/horiz_marker.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/vert_marker.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.864674 plotpy-2.3.1/plotpy/data/icons/mask/
+-rw-rw-rw-   0        0        0      368 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_circle.png
+-rw-rw-rw-   0        0        0      374 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_circle_outside.png
+-rw-rw-rw-   0        0        0      199 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_rectangle.png
+-rw-rw-rw-   0        0        0      200 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_rectangle_outside.png
+-rw-rw-rw-   0        0        0      164 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_tool.png
+-rw-rw-rw-   0        0        0      130 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/max.png
+-rw-rw-rw-   0        0        0      125 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/min.png
+-rw-rw-rw-   0        0        0      132 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/move.png
+-rw-rw-rw-   0        0        0      729 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/multipoint_selection.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/none.png
+-rw-rw-rw-   0        0        0      284 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/not_found.png
+-rw-rw-rw-   0        0        0      397 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/on_curve.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.895922 plotpy-2.3.1/plotpy/data/icons/patterns/
+-rw-rw-rw-   0        0        0      104 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/bdiagpattern.png
+-rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/crosspattern.png
+-rw-rw-rw-   0        0        0       76 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense1pattern.png
+-rw-rw-rw-   0        0        0       78 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense2pattern.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense3pattern.png
+-rw-rw-rw-   0        0        0       73 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense4pattern.png
+-rw-rw-rw-   0        0        0       88 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense5pattern.png
+-rw-rw-rw-   0        0        0       87 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense6pattern.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense7pattern.png
+-rw-rw-rw-   0        0        0      114 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/diagcrosspattern.png
+-rw-rw-rw-   0        0        0      112 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/fdiagpattern.png
+-rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/horpattern.png
+-rw-rw-rw-   0        0        0       74 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/nobrush.png
+-rw-rw-rw-   0        0        0       69 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/solidpattern.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/verpattern.png
+-rw-rw-rw-   0        0        0    17636 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy-banner.svg
+-rw-rw-rw-   0        0        0    17614 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy-vertical.svg
+-rw-rw-rw-   0        0        0    16339 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy.svg
+-rw-rw-rw-   0        0        0      216 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/point_selection.png
+-rw-rw-rw-   0        0        0      723 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/print.png
+-rw-rw-rw-   0        0        0      697 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/python.png
+-rw-rw-rw-   0        0        0      677 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/quickview.png
+-rw-rw-rw-   0        0        0      823 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/rectangular_select.png
+-rw-rw-rw-   0        0        0      740 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/refresh.png
+-rw-rw-rw-   0        0        0     1428 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/save_all.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.911548 plotpy-2.3.1/plotpy/data/icons/scales/
+-rw-rw-rw-   0        0        0      203 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/lin_lin.png
+-rw-rw-rw-   0        0        0      208 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/lin_log.png
+-rw-rw-rw-   0        0        0      219 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/log_lin.png
+-rw-rw-rw-   0        0        0      222 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/log_log.png
+-rw-rw-rw-   0        0        0      518 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/selection.png
+-rw-rw-rw-   0        0        0      851 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/settings.png
+-rw-rw-rw-   0        0        0      135 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shape.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.005297 plotpy-2.3.1/plotpy/data/icons/shapes/
+-rw-rw-rw-   0        0        0      530 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/circle.png
+-rw-rw-rw-   0        0        0      622 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/contour.png
+-rw-rw-rw-   0        0        0      547 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/ellipse_shape.png
+-rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/freeform.png
+-rw-rw-rw-   0        0        0      321 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/gtaxes.png
+-rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/marker.png
+-rw-rw-rw-   0        0        0      650 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/oblique_rectangle.png
+-rw-rw-rw-   0        0        0      118 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/point_shape.png
+-rw-rw-rw-   0        0        0      232 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/polyline.png
+-rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/rectangle.png
+-rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/segment.png
+-rw-rw-rw-   0        0        0     1150 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/snapshot.png
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.036556 plotpy-2.3.1/plotpy/data/icons/styles/
+-rw-rw-rw-   0        0        0       85 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dash.png
+-rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dashdot.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dashdotdot.png
+-rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dot.png
+-rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/solid.png
+-rw-rw-rw-   0        0        0      236 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trash.png
+-rw-rw-rw-   0        0        0      932 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trimage_lock.png
+-rw-rw-rw-   0        0        0      958 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trimage_unlock.png
+-rw-rw-rw-   0        0        0      159 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/vcursor.png
+-rw-rw-rw-   0        0        0      432 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/vflip.png
+-rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xcursor.png
+-rw-rw-rw-   0        0        0      128 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xmax.png
+-rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xmin.png
+-rw-rw-rw-   0        0        0      170 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xrange.png
+-rw-rw-rw-   0        0        0    46755 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/events.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.052174 plotpy-2.3.1/plotpy/external/
+-rw-rw-rw-   0        0        0      399 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.130302 plotpy-2.3.1/plotpy/external/sliders/
+-rw-rw-rw-   0        0        0     2108 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/__init__.py
+-rw-rw-rw-   0        0        0    14101 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_generic_range_slider.py
+-rw-rw-rw-   0        0        0    20447 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_generic_slider.py
+-rw-rw-rw-   0        0        0    23960 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/external/sliders/_labeled.py
+-rw-rw-rw-   0        0        0      758 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/external/sliders/_misc.py
+-rw-rw-rw-   0        0        0     9829 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/external/sliders/_range_style.py
+-rw-rw-rw-   0        0        0     1126 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_sliders.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.192801 plotpy-2.3.1/plotpy/interfaces/
+-rw-rw-rw-   0        0        0      517 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/__init__.py
+-rw-rw-rw-   0        0        0    14685 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/interfaces/items.py
+-rw-rw-rw-   0        0        0      461 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/panel.py
+-rw-rw-rw-   0        0        0     1049 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/plotmanager.py
+-rw-rw-rw-   0        0        0    24077 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/io.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.302177 plotpy-2.3.1/plotpy/items/
+-rw-rw-rw-   0        0        0     1517 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/items/__init__.py
+-rw-rw-rw-   0        0        0    30198 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/annotation.py
+-rw-rw-rw-   0        0        0     6355 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/contour.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.364675 plotpy-2.3.1/plotpy/items/curve/
+-rw-rw-rw-   0        0        0      176 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/curve/__init__.py
+-rw-rw-rw-   0        0        0    18860 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/curve/base.py
+-rw-rw-rw-   0        0        0    12987 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/curve/errorbar.py
+-rw-rw-rw-   0        0        0     7632 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/grid.py
+-rw-rw-rw-   0        0        0     7118 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/histogram.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.427172 plotpy-2.3.1/plotpy/items/image/
+-rw-rw-rw-   0        0        0      608 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/image/__init__.py
+-rw-rw-rw-   0        0        0    44532 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/base.py
+-rw-rw-rw-   0        0        0    11447 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/filter.py
+-rw-rw-rw-   0        0        0    28332 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/image_items.py
+-rw-rw-rw-   0        0        0    24911 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/masked.py
+-rw-rw-rw-   0        0        0    25205 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/misc.py
+-rw-rw-rw-   0        0        0    23529 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/transform.py
+-rw-rw-rw-   0        0        0    32816 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/items/label.py
+-rw-rw-rw-   0        0        0    13551 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/polygonmap.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.567800 plotpy-2.3.1/plotpy/items/shape/
+-rw-rw-rw-   0        0        0      457 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/shape/__init__.py
+-rw-rw-rw-   0        0        0     9972 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/axis.py
+-rw-rw-rw-   0        0        0     8592 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/base.py
+-rw-rw-rw-   0        0        0    11893 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/ellipse.py
+-rw-rw-rw-   0        0        0    16554 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/marker.py
+-rw-rw-rw-   0        0        0     2611 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/point.py
+-rw-rw-rw-   0        0        0    14718 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/polygon.py
+-rw-rw-rw-   0        0        0     9735 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/items/shape/range.py
+-rw-rw-rw-   0        0        0    11459 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/rectangle.py
+-rw-rw-rw-   0        0        0     4581 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/segment.py
+-rw-rw-rw-   0        0        0     4619 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/shape/svg.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:10.958428 plotpy-2.3.1/plotpy/locale/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:10.958428 plotpy-2.3.1/plotpy/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.599056 plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    32854 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/plotpy.mo
+-rw-rw-rw-   0        0        0     1918 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/lutrange.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.645928 plotpy-2.3.1/plotpy/mathutils/
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/arrayfuncs.py
+-rw-rw-rw-   0        0        0    10325 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/mathutils/colormap.py
+-rw-rw-rw-   0        0        0     6803 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/geometry.py
+-rw-rw-rw-   0        0        0     1892 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/scaler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.724050 plotpy-2.3.1/plotpy/panels/
+-rw-rw-rw-   0        0        0      270 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/panels/base.py
+-rw-rw-rw-   0        0        0    19745 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/panels/contrastadjustment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.786551 plotpy-2.3.1/plotpy/panels/csection/
+-rw-rw-rw-   0        0        0      480 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/csection/__init__.py
+-rw-rw-rw-   0        0        0    17094 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/panels/csection/csitem.py
+-rw-rw-rw-   0        0        0    16887 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/panels/csection/csplot.py
+-rw-rw-rw-   0        0        0    12868 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/panels/csection/cswidget.py
+-rw-rw-rw-   0        0        0     9425 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/itemlist.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.864676 plotpy-2.3.1/plotpy/plot/
+-rw-rw-rw-   0        0        0      325 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/plot/__init__.py
+-rw-rw-rw-   0        0        0    85147 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/plot/base.py
+-rw-rw-rw-   0        0        0    22002 2024-02-09 17:39:23.000000 plotpy-2.3.1/plotpy/plot/interactive.py
+-rw-rw-rw-   0        0        0    25295 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/plot/manager.py
+-rw-rw-rw-   0        0        0    34516 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/plot/plotwidget.py
+-rw-rw-rw-   0        0        0     2762 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/pyplot.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.005300 plotpy-2.3.1/plotpy/styles/
+-rw-rw-rw-   0        0        0     1738 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/styles/__init__.py
+-rw-rw-rw-   0        0        0     4155 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/axes.py
+-rw-rw-rw-   0        0        0    19338 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/base.py
+-rw-rw-rw-   0        0        0     3172 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/curve.py
+-rw-rw-rw-   0        0        0     1552 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/errorbar.py
+-rw-rw-rw-   0        0        0     3896 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/histogram.py
+-rw-rw-rw-   0        0        0    18053 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/image.py
+-rw-rw-rw-   0        0        0     8365 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/label.py
+-rw-rw-rw-   0        0        0     1631 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/polygonmap.py
+-rw-rw-rw-   0        0        0    13088 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/shape.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.052176 plotpy-2.3.1/plotpy/tests/
+-rw-rw-rw-   0        0        0      712 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.099055 plotpy-2.3.1/plotpy/tests/benchmarks/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/__init__.py
+-rw-rw-rw-   0        0        0     4226 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_benchmarks.py
+-rw-rw-rw-   0        0        0      836 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_bigimages.py
+-rw-rw-rw-   0        0        0     2847 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_loadtest.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.224050 plotpy-2.3.1/plotpy/tests/data/
+-rw-rw-rw-   0        0        0    39666 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/brain.png
+-rw-rw-rw-   0        0        0    35354 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/brain_cylinder.png
+-rw-rw-rw-   0        0        0   525620 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/mr-brain.dcm
+-rw-rw-rw-   0        0        0     1991 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/svg_target.svg
+-rw-rw-rw-   0        0        0     1765 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/svg_tool.svg
+-rw-rw-rw-   0        0        0     4363 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.520928 plotpy-2.3.1/plotpy/tests/features/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_auto_curve_image.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_autoscale_shapes.py
+-rw-rw-rw-   0        0        0     1660 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_builder.py
+-rw-rw-rw-   0        0        0     3014 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_colormap_editor.py
+-rw-rw-rw-   0        0        0     2221 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/features/test_colormap_manager.py
+-rw-rw-rw-   0        0        0     1381 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_computations.py
+-rw-rw-rw-   0        0        0     1275 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_contrast.py
+-rw-rw-rw-   0        0        0     1064 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_cursors.py
+-rw-rw-rw-   0        0        0     1164 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_dicom_image.py
+-rw-rw-rw-   0        0        0      798 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_fit.py
+-rw-rw-rw-   0        0        0     1483 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_image_coords.py
+-rw-rw-rw-   0        0        0     1648 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_imagefilter.py
+-rw-rw-rw-   0        0        0     1576 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/tests/features/test_imagesuperp.py
+-rw-rw-rw-   0        0        0     1116 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_hdf5.py
+-rw-rw-rw-   0        0        0     1453 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_json.py
+-rw-rw-rw-   0        0        0     6395 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_pickle.py
+-rw-rw-rw-   0        0        0     3123 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/features/test_manager.py
+-rw-rw-rw-   0        0        0      718 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_no_auto_tools.py
+-rw-rw-rw-   0        0        0      927 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_log.py
+-rw-rw-rw-   0        0        0     1214 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_types.py
+-rw-rw-rw-   0        0        0      846 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_yreverse.py
+-rw-rw-rw-   0        0        0     2114 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_pyplot.py
+-rw-rw-rw-   0        0        0      694 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_resize.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.645933 plotpy-2.3.1/plotpy/tests/items/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/__init__.py
+-rw-rw-rw-   0        0        0     1159 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_annotations.py
+-rw-rw-rw-   0        0        0     1534 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/items/test_curves.py
+-rw-rw-rw-   0        0        0     1660 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/items/test_curves_highdpi.py
+-rw-rw-rw-   0        0        0     2298 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_hist2d.py
+-rw-rw-rw-   0        0        0      710 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_histogram.py
+-rw-rw-rw-   0        0        0      840 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image.py
+-rw-rw-rw-   0        0        0      989 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_contour.py
+-rw-rw-rw-   0        0        0     1231 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_masked.py
+-rw-rw-rw-   0        0        0     1336 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_masked_xy.py
+-rw-rw-rw-   0        0        0      759 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_rgb.py
+-rw-rw-rw-   0        0        0      758 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_xy.py
+-rw-rw-rw-   0        0        0     2763 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/items/test_mandelbrot.py
+-rw-rw-rw-   0        0        0     2340 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_pcolor.py
+-rw-rw-rw-   0        0        0     2363 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/items/test_polygons.py
+-rw-rw-rw-   0        0        0      881 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/items/test_svgshapes.py
+-rw-rw-rw-   0        0        0     6217 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_transform.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.817807 plotpy-2.3.1/plotpy/tests/tools/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_actiontool.py
+-rw-rw-rw-   0        0        0     1151 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section.py
+-rw-rw-rw-   0        0        0     2466 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section_line.py
+-rw-rw-rw-   0        0        0     1097 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section_oblique.py
+-rw-rw-rw-   0        0        0     1804 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_customize_shape_tool.py
+-rw-rw-rw-   0        0        0     1692 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_downsample_curve.py
+-rw-rw-rw-   0        0        0     2865 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_edit_point.py
+-rw-rw-rw-   0        0        0     1757 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_point.py
+-rw-rw-rw-   0        0        0     2215 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_points.py
+-rw-rw-rw-   0        0        0     1118 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle.py
+-rw-rw-rw-   0        0        0     1741 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle_with_svg.py
+-rw-rw-rw-   0        0        0     1954 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_segment.py
+-rw-rw-rw-   0        0        0     2155 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_image_plot_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.067803 plotpy-2.3.1/plotpy/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     3867 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_annotation_tools.py
+-rw-rw-rw-   0        0        0     1125 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_aspect_ratio_tool.py
+-rw-rw-rw-   0        0        0     2165 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_baseplot.py
+-rw-rw-rw-   0        0        0     2728 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_annotation.py
+-rw-rw-rw-   0        0        0     6112 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_curve.py
+-rw-rw-rw-   0        0        0     3291 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_image.py
+-rw-rw-rw-   0        0        0     1655 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_shape.py
+-rw-rw-rw-   0        0        0     2352 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_contour.py
+-rw-rw-rw-   0        0        0     1497 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_cursor_tools.py
+-rw-rw-rw-   0        0        0     7980 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_curve_tools.py
+-rw-rw-rw-   0        0        0     2071 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_display_coords_tool.py
+-rw-rw-rw-   0        0        0     5505 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_events.py
+-rw-rw-rw-   0        0        0      415 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_fontparam.py
+-rw-rw-rw-   0        0        0     2840 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_geometry.py
+-rw-rw-rw-   0        0        0      937 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_highprecisionxy.py
+-rw-rw-rw-   0        0        0     3234 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_io.py
+-rw-rw-rw-   0        0        0     1702 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_line.py
+-rw-rw-rw-   0        0        0      888 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_line_cross_section_tool.py
+-rw-rw-rw-   0        0        0    14442 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_manipulate_selection.py
+-rw-rw-rw-   0        0        0     2021 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_mask_tool.py
+-rw-rw-rw-   0        0        0     2600 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_multiline_tools.py
+-rw-rw-rw-   0        0        0      909 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_oblique_cross_section_tool.py
+-rw-rw-rw-   0        0        0     2368 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_plot_curve.py
+-rw-rw-rw-   0        0        0     5331 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_plot_image.py
+-rw-rw-rw-   0        0        0     2165 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_rect_zoom.py
+-rw-rw-rw-   0        0        0      839 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_seg_dist.py
+-rw-rw-rw-   0        0        0     3032 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_styles.py
+-rw-rw-rw-   0        0        0      854 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_tools_export.py
+-rw-rw-rw-   0        0        0     8320 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/utils.py
+-rw-rw-rw-   0        0        0     1320 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/vistools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.177182 plotpy-2.3.1/plotpy/tests/widgets/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/__init__.py
+-rw-rw-rw-   0        0        0     6910 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_dotarraydemo.py
+-rw-rw-rw-   0        0        0     2725 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_filtertest1.py
+-rw-rw-rw-   0        0        0     3530 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_filtertest2.py
+-rw-rw-rw-   0        0        0     1698 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_fliprotate.py
+-rw-rw-rw-   0        0        0    14422 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_plot_timecurve.py
+-rw-rw-rw-   0        0        0     1185 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.py
+-rw-rw-rw-   0        0        0      763 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.ui
+-rw-rw-rw-   0        0        0     2173 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_resize_dialog.py
+-rw-rw-rw-   0        0        0     2920 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_rotatecrop.py
+-rw-rw-rw-   0        0        0     3740 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_simple_dialog.py
+-rw-rw-rw-   0        0        0    10267 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/widgets/test_simple_window.py
+-rw-rw-rw-   0        0        0     2846 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_syncplot.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.317805 plotpy-2.3.1/plotpy/tools/
+-rw-rw-rw-   0        0        0     1993 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tools/__init__.py
+-rw-rw-rw-   0        0        0     1945 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/annotation.py
+-rw-rw-rw-   0        0        0     3382 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/axes.py
+-rw-rw-rw-   0        0        0    18826 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tools/base.py
+-rw-rw-rw-   0        0        0     4654 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tools/cross_section.py
+-rw-rw-rw-   0        0        0     3447 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/cursor.py
+-rw-rw-rw-   0        0        0    42249 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tools/curve.py
+-rw-rw-rw-   0        0        0    42618 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tools/image.py
+-rw-rw-rw-   0        0        0     6460 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/item.py
+-rw-rw-rw-   0        0        0     3054 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/label.py
+-rw-rw-rw-   0        0        0    11326 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tools/misc.py
+-rw-rw-rw-   0        0        0     6115 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/plot.py
+-rw-rw-rw-   0        0        0     5730 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/selection.py
+-rw-rw-rw-   0        0        0     9273 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/shape.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.474052 plotpy-2.3.1/plotpy/widgets/
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1777 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/about.py
+-rw-rw-rw-   0        0        0    10076 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/basetransform.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.505304 plotpy-2.3.1/plotpy/widgets/colormap/
+-rw-rw-rw-   0        0        0      358 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/__init__.py
+-rw-rw-rw-   0        0        0     2221 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/_slider.py
+-rw-rw-rw-   0        0        0    10513 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/editor.py
+-rw-rw-rw-   0        0        0    15875 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/widgets/colormap/manager.py
+-rw-rw-rw-   0        0        0    25006 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/colormap/widget.py
+-rw-rw-rw-   0        0        0    30905 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/fit.py
+-rw-rw-rw-   0        0        0     8505 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/fliprotate.py
+-rw-rw-rw-   0        0        0     6375 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/imagefile.py
+-rw-rw-rw-   0        0        0     4120 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/qtdesigner.py
+-rw-rw-rw-   0        0        0     4988 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/resizedialog.py
+-rw-rw-rw-   0        0        0     8046 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/rotatecrop.py
+-rw-rw-rw-   0        0        0     5841 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/selectdialog.py
+-rw-rw-rw-   0        0        0      276 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy-tests.desktop
+-rw-rw-rw-   0        0        0     3410 2024-04-10 16:39:34.000000 plotpy-2.3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.520927 plotpy-2.3.1/qtdesigner/
+-rw-rw-rw-   0        0        0      361 2023-11-23 17:46:00.000000 plotpy-2.3.1/qtdesigner/plotplugin.py
+-rw-rw-rw-   0        0        0      220 2024-04-10 16:39:34.000000 plotpy-2.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 16:41:15.583426 plotpy-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     3257 2023-12-22 08:06:28.000000 plotpy-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.567802 plotpy-2.3.1/src/
+-rw-rw-rw-   0        0        0     5676 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/arrays.hpp
+-rw-rw-rw-   0        0        0  1210847 2024-05-06 16:41:09.000000 plotpy-2.3.1/src/contour2d.c
+-rw-rw-rw-   0        0        0    12546 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/contour2d.pyx
+-rw-rw-rw-   0        0        0     1162 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/debug.hpp
+-rw-rw-rw-   0        0        0   302415 2024-05-06 16:41:10.000000 plotpy-2.3.1/src/histogram2d.c
+-rw-rw-rw-   0        0        0     3407 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/histogram2d.pyx
+-rw-rw-rw-   0        0        0   240674 2024-05-06 16:41:10.000000 plotpy-2.3.1/src/mandelbrot.c
+-rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/mandelbrot.pyx
+-rw-rw-rw-   0        0        0    15123 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/pcolor.cpp
+-rw-rw-rw-   0        0        0     7785 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/points.hpp
+-rw-rw-rw-   0        0        0    26596 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/scaler.cpp
+-rw-rw-rw-   0        0        0     2555 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/scaler.hpp
+-rw-rw-rw-   0        0        0     4105 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/traits.hpp
```

### Comparing `PlotPy-2.3.0/LICENSE` & `plotpy-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/PKG-INFO` & `plotpy-2.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlotPy
-Version: 2.3.0
+Version: 2.3.1
 Summary: Curve and image plotting tools for Python/Qt applications
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
@@ -31,42 +31,49 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/PlotPyStack/plotpy/
 Project-URL: Documentation, https://plotpy.readthedocs.io/en/latest/
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidata>=3.4
 Requires-Dist: PythonQwt>=0.12.1
 Requires-Dist: NumPy>=1.17
 Requires-Dist: SciPy>=1.3
 Requires-Dist: Pillow
 Requires-Dist: tifffile
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Coverage; extra == "dev"
 Requires-Dist: Cython; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: PyQt5; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: myst_parser; extra == "doc"
```

### Comparing `PlotPy-2.3.0/PlotPy.egg-info/PKG-INFO` & `plotpy-2.3.1/PlotPy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlotPy
-Version: 2.3.0
+Version: 2.3.1
 Summary: Curve and image plotting tools for Python/Qt applications
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
@@ -31,42 +31,49 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/PlotPyStack/plotpy/
 Project-URL: Documentation, https://plotpy.readthedocs.io/en/latest/
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidata>=3.4
 Requires-Dist: PythonQwt>=0.12.1
 Requires-Dist: NumPy>=1.17
 Requires-Dist: SciPy>=1.3
 Requires-Dist: Pillow
 Requires-Dist: tifffile
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Coverage; extra == "dev"
 Requires-Dist: Cython; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: PyQt5; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: myst_parser; extra == "doc"
```

### Comparing `PlotPy-2.3.0/PlotPy.egg-info/SOURCES.txt` & `plotpy-2.3.1/PlotPy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+conftest.py
 plotpy-tests.desktop
 pyproject.toml
+requirements.txt
 setup.py
 ./src/contour2d.c
 ./src/histogram2d.c
 ./src/mandelbrot.c
 ./src/pcolor.cpp
 ./src/scaler.cpp
 PlotPy.egg-info/PKG-INFO
 PlotPy.egg-info/SOURCES.txt
 PlotPy.egg-info/dependency_links.txt
 PlotPy.egg-info/entry_points.txt
 PlotPy.egg-info/requires.txt
 PlotPy.egg-info/top_level.txt
+colormaps/README.md
+colormaps/_cm.py
+colormaps/colormap.py
+colormaps/matplotlib_cmaps.py
 doc/changelog.rst
 doc/conf.py
 doc/index.rst
 doc/requirements.rst
 doc/update_requirements.py
 doc/_static/favicon.ico
 doc/dev/build.rst
@@ -355,15 +362,14 @@
 plotpy/styles/errorbar.py
 plotpy/styles/histogram.py
 plotpy/styles/image.py
 plotpy/styles/label.py
 plotpy/styles/polygonmap.py
 plotpy/styles/shape.py
 plotpy/tests/__init__.py
-plotpy/tests/conftest.py
 plotpy/tests/data.py
 plotpy/tests/vistools.py
 plotpy/tests/benchmarks/__init__.py
 plotpy/tests/benchmarks/test_benchmarks.py
 plotpy/tests/benchmarks/test_bigimages.py
 plotpy/tests/benchmarks/test_loadtest.py
 plotpy/tests/data/brain.png
@@ -394,14 +400,15 @@
 plotpy/tests/features/test_plot_types.py
 plotpy/tests/features/test_plot_yreverse.py
 plotpy/tests/features/test_pyplot.py
 plotpy/tests/features/test_resize.py
 plotpy/tests/items/__init__.py
 plotpy/tests/items/test_annotations.py
 plotpy/tests/items/test_curves.py
+plotpy/tests/items/test_curves_highdpi.py
 plotpy/tests/items/test_hist2d.py
 plotpy/tests/items/test_histogram.py
 plotpy/tests/items/test_image.py
 plotpy/tests/items/test_image_contour.py
 plotpy/tests/items/test_image_masked.py
 plotpy/tests/items/test_image_masked_xy.py
 plotpy/tests/items/test_image_rgb.py
@@ -422,36 +429,40 @@
 plotpy/tests/tools/test_get_point.py
 plotpy/tests/tools/test_get_points.py
 plotpy/tests/tools/test_get_rectangle.py
 plotpy/tests/tools/test_get_rectangle_with_svg.py
 plotpy/tests/tools/test_get_segment.py
 plotpy/tests/tools/test_image_plot_tools.py
 plotpy/tests/unit/__init__.py
+plotpy/tests/unit/test_annotation_tools.py
 plotpy/tests/unit/test_aspect_ratio_tool.py
 plotpy/tests/unit/test_baseplot.py
 plotpy/tests/unit/test_builder_annotation.py
 plotpy/tests/unit/test_builder_curve.py
 plotpy/tests/unit/test_builder_image.py
 plotpy/tests/unit/test_builder_shape.py
 plotpy/tests/unit/test_contour.py
+plotpy/tests/unit/test_cursor_tools.py
+plotpy/tests/unit/test_curve_tools.py
 plotpy/tests/unit/test_display_coords_tool.py
+plotpy/tests/unit/test_events.py
 plotpy/tests/unit/test_fontparam.py
 plotpy/tests/unit/test_geometry.py
 plotpy/tests/unit/test_highprecisionxy.py
 plotpy/tests/unit/test_io.py
 plotpy/tests/unit/test_line.py
 plotpy/tests/unit/test_line_cross_section_tool.py
+plotpy/tests/unit/test_manipulate_selection.py
+plotpy/tests/unit/test_mask_tool.py
 plotpy/tests/unit/test_multiline_tools.py
 plotpy/tests/unit/test_oblique_cross_section_tool.py
 plotpy/tests/unit/test_plot_curve.py
 plotpy/tests/unit/test_plot_image.py
-plotpy/tests/unit/test_point_tools.py
 plotpy/tests/unit/test_rect_zoom.py
 plotpy/tests/unit/test_seg_dist.py
-plotpy/tests/unit/test_shape_tools.py
 plotpy/tests/unit/test_styles.py
 plotpy/tests/unit/test_tools_export.py
 plotpy/tests/unit/utils.py
 plotpy/tests/widgets/__init__.py
 plotpy/tests/widgets/test_dotarraydemo.py
 plotpy/tests/widgets/test_filtertest1.py
 plotpy/tests/widgets/test_filtertest2.py
```

### Comparing `PlotPy-2.3.0/README.md` & `plotpy-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/_static/favicon.ico` & `plotpy-2.3.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/conf.py` & `plotpy-2.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/dev/build.rst` & `plotpy-2.3.1/doc/dev/build.rst`

 * *Files 18% similar despite different names*

```diff
@@ -25,23 +25,22 @@
 
 * Python
 * pytest
 * coverage (optional)
 
 Then run the following command::
 
-    pytest plotpy
+    pytest
 
 To run test with coverage support, use the following command::
 
-    pytest -v --cov --cov-report=html plotpy
+    pytest -v --cov --cov-report=html
 
 
 Code formatting
 ^^^^^^^^^^^^^^^
 
-The code is formatted with `black <https://black.readthedocs.io/en/stable/>`_
-and `isort <https://isort.readthedocs.io/en/stable/>`_.
+The code is formatted with `ruff <https://pypi.org/project/ruff/>`_.
 
 If you are using `Visual Studio Code <https://code.visualstudio.com/>`_,
 the formatting is done automatically when you save a file, thanks to the
 project settings in the `.vscode` directory.
```

### Comparing `PlotPy-2.3.0/doc/dev/contribute.rst` & `plotpy-2.3.1/doc/dev/contribute.rst`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         pylint --disable=fixme,C,R,W plotpy
 
 * Run the tests and check that they all pass:
 
     .. code-block:: bash
 
-        pytest plotpy
+        pytest
 
 Pull request
 ~~~~~~~~~~~~
 
 If you want to contribute to the project, you can submit a patch. The
 recommended way to do this is to fork the project on GitHub, create a branch
 for your modifications and then send a pull request. The pull request will be
```

### Comparing `PlotPy-2.3.0/doc/dev/guiqwt_to_plotpy.csv` & `plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.csv`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/dev/guiqwt_to_plotpy.rst` & `plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/dev/platforms.rst` & `plotpy-2.3.1/doc/dev/platforms.rst`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     python setup.py build_ext --inplace
 
 That's it, you can now run the tests using the following command:
 
 .. code-block:: bash
 
-    pytest plotpy
+    pytest
 
 If you want to rely on Visual Studio Code for editing and take advantage of the
 project settings and tasks, you will need to set the following environment variable:
 
 .. code-block:: bash
 
     set PPSTACK_PYTHONEXE=C:\WPy64-31110\python-3.11.1.amd64\python.exe
@@ -156,8 +156,8 @@
     cd ~/path_to_plotpy_repo
     python setup.py build_ext --inplace
 
 That's it, you can now run the tests using the following command:
 
 .. code-block:: bash
 
-    pytest plotpy
+    pytest
```

### Comparing `PlotPy-2.3.0/doc/dev/v1_to_v2.csv` & `plotpy-2.3.1/doc/dev/v1_to_v2.csv`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/dev/v1_to_v2.rst` & `plotpy-2.3.1/doc/dev/v1_to_v2.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/items/builder.rst` & `plotpy-2.3.1/doc/features/items/builder.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/items/examples.rst` & `plotpy-2.3.1/doc/features/items/examples.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/items/overview.rst` & `plotpy-2.3.1/doc/features/items/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/items/reference.rst` & `plotpy-2.3.1/doc/features/items/reference.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/panels/overview.rst` & `plotpy-2.3.1/doc/features/panels/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/plot/examples.rst` & `plotpy-2.3.1/doc/features/plot/examples.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/plot/index.rst` & `plotpy-2.3.1/doc/features/plot/index.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/plot/overview.rst` & `plotpy-2.3.1/doc/features/plot/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/plot/reference.rst` & `plotpy-2.3.1/doc/features/plot/reference.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/signals.rst` & `plotpy-2.3.1/doc/features/signals.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/styles/overview.rst` & `plotpy-2.3.1/doc/features/styles/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/styles/reference.rst` & `plotpy-2.3.1/doc/features/styles/reference.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/tools/overview.rst` & `plotpy-2.3.1/doc/features/tools/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/features/tools/reference.rst` & `plotpy-2.3.1/doc/features/tools/reference.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/my_plot_manager.png` & `plotpy-2.3.1/doc/images/my_plot_manager.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/my_plot_manager.svg` & `plotpy-2.3.1/doc/images/my_plot_manager.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/panorama.png` & `plotpy-2.3.1/doc/images/panorama.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/panorama.svg` & `plotpy-2.3.1/doc/images/panorama.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/plot_widgets.png` & `plotpy-2.3.1/doc/images/plot_widgets.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/plot_widgets.svg` & `plotpy-2.3.1/doc/images/plot_widgets.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/plotpy-banner.png` & `plotpy-2.3.1/doc/images/plotpy-banner.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/plotpy-vertical.png` & `plotpy-2.3.1/doc/images/plotpy-vertical.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/__init__.png` & `plotpy-2.3.1/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/computations.png` & `plotpy-2.3.1/doc/images/screenshots/computations.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/contrast.png` & `plotpy-2.3.1/doc/images/screenshots/contrast.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/cross_section.png` & `plotpy-2.3.1/doc/images/screenshots/cross_section.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/cross_section2.png` & `plotpy-2.3.1/doc/images/screenshots/cross_section2.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/dotarraydemo.png` & `plotpy-2.3.1/doc/images/screenshots/dotarraydemo.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/filtertest1.png` & `plotpy-2.3.1/doc/images/screenshots/filtertest1.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/filtertest2.png` & `plotpy-2.3.1/doc/images/screenshots/filtertest2.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/fit.png` & `plotpy-2.3.1/doc/images/screenshots/fit.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/get_point.png` & `plotpy-2.3.1/doc/images/screenshots/get_point.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/hist2d.png` & `plotpy-2.3.1/doc/images/screenshots/hist2d.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/image_plot_tools.png` & `plotpy-2.3.1/doc/images/screenshots/image_plot_tools.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/imagefilter.png` & `plotpy-2.3.1/doc/images/screenshots/imagefilter.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/imagesuperp.png` & `plotpy-2.3.1/doc/images/screenshots/imagesuperp.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/imagexy.png` & `plotpy-2.3.1/doc/images/screenshots/imagexy.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/manager.png` & `plotpy-2.3.1/doc/images/screenshots/manager.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/mandelbrot.png` & `plotpy-2.3.1/doc/images/screenshots/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/pcolor.png` & `plotpy-2.3.1/doc/images/screenshots/pcolor.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/plot.png` & `plotpy-2.3.1/doc/images/screenshots/plot.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/simple_dialog.png` & `plotpy-2.3.1/doc/images/screenshots/simple_dialog.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/simple_window.png` & `plotpy-2.3.1/doc/images/screenshots/simple_window.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/images/screenshots/transform.png` & `plotpy-2.3.1/doc/images/screenshots/transform.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/index.rst` & `plotpy-2.3.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/intro/examples.rst` & `plotpy-2.3.1/doc/intro/examples.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/intro/installation.rst` & `plotpy-2.3.1/doc/intro/installation.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/intro/licenses.rst` & `plotpy-2.3.1/doc/intro/licenses.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/intro/motivation.rst` & `plotpy-2.3.1/doc/intro/motivation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 What are PlotPy V2 advantages over PlotPy V1?
 ---------------------------------------------
 
 From a developer point of view, PlotPy V2 is a major overhaul of PlotPy V1:
 
 * Architecture has been redesigned to be more modular and extensible, and more simple.
-* Code quality has been improved introducing `black`, `isort` and typing annotations
+* Code quality has been improved introducing `ruff` and typing annotations
   all over the codebase
 
 .. note::
     PlotPy V2 is fully typed using Python 3.8+ type annotations.
     This means that you can use your IDE to get autocompletion and type checking
     (e.g. with VSCode, Visual Studio, etc.).
     This is a major improvement when you write code using PlotPy V2:
```

### Comparing `PlotPy-2.3.0/doc/intro/overview.rst` & `plotpy-2.3.1/doc/intro/overview.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/requirements.rst` & `plotpy-2.3.1/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/doc/update_requirements.py` & `plotpy-2.3.1/doc/update_requirements.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/__init__.py` & `plotpy-2.3.1/plotpy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     * Python Package Index: `PyPI`_
     * Bug reports and feature requests: `GitHub`_
 
 .. _PyPI: https://pypi.python.org/pypi/plotpy
 .. _GitHub: https://github.com/PierreRaybaut/plotpy
 """
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 __VERSION__ = tuple([int(number) for number in __version__.split(".")])
 
 # --- Important note: DATAPATH and LOCALEPATH are used by guidata.configtools
 # ---                 to retrieve data and translation files paths
 #
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (e.g. icons) and translations:
```

### Comparing `PlotPy-2.3.0/plotpy/builder/__init__.py` & `plotpy-2.3.1/plotpy/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/annotation.py` & `plotpy-2.3.1/plotpy/builder/annotation.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/curvemarker.py` & `plotpy-2.3.1/plotpy/builder/curvemarker.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/image.py` & `plotpy-2.3.1/plotpy/builder/image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/label.py` & `plotpy-2.3.1/plotpy/builder/label.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/plot.py` & `plotpy-2.3.1/plotpy/builder/plot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/builder/shape.py` & `plotpy-2.3.1/plotpy/builder/shape.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/config.py` & `plotpy-2.3.1/plotpy/config.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/constants.py` & `plotpy-2.3.1/plotpy/constants.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/coords.py` & `plotpy-2.3.1/plotpy/coords.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/colormaps_default.json` & `plotpy-2.3.1/plotpy/data/colormaps_default.json`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/apply.png` & `plotpy-2.3.1/plotpy/data/icons/apply.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/arredit.png` & `plotpy-2.3.1/plotpy/data/icons/arredit.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/arrow_down.png` & `plotpy-2.3.1/plotpy/data/icons/arrow_down.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/arrow_up.png` & `plotpy-2.3.1/plotpy/data/icons/arrow_up.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/autorefresh.png` & `plotpy-2.3.1/plotpy/data/icons/autorefresh.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/autoscale.png` & `plotpy-2.3.1/plotpy/data/icons/autoscale.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/axes.png` & `plotpy-2.3.1/plotpy/data/icons/axes.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/copy.png` & `plotpy-2.3.1/plotpy/data/icons/copy.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/copytoclipboard.png` & `plotpy-2.3.1/plotpy/data/icons/copytoclipboard.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/csapplylut.png` & `plotpy-2.3.1/plotpy/data/icons/csapplylut.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/csection_oblique.png` & `plotpy-2.3.1/plotpy/data/icons/csection_oblique.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/curve_downsample.png` & `plotpy-2.3.1/plotpy/data/icons/curve_downsample.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/edit.png` & `plotpy-2.3.1/plotpy/data/icons/edit.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/edit_point_selection.png` & `plotpy-2.3.1/plotpy/data/icons/edit_point_selection.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/edit.png` & `plotpy-2.3.1/plotpy/data/icons/editors/edit.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/edit_add.png` & `plotpy-2.3.1/plotpy/data/icons/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/editcopy.png` & `plotpy-2.3.1/plotpy/data/icons/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/editdelete.png` & `plotpy-2.3.1/plotpy/data/icons/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/editpaste.png` & `plotpy-2.3.1/plotpy/data/icons/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/fileimport.png` & `plotpy-2.3.1/plotpy/data/icons/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/filesave.png` & `plotpy-2.3.1/plotpy/data/icons/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/editors/imshow.png` & `plotpy-2.3.1/plotpy/data/icons/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/eraser.png` & `plotpy-2.3.1/plotpy/data/icons/eraser.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/exit.png` & `plotpy-2.3.1/plotpy/data/icons/exit.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/export.png` & `plotpy-2.3.1/plotpy/data/icons/export.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/fileclose.png` & `plotpy-2.3.1/plotpy/data/icons/fileclose.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/fileimport.png` & `plotpy-2.3.1/plotpy/data/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/fileopen.png` & `plotpy-2.3.1/plotpy/data/icons/fileopen.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filesave.png` & `plotpy-2.3.1/plotpy/data/icons/filesave.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filesaveas.png` & `plotpy-2.3.1/plotpy/data/icons/filesaveas.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/doc.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/gif.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/html.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/jpg.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/pdf.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/png.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/pps.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/ps.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/tar.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/tgz.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/tif.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/txt.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/xls.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/filetypes/zip.png` & `plotpy-2.3.1/plotpy/data/icons/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/funct.png` & `plotpy-2.3.1/plotpy/data/icons/funct.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/imagestats.png` & `plotpy-2.3.1/plotpy/data/icons/imagestats.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/items/annotation.png` & `plotpy-2.3.1/plotpy/data/icons/items/annotation.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/items/histogram2d.png` & `plotpy-2.3.1/plotpy/data/icons/items/histogram2d.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/items/image.png` & `plotpy-2.3.1/plotpy/data/icons/items/image.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/items/label.png` & `plotpy-2.3.1/plotpy/data/icons/items/label.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/magnifier.png` & `plotpy-2.3.1/plotpy/data/icons/magnifier.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/multipoint_selection.png` & `plotpy-2.3.1/plotpy/data/icons/multipoint_selection.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/plotpy-banner.svg` & `plotpy-2.3.1/plotpy/data/icons/plotpy-banner.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/plotpy-vertical.svg` & `plotpy-2.3.1/plotpy/data/icons/plotpy-vertical.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/plotpy.svg` & `plotpy-2.3.1/plotpy/data/icons/plotpy.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/print.png` & `plotpy-2.3.1/plotpy/data/icons/print.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/python.png` & `plotpy-2.3.1/plotpy/data/icons/python.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/quickview.png` & `plotpy-2.3.1/plotpy/data/icons/quickview.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/rectangular_select.png` & `plotpy-2.3.1/plotpy/data/icons/rectangular_select.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/refresh.png` & `plotpy-2.3.1/plotpy/data/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/save_all.png` & `plotpy-2.3.1/plotpy/data/icons/save_all.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/selection.png` & `plotpy-2.3.1/plotpy/data/icons/selection.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/settings.png` & `plotpy-2.3.1/plotpy/data/icons/settings.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/shapes/circle.png` & `plotpy-2.3.1/plotpy/data/icons/shapes/circle.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/shapes/contour.png` & `plotpy-2.3.1/plotpy/data/icons/shapes/contour.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/shapes/ellipse_shape.png` & `plotpy-2.3.1/plotpy/data/icons/shapes/ellipse_shape.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/shapes/oblique_rectangle.png` & `plotpy-2.3.1/plotpy/data/icons/shapes/oblique_rectangle.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/snapshot.png` & `plotpy-2.3.1/plotpy/data/icons/snapshot.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/trimage_lock.png` & `plotpy-2.3.1/plotpy/data/icons/trimage_lock.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/data/icons/trimage_unlock.png` & `plotpy-2.3.1/plotpy/data/icons/trimage_unlock.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/events.py` & `plotpy-2.3.1/plotpy/events.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/__init__.py` & `plotpy-2.3.1/plotpy/external/sliders/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_generic_range_slider.py` & `plotpy-2.3.1/plotpy/external/sliders/_generic_range_slider.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_generic_slider.py` & `plotpy-2.3.1/plotpy/external/sliders/_generic_slider.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_labeled.py` & `plotpy-2.3.1/plotpy/external/sliders/_labeled.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     QStyle,
     QStyleOptionSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
 from ._misc import signals_blocked
-
 from ._sliders import QDoubleRangeSlider, QDoubleSlider, QRangeSlider
 
 
 class LabelPosition(IntEnum):
     NoLabel = 0
     LabelsAbove = auto()
     LabelsBelow = auto()
@@ -129,22 +128,20 @@
 class QLabeledSlider(_SliderProxy, QAbstractSlider):
     editingFinished = Signal()
 
     _slider_class = QSlider
     _slider: QSlider
 
     @overload
-    def __init__(self, parent: QWidget | None = ...) -> None:
-        ...
+    def __init__(self, parent: QWidget | None = ...) -> None: ...
 
     @overload
     def __init__(
         self, orientation: Qt.Orientation, parent: QWidget | None = ...
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         parent, orientation = _handle_overloaded_slider_sig(args, kwargs)
 
         super().__init__(parent)
         # accept focus events
         fp = self.style().styleHint(QStyle.StyleHint.SH_Button_FocusPolicy)
@@ -259,22 +256,20 @@
     _slider_class = QDoubleSlider
     _slider: QDoubleSlider
     _fvalueChanged = Signal(float)
     _fsliderMoved = Signal(float)
     _frangeChanged = Signal(float, float)
 
     @overload
-    def __init__(self, parent: QWidget | None = ...) -> None:
-        ...
+    def __init__(self, parent: QWidget | None = ...) -> None: ...
 
     @overload
     def __init__(
         self, orientation: Qt.Orientation, parent: QWidget | None = ...
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.setDecimals(2)
 
     def _setValue(self, value: float) -> None:
         """Convert the value from float to int before setting the slider value."""
@@ -296,22 +291,20 @@
     _valueChanged = Signal(tuple)
     editingFinished = Signal()
 
     _slider_class = QRangeSlider
     _slider: QRangeSlider
 
     @overload
-    def __init__(self, parent: QWidget | None = ...) -> None:
-        ...
+    def __init__(self, parent: QWidget | None = ...) -> None: ...
 
     @overload
     def __init__(
         self, orientation: Qt.Orientation, parent: QWidget | None = ...
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         parent, orientation = _handle_overloaded_slider_sig(args, kwargs)
         super().__init__(parent)
         self._rename_signals()
 
         self.setAttribute(Qt.WidgetAttribute.WA_ShowWithoutActivating)
@@ -541,22 +534,20 @@
 
 class QLabeledDoubleRangeSlider(QLabeledRangeSlider):
     _slider_class = QDoubleRangeSlider
     _slider: QDoubleRangeSlider
     _frangeChanged = Signal(float, float)
 
     @overload
-    def __init__(self, parent: QWidget | None = ...) -> None:
-        ...
+    def __init__(self, parent: QWidget | None = ...) -> None: ...
 
     @overload
     def __init__(
         self, orientation: Qt.Orientation, parent: QWidget | None = ...
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.setDecimals(2)
 
     def _rename_signals(self) -> None:
         super()._rename_signals()
```

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_misc.py` & `plotpy-2.3.1/plotpy/external/sliders/_misc.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_range_style.py` & `plotpy-2.3.1/plotpy/external/sliders/_range_style.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/external/sliders/_sliders.py` & `plotpy-2.3.1/plotpy/external/sliders/_sliders.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/interfaces/__init__.py` & `plotpy-2.3.1/plotpy/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/interfaces/items.py` & `plotpy-2.3.1/plotpy/interfaces/items.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/interfaces/plotmanager.py` & `plotpy-2.3.1/plotpy/interfaces/plotmanager.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/io.py` & `plotpy-2.3.1/plotpy/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     logger = logging.getLogger("pydicom")
     logger.setLevel(logging.CRITICAL)
 
     # This import statement must stay here because the purpose of this function
     # is to check if pydicom is installed:
     # pylint: disable=import-outside-toplevel
     # pylint: disable=import-error
-    from pydicom import dicomio  # type:ignore
+    from pydicom import dicomio  # type:ignore # noqa: F401
 
     logger.setLevel(logging.WARNING)
 
 
 def _imread_dcm(filename, **kwargs):
     """Open DICOM image with pydicom and return a NumPy array"""
     # pylint: disable=import-outside-toplevel
```

### Comparing `PlotPy-2.3.0/plotpy/items/__init__.py` & `plotpy-2.3.1/plotpy/items/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/annotation.py` & `plotpy-2.3.1/plotpy/items/annotation.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/contour.py` & `plotpy-2.3.1/plotpy/items/contour.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/curve/base.py` & `plotpy-2.3.1/plotpy/items/curve/base.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/curve/errorbar.py` & `plotpy-2.3.1/plotpy/items/curve/errorbar.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/grid.py` & `plotpy-2.3.1/plotpy/items/grid.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/histogram.py` & `plotpy-2.3.1/plotpy/items/histogram.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/__init__.py` & `plotpy-2.3.1/plotpy/items/image/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/base.py` & `plotpy-2.3.1/plotpy/items/image/base.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/filter.py` & `plotpy-2.3.1/plotpy/items/image/filter.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/image_items.py` & `plotpy-2.3.1/plotpy/items/image/image_items.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/masked.py` & `plotpy-2.3.1/plotpy/items/image/masked.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/misc.py` & `plotpy-2.3.1/plotpy/items/image/misc.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/image/transform.py` & `plotpy-2.3.1/plotpy/items/image/transform.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/label.py` & `plotpy-2.3.1/plotpy/items/label.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from guidata.dataset import update_dataset
 from guidata.utils.misc import assert_interfaces_valid
 from qtpy import QtCore as QC
 from qtpy import QtGui as QG
 from qwt import QwtPlotItem
 
 from plotpy.config import CONF, _
+from plotpy.coords import canvas_to_axes
 from plotpy.interfaces import IBasePlotItem, ISerializableType, IShapeItemType
 from plotpy.items.curve.base import CurveItem
 from plotpy.styles.label import LabelParam
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
@@ -424,36 +425,38 @@
     def move_local_shape(self, old_pos: QPointF, new_pos: QPointF) -> None:
         """Translate the shape such that old_pos becomes new_pos in canvas coordinates
 
         Args:
             old_pos: Old position
             new_pos: New position
         """
+        plot = self.plot()
+        if plot is None:
+            return
         if self.G in ANCHORS or not self.labelparam.move_anchor:
             # Move canvas offset
             lx, ly = self.C
             lx += new_pos.x() - old_pos.x()
             ly += new_pos.y() - old_pos.y()
             self.C = lx, ly
             self.labelparam.xc, self.labelparam.yc = lx, ly
+            lx0, ly0 = canvas_to_axes(self, old_pos)
+            lx1, ly1 = canvas_to_axes(self, new_pos)
         else:
             # Move anchor
-            plot = self.plot()
-            if plot is None:
-                return
             lx0, ly0 = self.G
             cx = plot.transform(self.xAxis(), lx0)
             cy = plot.transform(self.yAxis(), ly0)
             cx += new_pos.x() - old_pos.x()
             cy += new_pos.y() - old_pos.y()
             lx1 = plot.invTransform(self.xAxis(), cx)
             ly1 = plot.invTransform(self.yAxis(), cy)
             self.G = lx1, ly1
             self.labelparam.xg, self.labelparam.yg = lx1, ly1
-            plot.SIG_ITEM_MOVED.emit(self, lx0, ly0, lx1, ly1)
+        plot.SIG_ITEM_MOVED.emit(self, lx0, ly0, lx1, ly1)
 
     def move_with_selection(self, delta_x: float, delta_y: float) -> None:
         """Translate the item together with other selected items
 
         Args:
             delta_x: Translation in plot coordinates along x-axis
             delta_y: Translation in plot coordinates along y-axis
@@ -702,15 +705,15 @@
             legenditems: Legend items
 
         Returns:
             tuple: Tuple with four elements: (TW, TH, width, height)
         """
         width = 0
         height = 0
-        for text, _, _, _ in legenditems:
+        for text, _, _, _ in legenditems:  # noqa
             sz = text.size()
             if sz.width() > width:
                 width = sz.width()
             if sz.height() > height:
                 height = sz.height()
 
         TW = LEGEND_SPACEH * 3 + LEGEND_WIDTH + width
```

### Comparing `PlotPy-2.3.0/plotpy/items/polygonmap.py` & `plotpy-2.3.1/plotpy/items/polygonmap.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/axis.py` & `plotpy-2.3.1/plotpy/items/shape/axis.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/base.py` & `plotpy-2.3.1/plotpy/items/shape/base.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/ellipse.py` & `plotpy-2.3.1/plotpy/items/shape/ellipse.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/marker.py` & `plotpy-2.3.1/plotpy/items/shape/marker.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/point.py` & `plotpy-2.3.1/plotpy/items/shape/point.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/polygon.py` & `plotpy-2.3.1/plotpy/items/shape/polygon.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/range.py` & `plotpy-2.3.1/plotpy/items/shape/range.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,17 @@
             dosignal: True to emit the SIG_RANGE_CHANGED signal
         """
         self._min = _min
         self._max = _max
         if dosignal:
             self.plot().SIG_RANGE_CHANGED.emit(self, self._min, self._max)
 
-    def move_shape(self, old_pos: QC.QPointF, new_pos: QC.QPointF) -> None:
+    def move_shape(
+        self, old_pos: tuple[float, float], new_pos: tuple[float, float]
+    ) -> None:
         """Translate the shape such that old_pos becomes new_pos in axis coordinates
 
         Args:
             old_pos: Old position
             new_pos: New position
         """
         dx = new_pos[0] - old_pos[0]
```

### Comparing `PlotPy-2.3.0/plotpy/items/shape/rectangle.py` & `plotpy-2.3.1/plotpy/items/shape/rectangle.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/segment.py` & `plotpy-2.3.1/plotpy/items/shape/segment.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/items/shape/svg.py` & `plotpy-2.3.1/plotpy/items/shape/svg.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/locale/fr/LC_MESSAGES/plotpy.mo` & `plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/plotpy.mo`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/lutrange.py` & `plotpy-2.3.1/plotpy/lutrange.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/mathutils/arrayfuncs.py` & `plotpy-2.3.1/plotpy/mathutils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/mathutils/colormap.py` & `plotpy-2.3.1/plotpy/mathutils/colormap.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/mathutils/geometry.py` & `plotpy-2.3.1/plotpy/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/mathutils/scaler.py` & `plotpy-2.3.1/plotpy/mathutils/scaler.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/panels/base.py` & `plotpy-2.3.1/plotpy/panels/base.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/panels/contrastadjustment.py` & `plotpy-2.3.1/plotpy/panels/contrastadjustment.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/panels/csection/csitem.py` & `plotpy-2.3.1/plotpy/panels/csection/csitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,18 @@
     return x, y
 
 
 def compute_oblique_section(item, obj, debug=False):
     """Return oblique averaged cross section"""
     global TEMP_ITEM
 
+    if obj.plot() is None:
+        # Item has not yet been added to the plot
+        return np.array([]), np.array([])
+
     xa, ya, xb, yb = obj.get_bounding_rect_coords()
     x0, y0, x1, y1, x2, y2, x3, y3 = obj.get_rect()
 
     getcpi = item.get_closest_pixel_indexes
     ixa, iya = getcpi(xa, ya)
     ixb, iyb = getcpi(xb, yb)
     ix0, iy0 = getcpi(x0, y0)
```

### Comparing `PlotPy-2.3.0/plotpy/panels/csection/csplot.py` & `plotpy-2.3.1/plotpy/panels/csection/csplot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/panels/csection/cswidget.py` & `plotpy-2.3.1/plotpy/panels/csection/cswidget.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/panels/itemlist.py` & `plotpy-2.3.1/plotpy/panels/itemlist.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/plot/base.py` & `plotpy-2.3.1/plotpy/plot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,17 @@
         for axis in unused_axes:
             self.enableAxis(axis, False)
 
         if has_image:
             self.enableAxis(self.colormap_axis)
 
     def get_items(
-        self, z_sorted: bool = False, item_type: itf.IBasePlotItem | None = None
+        self,
+        z_sorted: bool = False,
+        item_type: type[itf.IItemType | itf.IBasePlotItem] | None = None,
     ) -> list[itf.IBasePlotItem]:
         """Return widget's item list
         (items are based on IBasePlotItem's interface)
 
         Args:
             z_sorted (bool): sort items by z order (optional, default=False)
             item_type (IItemType): the item type (optional, default=None)
```

### Comparing `PlotPy-2.3.0/plotpy/plot/interactive.py` & `plotpy-2.3.1/plotpy/plot/interactive.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/plot/manager.py` & `plotpy-2.3.1/plotpy/plot/manager.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/plot/plotwidget.py` & `plotpy-2.3.1/plotpy/plot/plotwidget.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/pyplot.py` & `plotpy-2.3.1/plotpy/pyplot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/__init__.py` & `plotpy-2.3.1/plotpy/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/axes.py` & `plotpy-2.3.1/plotpy/styles/axes.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/base.py` & `plotpy-2.3.1/plotpy/styles/base.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/curve.py` & `plotpy-2.3.1/plotpy/styles/curve.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/errorbar.py` & `plotpy-2.3.1/plotpy/styles/errorbar.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/histogram.py` & `plotpy-2.3.1/plotpy/styles/histogram.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/image.py` & `plotpy-2.3.1/plotpy/styles/image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/label.py` & `plotpy-2.3.1/plotpy/styles/label.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/polygonmap.py` & `plotpy-2.3.1/plotpy/styles/polygonmap.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/styles/shape.py` & `plotpy-2.3.1/plotpy/styles/shape.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/__init__.py` & `plotpy-2.3.1/plotpy/tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ===================
 """
 
 import os.path as osp
 
 from guidata.configtools import get_module_data_path
 
-import plotpy
+import plotpy  # noqa: F401
 
 TESTDATAPATH = get_module_data_path("plotpy", osp.join("tests", "data"))
 
 
 def get_path(filename: str) -> str:
     """Return absolute path of test file"""
     return osp.join(TESTDATAPATH, filename)
```

### Comparing `PlotPy-2.3.0/plotpy/tests/benchmarks/test_benchmarks.py` & `plotpy-2.3.1/plotpy/tests/benchmarks/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/benchmarks/test_bigimages.py` & `plotpy-2.3.1/plotpy/tests/benchmarks/test_bigimages.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/benchmarks/test_loadtest.py` & `plotpy-2.3.1/plotpy/tests/benchmarks/test_loadtest.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data/brain.png` & `plotpy-2.3.1/plotpy/tests/data/brain.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data/brain_cylinder.png` & `plotpy-2.3.1/plotpy/tests/data/brain_cylinder.png`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data/mr-brain.dcm` & `plotpy-2.3.1/plotpy/tests/data/mr-brain.dcm`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data/svg_target.svg` & `plotpy-2.3.1/plotpy/tests/data/svg_target.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data/svg_tool.svg` & `plotpy-2.3.1/plotpy/tests/data/svg_tool.svg`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/data.py` & `plotpy-2.3.1/plotpy/tests/data.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_auto_curve_image.py` & `plotpy-2.3.1/plotpy/tests/features/test_auto_curve_image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_autoscale_shapes.py` & `plotpy-2.3.1/plotpy/tests/features/test_autoscale_shapes.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 # guitest: show
 
 import numpy as np
 from guidata.qthelpers import qt_app_context
 
 from plotpy.builder import make
-from plotpy.items import PolygonShape
 from plotpy.plot import PlotDialog
-from plotpy.styles import ShapeParam
 from plotpy.tools import (
     AnnotatedCircleTool,
     AnnotatedEllipseTool,
     AnnotatedObliqueRectangleTool,
     AnnotatedPointTool,
     AnnotatedRectangleTool,
     AnnotatedSegmentTool,
```

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_builder.py` & `plotpy-2.3.1/plotpy/tests/features/test_builder.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_colormap_editor.py` & `plotpy-2.3.1/plotpy/tests/features/test_colormap_editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,27 +55,27 @@
         editor.set_colormap(new_cmap)
         editor.show()
 
         cmap_tuples = editor.get_colormap().to_tuples()
         cmap_tuples = tuple((int(val * 255 + 1), color) for val, color in cmap_tuples)
         print(
             "Initialization of a new default colormap editor, "
-            "modified post-initialization with the previous colormap with stops scaled by "
-            "255 + 1: ",
+            "modified post-initialization with the previous colormap "
+            "with stops scaled by 255 + 1: ",
             cmap_tuples,
         )
         new_cmap = EditableColormap.from_iterable(cmap_tuples)
         editor = ColorMapEditor(None)
         editor.set_colormap(new_cmap)
         editor.show()
 
         print(
             "Initialization of a new default colormap editor, "
-            "modified post-initialization with the previous colormap where the red stop is "
-            "replaced with a green stop: ",
+            "modified post-initialization with the previous colormap "
+            "where the red stop is replaced with a green stop: ",
             cmap_tuples,
         )
 
         editor = ColorMapEditor(None)
         editor.set_colormap(new_cmap)
         editor.colormap_widget.edit_color_stop(1, None, green)
         editor.show()
```

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_computations.py` & `plotpy-2.3.1/plotpy/tests/features/test_computations.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_contrast.py` & `plotpy-2.3.1/plotpy/tests/features/test_contrast.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_cursors.py` & `plotpy-2.3.1/plotpy/tests/features/test_cursors.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_dicom_image.py` & `plotpy-2.3.1/plotpy/tests/features/test_dicom_image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_fit.py` & `plotpy-2.3.1/plotpy/tests/features/test_fit.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_image_coords.py` & `plotpy-2.3.1/plotpy/tests/features/test_image_coords.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_imagefilter.py` & `plotpy-2.3.1/plotpy/tests/features/test_imagefilter.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,15 +28,19 @@
             yreverse=yreverse,
             type="image",
         )
         image = make.xyimage(x, y, data)
         plot = win.manager.get_plot()
         plot.add_item(image)
         xmin, xmax, ymin, ymax = filter_area
-        ifilter = lambda x, y, data: gaussian_filter(data, 5)
+
+        def ifilter(x, y, data):
+            """Image filter function"""
+            return gaussian_filter(data, 5)
+
         flt = make.imagefilter(xmin, xmax, ymin, ymax, image, filter=ifilter)
         plot.add_item(flt, z=1)
         plot.replot()
         win.show()
 
 
 def test_imagefilter():
```

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_imagesuperp.py` & `plotpy-2.3.1/plotpy/tests/features/test_imagesuperp.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_hdf5.py` & `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_hdf5.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_json.py` & `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_json.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_loadsaveitems_pickle.py` & `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_pickle.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_manager.py` & `plotpy-2.3.1/plotpy/tests/features/test_manager.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_no_auto_tools.py` & `plotpy-2.3.1/plotpy/tests/features/test_no_auto_tools.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_plot_log.py` & `plotpy-2.3.1/plotpy/tests/features/test_plot_log.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_plot_types.py` & `plotpy-2.3.1/plotpy/tests/features/test_plot_types.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_plot_yreverse.py` & `plotpy-2.3.1/plotpy/tests/features/test_plot_yreverse.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_pyplot.py` & `plotpy-2.3.1/plotpy/tests/features/test_pyplot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/features/test_resize.py` & `plotpy-2.3.1/plotpy/tests/features/test_resize.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_annotations.py` & `plotpy-2.3.1/plotpy/tests/items/test_annotations.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_curves.py` & `plotpy-2.3.1/plotpy/tests/items/test_curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # guitest: show
 
 import numpy as np
 from guidata.qthelpers import qt_app_context
 
 from plotpy.builder import make
 from plotpy.tests import vistools as ptv
+from plotpy.tools import CurveStatsTool
 
 
 def test_plot():
     """Curve plotting test"""
     x = np.linspace(-10, 10, 200)
     dy = x / 100.0
     y = np.sin(np.sin(np.sin(x)))
```

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_hist2d.py` & `plotpy-2.3.1/plotpy/tests/items/test_hist2d.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_histogram.py` & `plotpy-2.3.1/plotpy/tests/items/test_histogram.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image.py` & `plotpy-2.3.1/plotpy/tests/items/test_image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image_contour.py` & `plotpy-2.3.1/plotpy/tests/items/test_image_contour.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image_masked.py` & `plotpy-2.3.1/plotpy/tests/items/test_image_masked.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image_masked_xy.py` & `plotpy-2.3.1/plotpy/tests/items/test_image_masked_xy.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image_rgb.py` & `plotpy-2.3.1/plotpy/tests/items/test_image_rgb.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_image_xy.py` & `plotpy-2.3.1/plotpy/tests/items/test_image_xy.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_mandelbrot.py` & `plotpy-2.3.1/plotpy/tests/items/test_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_pcolor.py` & `plotpy-2.3.1/plotpy/tests/items/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_polygons.py` & `plotpy-2.3.1/plotpy/tests/items/test_polygons.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_svgshapes.py` & `plotpy-2.3.1/plotpy/tests/items/test_svgshapes.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # Licensed under the terms of the BSD 3-Clause
 # (see plotpy/LICENSE for details)
 
 """Test showing SVG shapes"""
 
 # guitest: show
 
-import os.path as osp
-
 from guidata.qthelpers import qt_app_context
 
 from plotpy.builder import make
 from plotpy.tests import get_path
 from plotpy.tests import vistools as ptv
```

### Comparing `PlotPy-2.3.0/plotpy/tests/items/test_transform.py` & `plotpy-2.3.1/plotpy/tests/items/test_transform.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_actiontool.py` & `plotpy-2.3.1/plotpy/tests/tools/test_actiontool.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_cross_section.py` & `plotpy-2.3.1/plotpy/tests/tools/test_cross_section.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_cross_section_line.py` & `plotpy-2.3.1/plotpy/tests/tools/test_cross_section_line.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_cross_section_oblique.py` & `plotpy-2.3.1/plotpy/tests/tools/test_cross_section_oblique.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_customize_shape_tool.py` & `plotpy-2.3.1/plotpy/tests/tools/test_customize_shape_tool.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_downsample_curve.py` & `plotpy-2.3.1/plotpy/tests/tools/test_downsample_curve.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_edit_point.py` & `plotpy-2.3.1/plotpy/tests/tools/test_edit_point.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_get_point.py` & `plotpy-2.3.1/plotpy/tests/tools/test_get_point.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_get_points.py` & `plotpy-2.3.1/plotpy/tests/tools/test_get_points.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_get_rectangle.py` & `plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_get_rectangle_with_svg.py` & `plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle_with_svg.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_get_segment.py` & `plotpy-2.3.1/plotpy/tests/tools/test_get_segment.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import numpy as np
 import qtpy.QtCore as QC
 from guidata.env import execenv
 from guidata.qthelpers import qt_app_context
 
 from plotpy.builder import make
-from plotpy.config import _
 from plotpy.coords import axes_to_canvas
 from plotpy.tools import AnnotatedSegmentTool
 from plotpy.widgets.selectdialog import SelectDialog, select_with_shape_tool
 
 SEG_AXES_COORDS = [20, 20, 70, 70]
```

### Comparing `PlotPy-2.3.0/plotpy/tests/tools/test_image_plot_tools.py` & `plotpy-2.3.1/plotpy/tests/tools/test_image_plot_tools.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_aspect_ratio_tool.py` & `plotpy-2.3.1/plotpy/tests/unit/test_aspect_ratio_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import qtpy.QtCore as QC
 from guidata.qthelpers import exec_dialog, qt_app_context
 
 from plotpy.interfaces.items import IImageItemType
 from plotpy.tests.unit.utils import create_window
 from plotpy.tools import AspectRatioTool
```

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_baseplot.py` & `plotpy-2.3.1/plotpy/tests/unit/test_baseplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from guidata.qthelpers import qt_app_context
 from qtpy import QtCore as QC
 from qtpy import QtWidgets as QW
 
 from plotpy.tests import vistools as ptv
 from plotpy.tests.features.test_auto_curve_image import make_curve_image_legend
-from plotpy.tools.curve import DownSamplingTool, EditPointTool, SelectPointsTool
+from plotpy.tools.curve import EditPointTool, SelectPointsTool
 
 
 def test_baseplot_api():
     """Testing BasePlot API"""
     with qt_app_context(exec_loop=True):
         items = make_curve_image_legend()
         win = ptv.show_items(items, wintitle=test_baseplot_api.__doc__)
```

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_builder_annotation.py` & `plotpy-2.3.1/plotpy/tests/unit/test_builder_annotation.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_builder_curve.py` & `plotpy-2.3.1/plotpy/tests/unit/test_builder_curve.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_builder_image.py` & `plotpy-2.3.1/plotpy/tests/unit/test_builder_image.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_builder_shape.py` & `plotpy-2.3.1/plotpy/tests/unit/test_builder_shape.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,15 +52,13 @@
 
 
 def test_builder_svgshape():
     items = []
     svg_path = get_path("svg_target.svg")
     with open(svg_path, "rb") as f:
         svg_data = f.read()
-    x = np.linspace(0, 1, 10)
-    y = x**2
     for shape_str in ("circle", "rectangle", "square"):
         for data_or_path in (svg_data, svg_path):
             items.append(
                 make.svg(shape_str, data_or_path, 0.0, 0.0, 1.0, 1.0, title="title")
             )
     show_items_qtbot(items)
```

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_contour.py` & `plotpy-2.3.1/plotpy/tests/unit/test_contour.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_geometry.py` & `plotpy-2.3.1/plotpy/tests/unit/test_geometry.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_highprecisionxy.py` & `plotpy-2.3.1/plotpy/tests/unit/test_highprecisionxy.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_io.py` & `plotpy-2.3.1/plotpy/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_line.py` & `plotpy-2.3.1/plotpy/tests/unit/test_line.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_line_cross_section_tool.py` & `plotpy-2.3.1/plotpy/tests/unit/test_line_cross_section_tool.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_oblique_cross_section_tool.py` & `plotpy-2.3.1/plotpy/tests/unit/test_oblique_cross_section_tool.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_plot_curve.py` & `plotpy-2.3.1/plotpy/tests/unit/test_plot_curve.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_plot_image.py` & `plotpy-2.3.1/plotpy/tests/unit/test_plot_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Licensed under the terms of the BSD 3-Clause
 # (see plotpy/LICENSE for details)
 
 """Plot Image unit tests"""
 
 import contextlib
@@ -10,14 +9,15 @@
 import numpy as np
 import pytest
 from guidata.qthelpers import exec_dialog, qt_app_context
 
 from plotpy.builder import make
 from plotpy.plot import BasePlot
 from plotpy.tools import ColormapTool, ReverseColormapTool
+from plotpy.tools.image import LockTrImageTool
 
 
 def compute_image():
     """Return a test image as numpy array"""
     N = 2000
     x = np.array(np.linspace(-5, 5, N), np.float32)
     img = np.zeros((N, N), np.float32)
@@ -100,14 +100,32 @@
             item.set_transform(0, 0, 0, 2.0, 3.0)
             plot.do_autoscale()
             bounds3 = item.bounds
             assert bounds3.width() == bounds2.width() * 2.0
             assert bounds3.height() == bounds2.height() * 3.0
 
 
+def test_lock_tr_image():
+    """Test LockTrImageTool"""
+    with qt_app_context(exec_loop=True):
+        win = make.dialog(type="image", toolbar=True)
+        win.show()
+        item = make.trimage(compute_image())
+        # with plot_image(item) as plot:
+        plot = win.manager.get_plot()
+        plot.add_item(item)
+        plot.select_item(item)
+        tool = win.manager.add_tool(LockTrImageTool)
+        tool.activate()
+        assert item.is_locked()
+        tool.activate(False)
+        assert not item.is_locked()
+        exec_dialog(win)
+
+
 @pytest.mark.parametrize("ratio", [1.0, 0.75, 1.5, 2.0, 3.0])
 def test_set_aspect_ratio(ratio):
     """Test BasePlot.set_aspect_ratio method()
 
     It ensures that the new height is correctly set."""
     with qt_app_context(exec_loop=False):
         win = make.dialog(type="image")
```

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_rect_zoom.py` & `plotpy-2.3.1/plotpy/tests/unit/test_rect_zoom.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_seg_dist.py` & `plotpy-2.3.1/plotpy/tests/unit/test_seg_dist.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_styles.py` & `plotpy-2.3.1/plotpy/tests/unit/test_styles.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/unit/test_tools_export.py` & `plotpy-2.3.1/plotpy/tests/unit/test_tools_export.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/vistools.py` & `plotpy-2.3.1/plotpy/tests/vistools.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_dotarraydemo.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_dotarraydemo.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 import numpy as np
 from guidata.configtools import get_image_file_path
 from guidata.qthelpers import qt_app_context
 from qtpy import QtCore as QC
 from qtpy import QtGui as QG
 from qtpy import QtWidgets as QW
 
-import plotpy.config  # Loading icons
-import plotpy.widgets
+import plotpy.config  # Loading icons  # noqa: F401
 from plotpy.interfaces import IImageItemType
 from plotpy.items import RawImageItem
 from plotpy.items.curve.errorbar import vmap
 from plotpy.plot import PlotDialog, PlotOptions
 from plotpy.tools import CopyToClipboardTool, HelpTool, PrintTool, SaveAsTool
 
 if TYPE_CHECKING:
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_filtertest1.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_filtertest1.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import scipy.ndimage as spi
 import scipy.signal as sps
 from guidata.configtools import get_icon
 from guidata.qthelpers import qt_app_context
 from qtpy import QtWidgets as QW
 
-import plotpy.config  # Loading icons
+import plotpy.config  # Loading icons  # noqa: F401
 from plotpy.builder import make
 
 
 class FilterTestWidget(QW.QWidget):
     """
     Filter testing widget
     parent: parent widget (QWidget)
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_filtertest2.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_filtertest2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import scipy.ndimage as spi
 import scipy.signal as sps
 from guidata.configtools import get_icon
 from guidata.qthelpers import qt_app_context, win32_fix_title_bar_background
 from qtpy import QtWidgets as QW
 
-import plotpy.config  # Loading icons
+import plotpy.config  # Loading icons # noqa: F401
 from plotpy.builder import make
 from plotpy.plot import BasePlot, BasePlotOptions
 from plotpy.plot.manager import PlotManager
 
 
 class FilterTestWidget(QW.QWidget):
     """
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_fliprotate.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_fliprotate.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 # Licensed under the terms of the BSD 3-Clause
 # (see plotpy/LICENSE for details)
 
 """Flip/rotate test"""
 
 # guitest: show
 
-from guidata.configtools import get_icon
-from guidata.qthelpers import (
-    add_actions,
-    create_toolbutton,
-    exec_dialog,
-    qt_app_context,
-)
+from guidata.qthelpers import exec_dialog, qt_app_context
 from qtpy import QtWidgets as QW
 
 from plotpy.tests.widgets.test_rotatecrop import create_test_data, imshow
 from plotpy.tools import RotationCenterTool
 from plotpy.widgets.fliprotate import FlipRotateDialog, FlipRotateWidget
 
 
@@ -31,32 +25,20 @@
     return widget
 
 
 def dialog_test(fname):
     """Test the flip/rotate dialog with rotation point changeable"""
     array0, item = create_test_data(fname)
     dlg = FlipRotateDialog(None, toolbar=True)
-    tool = dlg.manager.add_tool(
+    dlg.manager.add_tool(
         RotationCenterTool,
         rotation_center=False,
         rotation_point_move_with_shape=True,
         on_all_items=True,
-        toolbar_id=None,
     )
-    action = tool.action
-
-    rot_point_btn = create_toolbutton(
-        dlg.plot_widget, icon=get_icon("rotationcenter.jpg")
-    )
-    rot_point_btn.setPopupMode(QW.QToolButton.InstantPopup)
-    rotation_tool_menu = QW.QMenu(dlg.plot_widget)
-    add_actions(rotation_tool_menu, (action,))
-    rot_point_btn.setMenu(rotation_tool_menu)
-    dlg.toolbar.addWidget(rot_point_btn)
-
     dlg.transform.set_item(item)
     if exec_dialog(dlg) == QW.QDialog.Accepted:
         array1 = dlg.transform.get_result()
         dlg1 = imshow(array0, title="array0")
         dlg2 = imshow(array1, title="array1")
         return dlg, dlg1, dlg2
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_plot_timecurve.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_plot_timecurve.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_qtdesigner.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_qtdesigner.ui` & `plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.ui`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_resize_dialog.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_resize_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 # guitest: show
 
 import pytest
 from guidata.qthelpers import exec_dialog, qt_app_context
 from qtpy import QtCore as QC
-from qtpy.QtCore import Qt
 
 from plotpy.widgets.resizedialog import ResizeDialog
 
 size_list = [  # new_size, old_size, kepp_size, result[widtg, height, zoom]
     ((150, 100), (300, 200), False, (150, 100, 0.5)),
     ((800, 400), (200, 100), False, (800, 400, 4)),
     ((800, 400), (200, 100), True, (800, 400, 1)),
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_rotatecrop.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_rotatecrop.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         exec_dialog(dlg)
     return dlg
 
 
 def dialog_test(fname="brain.png"):
     """Test the rotate/crop dialog"""
     array0, item = create_test_data(fname)
-    dlg = RotateCropDialog(None)
+    dlg = RotateCropDialog(None, toolbar=True)
     dlg.transform.set_item(item)
     if exec_dialog(dlg) == QW.QDialog.Accepted:
         array1 = dlg.transform.get_result()
         if array0.shape == array1.shape:
             assert (array1 == array0).all()
             imshow(array1 - array0, title="array1-array0")
         else:
```

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_simple_dialog.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_simple_dialog.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_simple_window.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_simple_window.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tests/widgets/test_syncplot.py` & `plotpy-2.3.1/plotpy/tests/widgets/test_syncplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from __future__ import annotations
 
 import numpy as np
 from guidata.qthelpers import qt_app_context
 from qtpy import QtGui as QG
 
 from plotpy.builder import make
-from plotpy.config import _
 from plotpy.plot import BasePlot, PlotOptions
 from plotpy.plot.plotwidget import SyncPlotWindow
 from plotpy.tests.data import gen_2d_gaussian
 
 
 def plot(plot_type, *itemlists):
     """Plot items in SyncPlotDialog"""
```

### Comparing `PlotPy-2.3.0/plotpy/tools/__init__.py` & `plotpy-2.3.1/plotpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/annotation.py` & `plotpy-2.3.1/plotpy/tools/annotation.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/axes.py` & `plotpy-2.3.1/plotpy/tools/axes.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/base.py` & `plotpy-2.3.1/plotpy/tools/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,165 @@
 # -*- coding: utf-8 -*-
+
 from __future__ import annotations
 
 import weakref
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
 
 from guidata.configtools import get_icon
 from qtpy import QtCore as QC
 from qtpy import QtWidgets as QW
 
 from plotpy.constants import SHAPE_Z_OFFSET
 from plotpy.events import (
     RectangularSelectionHandler,
     StatefulEventFilter,
     setup_standard_tool_filter,
 )
 from plotpy.items.shape.rectangle import RectangleShape
 
+if TYPE_CHECKING:
+    from typing import Callable
+
+    from qtpy.QtCore import QPointF
+
+    from plotpy.plot import BasePlot, PlotManager
+
 
 class DefaultToolbarID:
+    """Default toolbar ID"""
+
     pass
 
 
 GuiToolT = TypeVar("GuiToolT", bound="GuiTool")
 
 
 class GuiTool(QC.QObject):
-    """Base class for interactive tool applying on a plot"""
+    """Base class for interactive tool applying on a plot
+
+    Args:
+        manager: plot manager
+        toolbar_id: toolbar ID
+    """
 
-    def __init__(self, manager, toolbar_id=DefaultToolbarID):
+    def __init__(
+        self,
+        manager: PlotManager,
+        toolbar_id: Any | type[DefaultToolbarID] | None = DefaultToolbarID,
+    ) -> None:
         """Constructor"""
         super().__init__()
         self.manager = manager
-        self.parent_tool = None
-        self.plots = set()
+        self.parent_tool: GuiTool | None = None
+        self.plots: set[BasePlot] = set()
 
         # pylint: disable=assignment-from-none
         self.action = self.create_action(manager)
-        self.menu: QW.QMenu | None = self.create_action_menu(manager)
+        self.menu = self.create_action_menu(manager)
 
         if self.menu is not None:
             self.action.setMenu(self.menu)
         if toolbar_id is DefaultToolbarID:
             toolbar = manager.get_default_toolbar()
         else:
             toolbar = manager.get_toolbar(toolbar_id)
         if toolbar is not None:
             self.setup_toolbar(toolbar)
 
-    def create_action(self, manager):
-        """Create and return tool's action"""
+    def create_action(self, manager: PlotManager) -> QW.QAction | None:
+        """Create and return tool's action
+
+        Args:
+            manager: plot manager
+
+        Returns:
+            Tool's action or None (if tool has no action)
+        """
         return None
 
-    def setup_toolbar(self, toolbar):
-        """Setup tool's toolbar"""
+    def setup_toolbar(self, toolbar: QW.QToolBar) -> None:
+        """Setup tool's toolbar
+
+        Args:
+            toolbar: toolbar
+        """
         toolbar.addAction(self.action)
         if self.menu is not None:
             widget = toolbar.widgetForAction(self.action)
-            widget.setPopupMode(QW.QToolButton.InstantPopup)
+            widget.setPopupMode(QW.QToolButton.ToolButtonPopupMode.InstantPopup)
 
-    def create_action_menu(self, manager):
-        """Create and return menu for the tool's action"""
+    def create_action_menu(self, manager: PlotManager) -> QW.QMenu | None:
+        """Create and return menu for the tool's action
+
+        Args:
+            manager: plot manager
+        """
         return None
 
-    def set_parent_tool(self, tool):
-        """Used to organize tools automatically in menu items"""
+    def set_parent_tool(self, tool: GuiToolT) -> None:
+        """Used to organize tools automatically in menu items
+
+        Args:
+            tool: parent tool
+        """
         self.parent_tool = tool
 
-    def register_plot(self, baseplot):
+    def register_plot(self, baseplot: BasePlot) -> None:
         """Every BasePlot using this tool should call register_plot
         to notify the tool about this widget using it
-        """
-        self.plots.add(baseplot)
 
-    def get_active_plot(self):
+        Args:
+            baseplot: base plot
         """
+        self.plots.add(baseplot)
 
-        :return:
-        """
+    def get_active_plot(self) -> BasePlot | None:
+        """Return the currently active BasePlot or None if no plot is active"""
         for plot in self.plots:
             canvas = plot.canvas()
             if canvas.hasFocus():
                 return plot
         if len(self.plots) == 1:
             return list(self.plots)[0]
         return None
 
-    def update_status(self, plot):
-        """called by to allow derived
-        classes to update the states of actions based on the currently
-        active BasePlot
+    def update_status(self, plot: BasePlot) -> None:
+        """Update the status of the tool based on the currently active plot
 
-        can also be called after an action modifying the BasePlot
+        Can also be called after an action modifying the BasePlot
         (e.g. in order to update action states when an item is deselected)
+
+        Args:
+            plot: base plot
         """
         pass
 
-    def setup_context_menu(self, menu, plot):
+    def setup_context_menu(self, menu: QW.QMenu, plot: BasePlot) -> None:
         """If the tool supports it, this method should install an action
-        in the context menu"""
+        in the context menu
+
+        Args:
+            menu: context menu
+            plot: base plot
+        """
         pass
 
 
 class InteractiveTool(GuiTool):
-    """Interactive tool base class"""
+    """Interactive tool base class
+
+    Args:
+        manager: plot manager
+        toolbar_id: toolbar ID
+        title: tool title
+        icon: tool icon
+        tip: tool tip
+        switch_to_default_tool: switch to default tool when finished
+    """
 
     TITLE = None
     ICON = None
     TIP = None
     CURSOR = QC.Qt.CursorShape.CrossCursor
     SWITCH_TO_DEFAULT_TOOL = False  # switch to default tool when finished
 
@@ -114,20 +167,20 @@
     SIG_VALIDATE_TOOL = QC.Signal(object)
 
     #: Signal emitted by InteractiveTool when tool job is finished
     SIG_TOOL_JOB_FINISHED = QC.Signal()
 
     def __init__(
         self,
-        manager,
+        manager: PlotManager,
         toolbar_id=DefaultToolbarID,
-        title=None,
-        icon=None,
-        tip=None,
-        switch_to_default_tool=None,
+        title: str | None = None,
+        icon: str | None = None,
+        tip: str | None = None,
+        switch_to_default_tool: bool | None = None,
     ):
         if title is not None:
             self.TITLE = title
         if icon is not None:
             self.ICON = icon
         if tip is not None:
             self.TIP = tip
@@ -136,33 +189,41 @@
         self.start_state = {}
 
         if switch_to_default_tool is None:
             switch_to_default_tool = self.SWITCH_TO_DEFAULT_TOOL
         if switch_to_default_tool:
             self.SIG_TOOL_JOB_FINISHED.connect(self.manager.activate_default_tool)
 
-    def create_action(self, manager):
-        """Create and return tool's action"""
+    def create_action(self, manager: PlotManager) -> QW.QAction:
+        """Create and return tool's action
+
+        Args:
+            manager: plot manager
+
+        Returns:
+            Tool's action
+        """
         action = manager.create_action(
             self.TITLE, icon=get_icon(self.ICON), tip=self.TIP, triggered=self.activate
         )
         action.setCheckable(True)
         group = self.manager.get_tool_group("interactive")
         group.addAction(action)
         group.triggered.connect(self.interactive_triggered)
         return action
 
-    def cursor(self):
-        """Return tool mouse cursor"""
+    def cursor(self) -> QC.Qt.CursorShape:
+        """Return tool mouse cursor shape"""
         return self.CURSOR
 
-    def register_plot(self, baseplot):
-        """
+    def register_plot(self, baseplot: BasePlot) -> None:
+        """Register plot
 
-        :param baseplot:
+        Args:
+            baseplot: base plot
         """
         # TODO: With the introduction of PlotManager it should
         # be possible to remove the per tool dictionary start_state
         # since all plots from a manager share the same set of tools
         # the State Machine generated by the calls to tool.setup_filter
         # should be the same for all plots. Thus it should be done only once
         # and not once per plot managed by the plot manager
@@ -170,197 +231,283 @@
         filter = baseplot.filter
         start_state = self.setup_filter(baseplot)
         self.start_state[baseplot] = start_state
         curs = self.cursor()
         if curs is not None:
             filter.set_cursor(curs, start_state)
 
-    def interactive_triggered(self, action):
-        """
+    def interactive_triggered(self, action: QW.QAction) -> None:
+        """Slot called when the tool action is triggered
 
-        :param action:
+        Args:
+            action: tool action
         """
         if action is self.action:
             self.activate()
         else:
             self.deactivate()
 
-    def activate(self):
+    def activate(self) -> None:
         """Activate tool"""
         for baseplot, start_state in list(self.start_state.items()):
             baseplot.filter.set_state(start_state, None)
         self.action.setChecked(True)
         self.manager.set_active_tool(self)
 
-    def deactivate(self):
+    def deactivate(self) -> None:
         """Deactivate tool"""
         self.action.setChecked(False)
 
-    def validate(self, filter, event):
-        """
+    def validate(self, filter: StatefulEventFilter, event: QC.QEvent) -> None:
+        """Validate tool action
 
-        :param filter:
-        :param event:
+        Args:
+            filter: event filter
+            event: event
         """
         self.SIG_VALIDATE_TOOL.emit(filter)
         self.SIG_TOOL_JOB_FINISHED.emit()
 
 
 class CommandTool(GuiTool):
-    """Base class for command tools: action, context menu entry"""
+    """Base class for command tools: action, context menu entry
+
+    Args:
+        manager: plot manager
+        title: tool title
+        icon: tool icon
+        tip: tool tip
+        toolbar_id: toolbar ID
+    """
 
     CHECKABLE = False
 
     def __init__(
         self,
-        manager,
-        title,
-        icon=None,
-        tip=None,
+        manager: PlotManager,
+        title: str,
+        icon: str | None = None,
+        tip: str | None = None,
         toolbar_id: Any | type[DefaultToolbarID] | None = DefaultToolbarID,
-    ):
+    ) -> None:
         self.title = title
         if icon and isinstance(icon, str):
             self.icon = get_icon(icon)
         else:
             self.icon = icon
         self.tip = tip
         super().__init__(manager, toolbar_id)
 
-    def create_action(self, manager):
-        """Create and return tool's action"""
+    def create_action(self, manager: PlotManager) -> QW.QAction:
+        """Create and return tool's action
+
+        Args:
+            manager: plot manager
+
+        Returns:
+            Tool's action
+        """
         return manager.create_action(
             self.title,
             icon=self.icon,
             tip=self.tip,
             triggered=self.activate,
             checkable=self.CHECKABLE,
         )
 
-    def setup_context_menu(self, menu, plot):
-        """
+    def setup_context_menu(self, menu: QW.QMenu, plot: BasePlot) -> None:
+        """Setup context menu
 
-        :param menu:
-        :param plot:
+        Args:
+            menu: context menu
+            plot: base plot
         """
         menu.addAction(self.action)
 
-    def activate(self, checked=True):
-        """
+    def activate(self, checked: bool = True) -> None:
+        """Activate tool
 
-        :param checked:
+        Args:
+            checked: checked
         """
         plot = self.get_active_plot()
         if plot is not None:
             self.activate_command(plot, checked)
 
-    def activate_command(self, plot, checked):
-        """Activate tool"""
-        pass
+    def activate_command(self, plot: BasePlot, checked: bool) -> None:
+        """Activate tool command
 
-    def set_status_active_item(self, plot):
+        Args:
+            plot: base plot
+            checked: checked
         """
+        pass
+
+    def set_status_active_item(self, plot: BasePlot) -> None:
+        """Set status active item
 
-        :param plot:
+        Args:
+            plot: base plot
         """
         item = plot.get_active_item()
         if item:
             self.action.setEnabled(True)
         else:
             self.action.setEnabled(False)
 
 
 class ActionTool(CommandTool):
-    """Tool that simply associate an action to a tool"""
+    """Tool that simply associate an action to a tool
+
+    Args:
+        manager: plot manager
+        action: action
+        item_types: item types
+        toolbar_id: toolbar ID
+    """
 
     def __init__(
         self,
-        manager,
-        action,
-        item_types=None,
+        manager: PlotManager,
+        action: QW.QAction,
+        item_types: Any | None = None,
         toolbar_id=DefaultToolbarID,
-    ):
+    ) -> None:
         self.associated_action = action
         self.item_types = item_types
         super().__init__(
             manager,
             action.text(),
             action.icon(),
             action.toolTip(),
             toolbar_id=toolbar_id,
         )
 
-    def update_status(self, plot):
-        """Update tool status"""
+    def update_status(self, plot: BasePlot) -> None:
+        """Update the status of the tool based on the currently active plot
+
+        Can also be called after an action modifying the BasePlot
+        (e.g. in order to update action states when an item is deselected)
+
+        Args:
+            plot: base plot
+        """
         if self.item_types is None:
             self.action.setEnabled(True)
         else:
             items = plot.get_selected_items()
             self.action.setEnabled(
                 any(isinstance(item, self.item_types) for item in items)
             )
 
-    def create_action(self, manager):
-        """Create and return tool's action"""
+    def create_action(self, manager: PlotManager) -> QW.QAction:
+        """Create and return tool's action
+
+        Args:
+            manager: plot manager
+
+        Returns:
+            Tool's action
+        """
         return self.associated_action
 
 
 class ToggleTool(CommandTool):
-    """ """
+    """Toggle tool base class
+
+    Args:
+        manager: plot manager
+        title: tool title
+        icon: tool icon
+        tip: tool tip
+        toolbar_id: toolbar ID
+    """
 
     CHECKABLE = True
 
-    def __init__(self, manager, title, icon=None, tip=None, toolbar_id=None):
+    def __init__(
+        self,
+        manager: PlotManager,
+        title: str,
+        icon: str | None = None,
+        tip: str | None = None,
+        toolbar_id: Any | type[DefaultToolbarID] | None = None,
+    ) -> None:
         super().__init__(manager, title, icon, tip, toolbar_id)
 
 
 class PanelTool(ToggleTool):
-    """ """
+    """Panel tool base class
+
+    Args:
+        manager: plot manager
+    """
 
     panel_id = None
     panel_name = None
 
-    def __init__(self, manager):
+    def __init__(self, manager: PlotManager) -> None:
         super().__init__(manager, self.panel_name)
         manager.get_panel(self.panel_id).SIG_VISIBILITY_CHANGED.connect(
             self.action.setChecked
         )
 
-    def activate_command(self, plot, checked):
-        """Activate tool"""
+    def activate_command(self, plot: BasePlot, checked: bool) -> None:
+        """Activate tool command
+
+        Args:
+            plot: base plot
+            checked: checked
+        """
         panel = self.manager.get_panel(self.panel_id)
         panel.setVisible(checked)
 
-    def update_status(self, plot):
-        """
+    def update_status(self, plot: BasePlot) -> None:
+        """Update the status of the tool based on the currently active plot
+
+        Can also be called after an action modifying the BasePlot
+        (e.g. in order to update action states when an item is deselected)
 
-        :param plot:
+        Args:
+            plot: base plot
         """
         panel = self.manager.get_panel(self.panel_id)
         self.action.setChecked(panel.isVisible())
 
 
 class RectangularActionTool(InteractiveTool):
-    """ """
+    """Rectangular action tool base class
+
+    Args:
+        manager: plot manager
+        func: function
+        shape_style: shape style
+        toolbar_id: toolbar ID
+        title: tool title
+        icon: tool icon
+        tip: tool tip
+        fix_orientation: fix orientation
+        switch_to_default_tool: switch to default tool
+    """
 
     SHAPE_STYLE_SECT = "plot"
     SHAPE_STYLE_KEY = "shape/drag"
     AVOID_NULL_SHAPE = False
 
     def __init__(
         self,
-        manager,
-        func,
-        shape_style=None,
-        toolbar_id=DefaultToolbarID,
-        title=None,
-        icon=None,
-        tip=None,
-        fix_orientation=False,
-        switch_to_default_tool=None,
+        manager: PlotManager,
+        func: Callable,
+        shape_style: tuple[str, str] | None = None,
+        toolbar_id: Any | type[DefaultToolbarID] | None = DefaultToolbarID,
+        title: str | None = None,
+        icon: str | None = None,
+        tip: str | None = None,
+        fix_orientation: bool = False,
+        switch_to_default_tool: bool | None = None,
     ):
         self.action_func = func
         self.fix_orientation = fix_orientation
         super().__init__(
             manager,
             toolbar_id,
             title=title,
@@ -370,92 +517,123 @@
         )
         if shape_style is not None:
             self.shape_style_sect = shape_style[0]
             self.shape_style_key = shape_style[1]
         else:
             self.shape_style_sect = self.SHAPE_STYLE_SECT
             self.shape_style_key = self.SHAPE_STYLE_KEY
-        self.last_final_shape = None
+        self.last_final_shape: RectangleShape | None = None
         self.switch_to_default_tool = switch_to_default_tool
 
-    def get_last_final_shape(self):
-        """
-
-        :return:
-        """
+    def get_last_final_shape(self) -> RectangleShape | None:
+        """Get last final shape"""
         if self.last_final_shape is not None:
             return self.last_final_shape()
 
-    def set_shape_style(self, shape):
-        """
+    def set_shape_style(self, shape: RectangleShape) -> None:
+        """Set shape style
 
-        :param shape:
+        Args:
+            shape: shape
         """
         shape.set_style(self.shape_style_sect, self.shape_style_key)
 
-    def create_shape(self):
-        """
+    def create_shape(self) -> tuple[RectangleShape, int, int]:
+        """Create shape
 
-        :return:
+        Returns:
+            A tuple with the shape, and the two handles
         """
         shape = RectangleShape(0, 0, 1, 1)
         self.set_shape_style(shape)
         return shape, 0, 2
 
-    def setup_shape(self, shape):
-        """
+    def setup_shape(self, shape: RectangleShape) -> None:
+        """Setup shape
 
-        :param shape:
+        Args:
+            shape: shape
         """
         pass
 
-    def get_shape(self):
-        """Reimplemented RectangularActionTool method"""
+    def get_shape(self) -> tuple[RectangleShape, int, int]:
+        """Get shape
+
+        Returns:
+            A tuple with the shape, and the two handles
+        """
         shape, h0, h1 = self.create_shape()
         self.setup_shape(shape)
         return shape, h0, h1
 
-    def get_final_shape(self, plot, p0, p1):
-        """
+    def get_final_shape(
+        self, plot: BasePlot, p0: QPointF, p1: QPointF
+    ) -> RectangleShape:
+        """Get final shape
+
+        Args:
+            plot: base plot
+            p0: point 0
+            p1: point 1
 
-        :param plot:
-        :param p0:
-        :param p1:
-        :return:
+        Returns:
+            Final shape
         """
         shape, h0, h1 = self.create_shape()
         self.setup_shape(shape)
         plot.add_item_with_z_offset(shape, SHAPE_Z_OFFSET)
         shape.move_local_point_to(h0, p0)
         shape.move_local_point_to(h1, p1)
         self.last_final_shape = weakref.ref(shape)
         return shape
 
-    def get_selection_handler(self, filter, start_state):
+    def get_selection_handler(
+        self, filter: StatefulEventFilter, start_state: int
+    ) -> RectangularSelectionHandler:
+        """Get selection handler
+
+        Args:
+            filter: event filter
+            start_state: start state
+
+        Returns:
+            Selection handler
+        """
         return RectangularSelectionHandler(
             filter, QC.Qt.LeftButton, start_state=start_state
         )
 
-    def setup_filter(self, baseplot):
+    def setup_filter(self, baseplot: BasePlot) -> int:
+        """Setup filter
+
+        Args:
+            baseplot: base plot
+
+        Returns:
+            Start state
+        """
         filter = baseplot.filter
         start_state = filter.new_state()
         handler = self.get_selection_handler(filter, start_state)
         shape, h0, h1 = self.get_shape()
         handler.set_shape(
             shape, h0, h1, self.setup_shape, avoid_null_shape=self.AVOID_NULL_SHAPE
         )
         handler.SIG_END_RECT.connect(self.end_rect)
         return setup_standard_tool_filter(filter, start_state)
 
-    def end_rect(self, filter: StatefulEventFilter, p0: QC.QPointF, p1: QC.QPointF):
-        """
-
-        :param filter:
-        :param p0:
-        :param p1:
+    def end_rect(
+        self, filter: StatefulEventFilter, p0: QC.QPointF, p1: QC.QPointF
+    ) -> None:
+        """End rect (this method is called when the rectangular selection is finished)
+
+        Args:
+            filter: event filter
+            p0: point 0
+            p1: point 1
         """
         plot = filter.plot
         if self.fix_orientation:
             left, right = min(p0.x(), p1.x()), max(p0.x(), p1.x())
             top, bottom = min(p0.y(), p1.y()), max(p0.y(), p1.y())
             self.action_func(plot, QC.QPointF(left, top), QC.QPointF(right, bottom))
         else:
```

### Comparing `PlotPy-2.3.0/plotpy/tools/cross_section.py` & `plotpy-2.3.1/plotpy/tools/cross_section.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/cursor.py` & `plotpy-2.3.1/plotpy/tools/cursor.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/curve.py` & `plotpy-2.3.1/plotpy/tools/curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,16 +727,17 @@
 
             # Get x and y arrays of neigboring points (at coordinates i-1, i, i+1)
             axes_x_points = self.downsampled_x[lower_index_bound:higher_index_bound]
             axes_y_points = self.downsampled_y[lower_index_bound:higher_index_bound]
 
             # Create empty array where axes coordinates will be converted to canvas
             # coordinates
-            canva_x_points, canva_y_points = np.zeros(axes_x_points.size), np.zeros(
-                axes_x_points.size
+            canva_x_points, canva_y_points = (
+                np.zeros(axes_x_points.size),
+                np.zeros(axes_x_points.size),
             )
 
             # Convert axes coordinates to canvas coordinates
             for i, (x, y) in enumerate(zip(axes_x_points, axes_y_points)):
                 new_x, new_y = axes_to_canvas(curve_item, x, y) or (None, None)
                 assert new_x is not None and new_y is not None
                 canva_x_points[i], canva_y_points[i] = new_x, new_y
@@ -851,15 +852,16 @@
             insertion_index: int = param.index + param.index_offset  # type: ignore
             new_x: float = self.__x[insertion_index - 1 : insertion_index + 1].mean()
             self.__x = np.insert(self.__x, insertion_index, new_x)  # type: ignore
             self.__y = np.insert(self.__y, insertion_index, param.value)  # type: ignore
             curve_item.set_data(self.__x, self.__y)
             new_pos = axes_to_canvas(curve_item, new_x, param.value)  # type: ignore
             self.__current_location_marker.move_local_point_to(
-                0, QC.QPointF(*new_pos)  # type: ignore
+                0,
+                QC.QPointF(*new_pos),  # type: ignore
             )
 
     def __get_active_curve_item(self, filter: StatefulEventFilter) -> CurveItem:
         """Get active curve item. Simple method to avoid type checking errors.
 
         Args:
             filter: StatefulEventFilter instance
```

### Comparing `PlotPy-2.3.0/plotpy/tools/image.py` & `plotpy-2.3.1/plotpy/tools/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from guidata.widgets.arrayeditor import ArrayEditor
 from qtpy import QtCore as QC
 from qtpy import QtWidgets as QW
 
 from plotpy import io
 from plotpy.config import _
 from plotpy.constants import ID_CONTRAST, PlotType
+from plotpy.coords import axes_to_canvas
 from plotpy.events import QtDragHandler, setup_standard_tool_filter
 from plotpy.interfaces import (
     IColormapImageItemType,
     IStatsImageItemType,
     IVoiImageItemType,
 )
 from plotpy.items import (
@@ -110,21 +111,18 @@
             Formatted string with informations on current shape or None.
         """
         if self.image_item is None:
             return None
         plot = self.image_item.plot()
         if plot is None:
             return None
-        p0y = plot.transform(0, self.shape.get_points()[0][1])
-        p0x = plot.transform(2, self.shape.get_points()[0][0])
-        p1y = plot.transform(0, self.shape.get_points()[1][1])
-        p1x = plot.transform(2, self.shape.get_points()[1][0])
-        p0 = QC.QPointF(p0x, p0y)
-        p1 = QC.QPointF(p1x, p1y)
-        items = get_items_in_rectangle(plot, p0, p1)
+        x0, y0, x1, y1 = self.shape.get_rect()
+        p0x, p0y = axes_to_canvas(self, x0, y0)
+        p1x, p1y = axes_to_canvas(self, x1, y1)
+        items = get_items_in_rectangle(plot, QC.QPointF(p0x, p0y), QC.QPointF(p1x, p1y))
         if len(items) >= 1:
             sorted_items = [
                 it for it in sorted(items, key=lambda obj: obj.z()) if it.isVisible()
             ]
             if len(sorted_items) >= 1:
                 self.image_item = sorted_items[-1]
             else:
@@ -450,17 +448,15 @@
     and saving).
 
     Args:
         manager: PlotManager Instance
         toolbar_id: Toolbar Id to use. Defaults to DefaultToolbarID.
     """
 
-    def __init__(
-        self, manager: PlotManager, toolbar_id=DefaultToolbarID
-    ) -> None:  # noqa: F821
+    def __init__(self, manager: PlotManager, toolbar_id=DefaultToolbarID) -> None:  # noqa: F821
         super().__init__(
             manager,
             _("Colormap"),
             tip=_("Select colormap for active image"),
             toolbar_id=toolbar_id,
         )
         self._active_colormap: EditableColormap = ALL_COLORMAPS["jet"]
@@ -482,14 +478,15 @@
             or not isinstance(self.action, QC.QObject)
             or not isinstance(self.action.text(), str)
         ):
             return
         manager = ColorMapManager(
             plot.parent(), active_colormap=self._active_colormap.name
         )
+        manager.SIG_APPLY_COLORMAP.connect(self.update_plot)
         if exec_dialog(manager) and (cmap := manager.get_colormap()) is not None:
             self.activate_cmap(cmap)
 
     def activate_cmap(self, cmap: str | EditableColormap) -> None:
         """Activate the given colormap. Supports mutliple input types.
 
         Args:
@@ -498,42 +495,53 @@
         assert isinstance(cmap, (str, EditableColormap))
         if isinstance(cmap, str):
             self._active_colormap = get_cmap(cmap)
         else:
             self._active_colormap = cmap
         plot: BasePlot = self.get_active_plot()
         if self._active_colormap is not None and plot is not None:
-            items = get_selected_images(plot, IColormapImageItemType)
-            for item in items:
-                param: BaseImageParam = item.param
-                param.colormap = self._active_colormap.name
-                param.update_item(item)
-                plot.SIG_ITEM_PARAMETERS_CHANGED.emit(item)
-            self.action.setText(_("Colormap: %s") % self._active_colormap.name)
-            plot.invalidate()
+            self.update_plot(self._active_colormap.name)
             self.update_status(plot)
 
+    def update_plot(self, cmap: str) -> None:
+        """Update the plot with the given colormap.
+
+        Args:
+            cmap: Colormap name
+        """
+        plot: BasePlot = self.get_active_plot()
+        items = get_selected_images(plot, IColormapImageItemType)
+        for item in items:
+            param: BaseImageParam = item.param
+            param.colormap = cmap
+            param.update_item(item)
+            plot.SIG_ITEM_PARAMETERS_CHANGED.emit(item)
+        plot.invalidate()
+
     def update_status(self, plot: BasePlot) -> None:
         """Update tool status if the plot type is not PlotType.CURVE.
 
         Args:
             plot: Plot Instance
         """
         if update_image_tool_status(self, plot):
             item: BaseImageItem = plot.get_last_active_item(IColormapImageItemType)
             icon = self.default_icon
+            cmap_name = "jet"
             if item:
                 self.action.setEnabled(True)
                 cmap = item.get_color_map()
                 if cmap is not None:
                     icon = build_icon_from_cmap_name(cmap.name)
                     self._active_colormap = get_cmap(cmap.name)
+                    cmap_name = cmap.name
             else:
                 self.action.setEnabled(False)
                 self._active_colormap = ALL_COLORMAPS["jet"]
+            self.action.setText(_("Colormap: %s") % cmap_name)
             self.action.setIcon(icon)
 
 
 class ReverseColormapTool(ToggleTool):
     """Togglable tool to reverse colormap
 
     Args:
```

### Comparing `PlotPy-2.3.0/plotpy/tools/item.py` & `plotpy-2.3.1/plotpy/tools/item.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/label.py` & `plotpy-2.3.1/plotpy/tools/label.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/misc.py` & `plotpy-2.3.1/plotpy/tools/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,16 +232,18 @@
 
     def activate_command(self, plot, checked):
         """Activate tool"""
         info = _(
             """<b>Keyboard/mouse shortcuts:</b><br><br>
   - <u>single left-click</u>: item (curve, image, ...) selection<br>
   - <u>single right-click</u>: context-menu relative to selected item<br>
-  - <u>shift</u>: on-active-curve (or image) cursor (+ <u>control</u> to maintain cursor visible)<br>
-  - <u>shift + control</u>: on-active-curve cursor (+ <u>control</u> to maintain cursor visible)<br>
+  - <u>shift</u>: on-active-curve (or image) cursor (+ <u>control</u> to maintain
+cursor visible)<br>
+  - <u>shift + control</u>: on-active-curve cursor (+ <u>control</u> to maintain
+cursor visible)<br>
   - <u>alt</u>: free cursor<br>
   - <u>left-click + mouse move</u>: move item (when available)<br>
   - <u>middle-click + mouse move</u>: pan<br>
   - <u>right-click + mouse move</u>: zoom"""
         )
         info += "<br><hr><br><b>" + _("Information on PlotPy:") + "</b><br><br>"
         info += about.about(html=True)
```

### Comparing `PlotPy-2.3.0/plotpy/tools/plot.py` & `plotpy-2.3.1/plotpy/tools/plot.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/selection.py` & `plotpy-2.3.1/plotpy/tools/selection.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/tools/shape.py` & `plotpy-2.3.1/plotpy/tools/shape.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/about.py` & `plotpy-2.3.1/plotpy/widgets/about.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/basetransform.py` & `plotpy-2.3.1/plotpy/widgets/basetransform.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/colormap/_slider.py` & `plotpy-2.3.1/plotpy/widgets/colormap/_slider.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/colormap/editor.py` & `plotpy-2.3.1/plotpy/widgets/colormap/editor.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/colormap/manager.py` & `plotpy-2.3.1/plotpy/widgets/colormap/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
         the first colormap in the list will be selected by default.
 
         The active colormap cannot be removed. If the active colormap is a custom
         colormap, the remove button will be enabled but a dialog box will warn the user
         that the colormap cannot be removed.
     """
 
+    SIG_APPLY_COLORMAP = QC.Signal(str)
+
     def __init__(
         self,
         parent: QW.QWidget | None = None,
         active_colormap: str | None = None,
     ) -> None:
         super().__init__(parent)
         self.setWindowIcon(get_icon("cmap_edit.png"))
@@ -192,21 +194,24 @@
         self.colormap_editor.colormap_widget.COLORMAP_CHANGED.connect(
             self._changes_not_saved
         )
 
         self._cmap_choice.currentIndexChanged.connect(self.set_colormap)
 
         self.bbox = QW.QDialogButtonBox(
-            QW.QDialogButtonBox.Save
+            QW.QDialogButtonBox.Apply
+            | QW.QDialogButtonBox.Save
             | QW.QDialogButtonBox.Ok
             | QW.QDialogButtonBox.Cancel
         )
         self._changes_saved = True
         self._save_btn = self.bbox.button(QW.QDialogButtonBox.Save)
         self._save_btn.setEnabled(False)  # type: ignore
+        self._apply_btn = self.bbox.button(QW.QDialogButtonBox.Apply)
+        self._apply_btn.setEnabled(False)  # type: ignore
         self.bbox.clicked.connect(self.button_clicked)
 
         dialog_layout = QW.QVBoxLayout()
         dialog_layout.addWidget(select_gbox)
         dialog_layout.addWidget(self._edit_gbox)
         dialog_layout.addWidget(self.bbox)
         self.setLayout(dialog_layout)
@@ -216,25 +221,31 @@
 
     def button_clicked(self, button: QW.QAbstractButton) -> None:
         """Callback function to be called when a button is clicked.
 
         Args:
             button: button clicked
         """
-        if button is self._save_btn:
+        if button is self._apply_btn:
+            if not self.current_changes_saved and not self.save_colormap():
+                return
+            self._apply_btn.setEnabled(False)
+            self.SIG_APPLY_COLORMAP.emit(self.colormap_editor.get_colormap().name)
+        elif button is self._save_btn:
             self.save_colormap()
         elif self.bbox.buttonRole(button) == QW.QDialogButtonBox.AcceptRole:
             self.accept()
         else:
             self.reject()
 
     def _changes_not_saved(self) -> None:
         """Callback function to be called when the colormap is modified. Enables the
         save button and sets the current_changes_saved attribute to False."""
         self._save_btn.setEnabled(True)  # type: ignore
+        self._apply_btn.setEnabled(True)  # type: ignore
         self._changes_saved = False
 
     @property
     def current_changes_saved(self) -> bool:
         """Getter to know if the current colormap has been saved or not.
 
         Returns:
```

### Comparing `PlotPy-2.3.0/plotpy/widgets/colormap/widget.py` & `plotpy-2.3.1/plotpy/widgets/colormap/widget.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/fit.py` & `plotpy-2.3.1/plotpy/widgets/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     FloatItem,
     IntItem,
     StringItem,
     restore_dataset,
     update_dataset,
 )
 from guidata.qthelpers import create_groupbox, exec_dialog
-from numpy import inf  # Do not remove this import (used by optimization funcs)
+
+# Do not remove this import (used by optimization funcs)
+from numpy import inf  # noqa: F401
 from qtpy import QtCore as QC
 from qtpy import QtWidgets as QW
 from qtpy.QtWidgets import QWidget  # only to help intersphinx find QWidget
 from scipy.optimize import fmin, fmin_bfgs, fmin_cg, fmin_l_bfgs_b, fmin_powell, leastsq
 
 from plotpy.builder import make
 from plotpy.config import _
```

### Comparing `PlotPy-2.3.0/plotpy/widgets/fliprotate.py` & `plotpy-2.3.1/plotpy/widgets/fliprotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         self.widget = FlipRotateWidget(parent=parent, options=options, toolbar=toolbar)
         self.setWindowFlags(QC.Qt.WindowType.Window)
 
         buttonhlayout = QW.QHBoxLayout()
         self.add_buttons_to_layout(buttonhlayout, edit)
 
         dialogvlayout = QW.QVBoxLayout()
+        dialogvlayout.addWidget(self.widget.plot_widget.toolbar)
         dialogvlayout.addWidget(self.widget)
         dialogvlayout.addLayout(buttonhlayout)
         self.setLayout(dialogvlayout)
 
         self.transform = self.widget.transform
         self.plot_widget = plot_widget = self.widget.plot_widget
         self.manager = plot_widget.manager
```

### Comparing `PlotPy-2.3.0/plotpy/widgets/imagefile.py` & `plotpy-2.3.1/plotpy/widgets/imagefile.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/qtdesigner.py` & `plotpy-2.3.1/plotpy/widgets/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/resizedialog.py` & `plotpy-2.3.1/plotpy/widgets/resizedialog.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/plotpy/widgets/rotatecrop.py` & `plotpy-2.3.1/plotpy/widgets/rotatecrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         self.widget = RotateCropWidget(parent=parent, options=options, toolbar=toolbar)
         self.setWindowFlags(QC.Qt.WindowType.Window)
 
         buttonhlayout = QW.QHBoxLayout()
         self.add_buttons_to_layout(buttonhlayout, edit)
 
         dialogvlayout = QW.QVBoxLayout()
+        dialogvlayout.addWidget(self.widget.plot_widget.toolbar)
         dialogvlayout.addWidget(self.widget)
         dialogvlayout.addLayout(buttonhlayout)
         self.setLayout(dialogvlayout)
 
         self.transform = self.widget.transform
         self.plot_widget = self.widget.plot_widget
         self.manager = self.widget.plot_widget.manager
```

### Comparing `PlotPy-2.3.0/plotpy/widgets/selectdialog.py` & `plotpy-2.3.1/plotpy/widgets/selectdialog.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/setup.py` & `plotpy-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/arrays.hpp` & `plotpy-2.3.1/src/arrays.hpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/contour2d.c` & `plotpy-2.3.1/src/contour2d.c`

 * *Files 0% similar despite different names*

```diff
@@ -1101,177 +1101,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1310,42 +1310,42 @@
 struct __pyx_obj_9contour2d_CoordGrid;
 struct __pyx_obj_9contour2d_Contour;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -9499,15 +9499,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_x, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_y, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9516,29 +9516,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9549,15 +9549,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9566,29 +9566,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9599,15 +9599,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9616,29 +9616,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9649,15 +9649,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9666,29 +9666,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9699,15 +9699,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9716,29 +9716,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9749,89 +9749,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9839,33 +9839,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9873,96 +9873,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9978,15 +9978,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9994,53 +9994,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -10048,30 +10048,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10086,15 +10086,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10110,15 +10110,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10126,53 +10126,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -10180,30 +10180,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10218,15 +10218,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10242,15 +10242,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10258,53 +10258,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -10312,30 +10312,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10350,176 +10350,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25746,26 +25746,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `PlotPy-2.3.0/src/contour2d.pyx` & `plotpy-2.3.1/src/contour2d.pyx`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/debug.hpp` & `plotpy-2.3.1/src/debug.hpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/histogram2d.c` & `plotpy-2.3.1/src/histogram2d.c`

 * *Files 4% similar despite different names*

```diff
@@ -1026,177 +1026,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1223,42 +1223,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3125,15 +3125,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_tmp.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3142,29 +3142,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3175,15 +3175,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3192,29 +3192,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3225,15 +3225,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3242,29 +3242,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3275,15 +3275,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3292,29 +3292,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3325,15 +3325,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3342,29 +3342,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3375,89 +3375,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3465,33 +3465,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3499,96 +3499,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3604,15 +3604,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3620,53 +3620,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -3674,30 +3674,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3712,15 +3712,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3736,15 +3736,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3752,53 +3752,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -3806,30 +3806,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3844,15 +3844,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3868,15 +3868,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3884,53 +3884,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -3938,30 +3938,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3976,176 +3976,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4244,26 +4244,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 948, __pyx_L1_error)
@@ -4647,15 +4647,15 @@
  * # Licensed under the terms of the BSD 3-Clause
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `PlotPy-2.3.0/src/histogram2d.pyx` & `plotpy-2.3.1/src/histogram2d.pyx`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/mandelbrot.c` & `plotpy-2.3.1/src/mandelbrot.c`

 * *Files 2% similar despite different names*

```diff
@@ -989,177 +989,177 @@
 
 static const char *__pyx_f[] = {
   "src\\mandelbrot.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1186,42 +1186,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2148,15 +2148,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2165,29 +2165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2198,15 +2198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2215,29 +2215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2248,15 +2248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2265,29 +2265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2298,15 +2298,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2315,29 +2315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2348,15 +2348,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2365,29 +2365,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2398,89 +2398,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2488,33 +2488,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2522,96 +2522,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2627,15 +2627,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2643,53 +2643,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -2697,30 +2697,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2735,15 +2735,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2759,15 +2759,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2775,53 +2775,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -2829,30 +2829,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2867,15 +2867,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2891,15 +2891,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2907,53 +2907,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -2961,30 +2961,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2999,176 +2999,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3258,26 +3258,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 948, __pyx_L1_error)
@@ -3627,15 +3627,15 @@
  * # Licensed under the terms of the BSD 3-Clause
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-y6qccuoo/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `PlotPy-2.3.0/src/mandelbrot.pyx` & `plotpy-2.3.1/src/mandelbrot.pyx`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/pcolor.cpp` & `plotpy-2.3.1/src/pcolor.cpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/points.hpp` & `plotpy-2.3.1/src/points.hpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/scaler.cpp` & `plotpy-2.3.1/src/scaler.cpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/scaler.hpp` & `plotpy-2.3.1/src/scaler.hpp`

 * *Files identical despite different names*

### Comparing `PlotPy-2.3.0/src/traits.hpp` & `plotpy-2.3.1/src/traits.hpp`

 * *Files identical despite different names*

