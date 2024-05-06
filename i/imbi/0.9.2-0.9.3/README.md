# Comparing `tmp/imbi-0.9.2.tar.gz` & `tmp/imbi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imbi-0.9.2.tar", last modified: Fri Mar 26 19:29:54 2021, max compression
+gzip compressed data, was "dist/imbi-0.9.3.tar", last modified: Fri Mar 26 21:15:20 2021, max compression
```

## Comparing `imbi-0.9.2.tar` & `imbi-0.9.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.015662 imbi-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-03-26 19:26:03.000000 imbi-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-03-26 19:26:03.000000 imbi-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2021-03-26 19:29:54.015662 imbi-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-03-26 19:26:03.000000 imbi-0.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-26 19:26:03.000000 imbi-0.9.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:53.987660 imbi-0.9.2/imbi/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:53.995660 imbi-0.9.2/imbi/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)     4625 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/authentication_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)    17928 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/cookie_cutters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/environments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/fact_type_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/fact_type_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/fact_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:53.995660 imbi-0.9.2/imbi/endpoints/operations/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/operations/changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_fact_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_facts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_link_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2236 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/project_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/projects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:53.995660 imbi-0.9.2/imbi/endpoints/reports/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/reports/namespace_kpis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/endpoints/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/ldap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/openapi.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/pkgfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.003661 imbi-0.9.2/imbi/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.003661 imbi-0.9.2/imbi/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/static/css/backend.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.011661 imbi-0.9.2/imbi/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   138628 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Black.woff
--rw-r--r--   0 runner    (1001) docker     (121)   102832 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Black.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   145612 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-BlackItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   108564 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-BlackItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   143100 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)   106052 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   149808 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   111644 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   142760 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraBold.woff
--rw-r--r--   0 runner    (1001) docker     (121)   106048 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraBold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   149372 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   111896 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   140736 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraLight.woff
--rw-r--r--   0 runner    (1001) docker     (121)   104128 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraLight.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   148664 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraLightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   110820 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ExtraLightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   143188 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   106604 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   140612 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Light.woff
--rw-r--r--   0 runner    (1001) docker     (121)   103944 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   148812 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-LightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   111212 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-LightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   142340 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (121)   105500 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   149704 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-MediumItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   111968 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-MediumItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   133856 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    98804 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   142760 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-SemiBold.woff
--rw-r--r--   0 runner    (1001) docker     (121)   105992 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-SemiBold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   149776 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-SemiBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   111676 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-SemiBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   135872 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (121)    99556 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   144128 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ThinItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   106320 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-ThinItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   240240 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-italic.var.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   224744 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter-roman.var.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   319784 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/fonts/Inter.var.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.015662 imbi-0.9.2/imbi/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/static/images/icon2x.png
--rw-r--r--   0 runner    (1001) docker     (121)    28807 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/static/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (121)    11658 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)  2403363 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/imbi.js
--rw-r--r--   0 runner    (1001) docker     (121)  5102173 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi/static/imbi.js.map
--rw-r--r--   0 runner    (1001) docker     (121)   930543 2021-03-26 19:26:36.000000 imbi-0.9.2/imbi/static/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:54.015662 imbi-0.9.2/imbi/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/templates/docs.html
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)   193720 2021-03-26 19:27:21.000000 imbi-0.9.2/imbi/templates/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/transcoders.py
--rw-r--r--   0 runner    (1001) docker     (121)    13077 2021-03-26 19:26:03.000000 imbi-0.9.2/imbi/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 19:29:53.991660 imbi-0.9.2/imbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-26 19:29:53.000000 imbi-0.9.2/imbi.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2021-03-26 19:29:54.015662 imbi-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       60 2021-03-26 19:26:03.000000 imbi-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.511232 imbi-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-03-26 21:11:31.000000 imbi-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-03-26 21:11:31.000000 imbi-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4506 2021-03-26 21:15:20.511232 imbi-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-03-26 21:11:31.000000 imbi-0.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-26 21:11:31.000000 imbi-0.9.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.475230 imbi-0.9.3/imbi/
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6812 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.483230 imbi-0.9.3/imbi/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (121)     4625 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/authentication_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17928 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/cookie_cutters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/default.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1531 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/environments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/fact_type_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/fact_type_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/fact_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1632 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.483230 imbi-0.9.3/imbi/endpoints/operations/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/operations/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_fact_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_facts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_link_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2236 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/project_urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10011 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/projects.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.483230 imbi-0.9.3/imbi/endpoints/reports/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/reports/namespace_kpis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/endpoints/ui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/pkgfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5159 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.491231 imbi-0.9.3/imbi/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.495231 imbi-0.9.3/imbi/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/static/css/backend.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.507231 imbi-0.9.3/imbi/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)   138628 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Black.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   102832 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Black.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   145612 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-BlackItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   108564 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-BlackItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   143100 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   106052 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   149808 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   111644 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   142760 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraBold.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   106048 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   149372 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   111896 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   140736 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraLight.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   104128 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraLight.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   148664 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraLightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   110820 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ExtraLightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   143188 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   106604 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   140612 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   103944 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   148812 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   111212 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   142340 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   105500 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   149704 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-MediumItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   111968 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-MediumItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   133856 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    98804 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   142760 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-SemiBold.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   105992 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-SemiBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   149776 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-SemiBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   111676 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-SemiBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   135872 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    99556 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   144128 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ThinItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   106320 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-ThinItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   240240 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-italic.var.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   224744 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter-roman.var.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   319784 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/fonts/Inter.var.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.511232 imbi-0.9.3/imbi/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     3927 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/static/images/icon2x.png
+-rw-r--r--   0 runner    (1001) docker     (121)    28807 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/static/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    11658 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)  2403427 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/imbi.js
+-rw-r--r--   0 runner    (1001) docker     (121)  5102320 2021-03-26 21:15:19.000000 imbi-0.9.3/imbi/static/imbi.js.map
+-rw-r--r--   0 runner    (1001) docker     (121)   930543 2021-03-26 21:12:02.000000 imbi-0.9.3/imbi/static/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.511232 imbi-0.9.3/imbi/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/templates/docs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)   193720 2021-03-26 21:12:46.000000 imbi-0.9.3/imbi/templates/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/transcoders.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13077 2021-03-26 21:11:31.000000 imbi-0.9.3/imbi/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-26 21:15:20.479230 imbi-0.9.3/imbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4506 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3243 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-26 21:15:20.000000 imbi-0.9.3/imbi.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     3040 2021-03-26 21:15:20.511232 imbi-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       60 2021-03-26 21:11:31.000000 imbi-0.9.3/setup.py
```

### Comparing `imbi-0.9.2/LICENSE` & `imbi-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/PKG-INFO` & `imbi-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbi
-Version: 0.9.2
+Version: 0.9.3
 Summary: Imbi is a DevOps Service Management Platform designed to provide an efficient way to manage a large environment that contains many services and applications.
 Home-page: https://github.com/aweber/imbi
 Author: Gavin M. Roy
 Author-email: gavinr@aweber.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/aweber/imbi/issues
 Project-URL: Documentation, https://imbi.readthedocs.io
```

### Comparing `imbi-0.9.2/README.rst` & `imbi-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/app.py` & `imbi-0.9.3/imbi/app.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/common.py` & `imbi-0.9.3/imbi/common.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/__init__.py` & `imbi-0.9.3/imbi/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/authentication_tokens.py` & `imbi-0.9.3/imbi/endpoints/authentication_tokens.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/base.py` & `imbi-0.9.3/imbi/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/cookie_cutters.py` & `imbi-0.9.3/imbi/endpoints/cookie_cutters.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/dashboard.py` & `imbi-0.9.3/imbi/endpoints/dashboard.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/environments.py` & `imbi-0.9.3/imbi/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/fact_type_enums.py` & `imbi-0.9.3/imbi/endpoints/fact_type_enums.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/fact_type_ranges.py` & `imbi-0.9.3/imbi/endpoints/fact_type_ranges.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/fact_types.py` & `imbi-0.9.3/imbi/endpoints/fact_types.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/groups.py` & `imbi-0.9.3/imbi/endpoints/groups.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/namespaces.py` & `imbi-0.9.3/imbi/endpoints/namespaces.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/openapi.py` & `imbi-0.9.3/imbi/endpoints/openapi.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_dependencies.py` & `imbi-0.9.3/imbi/endpoints/project_dependencies.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_fact_types.py` & `imbi-0.9.3/imbi/endpoints/project_fact_types.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_facts.py` & `imbi-0.9.3/imbi/endpoints/project_facts.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_link_types.py` & `imbi-0.9.3/imbi/endpoints/project_link_types.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_links.py` & `imbi-0.9.3/imbi/endpoints/project_links.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_types.py` & `imbi-0.9.3/imbi/endpoints/project_types.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/project_urls.py` & `imbi-0.9.3/imbi/endpoints/project_urls.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/projects.py` & `imbi-0.9.3/imbi/endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/reports/namespace_kpis.py` & `imbi-0.9.3/imbi/endpoints/reports/namespace_kpis.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/status.py` & `imbi-0.9.3/imbi/endpoints/status.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/endpoints/ui.py` & `imbi-0.9.3/imbi/endpoints/ui.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/ldap.py` & `imbi-0.9.3/imbi/ldap.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/openapi.py` & `imbi-0.9.3/imbi/openapi.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/pkgfiles.py` & `imbi-0.9.3/imbi/pkgfiles.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/server.py` & `imbi-0.9.3/imbi/server.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/session.py` & `imbi-0.9.3/imbi/session.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/css/backend.css` & `imbi-0.9.3/imbi/static/css/backend.css`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Black.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Black.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-BlackItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-BlackItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Bold.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Bold.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-BoldItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-BoldItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraBold.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraBold.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraBoldItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraBoldItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraLight.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraLight.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraLightItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ExtraLightItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Italic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Italic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Light.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Light.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-LightItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-LightItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Medium.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Medium.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-MediumItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-MediumItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Regular.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Regular.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-SemiBold.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-SemiBold.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-SemiBoldItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-SemiBoldItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Thin.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-Thin.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ThinItalic.woff` & `imbi-0.9.3/imbi/static/fonts/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-ThinItalic.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-italic.var.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter-roman.var.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/fonts/Inter.var.woff2` & `imbi-0.9.3/imbi/static/fonts/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/images/icon2x.png` & `imbi-0.9.3/imbi/static/images/icon2x.png`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/images/logo.ico` & `imbi-0.9.3/imbi/static/images/logo.ico`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/images/logo.png` & `imbi-0.9.3/imbi/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/images/logo.svg` & `imbi-0.9.3/imbi/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/static/imbi.js` & `imbi-0.9.3/imbi/static/imbi.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -44631,15 +44631,15 @@
     }
 
     function nu(e) {
         var n = e.fact,
             t = e.offset,
             r = $t().t,
             a = "border-gray-300";
-        return n.score >= 0 && (a = "border-red-600"), n.score > 69 && (a = "border-yellow-600"), n.score > 89 && (a = "border-green-600"), "boolean" === n.data_type && "true" === n.value && (a = "border-green-600"), s.a.createElement("div", {
+        return n.score > 0 && (a = "border-red-600"), n.score > 69 && (a = "border-yellow-600"), n.score > 89 && (a = "border-green-600"), "boolean" === n.data_type && "true" === n.value && (a = "border-green-600"), "boolean" === n.data_type && "false" === n.value && (a = "border-red-600"), s.a.createElement("div", {
             key: "fact-".concat(n.fact_type_id),
             className: "".concat(t % 2 == 0 ? "bg-gray-50" : "bg-white", " px-2 py-1 flex flex-row sm:px-6 border-l-4 mb-1 text-gray-900 ").concat(a)
         }, s.a.createElement("dt", {
             className: "font-medium text-gray-500 w-6/12"
         }, n.name), s.a.createElement("dd", {
             className: "w-6/12 mt-1 items-start sm:mt-0 truncate"
         }, s.a.createElement(Bi, {
```

### Comparing `imbi-0.9.2/imbi/static/imbi.js.map` & `imbi-0.9.3/imbi/static/imbi.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9283959283959283%*

 * *Differences: {"'mappings'": "'aACE,IAAIA,EAAmB,GAGvB,SAASC,EAAoBC,GAG5B,GAAGF,EAAiBE,GACnB,OAAOF,EAAiBE,GAAUC,QAGnC,IAAIC,EAASJ,EAAiBE,GAAY,CACzCG,EAAGH,EACHI,GAAG,EACHH,QAAS,IAUV,OANAI,EAAQL,GAAUM,KAAKJ,EAAOD,QAASC,EAAQA,EAAOD,QAASF,GAG/DG,EAAOE,GAAI,EAGJF,EAAOD,QAKfF,EAAoBQ,EAAIF,EAGxBN,EAAoBS,EAAIV,EAGxBC,EAAoBU,EAAI,SAASR,EAASS,EAAMC,GAC3CZ,EAAoBa,EAAEX,EAASS,IAClCG,OAAOC,eAAeb,EAASS,EAAM,CAAEK,YAAY,EAAMC,IAAKL,KAKhEZ,EAAoBkB,EAAI,SAAShB,GACX,oBAAXiB,QAA0BA,OAAOC,aAC1CN,OAAOC,eAAeb,EAASiB,OAAOC,YAAa,CAAEC,MAAO,WAE7D […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "imbi.js",
     "names": [
         "installedModules",
         "__webpack_require__",
         "moduleId",
         "exports",
         "module",
         "i",
@@ -10226,15 +10226,15 @@
         "import PropTypes from 'prop-types'\nimport React, { useContext, useEffect } from 'react'\n\nimport { Context } from '../../state'\nimport { WishedFutureState } from '../../components'\n\nfunction FactHistory({ urlPath }) {\n  const [state, dispatch] = useContext(Context)\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        title: 'project.factHistory',\n        url: new URL(`${urlPath}/fact-history`, state.baseURL)\n      }\n    })\n  }, [])\n  return (\n    <div className=\"pt-20 flex items-center justify-center\">\n      <WishedFutureState>\n        This tab will contain the history for fact changes in the project and\n        include visualizations that shows health score changes over time.\n      </WishedFutureState>\n    </div>\n  )\n}\nFactHistory.propTypes = {\n  urlPath: PropTypes.string.isRequired\n}\nexport { FactHistory }\n",
         "import PropTypes from 'prop-types'\nimport React, { useContext, useEffect } from 'react'\n\nimport { WishedFutureState } from '../../components'\nimport { Context } from '../../state'\n\nfunction Logs({ urlPath }) {\n  const [state, dispatch] = useContext(Context)\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        title: 'common.logs',\n        url: new URL(`${urlPath}/log`, state.baseURL)\n      }\n    })\n  }, [])\n  return (\n    <div className=\"pt-20 flex items-center justify-center\">\n      <WishedFutureState>\n        This tab will provide an interface for displaying project specific logs\n        from the log aggregation service (ELK, Loggly, etc).\n      </WishedFutureState>\n    </div>\n  )\n}\nLogs.propTypes = {\n  urlPath: PropTypes.string.isRequired\n}\nexport { Logs }\n",
         "import PropTypes from 'prop-types'\nimport React, { useContext, useEffect } from 'react'\n\nimport { Context } from '../../state'\nimport { WishedFutureState } from '../../components'\n\nfunction Notes({ urlPath }) {\n  const [state, dispatch] = useContext(Context)\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        title: 'common.notes',\n        url: new URL(`${urlPath}/notes`, state.baseURL)\n      }\n    })\n  }, [])\n  return (\n    <div className=\"pt-20 flex items-center justify-center\">\n      <WishedFutureState>\n        This tab will allow for the viewing and editing of project specific\n        notes.\n      </WishedFutureState>\n    </div>\n  )\n}\nNotes.propTypes = {\n  urlPath: PropTypes.string.isRequired\n}\nexport { Notes }\n",
         "import PropTypes from 'prop-types'\nimport React, { useContext, useEffect } from 'react'\n\nimport { WishedFutureState } from '../../components'\nimport { Context } from '../../state'\n\nfunction OpsLog({ urlPath }) {\n  const [state, dispatch] = useContext(Context)\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        title: 'operationsLog.title',\n        url: new URL(`${urlPath}/operations-log`, state.baseURL)\n      }\n    })\n  }, [])\n  return (\n    <div className=\"pt-20 flex items-center justify-center\">\n      <WishedFutureState>\n        This tab will allow for a project specific view of the operations log\n        entries.\n      </WishedFutureState>\n    </div>\n  )\n}\nOpsLog.propTypes = {\n  urlPath: PropTypes.string.isRequired\n}\nexport { OpsLog }\n",
         "import { compare } from 'fast-json-patch'\nimport PropTypes from 'prop-types'\nimport React, { Fragment, useContext, useEffect, useState } from 'react'\nimport { default as slugify } from 'slugify'\nimport { useTranslation } from 'react-i18next'\n\nimport { asOptions } from '../../metadata'\nimport { Card, ErrorBoundary, Form, Icon } from '../../components'\nimport { Context } from '../../state'\nimport { jsonSchema } from '../../schema/Project'\nimport { httpDelete, httpPost, httpPatch } from '../../utils'\n\nasync function saveLinkChanges(globalState, project, originalLinks, links) {\n  const errors = []\n  const ops = {\n    add: [],\n    delete: [],\n    update: []\n  }\n  // Build arrays of operations for syncing individual records\n  Object.entries(links).forEach(([key, url]) => {\n    const linkTypeID = parseInt(key)\n    if (url.trim() === '' && originalLinks[linkTypeID] !== undefined) {\n      ops.delete.push(linkTypeID)\n    } else if (originalLinks[linkTypeID] === undefined) {\n      ops.add.push({\n        project_id: project.id,\n        link_type_id: linkTypeID,\n        url: url.trim()\n      })\n    } else if (originalLinks[linkTypeID] !== url.trim()) {\n      ops.update.push([\n        linkTypeID,\n        compare(\n          {\n            project_id: project.id,\n            link_type_id: linkTypeID,\n            url: originalLinks[linkTypeID]\n          },\n          {\n            project_id: project.id,\n            link_type_id: linkTypeID,\n            url: url.trim()\n          }\n        )\n      ])\n    }\n  })\n\n  const linkURL = new URL(`/projects/${project.id}/links`, globalState.baseURL)\n  for (let payload of ops.add) {\n    const result = await httpPost(globalState.fetch, linkURL, payload)\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n\n  let linkTypeID\n  for (linkTypeID of ops.delete) {\n    linkURL.pathname = `/projects/${project.id}/links/${linkTypeID}`\n    const result = await httpDelete(globalState.fetch, linkURL)\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n\n  let patch\n  for (patch of ops.update) {\n    linkURL.pathname = `/projects/${project.id}/links/${patch[0]}`\n    const result = await httpPatch(globalState.fetch, linkURL, patch[1])\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n  return [errors.length === 0, errors]\n}\n\nasync function saveProjectChanges(globalState, project, values) {\n  const originalValues = {\n    name: project.name,\n    namespace_id: project.namespace_id,\n    project_type_id: project.project_type_id,\n    slug: project.slug,\n    description: project.description,\n    environments: project.environments\n  }\n  const patchValue = compare(originalValues, values)\n  if (patchValue.length > 0) {\n    const projectURL = new URL(`/projects/${project.id}`, globalState.baseURL)\n    const result = await httpPatch(globalState.fetch, projectURL, patchValue)\n    if (result.success === false) {\n      return [false, result.data]\n    }\n  }\n  return [true, null]\n}\n\nasync function saveURLChanges(globalState, project, environments, urls) {\n  const errors = []\n  const ops = {\n    add: [],\n    delete: [],\n    update: []\n  }\n  // Build arrays of operations for syncing individual records\n  Object.entries(urls).forEach(([key, url]) => {\n    if (url.trim() === '' && project.urls[key] !== undefined) {\n      ops.delete.push(key)\n    } else if (project.urls[key] === undefined) {\n      ops.add.push({\n        project_id: project.id,\n        environment: key,\n        url: url.trim()\n      })\n    } else if (project.urls[key] !== url.trim()) {\n      ops.update.push([\n        key,\n        compare(\n          {\n            project_id: project.id,\n            environment: key,\n            url: project.urls[key]\n          },\n          {\n            project_id: project.id,\n            environment: key,\n            url: url.trim()\n          }\n        )\n      ])\n    } else if (!environments.includes(key)) {\n      ops.delete.push(key)\n    }\n  })\n\n  const projectURL = new URL(\n    `/projects/${project.id}/urls`,\n    globalState.baseURL\n  )\n  for (let payload of ops.add) {\n    const result = await httpPost(globalState.fetch, projectURL, payload)\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n\n  for (let environment of ops.delete) {\n    projectURL.pathname = `/projects/${project.id}/urls/${environment}`\n    const result = await httpDelete(globalState.fetch, projectURL)\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n\n  for (let patch of ops.update) {\n    projectURL.pathname = `/projects/${project.id}/urls/${patch[0]}`\n    const result = await httpPatch(globalState.fetch, projectURL, patch[1])\n    if (result.success === false) {\n      errors.push(result.data)\n    }\n  }\n  return [errors.length === 0, errors]\n}\n\nfunction Edit({ project, onEditFinished }) {\n  const emptyErrors = {\n    namespace_id: null,\n    project_type_id: null,\n    name: null,\n    slug: null,\n    description: null,\n    environments: null\n  }\n  const [globalState] = useContext(Context)\n  const environmentIcons = Object.fromEntries(\n    globalState.metadata.environments.map((environment) => [\n      environment.name,\n      environment.icon_class\n    ])\n  )\n\n  const originalLinks = Object.fromEntries(\n    project.links.map((link) => [link.link_type_id, link.url])\n  )\n\n  const [state, setState] = useState({\n    errorMessage: null,\n    projectErrors: emptyErrors,\n    projectReady: false,\n    linkErrors: {},\n    linksReady: false,\n    saveComplete: false,\n    saving: false,\n    values: {\n      namespace_id: project.namespace_id,\n      project_type_id: project.project_type_id,\n      name: project.name,\n      slug: project.slug,\n      description: project.description,\n      environments: project.environments\n    },\n    links: originalLinks,\n    urlErrors: {},\n    urls: project.urls,\n    urlsReady: false\n  })\n  const { t } = useTranslation()\n\n  useEffect(() => {\n    const [linksReady, lErrors] = Form.validateURLs(state.links)\n    const linkErrors = Object.fromEntries(\n      lErrors.map((id) => [id, t('common.invalidURL')])\n    )\n    const [urlsReady, uErrors] = Form.validateURLs(state.urls)\n    const urlErrors = Object.fromEntries(\n      uErrors.map((environment) => [environment, t('common.invalidURL')])\n    )\n    const [projectReady, projectErrors] = Form.validateObject(\n      state.values,\n      jsonSchema\n    )\n    setState({\n      ...state,\n      linkErrors: linkErrors,\n      linksReady: linksReady,\n      projectErrors: { ...emptyErrors, ...projectErrors },\n      projectReady: projectReady,\n      urlErrors: urlErrors,\n      urlsReady: urlsReady\n    })\n  }, [state.links, state.urls, state.values])\n\n  useEffect(() => {\n    if (state.saveComplete === true) {\n      onEditFinished(true)\n    }\n  }, [state.saveComplete])\n\n  function onLinkChange(key, value) {\n    const linkKey = parseInt(key.split('-')[1])\n    if (state.links[linkKey] !== value)\n      setState({ ...state, links: { ...state.links, [linkKey]: value } })\n  }\n\n  function onURLChange(key, value) {\n    const urlKey = key.split('-')[1]\n    if (state.urls[urlKey] !== value)\n      setState({ ...state, urls: { ...state.urls, [urlKey]: value } })\n  }\n\n  function onValueChange(key, value) {\n    const values = { ...state.values, [key]: value }\n    if (state.values[key] !== value) {\n      if (key === 'name' && values.slug === '')\n        values.slug = slugify(value).toLowerCase()\n      setState({ ...state, values: values })\n    }\n  }\n\n  async function onSubmit() {\n    setState({ ...state, saving: true })\n    const [projectResult, projectErrorMessage] = await saveProjectChanges(\n      globalState,\n      project,\n      state.values\n    )\n    if (!projectResult) {\n      setState({ ...state, errorMessage: projectErrorMessage, saving: false })\n      return\n    }\n    const [linksResult, linksErrors] = await saveLinkChanges(\n      globalState,\n      project,\n      originalLinks,\n      state.links\n    )\n    if (!linksResult) {\n      console.log(linksErrors)\n      setState({ ...state, errorMessage: 'Error saving links', saving: false })\n      return\n    }\n    const [urlsResult, urlsErrors] = await saveURLChanges(\n      globalState,\n      project,\n      state.values.environments,\n      state.urls\n    )\n    if (!urlsResult) {\n      console.error(urlsErrors)\n      setState({ ...state, errorMessage: 'Error saving URLS', saving: false })\n      return\n    }\n    setState({ ...state, saving: false, saveComplete: true })\n  }\n\n  return (\n    <ErrorBoundary>\n      <Card className=\"flex flex-col h-full\">\n        <h2 className=\"font-medium mb-2\">{t('project.editInfo')}</h2>\n        <Form.SimpleForm\n          errorMessage={state.errorMessage}\n          onCancel={onEditFinished}\n          onSubmit={onSubmit}\n          ready={state.linksReady && state.projectReady && state.urlsReady}\n          saving={state.saving}>\n          <Form.Field\n            title={t('project.namespace')}\n            name=\"namespace_id\"\n            type=\"select\"\n            autoFocus={true}\n            castTo=\"number\"\n            options={asOptions(globalState.metadata.namespaces)}\n            onChange={onValueChange}\n            errorMessage={state.projectErrors.namespace_id}\n            required={true}\n            value={state.values.namespace_id}\n          />\n          <Form.Field\n            title={t('project.projectType')}\n            name=\"project_type_id\"\n            type=\"select\"\n            castTo=\"number\"\n            options={asOptions(globalState.metadata.projectTypes)}\n            onChange={onValueChange}\n            errorMessage={state.projectErrors.project_type_id}\n            required={true}\n            value={state.values.project_type_id}\n          />\n          <Form.Field\n            title={t('project.name')}\n            name=\"name\"\n            type=\"text\"\n            errorMessage={state.projectErrors.name}\n            onChange={onValueChange}\n            required={true}\n            value={state.values.name}\n          />\n          <Form.Field\n            title={t('common.slug')}\n            name=\"slug\"\n            type=\"text\"\n            description={t('common.slugDescription')}\n            errorMessage={state.projectErrors.slug}\n            onChange={onValueChange}\n            required={true}\n            value={state.values.slug}\n          />\n          <Form.Field\n            title={t('common.description')}\n            name=\"description\"\n            description={t('project.descriptionDescription')}\n            type=\"textarea\"\n            onChange={onValueChange}\n            errorMessage={state.projectErrors.description}\n            value={state.values.description}\n          />\n          <Form.Field\n            title={t('project.environments')}\n            name=\"environments\"\n            type=\"select\"\n            multiple={true}\n            options={asOptions(\n              globalState.metadata.environments,\n              'name',\n              'name'\n            )}\n            onChange={onValueChange}\n            errorMessage={state.projectErrors.environments}\n            value={state.values.environments}\n          />\n          {state.values.environments !== null &&\n            state.values.environments.map((environment) => {\n              return (\n                <Form.Field\n                  title={\n                    <Fragment>\n                      <Icon\n                        className=\"mr-2\"\n                        icon={environmentIcons[environment]}\n                      />\n                      {environment} URL\n                    </Fragment>\n                  }\n                  name={`url-${environment}`}\n                  key={`url-${environment}`}\n                  type=\"text\"\n                  errorMessage={state.urlErrors[environment]}\n                  onChange={onURLChange}\n                  value={\n                    state.urls[environment] !== undefined\n                      ? state.urls[environment]\n                      : ''\n                  }\n                />\n              )\n            })}\n          {globalState.metadata.projectLinkTypes.map((linkType) => {\n            return (\n              <Form.Field\n                title={\n                  <Fragment>\n                    <Icon className=\"mr-2\" icon={linkType.icon_class} />\n                    {linkType.link_type} URL\n                  </Fragment>\n                }\n                key={`link-${linkType.id}`}\n                name={`link-${linkType.id}`}\n                type=\"url\"\n                onChange={onLinkChange}\n                errorMessage={state.linkErrors[linkType.id]}\n                value={\n                  state.links[linkType.id] !== undefined\n                    ? state.links[linkType.id]\n                    : ''\n                }\n              />\n            )\n          })}\n        </Form.SimpleForm>\n      </Card>\n    </ErrorBoundary>\n  )\n}\nEdit.propTypes = {\n  project: PropTypes.object.isRequired,\n  onEditFinished: PropTypes.func.isRequired\n}\nexport { Edit }\n",
         "import PropTypes from 'prop-types'\nimport React, { Fragment } from 'react'\n\nimport { Button, Card, Icon } from '../../components'\nimport { useTranslation } from 'react-i18next'\n\nimport { Edit } from './Edit'\n\nfunction Definition({ term, icon, children, className }) {\n  return (\n    <Fragment>\n      <dt className=\"font-medium text-gray-500 w-48\">{term}</dt>\n      <dd\n        className={`mt-1 items-start sm:mt-0 truncate ${\n          className !== undefined ? className : ''\n        }`}>\n        {icon && <Icon icon={icon} className=\"mr-2 \" />}\n        {children}\n      </dd>\n    </Fragment>\n  )\n}\nDefinition.propTypes = {\n  term: PropTypes.string.isRequired,\n  icon: PropTypes.string,\n  children: PropTypes.oneOfType([\n    PropTypes.element,\n    PropTypes.string,\n    PropTypes.arrayOf(PropTypes.element)\n  ]),\n  className: PropTypes.string\n}\n\nfunction Display({ project, onEditClick, shouldGrow }) {\n  const { t } = useTranslation()\n  return (\n    <Card className={`flex flex-col ${shouldGrow ? 'h-full' : ''}`}>\n      <Fragment>\n        <h2 className=\"font-medium mb-2\">{t('terms.projectInfo')}</h2>\n        <dl className=\"lg:ml-4 my-3 space-y-3 overflow-hidden text-gray-900\">\n          <Definition term={t('terms.namespace')} icon={project.namespace_icon}>\n            {project.namespace}\n          </Definition>\n          <Definition term={t('terms.projectType')} icon={project.project_icon}>\n            {project.project_type}\n          </Definition>\n          <Definition term={t('terms.slug')} className=\"font-mono\">\n            {project.slug}\n          </Definition>\n          {project.environments && project.environments.length > 0 && (\n            <Definition term={t('terms.environments')}>\n              {project.environments.join(', ')}\n            </Definition>\n          )}\n          {project.environments &&\n            project.environments.map((environment) => {\n              if (project.urls[environment] === undefined) return null\n              return (\n                <Definition\n                  key={`display-${environment}-url`}\n                  term={`${environment} URL`}>\n                  <a\n                    className=\"text-blue-800 hover:text-blue-700\"\n                    title={project.urls[environment]}\n                    href={project.urls[environment]}\n                    target=\"_new\">\n                    <Icon icon=\"fas external-link-alt\" className=\"mr-2\" />\n                    {project.urls[environment]}{' '}\n                  </a>\n                </Definition>\n              )\n            })}\n          {project.links.map((link, index) => {\n            return (\n              <Definition key={`display-link-${index}`} term={link.title}>\n                <a\n                  className=\"text-blue-800 hover:text-blue-700\"\n                  href={link.url}\n                  title={link.url}\n                  target=\"_new\">\n                  <Icon icon=\"fas external-link-alt\" className=\"mr-2\" />\n                  {link.url}{' '}\n                </a>\n              </Definition>\n            )\n          })}\n        </dl>\n        {project.archived === false && (\n          <div className=\"flex-grow flex flex-row items-end\">\n            <div className=\"flex-grow text-right mt-2\">\n              <Button className=\"btn-white text-xs\" onClick={onEditClick}>\n                <Icon icon=\"fas edit\" className=\"mr-2\" />\n                {t('project.editProject')}\n              </Button>\n            </div>\n          </div>\n        )}\n      </Fragment>\n    </Card>\n  )\n}\nDisplay.propTypes = {\n  project: PropTypes.object.isRequired,\n  onEditClick: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\n\nfunction Details({ project, editing, onEditing, refresh, shouldGrow }) {\n  if (editing)\n    return (\n      <Edit\n        project={project}\n        onEditFinished={(refreshProject) => {\n          onEditing(false)\n          if (refreshProject === true) refresh()\n        }}\n      />\n    )\n  return (\n    <Display\n      project={project}\n      onEditClick={() => onEditing(true)}\n      shouldGrow={shouldGrow}\n    />\n  )\n}\nDetails.propTypes = {\n  project: PropTypes.object.isRequired,\n  editing: PropTypes.bool.isRequired,\n  onEditing: PropTypes.func.isRequired,\n  refresh: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\nexport { Details }\n",
         "import PropTypes from 'prop-types'\nimport React, { useContext, useEffect, useState } from 'react'\nimport { useTranslation } from 'react-i18next'\n\nimport { Card, ErrorBoundary, Form } from '../../components'\nimport { Context } from '../../state'\nimport { httpPost } from '../../utils'\n\nfunction EditFacts({ projectId, facts, factTypes, onEditFinished }) {\n  const [globalState] = useContext(Context)\n  const originalValues = Object.fromEntries(\n    facts.map((fact) => {\n      return [fact.fact_type_id, fact.value]\n    })\n  )\n  const { t } = useTranslation()\n  const [state, setState] = useState({\n    errors: Object.fromEntries(\n      facts.map((fact) => {\n        return [fact.fact_type_id, null]\n      })\n    ),\n    errorMessage: null,\n    facts: Object.fromEntries(\n      facts.map((fact) => {\n        return [fact.fact_type_id, fact.value]\n      })\n    ),\n    ready: false,\n    saving: false\n  })\n\n  useEffect(() => {\n    let ready = false\n    Object.entries(state.facts).forEach((value) => {\n      if (value[1] !== originalValues[value[0]] && ready === false) ready = true\n    })\n    if (state.ready !== ready) setState({ ...state, ready: ready })\n  }, [state.facts])\n\n  function onChange(name, value) {\n    const key = parseInt(name.split('-')[1])\n    if (state.facts[key] !== value)\n      setState({\n        ...state,\n        facts: {\n          ...state.facts,\n          [key]: value !== null ? value.toString() : null\n        }\n      })\n  }\n\n  async function onSubmit() {\n    setState({ ...state, saving: true })\n    const payload = []\n    const url = new URL(`/projects/${projectId}/facts`, globalState.baseURL)\n    for (let [factTypeId, value] of Object.entries(state.facts)) {\n      if (value !== originalValues[factTypeId]) {\n        payload.push({ fact_type_id: Number(factTypeId), value: value })\n      }\n    }\n    if (payload.length > 0) {\n      const result = await httpPost(globalState.fetch, url, payload)\n      if (result.success === false) {\n        console.error(`Error: ${result.data}`)\n      }\n    }\n    onEditFinished(true)\n  }\n\n  return (\n    <ErrorBoundary>\n      <Card className=\"flex flex-col h-full\">\n        <h2 className=\"font-medium mb-2\">{t('project.editFacts')}</h2>\n        <Form.SimpleForm\n          errorMessage={state.errorMessage}\n          onCancel={onEditFinished}\n          onSubmit={onSubmit}\n          ready={state.ready}\n          saving={state.saving}>\n          {factTypes.map((factType) => {\n            let step = undefined\n            let fieldType = 'text'\n            let value = state.facts[factType.id]\n            if (factType.data_type === 'boolean') {\n              fieldType = 'toggle'\n              value = value === 'true'\n            } else if (factType.data_type === 'decimal') {\n              fieldType = 'number'\n              step = '0.01'\n              value = Number(value)\n            } else if (factType.fact_type === 'enum') fieldType = 'select'\n            const name = `fact-${factType.id}`\n            return (\n              <Form.Field\n                key={name}\n                name={name}\n                title={factType.name}\n                type={fieldType}\n                description={factType.description}\n                errorMessage={state.errors[factType.id]}\n                options={\n                  factType.enum_values === null\n                    ? undefined\n                    : factType.enum_values.map((value) => {\n                        return { label: value, value: value }\n                      })\n                }\n                maximum={factType.max_value}\n                minimum={factType.min_value}\n                onChange={onChange}\n                step={step}\n                value={value}\n              />\n            )\n          })}\n        </Form.SimpleForm>\n      </Card>\n    </ErrorBoundary>\n  )\n}\nEditFacts.propTypes = {\n  projectId: PropTypes.number.isRequired,\n  facts: PropTypes.arrayOf(PropTypes.object).isRequired,\n  factTypes: PropTypes.arrayOf(PropTypes.object).isRequired,\n  onEditFinished: PropTypes.func.isRequired\n}\nexport { EditFacts }\n",
-        "import PropTypes from 'prop-types'\nimport React from 'react'\nimport { useTranslation } from 'react-i18next'\n\nimport { Button, Card, Icon, Tooltip } from '../../components'\n\nimport { EditFacts } from './EditFacts'\n\nfunction Fact({ fact, offset }) {\n  const { t } = useTranslation()\n  let color = 'border-gray-300'\n  if (fact.score >= 0) color = 'border-red-600'\n  if (fact.score > 69) color = 'border-yellow-600'\n  if (fact.score > 89) color = 'border-green-600'\n  if (fact.data_type === 'boolean' && fact.value === 'true')\n    color = 'border-green-600'\n\n  return (\n    <div\n      key={`fact-${fact.fact_type_id}`}\n      className={`${\n        offset % 2 === 0 ? 'bg-gray-50' : 'bg-white'\n      } px-2 py-1 flex flex-row sm:px-6 border-l-4 mb-1 text-gray-900 ${color}`}>\n      <dt className=\"font-medium text-gray-500 w-6/12\">{fact.name}</dt>\n      <dd className=\"w-6/12 mt-1 items-start sm:mt-0 truncate\">\n        <Tooltip value={`${t('terms.score')}: ${fact.score}`}>\n          <span className=\"w-6 inline-block text-center\">\n            {fact.value !== null && fact.data_type === 'boolean' && (\n              <Icon\n                className={`${\n                  fact.value === 'true' ? 'text-green-600' : 'text-red-600'\n                }`}\n                icon={`fas ${fact.value === 'true' ? 'check' : 'times-circle'}`}\n              />\n            )}\n            {fact.value !== null &&\n              fact.data_type === 'string' &&\n              fact.fact_type === 'enum' &&\n              fact.icon_class !== null && <Icon icon={fact.icon_class} />}\n          </span>\n          {fact.value !== null && fact.data_type !== 'boolean' && fact.value}\n          {fact.value !== null &&\n          fact.ui_options.includes('display-as-percentage')\n            ? '%'\n            : ''}\n          {fact.value === null && (\n            <span className=\"italic text-red-800 text-xs font-light\">\n              {t('common.notSet')}\n            </span>\n          )}\n        </Tooltip>\n      </dd>\n    </div>\n  )\n}\nFact.propTypes = {\n  fact: PropTypes.object.isRequired,\n  offset: PropTypes.number.isRequired\n}\n\nfunction Display({ project, onEditClick, shouldGrow }) {\n  const { t } = useTranslation()\n  let lastUpdated = 0\n  return (\n    <Card className={`flex flex-col ${shouldGrow ? 'h-full' : ''}`}>\n      <h2 className=\"font-medium mb-2\">{t('project.projectFacts')}</h2>\n      <dl className=\"lg:ml-4 my-3\">\n        {project.facts.map((fact, offset) => {\n          const updated = Date.parse(fact.recorded_at)\n          if (updated > lastUpdated) lastUpdated = updated\n          return (\n            <Fact\n              key={`fact-${fact.fact_type_id}`}\n              fact={fact}\n              offset={offset}\n            />\n          )\n        })}\n      </dl>\n      <div className=\"flex-grow flex flex-row items-end\">\n        <div className=\"flex-grow flex items-center mt-2\">\n          {lastUpdated > 0 && (\n            <div className=\"flex-1 text-xs italic\">\n              {t('common.lastUpdated', {\n                date: new Intl.DateTimeFormat('en-US').format(lastUpdated)\n              })}\n            </div>\n          )}\n          {project.archived === false && (\n            <div className=\"flex-1 text-xs text-right\">\n              <Button onClick={onEditClick}>\n                <Icon icon=\"fas edit\" className=\"mr-2\" />\n                {t('project.updateFacts')}\n              </Button>\n            </div>\n          )}\n        </div>\n      </div>\n    </Card>\n  )\n}\nDisplay.propTypes = {\n  project: PropTypes.object.isRequired,\n  onEditClick: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\n\nfunction Facts({\n  project,\n  factTypes,\n  editing,\n  onEditing,\n  refresh,\n  shouldGrow\n}) {\n  if (editing)\n    return (\n      <EditFacts\n        projectId={project.id}\n        facts={project.facts}\n        factTypes={factTypes}\n        onEditFinished={(refreshProject) => {\n          onEditing(false)\n          if (refreshProject === true) refresh()\n        }}\n      />\n    )\n  return (\n    <Display\n      project={project}\n      shouldGrow={shouldGrow}\n      onEditClick={() => onEditing(true)}\n    />\n  )\n}\nFacts.propTypes = {\n  project: PropTypes.object.isRequired,\n  factTypes: PropTypes.arrayOf(PropTypes.object).isRequired,\n  editing: PropTypes.bool.isRequired,\n  onEditing: PropTypes.func.isRequired,\n  refresh: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\nexport { Facts }\n",
+        "import PropTypes from 'prop-types'\nimport React from 'react'\nimport { useTranslation } from 'react-i18next'\n\nimport { Button, Card, Icon, Tooltip } from '../../components'\n\nimport { EditFacts } from './EditFacts'\n\nfunction Fact({ fact, offset }) {\n  const { t } = useTranslation()\n  let color = 'border-gray-300'\n  if (fact.score > 0) color = 'border-red-600'\n  if (fact.score > 69) color = 'border-yellow-600'\n  if (fact.score > 89) color = 'border-green-600'\n  if (fact.data_type === 'boolean' && fact.value === 'true')\n    color = 'border-green-600'\n  if (fact.data_type === 'boolean' && fact.value === 'false')\n    color = 'border-red-600'\n  return (\n    <div\n      key={`fact-${fact.fact_type_id}`}\n      className={`${\n        offset % 2 === 0 ? 'bg-gray-50' : 'bg-white'\n      } px-2 py-1 flex flex-row sm:px-6 border-l-4 mb-1 text-gray-900 ${color}`}>\n      <dt className=\"font-medium text-gray-500 w-6/12\">{fact.name}</dt>\n      <dd className=\"w-6/12 mt-1 items-start sm:mt-0 truncate\">\n        <Tooltip value={`${t('terms.score')}: ${fact.score}`}>\n          <span className=\"w-6 inline-block text-center\">\n            {fact.value !== null && fact.data_type === 'boolean' && (\n              <Icon\n                className={`${\n                  fact.value === 'true' ? 'text-green-600' : 'text-red-600'\n                }`}\n                icon={`fas ${fact.value === 'true' ? 'check' : 'times-circle'}`}\n              />\n            )}\n            {fact.value !== null &&\n              fact.data_type === 'string' &&\n              fact.fact_type === 'enum' &&\n              fact.icon_class !== null && <Icon icon={fact.icon_class} />}\n          </span>\n          {fact.value !== null && fact.data_type !== 'boolean' && fact.value}\n          {fact.value !== null &&\n          fact.ui_options.includes('display-as-percentage')\n            ? '%'\n            : ''}\n          {fact.value === null && (\n            <span className=\"italic text-red-800 text-xs font-light\">\n              {t('common.notSet')}\n            </span>\n          )}\n        </Tooltip>\n      </dd>\n    </div>\n  )\n}\nFact.propTypes = {\n  fact: PropTypes.object.isRequired,\n  offset: PropTypes.number.isRequired\n}\n\nfunction Display({ project, onEditClick, shouldGrow }) {\n  const { t } = useTranslation()\n  let lastUpdated = 0\n  return (\n    <Card className={`flex flex-col ${shouldGrow ? 'h-full' : ''}`}>\n      <h2 className=\"font-medium mb-2\">{t('project.projectFacts')}</h2>\n      <dl className=\"lg:ml-4 my-3\">\n        {project.facts.map((fact, offset) => {\n          const updated = Date.parse(fact.recorded_at)\n          if (updated > lastUpdated) lastUpdated = updated\n          return (\n            <Fact\n              key={`fact-${fact.fact_type_id}`}\n              fact={fact}\n              offset={offset}\n            />\n          )\n        })}\n      </dl>\n      <div className=\"flex-grow flex flex-row items-end\">\n        <div className=\"flex-grow flex items-center mt-2\">\n          {lastUpdated > 0 && (\n            <div className=\"flex-1 text-xs italic\">\n              {t('common.lastUpdated', {\n                date: new Intl.DateTimeFormat('en-US').format(lastUpdated)\n              })}\n            </div>\n          )}\n          {project.archived === false && (\n            <div className=\"flex-1 text-xs text-right\">\n              <Button onClick={onEditClick}>\n                <Icon icon=\"fas edit\" className=\"mr-2\" />\n                {t('project.updateFacts')}\n              </Button>\n            </div>\n          )}\n        </div>\n      </div>\n    </Card>\n  )\n}\nDisplay.propTypes = {\n  project: PropTypes.object.isRequired,\n  onEditClick: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\n\nfunction Facts({\n  project,\n  factTypes,\n  editing,\n  onEditing,\n  refresh,\n  shouldGrow\n}) {\n  if (editing)\n    return (\n      <EditFacts\n        projectId={project.id}\n        facts={project.facts}\n        factTypes={factTypes}\n        onEditFinished={(refreshProject) => {\n          onEditing(false)\n          if (refreshProject === true) refresh()\n        }}\n      />\n    )\n  return (\n    <Display\n      project={project}\n      shouldGrow={shouldGrow}\n      onEditClick={() => onEditing(true)}\n    />\n  )\n}\nFacts.propTypes = {\n  project: PropTypes.object.isRequired,\n  factTypes: PropTypes.arrayOf(PropTypes.object).isRequired,\n  editing: PropTypes.bool.isRequired,\n  onEditing: PropTypes.func.isRequired,\n  refresh: PropTypes.func.isRequired,\n  shouldGrow: PropTypes.bool.isRequired\n}\nexport { Facts }\n",
         "import PropTypes from 'prop-types'\nimport React, { Fragment, useContext, useEffect, useState } from 'react'\n\nimport { Details } from './Details'\nimport { Facts } from './Facts'\nimport { Context } from '../../state'\n\nfunction Overview({ factTypes, project, refresh, urlPath }) {\n  const [state, dispatch] = useContext(Context)\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        url: new URL(urlPath, state.baseURL),\n        title: project.name\n      }\n    })\n  }, [])\n  const [editing, setEditing] = useState({ details: false, facts: false })\n  return (\n    <Fragment>\n      <div\n        className={`flex flex-col lg:flex-row space-x-0 lg:space-x-3 space-y-3 lg:space-y-0 text-left text-gray-600 ${\n          editing.details === false && editing.facts === false\n            ? 'lg:items-stretch'\n            : ''\n        }`}>\n        <div\n          className={`flex-1 ${\n            factTypes.length > 0 ? 'lg:w-6/12' : ''\n          } w-full ${\n            editing.details === false && editing.facts === false\n              ? 'lg:flex-grow'\n              : ''\n          }`}>\n          <Details\n            project={project}\n            editing={editing.details}\n            refresh={refresh}\n            onEditing={(isEditing) =>\n              setEditing({ ...editing, details: isEditing })\n            }\n            shouldGrow={editing.details === false && editing.facts === false}\n          />\n        </div>\n        {factTypes.length > 0 && (\n          <div\n            className={`flex-1 lg:w-6/12 w-full ${\n              editing.details === false && editing.facts === false\n                ? 'lg:flex-grow'\n                : ''\n            }`}>\n            <Facts\n              project={project}\n              factTypes={factTypes}\n              editing={editing.facts}\n              refresh={refresh}\n              onEditing={(isEditing) =>\n                setEditing({ ...editing, facts: isEditing })\n              }\n              shouldGrow={editing.details === false && editing.facts === false}\n            />\n          </div>\n        )}\n      </div>\n    </Fragment>\n  )\n}\nOverview.propTypes = {\n  factTypes: PropTypes.arrayOf(PropTypes.object).isRequired,\n  project: PropTypes.object.isRequired,\n  refresh: PropTypes.func.isRequired,\n  urlPath: PropTypes.string.isRequired\n}\nexport { Overview }\n",
         "import { compare } from 'fast-json-patch'\nimport PropTypes from 'prop-types'\nimport React, { Fragment, useContext, useEffect, useState } from 'react'\nimport { useHistory } from 'react-router-dom'\n\nimport { Backdrop, Button, Card, ConfirmationDialog } from '../../components'\nimport { Context } from '../../state'\nimport { httpDelete, httpPatch } from '../../utils'\n\nasync function archiveProject(globalState, project) {\n  const originalValues = {\n    archived: project.archived\n  }\n  const values = {\n    archived: true\n  }\n  const patchValue = compare(originalValues, values)\n  if (patchValue.length > 0) {\n    const projectURL = new URL(`/projects/${project.id}`, globalState.baseURL)\n    const result = await httpPatch(globalState.fetch, projectURL, patchValue)\n    if (result.success === false) {\n      return [false, result.data]\n    }\n  }\n  return [true, null]\n}\n\nfunction Settings({ project, refresh, urlPath }) {\n  const [globalState, dispatch] = useContext(Context)\n  const history = useHistory()\n  const [state, setState] = useState({\n    showArchiveConfirmation: false,\n    showBackdrop: false,\n    showDeleteConfirmation: false\n  })\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        title: 'common.settings',\n        url: new URL(`${urlPath}/settings`, globalState.baseURL)\n      }\n    })\n  }, [])\n\n  async function onArchive() {\n    setState({ ...state, showArchiveConfirmation: false, showBackdrop: true })\n    await archiveProject(globalState, project)\n    refresh()\n    history.push(urlPath)\n  }\n\n  async function onDelete() {\n    setState({ ...state, showDeleteConfirmation: false, showBackdrop: true })\n    const projectURL = new URL(`/projects/${project.id}`, globalState.baseURL)\n    const result = await httpDelete(globalState.fetch, projectURL)\n    if (result.success === false) {\n      refresh()\n      return history.push(urlPath)\n    }\n    const url = new URL('/ui/projects/', globalState.baseURL)\n    url.searchParams.append(\n      'message',\n      `${project.name} was successfully deleted.`\n    )\n    history.replace(`${url.pathname}${url.search}`)\n  }\n\n  return (\n    <Fragment>\n      {state.showBackdrop && <Backdrop />}\n      {state.showArchiveConfirmation && (\n        <ConfirmationDialog\n          mode=\"warning\"\n          onCancel={() =>\n            setState({ ...state, showArchiveConfirmation: false })\n          }\n          onConfirm={onArchive}\n          title={`Archive ${project.name}?`}\n          confirmationButtonText={`Archive ${project.name}`}>\n          <div className=\"space-y-4\">\n            <p>Archiving the project will make it entirely read only.</p>\n            <p>\n              It will be hidden from the dashboard, won&rsquo;t show up in\n              searches, and will be disabled as a dependency for any other\n              projects that are dependent upon it.\n            </p>\n            <p className=\"font-semibold\">\n              Are you sure you want to archive this project?\n            </p>\n          </div>\n        </ConfirmationDialog>\n      )}\n      {state.showDeleteConfirmation && (\n        <ConfirmationDialog\n          mode=\"error\"\n          onCancel={() => setState({ ...state, showDeleteConfirmation: false })}\n          onConfirm={onDelete}\n          title={`Delete ${project.name}?`}\n          confirmationButtonText={`Delete ${project.name}`}>\n          <div className=\"space-y-4\">\n            <p>\n              This action will immediately and permanently delete the project,\n              all associated data, including facts, operation logs, and notes.\n            </p>\n            <p className=\"font-semibold\">\n              Are you ABSOLUTELY SURE you wish to delete this project?\n            </p>\n          </div>\n        </ConfirmationDialog>\n      )}\n      <Card className=\"space-y-10\">\n        <div className=\"space-y-3\">\n          <h1 className=\"border-b border-gray-300 font-bold pb-2 text-xl text-yellow-700\">\n            Archive Project\n          </h1>\n          <div className=\"ml-2 space-y-3\">\n            <p>Archiving the project will make it entirely read only.</p>\n            <p className=\"font-semibold\">\n              It will be hidden from the dashboard, won&rsquo;t show up in\n              searches, and will be disabled as a dependency for any other\n              projects that are dependent upon it.\n            </p>\n          </div>\n          <Button\n            className=\"btn-yellow text-sm\"\n            onClick={() => {\n              setState({ ...state, showArchiveConfirmation: true })\n            }}>\n            Archive Project\n          </Button>\n        </div>\n        <div className=\"space-y-3\">\n          <h1 className=\"border-b border-gray-300 font-bold pb-2 text-xl text-red-700\">\n            Delete Project\n          </h1>\n          <div className=\"ml-2 space-y-3\">\n            <p>\n              This action will{' '}\n              <span className=\"font-semibold\">\n                permanently delete{' '}\n                <span className=\"border border-gray-400 font-normal font-mono mx-1 px-1.5 py-1\">\n                  {project.name}\n                </span>{' '}\n                immediately\n              </span>\n              , removing the project and all associated data, including facts,\n              operation logs, and notes.\n            </p>\n            <p className=\"font-semibold\">\n              Are you ABSOLUTELY SURE you wish to delete this project?\n            </p>\n          </div>\n          <Button\n            className=\"btn-red text-sm\"\n            onClick={() => {\n              setState({ ...state, showDeleteConfirmation: true })\n            }}>\n            Delete Project\n          </Button>\n        </div>\n      </Card>\n    </Fragment>\n  )\n}\nSettings.propTypes = {\n  project: PropTypes.object.isRequired,\n  refresh: PropTypes.func.isRequired,\n  urlPath: PropTypes.string.isRequired\n}\nexport { Settings }\n",
         "import PropTypes from 'prop-types'\nimport React, { Fragment, useContext, useEffect, useState } from 'react'\nimport { Route, useParams } from 'react-router-dom'\nimport { useTranslation } from 'react-i18next'\nimport {\n  buildStyles,\n  CircularProgressbarWithChildren\n} from 'react-circular-progressbar'\nimport 'react-circular-progressbar/dist/styles.css'\n\nimport { Context } from '../../state'\nimport { httpRequest, requestOptions, setDocumentTitle } from '../../utils'\nimport {\n  Alert,\n  Error,\n  ErrorBoundary,\n  Icon,\n  IconBar,\n  Loading,\n  Markdown,\n  Tab,\n  Tooltip\n} from '../../components'\n\nimport { Configuration } from './Configuration'\nimport { Dependencies } from './Dependencies'\nimport { FactHistory } from './FactHistory'\nimport { Logs } from './Logs'\nimport { Notes } from './Notes'\nimport { OpsLog } from './OpsLog'\nimport { Overview } from './Overview'\nimport { Settings } from './Settings'\n\nfunction ProjectPage({ project, factTypes, refresh }) {\n  const [state, dispatch] = useContext(Context)\n  const { t } = useTranslation()\n  const baseURL = `/ui/projects/${project.id}`\n  let color = '#cccccc'\n  if (project.project_score >= 0) color = 'red'\n  if (project.project_score > 69) color = 'gold'\n  if (project.project_score > 89) color = '#00c800'\n\n  useEffect(() => {\n    dispatch({\n      type: 'SET_CURRENT_PAGE',\n      payload: {\n        url: new URL(baseURL, state.baseURL.toString()),\n        title: project.name\n      }\n    })\n  }, [])\n\n  return (\n    <ErrorBoundary>\n      <div className=\"flex-auto px-6 py-4 space-y-3\">\n        <div className=\"flex items-center\">\n          <div className=\"flex-1 flex flex-col space-y-2 ml-2\">\n            <h1 className=\"text-gray-600 text-xl\">\n              <Icon icon={project.project_icon} className=\"mr-2\" />\n              {project.name}\n              <span className=\"text-base ml-2\">({project.project_type})</span>\n            </h1>\n            <div className=\"text-gray-500\">\n              {project.links.length === 0 && ' '}\n              {project.links.length > 0 && (\n                <Fragment>\n                  <span className=\"mr-2\">{t('terms.links')}:</span>\n                  <IconBar icons={project.links} />\n                </Fragment>\n              )}\n            </div>\n          </div>\n          {project.archived === true && (\n            <div className=\"flex-1 flex justify-center\">\n              <Alert level=\"warning\" className=\"flex-shrink\">\n                {t('project.archived')}\n              </Alert>\n            </div>\n          )}\n          <div className=\"flex-1 flex justify-end\">\n            <div\n              className=\"flex-shrink mr-2\"\n              style={{ height: '60px', width: '60px' }}>\n              <Tooltip\n                value={t('project.projectHealthScore')}\n                arrowPosition=\"right\">\n                <CircularProgressbarWithChildren\n                  value={project.project_score}\n                  styles={buildStyles({\n                    pathColor: color,\n                    trailColor: '#ccc'\n                  })}>\n                  <div className=\"absolute text-gray-600 font-semibold text-lg\">\n                    {parseInt(project.project_score)}\n                  </div>\n                </CircularProgressbarWithChildren>\n              </Tooltip>\n            </div>\n          </div>\n        </div>\n        <Markdown className=\"mx-2 text-sm text-gray-500\">\n          {project.description}\n        </Markdown>\n        <nav\n          className=\"relative z-0 rounded-lg shadow flex divide-x divide-gray-200\"\n          aria-label=\"Tabs\">\n          <Tab to={baseURL} isFirst={true}>\n            {t('common.overview')}\n          </Tab>\n          <Tab to={`${baseURL}/configuration`}>{t('common.configuration')}</Tab>\n          <Tab to={`${baseURL}/dependencies`}>{t('project.dependencies')}</Tab>\n          <Tab to={`${baseURL}/fact-history`}>{t('project.factHistory')}</Tab>\n          <Tab to={`${baseURL}/logs`}>{t('common.logs')}</Tab>\n          <Tab to={`${baseURL}/notes`}>{t('common.notes')}</Tab>\n          <Tab to={`${baseURL}/operations-log`} isLast={project.archived}>\n            {t('operationsLog.title')}\n          </Tab>\n          {project.archived !== true && (\n            <Tab to={`${baseURL}/settings`} isLast={true} shrink={true}>\n              <Icon icon=\"fas cog\" />\n            </Tab>\n          )}\n        </nav>\n        <Fragment>\n          <Route path={`/ui/projects/${project.id}`} exact>\n            <Overview\n              factTypes={factTypes}\n              project={project}\n              refresh={refresh}\n              urlPath={baseURL}\n            />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/configuration`}>\n            <Configuration urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/dependencies`}>\n            <Dependencies urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/fact-history`}>\n            <FactHistory urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/logs`}>\n            <Logs urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/notes`}>\n            <Notes urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/operations-log`}>\n            <OpsLog urlPath={baseURL} />\n          </Route>\n          <Route path={`/ui/projects/${project.id}/settings`}>\n            <Settings project={project} refresh={refresh} urlPath={baseURL} />\n          </Route>\n        </Fragment>\n      </div>\n    </ErrorBoundary>\n  )\n}\nProjectPage.propTypes = {\n  factTypes: PropTypes.arrayOf(PropTypes.object).isRequired,\n  project: PropTypes.object.isRequired,\n  refresh: PropTypes.func\n}\n\nfunction Project() {\n  const [globalState] = useContext(Context)\n  const { projectId } = useParams()\n  const [state, setState] = useState({\n    errorMessage: null,\n    loading: false,\n    notFound: false,\n    project: null,\n    factTypes: null\n  })\n  const { t } = useTranslation()\n\n  function loadProject() {\n    setState({ ...state, loading: true })\n    const factTypeURL = new URL(\n      `/projects/${projectId}/fact-types`,\n      globalState.baseURL\n    )\n    const projectURL = new URL(`/projects/${projectId}`, globalState.baseURL)\n    projectURL.searchParams.append('full', 'true')\n    Promise.all([\n      httpRequest(globalState.fetch, factTypeURL, requestOptions),\n      httpRequest(globalState.fetch, projectURL, requestOptions)\n    ]).then(([factTypes, project]) => {\n      const newState = { ...state, errorMessage: null }\n      if (factTypes.success) newState.factTypes = factTypes.data\n      else newState.errorMessage = factTypes.data\n      if (project.success) newState.project = project.data\n      else {\n        if (project.status === 404) newState.notFound = true\n        newState.errorMessage = project.data\n      }\n      setState({ ...newState, loading: false })\n      window.scrollTo(0, 0)\n    })\n  }\n\n  useEffect(() => {\n    if (state.project === null) loadProject()\n  }, [projectId, state.project])\n\n  if (state.notFound) {\n    setDocumentTitle(t('common.notFound'))\n    return <Error>{t('error.notFound')}</Error>\n  } else if (state.project === null || state.loading) {\n    setDocumentTitle(t('common.loading'))\n    return <Loading />\n  } else\n    return (\n      <ProjectPage\n        errorMessage={state.errorMessage}\n        factTypes={state.factTypes}\n        project={state.project}\n        refresh={loadProject}\n      />\n    )\n}\nProject.propTypes = {}\nexport { Project }\n",
         "import { Create } from './Create'\nimport { Project as Detail } from './Project'\n\nexport const Project = {\n  Create: Create,\n  Detail: Detail\n}\n",
         "import PropTypes from 'prop-types'\nimport React from 'react'\nimport { useTranslation } from 'react-i18next'\n\nimport { Badge, Paginator, Table } from '../../components'\n\nfunction DataTable({\n  data,\n  disabled,\n  offset,\n  onRowClick,\n  onSortDirection,\n  pageSize,\n  rowCount,\n  setOffset,\n  setPageSize,\n  sort\n}) {\n  const { t } = useTranslation()\n  const columns = [\n    {\n      title: t('terms.namespace'),\n      name: 'namespace',\n      sortCallback: onSortDirection,\n      sortDirection: sort.namespace !== undefined ? sort.namespace : null,\n      type: 'text',\n      tableOptions: {\n        className: 'truncate',\n        headerClassName: 'w-3/12'\n      }\n    },\n    {\n      title: t('terms.name'),\n      name: 'name',\n      sortCallback: onSortDirection,\n      sortDirection: sort.name !== undefined ? sort.name : null,\n      type: 'text',\n      tableOptions: {\n        className: 'truncate',\n        headerClassName: 'w-3/12'\n      }\n    },\n    {\n      title: t('terms.projectType'),\n      name: 'project_type',\n      sortCallback: onSortDirection,\n      sortDirection: sort.project_type !== undefined ? sort.project_type : null,\n      type: 'text',\n      tableOptions: {\n        className: 'truncate',\n        headerClassName: 'w-3/12'\n      }\n    },\n    {\n      title: t('terms.healthScore'),\n      name: 'project_score',\n      sortCallback: onSortDirection,\n      sortDirection:\n        sort.project_score !== undefined ? sort.project_score : null,\n      type: 'text',\n      tableOptions: {\n        className: 'text-center',\n        headerClassName: 'w-2/12 text-center',\n        lookupFunction: (value) => {\n          value = parseInt(value)\n          let color = 'red'\n          if (value === 0) color = 'gray'\n          if (value > 69) color = 'yellow'\n          if (value > 89) color = 'green'\n          return (\n            <Badge className=\"text-sm\" color={color}>\n              {value.toString()}\n            </Badge>\n          )\n        }\n      }\n    }\n  ]\n\n  return (\n    <Paginator.Container\n      currentPage={offset / pageSize + 1}\n      itemCount={rowCount}\n      itemsPerPage={pageSize}\n      setCurrentPage={(currentPage) => {\n        const value = (currentPage - 1) * pageSize\n        setOffset(value)\n      }}\n      setPageSize={setPageSize}>\n      <Table\n        columns={columns}\n        data={data}\n        disabled={disabled}\n        onRowClick={onRowClick}\n      />\n      <Paginator.Controls\n        disabled={disabled}\n        showPageSizeSelector={true}\n        showStateDisplay={true}\n      />\n    </Paginator.Container>\n  )\n}\nDataTable.propTypes = {\n  data: PropTypes.arrayOf(PropTypes.object),\n  disabled: PropTypes.bool,\n  offset: PropTypes.number,\n  onRowClick: PropTypes.func,\n  onSortDirection: PropTypes.func,\n  pageSize: PropTypes.number,\n  rowCount: PropTypes.number,\n  setOffset: PropTypes.func,\n  setPageSize: PropTypes.func,\n  sort: PropTypes.object\n}\nexport { DataTable }\n",
         "export default function _extends() {\n  _extends = Object.assign || function (target) {\n    for (var i = 1; i < arguments.length; i++) {\n      var source = arguments[i];\n\n      for (var key in source) {\n        if (Object.prototype.hasOwnProperty.call(source, key)) {\n          target[key] = source[key];\n        }\n      }\n    }\n\n    return target;\n  };\n\n  return _extends.apply(this, arguments);\n}",
         "/*\n\nBased off glamor's StyleSheet, thanks Sunil \u2764\ufe0f\n\nhigh performance StyleSheet for css-in-js systems\n\n- uses multiple style tags behind the scenes for millions of rules\n- uses `insertRule` for appending in production for *much* faster performance\n\n// usage\n\nimport { StyleSheet } from '@emotion/sheet'\n\nlet styleSheet = new StyleSheet({ key: '', container: document.head })\n\nstyleSheet.insert('#box { border: 1px solid red; }')\n- appends a css rule into the stylesheet\n\nstyleSheet.flush()\n- empties the stylesheet of all its contents\n\n*/\n// $FlowFixMe\nfunction sheetForTag(tag) {\n  if (tag.sheet) {\n    // $FlowFixMe\n    return tag.sheet;\n  } // this weirdness brought to you by firefox\n\n  /* istanbul ignore next */\n\n\n  for (var i = 0; i < document.styleSheets.length; i++) {\n    if (document.styleSheets[i].ownerNode === tag) {\n      // $FlowFixMe\n      return document.styleSheets[i];\n    }\n  }\n}\n\nfunction createStyleElement(options) {\n  var tag = document.createElement('style');\n  tag.setAttribute('data-emotion', options.key);\n\n  if (options.nonce !== undefined) {\n    tag.setAttribute('nonce', options.nonce);\n  }\n\n  tag.appendChild(document.createTextNode(''));\n  tag.setAttribute('data-s', '');\n  return tag;\n}\n\nvar StyleSheet = /*#__PURE__*/function () {\n  function StyleSheet(options) {\n    var _this = this;\n\n    this._insertTag = function (tag) {\n      var before;\n\n      if (_this.tags.length === 0) {\n        before = _this.prepend ? _this.container.firstChild : _this.before;\n      } else {\n        before = _this.tags[_this.tags.length - 1].nextSibling;\n      }\n\n      _this.container.insertBefore(tag, before);\n\n      _this.tags.push(tag);\n    };\n\n    this.isSpeedy = options.speedy === undefined ? process.env.NODE_ENV === 'production' : options.speedy;\n    this.tags = [];\n    this.ctr = 0;\n    this.nonce = options.nonce; // key is the value of the data-emotion attribute, it's used to identify different sheets\n\n    this.key = options.key;\n    this.container = options.container;\n    this.prepend = options.prepend;\n    this.before = null;\n  }\n\n  var _proto = StyleSheet.prototype;\n\n  _proto.hydrate = function hydrate(nodes) {\n    nodes.forEach(this._insertTag);\n  };\n\n  _proto.insert = function insert(rule) {\n    // the max length is how many rules we have per style tag, it's 65000 in speedy mode\n    // it's 1 in dev because we insert source maps that map a single rule to a location\n    // and you can only have one source map per style tag\n    if (this.ctr % (this.isSpeedy ? 65000 : 1) === 0) {\n      this._insertTag(createStyleElement(this));\n    }\n\n    var tag = this.tags[this.tags.length - 1];\n\n    if (process.env.NODE_ENV !== 'production') {\n      var isImportRule = rule.charCodeAt(0) === 64 && rule.charCodeAt(1) === 105;\n\n      if (isImportRule && this._alreadyInsertedOrderInsensitiveRule) {\n        // this would only cause problem in speedy mode\n        // but we don't want enabling speedy to affect the observable behavior\n        // so we report this error at all times\n        console.error(\"You're attempting to insert the following rule:\\n\" + rule + '\\n\\n`@import` rules must be before all other types of rules in a stylesheet but other rules have already been inserted. Please ensure that `@import` rules are before all other rules.');\n      }\n      this._alreadyInsertedOrderInsensitiveRule = this._alreadyInsertedOrderInsensitiveRule || !isImportRule;\n    }\n\n    if (this.isSpeedy) {\n      var sheet = sheetForTag(tag);\n\n      try {\n        // this is the ultrafast version, works across browsers\n        // the big drawback is that the css won't be editable in devtools\n        sheet.insertRule(rule, sheet.cssRules.length);\n      } catch (e) {\n        if (process.env.NODE_ENV !== 'production' && !/:(-moz-placeholder|-ms-input-placeholder|-moz-read-write|-moz-read-only){/.test(rule)) {\n          console.error(\"There was a problem inserting the following rule: \\\"\" + rule + \"\\\"\", e);\n        }\n      }\n    } else {\n      tag.appendChild(document.createTextNode(rule));\n    }\n\n    this.ctr++;\n  };\n\n  _proto.flush = function flush() {\n    // $FlowFixMe\n    this.tags.forEach(function (tag) {\n      return tag.parentNode.removeChild(tag);\n    });\n    this.tags = [];\n    this.ctr = 0;\n\n    if (process.env.NODE_ENV !== 'production') {\n      this._alreadyInsertedOrderInsensitiveRule = false;\n    }\n  };\n\n  return StyleSheet;\n}();\n\nexport { StyleSheet };\n",
```

### Comparing `imbi-0.9.2/imbi/static/redoc.standalone.js` & `imbi-0.9.3/imbi/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/stats.py` & `imbi-0.9.3/imbi/stats.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/templates/base.html` & `imbi-0.9.3/imbi/templates/base.html`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/templates/docs.html` & `imbi-0.9.3/imbi/templates/docs.html`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/templates/error.html` & `imbi-0.9.3/imbi/templates/error.html`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/templates/openapi.yaml` & `imbi-0.9.3/imbi/templates/openapi.yaml`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/timestamp.py` & `imbi-0.9.3/imbi/timestamp.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/transcoders.py` & `imbi-0.9.3/imbi/transcoders.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi/user.py` & `imbi-0.9.3/imbi/user.py`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi.egg-info/PKG-INFO` & `imbi-0.9.3/imbi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbi
-Version: 0.9.2
+Version: 0.9.3
 Summary: Imbi is a DevOps Service Management Platform designed to provide an efficient way to manage a large environment that contains many services and applications.
 Home-page: https://github.com/aweber/imbi
 Author: Gavin M. Roy
 Author-email: gavinr@aweber.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/aweber/imbi/issues
 Project-URL: Documentation, https://imbi.readthedocs.io
```

### Comparing `imbi-0.9.2/imbi.egg-info/SOURCES.txt` & `imbi-0.9.3/imbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/imbi.egg-info/requires.txt` & `imbi-0.9.3/imbi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `imbi-0.9.2/setup.cfg` & `imbi-0.9.3/setup.cfg`

 * *Files identical despite different names*
