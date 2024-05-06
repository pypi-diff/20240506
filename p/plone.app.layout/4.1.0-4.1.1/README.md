# Comparing `tmp/plone_app_layout-4.1.0.tar.gz` & `tmp/plone_app_layout-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_app_layout-4.1.0.tar", last modified: Tue Apr 23 16:29:30 2024, max compression
+gzip compressed data, was "plone_app_layout-4.1.1.tar", last modified: Mon May  6 12:51:30 2024, max compression
```

## Comparing `plone_app_layout-4.1.0.tar` & `plone_app_layout-4.1.1.tar`

### file list

```diff
@@ -1,151 +1,147 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.822849 plone_app_layout-4.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    63007 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    65640 2024-04-23 16:29:30.822420 plone_app_layout-4.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      740 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.782891 plone_app_layout-4.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      678 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.783185 plone_app_layout-4.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.785782 plone_app_layout-4.1.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.787436 plone_app_layout-4.1.0/plone/app/layout/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.789005 plone_app_layout-4.1.0/plone/app/layout/analytics/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.789937 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2945 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/analytics.txt
--rw-r--r--   0 maurits    (501) staff       (20)      637 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)      199 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1193 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      234 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view_head.pt
--rw-r--r--   0 maurits    (501) staff       (20)      550 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.790780 plone_app_layout-4.1.0/plone/app/layout/dashboard/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      100 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)      103 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/user_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      885 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/favicon_handler.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.793385 plone_app_layout-4.1.0/plone/app/layout/globals/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1327 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9179 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/context.py
--rw-r--r--   0 maurits    (501) staff       (20)     4098 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     6502 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    12280 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.795316 plone_app_layout-4.1.0/plone/app/layout/globals/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.795672 plone_app_layout-4.1.0/plone/app/layout/globals/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)       30 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10563 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     3885 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     8497 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     6324 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_tools.py
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tools.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.796996 plone_app_layout-4.1.0/plone/app/layout/icons/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1553 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5639 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/icons.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.799051 plone_app_layout-4.1.0/plone/app/layout/links/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/author.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1166 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      284 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/favicon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      178 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/rsslink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      363 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/search.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.800327 plone_app_layout-4.1.0/plone/app/layout/links/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      803 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_canonical_url.py
--rw-r--r--   0 maurits    (501) staff       (20)     2707 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_favicon_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1402 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_rssviewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     7079 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.801965 plone_app_layout-4.1.0/plone/app/layout/navigation/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1749 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    14357 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/navtree.py
--rw-r--r--   0 maurits    (501) staff       (20)      445 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/root.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.803698 plone_app_layout-4.1.0/plone/app/layout/nextprevious/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      989 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      909 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/links.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1673 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/nextprevious.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1611 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      323 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.805206 plone_app_layout-4.1.0/plone/app/layout/sitemap/
--rw-r--r--   0 maurits    (501) staff       (20)      159 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      301 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4491 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)      820 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.805802 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11362 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     1184 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.818010 plone_app_layout-4.1.0/plone/app/layout/viewlets/
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      409 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/anontools.pt
--rw-r--r--   0 maurits    (501) staff       (20)      432 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)    20134 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    10329 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    19042 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     6241 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)      750 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/contentviews.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1239 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2062 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_byline.pt
--rw-r--r--   0 maurits    (501) staff       (20)      980 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_contributors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1833 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_relateditems.pt
--rw-r--r--   0 maurits    (501) staff       (20)      375 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_rights.pt
--rw-r--r--   0 maurits    (501) staff       (20)      139 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/dublin_core.pt
--rw-r--r--   0 maurits    (501) staff       (20)      793 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1579 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.py
--rw-r--r--   0 maurits    (501) staff       (20)      620 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/history_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      953 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/httpheaders.py
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/keywords.pt
--rw-r--r--   0 maurits    (501) staff       (20)      361 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/membertools.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1816 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/menu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      805 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/path_bar.pt
--rw-r--r--   0 maurits    (501) staff       (20)      515 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/popup_content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3320 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/review_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1621 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/searchbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/sections.pt
--rw-r--r--   0 maurits    (501) staff       (20)      552 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/site_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5451 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social_tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)      294 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social_tags_body.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.820686 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      665 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2621 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/history.txt
--rw-r--r--   0 maurits    (501) staff       (20)    27962 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_common.py
--rw-r--r--   0 maurits    (501) staff       (20)    14111 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)      590 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5391 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     5586 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_social.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tiny_logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)       66 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)      382 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toc.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2517 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1779 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.py
--rw-r--r--   0 maurits    (501) staff       (20)       79 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/viewport.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.821146 plone_app_layout-4.1.0/plone.app.layout.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    65640 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4961 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      440 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4284 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-23 16:29:30.822927 plone_app_layout-4.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2264 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.516477 plone_app_layout-4.1.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    63333 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    66001 2024-05-06 12:51:30.516054 plone_app_layout-4.1.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.475042 plone_app_layout-4.1.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.475342 plone_app_layout-4.1.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.478191 plone_app_layout-4.1.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.479756 plone_app_layout-4.1.1/plone/app/layout/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.481278 plone_app_layout-4.1.1/plone/app/layout/analytics/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.482233 plone_app_layout-4.1.1/plone/app/layout/analytics/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2945 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/tests/analytics.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1193 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/analytics/view_head.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      885 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/favicon_handler.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.484966 plone_app_layout-4.1.1/plone/app/layout/globals/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1327 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9179 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4098 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6502 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12280 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3801 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.487362 plone_app_layout-4.1.1/plone/app/layout/globals/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.487639 plone_app_layout-4.1.1/plone/app/layout/globals/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10563 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3885 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8497 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6324 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_tools.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/globals/tools.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.488975 plone_app_layout-4.1.1/plone/app/layout/icons/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/icons/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1553 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/icons/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5639 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/icons/icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/icons/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.491129 plone_app_layout-4.1.1/plone/app/layout/links/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/author.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1166 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      284 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/favicon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      178 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/rsslink.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/search.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.492698 plone_app_layout-4.1.1/plone/app/layout/links/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      803 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/tests/test_canonical_url.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2707 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/tests/test_favicon_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1402 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/tests/test_rssviewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7079 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/links/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.494458 plone_app_layout-4.1.1/plone/app/layout/navigation/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/navigation/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/navigation/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1749 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/navigation/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14357 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/navigation/navtree.py
+-rw-r--r--   0 maurits    (501) staff       (20)      445 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/navigation/root.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.496488 plone_app_layout-4.1.1/plone/app/layout/nextprevious/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      989 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/links.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1673 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/nextprevious.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1613 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/nextprevious/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      323 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.498137 plone_app_layout-4.1.1/plone/app/layout/sitemap/
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4491 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/sitemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.499020 plone_app_layout-4.1.1/plone/app/layout/sitemap/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11362 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/sitemap/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1184 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.511596 plone_app_layout-4.1.1/plone/app/layout/viewlets/
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/anontools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      432 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    20131 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10329 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    19042 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6241 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/contentviews.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/default_page_warning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1239 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/document_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2062 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/document_byline.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/document_contributors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1833 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/document_relateditems.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      375 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/document_rights.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/dublin_core.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/globalstatusmessage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1579 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/globalstatusmessage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      620 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/history_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      953 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/httpheaders.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/keywords.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      361 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/membertools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1816 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/menu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      805 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/path_bar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      515 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/popup_content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3320 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/review_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1621 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/searchbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/sections.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      552 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/site_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5451 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/social.py
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/social_tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/social_tags_body.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.514325 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      665 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2621 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/history.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    27962 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14111 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      590 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5391 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_social.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/tiny_logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       66 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      382 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/toc.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2517 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/toolbar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1779 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/toolbar.py
+-rw-r--r--   0 maurits    (501) staff       (20)       79 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/plone/app/layout/viewlets/viewport.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:51:30.514869 plone_app_layout-4.1.1/plone.app.layout.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    66001 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4839 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:51:30.000000 plone_app_layout-4.1.1/plone.app.layout.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4284 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:51:30.516553 plone_app_layout-4.1.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2024-05-06 12:51:29.000000 plone_app_layout-4.1.1/setup.py
```

### Comparing `plone_app_layout-4.1.0/CHANGES.rst` & `plone_app_layout-4.1.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.1 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Less DeprecationWarnings by using `plone.base.navigationroot.*` [@jensens] (#364)
+- Less DeprecationWarnings by using `plone.app.dexterity.behaviors.nextprevious.*` [@jensens] (#365)
+- Remove long outdated (Plone 5) deprecation `moved` for `dashboard` [@jensens] (#366)
+
+
 4.1.0 (2024-04-23)
 ------------------
 
 New features:
 
 
 - Add a field ``webstats_head_js`` to the Site controlpanel and render its
```

### Comparing `plone_app_layout-4.1.0/PKG-INFO` & `plone_app_layout-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.1.0
+Version: 4.1.1
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.content
+Requires-Dist: plone.app.dexterity
 Requires-Dist: plone.app.relationfield
 Requires-Dist: plone.app.uuid
 Requires-Dist: plone.app.viewletmanager>=1.2
 Requires-Dist: plone.base>=1.0.4
 Requires-Dist: plone.dexterity
 Requires-Dist: plone.formwidget.namedfile
 Requires-Dist: plone.i18n
@@ -74,14 +75,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.1 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Less DeprecationWarnings by using `plone.base.navigationroot.*` [@jensens] (#364)
+- Less DeprecationWarnings by using `plone.app.dexterity.behaviors.nextprevious.*` [@jensens] (#365)
+- Remove long outdated (Plone 5) deprecation `moved` for `dashboard` [@jensens] (#366)
+
+
 4.1.0 (2024-04-23)
 ------------------
 
 New features:
 
 
 - Add a field ``webstats_head_js`` to the Site controlpanel and render its
```

### Comparing `plone_app_layout-4.1.0/README.rst` & `plone_app_layout-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/docs/LICENSE.GPL` & `plone_app_layout-4.1.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/docs/LICENSE.txt` & `plone_app_layout-4.1.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/analytics/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/analytics/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/analytics/tests/analytics.txt` & `plone_app_layout-4.1.1/plone/app/layout/analytics/tests/analytics.txt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/analytics/tests/test_doctests.py` & `plone_app_layout-4.1.1/plone/app/layout/analytics/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/analytics/view.py` & `plone_app_layout-4.1.1/plone/app/layout/analytics/view.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/favicon_handler.py` & `plone_app_layout-4.1.1/plone/app/layout/favicon_handler.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/globals/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/context.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/context.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/interface.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/interface.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/interfaces.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/layout.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/layout.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/portal.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/portal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .interfaces import IPortalState
 from Acquisition import aq_inner
-from plone.app.layout.navigation.root import getNavigationRoot
-from plone.app.layout.navigation.root import getNavigationRootObject
 from plone.base.interfaces import IPloneSiteRoot
 from plone.base.interfaces import ISearchSchema
 from plone.base.interfaces import ISiteSchema
+from plone.base.navigationroot import get_navigation_root
+from plone.base.navigationroot import get_navigation_root_object
 from plone.i18n.interfaces import ILanguageSchema
 from plone.memoize.view import memoize
 from plone.memoize.view import memoize_contextless
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.CMFCore.utils import getToolByName
 from Products.Five.browser import BrowserView
@@ -44,15 +44,15 @@
     def portal_url(self):
         return self.portal().absolute_url()
 
     @memoize
     def navigation_root(self):
         context = aq_inner(self.context)
         portal = self.portal()
-        return getNavigationRootObject(context, portal)
+        return get_navigation_root_object(context, portal)
 
     @memoize
     def navigation_root_title(self):
         navigation_root = self.navigation_root()
         if IPloneSiteRoot.providedBy(navigation_root):
             return self.portal_title()
 
@@ -60,15 +60,15 @@
         if callable(title):
             return title()
         else:
             return title
 
     @memoize
     def navigation_root_path(self):
-        return getNavigationRoot(aq_inner(self.context))
+        return get_navigation_root(aq_inner(self.context))
 
     @memoize
     def navigation_root_url(self):
         rootPath = self.navigation_root_path()
         return self.request.physicalPathToURL(rootPath)
 
     @memoize_contextless
```

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_context.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_interface.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_layout.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_portal.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_tools.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/globals/tools.py` & `plone_app_layout-4.1.1/plone/app/layout/globals/tools.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/icons/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/icons/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/icons/icons.py` & `plone_app_layout-4.1.1/plone/app/layout/icons/icons.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/icons/interfaces.py` & `plone_app_layout-4.1.1/plone/app/layout/icons/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/author.pt` & `plone_app_layout-4.1.1/plone/app/layout/links/author.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_canonical_url.py` & `plone_app_layout-4.1.1/plone/app/layout/links/tests/test_canonical_url.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_favicon_viewlet.py` & `plone_app_layout-4.1.1/plone/app/layout/links/tests/test_favicon_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_rssviewlet.py` & `plone_app_layout-4.1.1/plone/app/layout/links/tests/test_rssviewlet.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/links/viewlets.py` & `plone_app_layout-4.1.1/plone/app/layout/links/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/navigation/interfaces.py` & `plone_app_layout-4.1.1/plone/app/layout/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/navigation/navtree.py` & `plone_app_layout-4.1.1/plone/app/layout/navigation/navtree.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/nextprevious/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/nextprevious/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/nextprevious/links.pt` & `plone_app_layout-4.1.1/plone/app/layout/nextprevious/links.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/nextprevious/nextprevious.pt` & `plone_app_layout-4.1.1/plone/app/layout/nextprevious/nextprevious.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/nextprevious/view.py` & `plone_app_layout-4.1.1/plone/app/layout/nextprevious/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from Acquisition import aq_inner
 from Acquisition import aq_parent
-from plone.app.layout.nextprevious.interfaces import INextPreviousProvider
+from plone.app.dexterity.behaviors.nextprevious import INextPreviousProvider
 from plone.app.layout.viewlets import ViewletBase
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ZopeTwoPageTemplateFile
 from zope.component import getMultiAdapter
 
 
 class NextPreviousView(BrowserView):
```

### Comparing `plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.py` & `plone_app_layout-4.1.1/plone/app/layout/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.xml` & `plone_app_layout-4.1.1/plone/app/layout/sitemap/sitemap.xml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/test_sitemap.py` & `plone_app_layout-4.1.1/plone/app/layout/sitemap/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/testing.py` & `plone_app_layout-4.1.1/plone/app/layout/testing.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/common.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from AccessControl import getSecurityManager
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from collections import defaultdict
 from functools import total_ordering
 from html import escape
 from plone.app.layout.globals.interfaces import IViewView
-from plone.app.layout.navigation.root import getNavigationRoot
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import IPloneSiteRoot
 from plone.base.interfaces import ISearchSchema
 from plone.base.interfaces import ISiteSchema
 from plone.base.interfaces.controlpanel import INavigationSchema
+from plone.base.navigationroot import get_navigation_root
 from plone.base.utils import safe_text
 from plone.i18n.interfaces import ILanguageSchema
 from plone.memoize.view import memoize
 from plone.protect.utils import addTokenToUrl
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.utils import getSiteLogo
@@ -230,15 +230,15 @@
 
     @property
     def language_settings(self):
         return self.registry.forInterface(ILanguageSchema, prefix="plone")
 
     @property
     def navtree_path(self):
-        return getNavigationRoot(self.context)
+        return get_navigation_root(self.context)
 
     @property
     def current_language(self):
         language_settings = self.registry.forInterface(ILanguageSchema, prefix="plone")
         return (
             self.request.get("LANGUAGE", None)
             or (self.context and aq_inner(self.context).Language())
```

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/configure.zcml` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/content.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/content.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/content_history.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/content_history.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/contentviews.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/contentviews.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/default_page_warning.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_actions.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/document_actions.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_byline.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/document_byline.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_contributors.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/document_contributors.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_relateditems.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/document_relateditems.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/globalstatusmessage.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/globalstatusmessage.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/history_view.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/history_view.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/httpheaders.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/httpheaders.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/interfaces.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/keywords.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/keywords.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/membertools.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/membertools.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/menu.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/menu.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/path_bar.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/path_bar.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/popup_content_history.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/popup_content_history.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/review_history.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/review_history.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/searchbox.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/searchbox.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/sections.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/sections.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/site_actions.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/site_actions.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/social.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/social.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/base.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/history.txt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/history.txt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_common.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_content.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_functional.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_history.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_social.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.pt` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/toolbar.pt`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.py` & `plone_app_layout-4.1.1/plone/app/layout/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/plone.app.layout.egg-info/PKG-INFO` & `plone_app_layout-4.1.1/plone.app.layout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.1.0
+Version: 4.1.1
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.content
+Requires-Dist: plone.app.dexterity
 Requires-Dist: plone.app.relationfield
 Requires-Dist: plone.app.uuid
 Requires-Dist: plone.app.viewletmanager>=1.2
 Requires-Dist: plone.base>=1.0.4
 Requires-Dist: plone.dexterity
 Requires-Dist: plone.formwidget.namedfile
 Requires-Dist: plone.i18n
@@ -74,14 +75,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.1 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Less DeprecationWarnings by using `plone.base.navigationroot.*` [@jensens] (#364)
+- Less DeprecationWarnings by using `plone.app.dexterity.behaviors.nextprevious.*` [@jensens] (#365)
+- Remove long outdated (Plone 5) deprecation `moved` for `dashboard` [@jensens] (#366)
+
+
 4.1.0 (2024-04-23)
 ------------------
 
 New features:
 
 
 - Add a field ``webstats_head_js`` to the Site controlpanel and render its
```

### Comparing `plone_app_layout-4.1.0/plone.app.layout.egg-info/SOURCES.txt` & `plone_app_layout-4.1.1/plone.app.layout.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 plone/app/layout/analytics/configure.zcml
 plone/app/layout/analytics/view.pt
 plone/app/layout/analytics/view.py
 plone/app/layout/analytics/view_head.pt
 plone/app/layout/analytics/tests/__init__.py
 plone/app/layout/analytics/tests/analytics.txt
 plone/app/layout/analytics/tests/test_doctests.py
-plone/app/layout/dashboard/__init__.py
-plone/app/layout/dashboard/dashboard.py
-plone/app/layout/dashboard/user_actions.py
 plone/app/layout/globals/__init__.py
 plone/app/layout/globals/configure.zcml
 plone/app/layout/globals/context.py
 plone/app/layout/globals/interface.py
 plone/app/layout/globals/interfaces.py
 plone/app/layout/globals/layout.py
 plone/app/layout/globals/portal.py
```

### Comparing `plone_app_layout-4.1.0/pyproject.toml` & `plone_app_layout-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone_app_layout-4.1.0/setup.py` & `plone_app_layout-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.1.0"
+version = "4.1.1"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.app.layout",
@@ -40,14 +40,15 @@
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "plone.app.content",
+        "plone.app.dexterity",
         "plone.app.relationfield",
         "plone.app.uuid",
         "plone.app.viewletmanager >=1.2",
         "plone.base >=1.0.4",
         "plone.dexterity",
         "plone.formwidget.namedfile",
         "plone.i18n",
```

