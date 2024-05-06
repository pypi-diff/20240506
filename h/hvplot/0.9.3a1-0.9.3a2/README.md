# Comparing `tmp/hvplot-0.9.3a1.tar.gz` & `tmp/hvplot-0.9.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvplot-0.9.3a1.tar", last modified: Fri Apr 19 09:55:33 2024, max compression
+gzip compressed data, was "hvplot-0.9.3a2.tar", last modified: Fri Apr 19 17:52:31 2024, max compression
```

## Comparing `hvplot-0.9.3a1.tar` & `hvplot-0.9.3a2.tar`

### file list

```diff
@@ -1,221 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/binder/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/binder/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/conda.recipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/conda.recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.917921 hvplot-0.9.3a1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.917921 hvplot-0.9.3a1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.925921 hvplot-0.9.3a1/doc/_static/home/
--rw-r--r--   0 runner    (1001) docker     (127)   198618 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/bokeh.gif
--rw-r--r--   0 runner    (1001) docker     (127)   244779 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/dask.gif
--rw-r--r--   0 runner    (1001) docker     (127)   873325 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/explorer.gif
--rw-r--r--   0 runner    (1001) docker     (127)    47722 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/geo.gif
--rw-r--r--   0 runner    (1001) docker     (127)   702643 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/geopandas.gif
--rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/intake.gif
--rw-r--r--   0 runner    (1001) docker     (127)    70800 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_hvplot.gif
--rw-r--r--   0 runner    (1001) docker     (127)    72465 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_pandas.gif
--rw-r--r--   0 runner    (1001) docker     (127)   173838 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_xarray.gif
--rw-r--r--   0 runner    (1001) docker     (127)   267815 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/large_data.gif
--rw-r--r--   0 runner    (1001) docker     (127)   109054 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/layout.gif
--rw-r--r--   0 runner    (1001) docker     (127)    84928 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (127)    36604 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/networkx.gif
--rw-r--r--   0 runner    (1001) docker     (127)    24841 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)    95678 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/pandas.gif
--rw-r--r--   0 runner    (1001) docker     (127)   116788 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/plotly.gif
--rw-r--r--   0 runner    (1001) docker     (127)   184170 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/widgets.gif
--rw-r--r--   0 runner    (1001) docker     (127)   241968 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/xarray.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.925921 hvplot-0.9.3a1/doc/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)   194737 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/images/heat_and_trees.png
--rw-r--r--   0 runner    (1001) docker     (127)   182260 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/images/portfolio.png
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo_horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo_stacked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/about.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   359182 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (127)  1080507 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151250 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)   463297 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (127)  1007817 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/streamz_demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/developer_guide/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.909921 hvplot-0.9.3a1/doc/governance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/governance/project-docs/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/MEMBERS.md
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.909921 hvplot-0.9.3a1/doc/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.933921 hvplot-0.9.3a1/doc/reference/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.937921 hvplot-0.9.3a1/doc/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/violin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    32456 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/releases.md
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/roadmap.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/topics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/doc/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21995 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Large_Timeseries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25917 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    31550 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22152 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23107 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/doc/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/images/simple.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.10-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.11-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.11-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.12-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.8-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.9-tests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/backend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   109238 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/cudf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/datasets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/fugue.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/ibis.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/intake.py
--rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21430 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/networkx.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/andrews_curves.py
--rw-r--r--   0 runner    (1001) docker     (127)    80862 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/lag_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/scatter_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/polars.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/streamz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.949921 hvplot-0.9.3a1/hvplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.949921 hvplot-0.9.3a1/hvplot/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/data/RGB-red.byte.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/hvplot/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testohlc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testscattermatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testbackend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testcharts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testfugue.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgeowithoutgv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgridplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testhelp.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testibis.py
--rw-r--r--   0 runner    (1001) docker     (127)    42090 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testnetworkx.py
--rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoperations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testpatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testplotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/teststreaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testtransforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testui.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/hvplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/scripts/update_conda_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.364089 hvplot-0.9.3a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 17:52:31.364089 hvplot-0.9.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/binder/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/conda.recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.320089 hvplot-0.9.3a2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.328089 hvplot-0.9.3a2/doc/_static/home/
+-rw-r--r--   0 runner    (1001) docker     (127)   198618 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/bokeh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   244779 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/dask.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   873325 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/explorer.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    47722 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/geo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   702643 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/geopandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/intake.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    70800 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/interactive_hvplot.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    72465 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/interactive_pandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   173838 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/interactive_xarray.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   267815 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/large_data.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   109054 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/layout.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    84928 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36604 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/networkx.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    24841 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95678 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/pandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   116788 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/plotly.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   184170 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/widgets.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   241968 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/home/xarray.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.332089 hvplot-0.9.3a2/doc/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   194737 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/images/heat_and_trees.png
+-rw-r--r--   0 runner    (1001) docker     (127)   182260 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/images/portfolio.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/logo_horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/_static/logo_stacked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/about.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.336089 hvplot-0.9.3a2/doc/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   359182 2024-04-19 17:52:20.000000 hvplot-0.9.3a2/doc/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1080507 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151250 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   463297 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1007817 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/assets/streamz_demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.336089 hvplot-0.9.3a2/doc/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/developer_guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.336089 hvplot-0.9.3a2/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/getting_started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/getting_started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.316089 hvplot-0.9.3a2/doc/governance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.336089 hvplot-0.9.3a2/doc/governance/project-docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/governance/project-docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/governance/project-docs/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/governance/project-docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/governance/project-docs/MEMBERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.316089 hvplot-0.9.3a2/doc/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.336089 hvplot-0.9.3a2/doc/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.340089 hvplot-0.9.3a2/doc/reference/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/tabular/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.344089 hvplot-0.9.3a2/doc/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/reference/xarray/violin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    32456 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/releases.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/roadmap.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/topics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.348089 hvplot-0.9.3a2/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21995 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Large_Timeseries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25917 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    31550 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22152 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23107 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.348089 hvplot-0.9.3a2/doc/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/images/simple.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/doc/user_guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.348089 hvplot-0.9.3a2/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.10-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.11-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.11-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.12-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.8-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/envs/py3.9-tests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.352089 hvplot-0.9.3a2/hvplot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/backend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109238 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.352089 hvplot-0.9.3a2/hvplot/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/datasets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/ibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/intake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21430 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/networkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.352089 hvplot-0.9.3a2/hvplot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/andrews_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80862 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/lag_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/plotting/scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/polars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/streamz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.356089 hvplot-0.9.3a2/hvplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.360089 hvplot-0.9.3a2/hvplot/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/data/RGB-red.byte.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.360089 hvplot-0.9.3a2/hvplot/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/plotting/testcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/plotting/testohlc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/plotting/testscattermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testbackend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testcharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testfugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testgeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testgeowithoutgv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testgridplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testhelp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42090 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testnetworkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testoperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testpatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testplotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/teststreaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testtransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/hvplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.360089 hvplot-0.9.3a2/hvplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 17:52:31.000000 hvplot-0.9.3a2/hvplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:52:31.360089 hvplot-0.9.3a2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 17:52:21.000000 hvplot-0.9.3a2/scripts/update_conda_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:52:31.364089 hvplot-0.9.3a2/setup.cfg
```

### Comparing `hvplot-0.9.3a1/.github/workflows/build.yaml` & `hvplot-0.9.3a2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/.github/workflows/docs.yaml` & `hvplot-0.9.3a2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/.github/workflows/test.yaml` & `hvplot-0.9.3a2/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 name: tests
 on:
   push:
+    tags:
+      - 'v[0-9]+.[0-9]+.[0-9]+'
+      - 'v[0-9]+.[0-9]+.[0-9]+a[0-9]+'
+      - 'v[0-9]+.[0-9]+.[0-9]+b[0-9]+'
+      - 'v[0-9]+.[0-9]+.[0-9]+rc[0-9]+'
     branches:
       - main
   pull_request:
     branches:
     - '*'
   workflow_dispatch:
     inputs:
```

### Comparing `hvplot-0.9.3a1/.gitignore` & `hvplot-0.9.3a2/.gitignore`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/.pre-commit-config.yaml` & `hvplot-0.9.3a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/LICENSE` & `hvplot-0.9.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/PKG-INFO` & `hvplot-0.9.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.9.3a1
+Version: 0.9.3a2
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Author-email: Philipp Rudiger <developers@holoviz.org>
 Maintainer-email: HoloViz developers <developers@holoviz.org>
 License: BSD
 Project-URL: Homepage, https://hvplot.holoviz.org
 Project-URL: Source, http://github.com/holoviz/hvplot
 Project-URL: HoloViz, https://holoviz.org/
```

### Comparing `hvplot-0.9.3a1/README.md` & `hvplot-0.9.3a2/README.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/binder/environment.yml` & `hvplot-0.9.3a2/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/conda.recipe/meta.yaml` & `hvplot-0.9.3a2/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/favicon.ico` & `hvplot-0.9.3a2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/bokeh.gif` & `hvplot-0.9.3a2/doc/_static/home/bokeh.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/dask.gif` & `hvplot-0.9.3a2/doc/_static/home/dask.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/explorer.gif` & `hvplot-0.9.3a2/doc/_static/home/explorer.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/geo.gif` & `hvplot-0.9.3a2/doc/_static/home/geo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/geopandas.gif` & `hvplot-0.9.3a2/doc/_static/home/geopandas.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/intake.gif` & `hvplot-0.9.3a2/doc/_static/home/intake.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/interactive_hvplot.gif` & `hvplot-0.9.3a2/doc/_static/home/interactive_hvplot.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/interactive_pandas.gif` & `hvplot-0.9.3a2/doc/_static/home/interactive_pandas.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/interactive_xarray.gif` & `hvplot-0.9.3a2/doc/_static/home/interactive_xarray.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/large_data.gif` & `hvplot-0.9.3a2/doc/_static/home/large_data.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/layout.gif` & `hvplot-0.9.3a2/doc/_static/home/layout.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/matplotlib.png` & `hvplot-0.9.3a2/doc/_static/home/matplotlib.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/networkx.gif` & `hvplot-0.9.3a2/doc/_static/home/networkx.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/overlay.png` & `hvplot-0.9.3a2/doc/_static/home/overlay.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/pandas.gif` & `hvplot-0.9.3a2/doc/_static/home/pandas.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/plotly.gif` & `hvplot-0.9.3a2/doc/_static/home/plotly.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/widgets.gif` & `hvplot-0.9.3a2/doc/_static/home/widgets.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/home/xarray.gif` & `hvplot-0.9.3a2/doc/_static/home/xarray.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/images/heat_and_trees.png` & `hvplot-0.9.3a2/doc/_static/images/heat_and_trees.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/images/portfolio.png` & `hvplot-0.9.3a2/doc/_static/images/portfolio.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/logo.png` & `hvplot-0.9.3a2/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/logo_horizontal.svg` & `hvplot-0.9.3a2/doc/_static/logo_horizontal.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/_static/logo_stacked.svg` & `hvplot-0.9.3a2/doc/_static/logo_stacked.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/about.md` & `hvplot-0.9.3a2/doc/about.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/console.png` & `hvplot-0.9.3a2/doc/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/console_server.gif` & `hvplot-0.9.3a2/doc/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/diagram.png` & `hvplot-0.9.3a2/doc/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/diagram.svg` & `hvplot-0.9.3a2/doc/assets/diagram.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/hvplot-wm.png` & `hvplot-0.9.3a2/doc/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/assets/streamz_demo.gif` & `hvplot-0.9.3a2/doc/assets/streamz_demo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/conf.py` & `hvplot-0.9.3a2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/conftest.py` & `hvplot-0.9.3a2/doc/conftest.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/developer_guide/index.md` & `hvplot-0.9.3a2/doc/developer_guide/index.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/getting_started/explorer.ipynb` & `hvplot-0.9.3a2/doc/getting_started/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/getting_started/hvplot.ipynb` & `hvplot-0.9.3a2/doc/getting_started/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/getting_started/index.md` & `hvplot-0.9.3a2/doc/getting_started/index.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/getting_started/installation.md` & `hvplot-0.9.3a2/doc/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/getting_started/interactive.ipynb` & `hvplot-0.9.3a2/doc/getting_started/interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/governance/project-docs/GOVERNANCE.md` & `hvplot-0.9.3a2/doc/governance/project-docs/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/governance/project-docs/MEMBERS.md` & `hvplot-0.9.3a2/doc/governance/project-docs/MEMBERS.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/index.md` & `hvplot-0.9.3a2/doc/index.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/geopandas/points.ipynb` & `hvplot-0.9.3a2/doc/reference/geopandas/points.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/geopandas/polygons.ipynb` & `hvplot-0.9.3a2/doc/reference/geopandas/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/andrewscurves.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/andrewscurves.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/area.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/area.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/bar.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/barh.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/barh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/bivariate.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/bivariate.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/box.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/box.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/errorbars.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/errorbars.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/heatmap.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/hexbin.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/hexbin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/hist.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/kde.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/labels.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/labels.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/lagplot.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/lagplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/line.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/ohlc.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/ohlc.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/parallelcoordinates.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/parallelcoordinates.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/scatter.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/scattermatrix.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/scattermatrix.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/step.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/step.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/table.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/table.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/tabular/violin.ipynb` & `hvplot-0.9.3a2/doc/reference/tabular/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/bar.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/contour.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/contour.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/contourf.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/contourf.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/hist.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/image.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/image.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/kde.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/line.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/quadmesh.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/rgb.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/rgb.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/vectorfield.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/reference/xarray/violin.ipynb` & `hvplot-0.9.3a2/doc/reference/xarray/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/releases.md` & `hvplot-0.9.3a2/doc/releases.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/roadmap.md` & `hvplot-0.9.3a2/doc/roadmap.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/topics.md` & `hvplot-0.9.3a2/doc/topics.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Customization.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Customization.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Explorer.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Geographic_Data.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Geographic_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Gridded_Data.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Gridded_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Integrations.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Integrations.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Interactive.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Introduction.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Large_Timeseries.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Large_Timeseries.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/NetworkX.ipynb` & `hvplot-0.9.3a2/doc/user_guide/NetworkX.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Pandas_API.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Pandas_API.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Plotting.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Plotting_Extensions.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Plotting_with_Plotly.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Statistical_Plots.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Statistical_Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Streaming.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Streaming.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Subplots.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Subplots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Timeseries_Data.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Timeseries_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Viewing.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/Widgets.ipynb` & `hvplot-0.9.3a2/doc/user_guide/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/images/simple.svg` & `hvplot-0.9.3a2/doc/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/doc/user_guide/index.md` & `hvplot-0.9.3a2/doc/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.10-tests.yaml` & `hvplot-0.9.3a2/envs/py3.10-tests.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.11-docs.yaml` & `hvplot-0.9.3a2/envs/py3.11-docs.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.11-tests.yaml` & `hvplot-0.9.3a2/envs/py3.11-tests.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.12-tests.yaml` & `hvplot-0.9.3a2/envs/py3.12-tests.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.8-tests.yaml` & `hvplot-0.9.3a2/envs/py3.8-tests.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/envs/py3.9-tests.yaml` & `hvplot-0.9.3a2/envs/py3.9-tests.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/__init__.py` & `hvplot-0.9.3a2/hvplot/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/backend_transforms.py` & `hvplot-0.9.3a2/hvplot/backend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/converter.py` & `hvplot-0.9.3a2/hvplot/converter.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/cudf.py` & `hvplot-0.9.3a2/hvplot/cudf.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/dask.py` & `hvplot-0.9.3a2/hvplot/dask.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/data/crime.csv` & `hvplot-0.9.3a2/hvplot/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/datasets.yaml` & `hvplot-0.9.3a2/hvplot/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/fugue.py` & `hvplot-0.9.3a2/hvplot/fugue.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/ibis.py` & `hvplot-0.9.3a2/hvplot/ibis.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/intake.py` & `hvplot-0.9.3a2/hvplot/intake.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/interactive.py` & `hvplot-0.9.3a2/hvplot/interactive.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/networkx.py` & `hvplot-0.9.3a2/hvplot/networkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/pandas.py` & `hvplot-0.9.3a2/hvplot/pandas.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/__init__.py` & `hvplot-0.9.3a2/hvplot/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/andrews_curves.py` & `hvplot-0.9.3a2/hvplot/plotting/andrews_curves.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/core.py` & `hvplot-0.9.3a2/hvplot/plotting/core.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/lag_plot.py` & `hvplot-0.9.3a2/hvplot/plotting/lag_plot.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/parallel_coordinates.py` & `hvplot-0.9.3a2/hvplot/plotting/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/plotting/scatter_matrix.py` & `hvplot-0.9.3a2/hvplot/plotting/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/polars.py` & `hvplot-0.9.3a2/hvplot/polars.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/sample_data.py` & `hvplot-0.9.3a2/hvplot/sample_data.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/streamz.py` & `hvplot-0.9.3a2/hvplot/streamz.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/conftest.py` & `hvplot-0.9.3a2/hvplot/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/data/RGB-red.byte.tif` & `hvplot-0.9.3a2/hvplot/tests/data/RGB-red.byte.tif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/plotting/testcore.py` & `hvplot-0.9.3a2/hvplot/tests/plotting/testcore.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/plotting/testohlc.py` & `hvplot-0.9.3a2/hvplot/tests/plotting/testohlc.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/plotting/testscattermatrix.py` & `hvplot-0.9.3a2/hvplot/tests/plotting/testscattermatrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/test_links.py` & `hvplot-0.9.3a2/hvplot/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testbackend_transforms.py` & `hvplot-0.9.3a2/hvplot/tests/testbackend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testcharts.py` & `hvplot-0.9.3a2/hvplot/tests/testcharts.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testfugue.py` & `hvplot-0.9.3a2/hvplot/tests/testfugue.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testgeo.py` & `hvplot-0.9.3a2/hvplot/tests/testgeo.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testgeowithoutgv.py` & `hvplot-0.9.3a2/hvplot/tests/testgeowithoutgv.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testgridplots.py` & `hvplot-0.9.3a2/hvplot/tests/testgridplots.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testhelp.py` & `hvplot-0.9.3a2/hvplot/tests/testhelp.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testinteractive.py` & `hvplot-0.9.3a2/hvplot/tests/testinteractive.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testnetworkx.py` & `hvplot-0.9.3a2/hvplot/tests/testnetworkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testoperations.py` & `hvplot-0.9.3a2/hvplot/tests/testoperations.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testoptions.py` & `hvplot-0.9.3a2/hvplot/tests/testoptions.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testoverrides.py` & `hvplot-0.9.3a2/hvplot/tests/testoverrides.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testpanel.py` & `hvplot-0.9.3a2/hvplot/tests/testpanel.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testpatch.py` & `hvplot-0.9.3a2/hvplot/tests/testpatch.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testplotting.py` & `hvplot-0.9.3a2/hvplot/tests/testplotting.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/teststreaming.py` & `hvplot-0.9.3a2/hvplot/tests/teststreaming.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testtransforms.py` & `hvplot-0.9.3a2/hvplot/tests/testtransforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testui.py` & `hvplot-0.9.3a2/hvplot/tests/testui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/testutil.py` & `hvplot-0.9.3a2/hvplot/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/tests/util.py` & `hvplot-0.9.3a2/hvplot/tests/util.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/ui.py` & `hvplot-0.9.3a2/hvplot/ui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/util.py` & `hvplot-0.9.3a2/hvplot/util.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/utilities.py` & `hvplot-0.9.3a2/hvplot/utilities.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot/xarray.py` & `hvplot-0.9.3a2/hvplot/xarray.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/hvplot.egg-info/PKG-INFO` & `hvplot-0.9.3a2/hvplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.9.3a1
+Version: 0.9.3a2
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Author-email: Philipp Rudiger <developers@holoviz.org>
 Maintainer-email: HoloViz developers <developers@holoviz.org>
 License: BSD
 Project-URL: Homepage, https://hvplot.holoviz.org
 Project-URL: Source, http://github.com/holoviz/hvplot
 Project-URL: HoloViz, https://holoviz.org/
```

### Comparing `hvplot-0.9.3a1/hvplot.egg-info/SOURCES.txt` & `hvplot-0.9.3a2/hvplot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+.git-blame-ignore-revs
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 README.md
 pyproject.toml
+.github/CONTRIBUTING.md
 .github/FUNDING.yml
 .github/workflows/build.yaml
 .github/workflows/docs.yaml
 .github/workflows/test.yaml
 binder/environment.yml
 binder/postBuild
 conda.recipe/meta.yaml
```

### Comparing `hvplot-0.9.3a1/hvplot.egg-info/requires.txt` & `hvplot-0.9.3a2/hvplot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/pyproject.toml` & `hvplot-0.9.3a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.3a1/scripts/update_conda_envs.py` & `hvplot-0.9.3a2/scripts/update_conda_envs.py`

 * *Files identical despite different names*

