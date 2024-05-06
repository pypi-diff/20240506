# Comparing `tmp/lantana-2.9.7.tar.gz` & `tmp/lantana-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantana-2.9.7.tar", last modified: Fri Apr 19 06:46:24 2024, max compression
+gzip compressed data, was "lantana-2.9.8.tar", last modified: Mon May  6 17:34:16 2024, max compression
```

## Comparing `lantana-2.9.7.tar` & `lantana-2.9.8.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.642030 lantana-2.9.7/
--rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.7/LICENCE.md
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2024-04-19 06:46:24.642030 lantana-2.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.618341 lantana-2.9.7/lantana/
--rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.7/lantana/404.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.7/lantana/__init__.py
--rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.7/lantana/__main__.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.7/lantana/after_header.html
--rw-rw-rw-   0        0        0     9493 2024-04-19 06:39:06.000000 lantana-2.9.7/lantana/base.html
--rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.7/lantana/before_header.html
--rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.7/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.627340 lantana-2.9.7/lantana/css/
--rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.7/lantana/css/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.7/lantana/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.7/lantana/css/default.min.css
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.629381 lantana-2.9.7/lantana/css/fonts/
--rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.7/lantana/css/fonts/bootstrap-icons.woff.css
--rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.7/lantana/css/fonts/bootstrap-icons.woff2.css
--rw-rw-rw-   0        0        0     4689 2024-03-18 13:12:54.000000 lantana-2.9.7/lantana/css/theme.css
--rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.7/lantana/css/vs.min.css
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.636968 lantana-2.9.7/lantana/extensions/
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.7/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.7/lantana/extensions/accordion.py
--rw-rw-rw-   0        0        0     2336 2024-03-11 05:59:29.000000 lantana-2.9.7/lantana/extensions/alerts.py
--rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.7/lantana/extensions/cards.py
--rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.7/lantana/extensions/codeblock_copybtn.py
--rw-rw-rw-   0        0        0     1349 2024-03-11 05:55:41.000000 lantana-2.9.7/lantana/extensions/lantana.py
--rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.7/lantana/extensions/link_opennewtab.py
--rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.9.7/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.7/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.7/lantana/extensions/mermaid_precompile.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.7/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.7/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.641000 lantana-2.9.7/lantana/js/
--rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.7/lantana/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.7/lantana/js/highlight.min.js
--rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.7/lantana/js/jquery-3.6.1.slim.min.js
--rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.7/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5560 2024-04-19 06:37:26.000000 lantana-2.9.7/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.7/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.7/lantana/nav.html
--rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.7/lantana/statics.html
--rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.7/lantana/toc.html
-drwxrwxrwx   0        0        0        0 2024-04-19 06:46:24.623341 lantana-2.9.7/lantana.egg-info/
--rw-rw-rw-   0        0        0      237 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 06:46:24.000000 lantana-2.9.7/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 06:46:24.642030 lantana-2.9.7/setup.cfg
--rw-rw-rw-   0        0        0     1716 2024-04-19 06:45:51.000000 lantana-2.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.436375 lantana-2.9.8/
+-rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.8/LICENCE.md
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2024-05-06 17:34:16.436375 lantana-2.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.401375 lantana-2.9.8/lantana/
+-rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.8/lantana/404.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.8/lantana/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.8/lantana/after_header.html
+-rw-rw-rw-   0        0        0     9493 2024-04-19 06:39:06.000000 lantana-2.9.8/lantana/base.html
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.8/lantana/before_header.html
+-rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.8/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.414646 lantana-2.9.8/lantana/css/
+-rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.8/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.8/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.8/lantana/css/default.min.css
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.417171 lantana-2.9.8/lantana/css/fonts/
+-rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.8/lantana/css/fonts/bootstrap-icons.woff.css
+-rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.8/lantana/css/fonts/bootstrap-icons.woff2.css
+-rw-rw-rw-   0        0        0     3949 2024-05-06 12:45:53.000000 lantana-2.9.8/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.8/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.429947 lantana-2.9.8/lantana/extensions/
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.8/lantana/extensions/accordion.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 13:25:21.000000 lantana-2.9.8/lantana/extensions/alerts.py
+-rw-rw-rw-   0        0        0     4704 2024-05-06 17:26:51.000000 lantana-2.9.8/lantana/extensions/alerts2.py
+-rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.8/lantana/extensions/cards.py
+-rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.8/lantana/extensions/codeblock_copybtn.py
+-rw-rw-rw-   0        0        0     1907 2024-05-06 17:26:41.000000 lantana-2.9.8/lantana/extensions/lantana.py
+-rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.8/lantana/extensions/link_opennewtab.py
+-rw-rw-rw-   0        0        0     1996 2024-05-06 10:05:23.000000 lantana-2.9.8/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.8/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.8/lantana/extensions/mermaid_precompile.py
+-rw-rw-rw-   0        0        0     2021 2024-05-06 17:30:11.000000 lantana-2.9.8/lantana/extensions/selector.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.8/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.8/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.435373 lantana-2.9.8/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.8/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.8/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.8/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.8/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5560 2024-04-19 06:37:26.000000 lantana-2.9.8/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.8/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.8/lantana/nav.html
+-rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.8/lantana/statics.html
+-rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.8/lantana/toc.html
+drwxrwxrwx   0        0        0        0 2024-05-06 17:34:16.408392 lantana-2.9.8/lantana.egg-info/
+-rw-rw-rw-   0        0        0      237 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      852 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      275 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 17:34:16.000000 lantana-2.9.8/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:34:16.436375 lantana-2.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1875 2024-05-06 17:33:33.000000 lantana-2.9.8/setup.py
```

### Comparing `lantana-2.9.7/LICENCE.md` & `lantana-2.9.8/LICENCE.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/README.md` & `lantana-2.9.8/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/404.html` & `lantana-2.9.8/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/__main__.py` & `lantana-2.9.8/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/base.html` & `lantana-2.9.8/lantana/base.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/bootstrap-icons.min.css` & `lantana-2.9.8/lantana/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/bootstrap.min.css` & `lantana-2.9.8/lantana/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/default.min.css` & `lantana-2.9.8/lantana/css/default.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/fonts/bootstrap-icons.woff.css` & `lantana-2.9.8/lantana/css/fonts/bootstrap-icons.woff.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/fonts/bootstrap-icons.woff2.css` & `lantana-2.9.8/lantana/css/fonts/bootstrap-icons.woff2.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/css/theme.css` & `lantana-2.9.8/lantana/css/theme.css`

 * *Files 23% similar despite different names*

```diff
@@ -62,20 +62,14 @@
     margin-bottom : 0.5rem;
 }
 
 svg{
     width: 100%;
 }
 
-.alert-heading:before{
-    font-family:bootstrap-icons;
-    padding-right: 0.25em;
-    font-size: 15px;
-}
-
 /*
 .accordion-button:before{
     font-family:bootstrap-icons;
     padding-right: 0.25em;
     font-size: 15px;
 }
 .note .accordion-button:before{
@@ -132,48 +126,14 @@
 .quote .accordion-item
 {
     --bs-accordion-active-bg : var(--bs-light-bg-subtle);
     --bs-accordion-active-color: var(--bs-light-text-emphasis);
     --bs-accordion-btn-focus-box-shadow : 0 0 0 0;
 }
 
-.note .alert-heading:before{
-    content:'\F26A';
-}
-.abstract .alert-heading:before{
-    content:'\F3B8';
-}
-.info .alert-heading:before{
-    content:'\F430';
-}
-.tip .alert-heading:before{
-    content:'\F468';
-}
-.success .alert-heading:before{
-    content:'\F272';
-}
-.question .alert-heading:before{
-    content:'\F504';
-}
-.warning .alert-heading:before{
-    content:'\F33A';
-}
-.failure .alert-heading:before{
-    content:'\F622';
-}
-.danger .alert-heading:before{
-    content:'\F67B';
-}
-.bug .alert-heading:before{
-    content:'\F1DB';
-}
-.example .alert-heading:before{
-    content:'\F41F';
-}
-
 @media print{
     .print-visible{
         display: none;
     }
     .print-hide{
         display: none;
     }
```

### Comparing `lantana-2.9.7/lantana/css/vs.min.css` & `lantana-2.9.8/lantana/css/vs.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/accordion.py` & `lantana-2.9.8/lantana/extensions/accordion.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/alerts.py` & `lantana-2.9.8/lantana/extensions/alerts.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,32 +17,59 @@
 
 def editRawHtml(html):
     soup = BeautifulSoup(html, 'html.parser')
 
     # MaterialのAdmonitionタイトルをAlertタイトルに置換
     replaceClass(soup,'.admonition .admonition-title','admonition-title',['alert-heading'])
 
+    # Alertにアイコンを適用
+    addIcon(soup,'.admonition.note > .alert-heading','bi-check2')
+    addIcon(soup,'.admonition.abstract > .alert-heading','bi-journal-text')
+    addIcon(soup,'.admonition.info > .alert-heading','bi-info-circle')
+    addIcon(soup,'.admonition.important > .alert-heading','bi-exclamation-circle')
+    addIcon(soup,'.admonition.tip > .alert-heading','bi-lightbulb')
+    addIcon(soup,'.admonition.success > .alert-heading','bi-check-all')
+    addIcon(soup,'.admonition.question > .alert-heading','bi-question-circle')
+    addIcon(soup,'.admonition.warning > .alert-heading','bi-exclamation-triangle')
+    addIcon(soup,'.admonition.failure > .alert-heading','bi-window-x')
+    addIcon(soup,'.admonition.danger > .alert-heading','bi-radioactive')
+    addIcon(soup,'.admonition.caution > .alert-heading','bi-exclamation-octagon')
+    addIcon(soup,'.admonition.bug > .alert-heading','bi-bug')
+    addIcon(soup,'.admonition.example > .alert-heading','bi-window-sidebar')
+    addIcon(soup,'.admonition.quote > .alert-heading','bi-chat-right-quote')
+
     # MaterialのAdmonition色をAlert色に置換
     replaceClass(soup,'.admonition.note','admonition',['alert','alert-primary'])
     replaceClass(soup,'.admonition.abstract','admonition',['alert','alert-secondary'])
     replaceClass(soup,'.admonition.info','admonition',['alert','alert-info'])
+    replaceClass(soup,'.admonition.important','admonition',['alert','alert-info'])
     replaceClass(soup,'.admonition.tip','admonition',['alert','alert-warning'])
     replaceClass(soup,'.admonition.success','admonition',['alert','alert-success'])
     replaceClass(soup,'.admonition.question','admonition',['alert','alert-secondary'])
     replaceClass(soup,'.admonition.warning','admonition',['alert','alert-warning'])
     replaceClass(soup,'.admonition.failure','admonition',['alert','alert-danger'])
+    replaceClass(soup,'.admonition.caution','admonition',['alert','alert-danger'])
     replaceClass(soup,'.admonition.danger','admonition',['alert','alert-danger'])
     replaceClass(soup,'.admonition.bug','admonition',['alert','alert-warning'])
     replaceClass(soup,'.admonition.example','admonition',['alert','alert-dark'])
     replaceClass(soup,'.admonition.quote','admonition',['alert','alert-light'])
 
     # Bootstrapのalert-linkを適用
     addClass(soup,'.alert a',['alert-link'])
     return str(soup)
 
+def addIcon(soup,selector,iconPoint):
+    for tag in soup.select(selector):
+            alert_heading_icon_tag = soup.new_tag('i')
+            alert_heading_icon_tag.attrs["class"] = ["bi",iconPoint]
+            if tag.string:
+                tag.string = ' ' + tag.string
+            tag.insert(0,alert_heading_icon_tag)
+
+
 def addClass(soup,selector,ar):
     for tag in soup.select(selector):
         tag.attrs.setdefault('class', list())
         tag["class"] += ar
 
 def replaceClass(soup,selector,remove,add):
     for tag in soup.select(selector):
```

### Comparing `lantana-2.9.7/lantana/extensions/cards.py` & `lantana-2.9.8/lantana/extensions/cards.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/codeblock_copybtn.py` & `lantana-2.9.8/lantana/extensions/codeblock_copybtn.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/link_opennewtab.py` & `lantana-2.9.8/lantana/extensions/link_opennewtab.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/mdx_embedly.py` & `lantana-2.9.8/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/mdx_wsid.py` & `lantana-2.9.8/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/extensions/mermaid_precompile.py` & `lantana-2.9.8/lantana/extensions/mermaid_precompile.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/favicon.png` & `lantana-2.9.8/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/favicon.svg` & `lantana-2.9.8/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/js/bootstrap.bundle.min.js` & `lantana-2.9.8/lantana/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/js/highlight.min.js` & `lantana-2.9.8/lantana/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/js/jquery-3.6.1.slim.min.js` & `lantana-2.9.8/lantana/js/jquery-3.6.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/js/theme.js` & `lantana-2.9.8/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/main.html` & `lantana-2.9.8/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/nav.html` & `lantana-2.9.8/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana/statics.html` & `lantana-2.9.8/lantana/statics.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.7/lantana.egg-info/SOURCES.txt` & `lantana-2.9.8/lantana.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,20 @@
 lantana/css/theme.css
 lantana/css/vs.min.css
 lantana/css/fonts/bootstrap-icons.woff.css
 lantana/css/fonts/bootstrap-icons.woff2.css
 lantana/extensions/__init__.py
 lantana/extensions/accordion.py
 lantana/extensions/alerts.py
+lantana/extensions/alerts2.py
 lantana/extensions/cards.py
 lantana/extensions/codeblock_copybtn.py
 lantana/extensions/lantana.py
 lantana/extensions/link_opennewtab.py
 lantana/extensions/mdx_embedly.py
 lantana/extensions/mdx_wsid.py
 lantana/extensions/mermaid_precompile.py
+lantana/extensions/selector.py
 lantana/js/bootstrap.bundle.min.js
 lantana/js/highlight.min.js
 lantana/js/jquery-3.6.1.slim.min.js
 lantana/js/theme.js
```

### Comparing `lantana-2.9.7/lantana.egg-info/entry_points.txt` & `lantana-2.9.8/lantana.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [console_scripts]
 lantana = lantana.__main__:cli
 
 [markdown.extensions]
 lantana = lantana.extensions.lantana:LantanaExtension
 lantana.accordion = lantana.extensions.accordion:AccordionExtension
 lantana.alerts = lantana.extensions.alerts:AlertsExtension
+lantana.alerts2 = lantana.extensions.alerts2:Alerts2Extension
 lantana.cards = lantana.extensions.cards:CardsExtension
 lantana.codeblock_copybtn = lantana.extensions.codeblock_copybtn:CodeBlockCopyBtnExtension
 lantana.link_opennewtab = lantana.extensions.link_opennewtab:OpenNewTabExtension
 lantana.mermaid_precompile = lantana.extensions.mermaid_precompile:MermaidPrecompileExtension
+lantana.selector = lantana.extensions.selector:SelectorExtension
 mdx_embedly = lantana.extensions.mdx_embedly:EmbedlyExtension
 mdx_wsid = lantana.extensions.mdx_wsid:WSIDExtension
 
 [mkdocs.themes]
 lantana = lantana
```

### Comparing `lantana-2.9.7/setup.py` & `lantana-2.9.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.9.7'
+VERSION = '2.9.8'
 
 setup(
     name="lantana",
     version=VERSION,
     url='https://lantana.wsoft.ws/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
@@ -23,14 +23,16 @@
         ],
         "markdown.extensions": [
             "mdx_wsid = lantana.extensions.mdx_wsid:WSIDExtension",
             "mdx_embedly = lantana.extensions.mdx_embedly:EmbedlyExtension",
             "lantana = lantana.extensions.lantana:LantanaExtension",
             "lantana.cards = lantana.extensions.cards:CardsExtension",
             "lantana.alerts = lantana.extensions.alerts:AlertsExtension",
+            "lantana.alerts2 = lantana.extensions.alerts2:Alerts2Extension",
+            "lantana.selector = lantana.extensions.selector:SelectorExtension",
             "lantana.accordion = lantana.extensions.accordion:AccordionExtension",
             "lantana.link_opennewtab = lantana.extensions.link_opennewtab:OpenNewTabExtension",
             "lantana.codeblock_copybtn = lantana.extensions.codeblock_copybtn:CodeBlockCopyBtnExtension",
             "lantana.mermaid_precompile = lantana.extensions.mermaid_precompile:MermaidPrecompileExtension",
         ]
     },
     zip_safe=False
```

