# Comparing `tmp/blissoda-0.4.0.tar.gz` & `tmp/blissoda-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissoda-0.4.0.tar", last modified: Sun May  5 14:56:54 2024, max compression
+gzip compressed data, was "blissoda-0.4.1.tar", last modified: Mon May  6 17:05:57 2024, max compression
```

## Comparing `blissoda-0.4.0.tar` & `blissoda-0.4.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.109564 blissoda-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-05 10:00:40.000000 blissoda-0.4.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6835 2024-05-05 14:56:54.109564 blissoda-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-05 10:00:40.000000 blissoda-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-05 10:00:40.000000 blissoda-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-05 14:56:54.109564 blissoda-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-05 10:00:40.000000 blissoda-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.077564 blissoda-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 14:52:05.000000 blissoda-0.4.0/src/blissoda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/cli_log_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/app/workflow_server/
--rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv0.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv1.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/app/workflow_server/subscribervid31.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/bm02/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/bm02/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/bm02/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/bm23/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/bm23/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/bm23/exafs_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.081564 blissoda-0.4.0/src/blissoda/demo/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/calib.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/example.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id11.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id12.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/id14.py
--rw-rw-rw-   0 root         (0) root         (0)     3629 2024-05-05 14:52:05.000000 blissoda-0.4.0/src/blissoda/demo/id22.py
--rw-rw-rw-   0 root         (0) root         (0)     8312 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/streamline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/demo/user_scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3712 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/all.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id11.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id12.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id14.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/id22.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/streamline.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/user_scripts/xrpd.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/demo/xrpd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/exafs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/exafs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    12940 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/plotter.py
--rw-rw-rw-   0 root         (0) root         (0)     9917 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exafs/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/flint/
--rw-rw-rw-   0 root         (0) root         (0)     1590 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/flint/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id09/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id09/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id09/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id11/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id11/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id12/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id12/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4624 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id12/converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id14/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id14/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4006 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id14/converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id22/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id22/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32576 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id22/stscan_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     5093 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id22/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id24/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id24/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id24/exafs_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/id31/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/id31/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11177 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/optimize_exposure.py
--rw-rw-rw-   0 root         (0) root         (0)     8944 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/streamline_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     3331 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/id31/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/persistent/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/persistent/ndarray/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv0.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv1.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/ordereddict.py
--rw-rw-rw-   0 root         (0) root         (0)     7605 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/persistent/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.085564 blissoda-0.4.0/src/blissoda/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/demo/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    47387 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/background.xy
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/demo/pdf_config.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/exafs/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/exafs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/exafs/exafs.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/id11/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)     3066 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_without_saving.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.089564 blissoda-0.4.0/src/blissoda/resources/id12/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id12/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id12/convert.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/id22/
--rw-rw-rw-   0 root         (0) root         (0)     6390 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/id22/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/streamline/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/reprocess.py
--rw-rw-rw-   0 root         (0) root         (0)     7835 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/streamline_with_calib.json
--rw-rw-rw-   0 root         (0) root         (0)     5685 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/streamline_without_calib.json
--rw-rw-rw-   0 root         (0) root         (0)     3758 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/streamline/time_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.093564 blissoda-0.4.0/src/blissoda/resources/xrpd/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_with_saving.json
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_without_saving.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/seslab/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/seslab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/seslab/streamline_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/streamline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25258 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/streamline/scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/tests/mock_id31/
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/attenuator.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/lima_image.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/setup_globals.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/mock_id31/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)    13550 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_id22.py
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_id31.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/tests/test_persistent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/directories.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/pyfai.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/utils/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda/xrpd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:56:48.000000 blissoda-0.4.0/src/blissoda/xrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/data.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     7078 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    20265 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2024-05-05 10:00:40.000000 blissoda-0.4.0/src/blissoda/xrpd/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:56:54.097564 blissoda-0.4.0/src/blissoda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6835 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4331 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1028 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-05 14:56:54.000000 blissoda-0.4.0/src/blissoda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.455587 blissoda-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-06 11:55:15.000000 blissoda-0.4.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6883 2024-05-06 17:05:57.455587 blissoda-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-06 11:55:15.000000 blissoda-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-06 11:55:15.000000 blissoda-0.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-05-06 17:05:57.455587 blissoda-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-06 11:55:15.000000 blissoda-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.427587 blissoda-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-06 14:35:43.000000 blissoda-0.4.1/src/blissoda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/cli_log_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/app/workflow_server/
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/workflow_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/workflow_server/subscriberv0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/workflow_server/subscriberv1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/app/workflow_server/subscribervid31.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/bm02/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/bm02/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/bm02/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/bm23/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/bm23/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/bm23/exafs_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/demo/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/calib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/id11.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/id12.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/id14.py
+-rw-rw-rw-   0 root         (0) root         (0)     3629 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     8312 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/streamline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/demo/user_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2024-05-06 14:35:43.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/all.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/id11.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/id12.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/id14.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/streamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/user_scripts/xrpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/demo/xrpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.431587 blissoda-0.4.1/src/blissoda/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/exafs/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    12985 2024-05-06 15:42:10.000000 blissoda-0.4.1/src/blissoda/exafs/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/exafs/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/flint/
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/flint/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id09/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id09/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id09/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id11/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id11/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id11/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id12/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id12/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4624 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id12/converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id14/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id14/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4006 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id14/converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id22/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id22/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32576 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id22/stscan_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5093 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id22/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id24/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id24/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id24/exafs_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/id31/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id31/optimize_exposure.py
+-rw-rw-rw-   0 root         (0) root         (0)     8944 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id31/streamline_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3331 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/id31/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/persistent/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/persistent/ndarray/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/ndarray/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/ndarray/ndarrayv0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/ndarray/ndarrayv1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/ordereddict.py
+-rw-rw-rw-   0 root         (0) root         (0)     7605 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/persistent/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/resources/demo/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/demo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    47387 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/demo/background.xy
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/demo/pdf_config.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.435588 blissoda-0.4.1/src/blissoda/resources/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/exafs/exafs.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/resources/id11/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id11/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_without_saving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/resources/id12/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id12/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id12/convert.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/resources/id22/
+-rw-rw-rw-   0 root         (0) root         (0)     6390 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/id22/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/resources/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/streamline/reprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2024-05-06 14:35:43.000000 blissoda-0.4.1/src/blissoda/resources/streamline/streamline_with_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2024-05-06 14:35:43.000000 blissoda-0.4.1/src/blissoda/resources/streamline/streamline_without_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/streamline/time_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/resources/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/xrpd/integrate_scan_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/resources/xrpd/integrate_scan_without_saving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/seslab/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/seslab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/seslab/streamline_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25258 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/streamline/scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.439587 blissoda-0.4.1/src/blissoda/tests/mock_id31/
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/attenuator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/lima_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/setup_globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/mock_id31/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    13550 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/test_id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/test_id31.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/tests/test_persistent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.443587 blissoda-0.4.1/src/blissoda/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/utils/directories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/utils/pyfai.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/utils/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.443587 blissoda-0.4.1/src/blissoda/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 17:05:52.000000 blissoda-0.4.1/src/blissoda/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/xrpd/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/xrpd/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     7078 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/xrpd/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    20265 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/xrpd/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2024-05-06 11:55:15.000000 blissoda-0.4.1/src/blissoda/xrpd/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:05:57.443587 blissoda-0.4.1/src/blissoda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6883 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4331 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-06 17:05:57.000000 blissoda-0.4.1/src/blissoda.egg-info/top_level.txt
```

### Comparing `blissoda-0.4.0/LICENSE.md` & `blissoda-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/PKG-INFO` & `blissoda-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.4.0
+Version: 0.4.1
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -65,14 +65,15 @@
 Provides-Extra: demoworker
 Requires-Dist: blissdata>=0.2.5; extra == "demoworker"
 Requires-Dist: ewoksjob; extra == "demoworker"
 Requires-Dist: ewoksjob[blissworker]>=0.2.1; extra == "demoworker"
 Requires-Dist: ewoksxrpd>=0.3; extra == "demoworker"
 Requires-Dist: est[full]; extra == "demoworker"
 Requires-Dist: orange3; extra == "demoworker"
+Requires-Dist: ewoksid12; extra == "demoworker"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-redis; extra == "test"
 Requires-Dist: scipy; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
```

### Comparing `blissoda-0.4.0/README.md` & `blissoda-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/setup.cfg` & `blissoda-0.4.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 	%(client)s
 demoworker = 
 	%(server)s
 	ewoksjob[blissworker] >=0.2.1
 	ewoksxrpd >=0.3
 	est[full]
 	orange3
+	ewoksid12
 test = 
 	pytest >=7
 	mock
 	pytest-mock
 	pytest-redis
 	scipy
 	%(client)s
```

### Comparing `blissoda-0.4.0/src/blissoda/__init__.py` & `blissoda-0.4.1/src/blissoda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 try:
     from gevent.monkey import is_anything_patched
     from gevent.monkey import is_module_patched
 except ImportError:
     pass
 else:
```

### Comparing `blissoda-0.4.0/src/blissoda/app/__main__.py` & `blissoda-0.4.1/src/blissoda/app/__main__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/app/cli_log_utils.py` & `blissoda-0.4.1/src/blissoda/app/cli_log_utils.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/app/workflow_server/__init__.py` & `blissoda-0.4.1/src/blissoda/app/workflow_server/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv0.py` & `blissoda-0.4.1/src/blissoda/app/workflow_server/subscriberv0.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/app/workflow_server/subscriberv1.py` & `blissoda-0.4.1/src/blissoda/app/workflow_server/subscriberv1.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/app/workflow_server/subscribervid31.py` & `blissoda-0.4.1/src/blissoda/app/workflow_server/subscribervid31.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/bm02/xrpd_processor.py` & `blissoda-0.4.1/src/blissoda/bm02/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/bm23/exafs_plotter.py` & `blissoda-0.4.1/src/blissoda/bm23/exafs_plotter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/exafs.py` & `blissoda-0.4.1/src/blissoda/demo/exafs.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/example.py` & `blissoda-0.4.1/src/blissoda/demo/example.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/id11.py` & `blissoda-0.4.1/src/blissoda/demo/id11.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/id12.py` & `blissoda-0.4.1/src/blissoda/demo/id12.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/id14.py` & `blissoda-0.4.1/src/blissoda/demo/id14.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/id22.py` & `blissoda-0.4.1/src/blissoda/demo/id22.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/streamline.py` & `blissoda-0.4.1/src/blissoda/demo/streamline.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/user_scripts/all.py` & `blissoda-0.4.1/src/blissoda/demo/user_scripts/all.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,14 @@
     print()
     print("SUCCESS: all objects can be printed")
 
 
 def all_demo():
     print()
     print("===================")
-    setup_globals.newcollection("exafs_collection")
-    exafs_demo()
-
-    print()
-    print("===================")
     setup_globals.newcollection("id22_stscan_collection")
     id22_stscan_demo()
 
     print()
     print("===================")
     setup_globals.newcollection("id22_xrpd_collection")
     id22_xrpd_demo()
@@ -90,14 +85,21 @@
     # id11_pdf_demo()
 
     print()
     print("===================")
     setup_globals.newcollection("xrpd_collection")
     xrpd_demo()
 
+    # TODO: ewoksxrpd needs to be imported before xraylarch?
+    #       Cannot load backend 'Qt5Agg' which requires the 'qt' interactive framework
+    print()
+    print("===================")
+    setup_globals.newcollection("exafs_collection")
+    exafs_demo()
+
     print()
     print("===================")
     setup_globals.newcollection("id14_collection")
     id14_demo()
 
     print()
     print("===================")
```

### Comparing `blissoda-0.4.0/src/blissoda/demo/user_scripts/id11.py` & `blissoda-0.4.1/src/blissoda/demo/user_scripts/id11.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/user_scripts/id22.py` & `blissoda-0.4.1/src/blissoda/demo/user_scripts/id22.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/user_scripts/streamline.py` & `blissoda-0.4.1/src/blissoda/demo/user_scripts/streamline.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/user_scripts/xrpd.py` & `blissoda-0.4.1/src/blissoda/demo/user_scripts/xrpd.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/demo/xrpd.py` & `blissoda-0.4.1/src/blissoda/demo/xrpd.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/exafs/plots.py` & `blissoda-0.4.1/src/blissoda/exafs/plots.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/exafs/plotter.py` & `blissoda-0.4.1/src/blissoda/exafs/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
         if filename is None:
             try:
                 filename = scan.writer.get_filename()
             except AttributeError:
                 # bliss < 1.0.0
                 filename = scan.writer.filename
         if os.path.exists(filename):
-            scannr = max(int(float(s)) for s in top_level_names(filename)) + 1
+            scans = top_level_names(filename, include_only=None)
+            scannr = max(int(float(s)) for s in scans) + 1
         else:
             scannr = 1
         scan_legend = f"{scannr}.1"
         scan_url = f"silx://{filename}::/{scannr}.1"
         scan_id = scan_url
         scan_name = os.path.split(os.path.dirname(filename))[-1]
         scan_name = f"{scan_name}:{scannr}.1"
```

### Comparing `blissoda-0.4.0/src/blissoda/exafs/widgets.py` & `blissoda-0.4.1/src/blissoda/exafs/widgets.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/flint/__init__.py` & `blissoda-0.4.1/src/blissoda/flint/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id09/xrpd_processor.py` & `blissoda-0.4.1/src/blissoda/id09/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id11/xrpd_processor.py` & `blissoda-0.4.1/src/blissoda/id11/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id12/converter.py` & `blissoda-0.4.1/src/blissoda/id12/converter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id14/converter.py` & `blissoda-0.4.1/src/blissoda/id14/converter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id22/stscan_processor.py` & `blissoda-0.4.1/src/blissoda/id22/stscan_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id22/xrpd_processor.py` & `blissoda-0.4.1/src/blissoda/id22/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id24/exafs_plotter.py` & `blissoda-0.4.1/src/blissoda/id24/exafs_plotter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id31/optimize_exposure.py` & `blissoda-0.4.1/src/blissoda/id31/optimize_exposure.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id31/streamline_scanner.py` & `blissoda-0.4.1/src/blissoda/id31/streamline_scanner.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/id31/xrpd_processor.py` & `blissoda-0.4.1/src/blissoda/id31/xrpd_processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/persistent/ndarray/__init__.py` & `blissoda-0.4.1/src/blissoda/persistent/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv0.py` & `blissoda-0.4.1/src/blissoda/persistent/ndarray/ndarrayv0.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/persistent/ndarray/ndarrayv1.py` & `blissoda-0.4.1/src/blissoda/persistent/ndarray/ndarrayv1.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/persistent/ordereddict.py` & `blissoda-0.4.1/src/blissoda/persistent/ordereddict.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/persistent/parameters.py` & `blissoda-0.4.1/src/blissoda/persistent/parameters.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/demo/background.xy` & `blissoda-0.4.1/src/blissoda/resources/demo/background.xy`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/exafs/exafs.ows` & `blissoda-0.4.1/src/blissoda/resources/exafs/exafs.ows`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving.json` & `blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json` & `blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_with_saving_pdf.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/id11/integrate_scan_without_saving.json` & `blissoda-0.4.1/src/blissoda/resources/id11/integrate_scan_without_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json` & `blissoda-0.4.1/src/blissoda/resources/id22/Sum_then_integrate_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/streamline/reprocess.py` & `blissoda-0.4.1/src/blissoda/resources/streamline/reprocess.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/streamline/streamline_with_calib.json` & `blissoda-0.4.1/src/blissoda/resources/streamline/streamline_with_calib.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998828125%*

 * *Differences: {"'nodes'": "{7: {'label': 'save_2th_hdf5', 'ows': {'title': 'save_2th_hdf5'}}}"}*

```diff
@@ -337,19 +337,19 @@
             "default_inputs": [
                 {
                     "name": "nxprocess_as_default",
                     "value": true
                 }
             ],
             "id": "7",
-            "label": "save_2th",
+            "label": "save_2th_hdf5",
             "ows": {
                 "name": "SaveNexusPattern1D",
                 "position": "(1019.0, 676.0)",
-                "title": "save_2th",
+                "title": "save_2th_hdf5",
                 "version": ""
             },
             "task_identifier": "ewoksxrpd.tasks.nexus.SaveNexusPattern1D",
             "task_type": "class"
         }
     ]
 }
```

### Comparing `blissoda-0.4.0/src/blissoda/resources/streamline/streamline_without_calib.json` & `blissoda-0.4.1/src/blissoda/resources/streamline/streamline_without_calib.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'nodes'": "{5: {'label': 'save_2th_hdf5', 'ows': {'title': 'save_2th_hdf5'}}}"}*

```diff
@@ -239,19 +239,19 @@
             "default_inputs": [
                 {
                     "name": "nxprocess_as_default",
                     "value": true
                 }
             ],
             "id": "5",
-            "label": "save_2th",
+            "label": "save_2th_hdf5",
             "ows": {
                 "name": "SaveNexusPattern1D",
                 "position": "(648.0, 455.0)",
-                "title": "save_2th",
+                "title": "save_2th_hdf5",
                 "version": ""
             },
             "task_identifier": "ewoksxrpd.tasks.nexus.SaveNexusPattern1D",
             "task_type": "class"
         }
     ]
 }
```

### Comparing `blissoda-0.4.0/src/blissoda/resources/streamline/time_record.py` & `blissoda-0.4.1/src/blissoda/resources/streamline/time_record.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_with_saving.json` & `blissoda-0.4.1/src/blissoda/resources/xrpd/integrate_scan_with_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/resources/xrpd/integrate_scan_without_saving.json` & `blissoda-0.4.1/src/blissoda/resources/xrpd/integrate_scan_without_saving.json`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/seslab/streamline_scanner.py` & `blissoda-0.4.1/src/blissoda/seslab/streamline_scanner.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/streamline/scanner.py` & `blissoda-0.4.1/src/blissoda/streamline/scanner.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/conftest.py` & `blissoda-0.4.1/src/blissoda/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/mock_id31/__init__.py` & `blissoda-0.4.1/src/blissoda/tests/mock_id31/__init__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/mock_id31/controllers.py` & `blissoda-0.4.1/src/blissoda/tests/mock_id31/controllers.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/mock_id31/simulate.py` & `blissoda-0.4.1/src/blissoda/tests/mock_id31/simulate.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/test_id22.py` & `blissoda-0.4.1/src/blissoda/tests/test_id22.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/test_id31.py` & `blissoda-0.4.1/src/blissoda/tests/test_id31.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/tests/test_persistent.py` & `blissoda-0.4.1/src/blissoda/tests/test_persistent.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/utils/directories.py` & `blissoda-0.4.1/src/blissoda/utils/directories.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/utils/pyfai.py` & `blissoda-0.4.1/src/blissoda/utils/pyfai.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/utils/trigger.py` & `blissoda-0.4.1/src/blissoda/utils/trigger.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/xrpd/data.py` & `blissoda-0.4.1/src/blissoda/xrpd/data.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/xrpd/plots.py` & `blissoda-0.4.1/src/blissoda/xrpd/plots.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/xrpd/plotter.py` & `blissoda-0.4.1/src/blissoda/xrpd/plotter.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/xrpd/processor.py` & `blissoda-0.4.1/src/blissoda/xrpd/processor.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda/xrpd/widgets.py` & `blissoda-0.4.1/src/blissoda/xrpd/widgets.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda.egg-info/PKG-INFO` & `blissoda-0.4.1/src/blissoda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.4.0
+Version: 0.4.1
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -65,14 +65,15 @@
 Provides-Extra: demoworker
 Requires-Dist: blissdata>=0.2.5; extra == "demoworker"
 Requires-Dist: ewoksjob; extra == "demoworker"
 Requires-Dist: ewoksjob[blissworker]>=0.2.1; extra == "demoworker"
 Requires-Dist: ewoksxrpd>=0.3; extra == "demoworker"
 Requires-Dist: est[full]; extra == "demoworker"
 Requires-Dist: orange3; extra == "demoworker"
+Requires-Dist: ewoksid12; extra == "demoworker"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-redis; extra == "test"
 Requires-Dist: scipy; extra == "test"
 Requires-Dist: blissdata>=0.2.5; extra == "test"
```

### Comparing `blissoda-0.4.0/src/blissoda.egg-info/SOURCES.txt` & `blissoda-0.4.1/src/blissoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blissoda-0.4.0/src/blissoda.egg-info/requires.txt` & `blissoda-0.4.1/src/blissoda.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 [demoworker]
 blissdata>=0.2.5
 ewoksjob
 ewoksjob[blissworker]>=0.2.1
 ewoksxrpd>=0.3
 est[full]
 orange3
+ewoksid12
 
 [dev]
 pytest>=7
 mock
 pytest-mock
 pytest-redis
 scipy
```

