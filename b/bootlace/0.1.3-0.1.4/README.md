# Comparing `tmp/bootlace-0.1.3.tar.gz` & `tmp/bootlace-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  9 17:02:56 2024, max compression
+gzip compressed data, last modified: Mon May  6 04:18:23 2024, max compression
```

## Comparing `bootlace-0.1.3.tar` & `bootlace-0.1.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      247 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/__about__.py
--rw-r--r--   0        0        0      384 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/__init__.py
--rw-r--r--   0        0        0      411 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/_version.py
--rw-r--r--   0        0        0     8751 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/breadcrumbs.py
--rw-r--r--   0        0        0     1447 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/extension.py
--rw-r--r--   0        0        0     1139 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/icon.py
--rw-r--r--   0        0        0      465 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/image.py
--rw-r--r--   0        0        0     1968 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/links.py
--rw-r--r--   0        0        0        0 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/py.typed
--rw-r--r--   0        0        0      669 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/size.py
--rw-r--r--   0        0        0     1217 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/style.py
--rw-r--r--   0        0        0     6892 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/util.py
--rw-r--r--   0        0        0        0 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/forms/__init__.py
--rw-r--r--   0        0        0     3037 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/forms/fields.py
--rw-r--r--   0        0        0      661 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/forms/widgets.py
--rw-r--r--   0        0        0     1571 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/forms/templates/bootlace/_form.html
--rw-r--r--   0        0        0      109 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/nav/__init__.py
--rw-r--r--   0        0        0     3972 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/nav/bar.py
--rw-r--r--   0        0        0     3518 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/nav/core.py
--rw-r--r--   0        0        0      427 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/nav/elements.py
--rw-r--r--   0        0        0     2475 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/nav/nav.py
--rw-r--r--   0        0        0    70330 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203179 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51796 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115988 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70404 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203183 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51871 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116065 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12066 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129328 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10127 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51370 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12059 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129343 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10199 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63944 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107824 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267492 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85353 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180382 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107692 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267433 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85282 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180218 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   280814 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.css
--rw-r--r--   0        0        0   679012 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.css.map
--rw-r--r--   0        0        0   232949 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   589162 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280393 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   678857 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   233056 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   588696 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0    88585 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.css
--rw-r--r--   0        0        0    47188 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.json
--rw-r--r--   0        0        0   211136 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   972584 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.svg
--rw-r--r--   0        0        0   207731 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444287 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80664 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331887 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135747 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305153 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74155 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222463 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145313 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.js
--rw-r--r--   0        0        0   306321 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    60578 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   220351 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0      253 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/table/__init__.py
--rw-r--r--   0        0        0     4469 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/table/base.py
--rw-r--r--   0        0        0     2056 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/table/columns.py
--rw-r--r--   0        0        0       67 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/testing/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-09 17:02:56.000000 bootlace-0.1.3/src/bootlace/testing/html.py
--rw-r--r--   0        0        0     1222 2024-04-09 17:02:56.000000 bootlace-0.1.3/.gitignore
--rw-r--r--   0        0        0     1096 2024-04-09 17:02:56.000000 bootlace-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      478 2024-04-09 17:02:56.000000 bootlace-0.1.3/README.md
--rw-r--r--   0        0        0     2545 2024-04-09 17:02:56.000000 bootlace-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1323 2024-04-09 17:02:56.000000 bootlace-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/__about__.py
+-rw-r--r--   0        0        0      384 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/_version.py
+-rw-r--r--   0        0        0     8751 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/breadcrumbs.py
+-rw-r--r--   0        0        0     1447 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/extension.py
+-rw-r--r--   0        0        0     1139 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/icon.py
+-rw-r--r--   0        0        0      465 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/image.py
+-rw-r--r--   0        0        0     2004 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/links.py
+-rw-r--r--   0        0        0        0 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/py.typed
+-rw-r--r--   0        0        0      669 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/size.py
+-rw-r--r--   0        0        0     1217 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/style.py
+-rw-r--r--   0        0        0     6950 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/util.py
+-rw-r--r--   0        0        0        0 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/__init__.py
+-rw-r--r--   0        0        0     3037 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/fields.py
+-rw-r--r--   0        0        0      661 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/widgets.py
+-rw-r--r--   0        0        0     1571 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/templates/bootlace/_form.html
+-rw-r--r--   0        0        0      109 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/__init__.py
+-rw-r--r--   0        0        0     4638 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/bar.py
+-rw-r--r--   0        0        0     5049 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/core.py
+-rw-r--r--   0        0        0      427 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/elements.py
+-rw-r--r--   0        0        0     2932 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/nav.py
+-rw-r--r--   0        0        0    70330 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203179 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51796 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115988 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70404 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203183 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51871 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116065 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12066 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129328 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10127 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51370 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12059 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129343 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10199 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63944 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107824 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267492 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85353 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180382 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107692 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267433 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85282 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180218 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280814 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.css
+-rw-r--r--   0        0        0   679012 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232949 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589162 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280393 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678857 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233056 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588696 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0    88585 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    47188 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.json
+-rw-r--r--   0        0        0   211136 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   972584 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207731 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444287 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80664 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331887 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305153 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74155 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222463 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306321 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60578 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220351 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0      299 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/__init__.py
+-rw-r--r--   0        0        0     4469 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/base.py
+-rw-r--r--   0        0        0     2339 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/columns.py
+-rw-r--r--   0        0        0       67 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/testing/__init__.py
+-rw-r--r--   0        0        0     4910 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/testing/html.py
+-rw-r--r--   0        0        0     1222 2024-05-06 04:18:23.000000 bootlace-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1096 2024-05-06 04:18:23.000000 bootlace-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      478 2024-05-06 04:18:23.000000 bootlace-0.1.4/README.md
+-rw-r--r--   0        0        0     2613 2024-05-06 04:18:23.000000 bootlace-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-05-06 04:18:23.000000 bootlace-0.1.4/PKG-INFO
```

### Comparing `bootlace-0.1.3/src/bootlace/breadcrumbs.py` & `bootlace-0.1.4/src/bootlace/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/extension.py` & `bootlace-0.1.4/src/bootlace/extension.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/icon.py` & `bootlace-0.1.4/src/bootlace/icon.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/links.py` & `bootlace-0.1.4/src/bootlace/links.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 __all__ = ["Link", "View"]
 
 
 @attrs.define(kw_only=True, frozen=True)
 class LinkBase(abc.ABC):
     text: MaybeTaggable
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def active(self) -> bool:
         raise NotImplementedError("LinkBase.active must be implemented in a subclass")
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def enabled(self) -> bool:
         raise NotImplementedError("LinkBase.enabled must be implemented in a subclass")
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def url(self) -> str:
         raise NotImplementedError("LinkBase.url must be implemented in a subclass")
 
     def __tag__(self) -> tags.html_tag:
 
         return tags.a(as_tag(self.text), href=self.url)
```

### Comparing `bootlace-0.1.3/src/bootlace/size.py` & `bootlace-0.1.4/src/bootlace/size.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/style.py` & `bootlace-0.1.4/src/bootlace/style.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/util.py` & `bootlace-0.1.4/src/bootlace/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
         if counter == 0:
             return scope
         return f"{scope}-{counter}"
 
     def factory(self, scope: str) -> functools.partial:
         return functools.partial(self, scope)
 
+    def reset(self) -> None:
+        self.scopes.clear()
+
 
 ids = HtmlIDScope()
 
 
 def maybe(cls: type[T]) -> Callable[[str | T], T]:
     """Convert a string to a class instance if necessary."""
```

### Comparing `bootlace-0.1.3/src/bootlace/forms/fields.py` & `bootlace-0.1.4/src/bootlace/forms/fields.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/forms/widgets.py` & `bootlace-0.1.4/src/bootlace/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/forms/templates/bootlace/_form.html` & `bootlace-0.1.4/src/bootlace/forms/templates/bootlace/_form.html`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/nav/bar.py` & `bootlace-0.1.4/src/bootlace/nav/bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
 from dominate.util import container
 
 from .core import Link
 from .core import NavElement
@@ -32,14 +34,28 @@
 
     #: The color of the navbar, if using a bootstrap color class
     color: ColorClass | None = ColorClass.TERTIARY
 
     #: Whether the navbar should be fluid (e.g. full width)
     fluid: bool = True
 
+    def serialize(self) -> dict[str, Any]:
+        data = super().serialize()
+        data["items"] = [item.serialize() for item in self.items]
+        data["expand"] = self.expand.value if self.expand else None
+        data["color"] = self.color.value if self.color else None
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict[str, Any]) -> NavElement:
+        data["items"] = [NavElement.deserialize(item) for item in data["items"]]
+        data["expand"] = SizeClass(data["expand"]) if data["expand"] else None
+        data["color"] = ColorClass(data["color"]) if data["color"] else None
+        return cls(**data)
+
     def __tag__(self) -> tags.html_tag:
         nav = tags.nav(cls="navbar")
         if self.expand:
             nav.classes.add(self.expand.add_to_class("navbar-expand"))
         if self.color:
             nav.classes.add(self.color.add_to_class("bg-body"))
```

### Comparing `bootlace-0.1.3/src/bootlace/nav/core.py` & `bootlace-0.1.4/src/bootlace/nav/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import warnings
 from typing import Any
+from typing import Self
 
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
 
 from bootlace import links
 from bootlace.image import Image
@@ -29,14 +30,34 @@
     FILL = "nav-fill"
     JUSTIFIED = "nav-justified"
 
 
 class NavElement:
     """Base class for nav components"""
 
+    _NAV_ELEMENT_REGISTRY: dict[str, type["NavElement"]] = {}
+
+    def __init_subclass__(cls) -> None:
+        cls._NAV_ELEMENT_REGISTRY[cls.__name__] = cls
+
+    def serialize(self) -> dict[str, Any]:
+        """Serialize the element to a dictionary"""
+        data = attrs.asdict(self)  # type: ignore
+        data["__type__"] = self.__class__.__name__
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict[str, Any]) -> "NavElement":
+        """Deserialize an element from a dictionary"""
+        if cls is NavElement:
+            element_cls = cls._NAV_ELEMENT_REGISTRY.get(data["__type__"], NavElement)
+            del data["__type__"]
+            return element_cls.deserialize(data)
+        return cls(**data)
+
     @property
     def active(self) -> bool:
         """Whether the element is active"""
         return False
 
     @property
     def enabled(self) -> bool:
@@ -68,14 +89,26 @@
 
     #: The link to display, either a URL or a view
     link: links.LinkBase
 
     #: The ID of the element
     id: str = attrs.field(factory=element_id.factory("nav-link"))
 
+    def serialize(self) -> dict[str, Any]:
+        data = super().serialize()
+        data["link"] = attrs.asdict(self.link)
+        data["link"]["__type__"] = self.link.__class__.__name__
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict[str, Any]) -> Self:
+        link_cls = getattr(links, data["link"].pop("__type__"))
+        data["link"] = link_cls(**data["link"])
+        return cls(**data)
+
     @classmethod
     def with_url(cls, url: str, text: str | Image, **kwargs: Any) -> "Link":
         """Create a link with a URL."""
         return cls(link=links.Link(url=url, text=text, **kwargs))
 
     @classmethod
     def with_view(cls, endpoint: str, text: str | Image, **kwargs: Any) -> "Link":
@@ -131,10 +164,20 @@
 
 @attrs.define
 class SubGroup(NavElement):
     """Any grouping of items in the nav bar"""
 
     items: list[NavElement] = attrs.field(factory=list)
 
+    def serialize(self) -> dict[str, Any]:
+        data = super().serialize()
+        data["items"] = [item.serialize() for item in self.items]
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict[str, Any]) -> Self:
+        data["items"] = [NavElement.deserialize(item) for item in data["items"]]
+        return cls(**data)
+
     @property
     def active(self) -> bool:
         return any(item.active for item in self.items)
```

### Comparing `bootlace-0.1.3/src/bootlace/nav/nav.py` & `bootlace-0.1.4/src/bootlace/nav/nav.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import warnings
+from typing import Any
+from typing import Self
 
 import attrs
 from dominate import tags
 
 from .core import NavAlignment
 from .core import NavStyle
 from .core import SubGroup
@@ -20,14 +22,26 @@
 
     #: The style of the nav
     style: NavStyle = NavStyle.PLAIN
 
     #: The alignment of the elments in the nav
     alignment: NavAlignment = NavAlignment.DEFAULT
 
+    def serialize(self) -> dict[str, Any]:
+        data = super().serialize()
+        data["style"] = self.style.name
+        data["alignment"] = self.alignment.name
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict[str, Any]) -> Self:
+        data["style"] = NavStyle[data["style"]]
+        data["alignment"] = NavAlignment[data["alignment"]]
+        return super().deserialize(data)
+
     def __tag__(self) -> tags.html_tag:
         active_endpoint = next((item for item in self.items if item.active), None)
         ul = tags.ul(cls="nav", id=self.id)
 
         if (style := self.style.value) != "":
             ul.classes.add(style)
```

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.min.css` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/css/bootstrap.rtl.min.css.map` & `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.css` & `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.json` & `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.scss` & `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/icons/bootstrap-icons.svg` & `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.min.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.bundle.min.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.min.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.esm.min.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.min.js` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/static/js/bootstrap.min.js.map` & `bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/table/base.py` & `bootlace-0.1.4/src/bootlace/table/base.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/src/bootlace/table/columns.py` & `bootlace-0.1.4/src/bootlace/table/columns.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,12 +55,21 @@
         if getattr(value, self.attribute):
             return as_tag(self.yes)
         return as_tag(self.no)
 
 
 @attrs.define
 class Datetime(ColumnBase):
-    """A column which shows a datetime attribute as an ISO formatted string."""
+    """A column which shows a datetime attribute as an ISO formatted string.
+
+    This column can also be used for date or time objects.
+
+    A format string can be provided to format the datetime object."""
+
+    format: str | None = attrs.field(default=None)
 
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
+        if self.format:
+            return text(getattr(value, self.attribute).strftime(self.format))
+
         return text(getattr(value, self.attribute).isoformat())
```

### Comparing `bootlace-0.1.3/src/bootlace/testing/html.py` & `bootlace-0.1.4/src/bootlace/testing/html.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/.gitignore` & `bootlace-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/LICENSE.txt` & `bootlace-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.3/pyproject.toml` & `bootlace-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/bootlace/_version.py"
 
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
+
 [project.urls]
 Documentation = "https://github.com/alexrudy/bootlace#readme"
 Issues = "https://github.com/alexrudy/bootlace/issues"
 Source = "https://github.com/alexrudy/bootlace"
 
 [tool.hatch.build.targets.sdist]
 include = ["src/"]
```

### Comparing `bootlace-0.1.3/PKG-INFO` & `bootlace-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bootlace
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pythonic Bootstrap Utilities
 Project-URL: Documentation, https://github.com/alexrudy/bootlace#readme
 Project-URL: Issues, https://github.com/alexrudy/bootlace/issues
 Project-URL: Source, https://github.com/alexrudy/bootlace
 Author-email: Alex Rudy <github@alexrudy.net>
 License-Expression: MIT
 License-File: LICENSE.txt
```

