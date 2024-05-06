# Comparing `tmp/marisa-trie-1.0.0.tar.gz` & `tmp/marisa-trie-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marisa-trie-1.0.0.tar", last modified: Sun Sep  3 10:40:46 2023, max compression
+gzip compressed data, was "marisa-trie-1.1.0.tar", last modified: Fri Oct  6 12:00:19 2023, max compression
```

## Comparing `marisa-trie-1.0.0.tar` & `marisa-trie-1.1.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.690352 marisa-trie-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (999)      279 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (999)     5280 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1086 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      275 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     8199 2023-09-03 10:40:46.690352 marisa-trie-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1702 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/bench/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/bench/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     6768 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/bench/speed.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/include/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/include/marisa/
--rw-r--r--   0 runner    (1001) docker     (999)     1456 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/agent.h
--rw-r--r--   0 runner    (1001) docker     (999)     6613 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/base.h
--rw-r--r--   0 runner    (1001) docker     (999)     2504 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/exception.h
--rw-r--r--   0 runner    (1001) docker     (999)      404 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/iostream.h
--rw-r--r--   0 runner    (1001) docker     (999)     1817 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/key.h
--rw-r--r--   0 runner    (1001) docker     (999)     1788 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/keyset.h
--rw-r--r--   0 runner    (1001) docker     (999)     1413 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/query.h
--rw-r--r--   0 runner    (1001) docker     (999)      953 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/scoped-array.h
--rw-r--r--   0 runner    (1001) docker     (999)      976 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/scoped-ptr.h
--rw-r--r--   0 runner    (1001) docker     (999)      248 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/stdio.h
--rw-r--r--   0 runner    (1001) docker     (999)     1251 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/include/marisa/trie.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/lib/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/lib/marisa/
--rw-r--r--   0 runner    (1001) docker     (999)     1073 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/agent.cc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.678351 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/algorithm/
--rw-r--r--   0 runner    (1001) docker     (999)     4335 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/algorithm/sort.h
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/algorithm.h
--rw-r--r--   0 runner    (1001) docker     (999)     3317 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/intrin.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.682351 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/
--rw-r--r--   0 runner    (1001) docker     (999)     4351 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/mapper.cc
--rw-r--r--   0 runner    (1001) docker     (999)     1490 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/mapper.h
--rw-r--r--   0 runner    (1001) docker     (999)     3413 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/reader.cc
--rw-r--r--   0 runner    (1001) docker     (999)     1359 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/reader.h
--rw-r--r--   0 runner    (1001) docker     (999)     3546 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/writer.cc
--rw-r--r--   0 runner    (1001) docker     (999)     1343 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/writer.h
--rw-r--r--   0 runner    (1001) docker     (999)      357 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.682351 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/
--rw-r--r--   0 runner    (1001) docker     (999)     1774 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/cache.h
--rw-r--r--   0 runner    (1001) docker     (999)     3597 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/config.h
--rw-r--r--   0 runner    (1001) docker     (999)     1825 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/entry.h
--rw-r--r--   0 runner    (1001) docker     (999)     1237 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/header.h
--rw-r--r--   0 runner    (1001) docker     (999)     1598 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/history.h
--rw-r--r--   0 runner    (1001) docker     (999)     5355 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/key.h
--rw-r--r--   0 runner    (1001) docker     (999)    26369 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.cc
--rw-r--r--   0 runner    (1001) docker     (999)     3694 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.h
--rw-r--r--   0 runner    (1001) docker     (999)     2468 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/range.h
--rw-r--r--   0 runner    (1001) docker     (999)     2761 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/state.h
--rw-r--r--   0 runner    (1001) docker     (999)     5677 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/tail.cc
--rw-r--r--   0 runner    (1001) docker     (999)     1645 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/tail.h
--rw-r--r--   0 runner    (1001) docker     (999)      319 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.682351 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/
--rw-r--r--   0 runner    (1001) docker     (999)    26213 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.cc
--rw-r--r--   0 runner    (1001) docker     (999)     4271 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.h
--rw-r--r--   0 runner    (1001) docker     (999)     5116 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/flat-vector.h
--rw-r--r--   0 runner    (1001) docker     (999)     2659 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/pop-count.h
--rw-r--r--   0 runner    (1001) docker     (999)     2276 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/rank-index.h
--rw-r--r--   0 runner    (1001) docker     (999)     6384 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/vector.h
--rw-r--r--   0 runner    (1001) docker     (999)      434 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector.h
--rw-r--r--   0 runner    (1001) docker     (999)     5857 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/keyset.cc
--rw-r--r--   0 runner    (1001) docker     (999)     6441 2023-09-03 10:40:43.000000 marisa-trie-1.0.0/marisa-trie/lib/marisa/trie.cc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.682351 marisa-trie-1.0.0/marisa_trie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     8199 2023-09-03 10:40:46.000000 marisa-trie-1.0.0/marisa_trie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2591 2023-09-03 10:40:46.000000 marisa-trie-1.0.0/marisa_trie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 10:40:46.000000 marisa-trie-1.0.0/marisa_trie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       53 2023-09-03 10:40:46.000000 marisa-trie-1.0.0/marisa_trie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-09-03 10:40:46.000000 marisa-trie-1.0.0/marisa_trie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-03 10:40:46.690352 marisa-trie-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)     2883 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.686351 marisa-trie-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (999)   153690 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/agent.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/agent.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   153348 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/base.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     2489 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/base.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   154753 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      228 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/iostream.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   153291 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/key.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      466 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/key.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   153500 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/keyset.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      696 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/keyset.pxd
--rw-r--r--   0 runner    (1001) docker     (999)  1407072 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/marisa_trie.cpp
--rw-r--r--   0 runner    (1001) docker     (999)    24773 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/marisa_trie.pyx
--rw-r--r--   0 runner    (1001) docker     (999)   153349 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/query.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      421 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/query.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   153893 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/std_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      456 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/std_iostream.pxd
--rw-r--r--   0 runner    (1001) docker     (999)   155092 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/trie.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     1117 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/src/trie.pxd
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:46.690352 marisa-trie-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6628 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/test_binary_trie.py
--rw-r--r--   0 runner    (1001) docker     (999)     3033 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/test_bytes_trie.py
--rw-r--r--   0 runner    (1001) docker     (999)     1892 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (999)      442 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/test_record_trie.py
--rw-r--r--   0 runner    (1001) docker     (999)     8511 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/test_trie.py
--rw-r--r--   0 runner    (1001) docker     (999)      220 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/tests/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (999)       51 2023-09-03 10:40:42.000000 marisa-trie-1.0.0/update_cpp.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.909148 marisa-trie-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2023-10-06 12:00:19.909148 marisa-trie-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/bench/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6768 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/bench/speed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.889146 marisa-trie-1.1.0/marisa-trie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.889146 marisa-trie-1.1.0/marisa-trie/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/marisa-trie/include/marisa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/agent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/exception.h
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/key.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/keyset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/query.h
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/scoped-array.h
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/scoped-ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/stdio.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/include/marisa/trie.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.889146 marisa-trie-1.1.0/marisa-trie/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/marisa-trie/lib/marisa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/agent.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/algorithm/sort.h
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/intrin.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.893147 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/mapper.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/mapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/writer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.901147 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/entry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/header.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/history.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/key.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26369 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/range.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/state.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/tail.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/tail.h
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.901147 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)    26213 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/flat-vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/pop-count.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/rank-index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/keyset.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2023-10-06 12:00:17.000000 marisa-trie-1.1.0/marisa-trie/lib/marisa/trie.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.901147 marisa-trie-1.1.0/marisa_trie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2023-10-06 12:00:19.000000 marisa-trie-1.1.0/marisa_trie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-10-06 12:00:19.000000 marisa-trie-1.1.0/marisa_trie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 12:00:19.000000 marisa-trie-1.1.0/marisa_trie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-06 12:00:19.000000 marisa-trie-1.1.0/marisa_trie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-06 12:00:19.000000 marisa-trie-1.1.0/marisa_trie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 12:00:19.909148 marisa-trie-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2929 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.905147 marisa-trie-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   153690 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/agent.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/agent.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   153348 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/base.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   154753 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/iostream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   153291 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/key.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/key.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   153500 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/keyset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/keyset.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)  1407072 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/marisa_trie.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24773 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/marisa_trie.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   153349 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/query.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/query.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   153893 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/std_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/std_iostream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   155092 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/trie.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/src/trie.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:19.909148 marisa-trie-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/test_binary_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/test_bytes_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/test_record_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/test_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/tests/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2023-10-06 12:00:15.000000 marisa-trie-1.1.0/update_cpp.sh
```

### Comparing `marisa-trie-1.0.0/CHANGES.rst` & `marisa-trie-1.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
 CHANGES
 =======
 
+1.1.0 (2023-10-06)
+------------------
+
+* Added Python 3.12 support.
+
 1.0.0 (2023-09-03)
 ------------------
 
 * Dropped Python 2.7, 3.4, 3.5, 3.6 support.
 * Added ``Trie.map()`` (#90).
 * Rebuilt Cython wrapper with Cython 3.0.2.
 * Fixed benchmark documentation typos (#89).
```

### Comparing `marisa-trie-1.0.0/LICENSE` & `marisa-trie-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/PKG-INFO` & `marisa-trie-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marisa-trie
-Version: 1.0.0
+Version: 1.1.0
 Summary: Static memory-efficient and fast Trie-like structures for Python.
 Home-page: https://github.com/pytries/marisa-trie
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -84,14 +85,19 @@
 
 Bundled `marisa-trie`_ C++ library is dual-licensed under
 LGPL and BSD 2-clause license.
 
 CHANGES
 =======
 
+1.1.0 (2023-10-06)
+------------------
+
+* Added Python 3.12 support.
+
 1.0.0 (2023-09-03)
 ------------------
 
 * Dropped Python 2.7, 3.4, 3.5, 3.6 support.
 * Added ``Trie.map()`` (#90).
 * Rebuilt Cython wrapper with Cython 3.0.2.
 * Fixed benchmark documentation typos (#89).
```

### Comparing `marisa-trie-1.0.0/README.rst` & `marisa-trie-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/bench/speed.py` & `marisa-trie-1.1.0/bench/speed.py`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/agent.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/agent.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/base.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/base.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/exception.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/exception.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/key.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/key.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/keyset.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/keyset.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/query.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/query.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/scoped-array.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/scoped-array.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/scoped-ptr.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/scoped-ptr.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/include/marisa/trie.h` & `marisa-trie-1.1.0/marisa-trie/include/marisa/trie.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/agent.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/agent.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/algorithm/sort.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/algorithm/sort.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/algorithm.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/algorithm.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/intrin.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/intrin.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/mapper.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/mapper.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/mapper.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/mapper.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/reader.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/reader.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/reader.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/reader.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/writer.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/writer.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/io/writer.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/io/writer.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/cache.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/cache.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/config.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/config.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/entry.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/entry.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/header.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/header.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/history.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/history.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/key.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/key.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/louds-trie.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/range.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/range.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/state.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/state.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/tail.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/tail.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/trie/tail.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/trie/tail.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/bit-vector.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/flat-vector.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/flat-vector.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/pop-count.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/pop-count.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/rank-index.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/rank-index.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/grimoire/vector/vector.h` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/grimoire/vector/vector.h`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/keyset.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/keyset.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa-trie/lib/marisa/trie.cc` & `marisa-trie-1.1.0/marisa-trie/lib/marisa/trie.cc`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/marisa_trie.egg-info/PKG-INFO` & `marisa-trie-1.1.0/marisa_trie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marisa-trie
-Version: 1.0.0
+Version: 1.1.0
 Summary: Static memory-efficient and fast Trie-like structures for Python.
 Home-page: https://github.com/pytries/marisa-trie
 Author: Mikhail Korobov
 Author-email: kmike84@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -84,14 +85,19 @@
 
 Bundled `marisa-trie`_ C++ library is dual-licensed under
 LGPL and BSD 2-clause license.
 
 CHANGES
 =======
 
+1.1.0 (2023-10-06)
+------------------
+
+* Added Python 3.12 support.
+
 1.0.0 (2023-09-03)
 ------------------
 
 * Dropped Python 2.7, 3.4, 3.5, 3.6 support.
 * Added ``Trie.map()`` (#90).
 * Rebuilt Cython wrapper with Cython 3.0.2.
 * Fixed benchmark documentation typos (#89).
```

### Comparing `marisa-trie-1.0.0/marisa_trie.egg-info/SOURCES.txt` & `marisa-trie-1.1.0/marisa_trie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/setup.py` & `marisa-trie-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,23 +48,24 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Text Processing :: Linguistic",
 ]
 
 setup(
     name="marisa-trie",
-    version="1.0.0",
+    version="1.1.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     author="Mikhail Korobov",
     author_email="kmike84@gmail.com",
     license=LICENSE,
     url="https://github.com/pytries/marisa-trie",
```

### Comparing `marisa-trie-1.0.0/src/agent.cpp` & `marisa-trie-1.1.0/src/agent.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/base.cpp` & `marisa-trie-1.1.0/src/base.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/base.pxd` & `marisa-trie-1.1.0/src/base.pxd`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/iostream.cpp` & `marisa-trie-1.1.0/src/iostream.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/key.cpp` & `marisa-trie-1.1.0/src/key.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/keyset.cpp` & `marisa-trie-1.1.0/src/keyset.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/keyset.pxd` & `marisa-trie-1.1.0/src/keyset.pxd`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/marisa_trie.cpp` & `marisa-trie-1.1.0/src/marisa_trie.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/marisa_trie.pyx` & `marisa-trie-1.1.0/src/marisa_trie.pyx`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/query.cpp` & `marisa-trie-1.1.0/src/query.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/std_iostream.cpp` & `marisa-trie-1.1.0/src/std_iostream.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/trie.cpp` & `marisa-trie-1.1.0/src/trie.cpp`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/src/trie.pxd` & `marisa-trie-1.1.0/src/trie.pxd`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/tests/test_binary_trie.py` & `marisa-trie-1.1.0/tests/test_binary_trie.py`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/tests/test_bytes_trie.py` & `marisa-trie-1.1.0/tests/test_bytes_trie.py`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/tests/test_packaging.py` & `marisa-trie-1.1.0/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `marisa-trie-1.0.0/tests/test_trie.py` & `marisa-trie-1.1.0/tests/test_trie.py`

 * *Files identical despite different names*

