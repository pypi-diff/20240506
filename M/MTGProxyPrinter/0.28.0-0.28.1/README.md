# Comparing `tmp/MTGProxyPrinter-0.28.0.tar.gz` & `tmp/mtgproxyprinter-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.28.0.tar", last modified: Sun Mar 24 18:18:46 2024, max compression, from Unix
+gzip compressed data, was "mtgproxyprinter-0.28.1.tar", last modified: Mon May  6 12:13:52 2024, max compression
```

## Comparing `MTGProxyPrinter-0.28.0.tar` & `mtgproxyprinter-0.28.1.tar`

### file list

```diff
@@ -1,289 +1,132 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.28.0/LICENSE.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/MANIFEST.in
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12080 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14903 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      300 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2024-03-24 18:18:45.000000 MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12080 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10192 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/ThirdPartyLicenses.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.952794 MTGProxyPrinter-0.28.0/doc/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    54645 2024-03-24 18:04:41.000000 MTGProxyPrinter-0.28.0/doc/changelog.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.952794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      749 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3251 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/__main__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1440 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/app_dirs.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11962 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/application.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2286 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/argument_parser.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    40517 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/card_info_downloader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    18204 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_downloader.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.956794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8211 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10399 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11290 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/re_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.956794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2942 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/_interface.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11619 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/card_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5140 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/compact_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6029 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/edit_document_settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2683 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/import_deck_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2823 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/load_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6429 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/move_cards.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2925 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/new_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8198 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/page_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4559 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/replace_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4175 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/shuffle_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3230 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/downloader_base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10487 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/http_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2729 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      981 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/meta_data.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3932 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/metered_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2795 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/missing_images_manager.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.956794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11923 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/card_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    45003 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8513 2024-02-29 16:41:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    33614 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb_migrations.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v2.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v3.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v4.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v5.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v6.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19573 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34386 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document_loader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2701 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    22360 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/imagedb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2535 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/string_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2487 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/natsort.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6743 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/print.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2900 2024-02-04 18:12:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/print_count_updater.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17401 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/printing_filter_updater.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2178 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/progress_meter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.956794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.948794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.956794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.948794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.960794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      490 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      516 2024-03-24 17:27:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/transform-rotate.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1255 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/view-hidden.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.964794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      441 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      675 2024-03-24 17:27:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/transform-rotate.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1327 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/view-hidden.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.964794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      675 2024-03-24 17:27:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/transform-rotate.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1327 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/view-hidden.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2024-01-08 13:08:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/index.theme
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.948794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/status/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/status/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/status/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7659 2024-03-24 17:27:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/resources.qrc
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7286 2024-02-29 16:40:57.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/about_dialog.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6300 2024-02-29 16:40:57.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5764 2024-02-29 16:40:57.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3464 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5216 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1044 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4242 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4095 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3715 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.968794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5022 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3117 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20414 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1948 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/document_settings_dialog.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10904 2024-03-21 14:22:20.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/main_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13271 2024-03-24 17:27:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1143 2024-01-30 21:09:30.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/progress_bar.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3607 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/debug_settings_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5454 2024-03-21 14:22:20.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/decklist_import_settings_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8091 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10845 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8332 2024-03-21 14:22:20.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/general_settings_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2192 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/hide_printings_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4154 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/page_size_printing_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3975 2024-02-22 13:45:03.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1468 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/runner.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19124 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8953 2024-01-30 21:09:29.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/sqlite_helpers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13120 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/add_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21553 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    15050 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/central_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6256 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1053 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/compiled_resources.pyi
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    32291 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/deck_import_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13744 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/dialogs.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8404 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/about_dialog.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8809 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8307 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4483 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6023 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1606 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.972794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5666 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5358 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4216 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6924 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4361 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    18010 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2084 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/document_settings_dialog.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14224 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16868 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2161 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/progress_bar.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5235 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/debug_settings_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8111 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/decklist_import_settings_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13554 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16100 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11669 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/general_settings_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3208 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/hide_printings_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5874 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/page_size_printing_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4345 2024-03-24 18:18:41.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4324 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/item_delegates.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26296 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11134 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5834 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_renderer.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    33713 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_scene.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7396 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/printing_filter_widgets.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4089 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/progress_bar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12923 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21411 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/settings_window_pages.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7495 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/units_and_sizes.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8460 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/mtg_proxy_printer/update_checker.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6040 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-03-24 18:18:45.976794 MTGProxyPrinter-0.28.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2024-03-24 18:18:15.000000 MTGProxyPrinter-0.28.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.922841 mtgproxyprinter-0.28.1/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 mtgproxyprinter-0.28.1/LICENSE.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      241 2024-04-09 21:25:41.000000 mtgproxyprinter-0.28.1/MANIFEST.in
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.920841 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12630 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5315 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2024-05-06 12:13:52.000000 mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12630 2024-05-06 12:13:52.921841 mtgproxyprinter-0.28.1/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10196 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.905841 mtgproxyprinter-0.28.1/doc/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/doc/ThirdPartyLicenses.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    55476 2024-05-06 11:59:50.000000 mtgproxyprinter-0.28.1/doc/changelog.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.908841 mtgproxyprinter-0.28.1/mtg_proxy_printer/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      749 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3251 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/__main__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1440 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/app_dirs.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11962 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/application.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2286 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/argument_parser.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    40549 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/card_info_downloader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    18217 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_downloader.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.909841 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8211 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10399 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/csv_parsers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11290 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/re_parsers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.910841 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2024-01-08 13:08:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2923 2024-05-06 07:40:40.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/_interface.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11619 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/card_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5140 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/compact_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6029 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/edit_document_settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2683 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/import_deck_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2823 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/load_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6429 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/move_cards.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2925 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/new_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8198 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/page_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4559 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/replace_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4175 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/shuffle_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3230 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/downloader_base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10487 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/http_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2729 2024-04-01 13:42:40.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      981 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/meta_data.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3932 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/metered_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2795 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/missing_images_manager.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.912841 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11923 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/card_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    45003 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8513 2024-02-29 16:41:03.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    33614 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb_migrations.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v2.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v3.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2024-01-08 13:08:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v4.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2024-01-08 13:08:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v5.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2024-01-30 21:09:30.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v6.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    19573 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34577 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document_loader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2701 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    22599 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/imagedb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2535 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/model/string_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2487 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/natsort.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7862 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/print.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2900 2024-02-04 18:12:15.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/print_count_updater.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17401 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/printing_filter_updater.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2178 2024-01-30 21:09:30.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/progress_meter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1468 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/runner.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20347 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8953 2024-01-30 21:09:29.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/sqlite_helpers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.916841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13112 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/add_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21553 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    15038 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/central_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6270 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)   988601 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/compiled_resources.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1053 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/compiled_resources.pyi
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    32400 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/deck_import_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13843 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/dialogs.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.917841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8404 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/about_dialog.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.917841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8776 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8274 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.918841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4483 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6023 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1606 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.918841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5645 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5339 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4201 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.919841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6924 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4361 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    18010 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2084 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/document_settings_dialog.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14224 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16868 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2161 2024-05-06 12:13:48.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/progress_bar.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:52.920841 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6770 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/debug_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8111 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/decklist_import_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1781 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/default_document_layout_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13554 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16100 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10213 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/general_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3184 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/hide_printings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5930 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/pdf_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2760 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/printer_settings_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4871 2024-05-06 12:13:49.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4303 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/item_delegates.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26244 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10920 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5768 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_renderer.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    33728 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_scene.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7169 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/printing_filter_widgets.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4086 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/progress_bar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12026 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25248 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/settings_window_pages.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7494 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/units_and_sizes.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8476 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/mtg_proxy_printer/update_checker.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3283 2024-05-06 12:03:28.000000 mtgproxyprinter-0.28.1/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2024-05-06 12:13:52.922841 mtgproxyprinter-0.28.1/setup.cfg
```

### Comparing `MTGProxyPrinter-0.28.0/LICENSE.md` & `mtgproxyprinter-0.28.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/MTGProxyPrinter.egg-info/PKG-INFO` & `mtgproxyprinter-0.28.1/MTGProxyPrinter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.28.0
+Version: 0.28.1
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -14,30 +14,42 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Requires-Python: !=3.11.1,<4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: platformdirs>=2.6.0
 Requires-Dist: PyQt5
 Requires-Dist: ijson>=3.1.0; python_version < "3.11"
 Requires-Dist: ijson>=3.2.0; python_version >= "3.11"
-Requires-Dist: pint<0.22; platform_system == "windows"
-Requires-Dist: pint; platform_system != "windows"
+Requires-Dist: ijson>=3.2.1; python_version >= "3.12"
+Requires-Dist: pint<0.22; python_version < "3.9"
+Requires-Dist: pint; python_version >= "3.9"
 Requires-Dist: delegateto==1.5
-Requires-Dist: PyHamcrest>=1.8.1
+Requires-Dist: PyHamcrest>=2
 Requires-Dist: truststore; python_version >= "3.10"
 Requires-Dist: certifi; python_version < "3.10"
+Requires-Dist: typing_extensions; python_version < "3.11"
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev"
+Requires-Dist: pytest-qt>=2.0; extra == "dev"
+Requires-Dist: tox>=4.0; extra == "dev"
+Provides-Extra: package
+Requires-Dist: build; extra == "package"
+Requires-Dist: cx_Freeze>=6.11.1; platform_python_implementation == "CPython" and extra == "package"
 
 # MTGProxyPrinter
 
 Print Magic: The Gathering cards for play-testing purposes.
 
 
 ## Feature overview
@@ -216,8 +228,8 @@
 Copyright (C) 2014 Uri Herrera <uri_herrera@nitrux.in> and others
 
 The icons shipped in the directory mtg_proxy_printer/resources/icons/ are used as a fallback if no
 system theme is present, and are sourced from Breeze icon theme created by the KDE project.
 These fall under the LGPL either version 3 of the License, or
 (at your option) any later version.
 
-See the [ThirdPartyLicenses.md](./ThirdPartyLicenses.md) file for details.
+See the [ThirdPartyLicenses.md](./doc/ThirdPartyLicenses.md) file for details.
```

### Comparing `MTGProxyPrinter-0.28.0/PKG-INFO` & `mtgproxyprinter-0.28.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.28.0
+Version: 0.28.1
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -14,30 +14,42 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Requires-Python: !=3.11.1,<4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: platformdirs>=2.6.0
 Requires-Dist: PyQt5
 Requires-Dist: ijson>=3.1.0; python_version < "3.11"
 Requires-Dist: ijson>=3.2.0; python_version >= "3.11"
-Requires-Dist: pint<0.22; platform_system == "windows"
-Requires-Dist: pint; platform_system != "windows"
+Requires-Dist: ijson>=3.2.1; python_version >= "3.12"
+Requires-Dist: pint<0.22; python_version < "3.9"
+Requires-Dist: pint; python_version >= "3.9"
 Requires-Dist: delegateto==1.5
-Requires-Dist: PyHamcrest>=1.8.1
+Requires-Dist: PyHamcrest>=2
 Requires-Dist: truststore; python_version >= "3.10"
 Requires-Dist: certifi; python_version < "3.10"
+Requires-Dist: typing_extensions; python_version < "3.11"
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev"
+Requires-Dist: pytest-qt>=2.0; extra == "dev"
+Requires-Dist: tox>=4.0; extra == "dev"
+Provides-Extra: package
+Requires-Dist: build; extra == "package"
+Requires-Dist: cx_Freeze>=6.11.1; platform_python_implementation == "CPython" and extra == "package"
 
 # MTGProxyPrinter
 
 Print Magic: The Gathering cards for play-testing purposes.
 
 
 ## Feature overview
@@ -216,8 +228,8 @@
 Copyright (C) 2014 Uri Herrera <uri_herrera@nitrux.in> and others
 
 The icons shipped in the directory mtg_proxy_printer/resources/icons/ are used as a fallback if no
 system theme is present, and are sourced from Breeze icon theme created by the KDE project.
 These fall under the LGPL either version 3 of the License, or
 (at your option) any later version.
 
-See the [ThirdPartyLicenses.md](./ThirdPartyLicenses.md) file for details.
+See the [ThirdPartyLicenses.md](./doc/ThirdPartyLicenses.md) file for details.
```

### Comparing `MTGProxyPrinter-0.28.0/README.md` & `mtgproxyprinter-0.28.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -179,8 +179,8 @@
 Copyright (C) 2014 Uri Herrera <uri_herrera@nitrux.in> and others
 
 The icons shipped in the directory mtg_proxy_printer/resources/icons/ are used as a fallback if no
 system theme is present, and are sourced from Breeze icon theme created by the KDE project.
 These fall under the LGPL either version 3 of the License, or
 (at your option) any later version.
 
-See the [ThirdPartyLicenses.md](./ThirdPartyLicenses.md) file for details.
+See the [ThirdPartyLicenses.md](./doc/ThirdPartyLicenses.md) file for details.
```

### Comparing `MTGProxyPrinter-0.28.0/ThirdPartyLicenses.md` & `mtgproxyprinter-0.28.1/doc/ThirdPartyLicenses.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/doc/changelog.md` & `mtgproxyprinter-0.28.1/doc/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 # Changelog
 
-# 0.28.0 (2024-03-24)  <a name="v0_28_0"></a>
+# Version 0.28.1 (2024-05-06)  <a name="v0_28_1"></a>
+
+## New features
+
+- Add a landscape printing workaround that can be enabled independently for direct printing and PDF export.
+  If enabled, landscape documents are internally rotated by 90° during the export/print process,
+  so that they are treated as regular, portrait-mode documents.
+
+## Changed features
+
+- Printer and PDF export options are moved to dedicated pages in the application settings window.
+
+## Fixed issues
+
+- Fixed broken card bleed rendering when row spacing or column spacing are set to zero.
+  The thick border around the cards is now continuous, as it was in version [0.27](#0_27_0).
+- Fix the page view not updating instantly when the application successfully downloads a card image that
+  failed to download during previous download attempts.
+
+# Version 0.28.0 (2024-03-24)  <a name="v0_28_0"></a>
 
 ## New features
 
 - Added a button to the document settings to toggle between portrait and landscape mode. 
 - Support automatic deck list downloads from [ManaBox.app](https://manabox.app).
 
 ## Changed features
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/__init__.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/__main__.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/__main__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/app_dirs.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/app_dirs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/application.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/application.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/argument_parser.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/argument_parser.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/card_info_downloader.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/card_info_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,23 +396,23 @@
             url, _ = self.get_scryfall_bulk_card_data_url()
             logger.debug(f"Obtained url: {url}")
         else:
             logger.debug(f"Reading from given URL {url}")
         # Ignore the monitor, because progress reporting is done in the main import loop.
         source, _ = self.read_from_url(url)
         with source:
-            yield from ijson.items(source, json_path)
+            yield from ijson.items(source, json_path, use_float=True)
 
     def read_json_card_data_from_file(self, file_path: Path, json_path: str = "item") -> CardStream:
         file_size = file_path.stat().st_size
         raw_file = file_path.open("rb")
         with self._wrap_in_metered_file(raw_file, file_size) as file:
             if file_path.suffix.casefold() == ".gz":
                 file = gzip.open(file, "rb")
-            yield from ijson.items(file, json_path)
+            yield from ijson.items(file, json_path, use_float=True)
 
     def _wrap_in_metered_file(self, raw_file, file_size):
         monitor = mtg_proxy_printer.metered_file.MeteredFile(raw_file, file_size, self)
         monitor.total_bytes_processed.connect(self.download_progress)
         monitor.io_begin.connect(lambda size: self.download_begins.emit(size, "Importing card data from disk:"))
         return monitor
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_downloader.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 logger.debug(f"Input is valid URL for {downloader_class.APPLICABLE_WEBSITES}")
                 return State.Acceptable, input_string, pos
         return State.Intermediate, input_string, pos
 
 
 class DecklistDownloader(DownloaderBase):
     DECKLIST_PATH_RE = re.compile(r"")
-    PARSER_CLASS: ParserBase = None
+    PARSER_CLASS: typing.Type[ParserBase] = None
     APPLICABLE_WEBSITES: str = ""
 
     def download(self, decklist_url: str) -> str:
         logger.info(f"About to fetch deck list from {decklist_url}")
         download_url = self.map_to_download_url(decklist_url)
         logger.debug(f"Obtained download URL: {download_url}")
         data, monitor = self.read_from_url(download_url, "Downloading deck list:")
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/common.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/csv_parsers.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/csv_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/decklist_parser/re_parsers.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/decklist_parser/re_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/_interface.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 if typing.TYPE_CHECKING:
     from mtg_proxy_printer.model.document import Document
 
 try:
     from typing import Self
 except ImportError:  # Compatibility with Python < 3.11
-    Self = typing.TypeVar("Self", bound="DocumentAction")
+    from typing_extensions import Self
 
 __all__ = [
     "DocumentAction",
     "IllegalStateError",
     "Self",
     "ActionList",
     "split_iterable",
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/card_actions.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/card_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/compact_document.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/compact_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/edit_document_settings.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/edit_document_settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/import_deck_list.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/import_deck_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/load_document.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/load_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/move_cards.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/move_cards.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/new_document.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/new_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/page_actions.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/page_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/replace_card.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/replace_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/document_controller/shuffle_document.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/document_controller/shuffle_document.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 from ._interface import DocumentAction, IllegalStateError, Self
 from mtg_proxy_printer.model.carddb import Card
 from mtg_proxy_printer.model.card_list import PageColumns
 from mtg_proxy_printer.model.document_page import CardContainer
 from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.units_and_sizes import PageType
-
 __all__ = [
     "ActionShuffleDocument",
 ]
+
 IndexedCards = typing.List[typing.Tuple[int, Card]]
 ModelIndexList = typing.List[QModelIndex]
 ItemDataRole = Qt.ItemDataRole
 
 
 class ActionShuffleDocument(DocumentAction):
     """
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/downloader_base.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/downloader_base.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/http_file.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/http_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/logger.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/logger.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/meta_data.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/meta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 PROGRAMNAME = "MTGProxyPrinter"
-__version__ = "0.28.0"
+__version__ = "0.28.1"
 COPYRIGHT = "(C) 2020-2024 Thomas Hess"
 HOME_PAGE = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter"
 
 DOWNLOAD_WEB_PAGE = f"{HOME_PAGE}/uv/download.html"
 USER_AGENT = f"{PROGRAMNAME}/{__version__} ({HOME_PAGE})"
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/metered_file.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/metered_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/missing_images_manager.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/missing_images_manager.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/card_list.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/card_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/carddb_migrations.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/carddb_migrations.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v2.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v2.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v3.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v3.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v4.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v4.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v5.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v5.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document-v6.sql` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document-v6.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document_loader.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,20 +120,23 @@
             document_settings.getint("margin-right-mm"),
             document_settings.getint("margin-top-mm"),
             document_settings.getint("paper-height-mm"),
             document_settings.getint("paper-width-mm"),
         )
 
     def to_page_layout(self, render_mode: "RenderMode") -> QPageLayout:
-        orientation = QPageLayout.Orientation
         margins = QMarginsF(self.margin_left, self.margin_top, self.margin_right, self.margin_bottom) \
             if render_mode.IMPLICIT_MARGINS in render_mode else QMarginsF(0, 0, 0, 0)
+        landscape_workaround = mtg_proxy_printer.settings.settings["printer"].getboolean("landscape-compatibility-workaround")
+        orientation = QPageLayout.Orientation.Portrait \
+            if self.page_width < self.page_height or landscape_workaround \
+            else QPageLayout.Orientation.Landscape
         layout = QPageLayout(
             QPageSize(QSizeF(*sorted([self.page_width, self.page_height])), QPageSize.Unit.Millimeter),
-            orientation.Portrait if self.page_width < self.page_height else orientation.Landscape,
+            orientation,
             margins,
             QPageLayout.Unit.Millimeter,
         )
         return layout
 
     def __lt__(self, other):
         if not isinstance(other, self.__class__):
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/document_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/document_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/imagedb.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/imagedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 import shutil
 import socket
 import string
 import threading
 import typing
 import urllib.error
 
-from PyQt5.QtCore import QObject, pyqtSignal as Signal, pyqtSlot as Slot, QSize, QModelIndex, Qt, QThreadPool
+from PyQt5.QtCore import QObject, pyqtSignal as Signal, pyqtSlot as Slot, QModelIndex, Qt, QThreadPool
 from PyQt5.QtGui import QPixmap, QColorConstants
 
+if typing.TYPE_CHECKING:
+    from mtg_proxy_printer.model.document import Document
+
 from mtg_proxy_printer.model.carddb import with_database_write_lock
 from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
 from mtg_proxy_printer.document_controller.replace_card import ActionReplaceCard
 from mtg_proxy_printer.document_controller.import_deck_list import ActionImportDeckList
 from mtg_proxy_printer.document_controller import DocumentAction
 import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.downloader_base
@@ -337,24 +340,28 @@
             self.batch_process_progress.emit(index)
         self.request_action.emit(action)
         self.batch_process_finished.emit()
         self.update_batch_processing_state(False)
         logger.info(f"Obtained images for {total_cards} cards.")
 
     def obtain_missing_images(self, card_indices: typing.List[QModelIndex]):
+        if not card_indices:
+            return
         total_cards = len(card_indices)
         logger.debug(f"Requesting {total_cards} missing images")
         blank = self.image_database.blank_image
+        document: "Document" = card_indices[0].model()
         self.update_batch_processing_state(True)
         self.batch_process_starting.emit(total_cards, "Fetching missing images")
         for index, card_index in enumerate(card_indices, start=1):
             card = card_index.data(ItemDataRole.UserRole)
             self.get_image_synchronous(card)
             if card.image_file is not blank:
                 self.missing_image_obtained.emit(card_index)
+            document.on_missing_image_obtained(card_index)
             self.batch_process_progress.emit(index)
         self.batch_process_finished.emit()
         self.update_batch_processing_state(False)
         logger.debug(f"Done fetching {total_cards} missing images.")
         self.missing_images_obtained.emit()
 
     def update_batch_processing_state(self, value: bool):
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/model/string_list.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/model/string_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/natsort.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/natsort.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/print.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/print.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 from PyQt5.QtCore import QObject, QMarginsF, QSizeF, pyqtSlot as Slot, QPersistentModelIndex
 from PyQt5.QtGui import QPainter, QPdfWriter, QPageSize
 from PyQt5.QtPrintSupport import QPrinter
 
 import mtg_proxy_printer.meta_data
 from mtg_proxy_printer.settings import settings
 from mtg_proxy_printer.model.document import Document
+from mtg_proxy_printer.model.document_loader import PageLayoutSettings
 from mtg_proxy_printer.ui.page_scene import RenderMode, PageScene
 from mtg_proxy_printer.logger import get_logger
 import mtg_proxy_printer.units_and_sizes
 logger = get_logger(__name__)
 del get_logger
 
 __all__ = [
     "export_pdf",
     "create_printer",
     "Renderer",
 ]
 
 
 def export_pdf(document: Document, file_path: str, parent: QObject = None):
-    pages_to_print = settings["documents"].getint("pdf-page-count-limit") or document.rowCount()
+    pages_to_print = settings["pdf-export"].getint("pdf-page-count-limit") or document.rowCount()
     if not pages_to_print:  # No pages in document. Return now, to avoid dividing by zero
         logger.error("Tried to export a document with zero pages as a PDF. Aborting.")
         return
     logger.info(f'Exporting document with {document.rowCount()} pages as PDF to "{file_path}"')
     total_documents = math.ceil(document.rowCount()/pages_to_print)
     for document_index in range(total_documents):
         logger.info(f"Creating PDF ({document_index+1}/{total_documents}) with up to {pages_to_print} pages.")
@@ -66,48 +67,59 @@
     printer.setDuplex(QPrinter.DuplexMode.DuplexNone)
     printer.setOutputFormat(QPrinter.OutputFormat.NativeFormat)
     if RenderMode.IMPLICIT_MARGINS not in renderer.render_mode:
         printer.setFullPage(True)
     return printer
 
 
+
+
 class PDFPrinter(QPdfWriter):
 
     def __init__(self, document: Document, file_path: str, parent: QObject = None,
                  document_index: int = 0, pages_to_print: int = None):
         self.document = document
         self.document_index = document_index
         self.pages_to_print: int = pages_to_print or document.rowCount()
+        self.landscape_workaround_enabled = settings["pdf-export"].getboolean("landscape-compatibility-workaround")
         if pages_to_print < document.rowCount():
             path = Path(file_path)
             # Add one to the document_index for human-readable counting starting at 1. suffix includes the separator
-            file_path = str(path.parent / f"{path.stem}-{document_index+1}{path.suffix}")
+            file_path = str(path.with_stem(f"{path.stem}-{document_index+1}"))
         super().__init__(file_path)
         self.setParent(parent)
         self.setCreator(f"{mtg_proxy_printer.meta_data.PROGRAMNAME}, v{mtg_proxy_printer.meta_data.__version__}")
         self.painter = QPainter()
         # magnitude returns a float by default, so round to int to avoid a TypeError
         self.setResolution(round(mtg_proxy_printer.units_and_sizes.RESOLUTION.magnitude))
-        self.setPageSize(QPageSize(
-            QSizeF(document.page_layout.page_width, document.page_layout.page_height),
-            QPageSize.Unit.Millimeter
-        ))
+        self.setPageSize(self._to_page_size(document.page_layout))
         # Prevent downscaling the page content
         self.setPageMargins(QMarginsF(0, 0, 0, 0))
         self.scene = PageScene(document, RenderMode.ON_PAPER, self)
         logger.info(f"Created {self.__class__.__name__} instance.")
 
+    def _to_page_size(self, layout: PageLayoutSettings) -> QPageSize:
+        size = QSizeF(layout.page_width, layout.page_height)
+        if layout.page_width > layout.page_height and self.landscape_workaround_enabled:
+            size.transpose()
+        return QPageSize(size, QPageSize.Unit.Millimeter)
+
     def print_document(self):
         logger.info("Begin rendering PDF document.")
+        layout = self.document.page_layout
+        scaling = 1
         self.painter.begin(self)
-        # Prevent quality loss by re-compressing the source images
-        self.painter.setRenderHint(QPainter.LosslessImageRendering)
+        if layout.page_width > layout.page_height and self.landscape_workaround_enabled:
+            scaling = self.scene.width()/self.scene.height()
+            self.painter.rotate(90)
+            self.painter.translate(0, -self.scene.height())
+        self.painter.setRenderHint(QPainter.LosslessImageRendering)  # Prevent avoidable image degradation
         self.painter.scale(
-                self.logicalDpiX()/self.resolution(),
-                self.logicalDpiY()/self.resolution()
+                scaling*self.logicalDpiX()/self.resolution(),
+                scaling*self.logicalDpiY()/self.resolution(),
             )
         first_index = self.document_index * self.pages_to_print
         last_index = min((self.document_index + 1) * self.pages_to_print, self.document.rowCount())
 
         for index in range(first_index, last_index):
             logger.debug(f"Rendering page {index+1}/{self.document.rowCount()}")
             self.scene.on_current_page_changed(QPersistentModelIndex(self.document.index(index, 0)))
@@ -127,15 +139,22 @@
         if not settings["printer"].getboolean("borderless-printing"):
             self.render_mode |= RenderMode.IMPLICIT_MARGINS
         self.scene = PageScene(document, self.render_mode, self)
 
     @Slot(QPrinter)
     def print_document(self, printer: QPrinter):
         logger.info("Begin printing document.")
+        landscape_workaround_enabled = settings["printer"].getboolean("landscape-compatibility-workaround")
+        is_landscape_document = self.scene.width() > self.scene.height()
         painter = QPainter(printer)
+        if is_landscape_document and landscape_workaround_enabled:
+            painter.rotate(90)
+            painter.translate(0, -self.scene.height())
+            scaling = self.scene.width()/self.scene.height()
+            painter.scale(scaling, scaling)
         painter.setRenderHint(QPainter.LosslessImageRendering)
         page_count = self.document.rowCount()
         for index in range(page_count):
             logger.debug(f"Printing page {index+1}/{page_count}")
             self.scene.on_current_page_changed(QPersistentModelIndex(self.document.index(index, 0)))
             self.scene.render(painter)
             if index+1 < page_count:
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/print_count_updater.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/print_count_updater.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/printing_filter_updater.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/printing_filter_updater.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/progress_meter.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/progress_meter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/runner.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/runner.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/settings.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,33 +101,31 @@
     "margin-top-mm": "5",
     "margin-bottom-mm": "5",
     "margin-left-mm": "5",
     "margin-right-mm": "5",
     "row-spacing-mm": "0",
     "column-spacing-mm": "0",
     "print-cut-marker": "False",
-    "pdf-page-count-limit": "0",
     "print-sharp-corners": "False",
     "print-page-numbers": "False",
     "default-document-name": "",
 }
 DEFAULT_SETTINGS["default-filesystem-paths"] = {
     "document-save-path": QStandardPaths.locate(QStandardPaths.DocumentsLocation, "", QStandardPaths.LocateDirectory),
-    "pdf-export-path": QStandardPaths.locate(QStandardPaths.DocumentsLocation, "", QStandardPaths.LocateDirectory),
     "deck-list-search-path": QStandardPaths.locate(QStandardPaths.DownloadLocation, "", QStandardPaths.LocateDirectory),
 }
 DEFAULT_SETTINGS["gui"] = {
     "central-widget-layout": "columnar",
     "show-toolbar": "True",
 }
 VALID_SEARCH_WIDGET_LAYOUTS = {"horizontal", "columnar", "tabbed"}
 DEFAULT_SETTINGS["debug"] = {
     "cutelog-integration": "False",
     "write-log-file": "True",
-    "log-level": "INFO"
+    "log-level": "INFO",
 }
 VALID_LOG_LEVELS = set(map(logging.getLevelName, range(10, 60, 10)))
 DEFAULT_SETTINGS["decklist-import"] = {
     "enable-print-guessing-by-default": "True",
     "prefer-already-downloaded-images": "True",
     "always-translate-deck-lists": "False",
     "remove-basic-wastes": "False",
@@ -135,15 +133,21 @@
 }
 DEFAULT_SETTINGS["application"] = {
     "last-used-version": mtg_proxy_printer.meta_data.__version__,
     "check-for-application-updates": "None",
     "check-for-card-data-updates": "None",
 }
 DEFAULT_SETTINGS["printer"] = {
-    "borderless-printing": "True"
+    "borderless-printing": "True",
+    "landscape-compatibility-workaround": "False",
+}
+DEFAULT_SETTINGS["pdf-export"] = {
+    "pdf-export-path": QStandardPaths.locate(QStandardPaths.DocumentsLocation, "", QStandardPaths.LocateDirectory),
+    "pdf-page-count-limit": "0",
+    "landscape-compatibility-workaround": "False",
 }
 MAX_DOCUMENT_NAME_LENGTH = 200
 
 
 def get_boolean_card_filter_keys():
     """Returns all keys for boolean card filter settings."""
     keys = DEFAULT_SETTINGS["card-filter"].keys()
@@ -220,14 +224,15 @@
     _validate_documents_section(read_settings)
     _validate_application_section(read_settings)
     _validate_gui_section(read_settings)
     _validate_debug_section(read_settings)
     _validate_decklist_import_section(read_settings)
     _validate_default_filesystem_paths_section(read_settings)
     _validate_printer_section(read_settings)
+    _validate_pdf_export_section(read_settings)
 
 
 def _validate_card_filter_section(settings: configparser.ConfigParser, section_name: str = "card-filter"):
     section = settings[section_name]
     defaults = DEFAULT_SETTINGS[section_name]
     boolean_keys = get_boolean_card_filter_keys()
     for key in boolean_keys:
@@ -332,15 +337,24 @@
     for key in section.keys():
         _validate_path_to_directory(section, defaults, key)
 
 
 def _validate_printer_section(settings: configparser.ConfigParser, section_name: str = "printer"):
     section = settings[section_name]
     defaults = DEFAULT_SETTINGS[section_name]
-    _validate_boolean(section, defaults, "borderless-printing")
+    for item in defaults.keys():
+        _validate_boolean(section, defaults, item)
+
+
+def _validate_pdf_export_section(to_validate: configparser.ConfigParser, section_name: str = "pdf-export"):
+    section = to_validate[section_name]
+    defaults = DEFAULT_SETTINGS[section_name]
+    _validate_path_to_directory(section, defaults, "pdf-export-path")
+    _validate_non_negative_int(section, defaults, "pdf-page-count-limit")
+    _validate_boolean(section, defaults, "landscape-compatibility-workaround")
 
 
 def _validate_path_to_directory(section: configparser.SectionProxy, defaults: configparser.SectionProxy, key: str):
     try:
         if not pathlib.Path(section[key]).resolve().is_dir():
             raise ValueError
     except Exception:
@@ -384,14 +398,15 @@
 
 def migrate_settings(settings: configparser.ConfigParser):
     _migrate_layout_setting(settings)
     _migrate_download_settings(settings)
     _migrate_default_save_paths_settings(settings)
     _migrate_print_guessing_settings(settings)
     _migrate_image_spacing_settings(settings)
+    _migrate_to_pdf_export_section(settings)
 
 
 def _migrate_layout_setting(settings: configparser.ConfigParser):
     try:
         gui_section = settings["gui"]
         layout = gui_section["search-widget-layout"]
     except KeyError:
@@ -449,10 +464,22 @@
         return
     section["row-spacing-mm"] = section["image-spacing-horizontal-mm"]
     section["column-spacing-mm"] = section["image-spacing-vertical-mm"]
     del section["image-spacing-horizontal-mm"]
     del section["image-spacing-vertical-mm"]
 
 
+def _migrate_to_pdf_export_section(to_migrate: configparser.ConfigParser):
+    section_name: str = "pdf-export"
+    if to_migrate.has_section(section_name):
+        return
+    to_migrate.add_section(section_name)
+    target = to_migrate[section_name]
+    target["pdf-page-count-limit"] = to_migrate["documents"]["pdf-page-count-limit"]
+    target["pdf-export-path"] = to_migrate["default-filesystem-paths"]["pdf-export-path"]
+    del to_migrate["documents"]["pdf-page-count-limit"]
+    del to_migrate["default-filesystem-paths"]["pdf-export-path"]
+
+
 # Read the settings from file during module import
 # This has to be performed before any modules containing GUI classes are imported.
 read_settings_from_file()
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/sqlite_helpers.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/add_card.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/add_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 from mtg_proxy_printer.ui.common import load_ui_from_file
 
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 try:
-    from mtg_proxy_printer.ui.generated.add_card_widget.vertical import Ui_AddCardWidget_Vertical
-    from mtg_proxy_printer.ui.generated.add_card_widget.horizontal import Ui_AddCardWidget_Horizontal
+    from mtg_proxy_printer.ui.generated.add_card_widget.vertical import Ui_VerticalAddCardWidget
+    from mtg_proxy_printer.ui.generated.add_card_widget.horizontal import Ui_HorizontalAddCardWidget
 except ModuleNotFoundError:
-    Ui_AddCardWidget_Vertical = load_ui_from_file("add_card_widget/vertical")
-    Ui_AddCardWidget_Horizontal = load_ui_from_file("add_card_widget/horizontal")
+    Ui_VerticalAddCardWidget = load_ui_from_file("add_card_widget/vertical")
+    Ui_HorizontalAddCardWidget = load_ui_from_file("add_card_widget/horizontal")
 
 
 __all__ = [
     "AddCardWidget",
     "VerticalAddCardWidget",
     "HorizontalAddCardWidget",
 ]
 
-UiTypes = Union[Type[Ui_AddCardWidget_Vertical], Type[Ui_AddCardWidget_Horizontal]]
+UiTypes = Union[Type[Ui_VerticalAddCardWidget], Type[Ui_HorizontalAddCardWidget]]
 StandardButton = QDialogButtonBox.StandardButton
 ItemDataRole = Qt.ItemDataRole
 
 
 class AddCardWidget(QWidget):
 
     request_action = Signal(ActionAddCard)
@@ -278,13 +278,13 @@
         else:
             return None
 
 
 class VerticalAddCardWidget(AddCardWidget):
 
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_AddCardWidget_Vertical, parent)
+        super().__init__(Ui_VerticalAddCardWidget, parent)
 
 
 class HorizontalAddCardWidget(AddCardWidget):
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_AddCardWidget_Horizontal, parent)
+        super().__init__(Ui_HorizontalAddCardWidget, parent)
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/central_widget.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/central_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,33 @@
 from mtg_proxy_printer.model.carddb import CardDatabase, Card, CardList, CheckCard, AnyCardType, AnyCardTypeForTypeCheck
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.document_controller import DocumentAction
 from mtg_proxy_printer.document_controller.card_actions import ActionRemoveCards, ActionAddCard
 from mtg_proxy_printer.ui.item_delegates import ComboBoxItemDelegate
 
 try:
-    from mtg_proxy_printer.ui.generated.central_widget.columnar import Ui_CentralWidget_Columnar
-    from mtg_proxy_printer.ui.generated.central_widget.grouped import Ui_CentralWidget_Grouped
-    from mtg_proxy_printer.ui.generated.central_widget.tabbed_vertical import Ui_CentralWidget_Tabbed
+    from mtg_proxy_printer.ui.generated.central_widget.columnar import Ui_ColumnarCentralWidget
+    from mtg_proxy_printer.ui.generated.central_widget.grouped import Ui_GroupedCentralWidget
+    from mtg_proxy_printer.ui.generated.central_widget.tabbed_vertical import Ui_TabbedCentralWidget
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
-    Ui_CentralWidget_Columnar = load_ui_from_file("central_widget/columnar")
-    Ui_CentralWidget_Grouped = load_ui_from_file("central_widget/grouped")
-    Ui_CentralWidget_Tabbed = load_ui_from_file("central_widget/tabbed_vertical")
+    Ui_ColumnarCentralWidget = load_ui_from_file("central_widget/columnar")
+    Ui_GroupedCentralWidget = load_ui_from_file("central_widget/grouped")
+    Ui_TabbedCentralWidget = load_ui_from_file("central_widget/tabbed_vertical")
 
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 
 __all__ = [
     "CentralWidget",
 ]
 
-UiType = Union[Type[Ui_CentralWidget_Grouped], Type[Ui_CentralWidget_Columnar], Type[Ui_CentralWidget_Tabbed]]
+UiType = Union[Type[Ui_GroupedCentralWidget], Type[Ui_ColumnarCentralWidget], Type[Ui_TabbedCentralWidget]]
 
 
 class CentralWidget(QWidget):
 
     request_action = Signal(DocumentAction)
     obtain_card_image = Signal(ActionAddCard)
 
@@ -282,11 +282,11 @@
             self.document.on_ui_selects_new_page(new_selection)
 
 
 def get_configured_central_widget_layout_class() -> UiType:
     gui_settings = mtg_proxy_printer.settings.settings["gui"]
     configured_layout = gui_settings["central-widget-layout"]
     if configured_layout == "horizontal":
-        return Ui_CentralWidget_Grouped
+        return Ui_GroupedCentralWidget
     if configured_layout == "columnar":
-        return Ui_CentralWidget_Columnar
-    return Ui_CentralWidget_Tabbed
+        return Ui_ColumnarCentralWidget
+    return Ui_TabbedCentralWidget
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/common.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     "format_size",
     "WizardBase",
 ]
 
 try:
     import mtg_proxy_printer.ui.compiled_resources
 except ModuleNotFoundError:
-    RESOURCE_PATH_PREFIX = str(pathlib.Path(__file__).resolve().parent.parent / "resources")
-    ICON_PATH_PREFIX = str(pathlib.Path(__file__).resolve().parent.parent / "resources" / "icons")
+    RESOURCE_PATH_PREFIX = str(pathlib.Path(__file__).resolve().parent.with_name("resources"))
+    ICON_PATH_PREFIX = str(pathlib.Path(__file__).resolve().parent.with_name("resources") / "icons")
     HAS_COMPILED_RESOURCES = False
 else:
     import atexit
     # Compiled resources found, so use it.
     RESOURCE_PATH_PREFIX = ":"
     ICON_PATH_PREFIX = ":/icons"
     HAS_COMPILED_RESOURCES = True
@@ -65,22 +65,22 @@
 
 
 class BlockedSignals:
     """
     Context manager used to temporarily prevent any QObject-derived object from emitting Qt signals.
     This can be used to break signal trigger loops or unwanted trigger chains.
     """
-    def __init__(self, qobject: QObject):
-        self.qobject = qobject
+    def __init__(self, qt_object: QObject):
+        self.qt_object = qt_object
 
     def __enter__(self):
-        self.qobject.blockSignals(True)
+        self.qt_object.blockSignals(True)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.qobject.blockSignals(False)
+        self.qt_object.blockSignals(False)
 
 
 def set_url_label(label: QLabel, path: pathlib.Path, display_text: str = None):
 
     url = QUrl.fromLocalFile(str(path.expanduser()))
     if not label.openExternalLinks():
         # The openExternalLinks property is not set in the UI file, so fail fast instead of doing workarounds.
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/compiled_resources.pyi` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/compiled_resources.pyi`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/deck_import_wizard.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/deck_import_wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 import re
 import typing
 import urllib.error
 
 from PyQt5.QtCore import pyqtSlot as Slot, pyqtSignal as Signal, pyqtProperty as Property, QStringListModel, Qt, \
     QItemSelection, QSize
 from PyQt5.QtGui import QValidator, QIcon
-from PyQt5.QtWidgets import QWizard, QFileDialog, QMessageBox, QWizardPage, QWidget
+from PyQt5.QtWidgets import QWizard, QFileDialog, QMessageBox, QWizardPage, QWidget, QRadioButton
 
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.decklist_parser import re_parsers, common, csv_parsers
 from mtg_proxy_printer.decklist_downloader import IsIdentifyingDeckUrlValidator, AVAILABLE_DOWNLOADERS, \
-    get_downloader_class
+    get_downloader_class, ParserBase
 from mtg_proxy_printer.model.carddb import CardDatabase
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.model.card_list import CardListModel, PageColumns
 from mtg_proxy_printer.natsort import NaturallySortedSortFilterProxyModel
 from mtg_proxy_printer.ui.common import load_ui_from_file, format_size, WizardBase
 from mtg_proxy_printer.ui.item_delegates import ComboBoxItemDelegate
 from mtg_proxy_printer.document_controller.import_deck_list import ActionImportDeckList
@@ -333,25 +333,27 @@
         self.ui.select_parser_custom_re.clicked.connect(
             lambda: setattr(self, "parser_creator", self._create_generic_re_parser)
         )
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     def initializePage(self) -> None:
         super().initializePage()
+        ui = self.ui
         used_downloader: str = self.field("deck-list-downloaded")
         if used_downloader:
             parser_to_use = AVAILABLE_DOWNLOADERS[used_downloader].PARSER_CLASS
-            {
-                re_parsers.MagicWorkstationDeckDataFormatParser: self.ui.select_parser_magic_workstation,
-                re_parsers.MTGArenaParser: self.ui.select_parser_mtg_arena,
-                re_parsers.MTGOnlineParser: self.ui.select_parser_mtg_online,
-                re_parsers.XMageParser: self.ui.select_parser_xmage,
-                csv_parsers.ScryfallCSVParser: self.ui.select_parser_scryfall_csv,
-                csv_parsers.TappedOutCSVParser: self.ui.select_parser_tappedout_csv,
-            }[parser_to_use].click()
+            parser_table: typing.Dict[typing.Type[ParserBase], QRadioButton] = {
+                re_parsers.MagicWorkstationDeckDataFormatParser: ui.select_parser_magic_workstation,
+                re_parsers.MTGArenaParser: ui.select_parser_mtg_arena,
+                re_parsers.MTGOnlineParser: ui.select_parser_mtg_online,
+                re_parsers.XMageParser: ui.select_parser_xmage,
+                csv_parsers.ScryfallCSVParser: ui.select_parser_scryfall_csv,
+                csv_parsers.TappedOutCSVParser: ui.select_parser_tappedout_csv,
+            }
+            parser_table[parser_to_use].click()
 
     def append_group_to_custom_re_input(self, value: str):
         self.ui.custom_re_input.setText(self.ui.custom_re_input.text()+value)
 
     def _create_magic_workstation_parser(self):
         self.selected_parser = re_parsers.MagicWorkstationDeckDataFormatParser(self.card_db, self.image_db, self)
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/dialogs.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,37 +46,38 @@
 logger = get_logger(__name__)
 del get_logger
 
 __all__ = [
     "SavePDFDialog",
     "SaveDocumentAsDialog",
     "LoadDocumentDialog",
-    "AboutMTGProxyPrinterDialog",
+    "AboutDialog",
     "PrintPreviewDialog",
     "PrintDialog",
     "DocumentSettingsDialog",
 ]
 
 
-def read_path(setting: str) -> str:
-    stored = mtg_proxy_printer.settings.settings["default-filesystem-paths"][setting]
+def read_path(section: str, setting: str) -> str:
+    stored = mtg_proxy_printer.settings.settings[section][setting]
     if not stored:
         return ""
     resolved = str(pathlib.Path(stored).resolve())
     if not resolved:
-        logger.warning(f"File system path stored in setting {setting} does not resolve to an existing path")
+        logger.warning(
+            f"File system path stored in section {section} setting {setting} does not resolve to an existing path")
     return resolved
 
 
 class SavePDFDialog(QFileDialog):
 
     def __init__(self, parent: QWidget, document: mtg_proxy_printer.model.document.Document):
         super().__init__(
             parent, "Export as PDF", self.get_preferred_file_name(document), "PDF-Documents (*.pdf)")
-        if default_path := read_path("pdf-export-path"):
+        if default_path := read_path("pdf-export", "pdf-export-path"):
             self.setDirectory(default_path)
         self.document = document
         self.setAcceptMode(QFileDialog.AcceptMode.AcceptSave)
         self.setDefaultSuffix("pdf")
         self.setFileMode(QFileDialog.FileMode.AnyFile)
         self.accepted.connect(self.on_accept)
         self.rejected.connect(self.on_reject)
@@ -106,15 +107,15 @@
 
 
 class SaveDocumentAsDialog(QFileDialog):
 
     def __init__(self, document: mtg_proxy_printer.model.document.Document, parent: QWidget = None, **kwargs):
         super().__init__(
             parent, "Save document as …", filter=f"MTGProxyPrinter document (*.{DEFAULT_SAVE_SUFFIX})", **kwargs)
-        if default_path := read_path("document-save-path"):
+        if default_path := read_path("default-filesystem-paths", "document-save-path"):
             self.setDirectory(default_path)
         self.document = document
         self.setAcceptMode(QFileDialog.AcceptMode.AcceptSave)
         self.setDefaultSuffix(DEFAULT_SAVE_SUFFIX)
         self.setFileMode(QFileDialog.FileMode.AnyFile)
         self.accepted.connect(self.on_accept)
         self.rejected.connect(self.on_reject)
@@ -136,15 +137,15 @@
 
     def __init__(
             self, parent: QWidget,
             document: mtg_proxy_printer.model.document.Document, **kwargs):
         super().__init__(
             parent, "Load MTGProxyPrinter document", filter=f"MTGProxyPrinter document (*.{DEFAULT_SAVE_SUFFIX})",
             **kwargs)
-        if default_path := read_path("document-save-path"):
+        if default_path := read_path("default-filesystem-paths", "document-save-path"):
             self.setDirectory(default_path)
         self.document = document
         self.setAcceptMode(QFileDialog.AcceptMode.AcceptOpen)
         self.setDefaultSuffix(DEFAULT_SAVE_SUFFIX)
         self.setFileMode(QFileDialog.FileMode.ExistingFile)
         self.accepted.connect(self.on_accept)
         self.rejected.connect(self.on_reject)
@@ -158,15 +159,15 @@
         logger.info(f"Requested loading document from {path}")
 
     @Slot()
     def on_reject(self):
         logger.debug("User aborted loading. Doing nothing.")
 
 
-class AboutMTGProxyPrinterDialog(QDialog):
+class AboutDialog(QDialog):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ui = Ui_AboutDialog()
         self.ui.setupUi(self)
         self._setup_about_text()
         self._setup_changelog_text()
@@ -249,22 +250,22 @@
 
 class HoverEventFilter(QObject):
     def __init__(self, settings: configparser.ConfigParser, parent: "DocumentSettingsDialog"):
         super().__init__(parent)
         self.settings = settings
 
     def eventFilter(self, object_, event: QEvent):
-        event_type = event.type()
+        event_type: QEvent.Type = event.type()
         # This check avoids a crash during application shutdown
-        if event_type not in {QEvent.HoverEnter, QEvent.HoverLeave}:
+        if event_type not in {QEvent.Type.HoverEnter, QEvent.Type.HoverLeave}:
             return False
         parent: "DocumentSettingsDialog" = self.parent()
-        if event_type == QEvent.HoverEnter:
+        if event_type == QEvent.Type.HoverEnter:
             parent.ui.page_config_groupbox.highlight_differing_settings(self.settings)
-        elif event_type == QEvent.HoverLeave:
+        elif event_type == QEvent.Type.HoverLeave:
             parent.clear_highlight()
         return False
 
 
 class DocumentSettingsDialog(QDialog):
 
     def __init__(self, document: mtg_proxy_printer.model.document.Document, parent: QWidget = None):
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/about_dialog.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,125 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_AddCardWidget_Horizontal(object):
-    def setupUi(self, AddCardWidget_Horizontal):
-        AddCardWidget_Horizontal.setObjectName("AddCardWidget_Horizontal")
-        AddCardWidget_Horizontal.resize(1242, 292)
-        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget_Horizontal)
-        self.gridLayout.setContentsMargins(0, 0, 0, 0)
+class Ui_VerticalAddCardWidget(object):
+    def setupUi(self, VerticalAddCardWidget):
+        VerticalAddCardWidget.setObjectName("VerticalAddCardWidget")
+        VerticalAddCardWidget.resize(349, 715)
+        self.gridLayout = QtWidgets.QGridLayout(VerticalAddCardWidget)
         self.gridLayout.setObjectName("gridLayout")
-        self.language_label = QtWidgets.QLabel(AddCardWidget_Horizontal)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
-        self.language_label.setSizePolicy(sizePolicy)
-        self.language_label.setObjectName("language_label")
-        self.gridLayout.addWidget(self.language_label, 7, 5, 1, 1)
-        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
-        sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
-        self.card_name_box.setSizePolicy(sizePolicy)
-        self.card_name_box.setObjectName("card_name_box")
-        self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.card_name_filter = QtWidgets.QLineEdit(self.card_name_box)
-        self.card_name_filter.setClearButtonEnabled(True)
-        self.card_name_filter.setObjectName("card_name_filter")
-        self.verticalLayout.addWidget(self.card_name_filter)
-        self.card_name_list = QtWidgets.QListView(self.card_name_box)
-        self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self.card_name_list.setAlternatingRowColors(True)
-        self.card_name_list.setObjectName("card_name_list")
-        self.verticalLayout.addWidget(self.card_name_list)
-        self.gridLayout.addWidget(self.card_name_box, 7, 1, 9, 1)
-        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
+        self.set_name_box = QtWidgets.QGroupBox(VerticalAddCardWidget)
         self.set_name_box.setEnabled(False)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
-        sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(0)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(7)
         sizePolicy.setHeightForWidth(self.set_name_box.sizePolicy().hasHeightForWidth())
         self.set_name_box.setSizePolicy(sizePolicy)
         self.set_name_box.setObjectName("set_name_box")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.set_name_box)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.set_name_filter = QtWidgets.QLineEdit(self.set_name_box)
         self.set_name_filter.setClearButtonEnabled(True)
         self.set_name_filter.setObjectName("set_name_filter")
         self.verticalLayout_2.addWidget(self.set_name_filter)
         self.set_name_list = QtWidgets.QListView(self.set_name_box)
         self.set_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.set_name_list.setAlternatingRowColors(True)
         self.set_name_list.setObjectName("set_name_list")
         self.verticalLayout_2.addWidget(self.set_name_list)
-        self.gridLayout.addWidget(self.set_name_box, 7, 2, 9, 1)
-        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
+        self.gridLayout.addWidget(self.set_name_box, 3, 0, 1, 3)
+        self.collector_number_box = QtWidgets.QGroupBox(VerticalAddCardWidget)
         self.collector_number_box.setEnabled(False)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
-        sizePolicy.setHorizontalStretch(5)
-        sizePolicy.setVerticalStretch(0)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(2)
         sizePolicy.setHeightForWidth(self.collector_number_box.sizePolicy().hasHeightForWidth())
         self.collector_number_box.setSizePolicy(sizePolicy)
         self.collector_number_box.setObjectName("collector_number_box")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.collector_number_box)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.collector_number_list = QtWidgets.QListView(self.collector_number_box)
         self.collector_number_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.collector_number_list.setAlternatingRowColors(True)
         self.collector_number_list.setObjectName("collector_number_list")
         self.verticalLayout_3.addWidget(self.collector_number_list)
-        self.gridLayout.addWidget(self.collector_number_box, 7, 3, 9, 1)
-        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget_Horizontal)
+        self.gridLayout.addWidget(self.collector_number_box, 10, 0, 1, 3)
+        self.card_name_box = QtWidgets.QGroupBox(VerticalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(7)
+        sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
+        self.card_name_box.setSizePolicy(sizePolicy)
+        self.card_name_box.setObjectName("card_name_box")
+        self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.card_name_filter = QtWidgets.QLineEdit(self.card_name_box)
+        self.card_name_filter.setClearButtonEnabled(True)
+        self.card_name_filter.setObjectName("card_name_filter")
+        self.verticalLayout.addWidget(self.card_name_filter)
+        self.card_name_list = QtWidgets.QListView(self.card_name_box)
+        self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.card_name_list.setAlternatingRowColors(True)
+        self.card_name_list.setObjectName("card_name_list")
+        self.verticalLayout.addWidget(self.card_name_list)
+        self.gridLayout.addWidget(self.card_name_box, 2, 0, 1, 3)
+        self.language_combo_box = QtWidgets.QComboBox(VerticalAddCardWidget)
         self.language_combo_box.setObjectName("language_combo_box")
-        self.gridLayout.addWidget(self.language_combo_box, 8, 5, 1, 1)
-        self.copies_label = QtWidgets.QLabel(AddCardWidget_Horizontal)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        self.gridLayout.addWidget(self.language_combo_box, 0, 1, 1, 2)
+        self.language_label = QtWidgets.QLabel(VerticalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
+        self.language_label.setSizePolicy(sizePolicy)
+        self.language_label.setObjectName("language_label")
+        self.gridLayout.addWidget(self.language_label, 0, 0, 1, 1)
+        self.copies_label = QtWidgets.QLabel(VerticalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.copies_label.sizePolicy().hasHeightForWidth())
         self.copies_label.setSizePolicy(sizePolicy)
         self.copies_label.setObjectName("copies_label")
-        self.gridLayout.addWidget(self.copies_label, 9, 5, 1, 1)
-        self.copies_input = QtWidgets.QSpinBox(AddCardWidget_Horizontal)
+        self.gridLayout.addWidget(self.copies_label, 11, 0, 1, 1)
+        self.copies_input = QtWidgets.QSpinBox(VerticalAddCardWidget)
         self.copies_input.setMinimum(1)
         self.copies_input.setObjectName("copies_input")
-        self.gridLayout.addWidget(self.copies_input, 10, 5, 1, 1)
-        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget_Horizontal)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.button_box.sizePolicy().hasHeightForWidth())
-        self.button_box.setSizePolicy(sizePolicy)
-        self.button_box.setOrientation(QtCore.Qt.Vertical)
+        self.gridLayout.addWidget(self.copies_input, 11, 1, 1, 2)
+        self.button_box = QtWidgets.QDialogButtonBox(VerticalAddCardWidget)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Ok|QtWidgets.QDialogButtonBox.Reset)
         self.button_box.setObjectName("button_box")
-        self.gridLayout.addWidget(self.button_box, 11, 5, 5, 1)
+        self.gridLayout.addWidget(self.button_box, 12, 0, 1, 3)
         self.language_label.setBuddy(self.language_combo_box)
         self.copies_label.setBuddy(self.copies_input)
 
-        self.retranslateUi(AddCardWidget_Horizontal)
-        QtCore.QMetaObject.connectSlotsByName(AddCardWidget_Horizontal)
-        AddCardWidget_Horizontal.setTabOrder(self.card_name_filter, self.card_name_list)
-        AddCardWidget_Horizontal.setTabOrder(self.card_name_list, self.set_name_filter)
-        AddCardWidget_Horizontal.setTabOrder(self.set_name_filter, self.set_name_list)
-        AddCardWidget_Horizontal.setTabOrder(self.set_name_list, self.collector_number_list)
-        AddCardWidget_Horizontal.setTabOrder(self.collector_number_list, self.language_combo_box)
-        AddCardWidget_Horizontal.setTabOrder(self.language_combo_box, self.copies_input)
+        self.retranslateUi(VerticalAddCardWidget)
+        QtCore.QMetaObject.connectSlotsByName(VerticalAddCardWidget)
+        VerticalAddCardWidget.setTabOrder(self.language_combo_box, self.card_name_filter)
+        VerticalAddCardWidget.setTabOrder(self.card_name_filter, self.card_name_list)
+        VerticalAddCardWidget.setTabOrder(self.card_name_list, self.set_name_filter)
+        VerticalAddCardWidget.setTabOrder(self.set_name_filter, self.set_name_list)
+        VerticalAddCardWidget.setTabOrder(self.set_name_list, self.collector_number_list)
+        VerticalAddCardWidget.setTabOrder(self.collector_number_list, self.copies_input)
 
-    def retranslateUi(self, AddCardWidget_Horizontal):
+    def retranslateUi(self, VerticalAddCardWidget):
         _translate = QtCore.QCoreApplication.translate
-        self.language_label.setText(_translate("AddCardWidget_Horizontal", "Language:"))
-        self.card_name_box.setTitle(_translate("AddCardWidget_Horizontal", "Card Name"))
-        self.card_name_filter.setToolTip(_translate("AddCardWidget_Horizontal", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
-        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget_Horizontal", "Filter card names"))
-        self.card_name_list.setToolTip(_translate("AddCardWidget_Horizontal", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
-        self.set_name_box.setToolTip(_translate("AddCardWidget_Horizontal", "The sets in which the currently selected card was printed."))
-        self.set_name_box.setTitle(_translate("AddCardWidget_Horizontal", "Set"))
-        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget_Horizontal", "Filter set names"))
-        self.collector_number_box.setTitle(_translate("AddCardWidget_Horizontal", "Collector Number"))
-        self.copies_label.setText(_translate("AddCardWidget_Horizontal", "Copies"))
+        self.set_name_box.setToolTip(_translate("VerticalAddCardWidget", "The sets in which the currently selected card was printed."))
+        self.set_name_box.setTitle(_translate("VerticalAddCardWidget", "Set"))
+        self.set_name_filter.setPlaceholderText(_translate("VerticalAddCardWidget", "Filter set names"))
+        self.collector_number_box.setTitle(_translate("VerticalAddCardWidget", "Collector Number"))
+        self.card_name_box.setTitle(_translate("VerticalAddCardWidget", "Card Name"))
+        self.card_name_filter.setToolTip(_translate("VerticalAddCardWidget", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
+        self.card_name_filter.setPlaceholderText(_translate("VerticalAddCardWidget", "Filter card names"))
+        self.card_name_list.setToolTip(_translate("VerticalAddCardWidget", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
+        self.language_label.setText(_translate("VerticalAddCardWidget", "Language:"))
+        self.copies_label.setText(_translate("VerticalAddCardWidget", "Copies:"))
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,132 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_AddCardWidget_Vertical(object):
-    def setupUi(self, AddCardWidget_Vertical):
-        AddCardWidget_Vertical.setObjectName("AddCardWidget_Vertical")
-        AddCardWidget_Vertical.resize(349, 715)
-        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget_Vertical)
+class Ui_HorizontalAddCardWidget(object):
+    def setupUi(self, HorizontalAddCardWidget):
+        HorizontalAddCardWidget.setObjectName("HorizontalAddCardWidget")
+        HorizontalAddCardWidget.resize(1242, 292)
+        self.gridLayout = QtWidgets.QGridLayout(HorizontalAddCardWidget)
+        self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
-        self.set_name_box.setEnabled(False)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        self.language_label = QtWidgets.QLabel(HorizontalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(7)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
+        self.language_label.setSizePolicy(sizePolicy)
+        self.language_label.setObjectName("language_label")
+        self.gridLayout.addWidget(self.language_label, 7, 5, 1, 1)
+        self.card_name_box = QtWidgets.QGroupBox(HorizontalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(7)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
+        self.card_name_box.setSizePolicy(sizePolicy)
+        self.card_name_box.setObjectName("card_name_box")
+        self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.card_name_filter = QtWidgets.QLineEdit(self.card_name_box)
+        self.card_name_filter.setClearButtonEnabled(True)
+        self.card_name_filter.setObjectName("card_name_filter")
+        self.verticalLayout.addWidget(self.card_name_filter)
+        self.card_name_list = QtWidgets.QListView(self.card_name_box)
+        self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.card_name_list.setAlternatingRowColors(True)
+        self.card_name_list.setObjectName("card_name_list")
+        self.verticalLayout.addWidget(self.card_name_list)
+        self.gridLayout.addWidget(self.card_name_box, 7, 1, 9, 1)
+        self.set_name_box = QtWidgets.QGroupBox(HorizontalAddCardWidget)
+        self.set_name_box.setEnabled(False)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(7)
+        sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.set_name_box.sizePolicy().hasHeightForWidth())
         self.set_name_box.setSizePolicy(sizePolicy)
         self.set_name_box.setObjectName("set_name_box")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.set_name_box)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.set_name_filter = QtWidgets.QLineEdit(self.set_name_box)
         self.set_name_filter.setClearButtonEnabled(True)
         self.set_name_filter.setObjectName("set_name_filter")
         self.verticalLayout_2.addWidget(self.set_name_filter)
         self.set_name_list = QtWidgets.QListView(self.set_name_box)
         self.set_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.set_name_list.setAlternatingRowColors(True)
         self.set_name_list.setObjectName("set_name_list")
         self.verticalLayout_2.addWidget(self.set_name_list)
-        self.gridLayout.addWidget(self.set_name_box, 3, 0, 1, 3)
-        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
+        self.gridLayout.addWidget(self.set_name_box, 7, 2, 9, 1)
+        self.collector_number_box = QtWidgets.QGroupBox(HorizontalAddCardWidget)
         self.collector_number_box.setEnabled(False)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(5)
+        sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.collector_number_box.sizePolicy().hasHeightForWidth())
         self.collector_number_box.setSizePolicy(sizePolicy)
         self.collector_number_box.setObjectName("collector_number_box")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.collector_number_box)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.collector_number_list = QtWidgets.QListView(self.collector_number_box)
         self.collector_number_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.collector_number_list.setAlternatingRowColors(True)
         self.collector_number_list.setObjectName("collector_number_list")
         self.verticalLayout_3.addWidget(self.collector_number_list)
-        self.gridLayout.addWidget(self.collector_number_box, 10, 0, 1, 3)
-        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(7)
-        sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
-        self.card_name_box.setSizePolicy(sizePolicy)
-        self.card_name_box.setObjectName("card_name_box")
-        self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.card_name_filter = QtWidgets.QLineEdit(self.card_name_box)
-        self.card_name_filter.setClearButtonEnabled(True)
-        self.card_name_filter.setObjectName("card_name_filter")
-        self.verticalLayout.addWidget(self.card_name_filter)
-        self.card_name_list = QtWidgets.QListView(self.card_name_box)
-        self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self.card_name_list.setAlternatingRowColors(True)
-        self.card_name_list.setObjectName("card_name_list")
-        self.verticalLayout.addWidget(self.card_name_list)
-        self.gridLayout.addWidget(self.card_name_box, 2, 0, 1, 3)
-        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget_Vertical)
+        self.gridLayout.addWidget(self.collector_number_box, 7, 3, 9, 1)
+        self.language_combo_box = QtWidgets.QComboBox(HorizontalAddCardWidget)
         self.language_combo_box.setObjectName("language_combo_box")
-        self.gridLayout.addWidget(self.language_combo_box, 0, 1, 1, 2)
-        self.language_label = QtWidgets.QLabel(AddCardWidget_Vertical)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
-        self.language_label.setSizePolicy(sizePolicy)
-        self.language_label.setObjectName("language_label")
-        self.gridLayout.addWidget(self.language_label, 0, 0, 1, 1)
-        self.copies_label = QtWidgets.QLabel(AddCardWidget_Vertical)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        self.gridLayout.addWidget(self.language_combo_box, 8, 5, 1, 1)
+        self.copies_label = QtWidgets.QLabel(HorizontalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.copies_label.sizePolicy().hasHeightForWidth())
         self.copies_label.setSizePolicy(sizePolicy)
         self.copies_label.setObjectName("copies_label")
-        self.gridLayout.addWidget(self.copies_label, 11, 0, 1, 1)
-        self.copies_input = QtWidgets.QSpinBox(AddCardWidget_Vertical)
+        self.gridLayout.addWidget(self.copies_label, 9, 5, 1, 1)
+        self.copies_input = QtWidgets.QSpinBox(HorizontalAddCardWidget)
         self.copies_input.setMinimum(1)
         self.copies_input.setObjectName("copies_input")
-        self.gridLayout.addWidget(self.copies_input, 11, 1, 1, 2)
-        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget_Vertical)
+        self.gridLayout.addWidget(self.copies_input, 10, 5, 1, 1)
+        self.button_box = QtWidgets.QDialogButtonBox(HorizontalAddCardWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.button_box.sizePolicy().hasHeightForWidth())
+        self.button_box.setSizePolicy(sizePolicy)
+        self.button_box.setOrientation(QtCore.Qt.Vertical)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Ok|QtWidgets.QDialogButtonBox.Reset)
         self.button_box.setObjectName("button_box")
-        self.gridLayout.addWidget(self.button_box, 12, 0, 1, 3)
+        self.gridLayout.addWidget(self.button_box, 11, 5, 5, 1)
         self.language_label.setBuddy(self.language_combo_box)
         self.copies_label.setBuddy(self.copies_input)
 
-        self.retranslateUi(AddCardWidget_Vertical)
-        QtCore.QMetaObject.connectSlotsByName(AddCardWidget_Vertical)
-        AddCardWidget_Vertical.setTabOrder(self.language_combo_box, self.card_name_filter)
-        AddCardWidget_Vertical.setTabOrder(self.card_name_filter, self.card_name_list)
-        AddCardWidget_Vertical.setTabOrder(self.card_name_list, self.set_name_filter)
-        AddCardWidget_Vertical.setTabOrder(self.set_name_filter, self.set_name_list)
-        AddCardWidget_Vertical.setTabOrder(self.set_name_list, self.collector_number_list)
-        AddCardWidget_Vertical.setTabOrder(self.collector_number_list, self.copies_input)
+        self.retranslateUi(HorizontalAddCardWidget)
+        QtCore.QMetaObject.connectSlotsByName(HorizontalAddCardWidget)
+        HorizontalAddCardWidget.setTabOrder(self.card_name_filter, self.card_name_list)
+        HorizontalAddCardWidget.setTabOrder(self.card_name_list, self.set_name_filter)
+        HorizontalAddCardWidget.setTabOrder(self.set_name_filter, self.set_name_list)
+        HorizontalAddCardWidget.setTabOrder(self.set_name_list, self.collector_number_list)
+        HorizontalAddCardWidget.setTabOrder(self.collector_number_list, self.language_combo_box)
+        HorizontalAddCardWidget.setTabOrder(self.language_combo_box, self.copies_input)
 
-    def retranslateUi(self, AddCardWidget_Vertical):
+    def retranslateUi(self, HorizontalAddCardWidget):
         _translate = QtCore.QCoreApplication.translate
-        self.set_name_box.setToolTip(_translate("AddCardWidget_Vertical", "The sets in which the currently selected card was printed."))
-        self.set_name_box.setTitle(_translate("AddCardWidget_Vertical", "Set"))
-        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget_Vertical", "Filter set names"))
-        self.collector_number_box.setTitle(_translate("AddCardWidget_Vertical", "Collector Number"))
-        self.card_name_box.setTitle(_translate("AddCardWidget_Vertical", "Card Name"))
-        self.card_name_filter.setToolTip(_translate("AddCardWidget_Vertical", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
-        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget_Vertical", "Filter card names"))
-        self.card_name_list.setToolTip(_translate("AddCardWidget_Vertical", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
-        self.language_label.setText(_translate("AddCardWidget_Vertical", "Language:"))
-        self.copies_label.setText(_translate("AddCardWidget_Vertical", "Copies:"))
+        self.language_label.setText(_translate("HorizontalAddCardWidget", "Language:"))
+        self.card_name_box.setTitle(_translate("HorizontalAddCardWidget", "Card Name"))
+        self.card_name_filter.setToolTip(_translate("HorizontalAddCardWidget", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
+        self.card_name_filter.setPlaceholderText(_translate("HorizontalAddCardWidget", "Filter card names"))
+        self.card_name_list.setToolTip(_translate("HorizontalAddCardWidget", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
+        self.set_name_box.setToolTip(_translate("HorizontalAddCardWidget", "The sets in which the currently selected card was printed."))
+        self.set_name_box.setTitle(_translate("HorizontalAddCardWidget", "Set"))
+        self.set_name_filter.setPlaceholderText(_translate("HorizontalAddCardWidget", "Filter set names"))
+        self.collector_number_box.setTitle(_translate("HorizontalAddCardWidget", "Collector Number"))
+        self.copies_label.setText(_translate("HorizontalAddCardWidget", "Copies"))
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,86 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/columnar.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/grouped.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_CentralWidget_Columnar(object):
-    def setupUi(self, CentralWidget_Columnar):
-        CentralWidget_Columnar.setObjectName("CentralWidget_Columnar")
-        CentralWidget_Columnar.resize(888, 258)
-        self.gridLayout = QtWidgets.QGridLayout(CentralWidget_Columnar)
+class Ui_GroupedCentralWidget(object):
+    def setupUi(self, GroupedCentralWidget):
+        GroupedCentralWidget.setObjectName("GroupedCentralWidget")
+        GroupedCentralWidget.resize(580, 539)
+        self.gridLayout = QtWidgets.QGridLayout(GroupedCentralWidget)
         self.gridLayout.setContentsMargins(-1, -1, -1, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.page_renderer = PageRenderer(CentralWidget_Columnar)
+        self.page_renderer = PageRenderer(GroupedCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(9)
-        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setHorizontalStretch(7)
+        sizePolicy.setVerticalStretch(10)
         sizePolicy.setHeightForWidth(self.page_renderer.sizePolicy().hasHeightForWidth())
         self.page_renderer.setSizePolicy(sizePolicy)
         self.page_renderer.setAcceptDrops(False)
         self.page_renderer.setRenderHints(QtGui.QPainter.Antialiasing|QtGui.QPainter.HighQualityAntialiasing)
         self.page_renderer.setObjectName("page_renderer")
-        self.gridLayout.addWidget(self.page_renderer, 4, 3, 3, 1)
-        self.page_card_table_view = QtWidgets.QTableView(CentralWidget_Columnar)
+        self.gridLayout.addWidget(self.page_renderer, 5, 3, 3, 1)
+        self.document_view = QtWidgets.QListView(GroupedCentralWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(3)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
+        self.document_view.setSizePolicy(sizePolicy)
+        self.document_view.setAlternatingRowColors(True)
+        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
+        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
+        self.document_view.setObjectName("document_view")
+        self.gridLayout.addWidget(self.document_view, 1, 0, 7, 2)
+        self.delete_selected_images_button = QtWidgets.QPushButton(GroupedCentralWidget)
+        self.delete_selected_images_button.setEnabled(False)
+        icon = QtGui.QIcon.fromTheme("edit-delete")
+        self.delete_selected_images_button.setIcon(icon)
+        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
+        self.gridLayout.addWidget(self.delete_selected_images_button, 7, 2, 1, 1)
+        self.page_card_table_view = QtWidgets.QTableView(GroupedCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(9)
-        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setHorizontalStretch(8)
+        sizePolicy.setVerticalStretch(10)
         sizePolicy.setHeightForWidth(self.page_card_table_view.sizePolicy().hasHeightForWidth())
         self.page_card_table_view.setSizePolicy(sizePolicy)
         self.page_card_table_view.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.page_card_table_view.setLineWidth(0)
         self.page_card_table_view.setAlternatingRowColors(True)
         self.page_card_table_view.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.page_card_table_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.page_card_table_view.setObjectName("page_card_table_view")
         self.page_card_table_view.verticalHeader().setVisible(False)
-        self.gridLayout.addWidget(self.page_card_table_view, 4, 2, 2, 1)
-        self.document_view_label = QtWidgets.QLabel(CentralWidget_Columnar)
-        self.document_view_label.setObjectName("document_view_label")
-        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 1)
-        self.page_view_label = QtWidgets.QLabel(CentralWidget_Columnar)
-        self.page_view_label.setObjectName("page_view_label")
-        self.gridLayout.addWidget(self.page_view_label, 0, 2, 1, 2)
-        self.delete_selected_images_button = QtWidgets.QPushButton(CentralWidget_Columnar)
-        self.delete_selected_images_button.setEnabled(False)
-        icon = QtGui.QIcon.fromTheme("edit-delete")
-        self.delete_selected_images_button.setIcon(icon)
-        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
-        self.gridLayout.addWidget(self.delete_selected_images_button, 6, 2, 1, 1)
-        self.add_card_widget_label = QtWidgets.QLabel(CentralWidget_Columnar)
-        self.add_card_widget_label.setObjectName("add_card_widget_label")
-        self.gridLayout.addWidget(self.add_card_widget_label, 0, 1, 1, 1)
-        self.add_card_widget = VerticalAddCardWidget(CentralWidget_Columnar)
+        self.gridLayout.addWidget(self.page_card_table_view, 5, 2, 2, 1)
+        self.add_card_widget = HorizontalAddCardWidget(GroupedCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setVerticalStretch(6)
         sizePolicy.setHeightForWidth(self.add_card_widget.sizePolicy().hasHeightForWidth())
         self.add_card_widget.setSizePolicy(sizePolicy)
         self.add_card_widget.setObjectName("add_card_widget")
-        self.gridLayout.addWidget(self.add_card_widget, 4, 1, 3, 1)
-        self.document_view = QtWidgets.QListView(CentralWidget_Columnar)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(4)
-        sizePolicy.setVerticalStretch(1)
-        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
-        self.document_view.setSizePolicy(sizePolicy)
-        self.document_view.setAlternatingRowColors(True)
-        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
-        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
-        self.document_view.setObjectName("document_view")
-        self.gridLayout.addWidget(self.document_view, 4, 0, 3, 1)
+        self.gridLayout.addWidget(self.add_card_widget, 1, 2, 2, 2)
+        self.document_view_label = QtWidgets.QLabel(GroupedCentralWidget)
+        self.document_view_label.setObjectName("document_view_label")
+        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 2)
+        self.add_card_widget_label = QtWidgets.QLabel(GroupedCentralWidget)
+        self.add_card_widget_label.setObjectName("add_card_widget_label")
+        self.gridLayout.addWidget(self.add_card_widget_label, 0, 2, 1, 2)
 
-        self.retranslateUi(CentralWidget_Columnar)
-        QtCore.QMetaObject.connectSlotsByName(CentralWidget_Columnar)
+        self.retranslateUi(GroupedCentralWidget)
+        QtCore.QMetaObject.connectSlotsByName(GroupedCentralWidget)
 
-    def retranslateUi(self, CentralWidget_Columnar):
+    def retranslateUi(self, GroupedCentralWidget):
         _translate = QtCore.QCoreApplication.translate
-        self.document_view_label.setText(_translate("CentralWidget_Columnar", "All pages:"))
-        self.page_view_label.setText(_translate("CentralWidget_Columnar", "Current page:"))
-        self.delete_selected_images_button.setText(_translate("CentralWidget_Columnar", "Remove selected"))
-        self.add_card_widget_label.setText(_translate("CentralWidget_Columnar", "Add new cards:"))
-from mtg_proxy_printer.ui.add_card import VerticalAddCardWidget
+        self.delete_selected_images_button.setText(_translate("GroupedCentralWidget", "Remove selected"))
+        self.document_view_label.setText(_translate("GroupedCentralWidget", "All pages:"))
+        self.add_card_widget_label.setText(_translate("GroupedCentralWidget", "Add new cards:"))
+from mtg_proxy_printer.ui.add_card import HorizontalAddCardWidget
 from mtg_proxy_printer.ui.page_renderer import PageRenderer
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/grouped.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/columnar.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_CentralWidget_Grouped(object):
-    def setupUi(self, CentralWidget_Grouped):
-        CentralWidget_Grouped.setObjectName("CentralWidget_Grouped")
-        CentralWidget_Grouped.resize(580, 539)
-        self.gridLayout = QtWidgets.QGridLayout(CentralWidget_Grouped)
+class Ui_ColumnarCentralWidget(object):
+    def setupUi(self, ColumnarCentralWidget):
+        ColumnarCentralWidget.setObjectName("ColumnarCentralWidget")
+        ColumnarCentralWidget.resize(888, 258)
+        self.gridLayout = QtWidgets.QGridLayout(ColumnarCentralWidget)
         self.gridLayout.setContentsMargins(-1, -1, -1, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.page_renderer = PageRenderer(CentralWidget_Grouped)
+        self.page_renderer = PageRenderer(ColumnarCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(10)
+        sizePolicy.setHorizontalStretch(9)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.page_renderer.sizePolicy().hasHeightForWidth())
         self.page_renderer.setSizePolicy(sizePolicy)
         self.page_renderer.setAcceptDrops(False)
         self.page_renderer.setRenderHints(QtGui.QPainter.Antialiasing|QtGui.QPainter.HighQualityAntialiasing)
         self.page_renderer.setObjectName("page_renderer")
-        self.gridLayout.addWidget(self.page_renderer, 5, 3, 3, 1)
-        self.document_view = QtWidgets.QListView(CentralWidget_Grouped)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(3)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
-        self.document_view.setSizePolicy(sizePolicy)
-        self.document_view.setAlternatingRowColors(True)
-        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
-        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
-        self.document_view.setObjectName("document_view")
-        self.gridLayout.addWidget(self.document_view, 1, 0, 7, 2)
-        self.delete_selected_images_button = QtWidgets.QPushButton(CentralWidget_Grouped)
-        self.delete_selected_images_button.setEnabled(False)
-        icon = QtGui.QIcon.fromTheme("edit-delete")
-        self.delete_selected_images_button.setIcon(icon)
-        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
-        self.gridLayout.addWidget(self.delete_selected_images_button, 7, 2, 1, 1)
-        self.page_card_table_view = QtWidgets.QTableView(CentralWidget_Grouped)
+        self.gridLayout.addWidget(self.page_renderer, 4, 3, 3, 1)
+        self.page_card_table_view = QtWidgets.QTableView(ColumnarCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(8)
-        sizePolicy.setVerticalStretch(10)
+        sizePolicy.setHorizontalStretch(9)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.page_card_table_view.sizePolicy().hasHeightForWidth())
         self.page_card_table_view.setSizePolicy(sizePolicy)
         self.page_card_table_view.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.page_card_table_view.setLineWidth(0)
         self.page_card_table_view.setAlternatingRowColors(True)
         self.page_card_table_view.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.page_card_table_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.page_card_table_view.setObjectName("page_card_table_view")
         self.page_card_table_view.verticalHeader().setVisible(False)
-        self.gridLayout.addWidget(self.page_card_table_view, 5, 2, 2, 1)
-        self.add_card_widget = HorizontalAddCardWidget(CentralWidget_Grouped)
+        self.gridLayout.addWidget(self.page_card_table_view, 4, 2, 2, 1)
+        self.document_view_label = QtWidgets.QLabel(ColumnarCentralWidget)
+        self.document_view_label.setObjectName("document_view_label")
+        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 1)
+        self.page_view_label = QtWidgets.QLabel(ColumnarCentralWidget)
+        self.page_view_label.setObjectName("page_view_label")
+        self.gridLayout.addWidget(self.page_view_label, 0, 2, 1, 2)
+        self.delete_selected_images_button = QtWidgets.QPushButton(ColumnarCentralWidget)
+        self.delete_selected_images_button.setEnabled(False)
+        icon = QtGui.QIcon.fromTheme("edit-delete")
+        self.delete_selected_images_button.setIcon(icon)
+        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
+        self.gridLayout.addWidget(self.delete_selected_images_button, 6, 2, 1, 1)
+        self.add_card_widget_label = QtWidgets.QLabel(ColumnarCentralWidget)
+        self.add_card_widget_label.setObjectName("add_card_widget_label")
+        self.gridLayout.addWidget(self.add_card_widget_label, 0, 1, 1, 1)
+        self.add_card_widget = VerticalAddCardWidget(ColumnarCentralWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(6)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.add_card_widget.sizePolicy().hasHeightForWidth())
         self.add_card_widget.setSizePolicy(sizePolicy)
         self.add_card_widget.setObjectName("add_card_widget")
-        self.gridLayout.addWidget(self.add_card_widget, 1, 2, 2, 2)
-        self.document_view_label = QtWidgets.QLabel(CentralWidget_Grouped)
-        self.document_view_label.setObjectName("document_view_label")
-        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 2)
-        self.add_card_widget_label = QtWidgets.QLabel(CentralWidget_Grouped)
-        self.add_card_widget_label.setObjectName("add_card_widget_label")
-        self.gridLayout.addWidget(self.add_card_widget_label, 0, 2, 1, 2)
+        self.gridLayout.addWidget(self.add_card_widget, 4, 1, 3, 1)
+        self.document_view = QtWidgets.QListView(ColumnarCentralWidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(4)
+        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
+        self.document_view.setSizePolicy(sizePolicy)
+        self.document_view.setAlternatingRowColors(True)
+        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
+        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
+        self.document_view.setObjectName("document_view")
+        self.gridLayout.addWidget(self.document_view, 4, 0, 3, 1)
 
-        self.retranslateUi(CentralWidget_Grouped)
-        QtCore.QMetaObject.connectSlotsByName(CentralWidget_Grouped)
+        self.retranslateUi(ColumnarCentralWidget)
+        QtCore.QMetaObject.connectSlotsByName(ColumnarCentralWidget)
 
-    def retranslateUi(self, CentralWidget_Grouped):
+    def retranslateUi(self, ColumnarCentralWidget):
         _translate = QtCore.QCoreApplication.translate
-        self.delete_selected_images_button.setText(_translate("CentralWidget_Grouped", "Remove selected"))
-        self.document_view_label.setText(_translate("CentralWidget_Grouped", "All pages:"))
-        self.add_card_widget_label.setText(_translate("CentralWidget_Grouped", "Add new cards:"))
-from mtg_proxy_printer.ui.add_card import HorizontalAddCardWidget
+        self.document_view_label.setText(_translate("ColumnarCentralWidget", "All pages:"))
+        self.page_view_label.setText(_translate("ColumnarCentralWidget", "Current page:"))
+        self.delete_selected_images_button.setText(_translate("ColumnarCentralWidget", "Remove selected"))
+        self.add_card_widget_label.setText(_translate("ColumnarCentralWidget", "Add new cards:"))
+from mtg_proxy_printer.ui.add_card import VerticalAddCardWidget
 from mtg_proxy_printer.ui.page_renderer import PageRenderer
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_CentralWidget_Tabbed(object):
-    def setupUi(self, CentralWidget_Tabbed):
-        CentralWidget_Tabbed.setObjectName("CentralWidget_Tabbed")
-        CentralWidget_Tabbed.resize(454, 765)
-        self.gridLayout = QtWidgets.QGridLayout(CentralWidget_Tabbed)
+class Ui_TabbedCentralWidget(object):
+    def setupUi(self, TabbedCentralWidget):
+        TabbedCentralWidget.setObjectName("TabbedCentralWidget")
+        TabbedCentralWidget.resize(454, 765)
+        self.gridLayout = QtWidgets.QGridLayout(TabbedCentralWidget)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.tab_widget = QtWidgets.QTabWidget(CentralWidget_Tabbed)
+        self.tab_widget = QtWidgets.QTabWidget(TabbedCentralWidget)
         self.tab_widget.setObjectName("tab_widget")
         self.document_view = QtWidgets.QListView()
         self.document_view.setObjectName("document_view")
         self.tab_widget.addTab(self.document_view, "")
         self.add_card_widget = VerticalAddCardWidget()
         self.add_card_widget.setObjectName("add_card_widget")
         self.tab_widget.addTab(self.add_card_widget, "")
@@ -53,20 +53,20 @@
         self.verticalLayout.addWidget(self.delete_selected_images_button)
         self.tab_widget.addTab(self.tab, "")
         self.page_renderer = PageRenderer()
         self.page_renderer.setObjectName("page_renderer")
         self.tab_widget.addTab(self.page_renderer, "")
         self.gridLayout.addWidget(self.tab_widget, 4, 0, 2, 2)
 
-        self.retranslateUi(CentralWidget_Tabbed)
+        self.retranslateUi(TabbedCentralWidget)
         self.tab_widget.setCurrentIndex(0)
-        QtCore.QMetaObject.connectSlotsByName(CentralWidget_Tabbed)
+        QtCore.QMetaObject.connectSlotsByName(TabbedCentralWidget)
 
-    def retranslateUi(self, CentralWidget_Tabbed):
+    def retranslateUi(self, TabbedCentralWidget):
         _translate = QtCore.QCoreApplication.translate
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.document_view), _translate("CentralWidget_Tabbed", "All pages"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.add_card_widget), _translate("CentralWidget_Tabbed", "Add new cards"))
-        self.delete_selected_images_button.setText(_translate("CentralWidget_Tabbed", "Remove selected"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab), _translate("CentralWidget_Tabbed", "Current page"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.page_renderer), _translate("CentralWidget_Tabbed", "Preview"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.document_view), _translate("TabbedCentralWidget", "All pages"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.add_card_widget), _translate("TabbedCentralWidget", "Add new cards"))
+        self.delete_selected_images_button.setText(_translate("TabbedCentralWidget", "Remove selected"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab), _translate("TabbedCentralWidget", "Current page"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.page_renderer), _translate("TabbedCentralWidget", "Preview"))
 from mtg_proxy_printer.ui.add_card import VerticalAddCardWidget
 from mtg_proxy_printer.ui.page_renderer import PageRenderer
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/document_settings_dialog.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/document_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/main_window.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/page_config_widget.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/progress_bar.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/progress_bar.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/debug_settings_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/debug_settings_page.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,63 +10,82 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_DebugSettingsPage(object):
     def setupUi(self, DebugSettingsPage):
         DebugSettingsPage.setObjectName("DebugSettingsPage")
+        DebugSettingsPage.resize(446, 291)
         self.gridlayout = QtWidgets.QGridLayout(DebugSettingsPage)
         self.gridlayout.setObjectName("gridlayout")
+        self.open_debug_log_location = QtWidgets.QPushButton(DebugSettingsPage)
+        icon = QtGui.QIcon.fromTheme("document-open")
+        self.open_debug_log_location.setIcon(icon)
+        self.open_debug_log_location.setObjectName("open_debug_log_location")
+        self.gridlayout.addWidget(self.open_debug_log_location, 8, 1, 1, 2)
+        self.enable_write_log_file = QtWidgets.QCheckBox(DebugSettingsPage)
+        self.enable_write_log_file.setObjectName("enable_write_log_file")
+        self.gridlayout.addWidget(self.enable_write_log_file, 5, 0, 1, 3)
+        self.enable_cutelog_integration = QtWidgets.QCheckBox(DebugSettingsPage)
+        self.enable_cutelog_integration.setObjectName("enable_cutelog_integration")
+        self.gridlayout.addWidget(self.enable_cutelog_integration, 4, 0, 1, 1)
+        self.debug_download_card_data_as_file = QtWidgets.QPushButton(DebugSettingsPage)
+        icon = QtGui.QIcon.fromTheme("edit-download")
+        self.debug_download_card_data_as_file.setIcon(icon)
+        self.debug_download_card_data_as_file.setObjectName("debug_download_card_data_as_file")
+        self.gridlayout.addWidget(self.debug_download_card_data_as_file, 9, 1, 1, 2)
         self.debug_settings_header_line = QtWidgets.QFrame(DebugSettingsPage)
         self.debug_settings_header_line.setFrameShape(QtWidgets.QFrame.HLine)
         self.debug_settings_header_line.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.debug_settings_header_line.setObjectName("debug_settings_header_line")
         self.gridlayout.addWidget(self.debug_settings_header_line, 1, 0, 1, 2)
-        self.open_debug_log_location = QtWidgets.QPushButton(DebugSettingsPage)
-        icon = QtGui.QIcon.fromTheme("document-open")
-        self.open_debug_log_location.setIcon(icon)
-        self.open_debug_log_location.setObjectName("open_debug_log_location")
-        self.gridlayout.addWidget(self.open_debug_log_location, 6, 1, 1, 1)
+        self.log_level_label = QtWidgets.QLabel(DebugSettingsPage)
+        self.log_level_label.setObjectName("log_level_label")
+        self.gridlayout.addWidget(self.log_level_label, 7, 0, 1, 1)
         self.log_level_combo_box = QtWidgets.QComboBox(DebugSettingsPage)
         self.log_level_combo_box.setObjectName("log_level_combo_box")
-        self.gridlayout.addWidget(self.log_level_combo_box, 5, 1, 1, 1)
-        self.enable_write_log_file = QtWidgets.QCheckBox(DebugSettingsPage)
-        self.enable_write_log_file.setObjectName("enable_write_log_file")
-        self.gridlayout.addWidget(self.enable_write_log_file, 4, 0, 1, 2)
+        self.gridlayout.addWidget(self.log_level_combo_box, 7, 1, 1, 2)
         self.debug_settings_headerlabel = QtWidgets.QLabel(DebugSettingsPage)
         self.debug_settings_headerlabel.setObjectName("debug_settings_headerlabel")
         self.gridlayout.addWidget(self.debug_settings_headerlabel, 0, 0, 1, 2)
+        spacerItem = QtWidgets.QSpacerItem(20, 32, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.gridlayout.addItem(spacerItem, 11, 0, 1, 2)
         self.debug_import_card_data_from_file = QtWidgets.QPushButton(DebugSettingsPage)
         icon = QtGui.QIcon.fromTheme("document-import")
         self.debug_import_card_data_from_file.setIcon(icon)
         self.debug_import_card_data_from_file.setObjectName("debug_import_card_data_from_file")
-        self.gridlayout.addWidget(self.debug_import_card_data_from_file, 8, 1, 1, 1)
-        self.debug_download_card_data_as_file = QtWidgets.QPushButton(DebugSettingsPage)
-        icon = QtGui.QIcon.fromTheme("edit-download")
-        self.debug_download_card_data_as_file.setIcon(icon)
-        self.debug_download_card_data_as_file.setObjectName("debug_download_card_data_as_file")
-        self.gridlayout.addWidget(self.debug_download_card_data_as_file, 7, 1, 1, 1)
-        self.enable_cutelog_integration = QtWidgets.QCheckBox(DebugSettingsPage)
-        self.enable_cutelog_integration.setObjectName("enable_cutelog_integration")
-        self.gridlayout.addWidget(self.enable_cutelog_integration, 3, 0, 1, 2)
-        spacerItem = QtWidgets.QSpacerItem(20, 32, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.gridlayout.addItem(spacerItem, 9, 0, 1, 2)
-        self.log_level_label = QtWidgets.QLabel(DebugSettingsPage)
-        self.log_level_label.setObjectName("log_level_label")
-        self.gridlayout.addWidget(self.log_level_label, 5, 0, 1, 1)
+        self.gridlayout.addWidget(self.debug_import_card_data_from_file, 10, 1, 1, 2)
+        self.open_cutelog_website_button = QtWidgets.QPushButton(DebugSettingsPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.open_cutelog_website_button.sizePolicy().hasHeightForWidth())
+        self.open_cutelog_website_button.setSizePolicy(sizePolicy)
+        self.open_cutelog_website_button.setText("")
+        icon = QtGui.QIcon.fromTheme("globe")
+        self.open_cutelog_website_button.setIcon(icon)
+        self.open_cutelog_website_button.setObjectName("open_cutelog_website_button")
+        self.gridlayout.addWidget(self.open_cutelog_website_button, 4, 2, 1, 1)
         self.log_level_label.setBuddy(self.log_level_combo_box)
 
         self.retranslateUi(DebugSettingsPage)
         QtCore.QMetaObject.connectSlotsByName(DebugSettingsPage)
+        DebugSettingsPage.setTabOrder(self.enable_cutelog_integration, self.open_cutelog_website_button)
+        DebugSettingsPage.setTabOrder(self.open_cutelog_website_button, self.enable_write_log_file)
+        DebugSettingsPage.setTabOrder(self.enable_write_log_file, self.log_level_combo_box)
+        DebugSettingsPage.setTabOrder(self.log_level_combo_box, self.open_debug_log_location)
+        DebugSettingsPage.setTabOrder(self.open_debug_log_location, self.debug_download_card_data_as_file)
+        DebugSettingsPage.setTabOrder(self.debug_download_card_data_as_file, self.debug_import_card_data_from_file)
 
     def retranslateUi(self, DebugSettingsPage):
         _translate = QtCore.QCoreApplication.translate
         self.open_debug_log_location.setText(_translate("DebugSettingsPage", "Open debug log directory"))
-        self.log_level_combo_box.setToolTip(_translate("DebugSettingsPage", "Only write events with the given severity level and higher to the log file."))
         self.enable_write_log_file.setText(_translate("DebugSettingsPage", "Enable writing a log file to disk"))
-        self.debug_settings_headerlabel.setText(_translate("DebugSettingsPage", "Debug settings (Changing these require an application restart)"))
-        self.debug_import_card_data_from_file.setText(_translate("DebugSettingsPage", "Import card data from file"))
-        self.debug_download_card_data_as_file.setText(_translate("DebugSettingsPage", "Download card data as file"))
         self.enable_cutelog_integration.setToolTip(_translate("DebugSettingsPage", "Cutelog is a live log event viewer that can be used to monitor events in real-time."))
         self.enable_cutelog_integration.setWhatsThis(_translate("DebugSettingsPage", "<html><head/><body><p>See <a href=\"https://github.com/busimus/cutelog\"><span style=\" text-decoration: underline; color:#2980b9;\">https://github.com/busimus/cutelog</span></a> for details about Cutelog.</p></body></html>"))
         self.enable_cutelog_integration.setText(_translate("DebugSettingsPage", "Enable Cutelog integration"))
+        self.debug_download_card_data_as_file.setText(_translate("DebugSettingsPage", "Download card data as file"))
         self.log_level_label.setText(_translate("DebugSettingsPage", "Event severity that gets logged to file:"))
+        self.log_level_combo_box.setToolTip(_translate("DebugSettingsPage", "Only write events with the given severity level and higher to the log file."))
+        self.debug_settings_headerlabel.setText(_translate("DebugSettingsPage", "Debug settings (Changing these require an application restart)"))
+        self.debug_import_card_data_from_file.setText(_translate("DebugSettingsPage", "Import card data from file"))
+        self.open_cutelog_website_button.setToolTip(_translate("DebugSettingsPage", "Open the Cutelog homepage"))
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/decklist_import_settings_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/decklist_import_settings_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/general_settings_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/general_settings_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_GeneralSettingsPage(object):
     def setupUi(self, GeneralSettingsPage):
         GeneralSettingsPage.setObjectName("GeneralSettingsPage")
+        GeneralSettingsPage.resize(398, 480)
         self.gridLayout = QtWidgets.QGridLayout(GeneralSettingsPage)
         self.gridLayout.setObjectName("gridLayout")
         self.look_and_feel_settings_group_box = QtWidgets.QGroupBox(GeneralSettingsPage)
         self.look_and_feel_settings_group_box.setObjectName("look_and_feel_settings_group_box")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.look_and_feel_settings_group_box)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.add_card_widget_style_label = QtWidgets.QLabel(self.look_and_feel_settings_group_box)
@@ -68,49 +69,34 @@
         self.check_card_data_updates_enabled.setObjectName("check_card_data_updates_enabled")
         self.verticalLayout_9.addWidget(self.check_card_data_updates_enabled)
         self.gridLayout.addWidget(self.update_check_group_box, 4, 0, 1, 2)
         self.default_paths_group_box = QtWidgets.QGroupBox(GeneralSettingsPage)
         self.default_paths_group_box.setObjectName("default_paths_group_box")
         self.gridLayout_4 = QtWidgets.QGridLayout(self.default_paths_group_box)
         self.gridLayout_4.setObjectName("gridLayout_4")
+        self.document_save_path_browse_button = QtWidgets.QPushButton(self.default_paths_group_box)
+        self.document_save_path_browse_button.setText("")
+        icon = QtGui.QIcon.fromTheme("document-open")
+        self.document_save_path_browse_button.setIcon(icon)
+        self.document_save_path_browse_button.setObjectName("document_save_path_browse_button")
+        self.gridLayout_4.addWidget(self.document_save_path_browse_button, 0, 2, 1, 1)
         self.document_save_path_label = QtWidgets.QLabel(self.default_paths_group_box)
         self.document_save_path_label.setObjectName("document_save_path_label")
         self.gridLayout_4.addWidget(self.document_save_path_label, 0, 0, 1, 1)
-        self.pdf_save_path_label = QtWidgets.QLabel(self.default_paths_group_box)
-        self.pdf_save_path_label.setObjectName("pdf_save_path_label")
-        self.gridLayout_4.addWidget(self.pdf_save_path_label, 1, 0, 1, 1)
-        self.pdf_save_path = QtWidgets.QLineEdit(self.default_paths_group_box)
-        self.pdf_save_path.setInputMethodHints(QtCore.Qt.ImhNoAutoUppercase)
-        self.pdf_save_path.setClearButtonEnabled(True)
-        self.pdf_save_path.setObjectName("pdf_save_path")
-        self.gridLayout_4.addWidget(self.pdf_save_path, 1, 1, 1, 1)
         self.document_save_path = QtWidgets.QLineEdit(self.default_paths_group_box)
         self.document_save_path.setInputMethodHints(QtCore.Qt.ImhNoAutoUppercase)
         self.document_save_path.setClearButtonEnabled(True)
         self.document_save_path.setObjectName("document_save_path")
         self.gridLayout_4.addWidget(self.document_save_path, 0, 1, 1, 1)
-        self.document_save_path_browse_button = QtWidgets.QPushButton(self.default_paths_group_box)
-        self.document_save_path_browse_button.setText("")
-        icon = QtGui.QIcon.fromTheme("document-open")
-        self.document_save_path_browse_button.setIcon(icon)
-        self.document_save_path_browse_button.setObjectName("document_save_path_browse_button")
-        self.gridLayout_4.addWidget(self.document_save_path_browse_button, 0, 2, 1, 1)
-        self.pdf_save_path_browse_button = QtWidgets.QPushButton(self.default_paths_group_box)
-        self.pdf_save_path_browse_button.setText("")
-        icon = QtGui.QIcon.fromTheme("document-open")
-        self.pdf_save_path_browse_button.setIcon(icon)
-        self.pdf_save_path_browse_button.setObjectName("pdf_save_path_browse_button")
-        self.gridLayout_4.addWidget(self.pdf_save_path_browse_button, 1, 2, 1, 1)
         self.gridLayout.addWidget(self.default_paths_group_box, 3, 0, 1, 2)
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.gridLayout.addItem(spacerItem, 5, 0, 1, 2)
         self.add_card_widget_style_label.setBuddy(self.add_card_widget_style_combo_box)
         self.preferred_language_label.setBuddy(self.preferred_language_combo_box)
         self.document_save_path_label.setBuddy(self.document_save_path)
-        self.pdf_save_path_label.setBuddy(self.pdf_save_path)
 
         self.retranslateUi(GeneralSettingsPage)
         QtCore.QMetaObject.connectSlotsByName(GeneralSettingsPage)
 
     def retranslateUi(self, GeneralSettingsPage):
         _translate = QtCore.QCoreApplication.translate
         self.look_and_feel_settings_group_box.setTitle(_translate("GeneralSettingsPage", "Look && Feel (Changing this requires an application restart)"))
@@ -131,15 +117,11 @@
         self.update_check_label.setText(_translate("GeneralSettingsPage", "Update checks are performed at application start, if enabled."))
         self.check_application_updates_enabled.setToolTip(_translate("GeneralSettingsPage", "If enabled, check for application updates, and notify if new updates are available for installation."))
         self.check_application_updates_enabled.setText(_translate("GeneralSettingsPage", "Check for application updates"))
         self.check_card_data_updates_enabled.setToolTip(_translate("GeneralSettingsPage", "If enabled, query the Scryfall API if new cards are available. If so, offer to update the local card data."))
         self.check_card_data_updates_enabled.setText(_translate("GeneralSettingsPage", "Check for new card data"))
         self.default_paths_group_box.setToolTip(_translate("GeneralSettingsPage", "These paths are selected by default when browsing the file system for files"))
         self.default_paths_group_box.setTitle(_translate("GeneralSettingsPage", "Default save paths"))
+        self.document_save_path_browse_button.setToolTip(_translate("GeneralSettingsPage", "Browse…"))
         self.document_save_path_label.setText(_translate("GeneralSettingsPage", "Document save path"))
-        self.pdf_save_path_label.setText(_translate("GeneralSettingsPage", "PDF export path"))
-        self.pdf_save_path.setToolTip(_translate("GeneralSettingsPage", "If set, use this as the default location for saving exported PDF documents."))
-        self.pdf_save_path.setPlaceholderText(_translate("GeneralSettingsPage", "Path to a directory"))
         self.document_save_path.setToolTip(_translate("GeneralSettingsPage", "If set, use this as the default location for saving documents."))
         self.document_save_path.setPlaceholderText(_translate("GeneralSettingsPage", "Path to a directory"))
-        self.document_save_path_browse_button.setToolTip(_translate("GeneralSettingsPage", "Browse…"))
-        self.pdf_save_path_browse_button.setToolTip(_translate("GeneralSettingsPage", "Browse…"))
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/hide_printings_page.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/hide_printings_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         HidePrintingsPage.setObjectName("HidePrintingsPage")
         self.verticalLayout = QtWidgets.QVBoxLayout(HidePrintingsPage)
         self.verticalLayout.setObjectName("verticalLayout")
         self.card_filter_settings_header_label = QtWidgets.QLabel(HidePrintingsPage)
         self.card_filter_settings_header_label.setWordWrap(True)
         self.card_filter_settings_header_label.setObjectName("card_filter_settings_header_label")
         self.verticalLayout.addWidget(self.card_filter_settings_header_label)
-        self.card_filter_general_settings = GeneralPrintingFilterWidget(HidePrintingsPage)
+        self.card_filter_general_settings = GeneralPrintingFilter(HidePrintingsPage)
         self.card_filter_general_settings.setObjectName("card_filter_general_settings")
         self.verticalLayout.addWidget(self.card_filter_general_settings)
-        self.card_filter_format_settings = FormatPrintingFilterWidget(HidePrintingsPage)
+        self.card_filter_format_settings = FormatPrintingFilter(HidePrintingsPage)
         self.card_filter_format_settings.setObjectName("card_filter_format_settings")
         self.verticalLayout.addWidget(self.card_filter_format_settings)
         self.set_filter_label = QtWidgets.QLabel(HidePrintingsPage)
         self.set_filter_label.setWordWrap(True)
         self.set_filter_label.setObjectName("set_filter_label")
         self.verticalLayout.addWidget(self.set_filter_label)
         self.set_filter_settings = QtWidgets.QPlainTextEdit(HidePrintingsPage)
@@ -41,8 +41,8 @@
         _translate = QtCore.QCoreApplication.translate
         self.card_filter_settings_header_label.setText(_translate("HidePrintingsPage", "These options allow hiding unwanted cards and printings. Hidden printings are treated as though they don’t exist. They can’t be found in the card search and are automatically replaced in loaded documents or imported deck lists, if possible. If all printings of a card are hidden, it won’t be available at all."))
         self.set_filter_label.setText(_translate("HidePrintingsPage", "Hide specific sets: Add set codes as listed on Scryfall, for example LEA or 2X2. Separate multiple entries with spaces or line breaks. All words not matching an exact set code are ignored."))
         self.set_filter_settings.setToolTip(_translate("HidePrintingsPage", "Example:\n"
 "\n"
 "LEA DDU TC13 J21"))
         self.set_filter_settings.setPlaceholderText(_translate("HidePrintingsPage", "No sets currently hidden."))
-from mtg_proxy_printer.ui.printing_filter_widgets import FormatPrintingFilterWidget, GeneralPrintingFilterWidget
+from mtg_proxy_printer.ui.printing_filter_widgets import FormatPrintingFilter, GeneralPrintingFilter
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,23 @@
         self.stacked_pages.setObjectName("stacked_pages")
         self.general_settings_page = GeneralSettingsPage()
         self.general_settings_page.setObjectName("general_settings_page")
         self.stacked_pages.addWidget(self.general_settings_page)
         self.decklist_import_settings_page = DecklistImportSettingsPage()
         self.decklist_import_settings_page.setObjectName("decklist_import_settings_page")
         self.stacked_pages.addWidget(self.decklist_import_settings_page)
-        self.page_size_page = PageSizePrintingSettingsPage()
-        self.page_size_page.setObjectName("page_size_page")
-        self.stacked_pages.addWidget(self.page_size_page)
+        self.pdf_settings_page = PDFSettingsPage()
+        self.pdf_settings_page.setObjectName("pdf_settings_page")
+        self.stacked_pages.addWidget(self.pdf_settings_page)
+        self.printer_settings_page = PrinterSettingsPage()
+        self.printer_settings_page.setObjectName("printer_settings_page")
+        self.stacked_pages.addWidget(self.printer_settings_page)
+        self.default_document_layout_page = DefaultDocumentLayoutSettingsPage()
+        self.default_document_layout_page.setObjectName("default_document_layout_page")
+        self.stacked_pages.addWidget(self.default_document_layout_page)
         self.hide_printings_page = HidePrintingsPage()
         self.hide_printings_page.setObjectName("hide_printings_page")
         self.stacked_pages.addWidget(self.hide_printings_page)
         self.debug_settings_page = DebugSettingsPage()
         self.debug_settings_page.setObjectName("debug_settings_page")
         self.stacked_pages.addWidget(self.debug_settings_page)
         self.gridLayout.addWidget(self.stacked_pages, 1, 1, 1, 1)
@@ -57,15 +63,16 @@
         self.gridLayout.addWidget(self.page_selection_list_view, 0, 0, 2, 1)
         self.button_box = QtWidgets.QDialogButtonBox(SettingsWindow)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Reset|QtWidgets.QDialogButtonBox.RestoreDefaults|QtWidgets.QDialogButtonBox.Save)
         self.button_box.setObjectName("button_box")
         self.gridLayout.addWidget(self.button_box, 2, 0, 1, 2)
 
         self.retranslateUi(SettingsWindow)
+        self.stacked_pages.setCurrentIndex(0)
         self.button_box.accepted.connect(SettingsWindow.accept) # type: ignore
         self.button_box.rejected.connect(SettingsWindow.reject) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(SettingsWindow)
 
     def retranslateUi(self, SettingsWindow):
         _translate = QtCore.QCoreApplication.translate
         SettingsWindow.setWindowTitle(_translate("SettingsWindow", "Settings"))
-from mtg_proxy_printer.ui.settings_window_pages import DebugSettingsPage, DecklistImportSettingsPage, GeneralSettingsPage, HidePrintingsPage, PageSizePrintingSettingsPage
+from mtg_proxy_printer.ui.settings_window_pages import DebugSettingsPage, DecklistImportSettingsPage, DefaultDocumentLayoutSettingsPage, GeneralSettingsPage, HidePrintingsPage, PDFSettingsPage, PrinterSettingsPage
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/item_delegates.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/item_delegates.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
     def createEditor(self, parent: QWidget, option: QStyleOptionViewItem, index: QModelIndex) -> QComboBox:
         editor = QComboBox(parent)
         return editor
 
     def setEditorData(self, editor: QComboBox, index: QModelIndex) -> None:
         model: typing.Union[Document, QSortFilterProxyModel] = index.model()
-        source_model: Document = model
         column = index.column()
-        while hasattr(source_model, "sourceModel"):  # Resolve the source model to gain access to the card database.
-            source_model = source_model.sourceModel()
+        while hasattr(model, "sourceModel"):  # Resolve the source model to gain access to the card database.
+            model = model.sourceModel()
+        source_model: Document = model
 
         if column == PageColumns.Set:
             matching_sets = source_model.card_db.find_sets_matching(
                 index.siblingAtColumn(PageColumns.CardName).data(ItemDataRole.EditRole),
                 index.siblingAtColumn(PageColumns.Language).data(ItemDataRole.EditRole),
                 is_front=index.siblingAtColumn(PageColumns.IsFront).data(ItemDataRole.EditRole),
             )
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/main_window.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from mtg_proxy_printer.document_controller.shuffle_document import ActionShuffleDocument
 from mtg_proxy_printer.document_controller.new_document import ActionNewDocument
 from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
 from mtg_proxy_printer.units_and_sizes import DEFAULT_SAVE_SUFFIX
 import mtg_proxy_printer.settings
 import mtg_proxy_printer.print
 from mtg_proxy_printer.ui.dialogs import SavePDFDialog, SaveDocumentAsDialog, LoadDocumentDialog, \
-    AboutMTGProxyPrinterDialog, PrintPreviewDialog, PrintDialog, DocumentSettingsDialog
+    AboutDialog, PrintPreviewDialog, PrintDialog, DocumentSettingsDialog
 from mtg_proxy_printer.ui.cache_cleanup_wizard import CacheCleanupWizard
 from mtg_proxy_printer.ui.deck_import_wizard import DeckImportWizard
 from mtg_proxy_printer.ui.progress_bar import ProgressBar
 
 try:
     from mtg_proxy_printer.ui.generated.main_window import Ui_MainWindow
 except ModuleNotFoundError:
@@ -99,16 +99,16 @@
             lambda: self.language_model.setStringList(self.card_database.get_all_languages())
         )
         self.ui.action_show_toolbar.setChecked(mtg_proxy_printer.settings.settings["gui"].getboolean("show-toolbar"))
         self._setup_platform_dependent_default_shortcuts()
         self.current_dialog: typing.Optional[QDialog] = None
         logger.info(f"Created {self.__class__.__name__} instance.")
 
-    def _create_about_dialog(self) -> AboutMTGProxyPrinterDialog:
-        about_dialog = AboutMTGProxyPrinterDialog(self)
+    def _create_about_dialog(self) -> AboutDialog:
+        about_dialog = AboutDialog(self)
         self.ui.action_show_about_dialog.triggered.connect(about_dialog.show_about)
         self.ui.action_show_changelog.triggered.connect(about_dialog.show_changelog)
         return about_dialog
 
     def _setup_platform_dependent_default_shortcuts(self):
         actions_with_shortcuts: typing.List[typing.Tuple[QAction, StandardKey]] = [
             (self.ui.action_new_document, StandardKey.New),
@@ -390,18 +390,18 @@
             )
 
     def show_application_update_available_message_box(self, newer_version: str):
         if QMessageBox.question(
                 self, "Application update available. Visit website?",
                 f"An application update is available: Version {newer_version}\n"
                 f"You are currently using version {mtg_proxy_printer.meta_data.__version__}.\n\n"
-                f"Open the {mtg_proxy_printer.meta_data.PROGRAMNAME} website in your webbrowser "
+                f"Open the {mtg_proxy_printer.meta_data.PROGRAMNAME} website in your web browser "
                 f"to download the new version?",
                 StandardButton.Yes | StandardButton.No, StandardButton.No
-                ) == StandardButton.Yes:
+        ) == StandardButton.Yes:
             url = QUrl(mtg_proxy_printer.meta_data.DOWNLOAD_WEB_PAGE, QUrl.ParsingMode.StrictMode)
             QDesktopServices.openUrl(url)
 
     def show_card_data_update_available_message_box(self, estimated_card_count: int):
         if QMessageBox.question(
                 self, "New card data available",
                 f"There are {estimated_card_count} new printings available on Scryfall. Update the local data now?",
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_config_widget.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_config_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
 
     def _setup_page_layout(self, ui: Ui_PageConfigWidget) -> PageLayoutSettings:
         # Implementation note: The signal connections below will also trigger
         # when programmatically populating the widget values.
         # Therefore, it is not necessary to ever explicitly set the page_layout
         # attributes to the current values.
         page_layout = PageLayoutSettings()
-        ui.column_spacing.valueChanged[int].connect(lambda value: logger.debug(f"Column spacing now {value}"))
-        ui.page_width.valueChanged[int].connect(lambda value: logger.debug(f"Page width now {value}"))
         ui.card_bleed.valueChanged[int].connect(partial(setattr, page_layout, "card_bleed"))
         ui.page_height.valueChanged[int].connect(partial(setattr, page_layout, "page_height"))
         ui.page_width.valueChanged[int].connect(partial(setattr, page_layout, "page_width"))
         ui.margin_top.valueChanged[int].connect(partial(setattr, page_layout, "margin_top"))
         ui.margin_bottom.valueChanged[int].connect(partial(setattr, page_layout, "margin_bottom"))
         ui.margin_left.valueChanged[int].connect(partial(setattr, page_layout, "margin_left"))
         ui.margin_right.valueChanged[int].connect(partial(setattr, page_layout, "margin_right"))
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_renderer.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,14 @@
             f"Usable keyboard shortcuts are:\n"
             f"Zoom in: {', '.join(shortcut.toString(QKeySequence.NativeText) for shortcut in self.zoom_in_action.shortcuts())}\n"
             f"Zoom out: {', '.join(shortcut.toString(QKeySequence.NativeText) for shortcut in self.zoom_out_action.shortcuts())}"
         )
         self._update_background_brush()
         logger.info(f"Created {self.__class__.__name__} instance.")
 
-    def scene(self) -> PageScene:
-        return super().scene()
-
     def changeEvent(self, event: QEvent) -> None:
         if event.type() in {QEvent.ApplicationPaletteChange, QEvent.PaletteChange}:
             self._update_background_brush()
             self.scene().setPalette(self.palette())
             event.accept()
         else:
             super().changeEvent(event)
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/page_scene.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/page_scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,17 @@
         right = self.corner_length
         self.setPolygon(QPolygonF((
             QPointF(left, top), QPointF(right, top), QPointF(right, top+h_px),
             QPointF(left+v_px, top+h_px),
             QPointF(left+v_px, bottom),
             QPointF(left, bottom), QPointF(left, top)
         )))
-        # Some renderers do draw zero-width elements as faint lines, so set zero-width bleeds to be transparent
-        self.setOpacity(h_px > 0 < v_px)
+        # Some renderers do draw zero-width elements as faint lines,
+        # so set zero-width bleeds to be transparent
+        self.setOpacity(h_px > 0 or v_px > 0)
 
 
 class NeighborsPresent(typing.NamedTuple):
     top: bool
     bottom: bool
     left: bool
     right: bool
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/printing_filter_widgets.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/printing_filter_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import abc
 import configparser
 from functools import partial
-from typing import Union, Type, List, Tuple
+from typing import List, Tuple
 
 from PyQt5.QtCore import QUrl
 from PyQt5.QtGui import QDesktopServices
 from PyQt5.QtWidgets import QGroupBox, QWidget, QCheckBox, QPushButton
 
 from mtg_proxy_printer.ui.common import highlight_widget
 
@@ -29,24 +29,18 @@
     from mtg_proxy_printer.ui.generated.settings_window.format_printing_filter import Ui_FormatPrintingFilter
     from mtg_proxy_printer.ui.generated.settings_window.general_printing_filter import Ui_GeneralPrintingFilter
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_FormatPrintingFilter = load_ui_from_file("settings_window/format_printing_filter")
     Ui_GeneralPrintingFilter = load_ui_from_file("settings_window/general_printing_filter")
 
-UiTypes = Union[Type[Ui_FormatPrintingFilter], Type[Ui_GeneralPrintingFilter]]
 ParsingMode = QUrl.ParsingMode
 
 
-class AbstractPrintingFilterWidget(QGroupBox):
-
-    def __init__(self, ui_class: UiTypes, parent: QWidget = None):
-        super().__init__(parent)
-        self.ui = ui_class()
-        self.ui.setupUi(self)
+class AbstractPrintingFilter(QGroupBox):
 
     def load_settings(self, settings: configparser.SectionProxy):
         for widget, key in self._get_widgets_with_keys():
             widget.setChecked(settings.getboolean(key))
 
     def save_settings(self, settings: configparser.SectionProxy):
         for widget, key in self._get_widgets_with_keys():
@@ -64,21 +58,22 @@
 
     @abc.abstractmethod
     def highlight_differing_settings(self, settings: configparser.ConfigParser):
         """Highlights GUI widgets with a state different from the given settings"""
         pass
 
 
-class GeneralPrintingFilterWidget(AbstractPrintingFilterWidget):
+class GeneralPrintingFilter(AbstractPrintingFilter):
     """
     Manages settings for all printing filters that are not related to bans in specific formats
     """
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_GeneralPrintingFilter, parent)
-        ui = self.ui
+        super().__init__(parent)
+        self.ui = ui = Ui_GeneralPrintingFilter()
+        ui.setupUi(self)
         ui.view_cards_depicting_racism.clicked.connect(
             partial(self.view_query_on_scryfall, "function:banned-due-to-racist-imagery"))
         ui.view_oversized_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:oversized"))
         ui.view_white_bordered_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:white"))
         ui.view_gold_bordered_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:gold"))
         ui.view_borderless_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:borderless"))
         ui.view_extended_art_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:extended"))
@@ -107,24 +102,25 @@
     def highlight_differing_settings(self, settings: configparser.ConfigParser):
         section = settings["card-filter"]
         for widget, setting in self._get_widgets_with_keys():
             if widget.isChecked() is not section.getboolean(setting):
                 highlight_widget(widget)
 
 
-class FormatPrintingFilterWidget(AbstractPrintingFilterWidget):
+class FormatPrintingFilter(AbstractPrintingFilter):
     """
     Manages printing filters for bans in specific formats. An enabled filter for a given format hides
     all cards that are banned in that format.
     """
     # TODO 1: Refactor to generate the checkbox list and button list from the format list in the settings
     # TODO 2: Write test that ensures that there is a bijection between settings keys and widgets
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_FormatPrintingFilter, parent)
-        ui = self.ui
+        super().__init__(parent)
+        self.ui = ui = Ui_FormatPrintingFilter()
+        ui.setupUi(self)
         for _, key in self._get_widgets_with_keys():
             format_name = key.split("-")[-1]
             button: QPushButton = getattr(ui, f"view_banned_in_{format_name}")
             button.clicked.connect(
                 partial(self.view_query_on_scryfall, f"banned:{format_name}")
             )
 
@@ -145,8 +141,8 @@
         ]
         return widgets_with_settings
 
     def highlight_differing_settings(self, settings: configparser.ConfigParser):
         section = settings["card-filter"]
         for widget, setting in self._get_widgets_with_keys():
             if widget.isChecked() is not section.getboolean(setting):
-                highlight_widget(widget)
+                highlight_widget(widget)
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/progress_bar.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         for item in (ui.inner_progress_bar, ui.inner_progress_label):
             self._set_retain_size_policy(item, True)
             item.hide()
         for item in (ui.outer_progress_bar, ui.outer_progress_label, ui.independent_bar, ui.independent_label):
             item.hide()
         
     @staticmethod
-    def _set_retain_size_policy(wigdget: QWidget, value: bool):
-        policy = wigdget.sizePolicy()
+    def _set_retain_size_policy(widget: QWidget, value: bool):
+        policy = widget.sizePolicy()
         policy.setRetainSizeWhenHidden(value)
-        wigdget.setSizePolicy(policy)
+        widget.setSizePolicy(policy)
 
     @Slot(int)
     @Slot(int, str)
     def begin_outer_progress(self, upper_limit: int, ui_hint: str = ""):
         self._begin_progress(self.ui.outer_progress_bar, self.ui.outer_progress_label, upper_limit, ui_hint)
 
     @Slot(int)
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/settings_window.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/settings_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 import configparser
 import pathlib
 import typing
 
 from PyQt5.QtCore import QStringListModel, pyqtSignal as Signal, Qt, QItemSelectionModel, QEvent, QObject
 from PyQt5.QtWidgets import QDialogButtonBox, QMessageBox, QWidget, QDialog
-from PyQt5.QtGui import QIcon, QStandardItemModel, QStandardItem, QResizeEvent
+from PyQt5.QtGui import QIcon, QStandardItemModel, QResizeEvent
 
 import mtg_proxy_printer.app_dirs
 from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.document_controller import DocumentAction
 from mtg_proxy_printer.document_controller.edit_document_settings import ActionEditDocumentSettings
 
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.logger import get_logger
 from mtg_proxy_printer.ui.settings_window_pages import Page, HidePrintingsPage
-from mtg_proxy_printer.units_and_sizes import OptStr
 
 try:
     from mtg_proxy_printer.ui.generated.settings_window.settings_window import Ui_SettingsWindow
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_SettingsWindow = load_ui_from_file("settings_window/settings_window")
 
@@ -46,26 +45,14 @@
 TALL_LAYOUT_THRESHOLD = 750
 
 __all__ = [
     "SettingsWindow",
 ]
 
 
-def item_factory(text: str, icon_name: OptStr, tooltip_text: OptStr = None) -> typing.Sequence[QStandardItem]:
-    item = QStandardItem(text)
-    if icon_name:
-        item.setIcon(QIcon.fromTheme(icon_name))
-    if tooltip_text:
-        item.setToolTip(tooltip_text)
-    size = item.sizeHint()
-    size.setHeight(32)
-    item.setSizeHint(size)
-    return item,
-
-
 class HoverEventFilter(QObject):
     def __init__(self, settings: configparser.ConfigParser, parent: "SettingsWindow"):
         super().__init__(parent)
         self.settings = settings
 
     def eventFilter(self, object_, event: QEvent):
         event_type = event.type()
@@ -103,19 +90,18 @@
         self._setup_hide_printing_page(ui.hide_printings_page, document.card_db)
         self._setup_button_box()
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     def _setup_pages_model(self, ui: Ui_SettingsWindow) -> QStandardItemModel:
         model = QStandardItemModel(self)
         # Create the model entries for each page, in the order they are stacked.
-        model.appendRow(item_factory("General settings", "configure"))
-        model.appendRow(item_factory("Deck list import", "edit-download", "Configure the deck list importer"))
-        model.appendRow(item_factory("Document & print settings", "document-print", "Configure document settings, page size and printing options"))
-        model.appendRow(item_factory("Hide printings", "view-hidden", "Hide unwanted printings"))
-        model.appendRow(item_factory("Debug settings", None, "Things useful for investigating bugs in the application"))
+        pages: typing.List[Page] = [ui.stacked_pages.widget(index) for index in range(ui.stacked_pages.count())]
+        for page in pages:
+            model.appendRow(page.display_item())
+
         # Set the models
         ui.page_selection_list_view.setModel(model)
         ui.page_selection_combo_box.setModel(model)
         ui.page_selection_list_view.setSelectionMode(ui.page_selection_list_view.SelectionMode.SingleSelection)
         first_page = model.index(0, 0)
         selection_model = ui.page_selection_list_view.selectionModel()
         selection_model.select(first_page, ClearAndSelect)
@@ -181,21 +167,16 @@
     def _adapt_layout_to_size(self, size):
         is_narrow = size.width() < TALL_LAYOUT_THRESHOLD
         self.ui.page_selection_list_view.setHidden(is_narrow)
         self.ui.page_selection_combo_box.setVisible(is_narrow)
 
     def _get_pages(self) -> typing.Sequence[Page]:
         ui = self.ui
-        return (
-            ui.debug_settings_page,
-            ui.decklist_import_settings_page,
-            ui.general_settings_page,
-            ui.hide_printings_page,
-            ui.page_size_page,
-        )
+        return [ui.stacked_pages.widget(index) for index in range(ui.stacked_pages.count())]
+
 
     def load_settings(self, settings: configparser.ConfigParser):
         logger.debug("Loading the settings")
         for page in self._get_pages():
             page.load(settings)
         logger.debug("Finished loading settings")
 
@@ -203,15 +184,15 @@
         """Automatically called when the user hits the "Save" button."""
         logger.info("User wants to save the settings.")
         old_preferred_language = mtg_proxy_printer.settings.settings["images"]["preferred-language"]
         new_preferred_language = self.ui.general_settings_page.ui.preferred_language_combo_box.currentText()
         if old_preferred_language != new_preferred_language:
             self.preferred_language_changed.emit(new_preferred_language)
         current_document_layout = self.document.page_layout
-        new_default_layout = self.ui.page_size_page.ui.page_configuration_group_box.page_layout
+        new_default_layout = self.ui.default_document_layout_page.ui.page_configuration_group_box.page_layout
         if current_document_layout != new_default_layout and QMessageBox.question(
                 self, "Apply settings to the current document?",
                 "The new default settings differ from the settings used by the current document.\n"
                 "Apply the new settings to the current document?",
                 MessageBoxButton.Yes | MessageBoxButton.No, MessageBoxButton.Yes
         ) == MessageBoxButton.Yes:
             logger.info("User applies changed document settings to the current document")
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/ui/settings_window_pages.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/ui/settings_window_pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,57 +12,90 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 import configparser
 import logging
+from functools import partial
 import pathlib
 import typing
 from abc import abstractmethod
 
 from PyQt5.QtCore import pyqtSignal as Signal, pyqtSlot as Slot, QUrl, QStandardPaths, QStringListModel, Qt, QThreadPool
-from PyQt5.QtGui import QDesktopServices
+from PyQt5.QtGui import QDesktopServices, QStandardItem, QIcon
 from PyQt5.QtWidgets import QWidget, QCheckBox, QFileDialog, QMessageBox, QApplication, QLineEdit
 
 import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.printing_filter_updater import PrintingFilterUpdater
 from mtg_proxy_printer.logger import get_logger
 from mtg_proxy_printer.ui.common import highlight_widget
+from mtg_proxy_printer.units_and_sizes import OptStr
+
+if typing.TYPE_CHECKING:
+    from mtg_proxy_printer.application import Application
 
 try:
     from mtg_proxy_printer.ui.generated.settings_window.debug_settings_page import Ui_DebugSettingsPage
-    from mtg_proxy_printer.ui.generated.settings_window.decklist_import_settings_page import Ui_DecklistImportSettingsPage
+    from mtg_proxy_printer.ui.generated.settings_window.decklist_import_settings_page \
+        import Ui_DecklistImportSettingsPage
     from mtg_proxy_printer.ui.generated.settings_window.general_settings_page import Ui_GeneralSettingsPage
     from mtg_proxy_printer.ui.generated.settings_window.hide_printings_page import Ui_HidePrintingsPage
-    from mtg_proxy_printer.ui.generated.settings_window.page_size_printing_page import Ui_PageSizePrintingSettings
+    from mtg_proxy_printer.ui.generated.settings_window.default_document_layout_settings_page \
+        import Ui_DefaultDocumentLayoutSettingsPage
+    from mtg_proxy_printer.ui.generated.settings_window.printer_settings_page import Ui_PrinterSettingsPage
+    from mtg_proxy_printer.ui.generated.settings_window.pdf_settings_page import Ui_PDFSettingsPage
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_DebugSettingsPage = load_ui_from_file("settings_window/debug_settings_page")
     Ui_DecklistImportSettingsPage = load_ui_from_file("settings_window/decklist_import_settings_page")
     Ui_GeneralSettingsPage = load_ui_from_file("settings_window/general_settings_page")
     Ui_HidePrintingsPage = load_ui_from_file("settings_window/hide_printings_page")
-    Ui_PageSizePrintingSettings = load_ui_from_file("settings_window/page_size_printing_page")
+    Ui_DefaultDocumentLayoutSettingsPage = load_ui_from_file("settings_window/default_document_layout_settings_page")
+    Ui_PrinterSettingsPage = load_ui_from_file("settings_window/printer_settings_page")
+    Ui_PDFSettingsPage = load_ui_from_file("settings_window/pdf_settings_page")
 
 CheckState = Qt.CheckState
 bool_to_check_state: typing.Dict[typing.Optional[bool], CheckState] = {
     True: CheckState.Checked,
     False: CheckState.Unchecked,
     None: CheckState.PartiallyChecked,
 }
 check_state_to_bool_str: typing.Dict[CheckState, str] = {v: str(k) for k, v in bool_to_check_state.items()}
 QueuedConnection = Qt.ConnectionType.QueuedConnection
 logger = get_logger(__name__)
 del get_logger
 
+class PageMetadata(typing.NamedTuple):
+    text: str
+    icon_name: OptStr
+    tooltip: OptStr = None
+
 
 class Page(QWidget):
     """The base class for settings page widgets. Defines the API used by the settings window"""
 
+    def display_item(self) -> typing.Sequence[QStandardItem]:
+        data = self.display_metadata
+        item = QStandardItem(data.text)
+        if data.icon_name:
+            item.setIcon(QIcon.fromTheme(data.icon_name))
+        if data.tooltip:
+            item.setToolTip(data.tooltip)
+        size = item.sizeHint()
+        size.setHeight(32)
+        item.setSizeHint(size)
+        return item,
+
+    @property
+    @abstractmethod
+    def display_metadata(self) -> PageMetadata:
+        return PageMetadata("FIXME: FILL DATA", None, "FIXME: FILL DATA")
+
     @abstractmethod
     def save(self):
         """Saves the GUI state into the global application settings"""
         pass
 
     @abstractmethod
     def load(self, settings: configparser.ConfigParser):
@@ -79,28 +112,32 @@
         for item in self.findChildren((QWidget,), options=Qt.FindChildOption.FindChildrenRecursively):  # type: QWidget
             item.setGraphicsEffect(None)
 
 
 class DebugSettingsPage(Page):
 
     requested_card_download = Signal(pathlib.Path)
+    display_metadata = PageMetadata("Debug settings", None, "Things useful for investigating bugs in the application")
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
         self.ui = ui = Ui_DebugSettingsPage()
         ui.setupUi(self)
         self.requested_card_download.connect(lambda _: ui.debug_download_card_data_as_file.setEnabled(False))
         ui.log_level_combo_box.addItems(map(logging.getLevelName, range(10, 60, 10)))
+        url = QUrl("https://github.com/busimus/cutelog", QUrl.ParsingMode.StrictMode)
+        ui.open_cutelog_website_button.clicked.connect(partial(QDesktopServices.openUrl, url))
 
     def load(self, settings: configparser.ConfigParser):
         section = settings["debug"]
         for widget, setting in self._get_debug_settings_checkbox_widgets():
             widget.setChecked(section.getboolean(setting))
         log_level_combo_box = self.ui.log_level_combo_box
-        log_level_combo_box.setCurrentIndex(log_level_combo_box.findText(section["log-level"]))
+        configured_level_index = log_level_combo_box.findText(section["log-level"])
+        log_level_combo_box.setCurrentIndex(configured_level_index)
 
     def save(self):
         debug_section = mtg_proxy_printer.settings.settings["debug"]
         for widget, setting in self._get_debug_settings_checkbox_widgets():
             debug_section[setting] = str(widget.isChecked())
         debug_section["log-level"] = self.ui.log_level_combo_box.currentText()
 
@@ -134,14 +171,15 @@
         location = QFileDialog.getExistingDirectory(
             self, "Select download location",
             QStandardPaths.locate(QStandardPaths.DownloadLocation, "", QStandardPaths.LocateDirectory))
         if not location:
             logger.debug("User cancelled location selection. Not downloading.")
             return
         if not (path := pathlib.Path(location)).is_dir():
+            logger.warning("User selected something that is not a directory. Aborting.")
             QMessageBox.critical(
                 self, "Selected location is not a directory",
                 f"Cannot write the card data at the given location, because it is not a directory:\n{location}",
                 QMessageBox.StandardButton.Ok, QMessageBox.StandardButton.Ok)
             return
         logger.info(f"Download card data to file {path}")
         self.requested_card_download.emit(path)
@@ -154,24 +192,27 @@
             QStandardPaths.locate(QStandardPaths.DownloadLocation, "", QStandardPaths.LocateDirectory),
             "Scryfall card data (*.json, *.json.gz)")
         logger.info(f"{location=}")
         if not location:
             logger.debug("User cancelled file selection. Not importing.")
             return
         if not (path := pathlib.Path(location)).is_file():
+            logger.warning("User selected something that is not a file. Aborting.")
             QMessageBox.critical(
                 self, "Selected location is not a file",
                 f"Cannot find the selected file:\n{location}",
                 QMessageBox.StandardButton.Ok, QMessageBox.StandardButton.Ok)
             return
         logger.info(f"Import card data from {path}")
-        QApplication.instance().card_info_downloader.import_from_file(path)
+        app: "Application" = QApplication.instance()
+        app.card_info_downloader.import_from_file(path)
 
 
 class DecklistImportSettingsPage(Page):
+    display_metadata = PageMetadata("Deck list import", "edit-download", "Configure the deck list importer")
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
         self.ui = ui = Ui_DecklistImportSettingsPage()
         ui.setupUi(self)
 
     @Slot()
@@ -227,14 +268,15 @@
         section = mtg_proxy_printer.settings.settings["default-filesystem-paths"]
         for widget, setting in self._get_save_path_settings_widgets():
             if widget.text() != section[setting]:
                 highlight_widget(widget)
 
 
 class GeneralSettingsPage(Page):
+    display_metadata = PageMetadata("General settings", "configure")
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
         self.ui = ui = Ui_GeneralSettingsPage()
         self.language_model = QStringListModel([], self)
         ui.setupUi(self)
         ui.add_card_widget_style_combo_box.addItem("Horizontal layout", "horizontal")
@@ -248,21 +290,14 @@
     @Slot()
     def on_document_save_path_browse_button_clicked(self):
         logger.debug("User about to select a new default document save path.")
         if location := QFileDialog.getExistingDirectory(self, "Select default save location"):
             logger.info("User selected a new default document save path.")
             self.ui.document_save_path.setText(location)
 
-    @Slot()
-    def on_pdf_save_path_browse_button_clicked(self):
-        logger.debug("User about to select a new default PDF document export path.")
-        if location := QFileDialog.getExistingDirectory(self, "Select default PDF export location"):
-            logger.info("User selected a new default PDF document export path.")
-            self.ui.pdf_save_path.setText(location)
-
     def load(self, settings: configparser.ConfigParser):
         self._load_layout_settings(settings)
         self._load_update_settings(settings)
         self._load_images_settings(settings)
         self._load_path_settings(settings)
 
     def _load_layout_settings(self, settings: configparser.ConfigParser):
@@ -360,20 +395,20 @@
             if section[setting] != widget.text():
                 highlight_widget(widget)
 
     def _get_save_path_settings_widgets(self):
         ui = self.ui
         widgets_with_settings: typing.List[typing.Tuple[QLineEdit, str]] = [
             (ui.document_save_path, "document-save-path"),
-            (ui.pdf_save_path, "pdf-export-path"),
         ]
         return widgets_with_settings
 
 
 class HidePrintingsPage(Page):
+    display_metadata = PageMetadata("Hide printings", "view-hidden", "Hide unwanted printings")
 
     error_occurred = Signal(str)
     long_running_process_begins = Signal(int, str)
     process_updated = Signal(int)
     process_finished = Signal()
 
     def __init__(self, parent: QWidget = None):
@@ -405,56 +440,102 @@
         ui = self.ui
         ui.card_filter_general_settings.highlight_differing_settings(settings)
         ui.card_filter_general_settings.highlight_differing_settings(settings)
         if section["hidden-sets"] != ui.set_filter_settings.toPlainText():
             highlight_widget(ui.set_filter_settings)
 
 
-class PageSizePrintingSettingsPage(Page):
+class DefaultDocumentLayoutSettingsPage(Page):
+    display_metadata = PageMetadata(
+        "Default document settings", "document-properties",
+        "Set the default document settings used for new documents,\nlike page size, margins, spacings, etc."
+    )
 
     def __init__(self, parent: QWidget = None):
         super().__init__(parent)
-        self.ui = ui = Ui_PageSizePrintingSettings()
+        self.ui = ui = Ui_DefaultDocumentLayoutSettingsPage()
         ui.setupUi(self)
         ui.page_configuration_group_box.setTitle("Default settings for new documents")
 
     def load(self, settings: configparser.ConfigParser):
+        self.ui.page_configuration_group_box.load_document_settings_from_config(settings)
+
+    def save(self):
+        self.ui.page_configuration_group_box.save_document_settings_to_config()
+
+    def highlight_differing_settings(self, settings: configparser.ConfigParser):
+        self.ui.page_configuration_group_box.highlight_differing_settings(settings)
+
+
+class PrinterSettingsPage(Page):
+    display_metadata = PageMetadata("Printer settings", "document-print", "Configure the printer")
+
+    def __init__(self, parent=None, flags=Qt.WindowFlags()):
+        super().__init__(parent, flags)
+        self.ui = ui = Ui_PrinterSettingsPage()
+        ui.setupUi(self)
+
+    def _get_printer_settings_widgets(self):
         ui = self.ui
-        ui.pdf_page_count_limit.setValue(settings["documents"].getint("pdf-page-count-limit"))
-        ui.page_configuration_group_box.load_document_settings_from_config(settings)
-        self._load_printer_settings(settings)
+        widgets_with_settings: typing.List[typing.Tuple[QCheckBox, str]] = [
+            (ui.printer_use_borderless_printing, "borderless-printing"),
+            (ui.landscape_workaround, "landscape-compatibility-workaround"),
+        ]
+        return widgets_with_settings
 
-    def _load_printer_settings(self, settings: configparser.ConfigParser):
+    def load(self, settings: configparser.ConfigParser):
         section = settings["printer"]
         for widget, setting in self._get_printer_settings_widgets():
             widget.setChecked(section.getboolean(setting))
 
     def save(self):
-        ui = self.ui
-        ui.page_configuration_group_box.save_document_settings_to_config()
-        mtg_proxy_printer.settings.settings["documents"]["pdf-page-count-limit"] = str(
-            ui.pdf_page_count_limit.value())
-        self._save_printer_settings()
-
-    def _save_printer_settings(self):
         section = mtg_proxy_printer.settings.settings["printer"]
         for widget, setting in self._get_printer_settings_widgets():
             section[setting] = str(widget.isChecked())
 
-    def _get_printer_settings_widgets(self):
-        ui = self.ui
-        widgets_with_settings: typing.List[typing.Tuple[QCheckBox, str]] = [
-            (ui.printer_use_borderless_printing, "borderless-printing")
-        ]
-        return widgets_with_settings
-
     def highlight_differing_settings(self, settings: configparser.ConfigParser):
-        ui = self.ui
-        ui.page_configuration_group_box.highlight_differing_settings(settings)
         section = settings["printer"]
         for widget, setting in self._get_printer_settings_widgets():
             if section.getboolean(setting) != widget.isChecked():
                 highlight_widget(widget)
-        section = settings["documents"]
+
+
+class PDFSettingsPage(Page):
+    display_metadata = PageMetadata("PDF export settings", "viewpdf", "Configure the PDF export")
+
+    def __init__(self, parent=None, flags=Qt.WindowFlags()):
+        super().__init__(parent, flags)
+        self.ui = ui = Ui_PDFSettingsPage()
+        ui.setupUi(self)
+
+    def load(self, settings: configparser.ConfigParser):
+        ui = self.ui
+        section = settings["pdf-export"]
+        ui.pdf_page_count_limit.setValue(section.getint("pdf-page-count-limit"))
+        ui.pdf_save_path.setText(section["pdf-export-path"])
+        ui.landscape_workaround.setChecked(section.getboolean("landscape-compatibility-workaround"))
+
+    def save(self):
+        ui = self.ui
+        section = mtg_proxy_printer.settings.settings["pdf-export"]
+        section["pdf-page-count-limit"] = str(ui.pdf_page_count_limit.value())
+        section["pdf-export-path"] = ui.pdf_save_path.text()
+        section["landscape-compatibility-workaround"] = str(ui.landscape_workaround.isChecked())
+
+    def highlight_differing_settings(self, settings: configparser.ConfigParser):
+        ui = self.ui
+        section = settings["pdf-export"]
         if section.getint("pdf-page-count-limit") != ui.pdf_page_count_limit.value():
             highlight_widget(ui.pdf_page_count_limit)
+        if ui.pdf_save_path.text() != section["pdf-export-path"]:
+            highlight_widget(ui.pdf_save_path)
+        if ui.landscape_workaround.isChecked() != section.getboolean("landscape-compatibility-workaround"):
+            highlight_widget(ui.landscape_workaround)
 
+    @Slot()
+    def on_pdf_save_path_browse_button_clicked(self):
+        logger.debug("User about to select a new default PDF document export path.")
+        if location := QFileDialog.getExistingDirectory(self, "Select default PDF export location"):
+            logger.info("User selected a new default PDF document export path.")
+            self.ui.pdf_save_path.setText(location)
+        else:
+            logger.debug("User cancelled path selection")
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/units_and_sizes.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/units_and_sizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """Contains some constants, like the card size"""
 import enum
 import re
 import typing
 try:
     from typing import NotRequired
 except ImportError:  # Compatibility with Python < 3.11
-    from typing import Optional as NotRequired
+    from typing_extensions import NotRequired
 
 import pint
 from PyQt5.QtCore import QSize
 
 unit_registry = pint.UnitRegistry()
 RESOLUTION: pint.Quantity = unit_registry("300dots/inch")
 DEFAULT_SAVE_SUFFIX = "mtgproxies"
```

### Comparing `MTGProxyPrinter-0.28.0/mtg_proxy_printer/update_checker.py` & `mtgproxyprinter-0.28.1/mtg_proxy_printer/update_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             except (urllib.error.URLError, socket.timeout, ijson.IncompleteJSONError) as e:
                 logger.warning(f"Failed to read update from mirror {mirror}. Reason: {e}")
                 continue
         return tags
 
     def _read_available_application_versions_from_mirror(self, mirror):
         data, _ = self.read_from_url(f"{mirror}/json/tag/list/")
-        items = ijson.items(data, "payload.tags.item")
+        items = ijson.items(data, "payload.tags.item", use_float=True)
         matches = filter(
             None,
             map(VERSION_TAG_MATCHER.fullmatch, items)
         )
         return natural_sorted((match["version"] for match in matches), reverse=True)
```

