# Comparing `tmp/evariste-1.2.0.tar.gz` & `tmp/evariste-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evariste-1.2.0.tar", last modified: Sat Oct  7 10:29:58 2023, max compression
+gzip compressed data, was "evariste-1.2.1.tar", last modified: Mon May  6 21:26:54 2024, max compression
```

## Comparing `evariste-1.2.0.tar` & `evariste-1.2.1.tar`

### file list

```diff
@@ -1,497 +1,497 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/
--rw-r--r--   0 louis     (1000) louis     (1000)      192 2022-01-31 16:27:08.000000 evariste-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 louis     (1000) louis     (1000)      196 2022-10-09 21:04:01.000000 evariste-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 louis     (1000) louis     (1000)      336 2022-10-11 18:56:35.000000 evariste-1.2.0/.pylintrc
--rw-r--r--   0 louis     (1000) louis     (1000)      351 2023-10-06 21:25:55.000000 evariste-1.2.0/.readthedocs.yaml
--rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:55:24.000000 evariste-1.2.0/AUTHORS
--rw-r--r--   0 louis     (1000) louis     (1000)    10651 2023-10-07 10:23:42.000000 evariste-1.2.0/CHANGELOG.md
--rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:55:24.000000 evariste-1.2.0/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)     2525 2023-10-07 10:29:58.901736 evariste-1.2.0/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     1082 2022-03-07 21:40:12.000000 evariste-1.2.0/README.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.741734 evariste-1.2.0/bin/
--rwxr-xr-x   0 louis     (1000) louis     (1000)      164 2020-06-21 10:55:24.000000 evariste-1.2.0/bin/evariste
--rwxr-xr-x   0 louis     (1000) louis     (1000)      151 2020-06-21 10:55:24.000000 evariste-1.2.0/bin/evs
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.749734 evariste-1.2.0/doc/
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:24.000000 evariste-1.2.0/doc/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)     6770 2020-06-21 10:55:24.000000 evariste-1.2.0/doc/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)     8743 2023-10-07 10:27:34.000000 evariste-1.2.0/doc/conf.py
--rw-r--r--   0 louis     (1000) louis     (1000)      878 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/evs.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     2030 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/index.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      419 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/install.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.753734 evariste-1.2.0/doc/lib/
--rw-r--r--   0 louis     (1000) louis     (1000)       82 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/builder.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       76 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/hooks.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.753734 evariste-1.2.0/doc/lib/plugins/
--rw-r--r--   0 louis     (1000) louis     (1000)      104 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins/action.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.757734 evariste-1.2.0/doc/lib/plugins/renderer/
--rw-r--r--   0 louis     (1000) louis     (1000)      411 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins/renderer/html.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      429 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins/renderer/jinja2.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      254 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins/renderer.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      364 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins/vcs.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      206 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/plugins.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       79 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/shared.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       73 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/tree.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       76 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib/utils.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      244 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/lib.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.757734 evariste-1.2.0/doc/plugins/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.761734 evariste-1.2.0/doc/plugins/action/
--rw-r--r--   0 louis     (1000) louis     (1000)     3160 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/action/autocommand.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     3106 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/action/command.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      522 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/action/make.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      340 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/action/raw.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     2730 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/action.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     1832 2022-10-11 19:56:40.000000 evariste-1.2.0/doc/plugins/logging.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      435 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/mandatory.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     1376 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/misc.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.761734 evariste-1.2.0/doc/plugins/renderer/
--rw-r--r--   0 louis     (1000) louis     (1000)     2874 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/renderer/html.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     2888 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/renderer/htmlplus.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     2663 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/renderer/jinja2.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     1089 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/renderer/text.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      462 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/renderer.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      682 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/vcs.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.765734 evariste-1.2.0/doc/plugins/write/
--rw-r--r--   0 louis     (1000) louis     (1000)     1366 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/write/action.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     6209 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/write/hooks.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      881 2022-03-07 21:41:20.000000 evariste-1.2.0/doc/plugins/write/renderer.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      209 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/plugins/write/vcs.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     5819 2022-03-07 21:42:30.000000 evariste-1.2.0/doc/plugins/write.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      657 2022-10-09 21:04:17.000000 evariste-1.2.0/doc/plugins.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      104 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/requirements.txt
--rw-r--r--   0 louis     (1000) louis     (1000)     2332 2022-03-07 21:40:12.000000 evariste-1.2.0/doc/usecase.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.769734 evariste-1.2.0/doc/user/
--rw-r--r--   0 louis     (1000) louis     (1000)     2045 2022-10-11 19:36:18.000000 evariste-1.2.0/doc/user/evsconfig.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      726 2022-03-07 21:40:13.000000 evariste-1.2.0/doc/user/format.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     4212 2022-03-07 21:42:35.000000 evariste-1.2.0/doc/user/quickstart.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     3134 2022-03-07 21:42:44.000000 evariste-1.2.0/doc/user/setup.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     1836 2022-03-07 21:40:13.000000 evariste-1.2.0/doc/user/source.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      352 2022-10-09 21:04:17.000000 evariste-1.2.0/doc/user/usage.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      175 2022-03-07 21:40:13.000000 evariste-1.2.0/doc/user.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.773734 evariste-1.2.0/evariste/
--rw-r--r--   0 louis     (1000) louis     (1000)      908 2023-10-07 10:27:34.000000 evariste-1.2.0/evariste/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)      841 2022-03-07 21:50:39.000000 evariste-1.2.0/evariste/__main__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     4166 2022-03-07 22:10:54.000000 evariste-1.2.0/evariste/builder.py
--rw-r--r--   0 louis     (1000) louis     (1000)     4824 2022-03-16 10:40:18.000000 evariste-1.2.0/evariste/cache.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1131 2020-06-21 10:55:25.000000 evariste-1.2.0/evariste/errors.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.777734 evariste-1.2.0/evariste/evs/
--rw-r--r--   0 louis     (1000) louis     (1000)      711 2020-06-21 10:55:25.000000 evariste-1.2.0/evariste/evs/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1870 2022-03-07 22:21:08.000000 evariste-1.2.0/evariste/evs/__main__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.781734 evariste-1.2.0/evariste/evs/cache/
--rw-r--r--   0 louis     (1000) louis     (1000)      727 2020-06-21 10:55:25.000000 evariste-1.2.0/evariste/evs/cache/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     7140 2022-03-07 21:52:03.000000 evariste-1.2.0/evariste/evs/cache/__main__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.781734 evariste-1.2.0/evariste/evs/compile/
--rw-r--r--   0 louis     (1000) louis     (1000)      737 2020-06-21 10:55:25.000000 evariste-1.2.0/evariste/evs/compile/__init__.py
--rwxr-xr-x   0 louis     (1000) louis     (1000)     2003 2022-10-11 18:56:27.000000 evariste-1.2.0/evariste/evs/compile/__main__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     3595 2022-10-12 19:47:40.000000 evariste-1.2.0/evariste/evs/compile/options.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.781734 evariste-1.2.0/evariste/evs/plugins/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:25.000000 evariste-1.2.0/evariste/evs/plugins/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2751 2022-03-07 21:52:44.000000 evariste-1.2.0/evariste/evs/plugins/__main__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5450 2022-03-07 21:40:13.000000 evariste-1.2.0/evariste/hooks.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.785735 evariste-1.2.0/evariste/plugins/
--rw-r--r--   0 louis     (1000) louis     (1000)    16929 2022-10-11 18:54:42.000000 evariste-1.2.0/evariste/plugins/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.785735 evariste-1.2.0/evariste/plugins/action/
--rw-r--r--   0 louis     (1000) louis     (1000)     4193 2022-03-07 22:28:33.000000 evariste-1.2.0/evariste/plugins/action/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     3713 2022-03-07 22:08:22.000000 evariste-1.2.0/evariste/plugins/action/autocommand.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1891 2022-03-07 22:08:21.000000 evariste-1.2.0/evariste/plugins/action/cached.py
--rw-r--r--   0 louis     (1000) louis     (1000)     6763 2023-10-06 20:57:24.000000 evariste-1.2.0/evariste/plugins/action/command.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1601 2022-03-07 21:55:42.000000 evariste-1.2.0/evariste/plugins/action/make.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2075 2022-03-07 21:56:01.000000 evariste-1.2.0/evariste/plugins/action/nothing.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5178 2022-03-07 21:56:43.000000 evariste-1.2.0/evariste/plugins/changed.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2342 2022-03-07 22:33:02.000000 evariste-1.2.0/evariste/plugins/copy.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2830 2022-03-07 22:33:02.000000 evariste-1.2.0/evariste/plugins/debug.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5408 2022-10-12 20:12:08.000000 evariste-1.2.0/evariste/plugins/logging.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.785735 evariste-1.2.0/evariste/plugins/renderer/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-01-30 14:06:20.000000 evariste-1.2.0/evariste/plugins/renderer/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/html/
--rw-r--r--   0 louis     (1000) louis     (1000)     1855 2022-10-11 18:08:13.000000 evariste-1.2.0/evariste/plugins/renderer/html/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.693733 evariste-1.2.0/evariste/plugins/renderer/html/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/html/data/templates/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/html/data/templates/file/
--rw-r--r--   0 louis     (1000) louis     (1000)      128 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/html/data/templates/file/default.html
--rw-r--r--   0 louis     (1000) louis     (1000)      274 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/html/data/templates/file/image.html
--rw-r--r--   0 louis     (1000) louis     (1000)     1122 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/html/data/templates/tree.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/html/file/
--rw-r--r--   0 louis     (1000) louis     (1000)     1514 2022-03-07 21:59:37.000000 evariste-1.2.0/evariste/plugins/renderer/html/file/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1076 2022-03-07 22:00:13.000000 evariste-1.2.0/evariste/plugins/renderer/html/file/image.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/html/readme/
--rw-r--r--   0 louis     (1000) louis     (1000)     1201 2022-03-07 22:00:55.000000 evariste-1.2.0/evariste/plugins/renderer/html/readme/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1108 2022-03-07 22:01:08.000000 evariste-1.2.0/evariste/plugins/renderer/html/readme/mdwn.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1593 2022-03-07 22:01:20.000000 evariste-1.2.0/evariste/plugins/renderer/html/readme/rst.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.789734 evariste-1.2.0/evariste/plugins/renderer/htmlplus/
--rw-r--r--   0 louis     (1000) louis     (1000)     2763 2022-10-11 18:08:13.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.697733 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.793735 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/
--rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/COPYING
--rw-r--r--   0 louis     (1000) louis     (1000)     2386 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/application-x-zerosize.png
--rw-r--r--   0 louis     (1000) louis     (1000)     1527 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/dialog-error.png
--rw-r--r--   0 louis     (1000) louis     (1000)     2901 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/dialog-ok-apply.png
--rw-r--r--   0 louis     (1000) louis     (1000)     2386 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/file.png
--rw-r--r--   0 louis     (1000) louis     (1000)     2355 2020-06-21 10:55:26.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/folder-open.png
--rw-r--r--   0 louis     (1000) louis     (1000)     2169 2020-06-21 10:55:27.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/folder.png
--rw-r--r--   0 louis     (1000) louis     (1000)     7651 2020-06-21 10:55:27.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/lgpl-3.0.txt
--rw-r--r--   0 louis     (1000) louis     (1000)     2629 2020-06-21 10:55:27.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/tree.css
--rw-r--r--   0 louis     (1000) louis     (1000)      488 2020-06-21 10:55:27.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/tree.js
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.793735 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/templates/
--rw-r--r--   0 louis     (1000) louis     (1000)     3581 2022-01-30 00:03:37.000000 evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/templates/page.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.793735 evariste-1.2.0/evariste/plugins/renderer/jinja2/
--rw-r--r--   0 louis     (1000) louis     (1000)    10446 2022-10-11 19:24:29.000000 evariste-1.2.0/evariste/plugins/renderer/jinja2/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2966 2022-03-07 22:33:16.000000 evariste-1.2.0/evariste/plugins/renderer/jinja2/file.py
--rw-r--r--   0 louis     (1000) louis     (1000)     4322 2022-03-07 22:33:16.000000 evariste-1.2.0/evariste/plugins/renderer/jinja2/readme.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5759 2023-10-06 20:56:16.000000 evariste-1.2.0/evariste/plugins/renderer/text.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2919 2022-03-07 22:33:02.000000 evariste-1.2.0/evariste/plugins/tree.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.793735 evariste-1.2.0/evariste/plugins/vcs/
--rw-r--r--   0 louis     (1000) louis     (1000)     2923 2022-10-11 19:25:02.000000 evariste-1.2.0/evariste/plugins/vcs/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1413 2022-03-07 22:05:33.000000 evariste-1.2.0/evariste/plugins/vcs/fs.py
--rw-r--r--   0 louis     (1000) louis     (1000)     3297 2022-03-07 22:05:44.000000 evariste-1.2.0/evariste/plugins/vcs/git.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1153 2022-03-07 22:05:59.000000 evariste-1.2.0/evariste/plugins/vcs/none.py
--rw-r--r--   0 louis     (1000) louis     (1000)     6208 2022-03-07 22:08:23.000000 evariste-1.2.0/evariste/setup.py
--rw-r--r--   0 louis     (1000) louis     (1000)     6587 2023-10-06 20:45:18.000000 evariste-1.2.0/evariste/shared.py
--rw-r--r--   0 louis     (1000) louis     (1000)    22939 2022-03-07 22:32:26.000000 evariste-1.2.0/evariste/tree.py
--rw-r--r--   0 louis     (1000) louis     (1000)     8546 2022-10-11 19:23:56.000000 evariste-1.2.0/evariste/utils.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.777734 evariste-1.2.0/evariste.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)     2525 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)    15075 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       97 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/entry_points.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-03-07 22:34:08.000000 evariste-1.2.0/evariste.egg-info/not-zip-safe
--rw-r--r--   0 louis     (1000) louis     (1000)       65 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/requires.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        9 2023-10-07 10:29:58.000000 evariste-1.2.0/evariste.egg-info/top_level.txt
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.797735 evariste-1.2.0/examples/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:27.000000 evariste-1.2.0/examples/.gitignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.797735 evariste-1.2.0/examples/example1/
--rw-r--r--   0 louis     (1000) louis     (1000)       58 2020-06-21 10:55:27.000000 evariste-1.2.0/examples/example1/.gitignore
--rwxr-xr-x   0 louis     (1000) louis     (1000)      157 2020-06-21 10:55:27.000000 evariste-1.2.0/examples/example1/compile.sh
--rw-r--r--   0 louis     (1000) louis     (1000)     1417 2022-10-11 19:55:59.000000 evariste-1.2.0/examples/example1/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.805735 evariste-1.2.0/examples/example1/repository/
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:27.000000 evariste-1.2.0/examples/example1/repository/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       46 2020-06-21 10:55:27.000000 evariste-1.2.0/examples/example1/repository/.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/.noaction2.tex.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.805735 evariste-1.2.0/examples/example1/repository/autocommand/
--rw-r--r--   0 louis     (1000) louis     (1000)       33 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/autocommand/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/autocommand/README.md
--rw-r--r--   0 louis     (1000) louis     (1000)     2482 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/autocommand/image.xcf
--rw-r--r--   0 louis     (1000) louis     (1000)    11216 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/autocommand/report.ods
--rw-r--r--   0 louis     (1000) louis     (1000)    20314 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/autocommand/report2.fods
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.809735 evariste-1.2.0/examples/example1/repository/depends/
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends/depends-sub.tex
--rw-r--r--   0 louis     (1000) louis     (1000)        7 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends/depends2.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends/plop.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      154 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends-nostrace.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       36 2022-02-16 11:25:41.000000 evariste-1.2.0/examples/example1/repository/depends-nostrace.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)      127 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends-nostrace.tex.html
--rw-r--r--   0 louis     (1000) louis     (1000)    20623 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends.png
--rw-r--r--   0 louis     (1000) louis     (1000)      154 2022-02-23 21:42:33.000000 evariste-1.2.0/examples/example1/repository/depends.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      191 2022-03-07 21:40:13.000000 evariste-1.2.0/examples/example1/repository/depends.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)      105 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends.tex.html
--rw-r--r--   0 louis     (1000) louis     (1000)       93 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/depends2.tex
--rw-r--r--   0 louis     (1000) louis     (1000)     1825 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/dummy.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)     1825 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/dummy.pdf.ignore
--rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/error1.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-01-29 23:58:02.000000 evariste-1.2.0/examples/example1/repository/error1.tex.html
--rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/error2.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/error2.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       47 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/error2.tex.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.813735 evariste-1.2.0/examples/example1/repository/foo/
--rw-r--r--   0 louis     (1000) louis     (1000)       30 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        9 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)       31 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/.foo.png.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       13 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       66 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/README.html
--rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:28.000000 evariste-1.2.0/examples/example1/repository/foo/foo-jpg1.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo-jpg2.txt
--rw-r--r--   0 louis     (1000) louis     (1000)    13017 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo.jpg
--rw-r--r--   0 louis     (1000) louis     (1000)       98 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo.jpg.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)    28286 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo.png
--rw-r--r--   0 louis     (1000) louis     (1000)    11876 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo.svg
--rw-r--r--   0 louis     (1000) louis     (1000)  1024360 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/foo.tiff
--rw-r--r--   0 louis     (1000) louis     (1000)      113 2022-03-07 21:40:13.000000 evariste-1.2.0/examples/example1/repository/foo/foo.tiff.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)    28286 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/foo/ignored.png
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.817735 evariste-1.2.0/examples/example1/repository/gcc/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/gcc/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/gcc/.hello.c.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       88 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/gcc/hello.c
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.821735 evariste-1.2.0/examples/example1/repository/multi/
--rw-r--r--   0 louis     (1000) louis     (1000)       36 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       30 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)    20623 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/command.png
--rw-r--r--   0 louis     (1000) louis     (1000)      139 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/command.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       99 2022-03-07 21:40:13.000000 evariste-1.2.0/examples/example1/repository/multi/command.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)     1218 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/index.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      144 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/multi/multicommand.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      156 2022-03-07 21:40:13.000000 evariste-1.2.0/examples/example1/repository/multi/multicommand.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/noaction1.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/noaction1.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/noaction1.tex.html
--rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/noaction2.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/noaction2.tex.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.821735 evariste-1.2.0/examples/example1/repository/parent/
--rw-r--r--   0 louis     (1000) louis     (1000)      126 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/parent/parent.tex
--rw-r--r--   0 louis     (1000) louis     (1000)       99 2022-03-07 21:40:13.000000 evariste-1.2.0/examples/example1/repository/parent/parent.tex.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)     3024 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/report.pdf
--rw-r--r--   0 louis     (1000) louis     (1000)       43 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/report.pdf.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.0/examples/example1/repository/single.tex
--rw-r--r--   0 louis     (1000) louis     (1000)      378 2023-10-06 21:35:31.000000 evariste-1.2.0/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)       65 2022-10-10 05:20:51.000000 evariste-1.2.0/requirements.txt
--rw-r--r--   0 louis     (1000) louis     (1000)     1525 2023-10-07 10:29:58.905736 evariste-1.2.0/setup.cfg
--rwxr-xr-x   0 louis     (1000) louis     (1000)       93 2020-06-21 10:55:29.000000 evariste-1.2.0/setup.py
--rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.0/stdeb.cfg
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.821735 evariste-1.2.0/test/
--rw-r--r--   0 louis     (1000) louis     (1000)      960 2020-06-21 10:55:29.000000 evariste-1.2.0/test/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.821735 evariste-1.2.0/test/test_compile/
--rw-r--r--   0 louis     (1000) louis     (1000)     5366 2022-02-16 21:32:14.000000 evariste-1.2.0/test/test_compile/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.721733 evariste-1.2.0/test/test_compile/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.821735 evariste-1.2.0/test/test_compile/data/actions/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:29.000000 evariste-1.2.0/test/test_compile/data/actions/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       38 2020-06-21 10:55:29.000000 evariste-1.2.0/test/test_compile/data/actions/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      249 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/actions/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.825735 evariste-1.2.0/test/test_compile/data/actions/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.825735 evariste-1.2.0/test/test_compile/data/actions/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:29.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:29.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/command-in.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:29.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/command-out.txt
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.825735 evariste-1.2.0/test/test_compile/data/actions/expected/html/make/
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/make/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/make/tagada.aaa
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/make/tagada.grepa
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/raw
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/toto.sort
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/html/toto.sorted
--rw-r--r--   0 louis     (1000) louis     (1000)     1025 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.829735 evariste-1.2.0/test/test_compile/data/actions/source/
--rw-r--r--   0 louis     (1000) louis     (1000)      143 2022-02-16 11:25:41.000000 evariste-1.2.0/test/test_compile/data/actions/source/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/command-in.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/command-in.txt.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.829735 evariste-1.2.0/test/test_compile/data/actions/source/make/
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/make/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/make/tagada.grepa
--rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/make/tagada.grepa.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/raw
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/raw.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/actions/source/toto.sort
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.829735 evariste-1.2.0/test/test_compile/data/config/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       21 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      202 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/config/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.829735 evariste-1.2.0/test/test_compile/data/config/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.833735 evariste-1.2.0/test/test_compile/data/config/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/aa
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/bb
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/bbb
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.833735 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/aa
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/bb
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.833735 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/dir/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/dir/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/dir1/dir/bbb
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.833735 evariste-1.2.0/test/test_compile/data/config/expected/html/dir2/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/html/dir2/bbb
--rw-r--r--   0 louis     (1000) louis     (1000)      992 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/config/source/
--rw-r--r--   0 louis     (1000) louis     (1000)      118 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/source/.aaa.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        7 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/source/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/source/.gitignore.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.0/test/test_compile/data/config/source/aa
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)       99 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/aaa.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/config/source/dir1/
--rw-r--r--   0 louis     (1000) louis     (1000)      124 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir1/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir1/aa
--rw-r--r--   0 louis     (1000) louis     (1000)       70 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir1/aa.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/config/source/dir1/dir/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir1/dir/aaa
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/config/source/dir2/
--rw-r--r--   0 louis     (1000) louis     (1000)      131 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir2/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/config/source/dir2/bbb
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/empty/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/empty/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/empty/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      180 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/empty/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/empty/expected/
--rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/empty/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.837735 evariste-1.2.0/test/test_compile/data/empty/source/
--rw-r--r--   0 louis     (1000) louis     (1000)       15 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/empty/source/README.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.841735 evariste-1.2.0/test/test_compile/data/extends/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       32 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      228 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/extends/evariste.setup
--rw-r--r--   0 louis     (1000) louis     (1000)      154 2022-02-16 11:25:41.000000 evariste-1.2.0/test/test_compile/data/extends/evariste2.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.841735 evariste-1.2.0/test/test_compile/data/extends/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.841735 evariste-1.2.0/test/test_compile/data/extends/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)       28 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/html/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/html/command-in.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/html/command-out.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/html/toto.sort
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/html/toto.sorted
--rw-r--r--   0 louis     (1000) louis     (1000)      504 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/extends/source/
--rw-r--r--   0 louis     (1000) louis     (1000)       28 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/source/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/source/command-in.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/source/command-in.txt.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/extends/source/toto.sort
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/ignore/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       20 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      201 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/ignore/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/ignore/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/ignore/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/aaa.out
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir1/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir1/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir1/aaa.out
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.845735 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir2/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir2/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/html/dir2/aaa.out
--rw-r--r--   0 louis     (1000) louis     (1000)      664 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.849736 evariste-1.2.0/test/test_compile/data/ignore/source/
--rw-r--r--   0 louis     (1000) louis     (1000)      136 2020-06-21 10:55:31.000000 evariste-1.2.0/test/test_compile/data/ignore/source/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/.ignored2.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/aaa
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.849736 evariste-1.2.0/test/test_compile/data/ignore/source/dir1/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir1/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir1/ignored1
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir1/ignored2
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.849736 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/.ignored2.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/aaa
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/ignored1
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/ignored1.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/dir2/ignored2
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.849736 evariste-1.2.0/test/test_compile/data/ignore/source/empty/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/empty/ignored
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/empty/ignored.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/ignored1
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/ignored1.evsignore
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/ignore/source/ignored2
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/misc/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       26 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      205 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/misc/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/misc/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/misc/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)     4058 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/expected/html/colors.png
--rw-r--r--   0 louis     (1000) louis     (1000)      262 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/misc/source/
--rw-r--r--   0 louis     (1000) louis     (1000)     4058 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/source/colors.png
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/misc/source/colors.png.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/targets/
--rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)       23 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/description.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      201 2022-10-13 19:36:02.000000 evariste-1.2.0/test/test_compile/data/targets/evariste.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.853736 evariste-1.2.0/test/test_compile/data/targets/expected/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.865736 evariste-1.2.0/test/test_compile/data/targets/expected/html/
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/one
--rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/one.a
--rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/two
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/two.a
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/two.b
--rw-r--r--   0 louis     (1000) louis     (1000)       10 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/html/zero
--rw-r--r--   0 louis     (1000) louis     (1000)      586 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/expected/index.html
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.865736 evariste-1.2.0/test/test_compile/data/targets/source/
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/one
--rw-r--r--   0 louis     (1000) louis     (1000)       95 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/one.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/two
--rw-r--r--   0 louis     (1000) louis     (1000)      126 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/two.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       10 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/zero
--rw-r--r--   0 louis     (1000) louis     (1000)       69 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_compile/data/targets/source/zero.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)     1358 2021-11-27 16:46:49.000000 evariste-1.2.0/test/test_doctest.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.865736 evariste-1.2.0/test/test_ignore/
--rw-r--r--   0 louis     (1000) louis     (1000)     2328 2022-10-13 19:38:46.000000 evariste-1.2.0/test/test_ignore/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.865736 evariste-1.2.0/test/test_ignore/data/
--rw-r--r--   0 louis     (1000) louis     (1000)       18 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/.gitignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.869736 evariste-1.2.0/test/test_ignore/data/tree/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/.bar.evsignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.869736 evariste-1.2.0/test/test_ignore/data/tree/a/
--rw-r--r--   0 louis     (1000) louis     (1000)        6 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/a/.evsignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.877736 evariste-1.2.0/test/test_ignore/data/tree/a/b/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/a/b/plop.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/a/b/pom.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/a/b/tagada.md
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/bar
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/baz
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.877736 evariste-1.2.0/test/test_ignore/data/tree/c/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/c/tata.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/c/titi.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/c/toto.txt
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.725734 evariste-1.2.0/test/test_ignore/data/tree/d/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.877736 evariste-1.2.0/test/test_ignore/data/tree/d/d/
--rw-r--r--   0 louis     (1000) louis     (1000)       22 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/.evsignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.881736 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/
--rw-r--r--   0 louis     (1000) louis     (1000)       12 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/.evsignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.881736 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.881736 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/d/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/d/tata.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/d/titi.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/d/toto.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/tata.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/titi.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/d/toto.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/tata.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/titi.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/d/toto.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/tata.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/titi.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/d/d/toto.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/foo
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.0/test/test_ignore/data/tree/foo.evsignore
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.893736 evariste-1.2.0/test/test_plugins/
--rw-r--r--   0 louis     (1000) louis     (1000)     1663 2022-10-11 19:58:47.000000 evariste-1.2.0/test/test_plugins/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_plugins/depends/
--rw-r--r--   0 louis     (1000) louis     (1000)     2349 2022-10-10 19:39:17.000000 evariste-1.2.0/test/test_plugins/depends/depends.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.725734 evariste-1.2.0/test/test_plugins/libdirs/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_plugins/libdirs/plug ins/
--rw-r--r--   0 louis     (1000) louis     (1000)      819 2022-02-23 17:53:35.000000 evariste-1.2.0/test/test_plugins/libdirs/plug ins/bar.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_plugins/libdirs/plugins/
--rw-r--r--   0 louis     (1000) louis     (1000)      819 2022-02-23 17:53:35.000000 evariste-1.2.0/test/test_plugins/libdirs/plugins/foo.py
--rw-r--r--   0 louis     (1000) louis     (1000)     5210 2022-10-11 18:13:51.000000 evariste-1.2.0/test/test_plugins/test_depends.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2981 2022-03-07 21:45:17.000000 evariste-1.2.0/test/test_plugins/test_libdirs.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/
--rw-r--r--   0 louis     (1000) louis     (1000)     2413 2022-03-07 21:45:17.000000 evariste-1.2.0/test/test_recursive/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/a/
--rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/a/.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/a/aa/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/a/aa/aaa
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/b/
--rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/b/.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/b/bb/
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/b/bb/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/b/bb/bbb
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/c/
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/c/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/c/cc
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.897736 evariste-1.2.0/test/test_recursive/data/d/
--rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/d/.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_recursive/data/d/dd/
--rw-r--r--   0 louis     (1000) louis     (1000)       15 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/d/dd/.evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/d/dd/ddd
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_recursive/data/e/
--rw-r--r--   0 louis     (1000) louis     (1000)       46 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/e/e.norec-evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)       61 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/e/e.rec-evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/e/ee
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.729734 evariste-1.2.0/test/test_recursive/data/f/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_recursive/data/f/ff/
--rw-r--r--   0 louis     (1000) louis     (1000)       35 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/f/ff/evsconfig
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/f/ff/fff
--rw-r--r--   0 louis     (1000) louis     (1000)       51 2022-02-16 19:36:36.000000 evariste-1.2.0/test/test_recursive/data/f.evsconfig
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_run/
--rw-r--r--   0 louis     (1000) louis     (1000)     5375 2023-10-06 20:57:28.000000 evariste-1.2.0/test/test_run/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_setup/
--rw-r--r--   0 louis     (1000) louis     (1000)     5461 2022-02-23 17:53:35.000000 evariste-1.2.0/test/test_setup/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.733734 evariste-1.2.0/test/test_setup/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_setup/data/cycle/
--rw-r--r--   0 louis     (1000) louis     (1000)       38 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_setup/data/cycle/a.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_setup/data/cycle/b/
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_setup/data/cycle/b/b.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_setup/data/cycle/c/
--rw-r--r--   0 louis     (1000) louis     (1000)       39 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_setup/data/cycle/c/c.setup
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-10-07 10:29:58.901736 evariste-1.2.0/test/test_setup/data/empty/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_setup/data/empty/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)     3381 2022-03-07 21:45:17.000000 evariste-1.2.0/test/test_shared.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1506 2020-06-21 10:55:32.000000 evariste-1.2.0/test/test_utils.py
--rw-r--r--   0 louis     (1000) louis     (1000)      667 2023-10-06 21:35:31.000000 evariste-1.2.0/tox.ini
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/
+-rw-r--r--   0 louis     (1000) louis     (1000)      192 2022-01-31 16:27:08.000000 evariste-1.2.1/.gitlab-ci.yml
+-rw-r--r--   0 louis     (1000) louis     (1000)      195 2024-05-05 18:18:51.000000 evariste-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 louis     (1000) louis     (1000)      336 2022-10-11 18:56:35.000000 evariste-1.2.1/.pylintrc
+-rw-r--r--   0 louis     (1000) louis     (1000)      351 2023-10-06 21:25:55.000000 evariste-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:55:24.000000 evariste-1.2.1/AUTHORS
+-rw-r--r--   0 louis     (1000) louis     (1000)    10781 2024-05-06 21:15:38.000000 evariste-1.2.1/CHANGELOG.md
+-rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:55:24.000000 evariste-1.2.1/LICENSE
+-rw-r--r--   0 louis     (1000) louis     (1000)     2525 2024-05-06 21:26:54.782761 evariste-1.2.1/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)     1082 2022-03-07 21:40:12.000000 evariste-1.2.1/README.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.706760 evariste-1.2.1/bin/
+-rwxr-xr-x   0 louis     (1000) louis     (1000)      164 2020-06-21 10:55:24.000000 evariste-1.2.1/bin/evariste
+-rwxr-xr-x   0 louis     (1000) louis     (1000)      151 2020-06-21 10:55:24.000000 evariste-1.2.1/bin/evs
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.710760 evariste-1.2.1/doc/
+-rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:24.000000 evariste-1.2.1/doc/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)     6770 2020-06-21 10:55:24.000000 evariste-1.2.1/doc/Makefile
+-rw-r--r--   0 louis     (1000) louis     (1000)     8743 2024-05-06 21:15:53.000000 evariste-1.2.1/doc/conf.py
+-rw-r--r--   0 louis     (1000) louis     (1000)      878 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/evs.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     2030 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/index.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      419 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/install.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.710760 evariste-1.2.1/doc/lib/
+-rw-r--r--   0 louis     (1000) louis     (1000)       82 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/builder.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)       76 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/hooks.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.710760 evariste-1.2.1/doc/lib/plugins/
+-rw-r--r--   0 louis     (1000) louis     (1000)      104 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins/action.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.710760 evariste-1.2.1/doc/lib/plugins/renderer/
+-rw-r--r--   0 louis     (1000) louis     (1000)      411 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins/renderer/html.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      429 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins/renderer/jinja2.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      254 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins/renderer.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      364 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins/vcs.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      206 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/plugins.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)       79 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/shared.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)       73 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/tree.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)       76 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib/utils.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      244 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/lib.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.714760 evariste-1.2.1/doc/plugins/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.714760 evariste-1.2.1/doc/plugins/action/
+-rw-r--r--   0 louis     (1000) louis     (1000)     3160 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/action/autocommand.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     3106 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/action/command.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      522 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/action/make.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      340 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/action/raw.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     2730 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/action.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     1832 2022-10-11 19:56:40.000000 evariste-1.2.1/doc/plugins/logging.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      435 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/mandatory.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     1376 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/misc.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.714760 evariste-1.2.1/doc/plugins/renderer/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2874 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/renderer/html.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     2888 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/renderer/htmlplus.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     2663 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/renderer/jinja2.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     1089 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/renderer/text.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      462 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/renderer.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      682 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/vcs.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.714760 evariste-1.2.1/doc/plugins/write/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1366 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/write/action.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     6209 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/write/hooks.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      881 2022-03-07 21:41:20.000000 evariste-1.2.1/doc/plugins/write/renderer.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      209 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/plugins/write/vcs.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     5819 2022-03-07 21:42:30.000000 evariste-1.2.1/doc/plugins/write.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      657 2022-10-09 21:04:17.000000 evariste-1.2.1/doc/plugins.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      104 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/requirements.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)     2332 2022-03-07 21:40:12.000000 evariste-1.2.1/doc/usecase.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.714760 evariste-1.2.1/doc/user/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2045 2022-10-11 19:36:18.000000 evariste-1.2.1/doc/user/evsconfig.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      726 2022-03-07 21:40:13.000000 evariste-1.2.1/doc/user/format.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     4212 2022-03-07 21:42:35.000000 evariste-1.2.1/doc/user/quickstart.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     3134 2022-03-07 21:42:44.000000 evariste-1.2.1/doc/user/setup.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)     1836 2022-03-07 21:40:13.000000 evariste-1.2.1/doc/user/source.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      352 2022-10-09 21:04:17.000000 evariste-1.2.1/doc/user/usage.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      175 2022-03-07 21:40:13.000000 evariste-1.2.1/doc/user.rst
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.718761 evariste-1.2.1/evariste/
+-rw-r--r--   0 louis     (1000) louis     (1000)      908 2024-05-06 21:16:47.000000 evariste-1.2.1/evariste/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)      841 2022-03-07 21:50:39.000000 evariste-1.2.1/evariste/__main__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     4166 2022-03-07 22:10:54.000000 evariste-1.2.1/evariste/builder.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     4824 2022-03-16 10:40:18.000000 evariste-1.2.1/evariste/cache.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1131 2020-06-21 10:55:25.000000 evariste-1.2.1/evariste/errors.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.722761 evariste-1.2.1/evariste/evs/
+-rw-r--r--   0 louis     (1000) louis     (1000)      711 2020-06-21 10:55:25.000000 evariste-1.2.1/evariste/evs/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1870 2022-03-07 22:21:08.000000 evariste-1.2.1/evariste/evs/__main__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.722761 evariste-1.2.1/evariste/evs/cache/
+-rw-r--r--   0 louis     (1000) louis     (1000)      727 2020-06-21 10:55:25.000000 evariste-1.2.1/evariste/evs/cache/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     7140 2022-03-07 21:52:03.000000 evariste-1.2.1/evariste/evs/cache/__main__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.722761 evariste-1.2.1/evariste/evs/compile/
+-rw-r--r--   0 louis     (1000) louis     (1000)      737 2020-06-21 10:55:25.000000 evariste-1.2.1/evariste/evs/compile/__init__.py
+-rwxr-xr-x   0 louis     (1000) louis     (1000)     2003 2022-10-11 18:56:27.000000 evariste-1.2.1/evariste/evs/compile/__main__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     3595 2022-10-12 19:47:40.000000 evariste-1.2.1/evariste/evs/compile/options.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.722761 evariste-1.2.1/evariste/evs/plugins/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:25.000000 evariste-1.2.1/evariste/evs/plugins/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2751 2022-03-07 21:52:44.000000 evariste-1.2.1/evariste/evs/plugins/__main__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     5450 2022-03-07 21:40:13.000000 evariste-1.2.1/evariste/hooks.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/
+-rw-r--r--   0 louis     (1000) louis     (1000)    16929 2022-10-11 18:54:42.000000 evariste-1.2.1/evariste/plugins/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/action/
+-rw-r--r--   0 louis     (1000) louis     (1000)     4193 2022-03-07 22:28:33.000000 evariste-1.2.1/evariste/plugins/action/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     3713 2022-03-07 22:08:22.000000 evariste-1.2.1/evariste/plugins/action/autocommand.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1891 2022-03-07 22:08:21.000000 evariste-1.2.1/evariste/plugins/action/cached.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     6763 2023-10-06 20:57:24.000000 evariste-1.2.1/evariste/plugins/action/command.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1601 2022-03-07 21:55:42.000000 evariste-1.2.1/evariste/plugins/action/make.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2075 2022-03-07 21:56:01.000000 evariste-1.2.1/evariste/plugins/action/nothing.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     5178 2022-03-07 21:56:43.000000 evariste-1.2.1/evariste/plugins/changed.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2342 2022-03-07 22:33:02.000000 evariste-1.2.1/evariste/plugins/copy.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2830 2022-03-07 22:33:02.000000 evariste-1.2.1/evariste/plugins/debug.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     5408 2022-10-12 20:12:08.000000 evariste-1.2.1/evariste/plugins/logging.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-01-30 14:06:20.000000 evariste-1.2.1/evariste/plugins/renderer/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1855 2022-10-11 18:08:13.000000 evariste-1.2.1/evariste/plugins/renderer/html/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.690760 evariste-1.2.1/evariste/plugins/renderer/html/data/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/html/data/templates/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/html/data/templates/file/
+-rw-r--r--   0 louis     (1000) louis     (1000)      128 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/html/data/templates/file/default.html
+-rw-r--r--   0 louis     (1000) louis     (1000)      274 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/html/data/templates/file/image.html
+-rw-r--r--   0 louis     (1000) louis     (1000)     1122 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/html/data/templates/tree.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/html/file/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1514 2022-03-07 21:59:37.000000 evariste-1.2.1/evariste/plugins/renderer/html/file/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1076 2022-03-07 22:00:13.000000 evariste-1.2.1/evariste/plugins/renderer/html/file/image.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/html/readme/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1201 2022-03-07 22:00:55.000000 evariste-1.2.1/evariste/plugins/renderer/html/readme/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1108 2022-03-07 22:01:08.000000 evariste-1.2.1/evariste/plugins/renderer/html/readme/mdwn.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1593 2022-03-07 22:01:20.000000 evariste-1.2.1/evariste/plugins/renderer/html/readme/rst.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.726761 evariste-1.2.1/evariste/plugins/renderer/htmlplus/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2763 2022-10-11 18:08:13.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.694760 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/
+-rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/COPYING
+-rw-r--r--   0 louis     (1000) louis     (1000)     2386 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/application-x-zerosize.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     1527 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/dialog-error.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     2901 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/dialog-ok-apply.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     2386 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/file.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     2355 2020-06-21 10:55:26.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/folder-open.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     2169 2020-06-21 10:55:27.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/folder.png
+-rw-r--r--   0 louis     (1000) louis     (1000)     7651 2020-06-21 10:55:27.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/lgpl-3.0.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)     2629 2020-06-21 10:55:27.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/tree.css
+-rw-r--r--   0 louis     (1000) louis     (1000)      488 2020-06-21 10:55:27.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/tree.js
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/templates/
+-rw-r--r--   0 louis     (1000) louis     (1000)     3581 2022-01-30 00:03:37.000000 evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/templates/page.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/evariste/plugins/renderer/jinja2/
+-rw-r--r--   0 louis     (1000) louis     (1000)    10446 2022-10-11 19:24:29.000000 evariste-1.2.1/evariste/plugins/renderer/jinja2/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2966 2022-03-07 22:33:16.000000 evariste-1.2.1/evariste/plugins/renderer/jinja2/file.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     4322 2022-03-07 22:33:16.000000 evariste-1.2.1/evariste/plugins/renderer/jinja2/readme.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     5759 2023-10-06 20:56:16.000000 evariste-1.2.1/evariste/plugins/renderer/text.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2919 2022-03-07 22:33:02.000000 evariste-1.2.1/evariste/plugins/tree.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/evariste/plugins/vcs/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2923 2022-10-11 19:25:02.000000 evariste-1.2.1/evariste/plugins/vcs/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1498 2024-05-06 21:08:45.000000 evariste-1.2.1/evariste/plugins/vcs/fs.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     3297 2022-03-07 22:05:44.000000 evariste-1.2.1/evariste/plugins/vcs/git.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1153 2022-03-07 22:05:59.000000 evariste-1.2.1/evariste/plugins/vcs/none.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     6208 2022-03-07 22:08:23.000000 evariste-1.2.1/evariste/setup.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     6587 2023-10-06 20:45:18.000000 evariste-1.2.1/evariste/shared.py
+-rw-r--r--   0 louis     (1000) louis     (1000)    22939 2024-05-05 18:06:24.000000 evariste-1.2.1/evariste/tree.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     8546 2022-10-11 19:23:56.000000 evariste-1.2.1/evariste/utils.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/evariste.egg-info/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2525 2024-05-06 21:26:53.000000 evariste-1.2.1/evariste.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)    15075 2024-05-06 21:26:54.000000 evariste-1.2.1/evariste.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2024-05-06 21:26:54.000000 evariste-1.2.1/evariste.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       97 2024-05-06 21:26:54.000000 evariste-1.2.1/evariste.egg-info/entry_points.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-03-07 22:34:08.000000 evariste-1.2.1/evariste.egg-info/not-zip-safe
+-rw-r--r--   0 louis     (1000) louis     (1000)       65 2024-05-06 21:26:54.000000 evariste-1.2.1/evariste.egg-info/requires.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        9 2024-05-06 21:26:54.000000 evariste-1.2.1/evariste.egg-info/top_level.txt
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/examples/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:27.000000 evariste-1.2.1/examples/.gitignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.730761 evariste-1.2.1/examples/example1/
+-rw-r--r--   0 louis     (1000) louis     (1000)       58 2020-06-21 10:55:27.000000 evariste-1.2.1/examples/example1/.gitignore
+-rwxr-xr-x   0 louis     (1000) louis     (1000)      157 2020-06-21 10:55:27.000000 evariste-1.2.1/examples/example1/compile.sh
+-rw-r--r--   0 louis     (1000) louis     (1000)     1417 2022-10-11 19:55:59.000000 evariste-1.2.1/examples/example1/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.738761 evariste-1.2.1/examples/example1/repository/
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:27.000000 evariste-1.2.1/examples/example1/repository/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       46 2020-06-21 10:55:27.000000 evariste-1.2.1/examples/example1/repository/.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/.noaction2.tex.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.738761 evariste-1.2.1/examples/example1/repository/autocommand/
+-rw-r--r--   0 louis     (1000) louis     (1000)       33 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/autocommand/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       41 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/autocommand/README.md
+-rw-r--r--   0 louis     (1000) louis     (1000)     2482 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/autocommand/image.xcf
+-rw-r--r--   0 louis     (1000) louis     (1000)    11216 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/autocommand/report.ods
+-rw-r--r--   0 louis     (1000) louis     (1000)    20314 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/autocommand/report2.fods
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.738761 evariste-1.2.1/examples/example1/repository/depends/
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends/depends-sub.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)        7 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends/depends2.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends/plop.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      154 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends-nostrace.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       36 2022-02-16 11:25:41.000000 evariste-1.2.1/examples/example1/repository/depends-nostrace.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)      127 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends-nostrace.tex.html
+-rw-r--r--   0 louis     (1000) louis     (1000)    20623 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends.png
+-rw-r--r--   0 louis     (1000) louis     (1000)      154 2022-02-23 21:42:33.000000 evariste-1.2.1/examples/example1/repository/depends.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      191 2022-03-07 21:40:13.000000 evariste-1.2.1/examples/example1/repository/depends.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)      105 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends.tex.html
+-rw-r--r--   0 louis     (1000) louis     (1000)       93 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/depends2.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)     1825 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/dummy.pdf
+-rw-r--r--   0 louis     (1000) louis     (1000)     1825 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/dummy.pdf.ignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/error1.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       48 2022-01-29 23:58:02.000000 evariste-1.2.1/examples/example1/repository/error1.tex.html
+-rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/error2.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       74 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/error2.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       47 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/error2.tex.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.742761 evariste-1.2.1/examples/example1/repository/foo/
+-rw-r--r--   0 louis     (1000) louis     (1000)       30 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        9 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       31 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/.foo.png.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       13 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       66 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/README.html
+-rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:28.000000 evariste-1.2.1/examples/example1/repository/foo/foo-jpg1.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo-jpg2.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)    13017 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo.jpg
+-rw-r--r--   0 louis     (1000) louis     (1000)       98 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo.jpg.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)    28286 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo.png
+-rw-r--r--   0 louis     (1000) louis     (1000)    11876 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo.svg
+-rw-r--r--   0 louis     (1000) louis     (1000)  1024360 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/foo.tiff
+-rw-r--r--   0 louis     (1000) louis     (1000)      113 2022-03-07 21:40:13.000000 evariste-1.2.1/examples/example1/repository/foo/foo.tiff.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)    28286 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/foo/ignored.png
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.742761 evariste-1.2.1/examples/example1/repository/gcc/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/gcc/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/gcc/.hello.c.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       88 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/gcc/hello.c
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/examples/example1/repository/multi/
+-rw-r--r--   0 louis     (1000) louis     (1000)       36 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       30 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)    20623 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/command.png
+-rw-r--r--   0 louis     (1000) louis     (1000)      139 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/command.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       99 2022-03-07 21:40:13.000000 evariste-1.2.1/examples/example1/repository/multi/command.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)     1218 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/index.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      144 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/multi/multicommand.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      156 2022-03-07 21:40:13.000000 evariste-1.2.1/examples/example1/repository/multi/multicommand.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/noaction1.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/noaction1.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/noaction1.tex.html
+-rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/noaction2.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/noaction2.tex.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/examples/example1/repository/parent/
+-rw-r--r--   0 louis     (1000) louis     (1000)      126 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/parent/parent.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)       99 2022-03-07 21:40:13.000000 evariste-1.2.1/examples/example1/repository/parent/parent.tex.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)     3024 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/report.pdf
+-rw-r--r--   0 louis     (1000) louis     (1000)       43 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/report.pdf.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:29.000000 evariste-1.2.1/examples/example1/repository/single.tex
+-rw-r--r--   0 louis     (1000) louis     (1000)      378 2024-05-05 18:17:03.000000 evariste-1.2.1/pyproject.toml
+-rw-r--r--   0 louis     (1000) louis     (1000)       65 2022-10-10 05:20:51.000000 evariste-1.2.1/requirements.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)     1525 2024-05-06 21:26:54.782761 evariste-1.2.1/setup.cfg
+-rwxr-xr-x   0 louis     (1000) louis     (1000)       93 2020-06-21 10:55:29.000000 evariste-1.2.1/setup.py
+-rw-r--r--   0 louis     (1000) louis     (1000)      100 2020-06-21 10:55:29.000000 evariste-1.2.1/stdeb.cfg
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/test/
+-rw-r--r--   0 louis     (1000) louis     (1000)      960 2020-06-21 10:55:29.000000 evariste-1.2.1/test/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/test/test_compile/
+-rw-r--r--   0 louis     (1000) louis     (1000)     5366 2022-02-16 21:32:14.000000 evariste-1.2.1/test/test_compile/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.698760 evariste-1.2.1/test/test_compile/data/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/test/test_compile/data/actions/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:29.000000 evariste-1.2.1/test/test_compile/data/actions/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       38 2020-06-21 10:55:29.000000 evariste-1.2.1/test/test_compile/data/actions/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      249 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/actions/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.746761 evariste-1.2.1/test/test_compile/data/actions/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/actions/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:29.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:29.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/command-in.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:29.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/command-out.txt
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/actions/expected/html/make/
+-rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/make/Makefile
+-rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/make/tagada.aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/make/tagada.grepa
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/raw
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/toto.sort
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/html/toto.sorted
+-rw-r--r--   0 louis     (1000) louis     (1000)     1025 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/actions/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)      143 2022-02-16 11:25:41.000000 evariste-1.2.1/test/test_compile/data/actions/source/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       44 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/command-in.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/command-in.txt.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/actions/source/make/
+-rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/make/Makefile
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/make/tagada.grepa
+-rw-r--r--   0 louis     (1000) louis     (1000)       59 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/make/tagada.grepa.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/raw
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/raw.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/actions/source/toto.sort
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/config/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       21 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      202 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/config/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.750761 evariste-1.2.1/test/test_compile/data/config/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/aa
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/bb
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/bbb
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/aa
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/bb
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/dir/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/dir/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/dir1/dir/bbb
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/expected/html/dir2/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/html/dir2/bbb
+-rw-r--r--   0 louis     (1000) louis     (1000)      992 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)      118 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/source/.aaa.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        7 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/source/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/source/.gitignore.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:30.000000 evariste-1.2.1/test/test_compile/data/config/source/aa
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)       99 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/aaa.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/source/dir1/
+-rw-r--r--   0 louis     (1000) louis     (1000)      124 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir1/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir1/aa
+-rw-r--r--   0 louis     (1000) louis     (1000)       70 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir1/aa.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.754761 evariste-1.2.1/test/test_compile/data/config/source/dir1/dir/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir1/dir/aaa
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/config/source/dir2/
+-rw-r--r--   0 louis     (1000) louis     (1000)      131 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir2/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/config/source/dir2/bbb
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/empty/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/empty/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       73 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/empty/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      180 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/empty/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/empty/expected/
+-rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/empty/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/empty/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)       15 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/empty/source/README.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/extends/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       32 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      228 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/extends/evariste.setup
+-rw-r--r--   0 louis     (1000) louis     (1000)      154 2022-02-16 11:25:41.000000 evariste-1.2.1/test/test_compile/data/extends/evariste2.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.758761 evariste-1.2.1/test/test_compile/data/extends/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/extends/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)       28 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/html/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/html/command-in.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/html/command-out.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/html/toto.sort
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/html/toto.sorted
+-rw-r--r--   0 louis     (1000) louis     (1000)      504 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/extends/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)       28 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/source/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/source/command-in.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      110 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/source/command-in.txt.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/extends/source/toto.sort
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/ignore/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       20 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      201 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/ignore/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/ignore/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/ignore/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/aaa.out
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir1/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir1/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir1/aaa.out
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.762761 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir2/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir2/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/html/dir2/aaa.out
+-rw-r--r--   0 louis     (1000) louis     (1000)      664 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/ignore/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)      136 2020-06-21 10:55:31.000000 evariste-1.2.1/test/test_compile/data/ignore/source/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/.ignored2.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/aaa
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/ignore/source/dir1/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir1/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir1/ignored1
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir1/ignored2
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/.ignored2.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/aaa
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/ignored1
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/ignored1.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/dir2/ignored2
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/ignore/source/empty/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/empty/ignored
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/empty/ignored.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/ignored1
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/ignored1.evsignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/ignore/source/ignored2
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/misc/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       26 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      205 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/misc/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/misc/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/misc/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)     4058 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/expected/html/colors.png
+-rw-r--r--   0 louis     (1000) louis     (1000)      262 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/misc/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)     4058 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/source/colors.png
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/misc/source/colors.png.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/targets/
+-rw-r--r--   0 louis     (1000) louis     (1000)       27 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)       23 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/description.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)      201 2022-10-13 19:36:02.000000 evariste-1.2.1/test/test_compile/data/targets/evariste.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.766761 evariste-1.2.1/test/test_compile/data/targets/expected/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.770761 evariste-1.2.1/test/test_compile/data/targets/expected/html/
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/one
+-rw-r--r--   0 louis     (1000) louis     (1000)        4 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/one.a
+-rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/two
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/two.a
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/two.b
+-rw-r--r--   0 louis     (1000) louis     (1000)       10 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/html/zero
+-rw-r--r--   0 louis     (1000) louis     (1000)      586 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/expected/index.html
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.770761 evariste-1.2.1/test/test_compile/data/targets/source/
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/one
+-rw-r--r--   0 louis     (1000) louis     (1000)       95 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/one.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       12 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/two
+-rw-r--r--   0 louis     (1000) louis     (1000)      126 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/two.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       10 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/zero
+-rw-r--r--   0 louis     (1000) louis     (1000)       69 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_compile/data/targets/source/zero.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)     1358 2021-11-27 16:46:49.000000 evariste-1.2.1/test/test_doctest.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.770761 evariste-1.2.1/test/test_ignore/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2328 2022-10-13 19:38:46.000000 evariste-1.2.1/test/test_ignore/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.770761 evariste-1.2.1/test/test_ignore/data/
+-rw-r--r--   0 louis     (1000) louis     (1000)       18 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/.gitignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.770761 evariste-1.2.1/test/test_ignore/data/tree/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/.bar.evsignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/a/
+-rw-r--r--   0 louis     (1000) louis     (1000)        6 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/a/.evsignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/a/b/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/a/b/plop.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/a/b/pom.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/a/b/tagada.md
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/bar
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/baz
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/c/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/c/tata.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/c/titi.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/c/toto.txt
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.698760 evariste-1.2.1/test/test_ignore/data/tree/d/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/d/d/
+-rw-r--r--   0 louis     (1000) louis     (1000)       22 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/.evsignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/
+-rw-r--r--   0 louis     (1000) louis     (1000)       12 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/.evsignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.774761 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/d/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/d/tata.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/d/titi.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/d/toto.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/tata.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/titi.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/d/toto.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/tata.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/titi.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/d/toto.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/tata.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/titi.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/d/d/toto.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/foo
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-07 21:44:26.000000 evariste-1.2.1/test/test_ignore/data/tree/foo.evsignore
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_plugins/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1663 2022-10-11 19:58:47.000000 evariste-1.2.1/test/test_plugins/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_plugins/depends/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2349 2022-10-10 19:39:17.000000 evariste-1.2.1/test/test_plugins/depends/depends.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.698760 evariste-1.2.1/test/test_plugins/libdirs/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_plugins/libdirs/plug ins/
+-rw-r--r--   0 louis     (1000) louis     (1000)      819 2022-02-23 17:53:35.000000 evariste-1.2.1/test/test_plugins/libdirs/plug ins/bar.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_plugins/libdirs/plugins/
+-rw-r--r--   0 louis     (1000) louis     (1000)      819 2022-02-23 17:53:35.000000 evariste-1.2.1/test/test_plugins/libdirs/plugins/foo.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     5210 2022-10-11 18:13:51.000000 evariste-1.2.1/test/test_plugins/test_depends.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2981 2022-03-07 21:45:17.000000 evariste-1.2.1/test/test_plugins/test_libdirs.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/
+-rw-r--r--   0 louis     (1000) louis     (1000)     2413 2022-03-07 21:45:17.000000 evariste-1.2.1/test/test_recursive/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/a/
+-rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/a/.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/a/aa/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/a/aa/aaa
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/b/
+-rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/b/.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/b/bb/
+-rw-r--r--   0 louis     (1000) louis     (1000)       41 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/b/bb/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/b/bb/bbb
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/c/
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/c/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/c/cc
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/d/
+-rw-r--r--   0 louis     (1000) louis     (1000)       40 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/d/.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/d/dd/
+-rw-r--r--   0 louis     (1000) louis     (1000)       15 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/d/dd/.evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/d/dd/ddd
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.778761 evariste-1.2.1/test/test_recursive/data/e/
+-rw-r--r--   0 louis     (1000) louis     (1000)       46 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/e/e.norec-evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)       61 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/e/e.rec-evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/e/ee
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.702760 evariste-1.2.1/test/test_recursive/data/f/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_recursive/data/f/ff/
+-rw-r--r--   0 louis     (1000) louis     (1000)       35 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/f/ff/evsconfig
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/f/ff/fff
+-rw-r--r--   0 louis     (1000) louis     (1000)       51 2022-02-16 19:36:36.000000 evariste-1.2.1/test/test_recursive/data/f.evsconfig
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_run/
+-rw-r--r--   0 louis     (1000) louis     (1000)     5375 2023-10-06 20:57:28.000000 evariste-1.2.1/test/test_run/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_setup/
+-rw-r--r--   0 louis     (1000) louis     (1000)     5461 2022-02-23 17:53:35.000000 evariste-1.2.1/test/test_setup/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.702760 evariste-1.2.1/test/test_setup/data/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_setup/data/cycle/
+-rw-r--r--   0 louis     (1000) louis     (1000)       38 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_setup/data/cycle/a.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_setup/data/cycle/b/
+-rw-r--r--   0 louis     (1000) louis     (1000)       41 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_setup/data/cycle/b/b.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_setup/data/cycle/c/
+-rw-r--r--   0 louis     (1000) louis     (1000)       39 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_setup/data/cycle/c/c.setup
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2024-05-06 21:26:54.782761 evariste-1.2.1/test/test_setup/data/empty/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_setup/data/empty/.gitignore
+-rw-r--r--   0 louis     (1000) louis     (1000)     3381 2022-03-07 21:45:17.000000 evariste-1.2.1/test/test_shared.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     1506 2020-06-21 10:55:32.000000 evariste-1.2.1/test/test_utils.py
+-rw-r--r--   0 louis     (1000) louis     (1000)      667 2023-10-06 21:35:31.000000 evariste-1.2.1/tox.ini
```

### Comparing `evariste-1.2.0/CHANGELOG.md` & `evariste-1.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+* evariste 1.2.1 (2024-05-06)
+
+    * Fix bug: plugins.vcs.fs simply did not work.
+
+    -- Louis Paternault <spalax@gresille.org>
+
 * evariste 1.2.0 (2023-10-07)
 
     * Python3.12 support.
 
     -- Louis Paternault <spalax@gresille.org>
 
 * evariste 1.1.0 (2022-10-13)
```

### Comparing `evariste-1.2.0/LICENSE` & `evariste-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/PKG-INFO` & `evariste-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evariste
-Version: 1.2.0
+Version: 1.2.1
 Summary: Publish annoted and compiled directory tree.
 Home-page: http://framagit.org/spalax/evariste
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://evariste.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/evariste
```

### Comparing `evariste-1.2.0/README.rst` & `evariste-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/Makefile` & `evariste-1.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/conf.py` & `evariste-1.2.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,22 +49,22 @@
 # source_encoding = 'utf-8-sig'
 
 # The main toctree document.
 root_doc = "index"
 
 # General information about the project.
 project = "Évariste"
-copyright = "2015-2023, Louis Paternault"
+copyright = "2015-2024, Louis Paternault"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "1.2.0"
+version = "1.2.1"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `evariste-1.2.0/doc/evs.rst` & `evariste-1.2.1/doc/evs.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/index.rst` & `evariste-1.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/action/autocommand.rst` & `evariste-1.2.1/doc/plugins/action/autocommand.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/action/command.rst` & `evariste-1.2.1/doc/plugins/action/command.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/action/make.rst` & `evariste-1.2.1/doc/plugins/action/make.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/action.rst` & `evariste-1.2.1/doc/plugins/action.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/logging.rst` & `evariste-1.2.1/doc/plugins/logging.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/misc.rst` & `evariste-1.2.1/doc/plugins/misc.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/renderer/html.rst` & `evariste-1.2.1/doc/plugins/renderer/html.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/renderer/htmlplus.rst` & `evariste-1.2.1/doc/plugins/renderer/htmlplus.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/renderer/jinja2.rst` & `evariste-1.2.1/doc/plugins/renderer/jinja2.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/renderer/text.rst` & `evariste-1.2.1/doc/plugins/renderer/text.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/vcs.rst` & `evariste-1.2.1/doc/plugins/vcs.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/write/action.rst` & `evariste-1.2.1/doc/plugins/write/action.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/write/hooks.rst` & `evariste-1.2.1/doc/plugins/write/hooks.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/write/renderer.rst` & `evariste-1.2.1/doc/plugins/write/renderer.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins/write.rst` & `evariste-1.2.1/doc/plugins/write.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/plugins.rst` & `evariste-1.2.1/doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/usecase.rst` & `evariste-1.2.1/doc/usecase.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/user/evsconfig.rst` & `evariste-1.2.1/doc/user/evsconfig.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/user/format.rst` & `evariste-1.2.1/doc/user/format.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/user/quickstart.rst` & `evariste-1.2.1/doc/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/user/setup.rst` & `evariste-1.2.1/doc/user/setup.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/doc/user/source.rst` & `evariste-1.2.1/doc/user/source.rst`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/__init__.py` & `evariste-1.2.1/evariste/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright Louis Paternault 2015-2023
+# Copyright Louis Paternault 2015-2024
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,10 +11,10 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Recursively compile files in a directory, and render result."""
 
-VERSION = "1.2.0"
+VERSION = "1.2.1"
 __AUTHOR__ = "Louis Paternault (spalax@gresille.org)"
-__COPYRIGHT__ = "(C) 2015-2023 Louis Paternault. GNU AGPL 3 or later."
+__COPYRIGHT__ = "(C) 2015-2024 Louis Paternault. GNU AGPL 3 or later."
```

### Comparing `evariste-1.2.0/evariste/__main__.py` & `evariste-1.2.1/evariste/__main__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/builder.py` & `evariste-1.2.1/evariste/builder.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/cache.py` & `evariste-1.2.1/evariste/cache.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/errors.py` & `evariste-1.2.1/evariste/errors.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/__init__.py` & `evariste-1.2.1/evariste/evs/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/__main__.py` & `evariste-1.2.1/evariste/evs/__main__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/cache/__init__.py` & `evariste-1.2.1/evariste/evs/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/cache/__main__.py` & `evariste-1.2.1/evariste/evs/cache/__main__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/compile/__init__.py` & `evariste-1.2.1/evariste/evs/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/compile/__main__.py` & `evariste-1.2.1/evariste/evs/compile/__main__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/compile/options.py` & `evariste-1.2.1/evariste/evs/compile/options.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/evs/plugins/__main__.py` & `evariste-1.2.1/evariste/evs/plugins/__main__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/hooks.py` & `evariste-1.2.1/evariste/hooks.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/__init__.py` & `evariste-1.2.1/evariste/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/__init__.py` & `evariste-1.2.1/evariste/plugins/action/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/autocommand.py` & `evariste-1.2.1/evariste/plugins/action/autocommand.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/cached.py` & `evariste-1.2.1/evariste/plugins/action/cached.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/command.py` & `evariste-1.2.1/evariste/plugins/action/command.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/make.py` & `evariste-1.2.1/evariste/plugins/action/make.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/action/nothing.py` & `evariste-1.2.1/evariste/plugins/action/nothing.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/changed.py` & `evariste-1.2.1/evariste/plugins/changed.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/copy.py` & `evariste-1.2.1/evariste/plugins/copy.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/debug.py` & `evariste-1.2.1/evariste/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/logging.py` & `evariste-1.2.1/evariste/plugins/logging.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/__init__.py` & `evariste-1.2.1/evariste/plugins/renderer/html/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/data/templates/tree.html` & `evariste-1.2.1/evariste/plugins/renderer/html/data/templates/tree.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/file/__init__.py` & `evariste-1.2.1/evariste/plugins/renderer/html/file/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/file/image.py` & `evariste-1.2.1/evariste/plugins/renderer/html/file/image.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/readme/__init__.py` & `evariste-1.2.1/evariste/plugins/renderer/html/readme/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/readme/mdwn.py` & `evariste-1.2.1/evariste/plugins/renderer/html/readme/mdwn.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/html/readme/rst.py` & `evariste-1.2.1/evariste/plugins/renderer/html/readme/rst.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/__init__.py` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/application-x-zerosize.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/application-x-zerosize.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/dialog-error.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/dialog-error.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/dialog-ok-apply.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/dialog-ok-apply.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/file.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/file.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/folder-open.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/folder-open.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/folder.png` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/folder.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/lgpl-3.0.txt` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/static/tree.css` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/static/tree.css`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/htmlplus/data/templates/page.html` & `evariste-1.2.1/evariste/plugins/renderer/htmlplus/data/templates/page.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/jinja2/__init__.py` & `evariste-1.2.1/evariste/plugins/renderer/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/jinja2/file.py` & `evariste-1.2.1/evariste/plugins/renderer/jinja2/file.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/jinja2/readme.py` & `evariste-1.2.1/evariste/plugins/renderer/jinja2/readme.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/renderer/text.py` & `evariste-1.2.1/evariste/plugins/renderer/text.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/tree.py` & `evariste-1.2.1/evariste/plugins/tree.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/vcs/__init__.py` & `evariste-1.2.1/evariste/plugins/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/vcs/fs.py` & `evariste-1.2.1/evariste/plugins/vcs/fs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright Louis Paternault 2016-2022
+# Copyright Louis Paternault 2016-2024
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,31 +12,33 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Access to any file on the file system."""
 
 import os
+import pathlib
 
 from . import VCS
 
 
 class FS(VCS):
     """Access all files on the file system."""
 
     keyword = "vcs.fs"
 
     def walk(self, *, root=None):
         if root is None:
-            root = self.workdir
+            root = pathlib.Path(self.workdir)
+        # From python3.12, we can use root.walk() instead
         for dirpath, dirnames, filenames in os.walk(root):
             for dirname in dirnames:
                 yield from self.walk(root=os.path.join(root, dirname))
             for filename in filenames:
-                yield os.path.relpath(os.path.join(dirpath, filename), self.workdir)
+                yield (pathlib.Path(dirpath) / filename).relative_to(self.workdir)
 
     def __contains__(self, path):
         return path.is_file() and (self.workdir in path.parents)
 
     @property
     def workdir(self):
         return str(self.source)
```

### Comparing `evariste-1.2.0/evariste/plugins/vcs/git.py` & `evariste-1.2.1/evariste/plugins/vcs/git.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/plugins/vcs/none.py` & `evariste-1.2.1/evariste/plugins/vcs/none.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/setup.py` & `evariste-1.2.1/evariste/setup.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/shared.py` & `evariste-1.2.1/evariste/shared.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/tree.py` & `evariste-1.2.1/evariste/tree.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste/utils.py` & `evariste-1.2.1/evariste/utils.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/evariste.egg-info/PKG-INFO` & `evariste-1.2.1/evariste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evariste
-Version: 1.2.0
+Version: 1.2.1
 Summary: Publish annoted and compiled directory tree.
 Home-page: http://framagit.org/spalax/evariste
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://evariste.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/evariste
```

### Comparing `evariste-1.2.0/evariste.egg-info/SOURCES.txt` & `evariste-1.2.1/evariste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/evariste.setup` & `evariste-1.2.1/examples/example1/evariste.setup`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/autocommand/image.xcf` & `evariste-1.2.1/examples/example1/repository/autocommand/image.xcf`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/autocommand/report.ods` & `evariste-1.2.1/examples/example1/repository/autocommand/report.ods`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/autocommand/report2.fods` & `evariste-1.2.1/examples/example1/repository/autocommand/report2.fods`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/depends.png` & `evariste-1.2.1/examples/example1/repository/depends.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/dummy.pdf` & `evariste-1.2.1/examples/example1/repository/dummy.pdf`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/dummy.pdf.ignore` & `evariste-1.2.1/examples/example1/repository/dummy.pdf.ignore`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/foo/foo.jpg` & `evariste-1.2.1/examples/example1/repository/foo/foo.jpg`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/foo/foo.png` & `evariste-1.2.1/examples/example1/repository/foo/foo.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/foo/foo.svg` & `evariste-1.2.1/examples/example1/repository/foo/foo.svg`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/foo/foo.tiff` & `evariste-1.2.1/examples/example1/repository/foo/foo.tiff`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/foo/ignored.png` & `evariste-1.2.1/examples/example1/repository/foo/ignored.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/multi/command.png` & `evariste-1.2.1/examples/example1/repository/multi/command.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/multi/index.tex` & `evariste-1.2.1/examples/example1/repository/multi/index.tex`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/examples/example1/repository/report.pdf` & `evariste-1.2.1/examples/example1/repository/report.pdf`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/setup.cfg` & `evariste-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = evariste
-version = 1.2.0
+version = 1.2.1
 author = Louis Paternault
 author_email = spalax@gresille.org
 license = AGPLv3 or any later version
 description = Publish annoted and compiled directory tree.
 keywords = compilation vcs publish html
 url = http://framagit.org/spalax/evariste
 project_urls =
```

### Comparing `evariste-1.2.0/test/__init__.py` & `evariste-1.2.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/__init__.py` & `evariste-1.2.1/test/test_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/actions/expected/index.html` & `evariste-1.2.1/test/test_compile/data/actions/expected/index.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/config/expected/index.html` & `evariste-1.2.1/test/test_compile/data/config/expected/index.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/ignore/expected/index.html` & `evariste-1.2.1/test/test_compile/data/ignore/expected/index.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/misc/expected/html/colors.png` & `evariste-1.2.1/test/test_compile/data/misc/expected/html/colors.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/misc/source/colors.png` & `evariste-1.2.1/test/test_compile/data/misc/source/colors.png`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_compile/data/targets/expected/index.html` & `evariste-1.2.1/test/test_compile/data/targets/expected/index.html`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_doctest.py` & `evariste-1.2.1/test/test_doctest.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_ignore/__init__.py` & `evariste-1.2.1/test/test_ignore/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/__init__.py` & `evariste-1.2.1/test/test_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/depends/depends.py` & `evariste-1.2.1/test/test_plugins/depends/depends.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/libdirs/plug ins/bar.py` & `evariste-1.2.1/test/test_plugins/libdirs/plug ins/bar.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/libdirs/plugins/foo.py` & `evariste-1.2.1/test/test_plugins/libdirs/plugins/foo.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/test_depends.py` & `evariste-1.2.1/test/test_plugins/test_depends.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_plugins/test_libdirs.py` & `evariste-1.2.1/test/test_plugins/test_libdirs.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_recursive/__init__.py` & `evariste-1.2.1/test/test_recursive/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_run/__init__.py` & `evariste-1.2.1/test/test_run/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_setup/__init__.py` & `evariste-1.2.1/test/test_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_shared.py` & `evariste-1.2.1/test/test_shared.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/test/test_utils.py` & `evariste-1.2.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `evariste-1.2.0/tox.ini` & `evariste-1.2.1/tox.ini`

 * *Files identical despite different names*

