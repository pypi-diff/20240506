# Comparing `tmp/sympy_plot_backends-3.3.0.tar.gz` & `tmp/sympy_plot_backends-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympy_plot_backends-3.3.0.tar", last modified: Sun Apr 14 17:57:04 2024, max compression
+gzip compressed data, was "sympy_plot_backends-3.4.0.tar", last modified: Mon May  6 08:56:37 2024, max compression
```

## Comparing `sympy_plot_backends-3.3.0.tar` & `sympy_plot_backends-3.4.0.tar`

### file list

```diff
@@ -1,183 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.074653 sympy_plot_backends-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-14 17:57:04.074653 sympy_plot_backends-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:57:04.074653 sympy_plot_backends-3.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.042652 sympy_plot_backends-3.3.0/spb/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.046652 sympy_plot_backends-3.3.0/spb/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/base_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.046652 sympy_plot_backends-3.3.0/spb/backends/bokeh/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/bokeh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.046652 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/arrow2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/mcircles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/ngrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/nichols.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/nyquist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/polezero.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/root_locus.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/sgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.050652 sympy_plot_backends-3.3.0/spb/backends/k3d/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/k3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.050652 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/arrow3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.050652 sympy_plot_backends-3.3.0/spb/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.054653 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/_sgrid_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/arrow2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/arrow3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/implicit2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/mcircles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/ngrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/nichols.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/nyquist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/polezero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/root_locus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/sgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/vector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.054653 sympy_plot_backends-3.3.0/spb/backends/mayavi/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/mayavi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.054653 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.054653 sympy_plot_backends-3.3.0/spb/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22056 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.058652 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/arrow2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/vector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    22021 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.058652 sympy_plot_backends-3.3.0/spb/ccomplex/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/ccomplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/ccomplex/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/ccomplex/wegert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.058652 sympy_plot_backends-3.3.0/spb/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57633 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/complex_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)   104780 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    68412 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/functions_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32186 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/graphics/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.062653 sympy_plot_backends-3.3.0/spb/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.062653 sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (127)    16263 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    31415 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/interactive/panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.062653 sympy_plot_backends-3.3.0/spb/plot_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43648 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/complex_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    52650 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    64846 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    39553 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/functions_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plot_functions/vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)   183807 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/series.py
--rw-r--r--   0 runner    (1001) docker     (127)    35757 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/spb/wegert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.070653 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-14 17:57:04.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-14 17:57:04.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:57:04.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:57:03.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-14 17:57:04.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 17:57:04.000000 sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.066653 sympy_plot_backends-3.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.066653 sympy_plot_backends-3.3.0/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24971 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/make_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    52843 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28531 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_k3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    84925 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    57115 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/backends/test_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.066653 sympy_plot_backends-3.3.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_complex_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    34946 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_control_min_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_functions_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/graphics/test_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.070653 sympy_plot_backends-3.3.0/tests/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/interactive/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/interactive/test_ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/interactive/test_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:57:04.070653 sympy_plot_backends-3.3.0/tests/plot_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    94547 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/test_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    51725 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/test_functions_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    33383 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/test_functions_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    52073 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/plot_functions/test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)   148076 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-14 17:56:59.000000 sympy_plot_backends-3.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.238813 sympy_plot_backends-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-06 08:56:37.238813 sympy_plot_backends-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:56:37.238813 sympy_plot_backends-3.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2105 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.206813 sympy_plot_backends-3.4.0/spb/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.206813 sympy_plot_backends-3.4.0/spb/animation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/animation/ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/animation/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.206813 sympy_plot_backends-3.4.0/spb/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27901 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/base_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.206813 sympy_plot_backends-3.4.0/spb/backends/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/bokeh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.210813 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/arrow2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/mcircles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/ngrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/nichols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/nyquist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/polezero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/root_locus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/sgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.210813 sympy_plot_backends-3.4.0/spb/backends/k3d/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17122 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/k3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.214814 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/arrow3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.214814 sympy_plot_backends-3.4.0/spb/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.218814 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/_sgrid_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/arrow2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/arrow3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/implicit2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/mcircles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/ngrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/nichols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/nyquist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/polezero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/root_locus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/sgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.218814 sympy_plot_backends-3.4.0/spb/backends/mayavi/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/mayavi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.218814 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.218814 sympy_plot_backends-3.4.0/spb/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22056 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.222813 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/arrow2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22021 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.222813 sympy_plot_backends-3.4.0/spb/ccomplex/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/ccomplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/ccomplex/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/ccomplex/wegert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.222813 sympy_plot_backends-3.4.0/spb/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57633 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/complex_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104780 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68412 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/functions_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32186 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/graphics/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.222813 sympy_plot_backends-3.4.0/spb/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/bokeh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.226813 sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31824 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/interactive/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.226813 sympy_plot_backends-3.4.0/spb/plot_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43648 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/complex_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52650 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64846 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39553 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/functions_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plot_functions/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26645 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183807 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37674 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/spb/wegert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.234813 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 08:56:37.000000 sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.226813 sympy_plot_backends-3.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.230813 sympy_plot_backends-3.4.0/tests/animation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/animation/test_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/animation/test_panel_ipywidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.230813 sympy_plot_backends-3.4.0/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24971 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/make_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52834 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28531 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_k3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84925 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57115 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/backends/test_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.230813 sympy_plot_backends-3.4.0/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_complex_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34946 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_control_min_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_functions_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/graphics/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.230813 sympy_plot_backends-3.4.0/tests/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/interactive/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/interactive/test_ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/interactive/test_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:37.234813 sympy_plot_backends-3.4.0/tests/plot_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94547 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51725 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/test_functions_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33383 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/test_functions_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52073 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/plot_functions/test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148076 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-05-06 08:56:33.000000 sympy_plot_backends-3.4.0/tests/test_utils.py
```

### Comparing `sympy_plot_backends-3.3.0/LICENSE` & `sympy_plot_backends-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/PKG-INFO` & `sympy_plot_backends-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy_plot_backends
-Version: 3.3.0
+Version: 3.4.0
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,26 +29,36 @@
 Requires-Dist: plotly>=4.14.3; extra == "all"
 Requires-Dist: panel>=1.0.0; extra == "all"
 Requires-Dist: ipywidgets_bokeh; extra == "all"
 Requires-Dist: colorcet; extra == "all"
 Requires-Dist: k3d>=2.9.7; extra == "all"
 Requires-Dist: vtk; extra == "all"
 Requires-Dist: control>=0.10.0; extra == "all"
+Requires-Dist: imageio; extra == "all"
+Requires-Dist: imageio-ffmpeg; extra == "all"
+Requires-Dist: psutil; extra == "all"
+Requires-Dist: av; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
 Requires-Dist: scipy>=1.7.1; extra == "dev"
 Requires-Dist: adaptive>=0.13.1; extra == "dev"
 Requires-Dist: notebook; extra == "dev"
 Requires-Dist: ipympl>=0.7.0; extra == "dev"
 Requires-Dist: plotly>=4.14.3; extra == "dev"
 Requires-Dist: panel>=1.0.0; extra == "dev"
 Requires-Dist: ipywidgets_bokeh; extra == "dev"
 Requires-Dist: colorcet; extra == "dev"
 Requires-Dist: k3d>=2.9.7; extra == "dev"
 Requires-Dist: vtk; extra == "dev"
 Requires-Dist: control>=0.10.0; extra == "dev"
+Requires-Dist: imageio; extra == "dev"
+Requires-Dist: imageio-ffmpeg; extra == "dev"
+Requires-Dist: psutil; extra == "dev"
+Requires-Dist: av; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: kaleido; extra == "dev"
 Requires-Dist: numpydoc; extra == "dev"
 
@@ -65,15 +75,15 @@
 
 The following plotting libraries are supported: [Matplolib](https://matplotlib.org/), [Plotly](https://plotly.com/), [Bokeh](https://github.com/bokeh/bokeh), [K3D-Jupyter](https://github.com/K3D-tools/K3D-jupyter).
 
 <div>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/iplot_bokeh.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/mpl-streamplot.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/plotly_streamlines_2.png" width=250/>
-<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-spherical-harmonics.png" width=250/>
+<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/animation.gif" width=250 style="width:250px;height:auto;"/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/bokeh_domain_coloring.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-cone-vectors.png" width=250/>
 </div>
 
 
 ## What's new in comparison to SymPy
 
@@ -84,14 +94,15 @@
 * visualize discontinuities on 2D line plots.
 * visualize 2D/3D vector fields with quivers or streamlines.
 * visualize complex functions with [domain coloring](https://en.wikipedia.org/wiki/Domain_coloring).
 * visualize entities from the `sympy.geometry` module.
 * visualize control systems' response to input signals, root locus, as well as Bode, Nyquist and Nichols diagrams.
 * create parametric-interactive plots using widgets
   (sliders, buttons, etc.) with *ipywidgets* or *Holoviz's Panel*.
+* create animations.
 
 Please, read the
 [following documentation page](https://sympy-plot-backends.readthedocs.io/en/latest/overview.html#differences-with-sympy-plotting)
 to understand the differences between this module and ``sympy.plotting``.
 
 
 ## Development and Support
```

### Comparing `sympy_plot_backends-3.3.0/README.md` & `sympy_plot_backends-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 The following plotting libraries are supported: [Matplolib](https://matplotlib.org/), [Plotly](https://plotly.com/), [Bokeh](https://github.com/bokeh/bokeh), [K3D-Jupyter](https://github.com/K3D-tools/K3D-jupyter).
 
 <div>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/iplot_bokeh.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/mpl-streamplot.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/plotly_streamlines_2.png" width=250/>
-<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-spherical-harmonics.png" width=250/>
+<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/animation.gif" width=250 style="width:250px;height:auto;"/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/bokeh_domain_coloring.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-cone-vectors.png" width=250/>
 </div>
 
 
 ## What's new in comparison to SymPy
 
@@ -30,14 +30,15 @@
 * visualize discontinuities on 2D line plots.
 * visualize 2D/3D vector fields with quivers or streamlines.
 * visualize complex functions with [domain coloring](https://en.wikipedia.org/wiki/Domain_coloring).
 * visualize entities from the `sympy.geometry` module.
 * visualize control systems' response to input signals, root locus, as well as Bode, Nyquist and Nichols diagrams.
 * create parametric-interactive plots using widgets
   (sliders, buttons, etc.) with *ipywidgets* or *Holoviz's Panel*.
+* create animations.
 
 Please, read the
 [following documentation page](https://sympy-plot-backends.readthedocs.io/en/latest/overview.html#differences-with-sympy-plotting)
 to understand the differences between this module and ``sympy.plotting``.
 
 
 ## Development and Support
```

### Comparing `sympy_plot_backends-3.3.0/setup.py` & `sympy_plot_backends-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     "ipympl>=0.7.0",
     "plotly>=4.14.3",
     "panel>=1.0.0", # this includes param and bokeh
     "ipywidgets_bokeh", # starting from panel v0.13.0, it is not part of panel anymore
     "colorcet",
     "k3d>=2.9.7",
     "vtk",  # needed for streamlines in k3d
-    "control>=0.10.0"
+    "control>=0.10.0",
+    "imageio", "imageio-ffmpeg", "psutil", "av", "tqdm", # to save animations
     # mayavi-related
     # "mayavi>=4.8.0",
     # "PyQt5>=5.15.7",
 ]
 
 _dev_deps = _all_deps + [
     "pytest",
```

### Comparing `sympy_plot_backends-3.3.0/spb/__init__.py` & `sympy_plot_backends-3.4.0/spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/base_backend.py` & `sympy_plot_backends-3.4.0/spb/backends/base_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,15 +416,15 @@
             ylim=self.ylim,
             zlim=self.zlim,
             size=self.size,
             is_iplot=self.is_iplot,
             use_latex=self._use_latex,
             camera=self.camera,
             polar_axis=self.polar_axis,
-            axis=self.axis,
+            axis=self.axis
         )
 
     def _init_cyclers(self, start_index_cl=None, start_index_cm=None):
         """Create infinite loop iterators over the provided color maps."""
 
         tb = type(self)
         colorloop = self.colorloop if not tb.colorloop else tb.colorloop
@@ -472,39 +472,14 @@
                 "steps to make it works:\n"
                 "1. Code an appropriate rendeder class.\n"
                 f"2. Execute {type(self).__name__}.renderers_map.update"
                 "({%s})\n" % f"{type(series).__name__}: YourRendererClass"
                 + "3. Execute again the plot statement."
             )
 
-    def _get_mode(self):
-        """Verify which environment is used to run the code.
-
-        Returns
-        =======
-            mode : int
-                0 - the code is running on Jupyter Notebook or qtconsole
-                1 - terminal running IPython
-                2 - other type (?)
-                3 - probably standard Python interpreter
-
-        # TODO: detect if we are running in Jupyter Lab.
-        """
-        # https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
-        try:
-            shell = get_ipython().__class__.__name__
-            if shell == "ZMQInteractiveShell":
-                return 0  # Jupyter notebook or qtconsole
-            elif shell == "TerminalInteractiveShell":
-                return 1  # Terminal running IPython
-            else:
-                return 2  # Other type (?)
-        except NameError:
-            return 3  # Probably standard Python interpreter
-
     def _use_cyclic_cm(self, param, is_complex):
         """When using complex_plot and `absarg=True`, it might happens that the
         argument is not fully covering the range [-pi, pi]. In such occurences,
         the use of a cyclic colormap would create a misleading plot.
         """
         np = import_module('numpy')
```

### Comparing `sympy_plot_backends-3.3.0/spb/backends/base_renderer.py` & `sympy_plot_backends-3.4.0/spb/backends/base_renderer.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/bokeh.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/bokeh.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Vector2DSeries, ComplexDomainColoringSeries, ContourSeries,
     GeometrySeries, GenericDataSeries, HVLineSeries, Arrow2DSeries,
     ZGridLineSeries, SGridLineSeries, NGridLineSeries, NicholsLineSeries,
     MCirclesSeries, PoleZeroSeries, PoleZeroWithSympySeries,
     SystemResponseSeries, ColoredSystemResponseSeries, RootLocusSeries,
     NyquistLineSeries
 )
+from spb.utils import get_environment
 from sympy.external import import_module
 
 
 class BokehBackend(Plot):
     """
     A backend for plotting SymPy's symbolic expressions using Bokeh.
     This implementation only supports 2D plots.
@@ -214,15 +215,15 @@
         self._use_latex = kwargs.get("use_latex", cfg["bokeh"]["use_latex"])
         self._set_labels()
         self._set_title()
 
         self._theme = kwargs.get("theme", cfg["bokeh"]["theme"])
 
         self._run_in_notebook = False
-        if self._get_mode() == 0:
+        if get_environment() == 0:
             self._run_in_notebook = True
             self.bokeh.io.output_notebook(hide_banner=True)
 
         if (
             (len([s for s in self._series if s.is_2Dline]) > 10) and
             (not type(self).colorloop) and
             not ("process_piecewise" in kwargs.keys())
```

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/__init__.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/arrow2d.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/arrow2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/complex.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/contour.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/contour.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,63 +5,55 @@
 def _draw_contour_helper(renderer, data):
     p, s = renderer.plot, renderer.series
     handle = []
 
     if s.is_polar:
         raise NotImplementedError()
     x, y, z = data
-    x, y, zz = [t.flatten() for t in [x, y, z]]
-    minx, miny, minz = min(x), min(y), min(zz)
-    maxx, maxy, maxz = max(x), max(y), max(zz)
+
+    # NOTE: at the time of writing this, Bokeh doesn't support
+    # levels=int number.
+    if "levels" in s.rendering_kw.keys():
+        levels = s.rendering_kw["levels"]
+    else:
+        levels = p.np.linspace(z.min(), z.max(), 10)
+
+    if (not s.is_filled) and s.show_clabels:
+        warnings.warn("BokehBackend doesn't currently support contour labels.")
 
     cm = next(p._cm)
-    ckw = dict(palette=cm)
+    ckw = dict(fill_color=cm, line_color=cm, levels=levels)
     kw = p.merge({}, ckw, s.rendering_kw)
 
-    if not s.is_filled:
-        warnings.warn("Bokeh does not support line contours.")
-
-    h = p._fig.image(
-        image=[z],
-        x=minx,
-        y=miny,
-        dw=abs(maxx - minx),
-        dh=abs(maxy - miny),
-        **kw
-    )
-    handle.append(h)
+    h = p._fig.contour(x, y, z, **kw)
+    handle.extend([h, levels])
     p._fig.add_tools(p.bokeh.models.HoverTool(
-        tooltips=[("x", "$x"), ("y", "$y"), ("z", "@image")],
+        tooltips=[("x", "@x"), ("y", "@y"), ("z", "@z")],
         renderers=[handle[0]]
     ))
 
     if s.colorbar:
-        colormapper = p.bokeh.models.LinearColorMapper(
-            palette=cm, low=minz, high=maxz)
-        cbkw = dict(width=8, title=s.get_label(p._use_latex))
-        colorbar = p.bokeh.models.ColorBar(
-            color_mapper=colormapper, **cbkw)
+        colorbar = h.construct_color_bar(title=s.get_label(p._use_latex))
         p._fig.add_layout(colorbar, "right")
         handle.append(colorbar)
 
     return handle
 
 
 def _update_contour_helper(renderer, data, handle):
-    s = renderer.series
+    p, s = renderer.plot, renderer.series
     x, y, z = data
-    minx, miny, minz = x.min(), y.min(), z.min()
-    maxx, maxy, maxz = x.max(), y.max(), z.max()
-    handle[0].data_source.data.update({"image": [z]})
-    handle[0].glyph.x = minx
-    handle[0].glyph.y = miny
-    handle[0].glyph.dw = abs(maxx - minx)
-    handle[0].glyph.dh = abs(maxy - miny)
+    countour_handle, levels, cb_handle = handle
+    levels = p.np.linspace(z.min(), z.max(), len(levels))
+
+    contour_data = p.bokeh.plotting.contour.contour_data(x, y, z, levels)
+    handle[0].set_data(contour_data)
     if s.colorbar:
-        cb = handle[1]
-        cb.color_mapper.update(low=minz, high=maxz)
+        # NOTE: as of Bokeh 3.4.1, there is a bug that prevents ticks to
+        # be updated.
+        handle[2].update(levels=list(levels))
 
 
 class ContourRenderer(Renderer):
     draw_update_map = {
         _draw_contour_helper: _update_contour_helper
     }
```

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/generic.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/geometry.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/hvline.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/line2d.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/mcircles.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/mcircles.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/ngrid.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/ngrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/nichols.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/nichols.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/nyquist.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/nyquist.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/polezero.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/polezero.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/root_locus.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/root_locus.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/sgrid.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/sgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/vector2d.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/bokeh/renderers/zgrid.py` & `sympy_plot_backends-3.4.0/spb/backends/bokeh/renderers/zgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/k3d.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/k3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Parametric3DLineSeries, ComplexParametric3DLineSeries,
     List3DSeries, Vector3DSeries, SliceVector3DSeries,
     RiemannSphereSeries, Implicit3DSeries,
     ComplexDomainColoringSeries, ComplexSurfaceSeries,
     SurfaceOver2DRangeSeries, ParametricSurfaceSeries,
     PlaneSeries, GeometrySeries, Arrow3DSeries
 )
+from spb.utils import get_environment
 from sympy.external import import_module
 import warnings
 
 
 class K3DBackend(Plot):
     """A backend for plotting SymPy's symbolic expressions using K3D-Jupyter.
 
@@ -158,15 +159,15 @@
             k3d.paraview_color_maps.Blue_to_Yellow,
         ]
         self.cyclic_colormaps = [
             cc.colorwheel, k3d.paraview_color_maps.Erdc_iceFire_H]
 
         self._init_cyclers()
         super().__init__(*args, **kwargs)
-        if (not self.skip_notebook_check) and (self._get_mode() != 0):
+        if (not self.skip_notebook_check) and (get_environment() != 0):
             warnings.warn(
                 "K3DBackend only works properly within Jupyter Notebook")
         self._use_latex = kwargs.get("use_latex", cfg["k3d"]["use_latex"])
         self._set_labels("%s")
         self._set_title("%s")
 
         self._show_label = kwargs.get("show_label", False)
@@ -466,15 +467,15 @@
 
         if ext in [".html", ".htm"]:
             with open(path, 'w') as f:
                 include_js = kwargs.pop("include_js", False)
                 self.fig.snapshot_include_js = include_js
                 f.write(self.fig.get_snapshot(**kwargs))
         elif ext == ".png":
-            if self._get_mode() != 0:
+            if get_environment() != 0:
                 raise ValueError(
                     "K3D-Jupyter requires the plot to be shown on the screen "
                     + "before saving a png file.")
 
             @self._fig.yield_screenshots
             def _func():
                 self._fig.fetch_screenshot(**kwargs)
```

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/__init__.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/arrow3d.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/arrow3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/complex.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/implicit3d.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/line3d.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/surface.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/k3d/renderers/vector3d.py` & `sympy_plot_backends-3.4.0/spb/backends/k3d/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/matplotlib.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/__init__.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/_sgrid_helper.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/_sgrid_helper.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/arrow2d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/arrow2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/arrow3d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/arrow3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/complex.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/contour.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/generic.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/geometry.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/hvline.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/implicit2d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/implicit2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/line2d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/line3d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/mcircles.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/mcircles.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/ngrid.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/ngrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/nichols.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/nichols.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/nyquist.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/nyquist.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/polezero.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/polezero.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/renderer.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/root_locus.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/root_locus.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/sgrid.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/sgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/surface.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/vector2d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/vector3d.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/matplotlib/renderers/zgrid.py` & `sympy_plot_backends-3.4.0/spb/backends/matplotlib/renderers/zgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/mayavi/mayavi.py` & `sympy_plot_backends-3.4.0/spb/backends/mayavi/mayavi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from spb.defaults import cfg
 from spb.backends.base_backend import Plot
 from spb.backends.mayavi.renderers import *
 from spb.series import *
+from spb.utils import get_environment
 from sympy.external import import_module
 import warnings
 
 
 class MayaviBackend(Plot):
     """A backend for plotting SymPy's symbolic expressions using Mayavi.
 
@@ -121,15 +122,15 @@
         super().__init__(*args, **kwargs)
         self._use_latex = kwargs.get("use_latex", cfg["mayavi"]["use_latex"])
         self._set_labels()
         window = kwargs.pop("window", False)
         notebook_kw = kwargs.pop("notebook_kw", dict())
         self.grid = kwargs.get("grid", cfg["mayavi"]["grid"])
 
-        if (self._get_mode() == 0) and (not window):
+        if (get_environment() == 0) and (not window):
             self.mlab.init_notebook(**notebook_kw)
 
         # NOTE/TODO: to adjust the aspect ratio, Mayavi uses the ``extent``
         # keyword argument on its plotting functions. Turns out that the grids
         # sorrounding the objects (giving indications of their dimensions)
         # reads the ``extent`` values. So, if aspect="auto" the grids will
         # show wrong values. Let's use a equal aspect ratio by default.
```

### Comparing `sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/implicit3d.py` & `sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/line3d.py` & `sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/surface.py` & `sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/mayavi/renderers/vector3d.py` & `sympy_plot_backends-3.4.0/spb/backends/mayavi/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/plotly.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/__init__.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/arrow2d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/arrow2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/complex.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/contour.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/generic.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/geometry.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/hvline.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/implicit3d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/line2d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/line3d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/surface.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/vector2d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/plotly/renderers/vector3d.py` & `sympy_plot_backends-3.4.0/spb/backends/plotly/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/backends/utils.py` & `sympy_plot_backends-3.4.0/spb/backends/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/ccomplex/complex.py` & `sympy_plot_backends-3.4.0/spb/ccomplex/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/control.py` & `sympy_plot_backends-3.4.0/spb/control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/defaults.py` & `sympy_plot_backends-3.4.0/spb/defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/doc_utils.py` & `sympy_plot_backends-3.4.0/spb/doc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,27 +303,30 @@
     Returns
     =======
 
     final_img : PIL.Image
     """
     import numpy as np
     from PIL import Image
-    from spb.interactive.panel import InteractivePlot
+    from spb.animation import BaseAnimation
+    from spb.interactive.panel import PanelCommon
     from spb import KB
     from sphinx_k3d_screenshot.utils import get_k3d_screenshot, get_driver
 
     if "panelplot" not in ns.keys():
         return img
 
     panelplot = ns["panelplot"]
-    if not isinstance(panelplot, InteractivePlot):
+    if not isinstance(panelplot, PanelCommon):
         return img
     if not isinstance(panelplot.backend, KB):
         return img
 
+    is_animation = isinstance(panelplot, BaseAnimation)
+
     # At this point img has dimension specified by `size`, but only the top
     # portion is actually populated with widgets. The remaining portions is
     # blank. Let's crop this image so it only contains widgets.
     # Guesstimate (in pixel) for the vertical space of each row of widgets
     hr = 50
     # number of rows used by the widgets
     nr = int(np.ceil(len(panelplot.backend[0].params) / panelplot._ncols))
@@ -336,10 +339,16 @@
     # generate K3D-Jupyter screenshot
     driver = get_driver(
         browser, browser_path, driver_path, driver_options)
     plot = get_k3d_screenshot(driver, size, panelplot.fig)
 
     # concatenate vertically the two images
     final = Image.new('RGB', (img.width, img.height + plot.height))
-    final.paste(img, (0, 0))
-    final.paste(plot, (0, img.height))
+    if is_animation:
+        # place play controls on the bottom
+        final.paste(plot, (0, 0))
+        final.paste(img, (0, plot.height))
+    else:
+        # place widgets on the top
+        final.paste(img, (0, 0))
+        final.paste(plot, (0, img.height))
     return final
```

### Comparing `sympy_plot_backends-3.3.0/spb/functions.py` & `sympy_plot_backends-3.4.0/spb/functions.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/__init__.py` & `sympy_plot_backends-3.4.0/spb/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/complex_analysis.py` & `sympy_plot_backends-3.4.0/spb/graphics/complex_analysis.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/control.py` & `sympy_plot_backends-3.4.0/spb/graphics/control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/functions_2d.py` & `sympy_plot_backends-3.4.0/spb/graphics/functions_2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/functions_3d.py` & `sympy_plot_backends-3.4.0/spb/graphics/functions_3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/graphics.py` & `sympy_plot_backends-3.4.0/spb/graphics/graphics.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/utils.py` & `sympy_plot_backends-3.4.0/spb/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/graphics/vectors.py` & `sympy_plot_backends-3.4.0/spb/graphics/vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/__init__.py` & `sympy_plot_backends-3.4.0/spb/interactive/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -112,22 +112,32 @@
     """Select which interactive module to use.
     """
     imodule = kwargs.pop("imodule", cfg["interactive"]["module"])
     if imodule is None:
         imodule = cfg["interactive"]["module"]
     imodule = imodule.lower()
 
+    animation = kwargs.get("animation", False)
+
     # NOTE: Holoviz's Panel is really slow to load, so let's load it only when
-        # it is necessary
-    if imodule == "panel":
-        from spb.interactive.panel import iplot
-        return iplot(*series, **kwargs)
-    elif imodule == "ipywidgets":
-        from spb.interactive.ipywidgets import iplot
-        return iplot(*series, **kwargs)
+    # it is necessary
+    if not animation:
+        if imodule == "panel":
+            from spb.interactive.panel import iplot
+            return iplot(*series, **kwargs)
+        elif imodule == "ipywidgets":
+            from spb.interactive.ipywidgets import iplot
+            return iplot(*series, **kwargs)
+    else:
+        if imodule == "panel":
+            from spb.animation.panel import animation
+            return animation(*series, **kwargs)
+        elif imodule == "ipywidgets":
+            from spb.animation.ipywidgets import animation
+            return animation(*series, **kwargs)
 
     raise ValueError("`%s` is not a valid interactive module" % imodule)
 
 
 class IPlot:
     """Mixin class for interactive plots containing common attributes and
     methods.
@@ -190,40 +200,7 @@
 
         backend_kw = self._backend._copy_kwargs()
         iplot_kw = self._get_iplot_kw()
         iplot_kw["show"] = False
 
         new_iplot = type(self)(*series, **merge({}, backend_kw, iplot_kw))
         return new_iplot
-
-
-def _aggregate_parameters(params, series):
-    """Loop over data series to extract the `params` dictionaries provided by
-    the user. This is necessary when dealing with the ``graphics`` module.
-
-    Parameters
-    ==========
-    params : dict
-        Whatever was provided by the user in the main function call (be it
-        plot(), plot_paramentric(), ..., graphics())
-    series : list
-        Data series of the current interactive widget plot.
-
-    Returns
-    =======
-    params : dict
-    """
-    if params is None:
-        params = {}
-    if len(params) == 0:
-        # this is the case when an interactive widget plot is build with
-        # the `graphics` interface.
-        for s in series:
-            if s.is_interactive:
-                # use s._original_params instead of s.params in order to
-                # keep track of multi-values widgets
-                params.update(s._original_params)
-    if len(params) == 0:
-        raise ValueError(
-            "In order to create an interactive plot, "
-            "the `params` dictionary must be provided.")
-    return params
```

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/__init__.py` & `sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/bootstrap.css` & `sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/bootstrap.css`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/bootstrap_spb/bootstrap.html` & `sympy_plot_backends-3.4.0/spb/interactive/bootstrap_spb/bootstrap.html`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/ipywidgets.py` & `sympy_plot_backends-3.4.0/spb/interactive/ipywidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ipywidgets
 from sympy import latex
 from sympy.external import import_module
 from spb.defaults import TWO_D_B, THREE_D_B
-from spb.interactive import _tuple_to_dict, IPlot, _aggregate_parameters
+from spb.interactive import _tuple_to_dict, IPlot
+from spb.utils import _aggregate_parameters
 from spb import BB, MB, PlotGrid
 from IPython.display import clear_output
 import warnings
 
 
 def _build_widgets(params, use_latex=True):
     widgets = []
@@ -262,15 +263,15 @@
        installation of the
        `ipympl module <https://github.com/matplotlib/ipympl>`_ .
 
 
     Examples
     ========
 
-    NOTE: the following examples use the ordinary plotting function because
+    NOTE: the following examples use the ordinary plotting functions because
     ``iplot`` is already integrated with them.
 
     Surface plot between -10 <= x, y <= 10 discretized with 50 points
     on both directions, with a damping parameter varying from 0 to 1, and a
     default value of 0.15:
 
     .. code-block::
```

### Comparing `sympy_plot_backends-3.3.0/spb/interactive/panel.py` & `sympy_plot_backends-3.4.0/spb/interactive/panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Implements interactive-widgets plotting with Holoviz Panel using
 `pn.bind`, which binds a function or method to the values of widgets.
 """
 
 from spb.defaults import TWO_D_B, THREE_D_B, cfg
 from spb.utils import _validate_kwargs
-from spb.interactive import _tuple_to_dict, IPlot, _aggregate_parameters
+from spb.interactive import _tuple_to_dict, IPlot
 from spb.interactive.bootstrap_spb import SymPyBootstrapTemplate
 from spb.plotgrid import PlotGrid
+from spb.utils import _aggregate_parameters
 from sympy import latex
 from sympy.external import import_module
 import warnings
 
 param = import_module(
     'param',
     min_module_version='1.11.0',
@@ -73,15 +74,144 @@
 
         # this must be present in order to assure correct behaviour
         super().__init__(name="", **kwargs)
 
         self.param.add_parameter("dyn_param_0", current_param)
 
 
-class InteractivePlot(IPlot):
+class PanelCommon(IPlot):
+    """Common code for interactive applications with Holoviz Panel.
+    """
+
+    @property
+    def pane_kw(self):
+        """Return the keyword arguments used to customize the wrapper to the
+        plot.
+        """
+        return self._pane_kw
+
+    def _init_pane(self):
+        """Here we wrap the figure exposed by the backend with a Pane, which
+        allows to set useful properties.
+        """
+        # NOTE: If the following import statement was located at the
+        # beginning of the file, there would be a circular import.
+        from spb import KB, MB, BB, PB
+
+        default_kw = {}
+        if isinstance(self._backend, PB):
+            pane_func = pn.pane.Plotly
+        elif (
+            isinstance(self._backend, MB) or        # vanilla MB
+            (
+                hasattr(self._backend, "is_matplotlib_fig") and
+                self._backend.is_matplotlib_fig     # plotgrid with all MBs
+            )
+        ):
+            # since we are using Jupyter and interactivity, it is useful to
+            # activate ipympl interactive frame, as well as setting a lower
+            # dpi resolution of the matplotlib image
+            default_kw["dpi"] = 96
+            # NOTE: the following must be set to False in order for the
+            # example outputs to become visible on Sphinx.
+            default_kw["interactive"] = False
+            pane_func = pn.pane.Matplotlib
+        elif isinstance(self._backend, BB):
+            pane_func = pn.pane.Bokeh
+        elif isinstance(self._backend, KB):
+            # TODO: for some reason, panel is going to set width=0
+            # if K3D-Jupyter is used.
+            # Temporary workaround: create a Pane with a default width.
+            # Long term solution: create a PR on panel to create a K3DPane
+            # so that panel will automatically deal with K3D, in the same
+            # way it does with Bokeh, Plotly, Matplotlib, ...
+            default_kw["width"] = 800
+            pane_func = pn.pane.panel
+        else:
+            # here we are dealing with plotgrid of BB/PB/or mixed backend...
+            # but not with plotgrids of MB
+            self._init_pane_for_plotgrid()
+            return
+        kw = self.merge({}, default_kw, self._pane_kw)
+        self.pane = pane_func(self._binding, **kw)
+
+    @property
+    def layout_controls(self):
+        """Return the controls used by the interactive application"""
+        raise NotImplementedError
+
+    def show(self):
+        self._init_pane()
+
+        if not self._servable:
+            if self._layout == "tb":
+                content = pn.Column(self.layout_controls, self.pane)
+            elif self._layout == "bb":
+                content = pn.Column(self.pane, self.layout_controls)
+            elif self._layout == "sbl":
+                content = pn.Row(
+                    pn.Column(self.layout_controls),
+                    pn.Column(self.pane), width_policy="max")
+            elif self._layout == "sbr":
+                content = pn.Row(
+                    pn.Column(self.pane),
+                    pn.Column(self.layout_controls))
+            return content
+
+        return self._create_template(True)
+
+    def _create_template(self, show=False):
+        """Instantiate a template, populate it and serves it.
+
+        Parameters
+        ==========
+
+        show : boolean
+            If True, the template will be served on a new browser window.
+            Otherwise, just return the template: ``show=False`` is used
+            by the documentation to visualize servable applications.
+        """
+        if not show:
+            self._init_pane()
+
+        # pn.theme was introduced with panel 1.0.0, before there was
+        # pn.template.theme
+        submodule = pn.theme if hasattr(pn, "theme") else pn.template.theme
+        theme = submodule.DarkTheme
+        if cfg["interactive"]["theme"] != "dark":
+            theme = submodule.DefaultTheme
+        default_template_kw = dict(title=self._name, theme=theme)
+
+        if (self._template is None) or isinstance(self._template, dict):
+            kw = self._template if isinstance(self._template, dict) else {}
+            kw = self.merge(default_template_kw, kw)
+            kw["sidebar_location"] = self._layout
+            if len(self._name.strip()) == 0:
+                kw.setdefault("show_header", False)
+            template = SymPyBootstrapTemplate(**kw)
+        elif isinstance(self._template, pn.template.base.BasicTemplate):
+            template = self._template
+        elif (isinstance(self._template, type) and
+            issubclass(self._template, pn.template.base.BasicTemplate)):
+            template = self._template(**default_template_kw)
+        else:
+            raise TypeError("`template` not recognized. It can either be a "
+                "dictionary of keyword arguments to be passed to the default "
+                "template, an instance of pn.template.base.BasicTemplate "
+                "or a subclass of pn.template.base.BasicTemplate. Received: "
+                "type(template) = %s" % type(self._template))
+
+        self._populate_template(template)
+
+        if show:
+            return template.servable().show()
+        return template
+
+
+class InteractivePlot(PanelCommon):
 
     def __new__(cls, *args, **kwargs):
         return object.__new__(cls)
 
     def __init__(self, *series, name="", params=None, **kwargs):
         """
         Parameters
@@ -190,159 +320,44 @@
         # first the traces are updated, then the pane creates the figure
         # (with only one single javascript update).
         # TODO: can the backend be modified by adding data and layout
         # attributes, avoiding the creation of the figure? The figure could
         # be created inside the fig getter.
         return self.fig.to_dict()
 
-    @property
-    def pane_kw(self):
-        """Return the keyword arguments used to customize the wrapper to the
-        plot.
-        """
-        return self._pane_kw
-
     def _get_iplot_kw(self):
         return {
             "backend": type(self._backend),
             "layout": self._layout,
             "template": self._template,
             "ncols": self._ncols,
             "throttled": self._throttled,
             "use_latex": self._use_latex,
             "params": self._original_params,
             "pane_kw": self._pane_kw
         }
 
-    def _init_pane(self):
-        """Here we wrap the figure exposed by the backend with a Pane, which
-        allows to set useful properties.
-        """
-        # NOTE: If the following import statement was located at the
-        # beginning of the file, there would be a circular import.
-        from spb import KB, MB, BB, PB
+    def _init_pane_for_plotgrid(self):
+        # First, set the necessary data to create bindings for each subplot
+        self._backend.pre_set_bindings(
+            list(self.mapping.keys()),
+            self._widgets_for_binding()
+        )
+        # Then, create the pn.GridSpec figure
+        self.pane = self._backend.fig
 
-        default_kw = {}
-        if isinstance(self._backend, PB):
-            pane_func = pn.pane.Plotly
-        elif (
-            isinstance(self._backend, MB) or        # vanilla MB
-            (
-                hasattr(self._backend, "is_matplotlib_fig") and
-                self._backend.is_matplotlib_fig     # plotgrid with all MBs
-            )
-        ):
-            # since we are using Jupyter and interactivity, it is useful to
-            # activate ipympl interactive frame, as well as setting a lower
-            # dpi resolution of the matplotlib image
-            default_kw["dpi"] = 96
-            # NOTE: the following must be set to False in order for the
-            # example outputs to become visible on Sphinx.
-            default_kw["interactive"] = False
-            pane_func = pn.pane.Matplotlib
-        elif isinstance(self._backend, BB):
-            pane_func = pn.pane.Bokeh
-        elif isinstance(self._backend, KB):
-            # TODO: for some reason, panel is going to set width=0
-            # if K3D-Jupyter is used.
-            # Temporary workaround: create a Pane with a default width.
-            # Long term solution: create a PR on panel to create a K3DPane
-            # so that panel will automatically deal with K3D, in the same
-            # way it does with Bokeh, Plotly, Matplotlib, ...
-            default_kw["width"] = 800
-            pane_func = pn.pane.panel
-        else:
-            # here we are dealing with plotgrid of BB/PB/or mixed backend...
-            # but not with plotgrids of MB
-            # First, set the necessary data to create bindings for each
-            # subplot
-            self._backend.pre_set_bindings(
-                list(self.mapping.keys()),
-                self._widgets_for_binding()
-            )
-            # Then, create the pn.GridSpec figure
-            self.pane = self._backend.fig
-            return
-        kw = self.merge({}, default_kw, self._pane_kw)
-        self.pane = pane_func(self._binding, **kw)
+    def _populate_template(self, template):
+        template.main.append(self.pane)
+        template.sidebar.append(self.layout_controls)
 
     @property
     def layout_controls(self):
         widgets = list(self.mapping.values())
         return pn.GridBox(*widgets, ncols=self._ncols)
 
-    def show(self):
-        self._init_pane()
-
-        if not self._servable:
-            if self._layout == "tb":
-                content = pn.Column(self.layout_controls, self.pane)
-            elif self._layout == "bb":
-                content = pn.Column(self.pane, self.layout_controls)
-            elif self._layout == "sbl":
-                content = pn.Row(
-                    pn.Column(self.layout_controls),
-                    pn.Column(self.pane), width_policy="max")
-            elif self._layout == "sbr":
-                content = pn.Row(
-                    pn.Column(self.pane),
-                    pn.Column(self.layout_controls))
-
-            return content
-
-        return self._create_template(True)
-
-    def _create_template(self, show=False):
-        """Instantiate a template, populate it and serves it.
-
-        Parameters
-        ==========
-
-        show : boolean
-            If True, the template will be served on a new browser window.
-            Otherwise, just return the template: ``show=False`` is used
-            by the documentation to visualize servable applications.
-        """
-        if not show:
-            self._init_pane()
-
-        # pn.theme was introduced with panel 1.0.0, before there was
-        # pn.template.theme
-        submodule = pn.theme if hasattr(pn, "theme") else pn.template.theme
-        theme = submodule.DarkTheme
-        if cfg["interactive"]["theme"] != "dark":
-            theme = submodule.DefaultTheme
-        default_template_kw = dict(title=self._name, theme=theme)
-
-        if (self._template is None) or isinstance(self._template, dict):
-            kw = self._template if isinstance(self._template, dict) else {}
-            kw = self.merge(default_template_kw, kw)
-            kw["sidebar_location"] = self._layout
-            if len(self._name.strip()) == 0:
-                kw.setdefault("show_header", False)
-            template = SymPyBootstrapTemplate(**kw)
-        elif isinstance(self._template, pn.template.base.BasicTemplate):
-            template = self._template
-        elif (isinstance(self._template, type) and
-            issubclass(self._template, pn.template.base.BasicTemplate)):
-            template = self._template(**default_template_kw)
-        else:
-            raise TypeError("`template` not recognized. It can either be a "
-                "dictionary of keyword arguments to be passed to the default "
-                "template, an instance of pn.template.base.BasicTemplate "
-                "or a subclass of pn.template.base.BasicTemplate. Received: "
-                "type(template) = %s" % type(self._template))
-
-        template.main.append(self.pane)
-        template.sidebar.append(self.layout_controls)
-
-        if show:
-            return template.servable().show()
-        return template
-
 
 def iplot(*series, show=True, **kwargs):
     """Create an interactive application containing widgets and charts in order
     to study symbolic expressions, using Holoviz's Panel for the user interace.
 
     This function is already integrated with many of the usual
     plotting functions: since their documentation is more specific, it is
@@ -528,15 +543,15 @@
        * rendering of gradient lines is slow.
        * color bars might not update their ranges.
 
 
     Examples
     ========
 
-    NOTE: the following examples use the ordinary plotting function because
+    NOTE: the following examples use the ordinary plotting functions because
     ``iplot`` is already integrated with them.
 
     Surface plot between -10 <= x, y <= 10 discretized with 50 points
     on both directions, with a damping parameter varying from 0 to 1, and a
     default value of 0.15:
 
     .. panel-screenshot::
```

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/__init__.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/complex_analysis.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/complex_analysis.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/control.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/functions_2d.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/functions_2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/functions_3d.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/functions_3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plot_functions/vectors.py` & `sympy_plot_backends-3.4.0/spb/plot_functions/vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/plotgrid.py` & `sympy_plot_backends-3.4.0/spb/plotgrid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from spb.animation import BaseAnimation
 from spb.defaults import cfg
 from spb.backends.matplotlib import MB
 from spb.backends.plotly import PB
 from spb.backends.bokeh import BB
 from spb.interactive import IPlot, create_interactive_plot
+from spb.utils import _aggregate_parameters
 from sympy.utilities.exceptions import sympy_deprecation_warning
 from sympy.external import import_module
 
 
 # NOTE: the code in this module, particularly the one about interactive widget
 # plot, is ugly and probably difficult to comprehend. Turns out that it is
 # extremely difficult to get ipywidgets (and in much less extent, panel) to
@@ -106,52 +108,14 @@
         p.draw()
         new_plots.append(p)
 
     fig.tight_layout()
     return fig, new_plots
 
 
-def _create_ipywidgets_figure(mapping, panel_kw):
-    ipy = import_module('ipywidgets')
-    plotly = import_module(
-        'plotly',
-        import_kwargs={'fromlist': ['graph_objects']},
-        warn_not_installed=True,
-        min_module_version='5.0.0')
-    go = plotly.graph_objects
-
-    fig = ipy.GridspecLayout(**panel_kw)
-    bokeh_outputs_plots = []
-    for spec, p in mapping.items():
-        rs = spec.rowspan
-        cs = spec.colspan
-        plot_fig = p.fig
-        if isinstance(p, PB):
-            # ipywidgets requires Plotly's FigureWidget
-            plot_fig = go.FigureWidget(p.fig.to_dict())
-        elif _are_all_plots_instances_of([p], BB):
-            bokeh = import_module(
-                'bokeh',
-                import_kwargs={'fromlist': ['io']},
-                warn_not_installed=True,
-                min_module_version='2.3.0')
-            # let's assume cfg["bokeh"]["height"] is an integer
-            min_height = str(cfg["bokeh"]["height"]) + "px"
-            new_fig = ipy.Output(layout=ipy.Layout(
-                height='auto', min_height=min_height,
-                width='100%', max_width="100%")
-            )
-            with new_fig:
-                bokeh.io.show(plot_fig)
-            bokeh_outputs_plots.append((new_fig, p))
-            plot_fig = new_fig
-        fig[slice(rs.start, rs.stop), slice(cs.start, cs.stop)] = ipy.Box([plot_fig])
-    return fig, bokeh_outputs_plots
-
-
 def _check_gs(gs):
     """Helper function to verify the provided GridSpec.
     """
     if not isinstance(gs, dict):
         raise TypeError("`gs` must be a dictionary.")
 
     matplotlib = import_module(
@@ -200,36 +164,14 @@
             "The provided interactive plots uses different interactive "
             "modules. This is not supported. Please, only chose one "
             "interactive module for all plots.\n"
             f"Received interactive modules: {imodules}")
     return imodules.pop() if len(imodules) > 0 else None
 
 
-def _check_imodules(plots_imodule, plotgrid_imodule):
-    def raise_error(plots_imodule, plotgrid_imodule):
-        raise ValueError(
-            "The interactive module used by `plotgrid` is different from "
-            "the interactive module used by the plots. This is not supported. "
-            "Please, only chose one interactive module. Received:\n"
-            f"plotgrid imodule={plotgrid_imodule}\n"
-            f"plots imodule={plots_imodule}"
-        )
-    default_imodule = cfg["interactive"]["module"]
-    if (plots_imodule is None) and (plotgrid_imodule is None):
-        pass
-    elif plots_imodule is None:
-        if plotgrid_imodule != default_imodule:
-            raise_error(default_imodule, plotgrid_imodule)
-    elif plotgrid_imodule is None:
-        if plots_imodule != default_imodule:
-            raise_error(plots_imodule, default_imodule)
-    elif plotgrid_imodule != plots_imodule:
-        raise_error(plots_imodule, plotgrid_imodule)
-
-
 def plotgrid(*args, **kwargs):
     """Combine multiple plots into a grid-like layout.
     This function has two modes of operation, depending on the input arguments.
     Make sure to read the examples to fully understand them.
 
     Parameters
     ==========
@@ -389,39 +331,204 @@
         _check_gs(gs)
         plots = list(gs.values())
         plots_imodule = _get_plots_imodule(plots)
         all_parameters, new_args = _get_all_parameters(plots)
     else:
         plots_imodule = None
 
-    _check_imodules(plots_imodule, kwargs.get("imodule", None))
+
+    plotgrid_imodule = kwargs.get("imodule", None)
+    if (plotgrid_imodule is None) and plots_imodule:
+        plotgrid_imodule = plots_imodule
+
+    # NOTE: plots_imodule can be None, meaning it was not provided by
+    # the user.
+    if plots_imodule and (plotgrid_imodule != plots_imodule):
+        raise ValueError(
+            "The interactive module used by `plotgrid` is different from "
+            "the interactive module used by the plots. This is not supported. "
+            "Please, only chose one interactive module. Received:\n"
+            f"plotgrid imodule={plotgrid_imodule}\n"
+            f"plots imodule={plots_imodule}"
+        )
+
+    if plotgrid_imodule:
+        # assure the proper interactive module is going to be used
+        kwargs["imodule"] = plotgrid_imodule
 
     is_iplot = len(all_parameters) > 0
     p = PlotGrid(nr, nc, *args, show=False, is_iplot=is_iplot, **kwargs)
     if is_iplot:
         kwargs["plotgrid"] = p
         kwargs["params"] = all_parameters
         kwargs["show"] = show
+        kwargs["animation"] = any(
+            isinstance(plot, BaseAnimation) for plot in p._all_plots)
         return create_interactive_plot(**kwargs)
 
     if not show:
         return p
     if p.is_matplotlib_fig:
         p.show()
         return p
     return p.show()
 
 
-class PlotGrid:
+class IpywidgetsEnabler:
+    """Necessary code to get ipywidgets and interactive features to work with
+    PlotGrid.
+    """
+
+    def _create_ipywidgets_figure(self, mapping, panel_kw):
+        ipy = import_module('ipywidgets')
+        plotly = import_module(
+            'plotly',
+            import_kwargs={'fromlist': ['graph_objects']},
+            warn_not_installed=True,
+            min_module_version='5.0.0')
+        go = plotly.graph_objects
+
+        fig = ipy.GridspecLayout(**panel_kw)
+        bokeh_outputs_plots = []
+        for spec, p in mapping.items():
+            rs = spec.rowspan
+            cs = spec.colspan
+            plot_fig = p.fig
+            if isinstance(p, PB):
+                # ipywidgets requires Plotly's FigureWidget
+                plot_fig = go.FigureWidget(p.fig.to_dict())
+            elif _are_all_plots_instances_of([p], BB):
+                bokeh = import_module(
+                    'bokeh',
+                    import_kwargs={'fromlist': ['io']},
+                    warn_not_installed=True,
+                    min_module_version='2.3.0')
+                # let's assume cfg["bokeh"]["height"] is an integer
+                min_height = str(cfg["bokeh"]["height"]) + "px"
+                new_fig = ipy.Output(layout=ipy.Layout(
+                    height='auto', min_height=min_height,
+                    width='100%', max_width="100%")
+                )
+                with new_fig:
+                    bokeh.io.show(plot_fig)
+                bokeh_outputs_plots.append((new_fig, p))
+                plot_fig = new_fig
+            fig[slice(rs.start, rs.stop), slice(cs.start, cs.stop)] = ipy.Box([plot_fig])
+        return fig, bokeh_outputs_plots
+
+
+class PanelEnabler:
+    """Necessary code to get panel and interactive features to work with
+    PlotGrid.
+
+    Notes
+    =====
+
+    In a panel figure, each subplot is wrapped by a pane, which is bound to
+    a particular update function, depending if the subplot is a Plotly figure
+    (or something else), or if it is an animation.
+    """
+    def __init__(self, *args, **kwargs):
+        # those are set by spb.interactive.panel, they allow binding widgets
+        # to appropriate update functions.
+        self._params_symbols, self._params_widgets = None, None
+        # this is set by spb.interactive.animation.panel. It allows to access
+        # the animation data
+        self._animation = None
+
+    def pre_set_bindings(self, symbols, widgets):
+        """Set the necessary data to create bindings for interactive widgets
+        plots with panel.
+        """
+        self._params_symbols = symbols
+        self._params_widgets = widgets
+
+    def pre_set_animation(self, animation):
+        """Let this PlotGrid instance know that we are dealing with an
+        animation. This attribute will be later used to execute the appropriate
+        update function.
+        """
+        self._animation = animation
+
+    def _update_plot(self, p, *values):
+        d = {symb: v for symb, v in zip(self._params_symbols, values)}
+        p.update_interactive(d)
+        return p.fig
+
+    def _update_plotly(self, p, *values):
+        d = {symb: v for symb, v in zip(self._params_symbols, values)}
+        p.update_interactive(d)
+        return p.fig.to_dict()
+
+    def _update_plot_animation(self, p, frame_idx):
+        d = self._animation._animation_data[frame_idx]
+        p.update_interactive(d)
+        return p.fig
+
+    def _update_plotly_animation(self, p, frame_idx):
+        d = self._animation._animation_data[frame_idx]
+        p.update_interactive(d)
+        return p.fig.to_dict()
+
+    def _create_panel_figure(self, mapping):
+        pn = import_module(
+            'panel',
+            min_module_version='0.12.0')
+        pn.extension("plotly")
+
+        panes_plots = {}
+        fig = pn.GridSpec(**self.panel_kw)
+        create_binding = self._params_symbols is not None
+        update_func = self._update_plot
+        update_func_plotly = self._update_plotly
+        if self._is_animation:
+            update_func = self._update_plot_animation
+            update_func_plotly = self._update_plotly_animation
+        for i, (spec, p) in enumerate(mapping.items()):
+            rs = spec.rowspan
+            cs = spec.colspan
+            if isinstance(p, IPlot):
+                # a panel's `pane` must receive a figure of some kind, not another
+                # panel's object, otherwise there will be performance penalty,
+                # especially noticeable with Plotly and Bokeh
+                p = p.backend
+            _fig = p.fig
+            if isinstance(p, PB):
+                pane = pn.pane.Plotly(
+                    _fig.to_dict() if not create_binding else
+                    pn.bind(update_func_plotly, p, *self._params_widgets)
+                )
+            elif isinstance(p, MB):
+                pane = pn.pane.Matplotlib(
+                    _fig if not create_binding else
+                    pn.bind(update_func, p, *self._params_widgets)
+                )
+            elif isinstance(p, BB):
+                pane = pn.pane.Bokeh(
+                    _fig if not create_binding else
+                    pn.bind(update_func, p, *self._params_widgets)
+                )
+            else:
+                pane = pn.pane.panel(
+                    _fig if not create_binding else
+                    pn.bind(update_func, p, *self._params_widgets)
+                )
+            fig[slice(rs.start, rs.stop), slice(cs.start, cs.stop)] = pane
+            panes_plots[pane] = p
+        return fig, panes_plots
+
+
+class PlotGrid(PanelEnabler, IpywidgetsEnabler):
     """Implement the logic to create a grid of plots. Refer to ``plotgrid``
     about examples.
     """
     _panel_row_height = 350
 
     def __init__(self, nrows, ncolumns, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.matplotlib = import_module(
             'matplotlib',
             import_kwargs={'fromlist': ['pyplot', 'gridspec']},
             min_module_version='1.1.0',
             catch=(RuntimeError,))
         self.plt = self.matplotlib.pyplot
 
@@ -443,29 +550,32 @@
         self._bokeh_outputs_plots = []
         # the following is used when imodule="panel". It maps plots to panes,
         # so that panel can update what is shown on the pane after the plots
         # have updated their data.
         self._panes_plots = {}
         self._is_iplot = kwargs.get("is_iplot", False)
         self._imodule = kwargs.get("imodule", cfg["interactive"]["module"])
-        # those are set by spb.interactive.panel, they allow binding widgets
-        # to appropriate update functions.
-        self._params_symbols, self._params_widgets = None, None
 
         # validate GridSpec, if provided
         self.gs = kwargs.get("gs", None)
         if self.gs:
             _check_gs(self.gs)
             self.is_matplotlib_fig = _are_all_plots_instances_of(
                 self.gs.values(), MB)
             self.is_bokeh_fig = _are_all_plots_instances_of(
                 self.gs.values(), BB)
+            self._all_plots = list(self.gs.values())
         else:
             self.is_matplotlib_fig = _are_all_plots_instances_of(args, MB)
             self.is_bokeh_fig = _are_all_plots_instances_of(args, BB)
+            self._all_plots = args
+
+        self._is_animation = kwargs.get("is_animation", any(
+            isinstance(p, BaseAnimation) for p in self._all_plots
+        ))
 
         self.panel_kw = kwargs.get("panel_kw", dict())
 
         if kwargs.get("show", True):
             self.show()
 
     @property
@@ -557,15 +667,15 @@
                     self.panel_kw.setdefault("width", "800px" if not size else get_size(size[0]))
                     if not self.is_bokeh_fig:
                         # NOTE: this doesn't work well with bokeh
                         self.panel_kw.setdefault("height",
                             str(nr * self._panel_row_height) + "px" if not size else get_size(size[1]))
                     self.panel_kw["n_rows"] = nr
                     self.panel_kw["n_columns"] = nc
-                    self._fig, self._bokeh_outputs_plots = _create_ipywidgets_figure(
+                    self._fig, self._bokeh_outputs_plots = self._create_ipywidgets_figure(
                         mapping, self.panel_kw)
 
         else:
             # Second mode of operation
             if self.is_matplotlib_fig:
                 self._fig, self._new_plots = _create_mpl_figure(
                     gs, self.imagegrid, self.size, is_iplot_panel)
@@ -580,77 +690,17 @@
                     self._fig, self._panes_plots = self._create_panel_figure(
                         gs)
                 else:
                     first_element = list(gs.keys())[0]
                     mpl_gs = first_element.get_gridspec()
                     self.panel_kw = {
                         "n_rows": mpl_gs.nrows, "n_columns": mpl_gs.ncols}
-                    self._fig, self._bokeh_outputs_plots = _create_ipywidgets_figure(
+                    self._fig, self._bokeh_outputs_plots = self._create_ipywidgets_figure(
                         gs, self.panel_kw)
 
-
-    def _create_panel_figure(self, mapping):
-        pn = import_module(
-            'panel',
-            min_module_version='0.12.0')
-        pn.extension("plotly")
-
-        panes_plots = {}
-        fig = pn.GridSpec(**self.panel_kw)
-        create_binding = self._params_symbols is not None
-        for i, (spec, p) in enumerate(mapping.items()):
-            rs = spec.rowspan
-            cs = spec.colspan
-            if isinstance(p, IPlot):
-                # a panel's `pane` must receive a figure of some kind, not another
-                # panel's object, otherwise there will be performance penalty,
-                # especially noticeable with Plotly and Bokeh
-                p = p.backend
-            _fig = p.fig
-            if isinstance(p, PB):
-                pane = pn.pane.Plotly(
-                    _fig.to_dict() if not create_binding else
-                    pn.bind(self._update_plotly, p, *self._params_widgets)
-                )
-            elif isinstance(p, MB):
-                pane = pn.pane.Matplotlib(
-                    _fig if not create_binding else
-                    pn.bind(self._update_plot, p, *self._params_widgets)
-                )
-            elif isinstance(p, BB):
-                pane = pn.pane.Bokeh(
-                    _fig if not create_binding else
-                    pn.bind(self._update_plot, p, *self._params_widgets)
-                )
-            else:
-                pane = pn.pane.panel(
-                    _fig if not create_binding else
-                    pn.bind(self._update_plot, p, *self._params_widgets)
-                )
-            fig[slice(rs.start, rs.stop), slice(cs.start, cs.stop)] = pane
-            panes_plots[pane] = p
-        return fig, panes_plots
-
-    def pre_set_bindings(self, symbols, widgets):
-        """Set the necessary data to create bindings for interactive widgets
-        plots with panel.
-        """
-        self._params_symbols = symbols
-        self._params_widgets = widgets
-
-    def _update_plot(self, p, *values):
-        d = {symb: v for symb, v in zip(self._params_symbols, values)}
-        p.update_interactive(d)
-        return p.fig
-
-    def _update_plotly(self, p, *values):
-        d = {symb: v for symb, v in zip(self._params_symbols, values)}
-        p.update_interactive(d)
-        return p.fig.to_dict()
-
     def update_interactive(self, params):
         """Implement the logic to update the data generated by
         interactive-widget plots.
 
         Parameters
         ==========
```

### Comparing `sympy_plot_backends-3.3.0/spb/series.py` & `sympy_plot_backends-3.4.0/spb/series.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/spb/utils.py` & `sympy_plot_backends-3.4.0/spb/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -977,7 +977,70 @@
         ct and isinstance(system, ct.TransferFunction) and
         (system.ninputs == 1) and (system.noutputs == 1)
     ):
         return True
     if isinstance(system, Expr):
         return True
     return False
+
+
+
+def _aggregate_parameters(params, series):
+    """Loop over data series to extract the `params` dictionaries provided by
+    the user. This is necessary when dealing with the ``graphics`` module.
+
+    Parameters
+    ==========
+    params : dict
+        Whatever was provided by the user in the main function call (be it
+        plot(), plot_paramentric(), ..., graphics())
+    series : list
+        Data series of the current interactive widget plot.
+
+    Returns
+    =======
+    params : dict
+    """
+    if params is None:
+        params = {}
+    # if len(params) == 0:
+    #     # this is the case when an interactive widget plot is build with
+    #     # the `graphics` interface.
+    for s in series:
+        if s.is_interactive:
+            # use s._original_params instead of s.params in order to
+            # keep track of multi-values widgets
+            params.update(s._original_params)
+    if len(params) == 0:
+        raise ValueError(
+            "In order to create an interactive plot, "
+            "the `params` dictionary must be provided.")
+    return params
+
+
+def get_environment():
+    """Find which environment is used to run the code.
+
+    Returns
+    =======
+    mode : int
+        0 - the code is running on Jupyter Notebook or qtconsole
+        1 - terminal running IPython
+        2 - other type (?)
+        3 - probably standard Python interpreter
+
+    References
+    ==========
+
+    https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
+
+    """
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == "ZMQInteractiveShell":
+            return 0  # Jupyter notebook or qtconsole
+        elif shell == "TerminalInteractiveShell":
+            return 1  # Terminal running IPython
+        else:
+            return 2  # Other type (?)
+    except NameError:
+        return 3  # Probably standard Python interpreter
```

### Comparing `sympy_plot_backends-3.3.0/spb/wegert.py` & `sympy_plot_backends-3.4.0/spb/wegert.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/PKG-INFO` & `sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy_plot_backends
-Version: 3.3.0
+Version: 3.4.0
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,26 +29,36 @@
 Requires-Dist: plotly>=4.14.3; extra == "all"
 Requires-Dist: panel>=1.0.0; extra == "all"
 Requires-Dist: ipywidgets_bokeh; extra == "all"
 Requires-Dist: colorcet; extra == "all"
 Requires-Dist: k3d>=2.9.7; extra == "all"
 Requires-Dist: vtk; extra == "all"
 Requires-Dist: control>=0.10.0; extra == "all"
+Requires-Dist: imageio; extra == "all"
+Requires-Dist: imageio-ffmpeg; extra == "all"
+Requires-Dist: psutil; extra == "all"
+Requires-Dist: av; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
 Requires-Dist: scipy>=1.7.1; extra == "dev"
 Requires-Dist: adaptive>=0.13.1; extra == "dev"
 Requires-Dist: notebook; extra == "dev"
 Requires-Dist: ipympl>=0.7.0; extra == "dev"
 Requires-Dist: plotly>=4.14.3; extra == "dev"
 Requires-Dist: panel>=1.0.0; extra == "dev"
 Requires-Dist: ipywidgets_bokeh; extra == "dev"
 Requires-Dist: colorcet; extra == "dev"
 Requires-Dist: k3d>=2.9.7; extra == "dev"
 Requires-Dist: vtk; extra == "dev"
 Requires-Dist: control>=0.10.0; extra == "dev"
+Requires-Dist: imageio; extra == "dev"
+Requires-Dist: imageio-ffmpeg; extra == "dev"
+Requires-Dist: psutil; extra == "dev"
+Requires-Dist: av; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: kaleido; extra == "dev"
 Requires-Dist: numpydoc; extra == "dev"
 
@@ -65,15 +75,15 @@
 
 The following plotting libraries are supported: [Matplolib](https://matplotlib.org/), [Plotly](https://plotly.com/), [Bokeh](https://github.com/bokeh/bokeh), [K3D-Jupyter](https://github.com/K3D-tools/K3D-jupyter).
 
 <div>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/iplot_bokeh.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/mpl-streamplot.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/plotly_streamlines_2.png" width=250/>
-<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-spherical-harmonics.png" width=250/>
+<img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/animation.gif" width=250 style="width:250px;height:auto;"/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/bokeh_domain_coloring.png" width=250/>
 <img src="https://raw.githubusercontent.com/Davide-sd/sympy-plot-backends/master/imgs/K3D-cone-vectors.png" width=250/>
 </div>
 
 
 ## What's new in comparison to SymPy
 
@@ -84,14 +94,15 @@
 * visualize discontinuities on 2D line plots.
 * visualize 2D/3D vector fields with quivers or streamlines.
 * visualize complex functions with [domain coloring](https://en.wikipedia.org/wiki/Domain_coloring).
 * visualize entities from the `sympy.geometry` module.
 * visualize control systems' response to input signals, root locus, as well as Bode, Nyquist and Nichols diagrams.
 * create parametric-interactive plots using widgets
   (sliders, buttons, etc.) with *ipywidgets* or *Holoviz's Panel*.
+* create animations.
 
 Please, read the
 [following documentation page](https://sympy-plot-backends.readthedocs.io/en/latest/overview.html#differences-with-sympy-plotting)
 to understand the differences between this module and ``sympy.plotting``.
 
 
 ## Development and Support
```

### Comparing `sympy_plot_backends-3.3.0/sympy_plot_backends.egg-info/SOURCES.txt` & `sympy_plot_backends-3.4.0/sympy_plot_backends.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 spb/doc_utils.py
 spb/functions.py
 spb/plotgrid.py
 spb/series.py
 spb/utils.py
 spb/vectors.py
 spb/wegert.py
+spb/animation/__init__.py
+spb/animation/ipywidgets.py
+spb/animation/panel.py
 spb/backends/__init__.py
 spb/backends/base_backend.py
 spb/backends/base_renderer.py
 spb/backends/utils.py
 spb/backends/bokeh/__init__.py
 spb/backends/bokeh/bokeh.py
 spb/backends/bokeh/renderers/__init__.py
@@ -102,14 +105,15 @@
 spb/graphics/control.py
 spb/graphics/functions_2d.py
 spb/graphics/functions_3d.py
 spb/graphics/graphics.py
 spb/graphics/utils.py
 spb/graphics/vectors.py
 spb/interactive/__init__.py
+spb/interactive/bokeh.py
 spb/interactive/ipywidgets.py
 spb/interactive/panel.py
 spb/interactive/bootstrap_spb/__init__.py
 spb/interactive/bootstrap_spb/bootstrap.css
 spb/interactive/bootstrap_spb/bootstrap.html
 spb/plot_functions/__init__.py
 spb/plot_functions/complex_analysis.py
@@ -125,14 +129,17 @@
 sympy_plot_backends.egg-info/top_level.txt
 tests/test_defaults.py
 tests/test_deprecated_module.py
 tests/test_doc_utils.py
 tests/test_plotgrid.py
 tests/test_series.py
 tests/test_utils.py
+tests/animation/__init__.py
+tests/animation/test_animation.py
+tests/animation/test_panel_ipywidgets.py
 tests/backends/__init__.py
 tests/backends/make_tests.py
 tests/backends/test_base_backend.py
 tests/backends/test_bokeh.py
 tests/backends/test_color_utils.py
 tests/backends/test_k3d.py
 tests/backends/test_matplotlib.py
```

### Comparing `sympy_plot_backends-3.3.0/tests/backends/__init__.py` & `sympy_plot_backends-3.4.0/tests/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/make_tests.py` & `sympy_plot_backends-3.4.0/tests/backends/make_tests.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_base_backend.py` & `sympy_plot_backends-3.4.0/tests/backends/test_base_backend.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_bokeh.py` & `sympy_plot_backends-3.4.0/tests/backends/test_bokeh.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     # surface settings
 
     # Bokeh doesn't use rendering_kw dictionary. Nothing to customize yet.
     p = make_test_plot_contour(BB, rendering_kw=dict(), use_latex=use_latex)
     assert len(p.backend.series) == 1
     f = p.fig
     assert len(f.renderers) == 1
-    assert isinstance(f.renderers[0].glyph, bokeh.models.glyphs.Image)
+    assert isinstance(f.renderers[0], bokeh.models.ContourRenderer)
     # 1 colorbar
     assert len(f.right) == 1
     assert f.right[0].title == label_func(use_latex, cos(a*x**2 + y**2))
     assert f.xaxis.axis_label == xl
     assert f.yaxis.axis_label == yl
 
 
@@ -263,15 +263,15 @@
     p = make_test_plot_vector_2d_quiver(
         BB, contour_kw=dict(), quiver_kw=dict(line_color="red", pivot=pivot)
     )
     if success:
         assert len(p.backend.series) == 2
         f = p.fig
         assert len(f.renderers) == 2
-        assert isinstance(f.renderers[0].glyph, bokeh.models.glyphs.Image)
+        assert isinstance(f.renderers[0], bokeh.models.ContourRenderer)
         assert isinstance(f.renderers[1].glyph, bokeh.models.glyphs.Segment)
         # 1 colorbar
         assert len(f.right) == 1
         assert f.right[0].title == "Magnitude"
         assert f.renderers[1].glyph.line_color == "red"
     else:
         raises(ValueError, lambda: p.fig)
@@ -297,15 +297,15 @@
     p = make_test_plot_vector_2d_streamlines(
         BB, stream_kw=dict(line_color="red"), contour_kw=dict(),
         scalar=scalar, use_latex=use_latex
     )
     assert len(p.backend.series) == 2
     f = p.fig
     assert len(f.renderers) == 2
-    assert isinstance(f.renderers[0].glyph, bokeh.models.glyphs.Image)
+    assert isinstance(f.renderers[0], bokeh.models.ContourRenderer)
     assert isinstance(f.renderers[1].glyph, bokeh.models.glyphs.MultiLine)
     # 1 colorbar
     assert len(f.right) == 1
     assert f.right[0].title == expected_label
     assert f.renderers[1].glyph.line_color == "red"
```

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_color_utils.py` & `sympy_plot_backends-3.4.0/tests/backends/test_color_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_k3d.py` & `sympy_plot_backends-3.4.0/tests/backends/test_k3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_matplotlib.py` & `sympy_plot_backends-3.4.0/tests/backends/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/backends/test_plotly.py` & `sympy_plot_backends-3.4.0/tests/backends/test_plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_complex_analysis.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_complex_analysis.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_control.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_control_min_module.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_control_min_module.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_functions_2d.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_functions_2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_functions_3d.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_functions_3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_graphics.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_graphics.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/graphics/test_vectors.py` & `sympy_plot_backends-3.4.0/tests/graphics/test_vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/interactive/test_interactive.py` & `sympy_plot_backends-3.4.0/tests/interactive/test_interactive.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/interactive/test_ipywidgets.py` & `sympy_plot_backends-3.4.0/tests/interactive/test_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/interactive/test_panel.py` & `sympy_plot_backends-3.4.0/tests/interactive/test_panel.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/plot_functions/test_complex.py` & `sympy_plot_backends-3.4.0/tests/plot_functions/test_complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/plot_functions/test_control.py` & `sympy_plot_backends-3.4.0/tests/plot_functions/test_control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/plot_functions/test_functions_2d.py` & `sympy_plot_backends-3.4.0/tests/plot_functions/test_functions_2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/plot_functions/test_functions_3d.py` & `sympy_plot_backends-3.4.0/tests/plot_functions/test_functions_3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/plot_functions/test_vectors.py` & `sympy_plot_backends-3.4.0/tests/plot_functions/test_vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/test_defaults.py` & `sympy_plot_backends-3.4.0/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/test_deprecated_module.py` & `sympy_plot_backends-3.4.0/tests/test_deprecated_module.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/test_doc_utils.py` & `sympy_plot_backends-3.4.0/tests/test_doc_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/test_plotgrid.py` & `sympy_plot_backends-3.4.0/tests/test_plotgrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,16 @@
 
         # unsymmetric grid (subplots in one line)
         p = PlotGrid(1, 3, p5, p6, p7, show=False)
         filename = "test_grid3.png"
         p.save(os.path.join(tmpdir, filename))
         p.close()
 
-        if pn is not None:
+        if plotly:
+            #
             # holoviz's panel objects
             p1, p2, p3, p4, p5, p6, p7 = _create_plots(PB)
 
             # symmetric grid
             p = PlotGrid(2, 2, p1, p2, p3, p4, show=False, imodule="panel")
             p.save("test_1.html")
```

### Comparing `sympy_plot_backends-3.3.0/tests/test_series.py` & `sympy_plot_backends-3.4.0/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-3.3.0/tests/test_utils.py` & `sympy_plot_backends-3.4.0/tests/test_utils.py`

 * *Files identical despite different names*

