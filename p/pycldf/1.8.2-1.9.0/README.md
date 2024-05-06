# Comparing `tmp/pycldf-1.8.2.tar.gz` & `tmp/pycldf-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycldf-1.8.2.tar", last modified: Thu Oct 24 08:27:36 2019, max compression
+gzip compressed data, was "dist/pycldf-1.9.0.tar", last modified: Tue Nov 26 15:21:46 2019, max compression
```

## Comparing `pycldf-1.8.2.tar` & `pycldf-1.9.0.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      404 2019-10-24 08:27:36.000000 pycldf-1.8.2/setup.cfg
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      235 2018-05-26 21:21:18.000000 pycldf-1.8.2/CONTRIBUTING.md
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      961 2018-05-26 21:21:18.000000 pycldf-1.8.2/RELEASING.md
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     4320 2018-05-26 21:21:18.000000 pycldf-1.8.2/README.md
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      162 2018-05-26 21:21:18.000000 pycldf-1.8.2/MANIFEST.in
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    11357 2018-05-26 21:21:18.000000 pycldf-1.8.2/LICENSE
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6465 2019-10-24 08:27:36.000000 pycldf-1.8.2/PKG-INFO
--rwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1671 2019-10-24 08:26:08.000000 pycldf-1.8.2/setup.py
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf/
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      147 2019-10-24 08:26:21.000000 pycldf-1.8.2/src/pycldf/__init__.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    21490 2019-10-24 07:12:01.000000 pycldf-1.8.2/src/pycldf/dataset.py
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf/modules/
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      254 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/modules/Generic-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2593 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/modules/Wordlist-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2693 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/modules/StructureDataset-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2802 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/modules/Dictionary-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2597 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/modules/ParallelText-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     4060 2019-09-16 08:35:13.000000 pycldf-1.8.2/src/pycldf/terms.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      993 2019-09-16 08:35:13.000000 pycldf-1.8.2/src/pycldf/util.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6042 2019-09-16 08:35:48.000000 pycldf-1.8.2/src/pycldf/sources.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    10168 2019-09-16 08:35:13.000000 pycldf-1.8.2/src/pycldf/db.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     3088 2019-09-16 08:35:13.000000 pycldf-1.8.2/src/pycldf/__main__.py
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf/components/
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1862 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/FunctionalEquivalentTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1114 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/CodeTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      895 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/ParameterTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      899 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/SenseTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      983 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/CognatesetTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2097 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/ExampleTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1944 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/ValueTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1009 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/FunctionalEquivalentsetTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1126 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/EntryTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1438 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/BorrowingTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1876 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/FormTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1810 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/CognateTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2291 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/components/LanguageTable-metadata.json
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1261 2019-09-16 08:35:13.000000 pycldf-1.8.2/src/pycldf/validators.py
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    34926 2018-05-26 21:21:18.000000 pycldf-1.8.2/src/pycldf/terms.rdf
-drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      159 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/requires.txt
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)       47 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/entry_points.txt
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        1 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/dependency_links.txt
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        1 2018-05-27 05:43:25.000000 pycldf-1.8.2/src/pycldf.egg-info/not-zip-safe
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6465 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/PKG-INFO
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1393 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/SOURCES.txt
--rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        7 2019-10-24 08:27:36.000000 pycldf-1.8.2/src/pycldf.egg-info/top_level.txt
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      404 2019-11-26 15:21:46.000000 pycldf-1.9.0/setup.cfg
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      235 2018-05-26 21:21:18.000000 pycldf-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      961 2018-05-26 21:21:18.000000 pycldf-1.9.0/RELEASING.md
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     4320 2018-05-26 21:21:18.000000 pycldf-1.9.0/README.md
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      162 2018-05-26 21:21:18.000000 pycldf-1.9.0/MANIFEST.in
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    11357 2018-05-26 21:21:18.000000 pycldf-1.9.0/LICENSE
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6465 2019-11-26 15:21:46.000000 pycldf-1.9.0/PKG-INFO
+-rwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1667 2019-11-26 15:20:41.000000 pycldf-1.9.0/setup.py
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      147 2019-11-26 15:21:05.000000 pycldf-1.9.0/src/pycldf/__init__.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    21597 2019-11-26 15:12:12.000000 pycldf-1.9.0/src/pycldf/dataset.py
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf/modules/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      254 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/modules/Generic-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2593 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/modules/Wordlist-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2693 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/modules/StructureDataset-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2802 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/modules/Dictionary-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2597 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/modules/ParallelText-metadata.json
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf/commands/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 07:08:24.000000 pycldf-1.9.0/src/pycldf/commands/__init__.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      769 2019-11-26 13:45:12.000000 pycldf-1.9.0/src/pycldf/commands/stats.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      698 2019-11-26 08:33:42.000000 pycldf-1.9.0/src/pycldf/commands/dumpdb.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      433 2019-11-26 09:45:09.000000 pycldf-1.9.0/src/pycldf/commands/createdb.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      376 2019-11-26 07:56:56.000000 pycldf-1.9.0/src/pycldf/commands/validate.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     4056 2019-11-26 15:15:21.000000 pycldf-1.9.0/src/pycldf/terms.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      991 2019-11-26 15:16:09.000000 pycldf-1.9.0/src/pycldf/util.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6063 2019-11-26 15:13:38.000000 pycldf-1.9.0/src/pycldf/sources.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    10165 2019-11-26 15:13:38.000000 pycldf-1.9.0/src/pycldf/db.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1144 2019-11-26 08:14:40.000000 pycldf-1.9.0/src/pycldf/__main__.py
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf/components/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1862 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/FunctionalEquivalentTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1114 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/CodeTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      895 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/ParameterTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      899 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/SenseTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      983 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/CognatesetTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2097 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/ExampleTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1944 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/ValueTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1009 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/FunctionalEquivalentsetTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1126 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/EntryTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1438 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/BorrowingTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1876 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/FormTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1810 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/CognateTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     2291 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/components/LanguageTable-metadata.json
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1268 2019-11-26 15:16:09.000000 pycldf-1.9.0/src/pycldf/validators.py
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)    34926 2018-05-26 21:21:18.000000 pycldf-1.9.0/src/pycldf/terms.rdf
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      798 2019-11-26 11:10:46.000000 pycldf-1.9.0/src/pycldf/cli_util.py
+drwxr-xr-x   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        0 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)      155 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/requires.txt
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)       47 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/entry_points.txt
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        1 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/dependency_links.txt
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        1 2018-05-27 05:43:25.000000 pycldf-1.9.0/src/pycldf.egg-info/not-zip-safe
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     6465 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/PKG-INFO
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)     1571 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/SOURCES.txt
+-rw-r--r--   0 forkel@shh.mpg.de (1706201286) domain users@shh.mpg.de (1706200513)        7 2019-11-26 15:21:46.000000 pycldf-1.9.0/src/pycldf.egg-info/top_level.txt
```

### Comparing `pycldf-1.8.2/RELEASING.md` & `pycldf-1.9.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/README.md` & `pycldf-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/LICENSE` & `pycldf-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/PKG-INFO` & `pycldf-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycldf
-Version: 1.8.2
+Version: 1.9.0
 Summary: A python library to read and write CLDF datasets
 Home-page: https://github.com/cldf/pycldf
 Author: Robert Forkel
 Author-email: forkel@shh.mpg.de
 License: Apache 2.0
 Description: # pycldf
         
@@ -168,9 +168,9 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycldf Version: 1.8.2 Summary: A python library to
+Metadata-Version: 2.1 Name: pycldf Version: 1.9.0 Summary: A python library to
 read and write CLDF datasets Home-page: https://github.com/cldf/pycldf Author:
 Robert Forkel Author-email: forkel@shh.mpg.de License: Apache 2.0 Description:
 # pycldf A python package to read and write [CLDF](http://cldf.clld.org)
 datasets. [![Build Status](https://travis-ci.org/cldf/
 pycldf.svg?branch=master)](https://travis-ci.org/cldf/pycldf) [![codecov]
 (https://codecov.io/gh/cldf/pycldf/branch/master/graph/badge.svg)](https://
 codecov.io/gh/cldf/pycldf) [![Requirements Status](https://requires.io/github/
```

### Comparing `pycldf-1.8.2/setup.py` & `pycldf-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pycldf',
-    version='1.8.2',
+    version='1.9.0',
     author='Robert Forkel',
     author_email='forkel@shh.mpg.de',
     description='A python library to read and write CLDF datasets',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='',
     license='Apache 2.0',
@@ -21,15 +21,15 @@
             'cldf=pycldf.__main__:main',
         ],
     },
     platforms='any',
     python_requires='>=3.5',
     install_requires=[
         'csvw>=1.5.5',
-        'clldutils>=1.13.10',
+        'clldutils>=3.5',
         'uritemplate>=3.0',
         'python-dateutil',
         'pybtex',
     ],
     extras_require={
         'dev': ['flake8', 'wheel', 'twine'],
         'test': [
```

### Comparing `pycldf-1.8.2/src/pycldf/dataset.py` & `pycldf-1.9.0/src/pycldf/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-from itertools import chain
-from collections import Counter, OrderedDict
-from pathlib import Path
+import pathlib
+import itertools
+import collections
 
 import attr
 from csvw.metadata import TableGroup, Table, Column, Link
 from csvw.dsv import iterrows
 from clldutils.path import git_describe
 from clldutils.misc import log_or_raise
 from clldutils import jsonlib
@@ -75,15 +75,15 @@
     def __init__(self, url, clone=None, version=None, **dc):
         self.url = url
         self.clone = clone
         self.version = version
         self.dc = dc
 
     def json_ld(self):
-        res = OrderedDict([
+        res = collections.OrderedDict([
             ('rdf:about', self.url),
             ('rdf:type', 'prov:Entity'),
         ])
         if self.version:
             res['dc:created'] = self.version
         elif self.clone:
             res['dc:created'] = git_describe(self.clone)
@@ -329,15 +329,15 @@
                     except ValueError:
                         success = False
                         log_or_raise('invalid CLDF URI: {0}'.format(col_uri), log=log)
                 for table_, col_, v_ in validators:
                     if (not table_ or table is self.get(table_)) and col is self.get((table, col_)):
                         validators_.append((col, v_))
 
-            fname = Path(table.url.resolve(table._parent.base))
+            fname = pathlib.Path(table.url.resolve(table._parent.base))
             if fname.exists():
                 for fname, lineno, row in table.iterdicts(log=log, with_metadata=True):
                     for col, validate in validators_:
                         try:
                             validate(self, table, col, row)
                         except ValueError as e:
                             log_or_raise(
@@ -365,36 +365,36 @@
 
     @property
     def version(self):
         return self.properties['dc:conformsTo'].split('/')[3]
 
     @classmethod
     def in_dir(cls, d, empty_tables=False):
-        fname = Path(d)
+        fname = pathlib.Path(d)
         if not fname.exists():
             fname.mkdir()
         assert fname.is_dir()
         res = cls.from_metadata(fname)
         if empty_tables:
             del res.tables[:]
         return res
 
     @classmethod
     def from_metadata(cls, fname):
-        fname = Path(fname)
+        fname = pathlib.Path(fname)
         if fname.is_dir():
             name = '{0}{1}'.format(cls.__name__, MD_SUFFIX)
             tablegroup = TableGroup.from_file(pkg_path('modules', name))
             # adapt the path of the metadata file such that paths to tables are resolved
             # correctly:
             tablegroup._fname = fname.joinpath(name)
         else:
             tablegroup = TableGroup.from_file(fname)
 
-        comps = Counter()
+        comps = collections.Counter()
         for table in tablegroup.tables:
             try:
                 dt = Dataset.get_tabletype(table)
                 if dt:
                     comps.update([dt])
             except ValueError:
                 pass
@@ -404,15 +404,15 @@
         for mod in get_modules():
             if mod.match(tablegroup):
                 return mod.cls(tablegroup)
         return cls(tablegroup)
 
     @classmethod
     def from_data(cls, fname):
-        fname = Path(fname)
+        fname = pathlib.Path(fname)
         colnames = next(iterrows(fname), [])
         if not colnames:
             raise ValueError('empty data file!')
         if cls is Dataset:
             try:
                 cls = next(mod.cls for mod in get_modules() if mod.match(fname))
             except StopIteration:
@@ -504,24 +504,25 @@
     def primary_table(self):
         if self.tables:
             try:
                 return self.get_tabletype(self.tables[0])
             except ValueError:
                 return None
 
-    def stats(self):
+    def stats(self, exact=False):
         res = []
         for table in self.tables:
             dctype = table.common_props.get('dc:conformsTo')
             if dctype and '#' in dctype and dctype.split('#')[1] in TERMS:
                 dctype = TERMS[dctype.split('#')[1]].csvw_prop('name')
             res.append((
                 table.url.string,
                 dctype,
-                table.common_props.get('dc:extent') or sum(1 for _ in table)))
+                sum(1 for _ in table) if (exact or 'dc:extent' not in table.common_props)
+                else int(table.common_props.get('dc:extent'))))
         if self.sources:
             res.append((self.bibpath.name, 'Sources', len(self.sources)))
         return res
 
     def write_metadata(self, fname=None):
         return self.tablegroup.to_file(fname or self.tablegroup._fname)
 
@@ -551,15 +552,15 @@
 
     def get_segments(self, row, table='FormTable'):
         col = self[table].get_column("http://cldf.clld.org/v1.0/terms.rdf#segments")
         sounds = row[col.name]
         if isinstance(sounds, str):
             # This may be the case when no morpheme boundaries are provided.
             sounds = [sounds]
-        return list(chain(*[s.split() for s in sounds]))
+        return list(itertools.chain(*[s.split() for s in sounds]))
 
     def get_subsequence(self, cognate, form=None):
         """
         Compute the subsequence of the morphemes of a form which is specified in a partial
         cognate assignment.
 
         :param partial_cognate:
```

### Comparing `pycldf-1.8.2/src/pycldf/modules/Wordlist-metadata.json` & `pycldf-1.9.0/src/pycldf/modules/Wordlist-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/modules/StructureDataset-metadata.json` & `pycldf-1.9.0/src/pycldf/modules/StructureDataset-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/modules/Dictionary-metadata.json` & `pycldf-1.9.0/src/pycldf/modules/Dictionary-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/modules/ParallelText-metadata.json` & `pycldf-1.9.0/src/pycldf/modules/ParallelText-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/terms.py` & `pycldf-1.9.0/src/pycldf/terms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import json
+import argparse
+import urllib.parse
 from xml.etree import ElementTree
-from json import loads
-from argparse import Namespace
-from urllib.parse import urlparse
 
 import attr
 from csvw.metadata import Column
 
 from pycldf.util import pkg_path
 
 __all__ = ['term_uri', 'TERMS', 'get_column_names']
@@ -59,15 +59,15 @@
                 if subClassOf is not None \
                 and subClassOf.attrib[qname(RDF, 'resource')] == \
                 'http://www.w3.org/ns/dcat#Distribution' else 'component'
         return cls(**kw)
 
     def csvw_prop(self, lname):
         if self.element.find(qname(CSVW, lname)) is not None:
-            return loads(self.element.find(qname(CSVW, lname)).text)
+            return json.loads(self.element.find(qname(CSVW, lname)).text)
 
     def to_column(self):
         col = Column(
             name=self.csvw_prop('name') or self.element.find(qname(RDFS, 'label')).text,
             propertyUrl=self.element.attrib[qname(RDF, 'about')],
             datatype=self.csvw_prop('datatype') or 'string')
         for k in ['separator', 'null', 'valueUrl']:
@@ -83,15 +83,15 @@
         terms = [Term.from_element(e) for e in r.findall(qname(RDF, 'Property'))]
         for e in r.findall(qname(RDFS, 'Class')):
             terms.append(Term.from_element(e))
         dict.__init__(self, {t.name: t for t in terms})
         self.by_uri = {t.uri: t for t in terms}
 
     def is_cldf_uri(self, uri):
-        if uri and urlparse(uri).netloc == 'cldf.clld.org':
+        if uri and urllib.parse.urlparse(uri).netloc == 'cldf.clld.org':
             if uri not in self.by_uri:
                 raise ValueError(uri)
             return True
         return False
 
     @property
     def properties(self):
@@ -111,21 +111,21 @@
 
 
 TERMS = Terms()
 
 
 def get_column_names(dataset):
     comp_names = {k: k.replace('Table', '').lower() + 's' for k in TERMS.components}
-    name_map = Namespace(**{k: None for k in comp_names.values()})
+    name_map = argparse.Namespace(**{k: None for k in comp_names.values()})
     for term, attr_ in comp_names.items():
         try:
             table = dataset[term]
             props = {}
             for k in TERMS.properties:
                 try:
                     props[k] = dataset[table, k].name
                 except KeyError:
                     props[k] = None
-            setattr(name_map, attr_, Namespace(**props))
+            setattr(name_map, attr_, argparse.Namespace(**props))
         except KeyError:
             pass
     return name_map
```

### Comparing `pycldf-1.8.2/src/pycldf/util.py` & `pycldf-1.9.0/src/pycldf/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import pathlib
 import itertools
-from pathlib import Path
 
 import pycldf
 
 
 def pkg_path(*comps):
-    return Path(pycldf.__file__).resolve().parent.joinpath(*comps)
+    return pathlib.Path(pycldf.__file__).resolve().parent.joinpath(*comps)
 
 
 def multislice(sliceable, *slices):
     res = type(sliceable)()
     for sl in slices:
         if isinstance(sl, str):
             if ':' in sl:
```

### Comparing `pycldf-1.8.2/src/pycldf/sources.py` & `pycldf-1.9.0/src/pycldf/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from collections import OrderedDict
 import re
-from pathlib import Path
+import pathlib
+import collections
 
 from pybtex import database
 from pybtex.database.output.bibtex import Writer as BaseWriter
 from clldutils.source import Source as BaseSource
 from clldutils.source import ID_PATTERN
 
 __all__ = ['Source', 'Reference']
@@ -23,21 +23,21 @@
         #
         return text
 
 
 class Source(BaseSource):
     @property
     def entry(self):
-        persons = OrderedDict([
+        persons = collections.OrderedDict([
             ('author', list(self.persons(self.get('author', '')))),
             ('editor', list(self.persons(self.get('editor', '')))),
         ])
         return database.Entry(
             self.genre,
-            fields=OrderedDict(
+            fields=collections.OrderedDict(
                 (k, v) for k, v in sorted(self.items()) if v and k not in ['author', 'editor']),
             persons=persons)
 
     def __str__(self):
         return self.text()
 
     def __repr__(self):
@@ -83,15 +83,15 @@
 class Sources(object):
     def __init__(self):
         self._bibdata = database.BibliographyData()
 
     @classmethod
     def from_file(cls, fname):
         res = cls()
-        fname = Path(fname)
+        fname = pathlib.Path(fname)
         if fname.exists():
             res.read(fname)
         return res
 
     def __bool__(self):
         return bool(self._bibdata.entries)
 
@@ -161,28 +161,28 @@
                     self._bibdata.add_entry(key, entry)
                 except database.BibliographyDataError as e:  # pragma: no cover
                     raise ValueError('%s' % e)
 
     def read(self, fname, **kw):
         self._add_entries(
             database.parse_string(
-                Path(fname).read_text(encoding='utf-8'),
+                pathlib.Path(fname).read_text(encoding='utf-8'),
                 bib_format='bibtex'),
             **kw)
 
     def write(self, fname, ids=None, **kw):
         if ids:
             bibdata = database.BibliographyData()
             for key, entry in self._bibdata.entries.items():
                 if key in ids:
                     bibdata.add_entry(key, entry)
         else:
             bibdata = self._bibdata
         if bibdata.entries:
-            with Path(fname).open('w', encoding='utf8') as fp:
+            with pathlib.Path(fname).open('w', encoding='utf8') as fp:
                 Writer().write_stream(bibdata, fp)
             return fname
 
     def add(self, *entries, **kw):
         """
         Add a source, either specified by glottolog reference id, or as bibtex record.
         """
```

### Comparing `pycldf-1.8.2/src/pycldf/db.py` & `pycldf-1.9.0/src/pycldf/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Functionality to load a set of CLDF datasets into a sqlite db.
 
 Notes:
 - Only CLDF components will be loaded into the db.
 - The names of the columns in the database are the names from the CSV files, not the
   preferred labels for the corresponding CLDF properties.
 """
-
+import pathlib
 import functools
 import collections
-from pathlib import Path
 
 import attr
 import csvw
 import csvw.db
 
 from pycldf.terms import TERMS
 from pycldf.sources import Reference, Sources, Source
@@ -210,15 +209,15 @@
         """
         Write the data from the db to a CLDF dataset according to the metadata in `self.dataset`.
 
         :param dest:
         :param mdname:
         :return: path of the metadata file
         """
-        dest = Path(dest)
+        dest = pathlib.Path(dest)
         if not dest.exists():
             dest.mkdir()
 
         data = self.read()
 
         if data[self.source_table_name]:
             sources = Sources()
```

### Comparing `pycldf-1.8.2/src/pycldf/components/FunctionalEquivalentTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/FunctionalEquivalentTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/CodeTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/CodeTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/ParameterTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/ParameterTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/SenseTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/SenseTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/CognatesetTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/CognatesetTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/ExampleTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/ExampleTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/ValueTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/ValueTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/FunctionalEquivalentsetTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/FunctionalEquivalentsetTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/EntryTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/EntryTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/BorrowingTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/BorrowingTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/FormTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/FormTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/CognateTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/CognateTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/components/LanguageTable-metadata.json` & `pycldf-1.9.0/src/pycldf/components/LanguageTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf/validators.py` & `pycldf-1.9.0/src/pycldf/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from functools import partial
+import functools
 
 
 def valid_references(dataset, table, column, row):
     if dataset.sources:
         dataset.sources.validate(row[column.name])
 
 
@@ -23,19 +23,19 @@
         raise ValueError('number of morphemes and glosses does not match')
 
 
 VALIDATORS = [
     (
         None,
         'http://cldf.clld.org/v1.0/terms.rdf#iso639P3code',
-        partial(valid_regex, re.compile(r'[a-z]{3}$'), 'ISO 639-3 code')),
+        functools.partial(valid_regex, re.compile(r'[a-z]{3}$'), 'ISO 639-3 code')),
     (
         None,
         'http://cldf.clld.org/v1.0/terms.rdf#glottocode',
-        partial(valid_regex, re.compile(r'[a-z0-9]{4}[0-9]{4}$'), 'glottocode')),
+        functools.partial(valid_regex, re.compile(r'[a-z0-9]{4}[0-9]{4}$'), 'glottocode')),
     (
         None,
         'http://cldf.clld.org/v1.0/terms.rdf#gloss',
         valid_igt),
     (
         None,
         'http://cldf.clld.org/v1.0/terms.rdf#source',
```

### Comparing `pycldf-1.8.2/src/pycldf/terms.rdf` & `pycldf-1.9.0/src/pycldf/terms.rdf`

 * *Files identical despite different names*

### Comparing `pycldf-1.8.2/src/pycldf.egg-info/PKG-INFO` & `pycldf-1.9.0/src/pycldf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycldf
-Version: 1.8.2
+Version: 1.9.0
 Summary: A python library to read and write CLDF datasets
 Home-page: https://github.com/cldf/pycldf
 Author: Robert Forkel
 Author-email: forkel@shh.mpg.de
 License: Apache 2.0
 Description: # pycldf
         
@@ -168,9 +168,9 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycldf Version: 1.8.2 Summary: A python library to
+Metadata-Version: 2.1 Name: pycldf Version: 1.9.0 Summary: A python library to
 read and write CLDF datasets Home-page: https://github.com/cldf/pycldf Author:
 Robert Forkel Author-email: forkel@shh.mpg.de License: Apache 2.0 Description:
 # pycldf A python package to read and write [CLDF](http://cldf.clld.org)
 datasets. [![Build Status](https://travis-ci.org/cldf/
 pycldf.svg?branch=master)](https://travis-ci.org/cldf/pycldf) [![codecov]
 (https://codecov.io/gh/cldf/pycldf/branch/master/graph/badge.svg)](https://
 codecov.io/gh/cldf/pycldf) [![Requirements Status](https://requires.io/github/
```

### Comparing `pycldf-1.8.2/src/pycldf.egg-info/SOURCES.txt` & `pycldf-1.9.0/src/pycldf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 MANIFEST.in
 README.md
 RELEASING.md
 setup.cfg
 setup.py
 src/pycldf/__init__.py
 src/pycldf/__main__.py
+src/pycldf/cli_util.py
 src/pycldf/dataset.py
 src/pycldf/db.py
 src/pycldf/sources.py
 src/pycldf/terms.py
 src/pycldf/terms.rdf
 src/pycldf/util.py
 src/pycldf/validators.py
 src/pycldf.egg-info/PKG-INFO
 src/pycldf.egg-info/SOURCES.txt
 src/pycldf.egg-info/dependency_links.txt
 src/pycldf.egg-info/entry_points.txt
 src/pycldf.egg-info/not-zip-safe
 src/pycldf.egg-info/requires.txt
 src/pycldf.egg-info/top_level.txt
+src/pycldf/commands/__init__.py
+src/pycldf/commands/createdb.py
+src/pycldf/commands/dumpdb.py
+src/pycldf/commands/stats.py
+src/pycldf/commands/validate.py
 src/pycldf/components/BorrowingTable-metadata.json
 src/pycldf/components/CodeTable-metadata.json
 src/pycldf/components/CognateTable-metadata.json
 src/pycldf/components/CognatesetTable-metadata.json
 src/pycldf/components/EntryTable-metadata.json
 src/pycldf/components/ExampleTable-metadata.json
 src/pycldf/components/FormTable-metadata.json
```

