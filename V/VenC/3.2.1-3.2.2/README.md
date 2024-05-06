# Comparing `tmp/VenC-3.2.1.tar.gz` & `tmp/VenC-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VenC-3.2.1.tar", last modified: Mon Apr 22 21:04:40 2024, max compression
+gzip compressed data, was "VenC-3.2.2.tar", last modified: Mon May  6 14:57:00 2024, max compression
```

## Comparing `VenC-3.2.1.tar` & `VenC-3.2.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/
--rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-04-22 21:04:40.970235 VenC-3.2.1/PKG-INFO
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/VenC.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-04-22 21:04:40.000000 VenC-3.2.1/VenC.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     2489 2024-04-22 21:04:40.000000 VenC-3.2.1/VenC.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-04-22 21:04:40.000000 VenC-3.2.1/VenC.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       17 2024-04-22 21:04:40.000000 VenC-3.2.1/VenC.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        6 2024-04-22 21:04:40.000000 VenC-3.2.1/VenC.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2024-04-22 21:04:40.970235 VenC-3.2.1/setup.cfg
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3163 2024-04-22 20:56:42.000000 VenC-3.2.1/setup.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.962235 VenC-3.2.1/share/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/embed_providers/
--rw-rw-r--   0 denis     (1000) denis     (1000)   123306 2023-12-19 14:41:00.000000 VenC-3.2.1/share/embed_providers/oembed.json
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.962235 VenC-3.2.1/share/themes/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/themes/concrete/
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/themes/concrete/assets/
--rw-rw-r--   0 denis     (1000) denis     (1000)     5109 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/assets/style.css
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/themes/concrete/chunks/
--rw-rw-r--   0 denis     (1000) denis     (1000)      356 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/atomEntry.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)        8 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/atomFooter.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      706 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/chunks/atomHeader.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      105 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/audio.html
--rw-rw-r--   0 denis     (1000) denis     (1000)     1810 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/chunks/entry.html
--rw-rw-r--   0 denis     (1000) denis     (1000)     1208 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/chunks/footer.html
--rw-rw-r--   0 denis     (1000) denis     (1000)     6088 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/chunks/header.html
--rw-rw-r--   0 denis     (1000) denis     (1000)      318 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/rssEntry.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/rssFooter.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      256 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/rssHeader.xml
--rw-rw-r--   0 denis     (1000) denis     (1000)      119 2024-02-17 16:56:20.000000 VenC-3.2.1/share/themes/concrete/chunks/video.html
--rw-rw-r--   0 denis     (1000) denis     (1000)      233 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes/concrete/config.yaml
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/themes_assets/
--rw-rw-r--   0 denis     (1000) denis     (1000)     6552 2023-12-19 14:41:00.000000 VenC-3.2.1/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)      951 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)     5436 2024-02-18 15:13:05.000000 VenC-3.2.1/share/themes_assets/VenC-Tree-0.2.0.js
--rw-rw-r--   0 denis     (1000) denis     (1000)    97152 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes_assets/concrete-dark.png
--rw-rw-r--   0 denis     (1000) denis     (1000)    64283 2024-04-21 10:17:35.000000 VenC-3.2.1/share/themes_assets/concrete.png
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/share/themes_templates/
--rw-rw-r--   0 denis     (1000) denis     (1000)      188 2023-12-19 14:41:00.000000 VenC-3.2.1/share/themes_templates/images
--rw-rw-r--   0 denis     (1000) denis     (1000)      138 2023-12-19 14:41:00.000000 VenC-3.2.1/share/themes_templates/kroki
--rw-rw-r--   0 denis     (1000) denis     (1000)      132 2023-12-19 14:41:00.000000 VenC-3.2.1/share/themes_templates/oEmbed
--rw-rw-r--   0 denis     (1000) denis     (1000)      151 2023-12-19 14:41:00.000000 VenC-3.2.1/share/themes_templates/pygmentize
--rwxrwxr-x   0 denis     (1000) denis     (1000)     2992 2023-12-19 14:41:00.000000 VenC-3.2.1/venc
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/venc3/
--rw-rw-r--   0 denis     (1000) denis     (1000)      799 2024-04-22 20:57:52.000000 VenC-3.2.1/venc3/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.966235 VenC-3.2.1/venc3/commands/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/commands/__init__.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)    10723 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/commands/export.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     1815 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/commands/install.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     7094 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/commands/new.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     4459 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/commands/print.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     9275 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/commands/remote.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4195 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/commands/serv.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/datastore/
--rw-rw-r--   0 denis     (1000) denis     (1000)     9560 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2515 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/archives.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     6612 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/configuration.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4116 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/entries.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     6920 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/entry.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1346 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/datastore/hardcoded_assets.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     1675 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/datastore/metadata.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4838 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/datastore/taxonomy.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     5487 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/datastore/theme.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     6619 2024-04-11 16:07:13.000000 VenC-3.2.1/venc3/exceptions.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     5027 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/helpers.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/l10n/
--rw-rw-r--   0 denis     (1000) denis     (1000)     1529 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/l10n/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     8277 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/l10n/en.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     9225 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/l10n/fr.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/markup_languages/
--rw-rw-r--   0 denis     (1000) denis     (1000)     2808 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/markup_languages/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1641 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/markup_languages/asciidoc.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2019 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/markup_languages/markdown.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1644 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/markup_languages/restructuredtext.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/parallelism/
--rw-rw-r--   0 denis     (1000) denis     (1000)     2443 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/parallelism/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2702 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/parallelism/build_entries.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5405 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/parallelism/export_entries.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    33331 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/patterns/datastore.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4645 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/patterns/non_contextual.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    11160 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/patterns/patterns_map.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)    12375 2024-03-08 02:35:29.000000 VenC-3.2.1/venc3/patterns/processor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1537 2024-04-22 20:41:30.000000 VenC-3.2.1/venc3/patterns/theme.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2611 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/kroki.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1232 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/latex2mathml.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3783 2024-02-11 16:20:57.000000 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/oembed.py
--rwxrwxr-x   0 denis     (1000) denis     (1000)     3256 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/patterns/third_party_wrapped_features/pygmentize.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1975 2024-04-04 17:42:26.000000 VenC-3.2.1/venc3/prompt.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-04-22 21:04:40.970235 VenC-3.2.1/venc3/threads/
--rw-rw-r--   0 denis     (1000) denis     (1000)    14843 2024-04-22 20:47:34.000000 VenC-3.2.1/venc3/threads/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2703 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/archives.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4745 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/categories.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     6225 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/chapters.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     6309 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/entries.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2136 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/feed.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2707 2024-04-21 10:17:35.000000 VenC-3.2.1/venc3/threads/main.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.967995 VenC-3.2.2/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-05-06 14:57:00.967995 VenC-3.2.2/PKG-INFO
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/VenC.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      451 2024-05-06 14:57:00.000000 VenC-3.2.2/VenC.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2489 2024-05-06 14:57:00.000000 VenC-3.2.2/VenC.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-05-06 14:57:00.000000 VenC-3.2.2/VenC.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       17 2024-05-06 14:57:00.000000 VenC-3.2.2/VenC.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        6 2024-05-06 14:57:00.000000 VenC-3.2.2/VenC.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2024-05-06 14:57:00.967995 VenC-3.2.2/setup.cfg
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3163 2024-05-06 14:48:26.000000 VenC-3.2.2/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/share/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/share/embed_providers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)   123306 2023-12-19 14:41:00.000000 VenC-3.2.2/share/embed_providers/oembed.json
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/share/themes/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/share/themes/concrete/
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.959994 VenC-3.2.2/share/themes/concrete/assets/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5109 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/assets/style.css
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/share/themes/concrete/chunks/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      356 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/atomEntry.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)        8 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/atomFooter.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      706 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/chunks/atomHeader.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      105 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/audio.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1810 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/chunks/entry.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1208 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/chunks/footer.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6088 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/chunks/header.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)      318 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/rssEntry.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/rssFooter.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      256 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/rssHeader.xml
+-rw-rw-r--   0 denis     (1000) denis     (1000)      119 2024-02-17 16:56:20.000000 VenC-3.2.2/share/themes/concrete/chunks/video.html
+-rw-rw-r--   0 denis     (1000) denis     (1000)      233 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes/concrete/config.yaml
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/share/themes_assets/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6552 2023-12-19 14:41:00.000000 VenC-3.2.2/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)      951 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5436 2024-02-18 15:13:05.000000 VenC-3.2.2/share/themes_assets/VenC-Tree-0.2.0.js
+-rw-rw-r--   0 denis     (1000) denis     (1000)    97152 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes_assets/concrete-dark.png
+-rw-rw-r--   0 denis     (1000) denis     (1000)    64283 2024-04-21 10:17:35.000000 VenC-3.2.2/share/themes_assets/concrete.png
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/share/themes_templates/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      188 2023-12-19 14:41:00.000000 VenC-3.2.2/share/themes_templates/images
+-rw-rw-r--   0 denis     (1000) denis     (1000)      138 2023-12-19 14:41:00.000000 VenC-3.2.2/share/themes_templates/kroki
+-rw-rw-r--   0 denis     (1000) denis     (1000)      132 2023-12-19 14:41:00.000000 VenC-3.2.2/share/themes_templates/oEmbed
+-rw-rw-r--   0 denis     (1000) denis     (1000)      151 2023-12-19 14:41:00.000000 VenC-3.2.2/share/themes_templates/pygmentize
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     2992 2023-12-19 14:41:00.000000 VenC-3.2.2/venc
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      799 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/commands/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/commands/__init__.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)    10723 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/commands/export.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     1815 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/commands/install.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     7094 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/commands/new.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     4459 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/commands/print.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     9275 2024-05-05 12:12:37.000000 VenC-3.2.2/venc3/commands/remote.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5309 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/commands/serv.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/datastore/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9560 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/datastore/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2515 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/datastore/archives.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     6612 2024-05-05 12:12:37.000000 VenC-3.2.2/venc3/datastore/configuration.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4116 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/datastore/entries.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     6920 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/datastore/entry.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1346 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/datastore/hardcoded_assets.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     1675 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/datastore/metadata.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4838 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/datastore/taxonomy.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     5487 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/datastore/theme.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6619 2024-04-11 16:07:13.000000 VenC-3.2.2/venc3/exceptions.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     5027 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/helpers.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/l10n/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1529 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/l10n/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     8316 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/l10n/en.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     9270 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/l10n/fr.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/markup_languages/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2808 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/markup_languages/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1641 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/markup_languages/asciidoc.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2019 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/markup_languages/markdown.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1644 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/markup_languages/restructuredtext.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/parallelism/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2443 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/parallelism/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2702 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/parallelism/build_entries.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5405 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/parallelism/export_entries.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.963994 VenC-3.2.2/venc3/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    33331 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/patterns/datastore.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4645 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/patterns/non_contextual.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    11160 2024-05-05 12:12:37.000000 VenC-3.2.2/venc3/patterns/patterns_map.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)    12375 2024-03-08 02:35:29.000000 VenC-3.2.2/venc3/patterns/processor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1537 2024-04-22 20:41:30.000000 VenC-3.2.2/venc3/patterns/theme.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.967995 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2611 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/kroki.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1232 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/latex2mathml.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3783 2024-02-11 16:20:57.000000 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/oembed.py
+-rwxrwxr-x   0 denis     (1000) denis     (1000)     3256 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/patterns/third_party_wrapped_features/pygmentize.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1975 2024-04-04 17:42:26.000000 VenC-3.2.2/venc3/prompt.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2024-05-06 14:57:00.967995 VenC-3.2.2/venc3/threads/
+-rw-rw-r--   0 denis     (1000) denis     (1000)    14839 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/threads/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2703 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/threads/archives.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4745 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/threads/categories.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6225 2024-04-21 10:17:35.000000 VenC-3.2.2/venc3/threads/chapters.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     6575 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/threads/entries.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1922 2024-05-06 14:48:26.000000 VenC-3.2.2/venc3/threads/feed.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2707 2024-05-05 12:12:37.000000 VenC-3.2.2/venc3/threads/main.py
```

### Comparing `VenC-3.2.1/VenC.egg-info/SOURCES.txt` & `VenC-3.2.2/VenC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/setup.py` & `VenC-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         dst_prefix+"share/VenC/themes_templates/",
         ["share/themes_templates/"+filename for filename in listdir("share/themes_templates")]
     )
 )
 
 setup(
     name='VenC',
-    version='3.2.1',
+    version='3.2.2',
     description='A static blog generator.',
     author='Denis Salem',
     author_email='denissalem@tuxfamily.org',
     url='https://github.com/DenisSalem/VenC',
     packages=[
         'venc3',
         'venc3.commands',
```

### Comparing `VenC-3.2.1/share/embed_providers/oembed.json` & `VenC-3.2.2/share/embed_providers/oembed.json`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes/concrete/assets/style.css` & `VenC-3.2.2/share/themes/concrete/assets/style.css`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes/concrete/chunks/atomHeader.xml` & `VenC-3.2.2/share/themes/concrete/chunks/atomHeader.xml`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes/concrete/chunks/entry.html` & `VenC-3.2.2/share/themes/concrete/chunks/entry.html`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes/concrete/chunks/footer.html` & `VenC-3.2.2/share/themes/concrete/chunks/footer.html`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes/concrete/chunks/header.html` & `VenC-3.2.2/share/themes/concrete/chunks/header.html`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js` & `VenC-3.2.2/share/themes_assets/VenC-Infinite-Scroll-1.2.0.js`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js` & `VenC-3.2.2/share/themes_assets/VenC-Scripts-Bootstrap-0.0.0.js`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes_assets/VenC-Tree-0.2.0.js` & `VenC-3.2.2/share/themes_assets/VenC-Tree-0.2.0.js`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes_assets/concrete-dark.png` & `VenC-3.2.2/share/themes_assets/concrete-dark.png`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/share/themes_assets/concrete.png` & `VenC-3.2.2/share/themes_assets/concrete.png`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc` & `VenC-3.2.2/venc`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/__init__.py` & `VenC-3.2.2/venc3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with VenC.  If not, see <http://www.gnu.org/licenses/>.
 
-venc_version = "3.2.1"
+venc_version = "3.2.2"
 __version__ = venc_version # PEP396
```

### Comparing `VenC-3.2.1/venc3/commands/export.py` & `VenC-3.2.2/venc3/commands/export.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/commands/install.py` & `VenC-3.2.2/venc3/commands/install.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/commands/new.py` & `VenC-3.2.2/venc3/commands/new.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/commands/print.py` & `VenC-3.2.2/venc3/commands/print.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/commands/remote.py` & `VenC-3.2.2/venc3/commands/remote.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/commands/serv.py` & `VenC-3.2.2/venc3/commands/serv.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,62 +16,95 @@
 #
 #    You should have received a copy of the GNU General Public License
 #    along with VenC.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import http.server
 from multiprocessing import Process
+import shutil
 import time
 import urllib.parse 
 
 from venc3.commands.export import export_blog
 from venc3.datastore.configuration import get_blog_configuration
 from venc3.helpers import copy_recursively
+from venc3.prompt import notify
 
 blog_configuration = get_blog_configuration() # TODO: Load only in time.
 
 WATCHED_FILES = {}
 LAST_WATCH_PASS = time.time()
 
 def get_files(folder=".."):
     files = []
     for item in os.listdir(folder):
         if item in ["extra", "includes", "entries", "theme", "blog_configuration.yaml"] or (folder != ".."):
             if item[0] != '.':
+                files += [folder+"/"+item]
                 if os.path.isdir(folder+"/"+item):
                     files += get_files(folder+"/"+item)
-                else:
-                    files += [folder+"/"+item]
-                
     return files
 
 def watch_files():
     global LAST_WATCH_PASS
     global WATCHED_FILES
     refresh_extra = False
     refresh_assets = False
     refresh_all = False
     
-    for path in get_files():
+    files = get_files()
+    for path in files:
         WATCHED_FILES[path] = os.path.getmtime(path)
-        if WATCHED_FILES[path] > LAST_WATCH_PASS:
-            if path[:len("../extra")] == "../extra":
+        if WATCHED_FILES[path] > LAST_WATCH_PASS and not os.path.isdir(path):
+            if path[:len("../extra")] == "../extra" :
                 refresh_extra |= True
 
             elif path[:len("../theme/assets")] == "../theme/assets":
                 refresh_assets |= True
                                 
             else:
               refresh_all |= True
               break
+    
+    keys = tuple(WATCHED_FILES.keys())
+    
+    for filename in keys:
+      if not filename in files:
+          WATCHED_FILES.pop(filename)
+          to_delete = None
+          if filename[:len("../extra")] == "../extra" and filename != "../extra":
+              to_delete = "blog"+filename[len("../extra"):]
+              
+          elif filename[:len("../theme/assets")] == "../theme/assets" and filename != "../theme/assets":
+              to_delete = "blog"+ filename[len("../theme/assets"):]
               
+          else:
+              refresh_all |= True
+              break
+          
+          if to_delete != None:
+              notify(("deleting_file", to_delete))
+              try:
+                  if os.path.isdir("../"+to_delete):
+                      shutil.rmtree("../"+to_delete)
+                      
+                  else:
+                          os.unlink("../"+to_delete)         
+              except FileNotFoundError:
+                  pass
+                      
     LAST_WATCH_PASS = time.time()
+    
     if refresh_all:
         return True
+        
     else:
+        if refresh_extra or refresh_assets:
+            notify(("copy_assets_and_extra_files",))
+            
         if refresh_extra:
             copy_recursively("../extra/", "./")
     
         if refresh_assets:
             copy_recursively("../theme/assets/", "./")
             
         return False
@@ -86,30 +119,28 @@
     export_blog(params)
     
 class VenCServer(http.server.CGIHTTPRequestHandler):    
     def __init__(self, request, client_address, server):
         super().__init__(request, client_address, server)
     
     def do_GET(self):
-        if watch_files(): # will silently trigger partial refresh of extra and assets
+        if watch_files(): # will trigger partial refresh of extra and assets
             sub_process = Process(target=export_blog_wrapper,args=([],))
             sub_process.start()
             sub_process.join()
         
         self.path = urllib.parse.unquote(self.path, encoding=blog_configuration["path_encoding"])
         super().do_GET()
 
     def send_error(self, code, message=None, explain=None):
         from venc3.datastore.hardcoded_assets import default_error_page
         self.error_message_format = default_error_page
         super().send_error(code, message, explain)
             
 def serv(params):            
-    from venc3.prompt import notify
-
     port = params[0] if len(params) else blog_configuration["server_port"]
         
     try:
         os.chdir("blog/")
         server_address = ("", port)
         notify(("do_not_use_in_production",), color="YELLOW")        
         notify(("serving_blog", port))
```

### Comparing `VenC-3.2.1/venc3/datastore/__init__.py` & `VenC-3.2.2/venc3/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/archives.py` & `VenC-3.2.2/venc3/datastore/archives.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/configuration.py` & `VenC-3.2.2/venc3/datastore/configuration.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/entries.py` & `VenC-3.2.2/venc3/datastore/entries.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/entry.py` & `VenC-3.2.2/venc3/datastore/entry.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/hardcoded_assets.py` & `VenC-3.2.2/venc3/datastore/hardcoded_assets.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/metadata.py` & `VenC-3.2.2/venc3/datastore/metadata.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/taxonomy.py` & `VenC-3.2.2/venc3/datastore/taxonomy.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/datastore/theme.py` & `VenC-3.2.2/venc3/datastore/theme.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/exceptions.py` & `VenC-3.2.2/venc3/exceptions.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/helpers.py` & `VenC-3.2.2/venc3/helpers.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/l10n/__init__.py` & `VenC-3.2.2/venc3/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/l10n/en.py` & `VenC-3.2.2/venc3/l10n/en.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,10 +117,11 @@
     not_installed = "is not installed."
     chapter_type_is_ambiguous = "Chapter index from entry is of type float #{0} and ambiguous. It should be str or int."
     current_python_implementation_doesnt_support_parallelism = "Current Python implementation doesn't support parallelism."
     no_parallel_processing_default_value = "No explicit value is defined for \"parallel_processing\" in your configuration file.\nBy default VenC will run {0} parallel processes."
     wrong_value_for_parallel_processing = "Wrong value for \"parallel_processing\" in your configuration file. It must be a non zero positive integer."
     invalid_variable_name_in_setting = "Invalid variable name {0} in \"{1}\" within your configuration file."
     invalid_value_in_setting = "Invalid value \"{0}\" in \"{1}\" within your configuration file."
+    deleting_file = "Deleting {0} ..."
     # Will not be hooked by l10n_cleanup
     generating_rss = "Generating RSS feed..."
     generating_atom = "Generating Atom feed..."
```

### Comparing `VenC-3.2.1/venc3/l10n/fr.py` & `VenC-3.2.2/venc3/l10n/fr.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,11 +117,12 @@
     not_installed = "n'est pas installé."
     chapter_type_is_ambiguous = "L'index du chapitre de la publication #{0} est de type float et est donc ambigu. Le type devrait être str ou int."
     current_python_implementation_doesnt_support_parallelism = "L'implémentation courante de Python ne supporte pas le parallélisme."
     no_parallel_processing_default_value = "Aucune valeur définie explicitement pour \"parallel_processing\" dans votre fichier de configuration.\nPar défaut, VenC utilisera {0} processus parallèles."
     wrong_value_for_parallel_processing = "La valeur de \"parallel_processing\" dans votre fichier de configuration est incorrecte, il doit s'agir d'un nombre entier supérieur à 0."
     invalid_variable_name_in_setting = "Variable {0} incorrecte dans \"{1}\" dans votre fichier de configuration."
     invalid_value_in_setting = "La valeur \"{0}\" dans \"{1}\", dans votre fichier de configuration, est incorrecte."
+    deleting_file = "Suppression de {0} ..."
     # Will not be hooked by l10n_cleanup
     generating_rss = "Génération du flux RSS..."
     generating_atom = "Génération du flux Atom..."
```

### Comparing `VenC-3.2.1/venc3/markup_languages/__init__.py` & `VenC-3.2.2/venc3/markup_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/markup_languages/asciidoc.py` & `VenC-3.2.2/venc3/markup_languages/asciidoc.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/markup_languages/markdown.py` & `VenC-3.2.2/venc3/markup_languages/markdown.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/markup_languages/restructuredtext.py` & `VenC-3.2.2/venc3/markup_languages/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/parallelism/__init__.py` & `VenC-3.2.2/venc3/parallelism/__init__.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/parallelism/build_entries.py` & `VenC-3.2.2/venc3/parallelism/build_entries.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/parallelism/export_entries.py` & `VenC-3.2.2/venc3/parallelism/export_entries.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/datastore.py` & `VenC-3.2.2/venc3/patterns/datastore.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/non_contextual.py` & `VenC-3.2.2/venc3/patterns/non_contextual.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/patterns_map.py` & `VenC-3.2.2/venc3/patterns/patterns_map.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/processor.py` & `VenC-3.2.2/venc3/patterns/processor.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/theme.py` & `VenC-3.2.2/venc3/patterns/theme.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/third_party_wrapped_features/kroki.py` & `VenC-3.2.2/venc3/patterns/third_party_wrapped_features/kroki.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/third_party_wrapped_features/latex2mathml.py` & `VenC-3.2.2/venc3/patterns/third_party_wrapped_features/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/third_party_wrapped_features/oembed.py` & `VenC-3.2.2/venc3/patterns/third_party_wrapped_features/oembed.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/patterns/third_party_wrapped_features/pygmentize.py` & `VenC-3.2.2/venc3/patterns/third_party_wrapped_features/pygmentize.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/prompt.py` & `VenC-3.2.2/venc3/prompt.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/threads/__init__.py` & `VenC-3.2.2/venc3/threads/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,27 +114,27 @@
         
         else:
             return string2
                 
     # Must be called in child class
     def organize_entries(self, entries):
         self.pages = list()
+        
+        self.most_recent_entry_date = max([entry.date for entry in entries])
+        
         for i in range(0, ceil(len(entries)/self.entries_per_page)):
             self.pages.append(
                 entries[i*self.entries_per_page:(i+1)*self.entries_per_page]
             )
 
         self.pages_count = len(self.pages)
 
     def get_last_entry_timestamp(self, pattern, time_format):
-        from venc3.exceptions import VenCException
-        raise VenCException(
-            ("you_cannot_use_this_pattern_here", "GetLastEntryTimestamp", pattern.root.context),
-            pattern
-        )
+        import datetime
+        return datetime.datetime.strftime(self.most_recent_entry_date, time_format)
         
     # Must be called in child class
     def get_next_page(self, pattern, string):
         '''page_number,entry_id,entry_title,path'''
         if self.current_page < self.pages_count - 1:
             params = {
                 "page_number" : str(self.current_page + 1),
```

### Comparing `VenC-3.2.1/venc3/threads/archives.py` & `VenC-3.2.2/venc3/threads/archives.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/threads/categories.py` & `VenC-3.2.2/venc3/threads/categories.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/threads/chapters.py` & `VenC-3.2.2/venc3/threads/chapters.py`

 * *Files identical despite different names*

### Comparing `VenC-3.2.1/venc3/threads/entries.py` & `VenC-3.2.2/venc3/threads/entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,22 @@
                 'entry_id': self.current_entry.id,
                 'entry_title': self.current_entry.title
             })
         
         except KeyError as e:
             from venc3.prompt import die
             die(("variable_error_in_filename", str(e)))
-            
+
+    def get_last_entry_timestamp(self, pattern, time_format):
+        from venc3.exceptions import VenCException
+        raise VenCException(
+            ("you_cannot_use_this_pattern_here", "GetLastEntryTimestamp", pattern.root.context),
+            pattern
+        )
+        
     def if_in_first_page(self, node, string1, string2=''):
         return string2.strip()
 
     def if_in_last_page(self, node, string1, string2=''):
         return string2.strip()
     
     def if_in_entry_id(self, node, entry_id, string1, string2=''):
```

### Comparing `VenC-3.2.1/venc3/threads/feed.py` & `VenC-3.2.2/venc3/threads/feed.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,14 @@
         self.columns_number = 1
         self.filename = self.datastore.blog_configuration["paths"][feed_type+"_file_name"]
         self.entries_per_page = self.datastore.blog_configuration["feed_length"]
         self.in_thread = True
         self.content_type = feed_type
 
     def do(self, entries, export_path, relative_origin):
-        self.last_entry = entries[-1]
         self.export_path = export_path
         self.relative_origin = relative_origin
         self.organize_entries(entries)
         super().do()
 
     def if_in_feed(self, node, string1, string2=''):
         return string1.strip()
-            
-    def get_last_entry_timestamp(self, pattern, time_format):
-        import datetime
-        return datetime.datetime.strftime(self.last_entry.date, time_format)
```

### Comparing `VenC-3.2.1/venc3/threads/main.py` & `VenC-3.2.2/venc3/threads/main.py`

 * *Files identical despite different names*

