# Comparing `tmp/taurus_pyqtgraph-0.9.0.tar.gz` & `tmp/taurus_pyqtgraph-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taurus_pyqtgraph-0.9.0.tar", last modified: Mon May  6 14:12:48 2024, max compression
+gzip compressed data, was "taurus_pyqtgraph-0.9.0a0.tar", last modified: Fri May  3 11:21:30 2024, max compression
```

## Comparing `taurus_pyqtgraph-0.9.0.tar` & `taurus_pyqtgraph-0.9.0a0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.173292 taurus_pyqtgraph-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     3310 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-06 14:12:48.173292 taurus_pyqtgraph-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.163292 taurus_pyqtgraph-0.9.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     5043 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-06 14:12:48.174292 taurus_pyqtgraph-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3542 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.168292 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/
--rw-rw-rw-   0 root         (0) root         (0)     2229 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5259 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/autopantool.py
--rw-rw-rw-   0 root         (0) root         (0)     6596 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/buffersizetool.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    36050 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curveproperties.py
--rw-rw-rw-   0 root         (0) root         (0)    21153 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curvesmodel.py
--rw-rw-rw-   0 root         (0) root         (0)     6762 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curvespropertiestool.py
--rw-rw-rw-   0 root         (0) root         (0)    10307 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/datainspectortool.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/dateaxisitem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.170292 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/axislabels.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/legendExample.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/taurusplotdataitem.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/taurustrendset.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/y2axis.py
--rw-rw-rw-   0 root         (0) root         (0)     4983 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/exporters.py
--rw-rw-rw-   0 root         (0) root         (0)     6495 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/forcedreadtool.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/legendtool.py
--rw-rw-rw-   0 root         (0) root         (0)     9469 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    10618 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/statisticstool.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusimageitem.py
--rw-rw-rw-   0 root         (0) root         (0)    22127 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusmodelchoosertool.py
--rw-rw-rw-   0 root         (0) root         (0)     6979 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusplotdataitem.py
--rw-rw-rw-   0 root         (0) root         (0)    19561 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurustrendset.py
--rw-rw-rw-   0 root         (0) root         (0)     1645 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/titlepatterneditor.py
--rw-rw-rw-   0 root         (0) root         (0)    22951 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/trend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.171292 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/ui/
--rw-rw-rw-   0 root         (0) root         (0)    15418 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui
--rw-rw-rw-   0 root         (0) root         (0)     3296 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/util.py
--rw-rw-rw-   0 root         (0) root         (0)    11038 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/y2axis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.169292 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1711 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      209 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-06 14:12:48.000000 taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:12:48.173292 taurus_pyqtgraph-0.9.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3143 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_curveproperties.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_dateaxisitem.py
--rw-rw-rw-   0 root         (0) root         (0)    19187 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_taurus_pyqtgraph.py
--rw-rw-rw-   0 root         (0) root         (0)    15834 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_trend.py
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/test_y2axis.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-06 14:12:39.000000 taurus_pyqtgraph-0.9.0/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.085572 taurus_pyqtgraph-0.9.0a0/
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     3310 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-03 11:21:30.085572 taurus_pyqtgraph-0.9.0a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.076572 taurus_pyqtgraph-0.9.0a0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     5043 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-03 11:21:30.086572 taurus_pyqtgraph-0.9.0a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.081572 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/autopantool.py
+-rw-rw-rw-   0 root         (0) root         (0)     6596 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/buffersizetool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    36050 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curveproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)    21153 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curvesmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6762 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curvespropertiestool.py
+-rw-rw-rw-   0 root         (0) root         (0)    10307 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/datainspectortool.py
+-rw-rw-rw-   0 root         (0) root         (0)    11913 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/dateaxisitem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.083572 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/axislabels.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/legendExample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/taurusplotdataitem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/taurustrendset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/y2axis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6495 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/forcedreadtool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/legendtool.py
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    10618 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/statisticstool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusimageitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    22127 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusmodelchoosertool.py
+-rw-rw-rw-   0 root         (0) root         (0)     6979 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusplotdataitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    19561 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurustrendset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/titlepatterneditor.py
+-rw-rw-rw-   0 root         (0) root         (0)    22951 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/trend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.083572 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/ui/
+-rw-rw-rw-   0 root         (0) root         (0)    15418 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    11038 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/y2axis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.082572 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-03 11:21:30.000000 taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 11:21:30.085572 taurus_pyqtgraph-0.9.0a0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3143 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_curveproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_dateaxisitem.py
+-rw-rw-rw-   0 root         (0) root         (0)    19187 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_taurus_pyqtgraph.py
+-rw-rw-rw-   0 root         (0) root         (0)    15834 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_trend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/test_y2axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-03 11:21:21.000000 taurus_pyqtgraph-0.9.0a0/tests/util.py
```

### Comparing `taurus_pyqtgraph-0.9.0/CHANGELOG.md` & `taurus_pyqtgraph-0.9.0a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/CONTRIBUTING.md` & `taurus_pyqtgraph-0.9.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/LICENSE.txt` & `taurus_pyqtgraph-0.9.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/PKG-INFO` & `taurus_pyqtgraph-0.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taurus_pyqtgraph
-Version: 0.9.0
+Version: 0.9.0a0
 Summary: Taurus extension providing pyqtgraph-based widgets
 Home-page: https://gitlab.com/taurus-org/taurus_pyqtgraph
 Author: Taurus Community
 Maintainer: Taurus Community
 Maintainer-email: tauruslib-devel@lists.sourceforge.net
 License: LGPLv3+
 Download-URL: https://gitlab.com/taurus-org/taurus_pyqtgraph
```

### Comparing `taurus_pyqtgraph-0.9.0/README.md` & `taurus_pyqtgraph-0.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/docs/Makefile` & `taurus_pyqtgraph-0.9.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/docs/conf.py` & `taurus_pyqtgraph-0.9.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/docs/installation.rst` & `taurus_pyqtgraph-0.9.0a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/docs/make.bat` & `taurus_pyqtgraph-0.9.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/setup.cfg` & `taurus_pyqtgraph-0.9.0a0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 0.9.0-alpha
 commit = True
 message = Bump version {current_version} to {new_version}
 tag = False
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
```

### Comparing `taurus_pyqtgraph-0.9.0/setup.py` & `taurus_pyqtgraph-0.9.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 
 setup(
     name="taurus_pyqtgraph",
-    version="0.9.0",
+    version="0.9.0-alpha",
     description=description,
     long_description=long_description,
     author=author,
     maintainer=maintainer,
     maintainer_email=maintainer_email,
     url=url,
     download_url=download_url,
```

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/__init__.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     deserialize_opts,
 )
 from .datainspectortool import DataInspectorLine, DataInspectorTool
 from .util import unique_data_item_name, ensure_unique_curve_name
 from .exporters import Taurus4TextExporter
 
 # Do not modify the __version__ manually. To be modified by bumpversion
-__version__ = "0.9.0"
+__version__ = "0.9.0-alpha"
```

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/autopantool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/autopantool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/buffersizetool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/buffersizetool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/cli.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/cli.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curveproperties.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curveproperties.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curvesmodel.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curvesmodel.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/curvespropertiestool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/curvespropertiestool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/datainspectortool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/datainspectortool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/dateaxisitem.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/dateaxisitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/__init__.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/axislabels.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/axislabels.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/legendExample.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/legendExample.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/taurusplotdataitem.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/taurusplotdataitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/taurustrendset.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/taurustrendset.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/examples/y2axis.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/examples/y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/exporters.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/exporters.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/forcedreadtool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/forcedreadtool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/legendtool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/legendtool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/plot.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/plot.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/statisticstool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/statisticstool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusimageitem.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusimageitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusmodelchoosertool.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusmodelchoosertool.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurusplotdataitem.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurusplotdataitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/taurustrendset.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/taurustrendset.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/titlepatterneditor.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/titlepatterneditor.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/trend.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/trend.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/ui/CurvesAppearanceChooser.ui`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/ui/TaurusItemConfDlg.ui`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/util.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/util.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph/y2axis.py` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph/y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/PKG-INFO` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taurus-pyqtgraph
-Version: 0.9.0
+Version: 0.9.0a0
 Summary: Taurus extension providing pyqtgraph-based widgets
 Home-page: https://gitlab.com/taurus-org/taurus_pyqtgraph
 Author: Taurus Community
 Maintainer: Taurus Community
 Maintainer-email: tauruslib-devel@lists.sourceforge.net
 License: LGPLv3+
 Download-URL: https://gitlab.com/taurus-org/taurus_pyqtgraph
```

### Comparing `taurus_pyqtgraph-0.9.0/taurus_pyqtgraph.egg-info/SOURCES.txt` & `taurus_pyqtgraph-0.9.0a0/taurus_pyqtgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_curveproperties.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_curveproperties.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_dateaxisitem.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_dateaxisitem.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_plot.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_taurus_pyqtgraph.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_taurus_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_trend.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_trend.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_util.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/test_y2axis.py` & `taurus_pyqtgraph-0.9.0a0/tests/test_y2axis.py`

 * *Files identical despite different names*

### Comparing `taurus_pyqtgraph-0.9.0/tests/util.py` & `taurus_pyqtgraph-0.9.0a0/tests/util.py`

 * *Files identical despite different names*

