# Comparing `tmp/S1Tiling-1.0.0rc3.tar.gz` & `tmp/s1tiling-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "S1Tiling-1.0.0rc3.tar", last modified: Thu Dec 14 10:58:19 2023, max compression
+gzip compressed data, was "s1tiling-1.1.0rc1.tar", last modified: Mon May  6 15:54:38 2024, max compression
```

## Comparing `S1Tiling-1.0.0rc3.tar` & `s1tiling-1.1.0rc1.tar`

### file list

```diff
@@ -1,67 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.383253 S1Tiling-1.0.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)     4658 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     6072 2023-12-14 10:58:19.383253 S1Tiling-1.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.235257 S1Tiling-1.0.0rc3/S1Tiling.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6072 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1480 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      294 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-12-14 10:58:19.000000 S1Tiling-1.0.0rc3/S1Tiling.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.239257 S1Tiling-1.0.0rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)    13627 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/CNES.rst
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/FAQ.rst
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/contribute.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/dataflow-filter.rst
--rw-rw-rw-   0 root         (0) root         (0)    15021 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/dataflow-main.rst
--rw-rw-rw-   0 root         (0) root         (0)    14823 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/dataflow-normlim.rst
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/dataflow.rst
--rw-rw-rw-   0 root         (0) root         (0)    16344 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/developers.rst
--rw-rw-rw-   0 root         (0) root         (0)    19216 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/files.rst
--rw-rw-rw-   0 root         (0) root         (0)     5722 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/how-to-developers.rst
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    11273 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)    10275 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/release_notes.rst
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    28927 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/docs/use.rst
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.239257 S1Tiling-1.0.0rc3/s1tiling/
--rwxrwxrwx   0 root         (0) root         (0)    34323 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/S1Processor.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/__meta__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.243257 S1Tiling-1.0.0rc3/s1tiling/libs/
--rwxrwxrwx   0 root         (0) root         (0)     1887 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/S1DateAcquisition.py
--rwxrwxrwx   0 root         (0) root         (0)    60266 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/S1FileManager.py
--rwxrwxrwx   0 root         (0) root         (0)     9550 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/S1FilteringProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)    17003 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/Utils.py
--rwxrwxrwx   0 root         (0) root         (0)      723 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/exits.py
--rwxrwxrwx   0 root         (0) root         (0)    85417 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/otbpipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    81169 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/otbwrappers.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/outcome.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/libs/vis.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/logging.conf.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.231258 S1Tiling-1.0.0rc3/s1tiling/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.255257 S1Tiling-1.0.0rc3/s1tiling/resources/Geoid/
--rwxrwxrwx   0 root         (0) root         (0)  4155868 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/Geoid/egm96.grd
--rwxrwxrwx   0 root         (0) root         (0)      186 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/Geoid/egm96.grd.hdr
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 10:58:19.375254 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/
--rwxrwxrwx   0 root         (0) root         (0) 31854441 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.dbf
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.prj
--rwxrwxrwx   0 root         (0) root         (0) 10941028 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.shp
--rwxrwxrwx   0 root         (0) root         (0)   455972 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.shx
--rwxrwxrwx   0 root         (0) root         (0)      385 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Info.dbf
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Info.prj
--rwxrwxrwx   0 root         (0) root         (0)      100 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Info.shp
--rwxrwxrwx   0 root         (0) root         (0)      100 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Info.shx
--rw-rw-rw-   0 root         (0) root         (0)  3100672 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/srtm_tiles.gpkg
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/s1tiling/s1tiling-cluster.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-12-14 10:58:19.383253 S1Tiling-1.0.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5680 2023-12-14 10:54:00.000000 S1Tiling-1.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.428563 s1tiling-1.1.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      600 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-05-06 15:54:38.428563 s1tiling-1.1.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.256562 s1tiling-1.1.0rc1/deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)     9550 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/deprecated/S1FilteringProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/deprecated/s1tiling-cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.260562 s1tiling-1.1.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/API.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13879 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/CNES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/FAQ.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.252562 s1tiling-1.1.0rc1/docs/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.264562 s1tiling-1.1.0rc1/docs/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10123 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/contribute.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/dataflow-filter.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15249 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/dataflow-main.rst
+-rw-rw-rw-   0 root         (0) root         (0)    26565 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/dataflow-normlim.rst
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/dataflow.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14118 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/developers.rst
+-rw-rw-rw-   0 root         (0) root         (0)    25507 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/files.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/how-to-developers.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12033 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/intro.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2815 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/list_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12624 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/release_notes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35099 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/docs/use.rst
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.264562 s1tiling-1.1.0rc1/s1tiling/
+-rwxrwxrwx   0 root         (0) root         (0)     8826 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/S1Processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/__meta__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.268562 s1tiling-1.1.0rc1/s1tiling/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/S1DateAcquisition.py
+-rw-rw-rw-   0 root         (0) root         (0)    66515 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/S1FileManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    28047 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39654 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    42013 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5966 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/exits.py
+-rw-rw-rw-   0 root         (0) root         (0)     3963 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/file_naming.py
+-rw-rw-rw-   0 root         (0) root         (0)     4177 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/node_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)    45112 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbpipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.272562 s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    74658 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/lia.py
+-rw-rw-rw-   0 root         (0) root         (0)    47234 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/s1_to_s2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/outcome.py
+-rw-rw-rw-   0 root         (0) root         (0)    54588 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/libs/vis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/logging.conf.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.272562 s1tiling-1.1.0rc1/s1tiling/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.284562 s1tiling-1.1.0rc1/s1tiling/resources/Geoid/
+-rwxrwxrwx   0 root         (0) root         (0)  4155868 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/Geoid/egm96.grd
+-rwxrwxrwx   0 root         (0) root         (0)      454 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/Geoid/egm96.grd.hdr
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.284562 s1tiling-1.1.0rc1/s1tiling/resources/generate-gpkg/
+-rwxrwxrwx   0 root         (0) root         (0)     5452 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/generate-gpkg/generate-DEM-gpkg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.416563 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/
+-rw-rw-rw-   0 root         (0) root         (0)  7991296 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/CopernicusDEM-CNES.gpkg
+-rw-rw-rw-   0 root         (0) root         (0) 31854441 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.dbf
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-06 15:52:31.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.prj
+-rw-rw-rw-   0 root         (0) root         (0) 10941028 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.shp
+-rw-rw-rw-   0 root         (0) root         (0)   455972 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.shx
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Info.dbf
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Info.prj
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Info.shp
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Info.shx
+-rw-rw-rw-   0 root         (0) root         (0)  3100672 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/s1tiling/resources/shapefile/srtm_tiles.gpkg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.424564 s1tiling-1.1.0rc1/s1tiling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 15:54:38.000000 s1tiling-1.1.0rc1/s1tiling.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-05-06 15:54:38.428563 s1tiling-1.1.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6038 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:54:38.424564 s1tiling-1.1.0rc1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    57026 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/tests/test_0200306-NR.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-06 15:52:32.000000 s1tiling-1.1.0rc1/tests/test_tsort.py
```

### Comparing `S1Tiling-1.0.0rc3/CONTRIBUTING.md` & `s1tiling-1.1.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/LICENSE` & `s1tiling-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/NOTICE.txt` & `s1tiling-1.1.0rc1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/PKG-INFO` & `s1tiling-1.1.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: S1Tiling
-Version: 1.0.0rc3
-Summary: On demand Ortho-rectification of Sentinel-1 data on Sentinel-2 grid.
-Home-page: https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
-Author: Thierry KOLECK
-Author-email: Thierry.Koleck@cnes.fr
-License: Apache 2.0
-Project-URL: Bug Tracker, https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues
-Project-URL: Documentation, https://s1-tiling.pages.orfeo-toolbox.org/s1tiling/latest
-Project-URL: Source Code, https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
-Project-URL: Community, https://forum.orfeo-toolbox.org/c/otb-chains/s1-tiling/11
-Keywords: Sentinel-1,Sentinel-2,orthorectification
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-License-File: NOTICE.txt
-
 # S1Tiling
 
 
 [![Sources](https://img.shields.io/badge/sources-gitlab.OTB-informational)](https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling)
 [![Fury](https://badge.fury.io/py/S1Tiling.svg)](https://badge.fury.io/py/S1Tiling)
 [![Docs (latest)](https://img.shields.io/badge/docs-passing-brightgreen)](https://s1-tiling.pages.orfeo-toolbox.org/s1tiling/latest/)
 [![S1Tiling Discourse (status)](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.orfeo-toolbox.org%2F)](https://forum.orfeo-toolbox.org/c/otb-chains/s1-tiling/11)
@@ -108,15 +72,17 @@
 
 # Community
 
 [![S1Tiling Discourse (status)](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.orfeo-toolbox.org%2F)](https://forum.orfeo-toolbox.org/c/otb-chains/s1-tiling/11)
 
 # Copyright
 
->   Copyright (c) CNES. All rights reserved.
+>   All rights reserved.
+>   Copyright 2017-2023 (c) CNES.
+>   Copyright 2022-2023 (c) CS GROUP France.
 >
 >   Licensed under the Apache License, Version 2.0 (the "License");
 >   you may not use this file except in compliance with the License.
 >   You may obtain a copy of the License at
 >
 >       http://www.apache.org/licenses/LICENSE-2.0
 >
@@ -133,9 +99,7 @@
 - Thierry KOLECK (CNES)
 - Luc HERMITTE (CS Group FRANCE)
 - Guillaume EYNARD-BONTEMPS (CNES)
 - Julien MICHEL (CNES)
 - Lesly SYLVESTRE (CNES)
 - Wenceslas SAINTE MARIE (CESBIO)
 - Arthur VINCENT (CESBIO)
-
-
```

### Comparing `S1Tiling-1.0.0rc3/docs/CNES.rst` & `s1tiling-1.1.0rc1/docs/CNES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+.. # define a hard line break for HTML
+.. |br| raw:: html
+
+   <br />
+
 .. _CNES:
 
 .. index:: HAL
 .. index:: TREX
 
 Some specificities about CNES clusters
 ======================================
@@ -22,21 +27,25 @@
     # Use the lastest version
     ml s1tiling
 
     # Check versions available
     ml av version
 
     # Activate a specific version
-    ml s1tiling/1.0.0rc2-otb7.4.2
+    ml s1tiling/1.0.0-otb7.4.2
+    # Or...
+    ml s1tiling/1.1.0rc1-otb9.0.0
 
 
 .. note::
 
-    For the moment, only S1Tiling 1.0 RC2 is installed with a dependency to OTB
-    7.4.2, Python 3.8.4 and G++ 8.2.
+    Only S1Tiling 1.0 will ever be installed with a dependency to OTB 7.4.2
+    (and Python 3.8.4 and g++ 8.2). |br|
+    S1Tiling 1.1.0 will be installed once with a dependency to OTB 7.4.2, and
+    once with a dependency to OTB 9.
 
 Installation on HAL/TREX
 ------------------------
 
 You may prefer to install S1Tiling yourself. In that case, there are mainly two
 X two ways to install S1Tiling on CNES clusters.
 
@@ -95,15 +104,15 @@
 
 .. note::
 
     This is the approach that has been chosen by the installation script we use
     internally. See: :download:`install-CNES.sh
     <../s1tiling/resources/install-CNES.sh>`
 
-    Prefer the later approach based on conda if you wish to use a different
+    Prefer the next approach based on conda if you wish to use a different
     version of Python.
 
 ...from available OTB module (and w/ conda)
 +++++++++++++++++++++++++++++++++++++++++++
 
 .. note::
    This approach permits to select a different version of Python, but it will
@@ -150,15 +159,15 @@
 
 ...from released OTB binaries...
 ++++++++++++++++++++++++++++++++
 
 Given :file:`otbenv.profile` cannot be unloaded, prefer the above methods based
 on OTB module.
 
-First let's start by installing OTB binaries somewhere in your personnal (or
+First let's start by installing OTB binaries somewhere in your personal (or
 project) environment.
 
 .. code:: bash
 
     # Start from a clean environment
     ml purge
     cd "${TST_DIR}"
@@ -311,31 +320,31 @@
 
       .. warning::
 
          Of course, we shall not use :file:`$TMPDIR` when running S1 Tiling on
          ``visu`` nodes. Actually, we should **not** use S1 Tiling for
          intensive computation on nodes not dedicated to computations.
 
-  * - :ref:`[PATHS].srtm <paths.srtm>`
-    - Original SRTM files are stored in
+  * - :ref:`[PATHS].dem_dir <paths.dem_dir>`
+    - Original DEM files are stored in
       :file:`/work/datalake/static_aux/MNT/SRTM_30_hgt`.
 
       .. code:: ini
 
           [PATHS]
-          srtm : /work/datalake/static_aux/MNT/SRTM_30_hgt
+          dem_dir : /work/datalake/static_aux/MNT/SRTM_30_hgt
 
-  * - :ref:`[Processing].cache_srtm_by <Processing.cache_srtm_by>`
-    - SRTM files should be **copied** locally on :ref:`[PATHS].tmp
+  * - :ref:`[Processing].cache_dem_by <Processing.cache_dem_by>`
+    - DEM and Geoid files should be **copied** locally on :ref:`[PATHS].tmp
       <paths.tmp>` instead of being symlinked over the GPFS.
 
       .. code:: ini
 
           [Processing]
-          cache_srtm_by : copy
+          cache_dem_by : copy
 
   * - :ref:`[Processing].nb_otb_threads <Processing.nb_otb_threads>`
     - This is the number of threads that will be used by each OTB application
       pipeline.
 
   * - :ref:`[Processing].nb_parallel_processes <Processing.nb_parallel_processes>`
     - This is the number of OTB application pipelines that will be executed in
@@ -343,15 +352,15 @@
 
   * - :ref:`[Processing].ram_per_process <Processing.ram_per_process>`
     - RAM allowed per OTB application pipeline, in MB.
 
   * - PBS resources
     - - At this time, S1 Tiling does not support multiple and related jobs. We
         can have multiple jobs but they should use different working spaces and
-        so on. This means ``select`` value shall be one.
+        so on. This means PBS ``select`` value shall be one.
 
       - The number of CPUs should be equal to the number of threads * the
         number of parallel processes -- and it shall not be less than the
         product of these two options.
 
       - The required memory shall be greater that the number of parallel
         processes per the RAM allowed to each OTB pipeline.
@@ -401,15 +410,15 @@
     export NB_OTB_THREADS=2
     # Let's deduce the number of OTB application pipelines to run in parallel
     export NB_OTB_PIPELINES=$(($NCPUS / $NB_OTB_THREADS))
     # These two variables have been exported to be automatically used from the
     # S1tiling request file.
 
     # Let's use an existing S1Tiling module
-    s1tiling/1.0.0rc2-otb7.4.2
+    ml s1tiling/1.1.0rc1-otb9.0.0
 
     # Expecting S1Processor.cfg in ${SLURM_SUBMIT_DIR}, the logs will be
     # produced in a subdirectory named after the the JOB ID.
     WORK_DIR="${SLURM_SUBMIT_DIR}/${SLURM_JOB_ID}"
     mkdir -p "${WORK_DIR}"
     cd "${WORK_DIR}"
     S1Processor --cache-before-ortho ../S1Processor.cfg || {
@@ -437,15 +446,15 @@
     export NB_OTB_THREADS=2
     # Let's deduce the number of OTB application pipelines to run in parallel
     export NB_OTB_PIPELINES=$(($NCPUS / $NB_OTB_THREADS))
     # These two variables have been exported to be automatically used from the
     # S1tiling request file.
 
     # Let's use an existing S1Tiling module
-    s1tiling/1.0.0rc2-otb7.4.2
+    ml s1tiling/1.1.0rc1-otb9.0.0
 
     # Expecting S1Processor.cfg in ${PBS_O_WORKDIR}, the logs will be
     # produced in a subdirectory named after the the JOB ID.
     WORK_DIR="${PBS_O_WORKDIR}/${PBS_JOBID}"
     mkdir -p "${WORK_DIR}"
     cd "${WORK_DIR}"
     S1Processor --cache-before-ortho ../S1Processor.cfg || {
@@ -458,17 +467,17 @@
 S1 Tiling request file: :file:`S1Processor.cfg`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: ini
 
       [PATHS]
       tmp : %(TMPDIR)s/s1tiling
-      srtm : /work/datalake/static_aux/MNT/SRTM_30_hgt
+      dem_dir : /work/datalake/static_aux/MNT/SRTM_30_hgt
       ...
 
       [Processing]
-      cache_srtm_by: copy
+      cache_dem_by: copy
       # Let's use the exported environment variables thanks to "%()s" syntax
       nb_parallel_processes: %(NB_OTB_PIPELINES)s
       nb_otb_threads: %(NB_OTB_THREADS)s
       ram_per_process: 4096
       ...
```

### Comparing `S1Tiling-1.0.0rc3/docs/FAQ.rst` & `s1tiling-1.1.0rc1/docs/FAQ.rst`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/docs/dataflow-filter.rst` & `s1tiling-1.1.0rc1/docs/dataflow-filter.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 .. index:: Spatial despeckle
 
 Spatial Despeckle filter
 ++++++++++++++++++++++++
 
 :Inputs:         Any :ref:`final S2 tiles <full-S2-tiles>`
 :Output:         A :ref:`filtered file <filtered-files>`
-:OTBApplication: :std:doc:`Despeckle <Applications/app_Despeckle>`
+:OTBApplication: :external:std:doc:`Despeckle <Applications/app_Despeckle>`
 :StepFactory:    :class:`s1tiling.libs.otbwrappers.SpatialDespeckle`
 
 This step applies any of the 3 spatial despeckling filters supported by
-:std:doc:`OTB Despeckle <Applications/app_Despeckle>`. See the documentation of
-this OTB application for more precise information.
+:external:std:doc:`OTB Despeckle <Applications/app_Despeckle>`. See the
+documentation of this OTB application for more precise information.
```

### Comparing `S1Tiling-1.0.0rc3/docs/dataflow-main.rst` & `s1tiling-1.1.0rc1/docs/dataflow-main.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,46 +21,48 @@
 
 1. It :ref:`downloads <downloading>` the necessary S1 images that intersect the
    S2 tile, within the specified time range, that are not already available in
    :ref:`input data cache <paths.s1_images>`
 
 2. Then, for each polarisation,
 
-   1. It :ref:`calibrates <calibration>`, :ref:`cuts <cutting>` and
-      :ref:`orthorectifies <orthorectification>` all the S1 images onto the S2
-      grid
-   2. It :ref:`superposes (concatenates) <concatenation>` the orthorectified
-      images into a single S2 tile.
-   3. It :ref:`builds masks <mask-generation>`, :ref:`if required <Mask.generate_border_mask>`
+   1. It :ref:`calibrates <calibration-proc>`, :ref:`cuts <cutting-proc>` and
+      :ref:`orthorectifies <orthorectification-proc>` all the S1 images onto
+      the S2 grid
+   2. It :ref:`superposes (concatenates) <concatenation-proc>` the
+      orthorectified images into a single S2 tile.
+   3. It :ref:`filters <filter-proc>` the orthorectified images.
+   4. It :ref:`builds masks <mask_generation-proc>`, :ref:`if required
+      <Mask.generate_border_mask>`
+
 
 
-.. _parallelization:
 
 .. index:: parallelization
 
 Parallelization
 ---------------
 
 The actual sequencing is not linear. S1 Tiling starts by building a
 dependencies graph expressed as a Dask Tasks graph. Dask framework then takes
 care of distributing the computations.
 
 In the following processing of 33NWB and 33NWC from 2020-01-01 to 2020-01-10,
 only two S2 images are generated. It's done by processing in parallel (but in
 any order compatible with the dependencies represented in the graph),
 
-- the S1 image inputs (first column) by :ref:`calibrating <calibration>` and
-  :ref:`cutting <cutting>` them to obtain...
+- the S1 image inputs (first column) by :ref:`calibrating <calibration-proc>`
+  and :ref:`cutting <cutting-proc>` them to obtain...
 - the :ref:`orthoready files <orthoready-files>` (second column), which are in
   turn :ref:`orthorectified <orthorectification>` to obtain...
 - the :ref:`orthorectified files <orthorectified-files>` (third column), which
   are in turn :ref:`concatenated <concatenation>` to obtain...
 - the :ref:`final S2 products <full-S2-tiles>` (fourth column),
 - :ref:`border masks <mask-files>`  can in turn be :ref:`generated
-  <mask-generation>` from them -- not represented on the graph.
+  <mask_generation-proc>` from them -- not represented on the graph.
 
 .. graphviz::
     :name: graph_S1Processing
     :caption: Tasks for processing 33NWB and 33NWC
     :alt: Complete task flow for processing 33NWB and 33NWC
     :align: center
 
@@ -152,59 +154,59 @@
         product was initially missing.
 
         You'll have to run it again with the same parameters!
 
 
 
 
-.. _calibration:
+.. _calibration-proc:
 .. index:: SAR Calibration
 
 SAR Calibration
 +++++++++++++++
 
 :Input:          An original :ref:`input S1 image <paths.s1_images>`
-:Output:         None: chained in memory with :ref:`cutting <cutting>`
-:OTBApplication: :std:doc:`OTB SARCalibration application
+:Output:         None: chained in memory with :ref:`cutting <cutting-proc>`
+:OTBApplication: :external:std:doc:`OTB SARCalibration application
                  <Applications/app_SARCalibration>`
 :StepFactory:    :class:`s1tiling.libs.otbwrappers.Calibrate`
 
 This step applies σ°, β°, or γ° radiometric correction.
 The type of calibration is controlled with :ref:`[Processing].calibration
 <Processing.calibration>` option. It also permits to remove thermal noise
 :ref:`if required <Processing.remove_thermal_noise>`.
 
 .. note:: At the end of this step, no file is produced as calibration is piped
-   in memory with :ref:`cutting <cutting>` to produce :ref:`orthorectification
-   ready images <orthoready-files>`
+   in memory with :ref:`cutting <cutting-proc>` to produce
+   :ref:`orthorectification ready images <orthoready-files>`
 
 .. note:: An extra artificial step is realized just after calibration to
    replace null values produced by denoising with a :ref:`minimal signal value
    <Processing.lower_signal_value>` > 0. This way, 0 can be used all along the
    way as the *no data* value.
 
 
-.. _cutting:
+.. _cutting-proc:
 .. index:: Margin cutting
 
 Margins cutting
 +++++++++++++++
 
 :Input:          None: chained in memory from :ref:`SAR Calibration
-                 <calibration>`
+                 <calibration-proc>`
 :Output:         - Either chained in memory with :ref:`orthorectification
-                   <orthorectification>`
+                   <orthorectification-proc>`
                  - or :ref:`orthorectification ready images <orthoready-files>`
-:OTBApplication: :std:doc:`OTB ResetMargin application
+:OTBApplication: :external:std:doc:`OTB ResetMargin application
                  <Applications/app_ResetMargin>`
 :StepFactory:    :class:`s1tiling.libs.otbwrappers.CutBorders`
 
 This step takes care of resetting margins content to 0 when too many no-data
 are detected within the margin. This phenomenon happens on coasts. The margins
-aren't cut out like what :std:doc:`ExtractROI <Applications/app_ExtractROI>`
+aren't cut out like what :external:std:doc:`ExtractROI <Applications/app_ExtractROI>`
 would do but filled with 0's, which permits to keeps the initial geometry.
 
 The implemented heuristic is to:
 
 - always cut 1000 pixels on the sides (2 x 10 km) products before Sentinel-1
   IPF v2.90 (see `MPC-0243: Masking "No-value" Pixels on GRD Products generated
   by the Sentinel-1 ESA IPF
@@ -222,51 +224,51 @@
 <orthoready-files>` may be produced. It could be interresting to :ref:`cache
 <data-caches>` these product as a same cut-and-calibrated S1 image can be
 orthorectified into several S2 grids it intersects. The default processing of
 these products in memory can be disabled by passing ``--cache-before-ortho`` to
 program:`S1Processor`.
 
 
-.. _orthorectification:
+.. _orthorectification-proc:
 .. index:: Orthorectification
 
 Orthorectification
 ++++++++++++++++++
 
-:Input:          - Either chained in memory from :ref:`cutting <cutting>`
+:Input:          - Either chained in memory from :ref:`cutting <cutting-proc>`
                  - or :ref:`orthorectification ready images <orthoready-files>`
 :Output:         :ref:`orthorectified S1 images <orthorectified-files>`
-:OTBApplication: :std:doc:`OTB OrthoRectification application
+:OTBApplication: :external:std:doc:`OTB OrthoRectification application
                  <Applications/app_OrthoRectification>`
 :StepFactory:    :class:`s1tiling.libs.otbwrappers.OrthoRectify`
 
 This steps ortho-rectifies the cut and calibrated (aka "orthoready") image in
 S1 geometry to S2 grid.
 
 It uses the following parameters from the request configuration file:
 
 - :ref:`[Processing].orthorectification_gridspacing
   <Processing.orthorectification_gridspacing>`
 - :ref:`[Processing].orthorectification_interpolation_method
   <Processing.orthorectification_interpolation_method>`
-- :ref:`[Paths].srtm <paths.srtm>`
+- :ref:`[Paths].dem_dir <paths.dem_dir>`
 - :ref:`[Paths].geoid_file <paths.geoid_file>`
 
 
-.. _concatenation:
+.. _concatenation-proc:
 .. index:: Concatenation
 
 Concatenation
 +++++++++++++
 
 :Inputs:         One or two consecutive :ref:`orthorectified S1 images
                  <orthorectified-files>`
 :Output:         The main product of S1 Tiling: the :ref:`final S2 tiles
                  <full-S2-tiles>`
-:OTBApplication: :std:doc:`OTB Synthetize application
+:OTBApplication: :external:std:doc:`OTB Synthetize application
                  <Applications/app_Synthetize>`
 :StepFactory:    :class:`s1tiling.libs.otbwrappers.Concatenate`
 
 This step takes care of merging all the images of the orthorectified S1
 products on a given S2 grid. As all orthorectified images are almost exclusive,
 they are concatenated by taking the first non null pixel.
 
@@ -287,36 +289,36 @@
 
     - .. image:: _static/s1a_33NWB_vh_DES_007_20200108txxxxxx.jpeg
            :scale: 50%
            :alt:   The orthorectified result
            :align: left
 
 
-.. _mask-generation:
+.. _mask_generation-proc:
 .. index:: Border mask generation
 
 Border mask generation
 ++++++++++++++++++++++
 
 :Inputs:          :ref:`final S2 tiles <full-S2-tiles>`
 :Output:          :ref:`border masks <mask-files>`
-:OTBApplications: - :std:doc:`OTB BandMath application <Applications/app_BandMath>`
-                  - :std:doc:`OTB BinaryMorphologicalOperation application
+:OTBApplications: - :external:std:doc:`OTB BandMath application <Applications/app_BandMath>`
+                  - :external:std:doc:`OTB BinaryMorphologicalOperation application
                     <Applications/app_BinaryMorphologicalOperation>`
 :StepFactories:   - :class:`s1tiling.libs.otbwrappers.BuildBorderMask`
                   - :class:`s1tiling.libs.otbwrappers.SmoothBorderMask`
 
 If :ref:`requested <Mask.generate_border_mask>`, :ref:`border masks
 <mask-files>` are generated.
 
 The actual generation is done in two steps:
 
-1. :std:doc:`OTB BandMath application <Applications/app_BandMath>` is used to
-   generate border masks by saturating non-zero data to 1's.
-2. :std:doc:`OTB BinaryMorphologicalOperation application
+1. :external:std:doc:`OTB BandMath application <Applications/app_BandMath>` is
+   used to generate border masks by saturating non-zero data to 1's.
+2. :external:std:doc:`OTB BinaryMorphologicalOperation application
    <Applications/app_BinaryMorphologicalOperation>` is used to smooth border
    masks with a ball of 5x5 radius used for *opening*.
 
 .. _data-caches:
 .. index:: Data caches
 
 Data caches
```

### Comparing `S1Tiling-1.0.0rc3/docs/files.rst` & `s1tiling-1.1.0rc1/docs/files.rst`

 * *Files 24% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 Orthorectified S2 tiles
 +++++++++++++++++++++++++++++
 
 :Content: Complete final product: concatenated orthorectified S1 images on S2
           grid
 
-:Directory:  :ref:`%(output) <paths.output>`:samp:`/{{tilename}}/`
+:Directory:  :ref:`%(output) <paths.output>`:samp:`/{{tilename}}/` by default
+
+:Directory format: :samp:`{{out_dir}}/{{tile_name}}`, see
+                   :ref:`[Processing].dname_fmt.tiled
+                   <Processing.dname_fmt.tiled>`
 
 :File name:
 
     - :samp:`s1{{a|b}}_{{tilename}}_{{polarity}}_{{orbitdirection}}_{{orbitnumber}}_{{YYYYMMDD}}txxxxxx.tif` when the tile has been assembled from the concatenation of several S1 images
     - :samp:`s1{{a|b}}_{{tilename}}_{{polarity}}_{{orbitdirection}}_{{orbitnumber}}_{{YYYYMMDD}}t{{hhmmss}}.tif` when the tile has been produced from a single S1 image
 
     .. note::
@@ -36,52 +40,58 @@
         :file:`_NormLim.tif`
 
 :File name format:
 
     - :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}.tif`, see :ref:`[Processing].fname_fmt.concatenation <Processing.fname_fmt.concatenation>`
     - or,  :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim.tif`, see :ref:`[Processing].fname_fmt.lia_corrected <Processing.fname_fmt.lia_corrected>`
 
-:Format: Float32 GeoTIFF, deflate compressed
+:Product encoding:
+
+    - defaults to Float32 GeoTIFF, deflate compressed
+    - defined in :ref:`[Processing].creation_options.tiled
+      <processing.creation_options.tiled>`
 
 :Metadata: The following metadata is added to the origin S1 images
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
 
       * - Metadata
         - Value
 
       * - ``ACQUISITION_DATETIME``
-        - time of the first S1 image
+        - time of the first S1 image (in UTC format since v1.1)
       * - ``ACQUISITION_DATETIME_1``
-        - time of the first S1 image
+        - time of the first S1 image (in UTC format since v1.1)
       * - ``ACQUISITION_DATETIME_2``
-        - time of the second S1 image
+        - time of the second S1 image (in UTC format since v1.1)
       * - ``CALIBRATION``
         - :ref:`chosen calibration option <Processing.calibration>`
       * - ``FLYING_UNIT_CODE``
         - :samp:`s1{{a|b}}`
       * - ``IMAGE_TYPE``
         - :samp:`GRD`
       * - ``INPUT_S1_IMAGES``
         - List of the input Sentinel-1 images used to generate this product
       * - ``LIA_FILE``
         - (when applies) name of the LIA file used for Normlim calibration
       * - ``NOISE_REMOVED``
         - :ref:`chosen noise removal option <Processing.remove_thermal_noise>`
-      * - ``ORBIT``
-        - :samp:`{{orbitnumber}}`
+      * - ``ORBIT_NUMBER``
+        - :samp:`{{orbitNumber}}`
       * - ``ORBIT_DIRECTION``
-        - :samp:`{{orbitdirection}}`
+        - :samp:`{{orbitDirection}}`
       * - ``ORTHORECTIFIED``
         - :samp:`true`
       * - ``POLARIZATION``
         - :samp:`{{polarisation}}`
+      * - ``RELATIVE_ORBIT_NUMBER``
+        - :samp:`{{relativeOrbitNumber}}`
       * - ``S2_TILE_CORRESPONDING_CODE``
         - :samp:`{{tilename}}`
       * - ``SPATIAL_RESOLUTION``
         - :ref:`chosen output spatial resolution option <Processing.output_spatial_resolution>`
       * - ``TIFFTAG_DATETIME``
         - is updated with the time when the tile has been generated by S1 Tiling.
       * - ``TIFFTAG_IMAGEDESCRIPTION``
@@ -95,20 +105,29 @@
 Mask files
 ++++++++++
 
 :Content:
 
     .. todo:: Thierry?
 
-:Directory:  :ref:`%(output) <paths.output>`:samp:`/{{tilename}}/`
+:Directory:  :ref:`%(output) <paths.output>`:samp:`/{{tilename}}/` by default
+
+:Directory format: :samp:`{{out_dir}}/{{tile_name}}`, see
+                   :ref:`[Processing].dname_fmt.mask
+                   <Processing.dname_fmt.mask>`
 
 :File name: the same as the one from :ref:`the S2 tiles <full-S2-tiles>`, with
             `_BorderMask` appended
 
-:Format: Byte GeoTIFF, deflate compressed
+:Product encoding:
+
+    - defaults to Byte GeoTIFF, deflate compressed
+    - defined in :ref:`[Processing].creation_options.mask
+      <processing.creation_options.mask>`
+
 
 :Metadata: This file contains the same metadata as the one from :ref:`the S2 tile product <full-S2-tiles>` it has been generated from, with the following as the only difference:
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
@@ -126,25 +145,35 @@
 Filtered files
 ++++++++++++++
 
 :Content:
 
     .. todo:: Thierry?
 
-:Directory:  :ref:`%(output) <paths.output>`:samp:`/filtered/{{tilename}}/`
+:Directory:  :ref:`%(output) <paths.output>`:samp:`/filtered/{{tilename}}/` by
+             default
+
+:Directory format: :samp:`{{out_dir}}/filtered/{{tile_name}}`, see
+                   :ref:`[Processing].dname_fmt.filtered
+                   <Processing.dname_fmt.filtered>`
 
 :File name: the same as the one from :ref:`the S2 tiles <full-S2-tiles>`, with
             `_filtered` appended
 
 :File name format:
 
     - :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_filtered.tif`, see :ref:`[Processing].fname_fmt.filtered <Processing.fname_fmt.filtered>`
     - or,  :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim_filtered.tif`
 
-:Format: Float32 GeoTIFF, deflate compressed
+:Product encoding:
+
+    - defaults to Float32 GeoTIFF, deflate compressed
+    - defined in :ref:`[Processing].creation_options.filtered
+      <processing.creation_options.filtered>`
+
 
 :Metadata: This file contains the same metadata as the one from :ref:`the S2 tile product <full-S2-tiles>` it has been generated from, with the following as the only difference:
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
@@ -184,43 +213,54 @@
     position, the LIA is the angle Θ\ :sub:`LIM` between the ground normal
     projected in range plane :math:`\overrightarrow{n}` (plane defined by S,
     T, and Earth's center) and :math:`\overrightarrow{TS}`.
 
     The values have been orthorectified on the Sentinel-2 tile from a pair of
     :ref:`LIA maps computed on S1 images <lia-s1-files>`.
 
-:Directory:  :ref:`%(output_lia)/ <paths.lia>`
+:Directory:  :ref:`%(output_lia)/ <paths.lia>` by default
+
+:Directory format: :samp:`{{lia_dir}}`, see
+                   :ref:`[Processing].dname_fmt.lia_product
+                   <Processing.dname_fmt.lia_product>`
 
 :File names:
 
     - :samp:`sin_LIA_s1{{a|b}}_{{tilename}}_{{orbitdirection}}_{{orbitnumber}}.tif` -- :math:`sin(Θ_{LIM})`
     - :samp:`LIA_s1{{a|b}}_{{tilename}}_{{orbitdirection}}_{{orbitnumber}}.tif` -- :math:`100 * Θ°_{LIM}`
 
 :File name format:
 
     :samp:`{{LIA_kind}}_{{flying_unit_code}}_{{tile_name}}_{{orbit_direction}}_{{orbit}}.tif`, see :ref:`[Processing].fname_fmt.lia_product <Processing.fname_fmt.lia_product>`
 
-:Format: Float32 (and Int16) GeoTIFF, deflate compressed
+:Product encoding:
+
+    - defaults to Float32 (/Uint16) GeoTIFF, deflate compressed
+    - defined in :ref:`[Processing].creation_options.lia_sin
+      <processing.creation_options.lia_sin>`
+      (/:ref:`[Processing].creation_options.lia_deg
+      <processing.creation_options.lia_deg>`)
+
 
 :Metadata: The following metadata is added to the origin S1 images
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
 
       * - Metadata
         - Value
 
       * - ``ACQUISITION_DATETIME``
-        - time of the first S1 image
+        - time of the first S1 image (in UTC format since v1.1)
       * - ``ACQUISITION_DATETIME_1``
-        - time of the first S1 image
+        - time of the first S1 image (in UTC format since v1.1)
       * - ``ACQUISITION_DATETIME_2``
-        - time of the second S1 image
+        - time of the second S1 image (in UTC format since v1.1)
       * - ``DATA_TYPE``
         - :samp:`100 * degree(LIA)` / :samp:`SIN(LIA)`
       * - ``FLYING_UNIT_CODE``
         - :samp:`s1{{a|b}}`
       * - ``IMAGE_TYPE``
         - :samp:`GRD`
       * - ``INPUT_S1_IMAGES``
@@ -256,47 +296,47 @@
 
 .. note:: It's up to you, end-user, to clean that directory regularly.
 
 .. _orthoready-files:
 
 Cut and calibrated S1 images ready for orthorectification
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-:Content: S1 images :ref:`calibrated <calibration>` and :ref:`cut <cutting>`.
+:Content: S1 images :ref:`calibrated <calibration-proc>` and :ref:`cut <cutting-proc>`.
 
 :Directory:  :ref:`%(tmp) <paths.tmp>`:samp:`/S1/`
 
 :File name: The same as the origin S1 file with ``_OrthoReady`` appended.
 
       .. note::
-            An accompanying OTB ``.geom`` file is also generated.
+            An accompanying OTB ``.geom`` file was also generated with OTB 7.
 
       Example:
 
       .. code-block:: none
 
            s1a-iw-grd-vv-20200108t044150-20200108t044215-030704-038506-001_sigma_OrthoReady.tiff
            s1a-iw-grd-vv-20200108t044150-20200108t044215-030704-038506-001_sigma_OrthoReady.geom
 
 :File name format:
 
     ``fname_fmt.cut_borders`` = :samp:`{{rootname}}_{{calibration_type}}_OrthoReady.tiff`
 
-:Format: Float32 GeoTIFF, uncompressed.
+:Product encoding: Float32 GeoTIFF, uncompressed.
 
 :Metadata: The following metadata are added at this step:
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
 
       * - Metadata
         - Value
       * - ``ACQUISITION_DATETIME``
-        - time of the input S1 image
+        - time of the input S1 image (in UTC format since v1.1)
       * - ``CALIBRATION``
         - :ref:`chosen calibration option <Processing.calibration>`
       * - ``FLYING_UNIT_CODE``
         - :samp:`s1{{a|b}}`
       * - ``IMAGE_TYPE``
         - :samp:`GRD`
       * - ``INPUT_S1_IMAGES``
@@ -333,52 +373,171 @@
 
 :File name: :samp:`s1{{a|b}}_{{tilename}}_{{polarity}}_{{orbitdirection}}_{{orbitnumber}}_{{YYYYMMDD}}t{{hhmmss}}_{{calibration}}.tif`
 
 :File name format:
 
     ``fname_fmt.orthorectification`` = :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_time}}_{{calibration_type}}.tif`
 
-:Format: Float32 GeoTIFF, deflate compressed
+:Product encoding: Float32 GeoTIFF, deflate compressed
 
 :Metadata: The metadata listed for :ref:`the S2 tile product <full-S2-tiles>`
            are actually produced at this step.
 
 .. note::
    These files are automatically cleaned up.
 
 .. _dem-vrt-files:
 
 DEM VRT files
 +++++++++++++
 
-:Content: Virtual aggregate of all the SRTM files that fully cover the
+:Content: Virtual aggregate of all the DEM files that fully cover the
           associated input S1 images (in both polarities).
 
 :Directory:  :ref:`%(tmp) <paths.tmp>`:samp:`/S1/`
 
-:File name: :samp:`DEM-s1{{a|b}}-iw-grd-{{start_stamp}}-{{end_stamp}}-{{nr1}}-{{nr2}}.tif`
+:File name:
+
+    - :samp:`DEM-s1{tilename}.tif`
+    - or deprecated: :samp:`DEM-s1{{a|b}}-iw-grd-{{start_stamp}}-{{end_stamp}}-{{nr1}}-{{nr2}}.tif`
 
 :File name format:
 
-    ``fname_fmt.dem_s1_agglomeration`` = :samp:`DEM_{{polarless_rootname}}.vrt`
+    - ``fname_fmt.dem_s2_agglomeration`` = :samp:`DEM_{{tile_name}}.vrt`
+    - or deprecated: ``fname_fmt.dem_s1_agglomeration`` = :samp:`DEM_{{polarless_rootname}}.vrt`
 
-:Format: VRT
+:Product encoding: VRT
 
 :Metadata: No metadata is added by S1Tiling to these files.
 
+:Cleanup: These files are cleaned automatically (since new workflow from v1.1).
+
+
+.. _DEM_on_S2-files:
+
+DEM data projected on S2 tile
++++++++++++++++++++++++++++++
+
+:Content:          DEM information projected on S2 tile according to
+                   :ref:`project_dem_to_s2-proc`
+:Directory:        :ref:`%(tmp) <paths.tmp>`:samp:`/S2/`
+:File name:        :samp:`DEM_projected_on_{{tilename}}.tiff`
+:File name format: ``fname_fmt.dem_on_s2`` = :samp:`DEM_projected_on_{{tile_name}}.tiff`
+:Product encoding: Float32 GeoTIFF, uncompressed.
+:Metadata:         The following metadata are added at this step:
+
+    .. list-table::
+      :widths: auto
+      :header-rows: 1
+      :stub-columns: 1
+
+      * - Metadata
+        - Value
+      * - ``S2_TILE_CORRESPONDING_CODE``
+        - :samp:`{{tilename}}`
+      * - ``SPATIAL_RESOLUTION``
+        - :ref:`chosen output spatial resolution option <Processing.output_spatial_resolution>`
+      * - ``DEM_LIST``
+        - List of DEM (SRTM currently) tiles used to generate the file
+      * - ``TIFFTAG_IMAGEDESCRIPTION``
+        - :samp:`Warped DEM to S2 tile`
+
+:Cleanup: These files are cleaned automatically.
+
+.. _height_on_S2-files:
+
+Height (DEM+Geoid) projected on S2 tile
++++++++++++++++++++++++++++++++++++++++
+
+:Content:          Height information (DEM + Geoid combined) projected on S2
+                   tile according to :ref:`project_geoid_to_s2-proc` and
+                   :ref:`Sum DEM + Geoid <sum_dem_geoid_on_s2-proc>`.
+:Directory:        :ref:`%(tmp) <paths.tmp>`:samp:`/S2/`
+:File name:        :samp:`DEM+GEOID_projected_on_{{tilename}}.tiff`
+:File name format: ``fname_fmt.height_on_s2`` = :samp:`DEM+GEOID_projected_on_{{tile_name}}.tiff`
+:Product encoding: Float32 GeoTIFF, uncompressed.
+:Metadata:         The following metadata changed from the :ref:`DEM projected on S2 tile <DEM_on_S2-files>`
+
+    .. list-table::
+      :widths: auto
+      :header-rows: 1
+      :stub-columns: 1
+
+      * - Metadata
+        - Value
+      * - ``TIFFTAG_IMAGEDESCRIPTION``
+        - :samp:`DEM + GEOID height info projected on S2 tile`
+
 :Cleanup:
 
     .. warning::
        These files still **need** to be cleaned manually. This should change
        eventually, or it may be conditionned to an option.
 
+
+.. _ground_and_sat_S2-files:
+
+Ground and sensor position in XYZ ECEF coordinates
+++++++++++++++++++++++++++++++++++++++++++++++++++
+
+:Content:          Six bands 64 bits float image that contains ground pixel
+                   coordinates and associated sensor position coordinates
+                   expressed as XYZ cartesian pixels in `ECEF
+                   <https://en.wikipedia.org/wiki/Earth-centered,_Earth-fixed_coordinate_system>`_
+                   spatial reference.
+                   The image footprint matches the associated S2 tile.
+:Directory:        :ref:`%(tmp) <paths.tmp>`:samp:`/S2/`
+:File name:        :samp:`XYZ_projected_on_{{tile_name}}_{{orbitdirection}}_{{orbitnumber}}.tif`
+:File name format: ``fname_fmt.ground_and_sat_s2`` = :samp:`XYZ_projected_on_{{tile_name}}_{{orbit_direction}}_{{orbit}}.tif`
+:Product encoding: Float64 GeoTIFF, 6 bands: XCartesian, YCartesian,
+                   ZCartesian. SensorXCartesian, SensorXCartesian,
+                   SensorZCartesian
+:Metadata:         The following metadata changed from the :ref:`DEM+GEOID projected on S2 tile <height_on_S2-files>`
+
+    .. list-table::
+      :widths: auto
+      :header-rows: 1
+      :stub-columns: 1
+
+      * - Metadata
+        - Value
+
+      * - ``ACQUISITION_DATETIME``
+        - time of the first S1 image (in UTC format since v1.1)
+      * - ``DEM_LIST``
+        - List of DEM (SRTM currently) tiles used to generate the file
+      * - ``FLYING_UNIT_CODE``
+        - :samp:`s1{{a|b}}`
+      * - ``IMAGE_TYPE``
+        - :samp:`GRD`
+      * - ``INPUT_S1_IMAGES``
+        - List of the input Sentinel-1 images used to generate this product
+      * - ``ORBIT``
+        - :samp:`{{orbitnumber}}`
+      * - ``ORBIT_DIRECTION``
+        - :samp:`{{orbitdirection}}`
+      * - ``PRJ.DIRECTIONTOSCANDEMC``
+        - Range direction for DEM scan.
+      * - ``PRJ.DIRECTIONTOSCANDEML``
+        - Azimuth direction for DEM scan.
+      * - ``PRJ.GAIN``
+        - Gain value
+      * - ``TIFFTAG_IMAGEDESCRIPTION``
+        - :samp:`XYZ ground and satellite positions on S2 tile`
+
+:Cleanup: These files are cleaned automatically.
+
+
+Deprecated temporary files
+--------------------------
+
 .. _S1_on_dem-files:
 
-Files of S1 coordinates projected on DEM geometry
-+++++++++++++++++++++++++++++++++++++++++++++++++
+Files of S1 coordinates projected on DEM geometry (deprecated)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 :Content: Pixels are in the :ref:`Virtual DEM <dem-vrt-files>` geometry. Their
           values contain the XYZ cartesian coordinates of the pixel and the
           position of the matching pixel in the original Sentinel-1 image.
           This file is produced with `DiapOTB SARDEMProjection
           <https://gitlab.orfeo-toolbox.org/remote_modules/diapotb/-/wikis/Applications/app_SARDEMProjection>`_
           application.
@@ -387,29 +546,30 @@
 
 :File name: :samp:`S1_on_DEM-s1{{a|b}}-iw-grd-{{start_stamp}}-{{end_stamp}}-{{nr1}}-{{nr2}}.tif`
 
 :File name format:
 
     ``fname_fmt.s1_on_dem`` = :samp:`S1_on_DEM_{{polarless_basename}}`
 
-:Format: Float32 GeoTIFF, 7 bands: C (colunm into SAR image), L (line into SAR
-         image), Z and Y, XCartesian, YCartesian, ZCartesian.
+:Product encoding: Float32 GeoTIFF, 7 bands: C (colunm into SAR image), L (line
+                   into SAR image), Z and Y, XCartesian, YCartesian,
+                   ZCartesian.
 
 :Metadata: The following metadata is added to the origin S1 images
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
 
       * - Metadata
         - Value
 
       * - ``ACQUISITION_DATETIME``
-        - time of the first S1 image
+        - time of the first S1 image (in UTC format since v1.1)
       * - ``DEM_LIST``
         - List of DEM (SRTM currently) tiles used to generate the file
       * - ``FLYING_UNIT_CODE``
         - :samp:`s1{{a|b}}`
       * - ``IMAGE_TYPE``
         - :samp:`GRD`
       * - ``INPUT_S1_IMAGES``
@@ -431,16 +591,16 @@
 
     .. warning::
        These files still **need** to be cleaned manually. This should change
        eventually, or it may be conditionned to an option.
 
 .. _xyz-files:
 
-Files of XYZ cartesian coordinates in S1 geometry
-+++++++++++++++++++++++++++++++++++++++++++++++++
+Files of XYZ cartesian coordinates in S1 geometry (deprecated)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 :Content: Pixels are in the original Sentinel-1 image geometry. Their
           values contain the XYZ cartesian coordinates of the pixel.
           This file is produced with `our patched version
           <https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0/-/merge_requests/1>`_
           of `DiapOTB SARCartesianMeanEstimation
           <https://gitlab.orfeo-toolbox.org/remote_modules/diapotb/-/wikis/Applications/app_SARCartesianMeanEstimation>`_
@@ -450,15 +610,15 @@
 
 :File name: :samp:`XYZ-s1{{a|b}}-iw-grd-{{start_stamp}}-{{end_stamp}}-{{nr1}}-{{nr2}}.tif`
 
 :File name format:
 
     ``fname_fmt.xyz`` = :samp:`XYZ_{{polarless_basename}}`
 
-:Format: Float32 GeoTIFF, 4 bands: XCartesian, YCartesian, ZCartesian, and ???
+:Product encoding: Float32 GeoTIFF, 4 bands: XCartesian, YCartesian, ZCartesian, and ???
 
 :Metadata: The following metadata changed from the :ref:`SARDEMProjected images <S1_on_dem-files>`
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
@@ -479,16 +639,16 @@
 
     .. warning::
        These files still **need** to be cleaned manually. This should change
        eventually, or it may be conditionned to an option.
 
 .. _lia-s1-files:
 
-Local Incidence Angle map files in S1 geometry
-++++++++++++++++++++++++++++++++++++++++++++++
+Local Incidence Angle map files in S1 geometry (deprecated)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 :Content:
 
     - Map of sines of Local Incidence Angle (LIA),
     - and optionally of LIA expressed in degree and scaled by a factor of 100.
 
     Given T, the target point on Earth's surface, and S the SAR sensor
@@ -507,15 +667,15 @@
     - :samp:`sin-LIA-s1{{a|b}}-iw-grd-{{start_stamp}}-{{end_stamp}}-{{nr1}}-{{nr2}}.tif`
 
 :File name format:
 
     - ``fname_fmt.s1_lia`` = :samp:`LIA_{{polarless_basename}}`
     - ``fname_fmt.s1_sin_lia`` = :samp:`sin_LIA_{{polarless_basename}}`
 
-:Format: Float32 GeoTIFF
+:Product encoding: Float32 GeoTIFF
 
 :Metadata: The following metadata is changed the :ref:`XYZ estimated coordinates <xyz-files>`
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
@@ -530,16 +690,16 @@
 
     .. warning::
        These files still **need** to be cleaned manually. This should change
        eventually, or it may be conditionned to an option.
 
 .. _lia-s2-half-files:
 
-Half Local Incidence Angle map files -- pre-concatenation.
-++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+Half Local Incidence Angle map files -- pre-concatenation. (deprecated)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 :Content:
 
     - Map of sines of Local Incidence Angle (LIA),
     - and optionally of LIA expressed in degree and scaled by a factor of 100.
 
     These files directly match the :ref:`LIA maps computed on S1 images
@@ -554,15 +714,15 @@
     - :samp:`sin_LIA_s1{{a|b}}_{{tilename}}_{{orbitdirection}}_{{orbitnumber}}_{{start_stamp}}.tif` -- :math:`sin(Θ_{LIM})`
     - :samp:`LIA_s1{{a|b}}_{{tilename}}_{{orbitdirection}}_{{orbitnumber}}_{{start_stamp}}.tif` -- :math:`100 * Θ°_{LIM}`
 
 :File name format:
 
     ``fname_fmt.lia_orthorectification`` = :samp:`{{LIA_kind}}_{{flying_unit_code}}_{{tile_name}}_{{orbit_direction}}_{{orbit}}_{{acquisition_time}}.tif`
 
-:Format: Float32 (and Int16) GeoTIFF, deflate compressed
+:Product encoding: Float32 (and Int16) GeoTIFF, deflate compressed
 
 :Metadata: The following metadata is changed from the :ref:`un-orthorectified LIA maps <lia-s1-files>`
 
     .. list-table::
       :widths: auto
       :header-rows: 1
       :stub-columns: 1
```

### Comparing `S1Tiling-1.0.0rc3/docs/how-to-developers.rst` & `s1tiling-1.1.0rc1/docs/how-to-developers.rst`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/docs/index.rst` & `s1tiling-1.1.0rc1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
    release_notes
 
 .. toctree::
    :maxdepth: 3
    :caption: Developer Documentation:
 
    contribute
+   API
    developers
    how-to-developers
    testing
 
 Indices and tables
 ==================
```

#### html2text {}

```diff
@@ -11,10 +11,10 @@
 status?server=https%3A%2F%2Fforum.orfeo-toolbox.org%2F :target: https://
 forum.orfeo-toolbox.org/c/otb-chains/s1-tiling/11 .. |License| image:: https://
 img.shields.io/pypi/l/s1tiling.svg :target: https://pypi.org/project/s1tiling/
 .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/
 s1tiling.svg :target: https://pypi.org/project/s1tiling/ On demand Ortho-
 rectification of Sentinel-1 data on Sentinel-2 grid. .. toctree:: :maxdepth: 3
 :caption: User Guide: intro install use dataflow files CNES FAQ release_notes
-.. toctree:: :maxdepth: 3 :caption: Developer Documentation: contribute
+.. toctree:: :maxdepth: 3 :caption: Developer Documentation: contribute API
 developers how-to-developers testing Indices and tables ================== * :
 ref:`genindex` * :ref:`modindex` * :ref:`search`
```

### Comparing `S1Tiling-1.0.0rc3/docs/install.rst` & `s1tiling-1.1.0rc1/docs/install.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,36 @@
 
 Manual installation with pip
 ----------------------------
 
 OTB & GDAL dependency
 +++++++++++++++++++++
 
-S1 Tiling depends on OTB 7.3+, but we recommend the latest, `OTB 7.4
-<https://www.orfeo-toolbox.org/CookBook-7.4/>`_ at the time.
+S1 Tiling depends on OTB 7.3+, or OTB 8.1.1+, but we recommend the latest,
+which at the moment is `OTB 9.0.0
+<https://www.orfeo-toolbox.org/CookBook-9.0/>`_. Or if you really need you can
+use `OTB 7.4.2 <https://www.orfeo-toolbox.org/CookBook-7.4/>`_.
+
 First install OTB on your platform. See the `related documentation
-<https://www.orfeo-toolbox.org/CookBook-7.4/Installation.html>`_ to install OTB
-on your system..
+<https://www.orfeo-toolbox.org/CookBook-9.0/Installation.html>`_ to install OTB
+on your system. Things has changed between versions 8.x and 9.x.
 
 Then, you'll also need a version of GDAL which is compatible with your OTB
 version.
 
 - In case you're using OTB binary distribution, you'll need to **patch** the
   files provided.
 
   - For that purpose you can **drop** this simplified and generic version of
     :download:`gdal-config <../s1tiling/resources/gdal-config>` into the
     ``bin/`` directory where you've extracted OTB. This will permit :samp:`pip
     install gdal=={vernum}` to work correctly.
-  - You'll also have to **patch** :file:`otbenv.profile` to **insert** OTB ``lib/``
-    directory at the start of :envvar:`$LD_LIBRARY_PATH`. This will permit
-    ``python3 -c 'from osgeo import gdal'`` to work correctly.
+  - You'll also have to **patch** :file:`otbenv.profile` to **insert** OTB
+    ``lib/`` directory at the start of :envvar:`$LD_LIBRARY_PATH`. This will
+    permit ``python3 -c 'from osgeo import gdal'`` to work correctly.
 
         .. code-block:: bash
 
             # For instance, type this, once!
             echo 'LD_LIBRARY_PATH="${CMAKE_PREFIX_PATH}${LD_LIBRARY_PATH:+:$LD_LIBRARY_PATH}"' >> otbenv.profile
 
   - You may also have to make sure ``numpy`` is installed before gdal Python
@@ -54,15 +57,15 @@
 
 - On clusters where OTB has been compiled from sources, you can simply load the
   associated module:
 
         .. code-block:: bash
 
             # Example, on TREX:
-            module load otb/7.4.2-Python3.8.4
+            module load otb/9.0.0-python3.8
 
         .. note::
 
             The installation script which is used on CNES clusters would be a
             good starting point. See: :download:`install-CNES.sh
             <../s1tiling/resources/install-CNES.sh>`
 
@@ -71,43 +74,43 @@
    you'll need to inject in your ``$PATH`` a version of :download:`gdal-config
    <../s1tiling/resources/gdal-config>` tuned to return GDAL configuration
    information.
 
 Possible conflicts on Python version
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-`eodag <https://github.com/CS-SI/eodag>`_ requires ``xarray`` which in turn
-requires at least Python 3.6 while default OTB 7.4 binaries are built with
-Python 3.5.  This means you'll likely need to recompile OTB Python bindings as
-described in:
+The Python version you have chosen may not match exactly the version used to
+generate Python bindings of the version of OTB you have selected.
+This means you'll likely need to recompile OTB Python bindings as described in:
 https://www.orfeo-toolbox.org/CookBook/Installation.html#recompiling-python-bindings
 
 
 .. code-block:: bash
 
-    cd OTB-7.4.2-Linux64
+    cd OTB-9.0.0-Linux64
     source otbenv.profile
-    # Load module on TREX
-    module load gcc
+    # require g++, cmake
     ctest3 -S share/otb/swig/build_wrapping.cmake -VV
 
 Conflicts between rasterio default wheel and OTB binaries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. note::
    **TL;DR** In the case you install **other programs alongside S1Tiling** in
-   the same environment, then use :program:`pip` with ``--no-binary rasterio``
-   parameter.
+   the same environment, and that programs depend on ``rasterio``, then use
+   :program:`pip` with ``--no-binary rasterio`` parameter.
 
    The current version of S1Tiling doesn't depend on any package that requires
    ``rasterio``, and thus ``pip install s1tiling`` is enough.
 
 
 The following paragraph applies **only** in case you install other Python
-programs alongside S1Tiling in the same environment.
+programs alongside S1Tiling in the same environment. And the wheels of these
+programs have hardcoded the version of GDAL they depend upon, like this is the
+case with ``rasterio``.
 
 We had found a compatibility issue between OTB and default rasterio packaging.
 The kind that produces:
 
 .. code-block:: none
 
     Unable to open EPSG support file gcs.csv
@@ -146,15 +149,15 @@
 
     # First go into a virtual environment (optional)
     # a- It could be a python virtual environment
     python3 -m venv myS1TilingEnv
     cd myS1TilingEnv
     source bin/activate
     # b- or a conda virtual environment
-    conda create -n myS1TilingEnv python==3.7.2
+    conda create -n myS1TilingEnv python==3.10
     conda activate myS1TilingEnv
 
     # Then, upgrade pip and setuptools in your virtual environment
     python -m pip install --upgrade pip
     python -m pip install --upgrade setuptools==57.5.0
 
     # Finally, install S1 Tiling
@@ -218,15 +221,15 @@
         - An un-extracted OTB binary release,
         - Python 3.8+,
         - A directory where S1Tiling has been cloned,
         - Conda.
 
     -
         - Creates a conda environment for the selected python version (3.8 by
-          default),
+          default with OTB 7.x, 3.11 w/ OTB 8.x, and 3.12 w/ OTB 9.x),
         - Extracts the OTB binary release in the directory where the
           ``OTB-M.m.p-Linux64.run`` file is,
         - Patches ``UseOTB.cmake`` if need be (in case of C++ ABI mismatch in
           7.4.2 OTB release),
         - Patches :file:`otbenv.profile`,
         - Regenerates Python bindings for OTB,
         - Installs GDAL python bindings from sources (to match GDAL version
@@ -236,76 +239,83 @@
           ``s1tiling/otb{Mmp}-py{Mm}`` (Major/minor/patch).
 
           .. note::
             You can source :file:`otbenv.profile` and activate the conda
             environement manually if you don't use `Lmod
             <https://lmod.readthedocs.io/en/latest/?badge=latest>`_.
 
+         .. note::
+            You will still need to install `LIA extra applications
+            <https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0>`_ in
+            order to :ref:`produce LIA maps <scenario.s1liamap>`, or to apply
+            :ref:`σ° NORMLIM calibration <scenario.s1processorlia>`.
+
 Extra packages
 ++++++++++++++
 
 You may want to install extra packages like `bokeh
 <https://pypi.org/project/bokeh/>`_ to monitor the execution of the multiple
 processing by Dask.
 
 
 .. _docker:
 
 Using S1Tiling with a docker
 ----------------------------
 
 As the installation of S1Tiling could be tedious, versions ready to be used are
-provided as Ubuntu 18.04 dockers.
+provided as Ubuntu dockers.
 
 You can browse the full list of available dockers in `S1Tiling registry
 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/container_registry>`_.
 Their naming scheme is
-:samp:`registry.orfeo-toolbox.org/s1-tiling/s1tiling:{{version}}-ubuntu-otb7.4.2`,
+:samp:`registry.orfeo-toolbox.org/s1-tiling/s1tiling:{{version}}-ubuntu-otb{{otbversion}}`,
 with the version being either ``develop``, ``latest`` or the version number of
 a recent release.
 
 The docker, containing the version of S1Tiling of which you're reading the
 documentation (i.e. version :samp:`{VERSION}`), could be fetched with:
 
 .. code-block:: bash
 
+    docker pull registry.orfeo-toolbox.org/s1-tiling/s1tiling:{VERSION}-ubuntu-otb9.0.0
+    # or
     docker pull registry.orfeo-toolbox.org/s1-tiling/s1tiling:{VERSION}-ubuntu-otb7.4.2
 
 or even directly used with
 
-
 .. code-block:: bash
 
     docker run                            \
         -v /localpath/to/MNT:/MNT         \
         -v "$(pwd)":/data                 \
         -v $HOME/.config/eodag:/eo_config \
-        --rm -it registry.orfeo-toolbox.org/s1-tiling/s1tiling:{VERSION}-ubuntu-otb7.4.2 \
+        --rm -it registry.orfeo-toolbox.org/s1-tiling/s1tiling:{VERSION}-ubuntu-otb9.0.0 \
         /data/MyS1ToS2.cfg
 
 .. note::
 
     This example considers:
 
-    - SRTM's are available on local host through :file:`/localpath/to/MNT/` and
+    - DEM's are available on local host through :file:`/localpath/to/MNT/` and
       they will be mounted into the docker as :file:`/MNT/`.
     - Logs and output files will be produced in current working directory (i.e.
       :file:`$(pwd)`) which will be mounted as :file:`data/`.
     - EODAG configuration file to be in :file:`$HOME/.config/eodag` which will
       be mounted as :file:`/eo_config/`.
     - A :ref:`configuration file <request-config-file>` named
       :file:`MyS1ToS2.cfg` is present in current working directory, which is
       seen from docker perspective as in :file:`data/` directory.
     - And it relates to the volumes mounted in the docker in the following way:
 
         .. code-block:: ini
 
             [Paths]
             output : /data/data_out
-            srtm : /MNT/SRTM_30_hgt
+            dem_dir : /MNT/SRTM_30_hgt
             ...
             [DataSource]
             eodag_config : /eo_config/eodag.yml
             ...
 
 .. _docker.S1LIAMap:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `S1Tiling-1.0.0rc3/docs/intro.rst` & `s1tiling-1.1.0rc1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/docs/release_notes.rst` & `s1tiling-1.1.0rc1/docs/release_notes.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,62 @@
 .. _release_notes:
 
 Release notes
 =============
 
+Version 1.1.0
+-------------
+
+This version integrates 3 main improvements:
+
+- it can support DEM from any sources (Copernicus DEM, RGE Alti DEM...),
+- it supports OTB 8 (and OTB 9) applications (while staying backward compatible
+  with OTB 7.4.2),
+- it improves the quality and the processing performances of
+  LIA/:math:`σ^0_{RTC}` NORMLIM calibration.
+
+v1.1.0 Improvements
++++++++++++++++++++
+
+- Improve API (separate CLI from computing functions)
+  (`#96 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/96>`_) --
+  contributed by CS Group FRANCE.
+- Support DEM files from other origins (Copernicus...). Their footprints,
+  organization on disk... need to be deduced from a DEM database.
+  (`#18 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/18>`_) --
+  contributed by CS Group FRANCE.
+- Add support for OTB 8 applications
+  (`#105 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/105>`_)
+  -- contributed by CS Group FRANCE.
+- Add support for OTB 9 applications as well
+  (`#152 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/152>`_).
+- Support DEM databases in any spatial reference (they are not restricted to
+  WGS84 anymore)
+  (`#149 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/149>`_).
+- Change LIA workflow in order to minimize occurrences of artefacts in rugged
+  areas, and to speed-up performances
+  (`#149 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/149>`_).
+- Product output directory can be configured through :ref:`dname_fmt.*
+  <processing.dname_fmt>` options
+  (`#148 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/148>`_).
+- Product encoding/compression options can be configured through
+  :ref:`creation_options.* <Processing.creation_options>` options
+  (`#66 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/66>`_).
+- GEOID file is also copied alongside DEM data when :ref:`[Processing].cache_dem_by
+  <Processing.cache_dem_by>` option is on.
+  (`#123 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/123>`_).
+
+v1.1.0 Breaking changes
++++++++++++++++++++++++
+
+- ``ACQUISITION_DATETIME`` image metadata is now in UTC format (e.g.
+  ``2020:01:08T04:41:50Z``). In previous versions it used to have the same
+  format as ``TIFFTAG_DATETIME`` (i.e.: ``2020:01:08 04:41:50``)
+
+
 Version 1.0.0
 -------------
 
 This version is a major improvement over v 0.3.x versions. A few breaking
 changes have been made in parameters, internal API...
 
 v1.0.0 Improvements
@@ -30,16 +80,16 @@
   <DataSource.relative_orbit_list>` and :ref:`tile_to_product_overlap_ratio
   <DataSource.tile_to_product_overlap_ratio>`.
   (`#83 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/83>`_,
   `#110 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/110>`_,
   `#133 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/133>`_.
 
 - Null values obtained after the optional *denoising* done during the
-  :ref:`calibration <calibration>` wil be set to a :ref:`minimal signal value
-  <Processing.lower_signal_value>` > 0. The objective is to keep 0 as the
+  :ref:`calibration <calibration-proc>` wil be set to a :ref:`minimal signal
+  value <Processing.lower_signal_value>` > 0. The objective is to keep 0 as the
   *nodata* value.
   (`#87 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/87>`_).
 
 - Spatial Speckle Filtering is supported
   (`#116 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/116>`_).
 
 - Improve the reporting of search or download failures. Also give another
@@ -49,16 +99,16 @@
   | `#139 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/139>`_)
 
 - On search timeout, S1Tiling will insist a few times (5 by default, can be
   overridden through CLI option). This is meant as a workaround of `EODAG issue
   #908 <https://github.com/CS-SI/eodag/issues/908>`_.
   (`#140 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/140>`_).
 
-v1.0.0 Bug fixed
-++++++++++++++++
+v1.0.0 Bugs fixed
++++++++++++++++++
 
 - Offline S1 products are now correctly detected and processed
   (`#71 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/71>`_,
   `#93 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/93>`_,
   `#108 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/108>`_):
 
     - their associated (and available) products won't be used to produce a S2
@@ -94,16 +144,16 @@
   (`#107 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/107>`_).
 
 Version 0.3.1
 -------------
 
 Bug fixes for version 0.3
 
-v0.3.1 Bug fixed
-++++++++++++++++
+v0.3.1 Bugs fixed
++++++++++++++++++
 
 - Don't produce partial products when complete ones already exist for a given
   S2 tile at a requested time
   (`#104 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/104>`_).
 
 Version 0.3.0
 -------------
@@ -185,16 +235,16 @@
   (`#2 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/2>`_)
 
     - Multiple log files are produced.
     - They can be sent by mail (though configuration)
     - Log level are supported
     - A summary of the successfully of failed computations is provided.
 
-v0.2 Bug fixed
-++++++++++++++
+v0.2 Bugs fixed
++++++++++++++++
 
 - Fix thermnal noise usage ((`#84 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/84>`_)
 - Fix pylint error ((`#82 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/82>`_)
 - Improve the srtm tiles database to avoid to request srtm tile which don't exist ((`#81 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/81>`_)
 - Work on the more complete product when there are multiple overlapping
   products (`#47
   <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/47>`_)
@@ -210,15 +260,15 @@
   (`#4 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/4>`_,
   `#10 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/10>`_,
   `#52 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/10>`_)
 
     - This reduces stress on IO that often are a bottleneck on clusters
 
 - Dedicated and optimized OTB applications have been written for :ref:`cutting
-  <cutting>`  and :ref:`calibration <calibration>`
+  <cutting-proc>`  and :ref:`calibration <calibration-proc>`
 - Execute only the processes that are needed to produce the requested products
 - Parallelization is done with dask
   (`#11 <https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues/11>`_)
 
     - This permits to parallelize computations of different types
 
 - When there is only one file to concatenate, it's simply renamed
```

### Comparing `S1Tiling-1.0.0rc3/docs/testing.rst` & `s1tiling-1.1.0rc1/docs/testing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. _testing:
-
 .. index:: testing
 
 ======================================================================
 Testing
 ======================================================================
 
 .. contents:: Contents:
@@ -55,15 +53,25 @@
 
 
 .. _pytest:
 
 Running the tests
 -----------------
 
-S1 Tiling tests depend on pytest. You can see all the supported options with:
+S1 Tiling tests depend on pytest.
+
+I usually execute the tests with:
+
+.. code:: bash
+
+    SRTM_DIR=/path/to/MNT/SRTM_30_hgt pytest --cov=s1tiling --baselinedir=/path/to/tests/20200306-NR/baseline/ \
+         -k 'not execute_OTB' -vvv --log-cli-level=DEBUG -o log_cli=true --capture=no --junitxml=report.xml \
+         --ram 2048 2>&1 | less -R
+
+You can see all the supported options with:
 
 .. code:: bash
 
     pytest --help
 
 In particular they depend on the following options:
 
@@ -84,17 +92,18 @@
    Directory where the temporary files will be generated.
 
    .. warning::
 
        Don't forget to clean it eventually.
 
 
-.. option:: --srtmdir=SRTMDIR
+.. option:: --demdir=SRTMDIR
 
-   Directory where SRTM files are -- default value: :envvar:`$SRTM_DIR`
+   Directory where DEM (like SRTM) files are -- default value:
+   :envvar:`$SRTM_DIR`.
 
 .. option:: --download
 
    Download the input files with eodag instead of using the compressed ones
    from the baseline. If true, raw S1 products will be downloaded into
    :file:`{tmpdir}/inputs`.
```

### Comparing `S1Tiling-1.0.0rc3/docs/use.rst` & `s1tiling-1.1.0rc1/docs/use.rst`

 * *Files 12% similar despite different names*

```diff
@@ -105,20 +105,19 @@
    If you wish to parallelize this scenario and dedicate a different cluster
    node to each date -- as recommended in ":ref:`scenario.parallelize_date`"
    scenario, you will **NEED** produce all the LIA maps beforehand.
    Otherwise a same file may be concurrently written to from different nodes,
    and it will likely end up corrupted.
 
 .. note::
-   This scenario requires `DiapOTB
-   <https://gitlab.orfeo-toolbox.org/remote_modules/diapotb>`_ and `NORMLIM σ0
+   This scenario requires `NORMLIM σ0
    <https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0>`_ binaries.
-   At this times, DiapOTB binaries are shipped with OTB 7.4 (but not with OTB
-   8), and NORMLIM σ\ :sup:`0` binaries need to be compiled manually.
-   Eventually both will be guaranteed in S1Tiling docker images.
+   At the moment, NORMLIM σ\ :sup:`0` binaries need to be compiled manually.
+   Unless you use either S1Tiling docker images, or S1Tiling on CNES TREX
+   cluster.
 
 
 .. _scenario.S1LIAMap:
 
 Preproduce maps of Local Incidence Angles for σ\ :sup:`0`\ :sub:`RTC` NORMLIM calibration
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
@@ -138,20 +137,19 @@
         S1LIAMap MyS1ToS2.cfg
 
 
 .. note::
    LIA maps are perfect products to be stored and reused.
 
 .. note::
-   This scenario requires `DiapOTB
-   <https://gitlab.orfeo-toolbox.org/remote_modules/diapotb>`_ and `NORMLIM σ0
+   This scenario requires `NORMLIM σ0
    <https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0>`_ binaries.
-   At this times, DiapOTB binaries are shipped with OTB 7.4 (but not with OTB
-   8), and NORMLIM σ\ :sup:`0` binaries need to be compiled manually.
-   Eventually both will be guaranteed in S1Tiling docker images.
+   At the moment, NORMLIM σ\ :sup:`0` binaries need to be compiled manually.
+   Unless you use either S1Tiling docker images, or S1Tiling on CNES TREX
+   cluster.
 
 .. note::
    To run :program:`S1LIAMap` from the official S1Tiling docker, use ``--lia``
    as the first parameter to the docker execution (just before the the
    request configuration file and other S1LIAMap related parameters). See
    :ref:`Using S1LIAMap with a docker <docker.S1LIAMap>`.
 
@@ -184,14 +182,58 @@
 
 .. warning::
    This scenario is not compatible with ``normlim`` calibration where the LIA
    maps would be computed on-the-fly. For ``normlim`` calibration, it's
    imperative to precompute (and store LIA maps) before going massively
    parallel.
 
+
+.. _scenario.choose_dem:
+
+Use any other set of DEM inputs
++++++++++++++++++++++++++++++++
+
+By default S1Tiling comes with a GPKG database that associates SRTM 30 tile ids
+to SRTM geometries.
+
+In order to use other DEM inputs, we need:
+
+1. DEM files stored in :ref:`[PATHS].dem_dir <paths.dem_dir>` directory.
+   |br|
+   The format of these DEM files needs to be supported by OTB/GDAL.
+
+2. A DEM (GPKG) database that holds a key (or set of keys) that enable(s) to
+   locate/name DEM files associated to a DEM geometry.
+   |br|
+   Set the :ref:`[PATHS].dem_database <paths.dem_database>` key accordingly.
+   |br|
+   For instance, `eotile <https://github.com/CS-SI/eotile>`_ provides a couple
+   of DEM databases for various types of DEM files.
+
+3. A naming scheme that will associate an identifier key from the :ref:`DEM
+   database <paths.dem_database>` to a DEM filename (located in
+   :ref:`[PATHS].dem_dir <paths.dem_dir>` directory).
+   |br|
+   Set the :ref:`[PATHS].dem_format <paths.dem_format>` key accordingly.
+   |br|
+   The default :file:`{{id}}.hgt` associates the ``id`` key to STRM 30m DEM
+   files.
+   |br|
+   Using `eotile <https://github.com/CS-SI/eotile>`_ :file:`DEM_Union.gpkg` as
+   DEM database, we could instead use:
+
+   - :file:`{{Product10}}.tif`  for Copernicus 30m DEM files, using
+     ``Product10`` key from the GPKG file.
+   - :file:`{{Product30}}.tif`  for Copernicus 90m DEM files, using
+     ``Product30`` key from the GPKG file.
+
+4. Make sure to use a Geoid file compatible with the chosen DEM. For instance
+   S1Tiling is shipped with EGM96 Geoid with is compatible with SRTM.
+   On the other hand, Copernicus DEM is related to EGM2008 (a.k.a EGM08)
+
 .. _request-config-file:
 
 .. index:: Request configuration file
 
 Request Configuration file
 --------------------------
 
@@ -239,17 +281,38 @@
       sometimes :ref:`cached <data-caches>` for longer periods.
 
       .. _paths.geoid_file:
   * - ``geoid_file``
     - Path to Geoid model. If left unspecified, it'll point automatically to
       the geoid resource shipped with S1 Tiling.
 
+      .. _paths.dem_database:
+  * - ``dem_database``
+    - Path to DEM (``.gpkg``) database.
+      |br|
+      By default points to the internal :file:`shapefile/srtm_tiles.gpkg` file
+      which knows the geometry of SRTM 30 DEM files.
+
+      .. _paths.dem_dir:
+  * - ``dem_dir``
+    - Path to DEM files.
+
+      .. _paths.dem_format:
+  * - ``dem_format``
+    - Filename format string to locate the DEM file associated to an
+      *identifier* within the :ref:`[PATHS].dem_dir <paths.dem_dir>` directory.
+      |br|
+      By default associates the ``id`` key of tiles found in the :ref:`DEM
+      database <paths.dem_database>` to :file:`{{id}}.hgt`. One may want to use
+      the keys from `eotile <https://github.com/CS-SI/eotile>`_ DEM database
+      like for instance :file:`{{Product10}}.tif` for Copernicus 30m DEM.
+
       .. _paths.srtm:
   * - ``srtm``
-    - Path to SRTM files.
+    - **(deprecated)** Use :ref:`[PATHS].dem_dir <paths.dem_dir>`. Path to SRTM files.
 
 .. _DataSource:
 
 ``[DataSource]`` section
 ++++++++++++++++++++++++
 
 .. list-table::
@@ -391,24 +454,28 @@
   :widths: auto
   :header-rows: 1
   :stub-columns: 1
 
   * - Option
     - Description
 
-      .. _Processing.cache_srtm_by:
-  * - ``cache_srtm_by``
-    - Tells whether SRTM files are copied in a temporary directory, or if
-      symbolic links are to be created.
+      .. _Processing.cache_dem_by:
+  * - ``cache_dem_by``
+    - Tells whether DEM and Geoid files are copied in a temporary directory, or
+      if symbolic links are to be created.
 
       For performance reasons with OTB 7.X, it's better to regroup the minimal
-      subset of the SRTM files required for processing. Symbolic links work
+      subset of the DEM files required for processing. Symbolic links work
       fine most of the time, however if the files are on a remote shared
       filesystem (GPFS, NAS...), performances will be degraded. In those cases,
-      it's better to copy the required SRTM files on a local filesystem.
+      it's better to copy the required DEM files on a local filesystem.
+
+      :ref:`Geoid file <paths.geoid_file>` will be also copied (or symlinked),
+      but in :samp:`{{tmp}}/geoid/`. It won't be removed automatically.  You
+      can also do it manually before running S1Tiling.
 
       Two values are supported for this option: ``copy`` and ``symlink``.
       (default: ``symlink``).
 
       .. _Processing.calibration:
   * - ``calibration``
     - Defines the calibration type: ``gamma``, ``beta``, ``sigma``, or
@@ -422,16 +489,16 @@
 
          This feature requires a version of OTB >= 7.4.0
 
       .. _Processing.lower_signal_value:
   * - ``lower_signal_value``
     - Noise removal may set some pixel values to 0.
       However, 0, is currently reserved by S1Tiling chain as a "nodata" value
-      introduced by :ref:`Margin Cutting<cutting>` and :ref:`Orthorectification
-      <orthorectification>`.
+      introduced by :ref:`Margin Cutting<cutting-proc>` and
+      :ref:`Orthorectification <orthorectification-proc>`.
 
       This parameter defines which value to use instead of 0 when :ref:`noise is
       removed <Processing.remove_thermal_noise>`.  By default: 1e-7 will be
       used.
 
       .. _Processing.output_spatial_resolution:
   * - ``output_spatial_resolution``
@@ -531,18 +598,29 @@
 
       .. note::
         This option will be ignored when no LIA sine map is required. The LIA
         sine map is produced by :ref:`S1LIAMap program <scenario.S1LIAMap>` ,
         or when :ref:`calibration mode <Processing.calibration>` is
         ``"normlim"``.
 
+      .. _Processing.dem_warp_resampling_method:
+  * - ``dem_warp_resampling_method``
+    - DEM files projected on S2 tiles are required to produce :ref:`LIA maps
+      <lia-files>`.
+      This parameters permits to select the resampling method that
+      :external:std:doc:`gdalwarp <programs/gdalwarp>` will use.
+
+      The possible values are: ``near``, ``bilinear``, ``cubic``,
+      ``cubicspline``, ``lanczos``, ``average``, ``rms``, ``mode``, ``max``,
+      ``min``, ``med``, ``q1``, ``q3`` and ``qum``.
+
       .. _Processing.override_azimuth_cut_threshold_to:
   * - ``override_azimuth_cut_threshold_to``
     - Permits to override the analysis on whether top/bottom lines shall be
-      forced to 0 in :ref:`cutting step <cutting>`. |br|
+      forced to 0 in :ref:`cutting step <cutting-proc>`. |br|
 
       Possible values are:
 
       :``True``:         Force cutting at the 1600th upper and the 1600th lower
                          lines.
       :``False``:        Force to keep every line.
       :not set/``None``: Default analysis heuristic is used.
@@ -560,15 +638,15 @@
       The filename formats can be overridden for both intermediary and final
       products. Only the final products are documented here. Filename formats
       for intermediary products are best left alone.
 
       If you change any, make sure to not introduce ambiguity by removing a
       field that would be used to distinguish two unrelated products.
 
-      Available fields comme from :func:`internal metadata <s1tiling.libs.otbpipeline.StepFactory.complete_meta>`. The main
+      Available fields come from :func:`internal metadata <s1tiling.libs.steps.StepFactory.complete_meta>`. The main
       ones of interest are:
 
       .. list-table::
         :widths: auto
         :header-rows: 1
         :stub-columns: 1
 
@@ -636,34 +714,135 @@
             S1 image geometry and not its content.
           - S1
 
       .. _Processing.fname_fmt.concatenation:
   * - ``fname_fmt.concatenation``
     - File format pattern for :ref:`concatenation products <full-S2-tiles>`,
       for β°, σ° and γ° calibrations.
-      :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}.tif`
+
+      Default value: :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}.tif`
 
       .. _Processing.fname_fmt.lia_corrected:
   * - ``fname_fmt.s2_lia_corrected``
     - File format pattern for :ref:`concatenation products <full-S2-tiles>`
       when NORMLIM calibrated.
-      :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim.tif`
+
+      Default value: :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim.tif`
 
       .. _Processing.fname_fmt.lia_product:
   * - ``fname_fmt.lia_product``
     - File format pattern for LIA and sin(LIA) files
-      :samp:`{{LIA_kind}}_{{flying_unit_code}}_{{tile_name}}_{{orbit_direction}}_{{orbit}}.tif`
+
+      Default value: :samp:`{{LIA_kind}}_{{flying_unit_code}}_{{tile_name}}_{{orbit_direction}}_{{orbit}}.tif`
 
       .. _Processing.fname_fmt.filtered:
   * - ``fname_fmt.filtered``
     - File format pattern for :ref:`filtered files <filtered-files>`
-      :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_filtered.tif`
+
+      Default value: :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_filtered.tif`
       for β°, σ° and γ° calibrations,
-      :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim_filtered.tif` when NORMLIM calibrated.
 
+      Default value: :samp:`{{flying_unit_code}}_{{tile_name}}_{{polarisation}}_{{orbit_direction}}_{{orbit}}_{{acquisition_stamp}}_NormLim_filtered.tif` when NORMLIM calibrated.
+
+      .. _Processing.dname_fmt:
+  * - ``dname_fmt.*``
+    - Set of directory format templates that permits to override the default
+      directories where products are generated.
+
+      The directory formats can only be overridden for final products.
+
+      The only fields available are:
+
+      .. list-table::
+        :widths: auto
+        :header-rows: 1
+        :stub-columns: 1
+
+        * - Field
+          - Reference to
+
+        * - :samp:`{{tile_name}}`
+          - Name of the related tile.
+        * - :samp:`{{out_dir}}`
+          - :ref:`[PATHS].output <paths.output>`
+        * - :samp:`{{tmp_dir}}`
+          - :ref:`[PATHS].tmp <paths.tmp>`
+        * - :samp:`{{lia_dir}}`
+          - :ref:`[PATHS].lia <paths.lia>`
+
+      .. list-table::
+        :widths: auto
+        :header-rows: 1
+        :stub-columns: 1
+
+        * - Products from
+          - Option ``dname_fmt.?``
+          - Default value
+
+            .. _Processing.dname_fmt.tiled:
+        * - :ref:`(β°/σ°/γ°/NORMLIM) Final tiled product <full-S2-tiles>`
+          - ``.tiled``
+          - :samp:`{{out_dir}}/{{tile_name}}`
+
+            .. _Processing.dname_fmt.mask:
+        * - :ref:`Masks <mask-files>`
+          - ``.mask``
+          - :samp:`{{out_dir}}/{{tile_name}}`
+
+            .. _Processing.dname_fmt.lia_product:
+        * - :ref:`degree(LIA) and sin(LIA) <lia-files>`
+          - ``.lia_product``
+          - :samp:`{{lia_dir}}`
+
+            .. _Processing.dname_fmt.filtered:
+        * - :ref:`Filtering <filtered-files>`
+          - ``.filtered``
+          - :samp:`{{out_dir}}/filtered/{{tile_name}}`
+
+      .. _Processing.creation_options:
+  * - ``creation_options.*``
+    - Set of extra options to create certain products. Creation options take a
+      first and optional pixel type (``uint8``, ``float64``...) and a list of
+      `GDAL creation options
+      <https://gdal.org/drivers/raster/gtiff.html#creation-options>`_.
+
+      .. list-table::
+        :widths: auto
+        :header-rows: 1
+        :stub-columns: 1
+
+        * - Products from
+          - Option ``creation_options.?``
+          - Default value
+
+            .. _Processing.creation_options.tiled:
+        * - Orthorectification, :ref:`(β°/σ°/γ°/NORMLIM) Concatenation
+            <full-S2-tiles>`...
+          - ``.tiled``
+          - ``COMPRESS=DEFLATE&gdal:co:PREDICTOR=3``
+
+            .. _Processing.creation_options.filtered:
+        * - :ref:`Filtering <filtered-files>`
+          - ``.filtered``
+          - ``COMPRESS=DEFLATE&gdal:co:PREDICTOR=3``
+
+            .. _Processing.creation_options.mask:
+        * - :ref:`Masks <mask-files>`
+          - ``.mask``
+          - ``uint8 COMPRESS=DEFLATE``
+
+            .. _Processing.creation_options.lia_deg:
+        * - :ref:`LIA (in degrees * 100) <lia-files>`
+          - ``.lia_deg``
+          - ``uint16 COMPRESS=DEFLATE&gdal``
+
+            .. _Processing.creation_options.lia_sin:
+        * - :ref:`sin(LIA) <lia-files>`
+          - ``.lia_sin``
+          - ``COMPRESS=DEFLATE&gdal:co:PREDICTOR=3``
 
 .. _Filtering:
 
 ``[Filtering]`` section
 +++++++++++++++++++++++
 
 .. note:: Multitemporal filtering is not yet integrated in S1Tiling.
@@ -676,15 +855,15 @@
 
   * - Option
     - Description
 
       .. _Filtering.filter:
   * - ``filter``
     - If ``none`` or empty, then no filtering is done. Otherwise the following
-      spatial speckling filter methods from :std:doc:`OTB Despeckle application
+      spatial speckling filter methods from :external:doc:`OTB Despeckle application
       <Applications/app_Despeckle>` are supported: ``Lee``, ``Frost``,
       ``Gammamap``, ``Kuan``.
 
       .. _Filtering.window_radius:
   * - ``window_radius``
     - Sets the window radius for the spatial filtering. |br|
       Take care that it is a radius, i.e. radius=1 means the filter does an 3x3
@@ -830,15 +1009,15 @@
       Sentinel-2 tiles <DataSource.roi_by_tiles>` within the :ref:`requested
       time range <DataSource.first_date>`.
 
       If :ref:`downloading <DataSource.download>` has been disabled, S1
       products are searched in the :ref:`local input directory
       <paths.s1_images>`.  See the log produced.
   * - 75
-    - Cannot find all the :ref:`SRTM products <paths.srtm>` that cover the
+    - Cannot find all the :ref:`DEM products <paths.dem_dir>` that cover the
       :ref:`requested Sentinel-2 tiles <DataSource.roi_by_tiles>`. See the log
       produced.
   * - 76
     - :ref:`Geoid file <paths.geoid_file>` is missing or the specified path is
       incorrect. See the log produced.
   * - 77
     - Some processing cannot be done because external applications cannot
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/S1Processor.py` & `s1tiling-1.1.0rc1/s1tiling/libs/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # =========================================================================
 #   Program:   S1Processor
 #
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   All rights reserved.
+#   Copyright 2017-2024 (c) CNES.
+#   Copyright 2022-2024 (c) CS GROUP France.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -24,183 +26,162 @@
 #
 # Authors: Thierry KOLECK (CNES)
 #          Luc HERMITTE (CS Group)
 #
 # =========================================================================
 
 """
-S1Tiling Command Line Interface
-
-Usage: S1Processor [OPTIONS] CONFIGFILE
-
-  On demand Ortho-rectification of Sentinel-1 data on Sentinel-2 grid.
-
-  It performs the following steps:
-   1- Download S1 images from S1 data provider (through eodag)
-   2- Calibrate the S1 images to gamma0
-   3- Orthorectify S1 images and cut their on geometric tiles
-   4- Concatenate images from the same orbit on the same tile
-   5- Build mask files
-
-  Parameters have to be set by the user in the S1Processor.cfg file
-
-Options:
-  --version  Show the version and exit.
-  --help     Show this message and exit.
-  --dryrun    Display the processing shall would be realized, but none is done.
-  --debug-otb Investigation mode were OTB Applications are directly used without Dask
-              in order to run them through gdb for instance.
-  --graphs    Generate task graphs showing the processing flow that need to be done.
+Submodule that defines all API related functions and classes.
 """
 
-from __future__ import absolute_import, print_function, unicode_literals
-
 import logging
+import logging.config
 import os
 from pathlib import Path
-import sys
-from typing import Dict, Union, Tuple
+from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Type, Union
 
-import click
 from distributed.scheduler import KilledWorker
 from dask.distributed import Client, LocalCluster
 
-from s1tiling.libs.S1FileManager import (
+from s1tiling.libs.vis import SimpleComputationGraph  # Graphs
+from .S1FileManager import (
         S1FileManager, WorkspaceKinds, EODAG_DEFAULT_DOWNLOAD_WAIT, EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
         EODAG_DEFAULT_SEARCH_MAX_RETRIES, EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
 )
-# from libs import S1FilteringProcessor
-from s1tiling.libs import Utils
-from s1tiling.libs.configuration import Configuration
-from s1tiling.libs.otbpipeline import FirstStep, PipelineDescriptionSequence
-from s1tiling.libs.otbwrappers import (
-        AbstractStep,
+from . import exits
+from . import exceptions
+from . import Utils
+from .configuration import Configuration
+from .otbpipeline import FirstStep, PipelineDescription, PipelineDescriptionSequence, StepFactory, AbstractStep
+from .otbwrappers import (
+        # Main S1 -> S2 Step Factories
         ExtractSentinel1Metadata, AnalyseBorders, Calibrate, CorrectDenoising,
-        CutBorders, OrthoRectify, Concatenate, BuildBorderMask,
-        SmoothBorderMask, AgglomerateDEM, SARDEMProjection,
-        SARCartesianMeanEstimation, ComputeNormals, ComputeLIA, filter_LIA,
-        OrthoRectifyLIA, ConcatenateLIA, SelectBestCoverage,
-        ApplyLIACalibration, SpatialDespeckle)
-from s1tiling.libs import exits
-from s1tiling.libs.outcome import Outcome
+        CutBorders, OrthoRectify, Concatenate, BuildBorderMask, SmoothBorderMask,
+        # LIA relate Step Factories
+        AgglomerateDEMOnS2, ProjectDEMToS2Tile, ProjectGeoidToS2Tile,
+        SumAllHeights, ComputeGroundAndSatPositionsOnDEM,
+        ComputeLIAOnS2, filter_LIA, ComputeNormalsOnS2,
+        ApplyLIACalibration,
+        # Deprecated LIA related Step Factories
+        AgglomerateDEMOnS1, SARDEMProjection, SARCartesianMeanEstimation,
+        ComputeNormalsOnS1, OrthoRectifyLIA, ComputeLIAOnS1, ConcatenateLIA, SelectBestCoverage,
+        # Filter Step Factories
+        SpatialDespeckle)
+from .outcome import Outcome
+
 
-# Graphs
-from s1tiling.libs.vis import SimpleComputationGraph
+logger = logging.getLogger('s1tiling.api')
 
-# logger = None
-logger = logging.getLogger('s1tiling.processor')
 
-def remove_files(files, what: str) -> None:
+def remove_files(files: List[Union[str, Path]], what: str) -> None:
     """
     Removes the files from the disk
     """
     logger.debug("Remove %s: %s", what, files)
     for file_it in files:
         if os.path.exists(file_it):
             os.remove(file_it)
 
 
-def extract_tiles_to_process(cfg, s1_file_manager):
+def extract_tiles_to_process(cfg: Configuration, s1_file_manager: S1FileManager) -> List[str]:
     """
     Deduce from the configuration all the tiles that need to be processed.
     """
-
     logger.info('Requested tiles: %s', cfg.tile_list)
 
     all_requested = False
     tiles_to_process = []
     if cfg.tile_list[0] == "ALL":
         all_requested = True
     else:
         for tile in cfg.tile_list:
+            # TODO: In order to avoid opening the Layer 42 times, Check all tiles at once
             if s1_file_manager.tile_exists(tile):
                 tiles_to_process.append(tile)
             else:
                 logger.warning("Tile %s does not exist, skipping ...", tile)
 
     # We can not require both to process all tiles covered by downloaded products
     # and and download all tiles
 
     if all_requested:
-        if cfg.download and "ALL" in cfg.roi_by_tiles:
-            logger.critical("Can not request to download 'ROI_by_tiles : ALL' if 'Tiles : ALL'."
-                    + " Change either value or deactivate download instead")
-            sys.exit(exits.CONFIG_ERROR)
-        else:
-            tiles_to_process = s1_file_manager.get_tiles_covered_by_products()
-            logger.info("All tiles for which more than %s%% of the surface is covered by products will be produced: %s",
-                    100 * cfg.tile_to_product_overlap_ratio, tiles_to_process)
+        # Check already done in the configuration object
+        assert not (cfg.download and "ALL" in cfg.roi_by_tiles), \
+            "Can not request to download 'ROI_by_tiles : ALL' if 'Tiles : ALL'. Change either value or deactivate download instead"
+        tiles_to_process = s1_file_manager.get_tiles_covered_by_products()
+        logger.info("All tiles for which more than %s%% of the surface is covered by products will be produced: %s",
+                100 * cfg.tile_to_product_overlap_ratio, tiles_to_process)
 
     logger.info('The following tiles will be processed: %s', tiles_to_process)
     return tiles_to_process
 
 
-def check_tiles_to_process(tiles_to_process, s1_file_manager):
+def check_tiles_to_process(tiles_to_process: List[str], s1_file_manager: S1FileManager) -> Tuple[List[str], Dict, Dict[str, Dict]]:
     """
-    Search the SRTM tiles required to process the tiles to process.
+    Search the DEM tiles required to process the tiles to process.
     """
-    needed_srtm_tiles = []
+    needed_dem_tiles = {}
     tiles_to_process_checked = []  # TODO: don't they exactly match tiles_to_process?
 
-    # Analyse SRTM coverage for MGRS tiles to be processed
-    srtm_tiles_check = s1_file_manager.check_srtm_coverage(tiles_to_process)
+    # Analyse DEM coverage for MGRS tiles to be processed
+    dem_tiles_check = s1_file_manager.check_dem_coverage(tiles_to_process)
 
     # For each MGRS tile to process
     for tile in tiles_to_process:
-        logger.info("Check SRTM coverage for %s", tile)
-        # Get SRTM tiles coverage statistics
-        srtm_tiles = srtm_tiles_check[tile]
+        logger.info("Check DEM coverage for %s", tile)
+        # Get DEM tiles coverage statistics
+        dem_tiles = dem_tiles_check[tile]
         current_coverage = 0
-        current_needed_srtm_tiles = []
         # Compute global coverage
-        for (srtm_tile, coverage) in srtm_tiles:
-            current_needed_srtm_tiles.append(srtm_tile)
-            current_coverage += coverage
-        # If SRTM coverage of MGRS tile is enough, process it
-        needed_srtm_tiles += current_needed_srtm_tiles
+        for _, dem_info in dem_tiles.items():
+            current_coverage += dem_info['_coverage']
+        needed_dem_tiles.update(dem_tiles)
+        # If DEM coverage of MGRS tile is enough, process it
         tiles_to_process_checked.append(tile)
         # Round coverage at 3 digits as tile footprint has a very limited precision
         current_coverage = round(current_coverage, 3)
         if current_coverage < 1.:
-            logger.warning("Tile %s has insuficient SRTM coverage (%s%%)",
+            logger.warning("Tile %s has insufficient DEM coverage (%s%%)",
                     tile, 100 * current_coverage)
         else:
             logger.info("-> %s coverage = %s => OK", tile, current_coverage)
 
     # Remove duplicates
-    needed_srtm_tiles = list(set(needed_srtm_tiles))
-    return tiles_to_process_checked, needed_srtm_tiles
+    return tiles_to_process_checked, needed_dem_tiles, dem_tiles_check
 
 
-def check_srtm_tiles(cfg, srtm_tiles_id, srtm_suffix='.hgt'):
+def check_dem_tiles(cfg: Configuration, dem_tile_infos: Dict) -> bool:
     """
-    Check the SRTM tiles exist on disk.
+    Check the DEM tiles exist on disk.
     """
+    fmt = cfg.dem_filename_format
     res = True
-    for srtm_tile in srtm_tiles_id:
-        tile_path_hgt = Path(cfg.srtm, srtm_tile + srtm_suffix)
+    for _, dem_tile_info in dem_tile_infos.items():
+        dem_filename = fmt.format_map(dem_tile_info)
+        tile_path_hgt = Path(cfg.dem, dem_filename)
+        # logger.debug('checking "%s" # "%s" =(%s)=> "%s"', cfg.dem, dem_filename, fmt, tile_path_hgt)
         if not tile_path_hgt.exists():
             res = False
             logger.critical("%s is missing!", tile_path_hgt)
     return res
 
 
-def clean_logs(config, nb_workers) -> None:
+def clean_logs(config: Dict, nb_workers: int) -> None:
     """
     Clean all the log files.
     Meant to be called once, at startup
     """
     filenames = []
     for _, cfg in config['handlers'].items():
         if 'filename' in cfg and '{kind}' in cfg['filename']:
             filenames += [cfg['filename'].format(kind=f"worker-{w}") for w in range(nb_workers)]
     remove_files(filenames, "logs")
 
 
-def setup_worker_logs(config, dask_worker) -> None:
+def setup_worker_logs(config: Dict, dask_worker) -> None:
     """
     Set-up the logger on Dask Worker.
     """
     d_logger = logging.getLogger('distributed.worker')
     r_logger = logging.getLogger()
     old_handlers = d_logger.handlers[:]
 
@@ -215,124 +196,143 @@
         d_logger.addHandler(hdlr)
         r_logger.addHandler(hdlr)  # <-- this way we send s1tiling messages to dask channel
 
     # From now on, redirect stdout/stderr messages to s1tiling
     Utils.RedirectStdToLogger(logging.getLogger('s1tiling'))
 
 
+the_config : Configuration
+
+
 class DaskContext:
     """
     Custom context manager for :class:`dask.distributed.Client` +
     :class:`dask.distributed.LocalCluster` classes.
     """
-    def __init__(self, config, debug_otb):
-        self.__client    = None
-        self.__cluster   = None
-        self.__config    = config
-        self.__debug_otb = debug_otb
+    def __init__(self, config: Configuration, debug_otb: bool) -> None:
+        self.__client    : Optional[Client]       = None
+        self.__cluster   : Optional[LocalCluster] = None
+        self.__config    : Configuration          = config
+        self.__debug_otb : bool                   = debug_otb
 
-    def __enter__(self):
+    def __enter__(self) -> "DaskContext":
         if not self.__debug_otb:
             clean_logs(self.__config.log_config, self.__config.nb_procs)
             self.__cluster = LocalCluster(
                     threads_per_worker=1, processes=True, n_workers=self.__config.nb_procs,
                     silence_logs=False)
             self.__client = Client(self.__cluster)
             # Work around: Cannot pickle local object in lambda...
             global the_config
             the_config = self.__config
             self.__client.register_worker_callbacks(
                     lambda dask_worker: setup_worker_logs(the_config.log_config, dask_worker))
         return self
 
-    def __exit__(self, exception_type, exception_value, exception_traceback):
+    def __exit__(self, exception_type, exception_value, exception_traceback) -> Literal[False]:
         if self.__client:
             self.__client.close()
+            assert self.__cluster, "client existence implies cluster existence"
             self.__cluster.close()
         return False
 
     @property
-    def client(self):
+    def client(self) -> Optional[Client]:
         """
         Return a :class:`dask.distributed.Client`
         """
         return self.__client
 
 
-def _how2str(how: Union[Tuple,AbstractStep]) -> str:
+def _how2str(how: Union[Tuple, AbstractStep]) -> str:
     """
     Make task definition from logger friendly
     """
     if isinstance(how, AbstractStep):
         return str(how)
     else:
         return f"Task(pipeline: {how[1]}; keys: {how[2]})"
 
 
-def _execute_tasks_debug(dsk, tile_name):
+def _execute_tasks_debug(dsk: Dict, tile_name: str) -> List:
     """
     Execute the tasks directly, one after the other, without Dask layer.
     The objective is to be able to debug OTB applications.
     """
     tasks = list(Utils.tsort(dsk, dsk.keys(),
         lambda dasktask_data : [] if isinstance(dasktask_data, FirstStep) else dasktask_data[2])
-        )
-    logger.debug('%s tasks', len(tasks))
+    )
+    logger.debug('Debug execution of %s tasks', len(tasks))
     for product in reversed(tasks):
         how = dsk[product]
         logger.debug('- task: %s <-- %s', product, _how2str(how))
     logger.info('Executing tasks one after the other for %s (debugging OTB)', tile_name)
     results = []
     for product in reversed(tasks):
         how = dsk[product]
         logger.info('- execute: %s <-- %s', product, _how2str(how))
         if not issubclass(type(how), FirstStep):
             results += [how[0](*list(how)[1:])]
     return results
 
 
-def _execute_tasks_with_dask(dsk, tile_name, tile_idx, intersect_raster_list, required_products,
-        client, pipelines, do_watch_ram, debug_tasks):
+def _execute_tasks_with_dask(  # pylint: disable=too-many-arguments
+    dsk:                   Dict[str, Union[Tuple, "FirstStep"]],
+    tile_name:             str,
+    tile_idx:              int,
+    intersect_raster_list: List[Dict],
+    required_products:     List[str],
+    client:                Client,
+    pipelines:             PipelineDescriptionSequence,
+    do_watch_ram:          bool,
+    debug_tasks:           bool
+) -> List:
     """
     Execute the tasks in parallel through Dask.
     """
-    for product, how in dsk.items():
-        logger.debug('- task: %s <-- %s', product, _how2str(how))
-
     if debug_tasks:
         SimpleComputationGraph().simple_graph(
                 dsk, filename=f'tasks-{tile_idx+1}-{tile_name}.svg')
     logger.info('Start S1 -> S2 transformations for %s', tile_name)
     nb_tries = 2
-    for run_attemp in range(1, nb_tries+1):
+    for run_attempt in range(1, nb_tries + 1):
         try:
+            logger.debug("  Execute tasks, attempt #%s", run_attempt)
             results = client.get(dsk, required_products)
             return results
         except KilledWorker as e:
             logger.critical('%s', dir(e))
             logger.exception("Worker %s has been killed when processing %s on %s tile: (%s). Workers will be restarted: %s/%s",
-                    e.last_worker.name, e.task, tile_name, e, run, nb_tries)
+                    e.last_worker.name, e.task, tile_name, e, run_attempt, nb_tries)
             # TODO: don't overwrite previous logs
             # And we'll need to use the synchronous=False parameter to be able to check
             # successful executions but then, how do we clean up futures and all??
             client.restart()
             # Update the list of remaining tasks
-            if run_attemp < nb_tries:
+            if run_attempt < nb_tries:
                 dsk, required_products = pipelines.generate_tasks(tile_name,
                         intersect_raster_list, do_watch_ram=do_watch_ram)
             else:
                 raise
     return []
 
 
-def process_one_tile(
-        tile_name, tile_idx, tiles_nb,
-        s1_file_manager: S1FileManager, pipelines, client,
-        required_workspaces,
-        debug_otb=False, dryrun=False, do_watch_ram=False, debug_tasks=False):
+def process_one_tile(  # pylint: disable=too-many-arguments, too-many-locals
+    tile_name:               str,
+    tile_idx:                int,
+    tiles_nb:                int,
+    s1_file_manager:         S1FileManager,
+    pipelines:               PipelineDescriptionSequence,
+    client:                  Optional[Client],
+    required_workspaces:     List[WorkspaceKinds],
+    debug_otb:               bool = False,
+    dryrun:                  bool = False,
+    do_watch_ram:            bool = False,
+    debug_tasks:             bool = False
+) -> List:
     """
     Process one S2 tile.
 
     I.E. run the OTB pipeline on all the S1 images that match the S2 tile.
     """
     s1_file_manager.ensure_tile_workspaces_exist(tile_name, required_workspaces)
 
@@ -341,81 +341,84 @@
     s1_file_manager.keep_X_latest_S1_files(1000, tile_name)
 
     try:
         with Utils.ExecutionTimer("Downloading images related to " + tile_name, True):
             s1_file_manager.download_images(tiles=[tile_name], dryrun=dryrun)
             # download_images will have updated the list of know products
     except RuntimeError as e:
-        logger.debug('Cannot download S1 images associated to %s: %s', tile_name, e)
+        logger.warning('Cannot download S1 images associated to %s: %s', tile_name, e)
         return [Outcome(e)]
 
-    except BaseException:  # pylint: disable=broad-except
-        logger.exception('Cannot download S1 images associated to %s', tile_name)
-        sys.exit(exits.DOWNLOAD_ERROR)
+    except BaseException as e:
+        logger.debug('Download error intercepted: %s', e)
+        raise exceptions.DownloadS1FileError(tile_name)
 
     with Utils.ExecutionTimer("Intersecting raster list w/ " + tile_name, True):
         intersect_raster_list = s1_file_manager.get_s1_intersect_by_tile(tile_name)
         logger.debug('%s products found to intersect %s: %s', len(intersect_raster_list), tile_name, intersect_raster_list)
 
     if len(intersect_raster_list) == 0:
         logger.info("No intersection with tile %s", tile_name)
         return []
 
-    dsk, required_products = pipelines.generate_tasks(tile_name, intersect_raster_list,
-            do_watch_ram=do_watch_ram)
+    dsk, required_products = pipelines.generate_tasks(tile_name, intersect_raster_list, do_watch_ram)
     logger.debug('######################################################################')
-    logger.debug('Summary of tasks related to S1 -> S2 transformations of %s', tile_name)
+    logger.debug('Summary of %s tasks related to S1 -> S2 transformations of %s', len(dsk), tile_name)
+    for product, how in dsk.items():
+        logger.debug('- task: %s <-- %s', product, _how2str(how))
+
     if debug_otb:
         return _execute_tasks_debug(dsk, tile_name)
     else:
+        assert client, "Dask client shall exist when not debugging calls to OTB applications"
         return _execute_tasks_with_dask(dsk, tile_name, tile_idx, intersect_raster_list,
                 required_products, client, pipelines, do_watch_ram, debug_tasks)
 
 
-def read_config(config_opt):
+def read_config(config_opt: Union[str, Configuration]) -> Configuration:
     """
     The config_opt can be either the configuration filename or an already initialized configuration
     object
     """
     if isinstance(config_opt, str):
         return Configuration(config_opt)
     else:
         return config_opt
 
 
-def _extend_config(config, extra_opts: Dict, overwrite: bool = False):
+def _extend_config(config: Configuration, extra_opts: Dict, overwrite: bool = False) -> Configuration:
     """
     Adds attributes to configuration object.
 
     .. todo:: Configuration object shall be closer to a dictionary to avoid these workarounds...
     """
     for k in extra_opts:
         if overwrite or not hasattr(config, k):
             setattr(config, k, extra_opts[k])
     return config
 
 
-def do_process_with_pipeline(
-        config_opt,
-        pipeline_builder,
-        dl_wait                : int  = EODAG_DEFAULT_DOWNLOAD_WAIT,
-        dl_timeout             : int  = EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
-        searched_items_per_page: int  = EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
-        nb_max_search_retries  : int  = EODAG_DEFAULT_SEARCH_MAX_RETRIES,
-        dryrun                 : bool = False,
-        debug_caches           : bool = False,
-        debug_otb              : bool = False,
-        watch_ram              : bool = False,
-        debug_tasks            : bool = False,
+def do_process_with_pipeline(  # pylint: disable=too-many-arguments, too-many-locals
+    config_opt             : Union[str, Configuration],
+    pipeline_builder,
+    dl_wait                : int  = EODAG_DEFAULT_DOWNLOAD_WAIT,
+    dl_timeout             : int  = EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
+    searched_items_per_page: int  = EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
+    nb_max_search_retries  : int  = EODAG_DEFAULT_SEARCH_MAX_RETRIES,
+    dryrun                 : bool = False,
+    debug_caches           : bool = False,
+    debug_otb              : bool = False,
+    watch_ram              : bool = False,
+    debug_tasks            : bool = False,
 ) -> exits.Situation:
     """
     Internal function for executing pipelines.
     # TODO: parametrize tile loop, product download...
     """
-    config = read_config(config_opt)
+    config: Configuration  = read_config(config_opt)
     extra_opts = {
             "dl_wait"                : dl_wait,
             "dl_timeout"             : dl_timeout,
             "searched_items_per_page": searched_items_per_page,
             "nb_max_search_retries"  : nb_max_search_retries,
     }
     _extend_config(config, extra_opts, overwrite=False)
@@ -423,141 +426,261 @@
     os.environ["ITK_GLOBAL_DEFAULT_NUMBER_OF_THREADS"] = str(config.OTBThreads)
     # For the OTB applications that don't receive the path as a parameter (like SARDEMProjection)
     # -> we set $OTB_GEOID_FILE
     os.environ["OTB_GEOID_FILE"] = config.GeoidFile
     with S1FileManager(config) as s1_file_manager:
         tiles_to_process = extract_tiles_to_process(config, s1_file_manager)
         if len(tiles_to_process) == 0:
-            logger.critical("No existing tiles found, exiting ...")
-            sys.exit(exits.NO_S2_TILE)
+            raise exceptions.NoS2TileError()
 
-        tiles_to_process_checked, needed_srtm_tiles = check_tiles_to_process(
+        tiles_to_process_checked, needed_dem_tiles, dems_by_s2_tiles = check_tiles_to_process(
                 tiles_to_process, s1_file_manager)
 
         logger.info("%s images to process on %s tiles",
                 s1_file_manager.nb_images, tiles_to_process_checked)
 
         if len(tiles_to_process_checked) == 0:
-            logger.critical("No tiles to process, exiting ...")
-            sys.exit(exits.NO_S1_IMAGE)
+            raise exceptions.NoS1ImageError()
 
-        logger.info("Required SRTM tiles: %s", needed_srtm_tiles)
+        logger.info("Required DEM tiles: %s", list(needed_dem_tiles.keys()))
 
-        if not check_srtm_tiles(config, needed_srtm_tiles):
-            logger.critical("Some SRTM tiles are missing, exiting ...")
-            sys.exit(exits.MISSING_SRTM)
+        if not check_dem_tiles(config, needed_dem_tiles):
+            raise exceptions.MissingDEMError()
 
         if not os.path.exists(config.GeoidFile):
-            logger.critical("Geoid file does not exists (%s), exiting ...", config.GeoidFile)
-            sys.exit(exits.MISSING_GEOID)
+            raise exceptions.MissingGeoidError(config.GeoidFile)
 
         # Prepare directories where to store temporary files
         # These directories won't be cleaned up automatically
         S1_tmp_dir = os.path.join(config.tmpdir, 'S1')
         os.makedirs(S1_tmp_dir, exist_ok=True)
 
-        config.tmp_srtm_dir = s1_file_manager.tmpsrtmdir(needed_srtm_tiles)
+        config.tmp_dem_dir = s1_file_manager.tmpdemdir(
+                needed_dem_tiles, config.dem_filename_format,
+                config.GeoidFile)
 
         pipelines, required_workspaces = pipeline_builder(config, dryrun=dryrun, debug_caches=debug_caches)
+        config.register_dems_related_to_S2_tiles(dems_by_s2_tiles)
 
-        log_level = lambda res: logging.INFO if bool(res) else logging.WARNING
+        log_level : Callable[[Any], int] = lambda res: logging.INFO if bool(res) else logging.WARNING
+        results = []
         with DaskContext(config, debug_otb) as dask_client:
-            results = []
             for idx, tile_it in enumerate(tiles_to_process_checked):
                 with Utils.ExecutionTimer("Processing of tile " + tile_it, True):
                     res = process_one_tile(
                             tile_it, idx, len(tiles_to_process_checked),
                             s1_file_manager, pipelines, dask_client.client,
                             required_workspaces,
                             debug_otb=debug_otb, dryrun=dryrun, do_watch_ram=watch_ram,
                             debug_tasks=debug_tasks)
                     results += res
 
-            nb_errors_detected = sum(not bool(res) for res in results)
+        nb_errors_detected = sum(not bool(res) for res in results)
 
-            skipped_for_download_failures = s1_file_manager.get_skipped_S2_products()
-            results.extend([fp for fp in skipped_for_download_failures])
+        skipped_for_download_failures = s1_file_manager.get_skipped_S2_products()
+        results.extend(skipped_for_download_failures)
 
-            logger.debug('#############################################################################')
-            nb_issues = nb_errors_detected + len(skipped_for_download_failures)
-            if nb_issues > 0:
-                logger.warning('Execution report: %s errors detected', nb_issues)
-            else:
-                logger.info('Execution report: no error detected')
+        logger.debug('#############################################################################')
+        nb_issues = nb_errors_detected + len(skipped_for_download_failures)
+        if nb_issues > 0:
+            logger.warning('Execution report: %s errors detected', nb_issues)
+        else:
+            logger.info('Execution report: no error detected')
 
-            if results:
-                for res in results:
-                    logger.log(log_level(res), ' - %s', res)
-            else:
-                logger.info(' -> Nothing has been executed')
+        if results:
+            for res in results:
+                logger.log(log_level(res), ' - %s', res)
+        else:
+            logger.info(' -> Nothing has been executed')
 
-            search_failures   = s1_file_manager.get_search_failures()
-            download_failures = s1_file_manager.get_download_failures()
-            download_timeouts = s1_file_manager.get_download_timeouts()
-            return exits.Situation(
-                    nb_computation_errors=nb_errors_detected - search_failures,
-                    nb_search_failures=search_failures,
-                    nb_download_failures=len(download_failures),
-                    nb_download_timeouts=len(download_timeouts)
-                    )
+        search_failures   = s1_file_manager.get_search_failures()
+        download_failures = s1_file_manager.get_download_failures()
+        download_timeouts = s1_file_manager.get_download_timeouts()
+        return exits.Situation(
+                nb_computation_errors=nb_errors_detected - search_failures,
+                nb_search_failures=search_failures,
+                nb_download_failures=len(download_failures),
+                nb_download_timeouts=len(download_timeouts)
+        )
 
 
-def register_LIA_pipelines(pipelines: PipelineDescriptionSequence, produce_angles: bool):
+def register_LIA_pipelines_v0(pipelines: PipelineDescriptionSequence, produce_angles: bool) -> PipelineDescription:
     """
     Internal function that takes care to register all pipelines related to
     LIA map and sin(LIA) map.
     """
-    dem = pipelines.register_pipeline([AgglomerateDEM], 'AgglomerateDEM',
+    dem = pipelines.register_pipeline([AgglomerateDEMOnS1], 'AgglomerateDEM',
             inputs={'insar': 'basename'})
+
     demproj = pipelines.register_pipeline([ExtractSentinel1Metadata, SARDEMProjection], 'SARDEMProjection', is_name_incremental=True,
             inputs={'insar': 'basename', 'indem': dem})
     xyz = pipelines.register_pipeline([SARCartesianMeanEstimation],                     'SARCartesianMeanEstimation',
             inputs={'insar': 'basename', 'indem': dem, 'indemproj': demproj})
-    lia = pipelines.register_pipeline([ComputeNormals, ComputeLIA],                     'Normals|LIA', is_name_incremental=True,
+    lia = pipelines.register_pipeline([ComputeNormalsOnS1, ComputeLIAOnS1],                     'Normals|LIA', is_name_incremental=True,
             inputs={'xyz': xyz})
 
     # "inputs" parameter doesn't need to be specified in the following pipeline declarations
     # but we still use it for clarity!
-    ortho           = pipelines.register_pipeline([filter_LIA('LIA'), OrthoRectifyLIA],        'OrthoLIA',  inputs={'in': lia}, is_name_incremental=True)
-    concat          = pipelines.register_pipeline([ConcatenateLIA],                            'ConcatLIA', inputs={'in': ortho})
-    pipelines.register_pipeline([SelectBestCoverage],                                          'SelectLIA', inputs={'in': concat}, product_required=produce_angles)
-
-    ortho_sin       = pipelines.register_pipeline([filter_LIA('sin_LIA'), OrthoRectifyLIA],    'OrthoSinLIA',  inputs={'in': lia}, is_name_incremental=True)
-    concat_sin      = pipelines.register_pipeline([ConcatenateLIA],                            'ConcatSinLIA', inputs={'in': ortho_sin})
-    best_concat_sin = pipelines.register_pipeline([SelectBestCoverage],                        'SelectSinLIA', inputs={'in': concat_sin}, product_required=True)
+    ortho_deg       = pipelines.register_pipeline(
+            [filter_LIA('LIA'), OrthoRectifyLIA],
+            'OrthoLIA',
+            inputs={'in': lia},
+            is_name_incremental=True)
+    concat_deg      = pipelines.register_pipeline(
+            [ConcatenateLIA],
+            'ConcatLIA',
+            inputs={'in': ortho_deg})
+    pipelines.register_pipeline(
+            [SelectBestCoverage],
+            'SelectLIA',
+            inputs={'in': concat_deg},
+            product_required=produce_angles)
+
+    ortho_sin       = pipelines.register_pipeline(
+            [filter_LIA('sin_LIA'), OrthoRectifyLIA],
+            'OrthoSinLIA',
+            inputs={'in': lia},
+            is_name_incremental=True)
+    concat_sin      = pipelines.register_pipeline(
+            [ConcatenateLIA],
+            'ConcatSinLIA',
+            inputs={'in': ortho_sin})
+    best_concat_sin = pipelines.register_pipeline(
+            [SelectBestCoverage],
+            'SelectSinLIA',
+            inputs={'in': concat_sin},
+            product_required=True)
 
     return best_concat_sin
 
 
-def s1_process(
-        config_opt,
+def register_LIA_pipelines(pipelines: PipelineDescriptionSequence, produce_angles: bool) -> PipelineDescription:
+    """
+    Internal function that takes care to register all pipelines related to
+    LIA map and sin(LIA) map.
+    """
+    dem_vrt = pipelines.register_pipeline(
+            [AgglomerateDEMOnS2], 'AgglomerateDEM',
+            inputs={'tilename': 'tilename'},
+    )
+
+    s2_dem = pipelines.register_pipeline(
+            [ProjectDEMToS2Tile], "ProjectDEMToS2Tile",
+            is_name_incremental=True,
+            inputs={"indem": dem_vrt}
+    )
+
+    s2_height = pipelines.register_pipeline(
+            [ProjectGeoidToS2Tile, SumAllHeights], "GenerateHeightForS2Tile",
+            is_name_incremental=True,
+            inputs={"in_s2_dem": s2_dem},
+    )
+
+    # Notes:
+    # * ComputeGroundAndSatPositionsOnDEM cannot be merged in memory with
+    #   normals production AND LIA production: indeed the XYZ, and satposXYZ
+    #   data needs to be reused several times, and in-memory pipeline can't
+    #   support that (yet?)
+    # * ExtractSentinel1Metadata needs to be in its own pipeline to make sure
+    #   all meta are available later on to filter on the coverage.
+    # * ComputeGroundAndSatPositionsOnDEM takes care of filtering on the
+    #   coverage. We don't need any SelectBestS1onS2Coverage prior to this step.
+    sar = pipelines.register_pipeline(
+            [ExtractSentinel1Metadata],
+            inputs={'inrawsar': 'basename'}
+    )
+    xyz = pipelines.register_pipeline(
+            [ComputeGroundAndSatPositionsOnDEM],
+            "ComputeGroundAndSatPositionsOnDEM",
+            inputs={'insar': sar, 'inheight': s2_height},
+    )
+
+    # Always generate sin(LIA). If LIA° is requested, then it's also a
+    # final/requested product.
+    # produce_angles is ignored as there is no extra select_LIA step
+    lia = pipelines.register_pipeline(
+            [ComputeNormalsOnS2, ComputeLIAOnS2],
+            'ComputeLIAOnS2',
+            is_name_incremental=True,
+            inputs={'xyz': xyz},
+            product_required=True,
+    )
+    return lia
+
+
+def s1_process(  # pylint: disable=too-many-arguments, too-many-locals
+        config_opt              : Union[str, Configuration],
         dl_wait                 : int  = EODAG_DEFAULT_DOWNLOAD_WAIT,
         dl_timeout              : int  = EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
         searched_items_per_page : int  = EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
         nb_max_search_retries   : int  = EODAG_DEFAULT_SEARCH_MAX_RETRIES,
         dryrun                  : bool = False,
         debug_otb               : bool = False,
         debug_caches            : bool = False,
         watch_ram               : bool = False,
         debug_tasks             : bool = False,
-        cache_before_ortho      : bool = False
+        cache_before_ortho      : bool = False,
+        lia_process                    = None,
 ) -> exits.Situation:
     """
-      On demand Ortho-rectification of Sentinel-1 data on Sentinel-2 grid.
-
-      It performs the following steps:
-      1. Download S1 images from S1 data provider (through eodag)
-      2. Calibrate the S1 images to gamma0
-      3. Orthorectify S1 images and cut their on geometric tiles
-      4. Concatenate images from the same orbit on the same tile
-      5. Build mask files
+    Entry point to :ref:`S1Tiling classic scenario <scenario.S1Processor>` and
+    :ref:`S1Tiling NORMLIM scenario <scenario.S1ProcessorLIA>` of on demand
+    Ortho-rectification of Sentinel-1 data on Sentinel-2 grid for all
+    calibration kinds.
+
+    It performs the following steps:
+
+    1. Download S1 images from S1 data provider (through eodag)
+        This step may be ignored if ``config_opt`` *download* option is false;
+    2. Calibrate the S1 images according to the *calibration* option from ``config_opt``;
+    3. Orthorectify S1 images and cut their on geometric tiles;
+    4. Concatenate images from the same orbit on the same tile;
+    5. Build mask files;
+    6. Despeckle final images.
+
+    :param config_opt:
+        Either a :ref:`request configuration file <request-config-file>` or a
+        :class:`s1tiling.libs.configuration.Configuration` instance.
+    :param dl_wait:
+        Permits to override EODAG default wait time in minutes between two
+        download tries.
+    :param dl_timeout:
+        Permits to override EODAG default maximum time in mins before stop
+        retrying to download (default=20)
+    :param searched_items_per_page:
+        Tells how many items are to be returned by EODAG when searching for S1
+        images.
+    :param dryrun:
+        Used for debugging: external (OTB/GDAL) application aren't executed.
+    :param debug_otb:
+        Used for debugging: Don't execute processing tasks in DASK workers but
+        directly in order to be able to analyse OTB/external application
+        through a debugger.
+    :param debug_caches:
+        Used for debugging: Don't delete the intermediary files but leave them
+        behind.
+    :param watch_ram:
+        Used for debugging: Monitoring Python/Dask RAM consumption.
+    :param debug_tasks:
+        Generate SVG images showing task graphs of the processing flows
+    :param cache_before_ortho:
+        Cutting, calibration and orthorectification are chained in memory
+        unless this option is true. In that case, :ref:`Cut and calibrated (aka
+        "OrthoReady") files <orthoready-files>` are stored in :ref:`%(tmp)
+        <paths.tmp>`:samp:`/S1/` directory.
+        Do not forget to regularly clean up this space.
+
+    :return:
+        A *nominal* exit code depending of whether everything could have been
+        downloaded and produced.
+    :rtype: :class:`s1tiling.libs.exits.Situation`
 
-      Parameters have to be set by the user in the S1Processor.cfg file
+    :exception Error: A variety of exceptions. See below (follow the link).
     """
-    def builder(config, dryrun, debug_caches):
+    def builder(config: Configuration, dryrun: bool, debug_caches: bool) -> Tuple[PipelineDescriptionSequence, List[WorkspaceKinds]]:
         assert (not config.filter) or (config.keep_non_filtered_products or not config.mask_cond), \
                 'Cannot purge non filtered products when mask are also produced!'
 
         chain_LIA_and_despeckle_inmemory    = config.filter and not config.keep_non_filtered_products
         chain_concat_and_despeckle_inmemory = False  # See issue #118
 
         pipelines = PipelineDescriptionSequence(config, dryrun=dryrun, debug_caches=debug_caches)
@@ -574,45 +697,61 @@
         else:
             calib_seq += [OrthoRectify]
             pipelines.register_pipeline(calib_seq, 'FullOrtho', product_required=False, is_name_incremental=True)
 
         calibration_is_done_in_S1 = config.calibration_type in ['sigma', 'beta', 'gamma', 'dn']
 
         # Concatenation (... + Despeckle)  // not working yet, see issue #118
-        concat_seq = [Concatenate]
+        concat_seq : List[Type[StepFactory]] = [Concatenate]
         if chain_concat_and_despeckle_inmemory:
             concat_seq.append(SpatialDespeckle)
             need_to_keep_non_filtered_products = False
         else:
             need_to_keep_non_filtered_products = True
 
-        concat_S2 = pipelines.register_pipeline(concat_seq, product_required=calibration_is_done_in_S1, is_name_incremental=True)
+        concat_S2 = pipelines.register_pipeline(
+                concat_seq,
+                product_required=calibration_is_done_in_S1,
+                is_name_incremental=True
+        )
         last_product_S2 = concat_S2
 
         required_workspaces = [WorkspaceKinds.TILE]
 
         # LIA Calibration (...+ Despeckle)
         if config.calibration_type == 'normlim':
-            apply_LIA_seq = [ApplyLIACalibration]
+            apply_LIA_seq : List[Type[StepFactory]] = [ApplyLIACalibration]
             if chain_LIA_and_despeckle_inmemory:
                 apply_LIA_seq.append(SpatialDespeckle)
                 need_to_keep_non_filtered_products = False
             else:
                 need_to_keep_non_filtered_products = True
 
-            concat_sin = register_LIA_pipelines(pipelines, produce_angles=config.produce_lia_map)
+            LIA_registration = lia_process or register_LIA_pipelines
+            lias = LIA_registration(pipelines, config.produce_lia_map)
+
+            # This steps helps forwarding sin(LIA) (only) to the next step
+            # that corrects the β° with sin(LIA) map.
+            sin_LIA = pipelines.register_pipeline(
+                    [filter_LIA('sin_LIA')],
+                    'SelectSinLIA',
+                    is_name_incremental=True,
+                    inputs={'in': lias},
+            )
+            # TODO: Merge filter_LIA in apply_LIA_seq!
             apply_LIA = pipelines.register_pipeline(apply_LIA_seq, product_required=True,
-                    inputs={'sin_LIA': concat_sin, 'concat_S2': concat_S2}, is_name_incremental=True)
+                    inputs={'sin_LIA': sin_LIA, 'concat_S2': concat_S2}, is_name_incremental=True)
             last_product_S2 = apply_LIA
             required_workspaces.append(WorkspaceKinds.LIA)
 
         # Masking
         if config.mask_cond:
             pipelines.register_pipeline([BuildBorderMask, SmoothBorderMask], 'GenerateMask',
                     product_required=True, inputs={'in': last_product_S2})
+            required_workspaces.append(WorkspaceKinds.MASK)
 
         # Despeckle in non-inmemory case
         if config.filter:
             # Use SpatialDespeckle, only if filter ∈ [lee, gammamap, frost, kuan]
             required_workspaces.append(WorkspaceKinds.FILTER)
             if need_to_keep_non_filtered_products:  # config.keep_non_filtered_products:
                 # Define another pipeline if chaining cannot be done in memory
@@ -627,190 +766,166 @@
             searched_items_per_page=searched_items_per_page,
             nb_max_search_retries=nb_max_search_retries,
             dryrun=dryrun,
             debug_otb=debug_otb,
             debug_caches=debug_caches,
             watch_ram=watch_ram,
             debug_tasks=debug_tasks,
-            )
+    )
 
 
-def s1_process_lia(
-        config_opt,
+def s1_process_lia_v0(  # pylint: disable=too-many-arguments
+        config_opt             : Union[str, Configuration],
         dl_wait                : int  = EODAG_DEFAULT_DOWNLOAD_WAIT,
         dl_timeout             : int  = EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
         searched_items_per_page: int  = EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
         nb_max_search_retries  : int  = EODAG_DEFAULT_SEARCH_MAX_RETRIES,
         dryrun                 : bool = False,
         debug_otb              : bool = False,
         debug_caches           : bool = False,
         watch_ram              : bool = False,
         debug_tasks            : bool = False,
 ) -> exits.Situation:
     """
-      Generate Local Incidence Angle Maps on S2 geometry.
+    Entry point to :ref:`LIA Map production scenario <scenario.S1LIAMap>` that
+    generates Local Incidence Angle Maps on S2 geometry.
+
+    It performs the following steps:
+
+    1. Determine the S1 products to process
+        Given a list of S2 tiles, we first determine the day that'll the best
+        coverage of each S2 tile in terms of S1 products.
+
+        In case there is no single day that gives the best coverage for all
+        S2 tiles, we try to determine the best solution that minimizes the
+        number of S1 products to download and process.
+    2. Process these S1 products
+
+    :param config_opt:
+        Either a :ref:`request configuration file <request-config-file>` or a
+        :class:`s1tiling.libs.configuration.Configuration` instance.
+    :param dl_wait:
+        Permits to override EODAG default wait time in minutes between two
+        download tries.
+    :param dl_timeout:
+        Permits to override EODAG default maximum time in mins before stop
+        retrying to download (default=20)
+    :param searched_items_per_page:
+        Tells how many items are to be returned by EODAG when searching for S1
+        images.
+    :param dryrun:
+        Used for debugging: external (OTB/GDAL) application aren't executed.
+    :param debug_otb:
+        Used for debugging: Don't execute processing tasks in DASK workers but
+        directly in order to be able to analyse OTB/external application
+        through a debugger.
+    :param debug_caches:
+        Used for debugging: Don't delete the intermediary files but leave them
+        behind.
+    :param watch_ram:
+        Used for debugging: Monitoring Python/Dask RAM consumption.
+    :param debug_tasks:
+        Generate SVG images showing task graphs of the processing flows
+
+    :return:
+        A *nominal* exit code depending of whether everything could have been
+        downloaded and produced.
+    :rtype: :class:`s1tiling.libs.exits.Situation`
 
-      1. Determine the S1 products to process
-          Given a list of S2 tiles, we first determine the day that'll the best
-          coverage of each S2 tile in terms of S1 products.
-
-          In case there is no single day that gives the best coverage for all
-          S2 tiles, we try to determine the best solution that minimizes the
-          number of S1 products to download and process.
-      2. Process these S1 products
+    :exception Error: A variety of exceptions. See below (follow the link).
     """
-    def builder(config, dryrun, debug_caches):
+    def builder(config: Configuration, dryrun: bool, debug_caches: bool) -> Tuple[PipelineDescriptionSequence, List[WorkspaceKinds]]:
         pipelines = PipelineDescriptionSequence(config, dryrun=dryrun, debug_caches=debug_caches)
-        register_LIA_pipelines(pipelines, produce_angles=config.produce_lia_map)
+        register_LIA_pipelines_v0(pipelines, produce_angles=config.produce_lia_map)
         required_workspaces = [WorkspaceKinds.LIA]
         return pipelines, required_workspaces
 
     return do_process_with_pipeline(
             config_opt, builder,
             dl_wait=dl_wait, dl_timeout=dl_timeout,
             searched_items_per_page=searched_items_per_page,
             nb_max_search_retries=nb_max_search_retries,
             dryrun=dryrun,
             debug_caches=debug_caches,
             debug_otb=debug_otb,
             watch_ram=watch_ram,
             debug_tasks=debug_tasks,
-            )
+    )
 
-# ======================================================================
-@click.command(context_settings=dict(help_option_names=["-h", "--help"]))
-@click.version_option()
-@click.option(
-        "--cache-before-ortho/--no-cache-before-ortho",
-        is_flag=True,
-        default=False,
-        help="""Force to store Calibration|Cutting result on disk before orthorectorectification.
-
-        BEWARE, this option will produce temporary files that you'll need to explicitely delete.""")
-@click.option(
-        "--searched_items_per_page",
-        default=EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
-        help="Number of products simultaneously requested by eodag"
-        )
-@click.option(
-        "--nb_max_search_retries",
-        default=EODAG_DEFAULT_SEARCH_MAX_RETRIES,
-        help="Number of times to retry on timeout when searching for compatible remote products"
-        )
-@click.option(
-        "--eodag_download_timeout",
-        default=EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
-        help="If download fails, maximum time in mins before stop retrying to download (default: 20 mins)"
-        )
-@click.option(
-        "--eodag_download_wait",
-        default=EODAG_DEFAULT_DOWNLOAD_WAIT,
-        help="If download fails, wait time in minutes between two download tries (default: 2 mins)"
-        )
-@click.option(
-        "--dryrun",
-        is_flag=True,
-        help="Display the processing shall would be realized, but none is done.")
-@click.option(
-        "--debug-otb",
-        is_flag=True,
-        help="Investigation mode were OTB Applications are directly used without Dask in order to run them through gdb for instance.")
-@click.option(
-        "--debug-caches",
-        is_flag=True,
-        help="Investigation mode were intermediary cached files are not purged.")
-@click.option(
-        "--watch-ram",
-        is_flag=True,
-        help="Trigger investigation mode for watching memory usage")
-@click.option(
-        "--graphs", "debug_tasks",
-        is_flag=True,
-        help="Generate SVG images showing task graphs of the processing flows")
-@click.argument('config_filename', type=click.Path(exists=True))
-def run( searched_items_per_page, nb_max_search_retries, dryrun, debug_caches, debug_otb, watch_ram,
-         debug_tasks, cache_before_ortho, config_filename,
-         eodag_download_wait, eodag_download_timeout):
-    """
-    This function is used as entry point to create console scripts with setuptools.
-
-    Returns the number of tasks that could not be processed.
-    """
-    situation = s1_process(
-            config_filename,
-            dl_wait=eodag_download_wait, dl_timeout=eodag_download_timeout,
-            searched_items_per_page=searched_items_per_page,
-            nb_max_search_retries=nb_max_search_retries,
-            dryrun=dryrun,
-            debug_otb=debug_otb,
-            debug_caches=debug_caches,
-            watch_ram=watch_ram,
-            debug_tasks=debug_tasks,
-            cache_before_ortho=cache_before_ortho)
-    sys.exit(situation.code)
 
-# ======================================================================
-@click.command(context_settings=dict(help_option_names=["-h", "--help"]))
-@click.version_option()
-@click.option(
-        "--searched_items_per_page",
-        default=EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
-        help="Number of products simultaneously requested by eodag"
-        )
-@click.option(
-        "--nb_max_search_retries",
-        default=EODAG_DEFAULT_SEARCH_MAX_RETRIES,
-        help="Number of times to retry on timeout when searching for compatible remote products"
-        )
-@click.option(
-        "--eodag_download_timeout",
-        default=EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
-        help="If download fails, maximum time in mins before stop retrying to download"
-        )
-@click.option(
-        "--eodag_download_wait",
-        default=EODAG_DEFAULT_DOWNLOAD_WAIT,
-        help="If download fails, wait time in minutes between two download tries"
-        )
-@click.option(
-        "--dryrun",
-        is_flag=True,
-        help="Display the processing shall would be realized, but none is done.")
-@click.option(
-        "--debug-otb",
-        is_flag=True,
-        help="Investigation mode were OTB Applications are directly used without Dask in order to run them through gdb for instance.")
-@click.option(
-        "--debug-caches",
-        is_flag=True,
-        help="Investigation mode were intermediary cached files are not purged.")
-@click.option(
-        "--watch-ram",
-        is_flag=True,
-        help="Trigger investigation mode for watching memory usage")
-@click.option(
-        "--graphs", "debug_tasks",
-        is_flag=True,
-        help="Generate SVG images showing task graphs of the processing flows")
-@click.argument('config_filename', type=click.Path(exists=True))
-def run_lia( searched_items_per_page, nb_max_search_retries, dryrun, debug_otb, debug_caches, watch_ram,
-         debug_tasks, config_filename, eodag_download_wait, eodag_download_timeout):
-    """
-    This function is used as entry point to create console scripts with setuptools.
-
-    Returns the number of tasks that could not be processed.
-    """
-    situation = s1_process_lia(
-            config_filename,
-            dl_wait=eodag_download_wait, dl_timeout=eodag_download_timeout,
+def s1_process_lia(  # pylint: disable=too-many-arguments
+        config_opt             : Union[str, Configuration],
+        dl_wait                : int  = EODAG_DEFAULT_DOWNLOAD_WAIT,
+        dl_timeout             : int  = EODAG_DEFAULT_DOWNLOAD_TIMEOUT,
+        searched_items_per_page: int  = EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE,
+        nb_max_search_retries  : int  = EODAG_DEFAULT_SEARCH_MAX_RETRIES,
+        dryrun                 : bool = False,
+        debug_otb              : bool = False,
+        debug_caches           : bool = False,
+        watch_ram              : bool = False,
+        debug_tasks            : bool = False,
+) -> exits.Situation:
+    """
+    Entry point to :ref:`LIA Map production scenario <scenario.S1LIAMap>` that
+    generates Local Incidence Angle Maps on S2 geometry.
+
+    It performs the following steps:
+
+    1. Determine the S1 products to process
+        Given a list of S2 tiles, we first determine the day that'll the best
+        coverage of each S2 tile in terms of S1 products.
+
+        In case there is no single day that gives the best coverage for all
+        S2 tiles, we try to determine the best solution that minimizes the
+        number of S1 products to download and process.
+    2. Process these S1 products
+
+    :param config_opt:
+        Either a :ref:`request configuration file <request-config-file>` or a
+        :class:`s1tiling.libs.configuration.Configuration` instance.
+    :param dl_wait:
+        Permits to override EODAG default wait time in minutes between two
+        download tries.
+    :param dl_timeout:
+        Permits to override EODAG default maximum time in mins before stop
+        retrying to download (default=20)
+    :param searched_items_per_page:
+        Tells how many items are to be returned by EODAG when searching for S1
+        images.
+    :param dryrun:
+        Used for debugging: external (OTB/GDAL) application aren't executed.
+    :param debug_otb:
+        Used for debugging: Don't execute processing tasks in DASK workers but
+        directly in order to be able to analyse OTB/external application
+        through a debugger.
+    :param debug_caches:
+        Used for debugging: Don't delete the intermediary files but leave them
+        behind.
+    :param watch_ram:
+        Used for debugging: Monitoring Python/Dask RAM consumption.
+    :param debug_tasks:
+        Generate SVG images showing task graphs of the processing flows
+
+    :return:
+        A *nominal* exit code depending of whether everything could have been
+        downloaded and produced.
+    :rtype: :class:`s1tiling.libs.exits.Situation`
+
+    :exception Error: A variety of exceptions. See below (follow the link).
+    """
+    def builder(config: Configuration, dryrun: bool, debug_caches: bool) -> Tuple[PipelineDescriptionSequence, List[WorkspaceKinds]]:
+        pipelines = PipelineDescriptionSequence(config, dryrun=dryrun, debug_caches=debug_caches)
+        register_LIA_pipelines(pipelines, produce_angles=config.produce_lia_map)
+        required_workspaces = [WorkspaceKinds.LIA]
+        return pipelines, required_workspaces
+
+    return do_process_with_pipeline(
+            config_opt, builder,
+            dl_wait=dl_wait, dl_timeout=dl_timeout,
             searched_items_per_page=searched_items_per_page,
             nb_max_search_retries=nb_max_search_retries,
             dryrun=dryrun,
-            debug_otb=debug_otb,
             debug_caches=debug_caches,
+            debug_otb=debug_otb,
             watch_ram=watch_ram,
-            debug_tasks=debug_tasks)
-    sys.exit(situation.code)
-
-# ======================================================================
-if __name__ == '__main__':  # Required for Dask: https://github.com/dask/distributed/issues/2422
-    run()
+            debug_tasks=debug_tasks,
+    )
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/__init__.py` & `s1tiling-1.1.0rc1/s1tiling/__init__.py`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/__meta__.py` & `s1tiling-1.1.0rc1/s1tiling/__meta__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # =========================================================================
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   Copyright 2017-2024 (c) CNES. All rights reserved.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -29,13 +29,13 @@
 Holds project meta-information for setup.py
 """
 
 from __future__ import unicode_literals
 
 __title__ = "S1Tiling"
 __description__ = "On demand Ortho-rectification of Sentinel-1 data on Sentinel-2 grid."
-__version__ = "1.0.0rc3"
+__version__ = "1.1.0rc1"
 __author__ = "Thierry KOLECK"
 __author_email__ = "Thierry.Koleck@cnes.fr"
 __url__ = "https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling"
 __license__ = "Apache 2.0"
-__copyright__ = "2017-2023, CNES"
+__copyright__ = "2017-2024, CNES"
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/S1FileManager.py` & `s1tiling-1.1.0rc1/s1tiling/libs/S1FileManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # =========================================================================
 #   Program:   S1Processor
 #
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   All rights reserved.
+#   Copyright 2017-2024 (c) CNES.
+#   Copyright 2022-2024 (c) CS GROUP France.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -31,100 +33,112 @@
 """ This module contains the S1FileManager class"""
 
 from enum import Enum
 import fnmatch
 from functools import partial
 import glob
 import logging
+import logging.handlers
 import multiprocessing
 import os
 from pathlib import Path
 import re
 import shutil
-import sys
 import tempfile
-from typing import List, Optional
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
-from requests.exceptions import ReadTimeout
-from eodag.api.core         import EODataAccessGateway
+from osgeo import ogr
+from requests.exceptions     import ReadTimeout
+from eodag.api.core          import EODataAccessGateway
+from eodag.api.product       import EOProduct
 from eodag.api.search_result import SearchResult
-from eodag.utils.logging    import setup_logging
-from eodag.utils.exceptions import NotAvailableError
-from eodag.utils            import get_geometry_from_various
+from eodag.utils             import get_geometry_from_various
+from eodag.utils.exceptions  import NotAvailableError
+from eodag.utils.logging     import setup_logging
 try:
     from shapely.errors import TopologicalError
 except ImportError:
     from shapely.geos   import TopologicalError
 
 import numpy as np
 
-from s1tiling.libs import exits
-from .Utils import get_shape, list_dirs, Layer, extract_product_start_time, get_orbit_direction, get_relative_orbit
+from s1tiling.libs      import exceptions
+from .Utils             import (
+    Layer,
+    extract_product_start_time, find_dem_intersecting_poly, get_mgrs_tile_geometry_by_name,
+    get_orbit_direction, get_relative_orbit, get_shape, list_dirs,
+)
 from .S1DateAcquisition import S1DateAcquisition
-from .otbpipeline import mp_worker_config
-from .outcome import DownloadOutcome
+from .configuration     import (
+        Configuration, dname_fmt_lia_product, dname_fmt_mask, dname_fmt_tiled, dname_fmt_filtered, fname_fmt_concatenation, fname_fmt_filtered
+)
+from .otbpipeline       import mp_worker_config
+from .outcome           import DownloadOutcome
 
 setup_logging(verbose=1)
 
 logger = logging.getLogger('s1tiling.filemanager')
 
 
 # Default configuration value for people using S1Tiling API functions s1_process, and s1_process_lia.
 EODAG_DEFAULT_DOWNLOAD_WAIT         = 2   #: If download fails, wait time in minutes between two download tries
 EODAG_DEFAULT_DOWNLOAD_TIMEOUT      = 20  #: If download fails, maximum time in minutes before stop retrying to download
-EODAG_DEFAULT_SEARCH_MAX_RETRIES    =  5  #: If search fails on timeout, number of retries attempted 
+EODAG_DEFAULT_SEARCH_MAX_RETRIES    = 5   #: If search fails on timeout, number of retries attempted
 EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE = 20  #: Number of items returns by each page search
 
+
 class WorkspaceKinds(Enum):
     """
     Enum used to list the kinds of "workspaces" needed.
     A workspace is a directory where products will be stored.
 
     :todo: Use a more flexible and OCP (Open-Close Principle) compliant solution.
         Indeed At this moment, only two kinds of workspaces are supported.
     """
     TILE   = 1
     LIA    = 2
     FILTER = 3
+    MASK   = 4
 
 
-def product_property(prod, key, default=None):
+def product_property(prod: EOProduct, key: str, default=None):
     """
     Returns the required (EODAG) product property, or default in the property isn't found.
     """
     res = prod.properties.get(key, default)
     return res
 
 
-def product_cover(product, geometry):
+def product_cover(product: EOProduct, geometry: Dict[str, float]) -> float:
     """
     Compute the coverage of the intersection of the product and the target geometry
     relativelly to the target geometry.
     Return a percentage in the range [0..100].
 
     This function has been extracted and adapted from
     :func:`eodag.plugins.crunch.filter_overlap.FilterOverlap.proceed`, which is
     under the Apache Licence 2.0.
 
     Unlike the original function, the actual filtering is done differenty and we
     only need the computed coverage. Also, we are not interrested in the
     coverage of the intersection relativelly to the input product.
     """
     search_geom = get_geometry_from_various(geometry=geometry)
+    assert search_geom, "Let's suppose eodag returns a geometry"
     if product.search_intersection:
         intersection = product.search_intersection
         product_geometry = product.geometry
     elif product.geometry.is_valid:
         product_geometry = product.geometry
         intersection = search_geom.intersection(product_geometry)
     else:
         logger.debug(
                 "Trying our best to deal with invalid geometry on product: %r",
                 product,
-                )
+        )
         product_geometry = product.geometry.buffer(0)
         try:
             intersection = search_geom.intersection(product_geometry)
         except TopologicalError:
             logger.debug("Product geometry still invalid. Force its acceptance")
         return 100
 
@@ -143,16 +157,21 @@
 #             logger.warning("%s is corrupted. This file will be removed", file_it.path)
 #         try:
 #             os.remove(file_it.path)
 #         except OSError:
 #             pass
 
 
-def does_final_product_need_to_be_generated_for(
-        product, tile_name, polarizations, cfg, s2images):
+def does_final_product_need_to_be_generated_for(  # pylint: disable=too-many-locals
+    product:       EOProduct,
+    tile_name:     str,
+    polarizations: List[str],
+    cfg:           Configuration,
+    s2images:      List[str]
+) -> bool:
     """
     Tells whether finals products associated to a tile needs to be generated.
 
     :param product:       S1 images that are available for download through EODAG
     :param tile_name:     Name of the S2 tile
     :param polarizations: Requested polarizations as per configuration.
     :param s2images:      List of already globbed S2 images files
@@ -162,44 +181,48 @@
     """
     logger.debug('>  Searching whether %s final products have already been generated (in polarizations: %s)',
                  product, polarizations)
     if len(s2images) == 0:
         return True
     # e.g. id=S1A_IW_GRDH_1SDV_20200108T044150_20200108T044215_030704_038506_C7F5,
     prod_re = re.compile(r'(S1.)_IW_...._...._(\d{8})T\d{6}.*')
-    sat, start = prod_re.match(product.as_dict()['id']).groups()
+    pid = product.as_dict()['id']
+    match = prod_re.match(pid)
+    if not match:
+        raise AssertionError(f"Unexpected name for S1 Product: {pid} doesn't match expected pattern")
+    sat, start = match.groups()
     keys = {
-            'flying_unit_code'  : sat.lower(),
-            'tile_name'         : tile_name,
-            'acquisition_stamp' : f'{start}t??????',
-            'orbit_direction'   : '*',
-            'orbit'             : '*',
-            'calibration_type'  : cfg.calibration_type,
-            }
-    fname_fmt_concatenation = cfg.fname_fmt_concatenation
-    fname_fmt_filtered      = cfg.fname_fmt_filtered
+        'flying_unit_code'  : sat.lower(),
+        'tile_name'         : tile_name,
+        'acquisition_stamp' : f'{start}t??????',
+        'orbit_direction'   : '*',
+        'orbit'             : '*',
+        'calibration_type'  : cfg.calibration_type,
+    }
+    fname_fmt_4concatenation = fname_fmt_concatenation(cfg)
+    fname_fmt_4filtered      = fname_fmt_filtered(cfg)
     for polarisation in polarizations:
         # e.g. s1a_{tilename}_{polarization}_DES_007_20200108txxxxxx.tif
         # We should use the `Processing.fname_fmt.concatenation` option
-        pat          = fname_fmt_concatenation.format(**keys, polarisation=polarisation)
-        pat_filtered = fname_fmt_filtered.format(**keys, polarisation=polarisation)
+        pat          = fname_fmt_4concatenation.format(**keys, polarisation=polarisation)
+        pat_filtered = fname_fmt_4filtered.format(**keys, polarisation=polarisation)
         found_s2 = fnmatch.filter(s2images, pat)
         found_filt = fnmatch.filter(s2images, pat_filtered)
         found = found_s2 or found_filt
         logger.debug('   searching w/ %s and %s ==> Found: %s', pat, pat_filtered, found)
         if not found:
             return True
         # FIXME:
         # - if found_s2 and not found_filt => we have everything that is needed
         # - if found_filt and not found_s2 => we have prevent the required S1 products from being downloaded
         #                                     if the S2 product is required
     return False
 
 
-def filter_images_or_ortho(kind, all_images):
+def filter_images_or_ortho(kind, all_images: List[str]) -> List[str]:
     """
     Analyses the existing orthorectified image files, or the ortho ready ones, for the input
     raster provided.
     This will be used to register the image raster to transform.
     """
     pattern = "*" + kind + "*-???.tiff"
     ortho_pattern = "*" + kind + "*-???_OrthoReady.tiff"
@@ -210,39 +233,46 @@
     if not images:
         images = [f.replace("_OrthoReady.tiff", ".tiff")
                 for f in fnmatch.filter(all_images, ortho_pattern)]
         logger.debug("    %s images from Ortho: %s", kind, images)
     return images
 
 
-def _filter_images_providing_enough_cover_by_pair(
-        products, target_cover, ident, get_cover, get_orbit):
+def _filter_images_providing_enough_cover_by_pair(  # pylint: disable=too-many-locals
+    products:     Union[List[EOProduct], List[Dict]],  # EOProduct or content_info
+    target_cover: float,
+    ident:        Callable[[Union[EOProduct, Dict]], str],
+    get_cover:    Callable[[Union[EOProduct, Dict]], float],
+    get_orbit:    Callable[[Union[EOProduct, Dict]], int],
+) -> Union[List[EOProduct], List[Dict]]:
     """
     Associate products of the same date and orbit into pairs (at most),
     to compute the total coverage of the target zone.
     If the total coverage is inferior to the target coverage, the products
     are filtered out.
 
     This function can be used on product information returned by EODAG as well
     as product information extracted from existing files. It's acheived thanks
     to the `ident`, `get_cover` and `get_orbit` variation points.
     """
     if not products or not target_cover:
         return products
     prod_re = re.compile(r'S1._IW_...._...._(\d{8})T\d{6}_\d{8}T\d{6}.*')
-    kept_products = []
-    date_grouped_products = {}
+    kept_products : Union[List[EOProduct], List[Dict]] = []
+    date_grouped_products : Dict[str, Dict[float, EOProduct]] = {}
     logger.debug('Checking coverage for each product')
     for p in products:
-        id    = ident(p)
-        date  = prod_re.match(id).groups()[0]
+        pid   = ident(p)
+        match = prod_re.match(pid)
+        assert match
+        date  = match.groups()[0]
         cover = get_cover(p)
         ron   = get_orbit(p)
         dron  = f'{date}#{ron:03}'
-        logger.debug('* @ %s, %s%% coverage for %s', dron, round(cover, 2), id)
+        logger.debug('* @ %s, %s%% coverage for %s', dron, round(cover, 2), pid)
         if dron not in date_grouped_products:
             date_grouped_products[dron] = {}
         date_grouped_products[dron].update({cover : p})
 
     logger.debug('Checking coverage for each date (and # relative orbit number)')
     for dron, cov_prod in date_grouped_products.items():
         covers         = cov_prod.keys()
@@ -254,15 +284,19 @@
                     dron, str_cov_to_sum, cov_sum, target_cover,
                     [ident(p) for p in cov_prod.values()])
         else:
             kept_products.extend(cov_prod.values())
     return kept_products
 
 
-def _keep_products_with_enough_coverage(content_info, target_cover, current_tile):
+def _keep_products_with_enough_coverage(
+    content_info: List[Dict],
+    target_cover: float,
+    current_tile: ogr.Feature,
+) -> List[Dict]:
     """
     Helper function that filters the products (/pairs of products) that provide
     enough coverage.
     It's meant to be used on product information extracted from existing files.
     """
     tile_footprint = current_tile.GetGeometryRef()
     area_polygon = tile_footprint.GetGeometryRef(0)
@@ -288,46 +322,56 @@
             content_info_with_intersection.append(ci)
 
     return _filter_images_providing_enough_cover_by_pair(
             content_info_with_intersection, target_cover,
             ident=lambda ci: ci['product'].name,
             get_cover=lambda ci: ci['coverage'],
             get_orbit=lambda ci: ci['relative_orbit'],
-            )
+    )
 
 
-def _discard_small_redundant(products, ident=None):
+def _discard_small_redundant(
+    products: Union[List[EOProduct], List[os.DirEntry]],
+    ident:    Callable[[Union[EOProduct, os.DirEntry]], str],
+) -> Union[List[EOProduct], List[os.DirEntry]]:
     """
     Sometimes there are several S1 product with the same start date, but a different end-date.
     Let's discard the smallest products
     """
     if not products:
         return products
-    if not ident:
-        ident = lambda name: name
+    assert ident is not None, "Please call with a ident parameter!"
     prod_re = re.compile(r'S1._IW_...._...._(\d{8}T\d{6})_(\d{8}T\d{6}).*')
 
-    ordered_products = sorted(products, key=lambda p: ident(p))
+    ordered_products = sorted(products, key=ident)
     # logger.debug("all products before clean: %s", ordered_products)
     res = [ordered_products[0]]
-    last, _ = prod_re.match(ident(res[0])).groups()
+    match = prod_re.match(ident(res[0]))
+    assert match
+    last, _ = match.groups()
     for product in ordered_products[1:]:
-        start, __unused = prod_re.match(ident(product)).groups()
+        match = prod_re.match(ident(product))
+        assert match
+        start, _ = match.groups()
         if last == start:
             # We can suppose the new end date to be >
             # => let's replace
             logger.warning('Discarding %s that is smallest than %s', res[-1], product)
             res[-1] = product
         else:
             res.append(product)
             last = start
     return res
 
 
-def _keep_requested_orbits(content_info, rq_orbit_direction, rq_relative_orbit_list):
+def _keep_requested_orbits(
+    content_info:           List[Dict],
+    rq_orbit_direction:     Optional[str],
+    rq_relative_orbit_list: List[int],
+) -> List[Dict]:
     """
     Takes care of discarding products that don't match the requested orbit
     specification.
 
     Note: Beware that specifications could be contradictory and end up
     discarding everything.
     """
@@ -349,15 +393,19 @@
             if orbit not in rq_relative_orbit_list:
                 logger.debug('Discard %s as its orbit (%s) differs from the requested ones %s',
                         p.name, orbit, rq_relative_orbit_list)
                 continue
         kept_products.append(ci)
     return kept_products
 
-def _keep_requested_platforms(content_info, rq_platform_list):
+
+def _keep_requested_platforms(
+    content_info: List[Dict],
+    rq_platform_list: List[str]
+) -> List[Dict]:
     """
     Takes care of discarding products that don't match the requested platform specification.
 
     Note: Beware that specifications could be contradictory and end up discarding everything.
     """
     if not rq_platform_list:
         return content_info
@@ -372,88 +420,109 @@
                 logger.debug('Discard %s as its platform (%s) differs from the requested ones %s',
                         p.name, platform, rq_platform_list)
                 continue
         kept_products.append(ci)
     return kept_products
 
 
-def _download_and_extract_one_product(dag, raw_directory, dl_wait, dl_timeout, product) -> DownloadOutcome:
+def _download_and_extract_one_product(
+    dag:           EODataAccessGateway,
+    raw_directory: str,
+    dl_wait:       int,
+    dl_timeout:    int,
+    product:       EOProduct
+) -> DownloadOutcome[str, EOProduct]:
     """
     Takes care of downloading exactly one remote product and unzipping it,
     if required.
 
     Some products are already unzipped on the fly by eodag.
     """
     logging.info("Starting download of %s...", product)
     ok_msg = f"Successful download (and extraction) of {product}"  # because eodag'll clear product
-    file = os.path.join(raw_directory, product.as_dict()['id']) + '.zip'
-    path: DownloadOutcome
+    prod_id = product.as_dict()['id']
+    zip_file = os.path.join(raw_directory, prod_id) + '.zip'
+    path: DownloadOutcome[str, EOProduct]
     try:
         path = DownloadOutcome(
                 dag.download(
-                    product,           # EODAG will clear this variable
-                    extract=True,      # Let's eodag do the job
-                    wait=dl_wait,      # Wait time in minutes between two download tries
-                    timeout=dl_timeout # Maximum time in mins before stop retrying to download (default=20’)
+                    product,            # EODAG will clear this variable
+                    extract=True,       # Let's eodag do the job
+                    wait=dl_wait,       # Wait time in minutes between two download tries
+                    timeout=dl_timeout  # Maximum time in mins before stop retrying to download (default=20’)
                 ),
                 product)
         logging.debug(ok_msg)
-        if os.path.exists(file) :
+        if os.path.exists(zip_file) :
             try:
-                logger.debug('Removing downloaded ZIP: %s', file)
-                os.remove(file)
+                logger.debug('Removing downloaded ZIP: %s', zip_file)
+                os.remove(zip_file)
             except OSError:
                 pass
+        # eodag may say the product is correctly downloaded while it failed to do so
+        # => let's do a quick sanity check
+        manifest = os.path.join(raw_directory, prod_id, f'{prod_id}.SAFE', 'manifest.safe')
+        if not os.path.exists(manifest):
+            logger.error('Actually download of %s failed, the expected manifest could not be found in the product (%s)', prod_id, manifest)
+            e = exceptions.CorruptedDataSAFEError(prod_id, f"no manifest file named {manifest!r} found")
+            path = DownloadOutcome(e, product)
     except BaseException as e:  # pylint: disable=broad-except
         logger.warning('%s', e)  # EODAG error message is good and precise enough, just use it!
         # logger.error('Product is %s', product_property(product, 'storageStatus', 'online?'))
         logger.debug('Exception type is: %s', e.__class__.__name__)
         ## ERROR - Product is OFFLINE
         ## ERROR - Exception type is: NotAvailableError
         # logger.error('======================')
         # logger.exception(e)
         ## Traceback (most recent call last):
         ##   File "s1tiling/libs/S1FileManager.py", line 350, in _download_and_extract_one_product
-        ##     path = Outcome(dag.download(
+        ##     path = DownloadOutcome(dag.download(
         ##   File "site-packages/eodag/api/core.py", line 1487, in download
         ##     path = product.download(
         ##   File "site-packages/eodag/api/product/_product.py", line 288, in download
         ##     fs_path = self.downloader.download(
         ##   File "site-packages/eodag/plugins/download/http.py", line 269, in download
         ##     raise NotAvailableError(
-        ## eodag.utils.exceptions.NotAvailableError: S1A_IW_GRDH_1SDV_20200401T044214_20200401T044239_031929_03AFBC_0C9E is not available (OFFLINE) and could not be downloaded, timeout reached
+        ## eodag.utils.exceptions.NotAvailableError: S1A_IW_GRDH_1SDV_20200401T044214_20200401T044239_031929_03AFBC_0C9E
+        ##                                           is not available (OFFLINE) and could not be downloaded, timeout reached
 
         path = DownloadOutcome(e, product)
 
     return path
 
 
-def _parallel_download_and_extraction_of_products(
-        dag, raw_directory, products, nb_procs: int, tile_name: str, dl_wait: int, dl_timeout: int
+def _parallel_download_and_extraction_of_products(  # pylint: disable=too-many-arguments, too-many-locals
+    dag:           EODataAccessGateway,
+    raw_directory: str,
+    products:      List[EOProduct],
+    nb_procs:      int,
+    tile_name:     str,
+    dl_wait:       int,
+    dl_timeout:    int,
 ) -> List[DownloadOutcome]:
     """
     Takes care of downloading exactly all remote products and unzipping them,
     if required, in parallel.
 
     Returns :class:`DownloadOutcome` of :class:`EOProduct` or Exception.
     """
     nb_products = len(products)
     paths = []
-    log_queue = multiprocessing.Queue()
+    log_queue : multiprocessing.Queue = multiprocessing.Queue()
     log_queue_listener = logging.handlers.QueueListener(log_queue)
     dl_work = partial(_download_and_extract_one_product, dag, raw_directory, dl_wait, dl_timeout)
     with multiprocessing.Pool(nb_procs, mp_worker_config, [log_queue]) as pool:
         log_queue_listener.start()
         try:
             # In case timeout happens, we try again if and only if we have been able to
             # download other products after the timeout.
             # -> IOW, downloading instability justifies trying again.
             # /> On the contrary, on a complete network failure, we should not try again and again...
             while len(products) > 0:
-                products_in_timeout = []
+                products_in_timeout : List[EOProduct] = []
                 nb_successes_since_timeout = 0
                 for count, result in enumerate(pool.imap_unordered(dl_work, products), 1):
                     # logger.debug('DL -> %s', result)
                     if result:
                         logger.info("%s correctly downloaded", result.value())
                         logger.info(' --> Downloading products for %s... %s%%', tile_name, count * 100. / nb_products)
                         paths.append(result)
@@ -490,38 +559,39 @@
 
     Then, this list of all known products is filtered according to the target S2
     tile to retain only the S1 products that provide enough coverage.
 
     Eventually, the S1 products are scanned for the raster images of
     polarisation compatible with the requested one(s).
     """
-    def __init__(self, cfg) -> None:
+
+    tiff_pattern     = "measurement/*.tiff"
+    manifest_pattern = "manifest.safe"
+
+    def __init__(self, cfg: Configuration) -> None:
         # Configuration
         self.cfg              = cfg
         self.__searched_items_per_page = getattr(cfg, 'searched_items_per_page', EODAG_DEFAULT_SEARCH_ITEMS_PER_PAGE)
         self.__nb_max_search_retries   = getattr(cfg, 'nb_max_search_retries',   EODAG_DEFAULT_SEARCH_MAX_RETRIES)
         self.__dl_wait                 = getattr(cfg, 'dl_wait',                 EODAG_DEFAULT_DOWNLOAD_WAIT)
         self.__dl_timeout              = getattr(cfg, 'dl_timeout',              EODAG_DEFAULT_DOWNLOAD_TIMEOUT)
 
-        self.raw_raster_list  = []
+        self.raw_raster_list  : List[S1DateAcquisition] = []
         self.nb_images        = 0
 
         # Failures related to download (e.g. missing products)
         self.__search_failures                = 0
-        self.__download_failures              = []
-        self.__failed_S1_downloads_by_S2_uid  = {}  # by S2 unique id: date + rel_orbit
-        self.__skipped_S2_products            = []
+        self.__download_failures              : List[DownloadOutcome]            = []
+        self.__failed_S1_downloads_by_S2_uid  : Dict[str, List[DownloadOutcome]] = {}  # by S2 unique id: date + rel_orbit
+        self.__skipped_S2_products            : List[str]                        = []
 
-        self.__tmpsrtmdir     = None
-        self.__caching_option = cfg.cache_srtm_by
+        self.__tmpdemdir      : Optional[tempfile.TemporaryDirectory] = None
+        self.__caching_option = cfg.cache_dem_by
         assert self.__caching_option in ['copy', 'symlink']
 
-        self.tiff_pattern     = "measurement/*.tiff"
-        self.manifest_pattern = "manifest.safe"
-
         self._ensure_workspaces_exist()
         self.processed_filenames = self.get_processed_filenames()
 
         self.first_date = cfg.first_date
         self.last_date  = cfg.last_date
         self._refresh_s1_product_list()
         if self.cfg.download:
@@ -534,129 +604,164 @@
                 if hasattr(self._dag.providers_config[provider], 'download'):
                     self._dag.providers_config[provider].download.update(
                             {'outputs_prefix': dest_dir})
                     logger.debug(' - for %s', provider)
                 else:
                     logger.debug(' - NOT for %s', provider)
 
-            self.roi_by_tiles = self.cfg.ROI_by_tiles
+            self.roi_by_tiles = self.cfg.roi_by_tiles
 
-    def __enter__(self):
+    def __enter__(self) -> "S1FileManager":
         """
         Turn the S1FileManager into a context manager, context acquisition function
         """
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         """
         Turn the S1FileManager into a context manager, cleanup function
         """
-        if self.__tmpsrtmdir:
-            logger.debug('Cleaning temporary SRTM diretory (%s)', self.__tmpsrtmdir)
-            self.__tmpsrtmdir.cleanup()
-            self.__tmpsrtmdir = None
+        if self.__tmpdemdir:
+            logger.debug('Cleaning temporary DEM diretory (%s)', self.__tmpdemdir)
+            self.__tmpdemdir.cleanup()
+            self.__tmpdemdir = None
         return False
 
-    def get_skipped_S2_products(self):
+    def get_skipped_S2_products(self) -> List[str]:
         """
         List of S2 products whose production will be skipped because of a
         download failure of a S1 product.
         """
         return self.__skipped_S2_products
 
     def get_search_failures(self) -> int:
         """Returns the number of times querying matching products failed"""
         return self.__search_failures
 
-    def get_download_failures(self):
+    def get_download_failures(self) -> List[DownloadOutcome]:
+        """
+        Returns the list of download failures as a list of :class:DownloadOutcome`
+        """
         return self.__download_failures
 
-    def get_download_timeouts(self):
+    def get_download_timeouts(self) -> List[DownloadOutcome]:
+        """
+        Returns the list of download timeours as a list of :class:DownloadOutcome`
+        """
         return list(filter(lambda f: isinstance(f.error(), NotAvailableError), self.__download_failures))
 
-    def _ensure_workspaces_exist(self):
+    def _ensure_workspaces_exist(self) -> None:
         """
         Makes sure the directories used for :
         - raw data
         - output data
         - and temporary data
         all exist
         """
         for path in [self.cfg.raw_directory, self.cfg.tmpdir, self.cfg.output_preprocess]:
             if not os.path.isdir(path):
                 os.makedirs(path, exist_ok=True)
 
-    def ensure_tile_workspaces_exist(self, tile_name, required_workspaces):
+    def ensure_tile_workspaces_exist(self, tile_name: str, required_workspaces: List[WorkspaceKinds]) -> None:
         """
         Makes sure the directories used for :
         - output data/{tile},
         - temporary data/S2/{tile}
         - and LIA data (if required)
         all exist
         """
+        directories = {
+                'out_dir': self.cfg.output_preprocess,
+                'tmp_dir': self.cfg.tmpdir,
+                'lia_dir': self.cfg.lia_directory,
+        }
+
         working_directory = os.path.join(self.cfg.tmpdir, 'S2', tile_name)
         os.makedirs(working_directory, exist_ok=True)
 
         if WorkspaceKinds.TILE in required_workspaces:
-            out_dir = os.path.join(self.cfg.output_preprocess, tile_name)
-            os.makedirs(out_dir, exist_ok=True)
+            wdir = dname_fmt_tiled(self.cfg).format(**directories, tile_name=tile_name)
+            os.makedirs(wdir, exist_ok=True)
+
+        if WorkspaceKinds.MASK in required_workspaces:
+            wdir = dname_fmt_mask(self.cfg).format(**directories, tile_name=tile_name)
+            os.makedirs(wdir, exist_ok=True)
 
         if WorkspaceKinds.FILTER in required_workspaces:
-            filter_directory = os.path.join(self.cfg.output_preprocess, 'filtered', tile_name)
-            os.makedirs(filter_directory, exist_ok=True)
+            wdir = dname_fmt_filtered(self.cfg).format(**directories, tile_name=tile_name)
+            os.makedirs(wdir, exist_ok=True)
 
         # if self.cfg.calibration_type == 'normlim':
         if WorkspaceKinds.LIA in required_workspaces:
-            lia_directory = self.cfg.lia_directory
-            os.makedirs(lia_directory, exist_ok=True)
+            wdir = dname_fmt_lia_product(self.cfg).format(**directories, tile_name=tile_name)
+            os.makedirs(wdir, exist_ok=True)
 
-    def tmpsrtmdir(self, srtm_tiles_id, srtm_suffix='.hgt'):
+    def tmpdemdir(self, dem_tile_infos: Dict, dem_filename_format: str, geoid_file: str) -> str:
         """
-        Generate the temporary directory for SRTM tiles on the fly,
-        and either populate it with symbolic links to the actual SRTM
-        tiles, or copies of the actual SRTM tiles.
+        Generate the temporary directory for DEM tiles on the fly,
+        and either populate it with symbolic links to the actual DEM
+        tiles, or copies of the actual DEM tiles.
         """
         assert self.__caching_option in ['copy', 'symlink']
-        if not self.__tmpsrtmdir:
-            # copy all needed SRTM file in a temp directory for orthorectification processing
-            self.__tmpsrtmdir = tempfile.TemporaryDirectory(dir=self.cfg.tmpdir)
-            logger.debug('Create temporary SRTM diretory (%s) for needed tiles %s', self.__tmpsrtmdir.name, srtm_tiles_id)
-            assert Path(self.__tmpsrtmdir.name).is_dir()
-            for srtm_tile in srtm_tiles_id:
-                srtm_tile_filepath=Path(self.cfg.srtm, srtm_tile + srtm_suffix)
-                srtm_tile_filelink=Path(self.__tmpsrtmdir.name, srtm_tile + srtm_suffix)
-                if self.__caching_option == 'symlink':
-                    logger.debug('- ln -s %s <-- %s', srtm_tile_filepath, srtm_tile_filelink)
-                    srtm_tile_filelink.symlink_to(srtm_tile_filepath)
-                else:
-                    logger.debug('- cp %s <-- %s', srtm_tile_filepath, srtm_tile_filelink)
-                    shutil.copy2(srtm_tile_filepath, srtm_tile_filelink)
+        if not self.__tmpdemdir:
+            # copy all needed DEM & geoid files in a temp directory for orthorectification processing
+            self.__tmpdemdir = tempfile.TemporaryDirectory(dir=self.cfg.tmpdir)
+            logger.debug('Create temporary DEM diretory (%s) for needed tiles %s', self.__tmpdemdir.name, list(dem_tile_infos.keys()))
+            assert Path(self.__tmpdemdir.name).is_dir()
+            def do_symlink(src: Union[Path, str], dst: Path):
+                logger.debug('- ln -s %s <-- %s', src, dst)
+                dst.symlink_to(src)
+            def do_copy(src: Union[Path, str], dst: Path):
+                logger.debug('- cp %s --> %s', src, dst)
+                shutil.copy2(src, dst)
+            do_localize = do_symlink if self.__caching_option == 'symlink' else do_copy
+
+            for _, dem_tile_info in dem_tile_infos.items():
+                dem_file          = dem_filename_format.format_map(dem_tile_info)
+                dem_tile_filepath = Path(self.cfg.dem, dem_file)
+                dem_tile_filelink = Path(self.__tmpdemdir.name, os.path.basename(dem_file))  # for copernicus dem
+                dem_tile_filelink.parent.mkdir(parents=True, exist_ok=True)
+                do_localize(dem_tile_filepath, dem_tile_filelink)
+            # + copy/link geoid
+            geoid_filelink = Path(self.cfg.tmpdir, 'geoid', os.path.basename(geoid_file))
+            if not geoid_filelink.exists():
+                geoid_filelink.parent.mkdir(parents=True, exist_ok=True)
+                do_localize(geoid_file, geoid_filelink)
+                # in case there is an associated file like (egm96.grd.hdr), copy/symlink it as well
+                if os.path.isfile(with_hdr := f"{geoid_file}.hdr"):
+                    do_localize(with_hdr, geoid_filelink.with_suffix(geoid_filelink.suffix+'.hdr'))
 
-        return self.__tmpsrtmdir.name
+        return self.__tmpdemdir.name
 
-    def keep_X_latest_S1_files(self, threshold, tile_name):
+    def keep_X_latest_S1_files(self, threshold: int, tile_name: str) -> None:
         """
         Makes sure there is no more than `threshold`  S1 SAFEs in the raw directory.
         Oldest ones will be removed.
         """
         safefile_list = sorted(
                 glob.glob(os.path.join(self.cfg.raw_directory, "*")),
                 key=os.path.getctime)
         if len(safefile_list) > threshold:
             for safe in safefile_list[ : len(safefile_list) - threshold]:
                 logger.debug("Remove old SAFE: %s", os.path.basename(safe))
                 shutil.rmtree(safe, ignore_errors=True)
             self._refresh_s1_product_list()  # TODO: decremental update
             self._update_s1_img_list_for(tile_name)
 
-    def _search_products(
-            self, dag: EODataAccessGateway,
-            extent, first_date, last_date,
-            platform_list, orbit_direction, relative_orbit_list, polarization,
-            dryrun
+    def _search_products(  # pylint: disable=too-many-arguments, too-many-locals
+        self,
+        dag:                            EODataAccessGateway,
+        extent:                         Dict[str, float],
+        first_date:                     str,
+        last_date:                      str,
+        platform_list:                  List[str],
+        orbit_direction:                Optional[str],
+        relative_orbit_list:            List[int],
+        polarization:                   str,
+        dryrun:                         bool,
     ) -> SearchResult:
         """
         Process with the call to eodag search.
         """
         product_type = 'S1_SAR_GRD'
         products = SearchResult(None)
         page = 1
@@ -696,16 +801,16 @@
             else:
                 assert isinstance(timeout, ReadTimeout)
                 raise RuntimeError(f"Product search has timeout'd {self.__nb_max_search_retries} times") from timeout
 
             if len(page_products) < self.__searched_items_per_page:
                 break
         logger.debug("%s remote S1 products found: %s", len(products), products)
-        ##for p in products:
-        ##    logger.debug("%s --> %s -- %s", p, p.provider, p.properties)
+        ## for p in products:
+        ##     logger.debug("%s --> %s -- %s", p, p.provider, p.properties)
 
         # Filter relative_orbits -- if it could not be done earlier in the search() request.
         if len(relative_orbit_list) > 1:
             filtered_products = SearchResult(None)
             for rel_orbit in relative_orbit_list:
                 filtered_products.extend(products.filter_property(relativeOrbitNumber=rel_orbit))
             products = filtered_products
@@ -735,146 +840,180 @@
         if orbit_filter_log:
             extra_filters.append(orbit_filter_log)
         logger.info("%s remote S1 product(s) found and filtered (%s): %s", len(products),
                     " && ".join(extra_filters), products)
 
         return products
 
-    def _filter_products(self, products, extent, tile_out_dir, tile_name, polarization, cover):
+    def _filter_products(  # pylint: disable=too-many-arguments
+        self,
+        products:     List[EOProduct],
+        extent:       Dict[str, float],
+        tile_out_dir: str,
+        tile_name:    str,
+        polarization: str,
+        cover:        float
+    ) -> List[EOProduct]:
         """
         Filter products to download according to their polarization and coverage
         """
         if not products:  # no need to continue
             return []
 
         # Filter out products that either:
         # - are overlapped by bigger ones
-        #   Sometimes there are several S1 product with the same start
-        #   date, but a different end-date.  Let's discard the
-        #   smallest products
-        products = _discard_small_redundant(products, ident=lambda p: p.as_dict()['id'])
+        #   Sometimes there are several S1 product with the same start date, but a different end-date.
+        #   Let's discard the smallest products
+        def ident(p: EOProduct) -> str:
+            # assert isinstance(p, EOProduct), f"Expecting a EOProduct, got: {type(p)!r}"
+            return p.as_dict()['id']
+
+        products = _discard_small_redundant(products, ident=ident)
         logger.debug("%s remote S1 product(s) left after discarding smallest redundant ones: %s", len(products), products)
         # Filter cover
         if cover:
             products = _filter_images_providing_enough_cover_by_pair(
                     products, cover,
-                    ident=lambda p: p.as_dict()['id'],
+                    ident=ident,
                     get_cover=lambda p: product_cover(p, extent),
                     get_orbit=lambda p: product_property(p, 'relativeOrbitNumber')
                     )
             # products = products.filter_overlap(
             #         minimum_overlap=cover, geometry=extent)
             logger.debug("%s remote S1 product(s) found and filtered (cover >= %s): %s", len(products), cover, products)
 
-
         # - already exist in the "cache"
         # logger.debug('Check products against the cache: %s', self.product_list)
         # self._refresh_s1_product_list()  # No need: as it has been done at startup, and after download
                                            # And let's suppose nobody deletd files
                                            # manually!
-        products = [p for p in products
-                if p.as_dict()['id'] not in self._product_list.keys()
-                ]
+        products = list(filter(lambda p: ident(p) not in self._product_list, products))
+        # products = [p for p in products if ident(p) not in self._product_list]
         # logger.debug('Products cache: %s', self._product_list.keys())
         logger.debug("%s remote S1 product(s) are not yet in the cache: %s", len(products), products)
         if not products:  # no need to continue
             return []
         # - or for which we found matching dates
         #   Beware: a matching VV while the VH doesn't exist and is present in the
         #   remote product shall trigger the download of the product.
         #   TODO: We should actually inject the expected filenames into the task graph
         #   generator in order to download what is stricly necessary and nothing more
         polarizations = polarization.lower().split(' ')
         s2images_pat = f's1?_{tile_name}_*.tif'
         logger.debug('Search %s for %s on disk in %s(/filtered)/%s', s2images_pat, polarizations, tile_out_dir, tile_name)
-        def glob1(pat, *paths):
+
+        def glob1(pat, *paths) -> List[str]:
             pathname = glob.escape(os.path.join(*paths))
             return [os.path.basename(p) for p in glob.glob(os.path.join(pathname, pat))]
-        s2images = glob1(s2images_pat, tile_out_dir, tile_name) + glob1(s2images_pat, tile_out_dir, "filtered", tile_name)
+        dname_options = { 'tile_name': tile_name, 'out_dir': tile_out_dir, }
+        s2images = glob1(
+                s2images_pat, dname_fmt_tiled(self.cfg).format_map(dname_options)
+        ) + glob1(
+                s2images_pat, dname_fmt_filtered(self.cfg).format_map(dname_options)
+        )
         logger.debug(' => S2 products found on %s: %s', tile_name, s2images)
         products = [p for p in products
                 if does_final_product_need_to_be_generated_for(
                     p, tile_name, polarizations, self.cfg, s2images)
                 ]
         return products
 
-    def _download(
-            self, dag: EODataAccessGateway,
-            lonmin, lonmax, latmin, latmax,
-            first_date, last_date,
-            tile_out_dir, tile_name: str,
-            platform_list, orbit_direction, relative_orbit_list, polarization, cover,
-            dryrun
+    def _download(  # pylint: disable=too-many-arguments, too-many-locals
+        self,
+        dag:                     EODataAccessGateway,
+        lonmin:                  float,
+        lonmax:                  float,
+        latmin:                  float,
+        latmax:                  float,
+        first_date:              str,
+        last_date:               str,
+        tile_out_dir:            str,
+        tile_name:               str,
+        platform_list:           List[str],
+        orbit_direction:         Optional[str],
+        relative_orbit_list:     List[int],
+        polarization:            str,
+        cover:                   float,
+        dryrun:                  bool,
     ) -> List[DownloadOutcome]:
         """
         Process with the call to eodag search + filter + download.
 
         :rtype: :class:`DownloadOutcome` of :class:`EOProduct` or Exception.
         :raises RuntimeError: If the search fails
         """
         extent = {
                 'lonmin': lonmin,
                 'lonmax': lonmax,
                 'latmin': latmin,
                 'latmax': latmax
                 }
         try:
-            products = self._search_products(
+            sproducts = self._search_products(
                     dag, extent,
                     first_date, last_date, platform_list, orbit_direction, relative_orbit_list,
                     polarization, dryrun)
         except Exception as e:
             self.__search_failures += 1
             raise RuntimeError(f"Cannot request products for tile {tile_name} on data provider: {e}") from e
 
-        products = self._filter_products(products, extent, tile_out_dir, tile_name, polarization, cover)
+        products = self._filter_products(list(sproducts), extent, tile_out_dir, tile_name, polarization, cover)
 
         # And finally download all!
         # TODO: register downloading into Dask
         logger.info("%s remote S1 product(s) will be downloaded", len(products))
         for p in products:
             logger.info('- %s: %s %s, [%s]', p,
                     product_property(p, "orbitDirection", ""),
                     product_property(p, "relativeOrbitNumber", ""),
                     product_property(p, "startTimeFromAscendingNode", ""),
                     )
         if not products:  # no need to continue
             # Actually, in that special case we could almost detect there is nothing to do
             return []
         if dryrun:
-            paths = [p.as_dict()['id'] for p in products] # TODO: return real name
+            paths = [p.as_dict()['id'] for p in products]  # TODO: return real name
             logger.info("Remote S1 products would have been saved into %s", paths)
             return paths
 
         paths = _parallel_download_and_extraction_of_products(
                 dag, self.cfg.raw_directory, products, self.cfg.nb_download_processes,
                 tile_name,
                 self.__dl_wait, self.__dl_timeout)
         logger.info("Remote S1 products saved into %s", [p.value() for p in paths if p.has_value()])
         return paths
 
-    def download_images(self, dryrun=False, tiles=None) -> None:
+    def download_images(
+        self,
+        dryrun: bool                = False,
+        tiles:  Optional[List[str]] = None
+    ) -> None:
         """ This method downloads the required images if download is True"""
         if not self.cfg.download:
             logger.info("Using images already downloaded, as per configuration request")
             return
 
+        # TODO: Fix the logic behind these tests and the fonction interface/calls
+        # -> i.e. download_images is always called with tiles=[one_tile_name]
         if tiles:
             tile_list = tiles
         elif "ALL" in self.roi_by_tiles:
             tile_list = self.cfg.tile_list
         else:
             tile_list = re.split(r'\s*,\s*', self.roi_by_tiles)
         logger.debug("Tiles requested to download: %s", tile_list)
 
         self.__failed_S1_downloads_by_S2_uid = {}  # Needs to be reset for each tile!
-        downloaded_products = []
-        layer = Layer(self.cfg.output_grid)
+        downloaded_products: List[DownloadOutcome] = []
+        layer = Layer(self.cfg.output_grid)  # TODO: This could be cached
         for current_tile in layer:
-            tile_name = current_tile.GetField('NAME')
+            name = current_tile.GetField('NAME')
+            if not isinstance(name, str):
+                raise AssertionError(f"Invalid data type for current tile NAME field: {name}. `str` was expected")
+            tile_name : str = name
             if tile_name in tile_list:
                 tile_footprint = current_tile.GetGeometryRef().GetGeometryRef(0)
                 latmin = np.min([p[1] for p in tile_footprint.GetPoints()])
                 latmax = np.max([p[1] for p in tile_footprint.GetPoints()])
                 lonmin = np.min([p[0] for p in tile_footprint.GetPoints()])
                 lonmax = np.max([p[0] for p in tile_footprint.GetPoints()])
                 downloaded_products += self._download(self._dag,
@@ -885,63 +1024,67 @@
                         platform_list=self.cfg.platform_list,
                         orbit_direction=self.cfg.orbit_direction,
                         relative_orbit_list=self.cfg.relative_orbit_list,
                         polarization=self.cfg.polarisation,
                         cover=self.cfg.tile_to_product_overlap_ratio,
                         dryrun=dryrun)
         if downloaded_products:
-            failed_products = list(filter(lambda p: not p, downloaded_products))
+            failed_products: List[DownloadOutcome] = list(filter(lambda p: not p, downloaded_products))
             if failed_products:
                 self._analyse_download_failures(failed_products)
-            success_products = list((p.value() for p in filter(lambda p: p.has_value(), downloaded_products)))
+            success_products = [p.value() for p in filter(lambda p: p.has_value(), downloaded_products)]
             self._refresh_s1_product_list(success_products)  # incremental update
 
-    def _analyse_download_failures(self, failed_products) -> None:
+    def _analyse_download_failures(self, failed_products: List[DownloadOutcome]) -> None:
         """
         Record the download failures and mark S2 products that cannot be generated.
         """
         logger.warning('Some products could not be downloaded. Analysing donwload failures...')
         for fp in failed_products:
             logger.warning('* %s', fp.error())
-            prod  = fp.related_product()
-            day   = '{YYYY}{MM}{DD}'.format_map(extract_product_start_time(prod.as_dict()['id']))
+            prod: EOProduct = fp.related_product()
+            start_time = extract_product_start_time(prod.as_dict()['id'])
+            day   = '{YYYY}{MM}{DD}'.format_map(start_time) if start_time else "????????"
             orbit = product_property(prod, 'relativeOrbitNumber')
             key = f'{day}#{orbit}'
             if key in self.__failed_S1_downloads_by_S2_uid:
                 self.__failed_S1_downloads_by_S2_uid[key].append(fp)
             else:
                 self.__failed_S1_downloads_by_S2_uid[key] = [fp]
             logger.debug('Register product to ignore: %s --> %s', key, self.__failed_S1_downloads_by_S2_uid[key])
         self.__download_failures.extend(failed_products)
 
-    def _refresh_s1_product_list(self, new_products=None):
+    def _refresh_s1_product_list(self, new_products: Optional[List[EOProduct]] = None) -> None:
         """
         Scan all the available products and filter them according to:
         - platform requirements
         - orbit requirements
         - date requirements
 
         Todo: optimize the workflow:
             - remove product (from keep_X_latest_S1_files()
         """
         content = list_dirs(self.cfg.raw_directory, 'S1*_IW_GRD*')  # ignore of .download on the-fly
         logger.debug('%s local products found on disk', len(content))
         # Filter with new product only
         if new_products:
             logger.debug('new products:')
-            for np in new_products:
-                logger.debug('%s -> %s', np.__class__.__name__, np)
+            for new_product in new_products:
+                logger.debug('-> %s', new_product)
             # content is DirEntry
             # NEW is str!! Always
             # logger.debug('content[0]: %s -> %s', type(content[0]), content[0])
             # logger.debug('NEW[0]: %s -> %s', type(new_products[0]), new_products[0])
             # logger.debug('dirs found: %s', content)
             # If the directory appear directly
             content0 = content
-            content = list(filter(lambda d: d.path in new_products, content0))
+
+            def in_new_products(d: os.DirEntry) -> bool:
+                return d.path in new_products
+            content = list(filter(in_new_products, content0))
             # Or if the directory appear with an indirection: e.g. {prod}/{prod}.SAFE
             # content += list(filter(lambda d: d.path in (p.parent for p in new_products), content0))
             parent_dirs = [os.path.dirname(p) for p in new_products]
             content += list(filter(lambda d: d.path in parent_dirs, content0))
 
             logger.debug('dirs found & filtered: %s', content)  # List(DirEntry)
             logger.debug("products DL'ed: %s", new_products)    # List(str)
@@ -951,15 +1094,19 @@
             self._product_list = {}
             self._products_info = []
 
         # Filter by date specification
         content = [d for d in content if self.is_product_in_time_range(d.name)]
         logger.debug('%s local products remaining in the specified time range', len(content))
         # Discard incomplete products (when the complete products are there)
-        content = _discard_small_redundant(content, ident=lambda d: d.name)
+
+        def ident(d: os.DirEntry) -> str:
+            # assert isinstance(d, os.DirEntry), f"Expecting a DirEntry, got: {type(d)!r}"
+            return d.name
+        content = _discard_small_redundant(content, ident=ident)
         logger.debug('%s local products remaining after discarding incomplete and redundant products', len(content))
 
         # Build tuples of {product_dir, safe_dir, manifest_path,
         # orbit_direction, relative_orbit}
         products_info = [ {
             'product':  p,
             # EODAG saves SAFEs into {rawdir}/{prod}/{prod}.SAFE
@@ -994,85 +1141,93 @@
                 current_content = ci['product']
                 logger.debug('* %s', current_content.name)
                 self._product_list[current_content.name] = current_content
             self._products_info.extend(products_info)
         else:
             logger.warning('No time and orbit compatible products found on disk!')
 
-    def _filter_complete_dowloads_by_pair(self, tile_name, s1_products_info):
+    def _filter_complete_dowloads_by_pair(  # pylint: disable=too-many-locals
+            self, tile_name: str, s1_products_info: List[Dict]
+    ) -> List[Dict]:
         keys = {
-                'tile_name'         : tile_name,
-                'calibration_type'  : self.cfg.calibration_type,
-                }
-        fname_fmt_concatenation = self.cfg.fname_fmt_concatenation
+            'tile_name'         : tile_name,
+            'calibration_type'  : self.cfg.calibration_type,
+        }
+        fname_fmt_4concatenation = fname_fmt_concatenation(self.cfg)
         k_dir_assoc = { 'ascending': 'ASC', 'descending': 'DES' }
-        ident     = lambda ci: ci['product'].name
-        get_orbit = lambda ci: ci['relative_orbit']
-        get_direc = lambda ci: k_dir_assoc.get(ci['orbit_direction'], ci['orbit_direction'])
+        ident     : Callable[[Dict], str] = lambda ci: ci['product'].name
+        get_orbit : Callable[[Dict], int] = lambda ci: ci['relative_orbit']
+        get_direc : Callable[[Dict], str] = lambda ci: k_dir_assoc.get(ci['orbit_direction'], ci['orbit_direction'])
         prod_re = re.compile(r'(S1.)_IW_...._...._(\d{8})T\d{6}_\d{8}T\d{6}.*')
 
         # We need to report every S2 product that could not be generated,
         # even if we have no S1 product associated. We cannot use s1_products_info
         # list for that purpose as it only contains S1 products that have been
         # successfully downloaded. => we iterate over the download blacklist
         for failure, missing in self.__failed_S1_downloads_by_S2_uid.items():
             # Reference missing product for the orbit + date
             # (we suppose there won't be a mix of S1A + S1B for the same pair)
             ref_missing_S1_product = missing[0].related_product()
             eo_ron  = product_property(ref_missing_S1_product, 'relativeOrbitNumber')
             eo_dir  = product_property(ref_missing_S1_product, 'orbitDirection')
             eo_dir  = k_dir_assoc.get(eo_dir, eo_dir)
             eo_id   = ref_missing_S1_product.as_dict()['id']
-            eo_date = prod_re.match(eo_id).groups()[1]
+            match   = prod_re.match(eo_id)
+            eo_date = match.groups()[1] if match else "????????"
             # Generate the reference name of S2 products that can't be produced
             keys['orbit_direction']   = eo_dir
             keys['orbit']             = f'{eo_ron:03}'  # 3 digits, pad w/ zeros
-            keys['flying_unit_code']  = prod_re.match(eo_id).groups()[0].lower()
+            match                     = prod_re.match(eo_id)
+            keys['flying_unit_code']  = match.groups()[0].lower() if match else "S1?"
             keys['acquisition_stamp'] = f'{eo_date}txxxxxx'
             keys['polarisation']      = '*'
-            s2_product_name = fname_fmt_concatenation.format_map(keys)
+            s2_product_name = fname_fmt_4concatenation.format_map(keys)
             keeps   = []  # Workaround to filter out the current list.
             for ci in s1_products_info:
-                id   = ident(ci)
-                date = prod_re.match(id).groups()[1]
-                ron  = get_orbit(ci)
-                logger.debug('Check if the ignore-key %s matches the key (%s) of the paired S1 product %s', f'{date}#{ron}', failure, id)
+                pid   = ident(ci)
+                match = prod_re.match(pid)
+                date  = match.groups()[1] if match else "????????"
+                ron   = get_orbit(ci)
+                logger.debug('Check if the ignore-key %s matches the key (%s) of the paired S1 product %s', f'{date}#{ron}', failure, pid)
                 if f'{date}#{ron}' == failure:
                     assert eo_date == date
                     assert eo_ron  == ron
-                    assert eo_dir  == get_direc(ci), f"EO product: {eo_id} doesn't match product on disk: {id}"
+                    assert eo_dir  == get_direc(ci), f"EO product: {eo_id} doesn't match product on disk: {pid}"
                     logger.debug('%s will be ignored to produce %s because: %s', ci, s2_product_name, missing)
                     # At most this could happen once as s1 products go by pairs,
                     # and thus a DL failure may be associated to zero or one DL success.
                     # assert len(self.__download_failures[failure]) == 1
                     # dont-break  # We don't actually need to continue except to... keep non "failure" products...
                 else:
                     keeps.append(ci)
             s1_products_info = keeps
             logger.warning("Don't generate %s, because %s", s2_product_name, missing)
-            self.__skipped_S2_products.append(f'Download failure: {s2_product_name} cannot be produced because of the following issues with the inputs: {missing}')
+            self.__skipped_S2_products.append(
+                    f'Download failure: {s2_product_name} cannot be produced because of the following issues with the inputs: {missing}')
         return s1_products_info
 
-    def _filter_products_with_enough_coverage(self, tile_name, products_info):
+    def _filter_products_with_enough_coverage(self, tile_name: str, products_info: List[Dict]) -> List[Dict]:
         """
         Filter products (/pairs of products) that provide enough coverage for
         the requested tile.
 
         This function is meant to be a mock entry-point.
         """
         layer = Layer(self.cfg.output_grid)
         current_tile = layer.find_tile_named(tile_name)
         if not current_tile:
             logger.info("Tile %s does not exist", tile_name)
             return []
-        products_info = _keep_products_with_enough_coverage(products_info,
-                self.cfg.tile_to_product_overlap_ratio, current_tile)
+        products_info = _keep_products_with_enough_coverage(
+                products_info, self.cfg.tile_to_product_overlap_ratio, current_tile)
         return products_info
 
-    def _update_s1_img_list_for(self, tile_name):
+    def _update_s1_img_list_for(  # pylint: disable=too-many-locals
+            self, tile_name: str
+    ) -> None:
         """
         This method updates the list of S1 images available
         (from analysis of raw_directory), and it keeps only the images (/pairs
         or images) that provide enough coverage.
 
         Returns:
            the list of S1 images available as instances
@@ -1109,59 +1264,58 @@
             for image in vv_images + vh_images + hv_images + hh_images:
                 if image not in self.processed_filenames:
                     acquisition.add_image(image)
                     self.nb_images += 1
             if l_vv + l_vh + l_hv + l_hh == 0:
                 # There is not a single file that would have been compatible
                 # with what is expected
-                logger.critical("Problem with %s", manifest)
-                logger.critical("Please remove the raw data for %s SAFE file", manifest)
-                sys.exit(exits.CORRUPTED_DATA_SAFE)
+                logger.warning("Product associated to %s is corrupted: no VV, VH, HV or HH file found", manifest)
+                raise exceptions.CorruptedDataSAFEError(current_content.name, f"no image files in {safe_dir!r} found")
 
             self.raw_raster_list.append(acquisition)
 
-    def _filter_images_or_ortho_according_to_conf(self, polarisation, all_tiffs):
+    def _filter_images_or_ortho_according_to_conf(self, polarisation: str, all_tiffs: List[str]) -> Tuple[int, List[str]]:
         """
         Helper function that returns the images compatible with the required
         polarisation, and if that polarisation has been requested in the
         configuration file.
 
         It also returns the number of file that would have been compatibles,
         independently of the requested polarisation. This will permit to control
         the SAFE contains what it's expected to contain.
         """
         k_polarisation_associations = {
-                'vv' : ['VV', 'VV VH'],
-                'vh' : ['VH', 'VV VH'],
-                'hv' : ['HV', 'HH HV'],
-                'hh' : ['HH', 'HH HV'],
-                }
+            'vv' : ['VV', 'VV VH'],
+            'vh' : ['VH', 'VV VH'],
+            'hv' : ['HV', 'HH HV'],
+            'hh' : ['HH', 'HH HV'],
+        }
         all_images = filter_images_or_ortho(polarisation, all_tiffs)
         pol_images = all_images if self.cfg.polarisation in k_polarisation_associations[polarisation] else []
         return len(all_images), pol_images
 
-    def tile_exists(self, tile_name_field):
+    def tile_exists(self, tile_name_field: str) -> bool:
         """
         This method check if a given MGRS tiles exists in the database
 
         Args:
           tile_name_field: MGRS tile identifier
 
         Returns:
           True if the tile exists, False otherwise
         """
         layer = Layer(self.cfg.output_grid)
 
         for current_tile in layer:
-            #logger.debug("%s", current_tile.GetField('NAME'))
+            # logger.debug("%s", current_tile.GetField('NAME'))
             if current_tile.GetField('NAME') == tile_name_field:
                 return True
         return False
 
-    def get_tiles_covered_by_products(self):
+    def get_tiles_covered_by_products(self) -> List[str]:
         """
         This method returns the list of MGRS tiles covered
         by available S1 products.
 
         Returns:
            The list of MGRS tiles identifiers covered by product as string
         """
@@ -1180,29 +1334,29 @@
                 if intersection.GetArea() / tile_footprint.GetArea()\
                    > self.cfg.tile_to_product_overlap_ratio:
                     tile_name = current_tile.GetField('NAME')
                     if tile_name not in tiles:
                         tiles.append(tile_name)
         return tiles
 
-    def is_product_in_time_range(self, product : str):
+    def is_product_in_time_range(self, product : str) -> bool:
         """
         Returns whether the product name is within time range [first_date, last_date]
         """
         assert '/' not in product, f"Expecting a basename for {product}"
         start_time = extract_product_start_time(product)
         if not start_time:
             return False
         start = '{YYYY}-{MM}-{DD}'.format_map(start_time)
         is_in_range = self.first_date <= start <= self.last_date
         logger.debug('  %s %s /// %s == %s <= %s <= %s', 'KEEP' if is_in_range else 'DISCARD',
                 product, is_in_range, self.first_date, start, self.last_date)
         return is_in_range
 
-    def get_s1_intersect_by_tile(self, tile_name_field):
+    def get_s1_intersect_by_tile(self, tile_name_field: str) -> List[Dict]:
         """
         This method returns the list of S1 product intersecting a given MGRS tile
 
         Args:
           tile_name_field: The MGRS tile identifier
 
         Returns:
@@ -1229,82 +1383,54 @@
                 'tile_coverage'  : image.product_info['coverage'],
                 # 'orbit_direction': get_orbit_direction(manifest),
                 # 'orbit'          : '{:0>3d}'.format(get_relative_orbit(manifest)),
                 })
 
         return intersect_raster
 
-    def _get_mgrs_tile_geometry_by_name(self, mgrs_tile_name):
-        """
-        This method returns the MGRS tile geometry
-        as OGRGeometry given its identifier
-
-        Args:
-          mgrs_tile_name: MGRS tile identifier
-
-        Returns:
-          The MGRS tile geometry as OGRGeometry or raise ValueError
-        """
-        mgrs_layer = Layer(self.cfg.output_grid)
-
-        for mgrs_tile in mgrs_layer:
-            if mgrs_tile.GetField('NAME') == mgrs_tile_name:
-                return mgrs_tile.GetGeometryRef().Clone()
-        raise ValueError("MGRS tile does not exist", mgrs_tile_name)
-
-    def check_srtm_coverage(self, tiles_to_process):
+    def check_dem_coverage(self, tiles_to_process: List[str]) -> Dict[str, Dict]:
         """
         Given a set of MGRS tiles to process, this method
-        returns the needed SRTM tiles and the corresponding coverage.
+        returns the needed DEM tiles and the corresponding coverage.
 
         Args:
           tile_to_process: The list of MGRS tiles identifiers to process
 
         Return:
-          A list of tuples (SRTM tile id, coverage of MGRS tiles).
+          A list of tuples (DEM tile id, coverage of MGRS tiles).
           Coverage range is [0,1]
         """
-        srtm_layer = Layer(self.cfg.srtm_db_filepath, driver_name='GPKG')
+        dem_layer  = Layer(self.cfg.dem_db_filepath)
+        mgrs_layer = Layer(self.cfg.output_grid)
 
-        needed_srtm_tiles = {}
+        needed_dem_tiles = {}
 
         for tile in tiles_to_process:
-            logger.debug("Check SRTM tile for %s", tile)
-
-            srtm_tiles = []
-            mgrs_footprint = self._get_mgrs_tile_geometry_by_name(tile)
-            area = mgrs_footprint.GetArea()
-            srtm_layer.reset_reading()
-            for srtm_tile in srtm_layer:
-                srtm_footprint = srtm_tile.GetGeometryRef()
-                intersection = mgrs_footprint.Intersection(srtm_footprint)
-                if intersection.GetArea() > 0:
-                    coverage = intersection.GetArea() / area
-                    srtm_tiles.append((srtm_tile.GetField('id'), coverage))
-            needed_srtm_tiles[tile] = srtm_tiles
-        logger.info("SRTM ok")
-        return needed_srtm_tiles
-
-    def record_processed_filenames(self):
-        """ Record the list of processed filenames (DEPRECATED)"""
-        with open(os.path.join(self.cfg.output_preprocess,
-                               "processed_filenames.txt"), "a") as in_file:
-            for fic in self.processed_filenames:
-                in_file.write(fic + "\n")
+            logger.debug("Check DEM tiles for %s", tile)
+            mgrs_footprint = get_mgrs_tile_geometry_by_name(tile, mgrs_layer)
+            logger.debug("%s original %s footprint is %s", tile, mgrs_footprint.GetSpatialReference().GetName(), mgrs_footprint)
+            dem_tiles = find_dem_intersecting_poly(
+                    mgrs_footprint, dem_layer, self.cfg.dem_field_ids, self.cfg.dem_main_field_id)
+            needed_dem_tiles[tile] = dem_tiles
+            logger.info("S2 tile %s is covered by %s DEM tiles", tile, len(dem_tiles))
+        logger.info("DEM ok")
+        return needed_dem_tiles
 
-    def get_processed_filenames(self):
+    def get_processed_filenames(self) -> List[str]:
         """ Read back the list of processed filenames (DEPRECATED)"""
         try:
-            with open(os.path.join(self.cfg.output_preprocess,
-                                   "processed_filenames.txt"), "r") as in_file:
+            with open(
+                    os.path.join(self.cfg.output_preprocess, "processed_filenames.txt"),
+                    "r",
+                    encoding="utf-8")as in_file:
                 return in_file.read().splitlines()
         except (IOError, OSError):
             return []
 
-    def get_raster_list(self):
+    def get_raster_list(self) -> List[S1DateAcquisition]:
         """
         Get the list of raw S1 product rasters
 
         Returns:
           the list of raw rasters
         """
         return self.raw_raster_list
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/S1FilteringProcessor.py` & `s1tiling-1.1.0rc1/deprecated/S1FilteringProcessor.py`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/__init__.py` & `s1tiling-1.1.0rc1/s1tiling/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/otbpipeline.py` & `s1tiling-1.1.0rc1/s1tiling/libs/otbwrappers/lia.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # =========================================================================
 #   Program:   S1Processor
 #
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   All rights reserved.
+#   Copyright 2017-2024 (c) CNES.
+#   Copyright 2022-2024 (c) CS GROUP France.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -22,2147 +24,1709 @@
 #
 # =========================================================================
 #
 # Authors: Thierry KOLECK (CNES)
 #          Luc HERMITTE (CS Group)
 # =========================================================================
 
-# from __future__ import annotations  # Require Python 3.7+...
-
 """
-This module provides pipeline for chaining OTB applications, and a pool to execute them.
+This modules defines the specialized Python wrappers for the OTB Applications used in
+the pipeline for LIA production needs.
 """
 
+import logging
 import os
-import sys
-import shutil
 import re
-import datetime
-import copy
-from abc import ABC, abstractmethod
-from itertools import filterfalse
-import logging
-import logging.handlers
-import multiprocessing
-import subprocess
-from pathlib import Path
-
-# memory leaks
-from distributed import get_worker
-import objgraph
-from pympler import tracker # , muppy
+from typing import Dict, List, Optional, Type
+# from packaging import version
 
 from osgeo import gdal
 import otbApplication as otb
-from . import Utils
-from . import exits
-from .outcome import PipelineOutcome
 
-logger = logging.getLogger('s1tiling.pipeline')
+from s1tiling.libs.otbtools import otb_version
 
-re_tiff    = re.compile(r'\.tiff?$')
-re_any_ext = re.compile(r'\.[^.]+$')  # Match any kind of file extension
-
-
-def otb_version():
-    """
-    Returns the current version on OTB (through a call to ResetMargin -version)
-    The result is cached
+from ..file_naming   import (
+        OutputFilenameGeneratorList, TemplateOutputFilenameGenerator,
+)
+from ..meta import (
+        Meta, append_to, in_filename, out_filename, tmp_filename, is_running_dry,
+)
+from ..steps import (
+        InputList, OTBParameters, ExeParameters,
+        _check_input_step_type,
+        AbstractStep, StepFactory,
+        _FileProducingStepFactory, AnyProducerStepFactory, ExecutableStepFactory, OTBStepFactory,
+        commit_execution,
+        ram,
+)
+from ..otbpipeline   import (
+    fetch_input_data, fetch_input_data_all_inputs, TaskInputInfo,
+)
+from .helpers        import (
+        does_s2_data_match_s2_tile, does_sin_lia_match_s2_tile_for_orbit, remove_polarization_marks,
+)
+from .s1_to_s2       import (
+        s2_tile_extent, _ConcatenatorFactory, _OrthoRectifierFactory,
+)
+from ..              import Utils
+from ..configuration import (
+        Configuration,
+        dname_fmt_lia_product, dname_fmt_tiled,
+        extended_filename_lia_degree, extended_filename_lia_sin, extended_filename_tiled,
+        pixel_type,
+)
+
+logger = logging.getLogger('s1tiling.wrappers.lia')
+
+
+class AgglomerateDEMOnS2(AnyProducerStepFactory):
     """
-    if not hasattr(otb_version, "_version"):
-        try:
-            r = subprocess.run(['otbcli_ResetMargin', '-version'], stdout=subprocess.PIPE,
-                    stderr=subprocess.STDOUT)
-            version = r.stdout.decode('utf-8').strip('\n')
-            version = re.search(r'\d+(\.\d+)+$', version)[0]
-            logger.info("OTB version detected on the system is %s", version)
-            otb_version._version = version
-        except Exception as ex:  # pylint: disable=broad-except
-            logger.exception(ex)
-            raise RuntimeError("Cannot determine current OTB version")
-    return otb_version._version
+    Factory that produces a :class:`Step` that builds a VRT from a list of DEM files.
 
-
-def as_list(param):
-    """
-    Make sure ``param`` is either a list or encapsulated in a list.
+    The choice has been made to name the VRT file after the basename of the
+    root S1 product and not the names of the DEM tiles.
     """
-    if isinstance(param, list):
-        return param
-    else:
-        return [param]
-
 
-class OutputFilenameGenerator(ABC):
-    """
-    Abstract class for generating filenames.
-    Several policies are supported as of now:
-    - return the input string (default implementation)
-    - replace a text with another one
-    - {template} strings
-    - list of any of the other two
-    """
-    def generate(self, basename, keys):  # pylint: disable=unused-argument,no-self-use
-        """
-        Default implementation does nothing.
-        """
-        return basename
-
-
-class ReplaceOutputFilenameGenerator(OutputFilenameGenerator):
-    """
-    Given a pair ``[text_to_search, text_to_replace_with]``,
-    replace the exact matching text with new text in ``basename`` metadata.
-    """
-    def __init__(self, before_afters):
-        assert isinstance(before_afters, list)
-        self.__before_afters = before_afters
-
-    def generate(self, basename, keys):
-        filename = basename.replace(*self.__before_afters)
-        return filename
-
-
-class CannotGenerateFilename(KeyError):
-    """
-    Exception used to filter out cases where a meta cannot serve as a direct
-    input of a :class:`StepFactory`.
-    """
-    pass
-
-
-class TemplateOutputFilenameGenerator(OutputFilenameGenerator):
-    """
-    Given a template: ``"text{key1}_{another_key}_.."``,
-    inject the metadata instead of the template keys.
-    """
-    def __init__(self, template):
-        assert isinstance(template, str)
-        self.__template = template
-
-    def generate(self, basename, keys):
-        try:
-            rootname = os.path.splitext(basename)[0]
-            filename = self.__template.format(**keys, rootname=rootname)
-            return filename
-        except KeyError as e:
-            raise CannotGenerateFilename(f'Impossible to generate a filename matching {self.__template} from {keys}') from e
-
-
-class OutputFilenameGeneratorList(OutputFilenameGenerator):
-    """
-    Some steps produce several products.
-    This specialization permits to generate several output filenames.
-
-    It's constructed from other filename generators.
-    """
-    def __init__(self, generators):
-        assert isinstance(generators, list)
-        self.__generators = generators
-
-    def generate(self, basename, keys):
-        filenames = [generator.generate(basename, keys) for generator in self.__generators]
-        return filenames
-
-
-def as_app_shell_param(param):
-    """
-    Internal function used to stringigy value to appear like a a parameter for a program
-    launched through shell.
-
-    foo     -> 'foo'
-    42      -> 42
-    [a, 42] -> 'a' 42
-    """
-    if   isinstance(param, list):
-        return ' '.join(as_app_shell_param(e) for e in param)
-    elif isinstance(param, int):
-        return param
-    else:
-        return f"'{param}'"
-
-
-def in_filename(meta):
-    """
-    Helper accessor to access the input filename of a `Step`.
-    """
-    assert 'in_filename' in meta
-    return meta['in_filename']
-
-
-def out_filename(meta):
-    """
-    Helper accessor to access the ouput filename of a `Step`.
-    """
-    return meta.get('out_filename')
-
-
-def tmp_filename(meta):
-    """
-    Helper accessor to access the temporary ouput filename of a `Step`.
-    """
-    assert 'out_tmp_filename' in meta
-    return meta.get('out_tmp_filename')
-
-
-def get_task_name(meta):
-    """
-    Helper accessor to the task name related to a `Step`.
-
-    By default, the task name is stored in `out_filename` key.
-    In the case of reducing :class:`MergeStep`, a dedicated name shall be
-    provided. See :class:`Concatenate`
-
-    Important, task names shall be unique and attributed to a single step.
-    """
-    if 'task_name' in meta:
-        return meta['task_name']
-    else:
-        return out_filename(meta)
-
-
-def out_extended_filename_complement(meta):
-    """
-    Helper accessor to the extended filename to use to produce the image.
-    """
-    return meta.get('out_extended_filename_complement', '')
-
-
-def _fetch_input_data(key, inputs):
-    """
-    Helper function that extract the meta data associated to a key from a
-    multiple-inputs list of inputs.
-    """
-    keys = set().union(*(input.keys() for input in inputs))
-    assert key in keys, f"Cannot find input '{key}' among {keys}"
-    return [input[key] for input in inputs if key in input.keys()][0]
-
-
-def manifest_to_product_name(manifest):
-    """
-    Helper function that returns the product name (SAFE directory without the
-    ``.SAFE`` extension) from the full path to the :file:`manifest.safe` file.
-    """
-    fullpath = Path(manifest)
-    return fullpath.parent.stem
-
-
-def product_exists(meta):
-    """
-    Helper accessor that tells whether the product described by the metadata
-    already exists.
-    """
-    if 'does_product_exist' in meta:
-        return meta['does_product_exist']()
-    else:
-        return os.path.isfile(out_filename(meta))
-
-
-def _is_compatible(output_meta, input_meta):
-    """
-    Tells whether ``input_meta`` is a valid input for ``output_meta``
-
-    Uses the optional meta information ``is_compatible`` from ``output_meta``
-    to tell whether they are compatible.
-
-    This will be uses for situations where an input file will be used as input
-    for several different new files. Typical example: all final normlimed
-    outputs on a S2 tile will rely on the same map of sin(LIA). As such,
-    the usual __input -> expected output__ approach cannot work.
-    """
-    if 'is_compatible' in output_meta:
-        return output_meta['is_compatible'](input_meta)
-    else:
-        return False
-
-
-def files_exist(files):
-    """
-    Checks whether a single file, or all files from a list, exist.
-    """
-    if isinstance(files, str):
-        return os.path.isfile(files)
-    else:
-        for file in files:
-            if not os.path.isfile(file):
-                return False
-        return True
-
-
-def is_running_dry(meta):
-    """
-    Helper function to test whether metadata has ``dryrun`` property set to True.
-    """
-    return meta.get('dryrun', False)
-
-
-def is_debugging_caches(meta):
-    """
-    Helper function to test whether metadata has ``debug_caches`` property set to True.
-    """
-    return meta.get('debug_caches', False)
-
-
-def execute(params, dryrun):
-    """
-    Helper function to execute any external command.
-
-    And log its execution, measure the time it takes.
-    """
-    msg = ' '.join([str(p) for p in params])
-    logging.info('$> '+msg)
-    if not dryrun:
-        with Utils.ExecutionTimer(msg, True):
-            subprocess.run(args=params, check=True)
-
-
-class AbstractStep:
-    """
-    Internal root class for all actual `Step` s.
-
-    There are several kinds of steps:
-
-    - :class:`FirstStep` that contains information about input files
-    - :class:`Step` that registers an otbapplication binding
-    - :class:`StoreStep` that momentarilly disconnect on-memory pipeline to
-      force storing of the resulting file.
-    - :class:`ExecutableStep` that executes external applications
-    - :class:`MergeStep` that operates a rendez-vous between several steps
-      producing files of a same kind.
-
-    The step will contain information like the current input file, the current
-    output file...
-    """
-    def __init__(self, *unused_argv, **kwargs):
+    def __init__(self, cfg: Configuration, *args, **kwargs) -> None:
         """
         constructor
         """
-        meta = kwargs
-        if 'basename' not in meta:
-            logger.critical('no "basename" in meta == %s', meta)
-        assert 'basename' in meta
-        # Clear basename from any noise
-        self._meta = meta
+        fname_fmt = 'DEM_{tile_name}.vrt'
+        fname_fmt = cfg.fname_fmt.get('dem_s2_agglomeration', fname_fmt)
+        super().__init__(  # type: ignore # mypy issue 4335
+                cfg,
+                # Because VRT links temporary files, it must not be reused in case of a crash => use tmp_dem_dir
+                gen_tmp_dir=os.path.join(cfg.tmpdir, cfg.tmp_dem_dir),
+                gen_output_dir=None,      # Use gen_tmp_dir,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                name="AgglomerateDEMOnS2",
+                action=AgglomerateDEMOnS2.agglomerate,
+                *args, **kwargs)
+        self.__cfg = cfg  # Will be used to access cached DEM intersecting S2 tile
+        self.__dem_dir             = cfg.tmp_dem_dir
+        self.__dem_filename_format = cfg.dem_filename_format
 
-    @property
-    def is_first_step(self):
+    @staticmethod
+    def agglomerate(parameters: ExeParameters, dryrun: bool) -> None:
         """
-        Tells whether this step is the first of a pipeline.
+        The function that calls :func:`gdal.BuildVRT()`.
         """
-        return True
+        logger.info("gdal.BuildVRT(%s, %s)", parameters[0], parameters[1:])
+        assert len(parameters) > 0
+        if not dryrun:
+            gdal.BuildVRT(parameters[0], parameters[1:])
 
-    @property
-    def meta(self):
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
         """
-        Step meta data property.
+        Factory that takes care of extracting meta data from S1 input files.
         """
-        return self._meta
+        meta = super().complete_meta(meta, all_inputs)
+        # find DEMs that intersect the input image
+        meta['dem_infos'] = self.__cfg.get_dems_covering_s2_tile(meta['tile_name'])
+        meta['dems'] = sorted(meta['dem_infos'].keys())
+        logger.debug("DEM found for %s: %s", in_filename(meta), meta['dems'])
+        dem_files = list(map(
+                lambda s: os.path.join(
+                    self.__dem_dir,    # Use copies/links from cached DEM directory
+                    os.path.basename(  # => Strip any dirname from the input dem_filename_format
+                        self.__dem_filename_format.format_map(meta['dem_infos'][s]))),
+                meta['dem_infos']))
+        meta['dem_files'] = dem_files
+        missing_dems = list(filter(lambda f: not os.path.isfile(f), dem_files))
+        if len(missing_dems) > 0:
+            raise RuntimeError(
+                    f"Cannot create DEM vrt for {meta['tile_name']}: the following DEM files are missing: {', '.join(missing_dems)}")
+        return meta
 
-    @property
-    def basename(self):
-        """
-        Basename property will be used to generate all future output filenames.
-        """
-        return self._meta['basename']
+    def parameters(self, meta: Meta) -> ExeParameters:
+        # While it won't make much a difference here, we are still using tmp_filename.
+        return [tmp_filename(meta)] + meta['dem_files']
+
+
+class ProjectDEMToS2Tile(ExecutableStepFactory):
+    """
+    Factory that produces a :class:`ExecutableStep` that projects DEM onto target S2 tile
+    as described in :ref:`Project DEM to S2 tile <project_dem_to_s2-proc>`.
+
+    It requires the following information from the configuration object:
+
+    - `ram_per_process`
+    - `tmp_dir`
+    - `fname_fmt`  -- optional key: `dem_on_s2`
+    - `out_spatial_res`
+    - `interpolation_method` -- OTB key converted to GDAL equivalent
+    - `nb_procs`
+
+    It requires the following information from the metadata dictionary:
+
+    - `tile_name`
+    - `tile_origin`
+    - `nodata` -- optional
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'DEM_projected_on_{tile_name}.tiff'
+        fname_fmt = cfg.fname_fmt.get('dem_on_s2', fname_fmt)
+        super().__init__(
+                cfg,
+                exename='gdalwarp', name='ProjectDEMToS2Tile',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=None,      # Use gen_tmp_dir,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description="Warped DEM to S2 tile",
+        )
+        self.__out_spatial_res   = cfg.out_spatial_res
+        self.__resampling_method = cfg.dem_warp_resampling_method
+        self.__nb_threads        = cfg.nb_procs
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        """
+        Register temporary files from previous step for removal.
+        """
+        meta = super().complete_meta(meta, all_inputs)
+
+        in_file = in_filename(meta)
+        meta['files_to_remove'] = [in_file]  # DEM VRT
+        logger.debug('Register files to remove after DEM warping on S2 computation: %s', meta['files_to_remove'])
+        return meta
 
-    @property
-    def out_filename(self):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        Property that returns the name of the file produced by the current step.
+        Set S2 related information, that should have been carried around...
         """
-        assert 'out_filename' in self._meta
-        return self._meta['out_filename']
+        super().update_image_metadata(meta, all_inputs)
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        imd['S2_TILE_CORRESPONDING_CODE'] = meta['tile_name']
+        imd['SPATIAL_RESOLUTION']         = str(self.__out_spatial_res)
+        imd['DEM_RESAMPLING_METHOD']      = self.__resampling_method
+        # TODO: shall we set "ORTHORECTIFIED = True" ??
+        # TODO: DEM_LIST
+
+    def parameters(self, meta: Meta) -> ExeParameters:
+        """
+        Returns the parameters to use with :external:std:doc:`gdalwarp
+        <programs/gdalwarp>` to projected the DEM onto the S2 geometry.
+        """
+        image       = in_filename(meta)
+        tile_name   = meta['tile_name']
+        tile_origin = meta['tile_origin']
+        spacing     = self.__out_spatial_res
+        logger.debug("%s.parameters(%s) /// image: %s /// tile_name: %s",
+                self.__class__.__name__, meta, image, tile_name)
+
+        extent = s2_tile_extent(tile_name, tile_origin, in_epsg=4326, spacing=spacing)
+
+        nodata = meta.get('nodata', -32768)
+        parameters = [
+                "-wm", str(self.ram_per_process*1024*1024),
+                "-multi", "-wo", f"{self.__nb_threads}",  # It's already quite fast...
+                "-t_srs", f"epsg:{extent['epsg']}",
+                "-tr", f"{spacing}", f"-{spacing}",
+                "-ot", "Float32",
+                # "-crop_to_cutline",
+                "-te", f"{extent['xmin']}", f"{extent['ymin']}", f"{extent['xmax']}", f"{extent['ymax']}",
+                "-r", self.__resampling_method,
+                "-dstnodata", str(nodata),
+                image,
+                tmp_filename(meta),
+        ]
+        return parameters
+
+
+class ProjectGeoidToS2Tile(OTBStepFactory):
+    """
+    Factory that produces a :class:`Step` that projects any kind of Geoid onto
+    target S2 tile as described in :ref:`Project Geoid to S2 tile
+    <project_geoid_to_s2-proc>`.
+
+    This particular implementation uses another file in the expected geometry
+    and :external:std:doc:`super impose <Applications/app_Superimpose>` the
+    Geoid onto it. Unlike :external:std:doc:`gdalwarp <programs/gdalwarp>`,
+    OTB application supports non-raster geoid formats.
+
+    It requires the following information from the configuration object:
+
+    - `ram_per_process`
+    - `tmp_dir`    -- useless in the in-memory nomical case
+    - `fname_fmt`  -- optional key: `geoid_on_s2`, useless in the in-memory nominal case
+    - `interpolation_method` -- for use by :external:std:doc:`super impose
+      <Applications/app_Superimpose>`
+    - `out_spatial_res` -- as a workaround...
+
+    It requires the following information from the metadata dictionary:
+
+    - `tile_name`
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'GEOID_projected_on_{tile_name}.tiff'
+        fname_fmt = cfg.fname_fmt.get('geoid_on_s2', fname_fmt)
+        super().__init__(
+                cfg,
+                param_in="inr", param_out="out",
+                appname='Superimpose', name='ProjectGeoidToS2Tile',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=None,      # Use gen_tmp_dir,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description="Geoid superimposed on S2 tile",
+        )
+        self.__GeoidFile            = os.path.join(cfg.tmpdir, 'geoid', os.path.basename(cfg.GeoidFile))
+        self.__interpolation_method = cfg.interpolation_method
+        self.__out_spatial_res      = cfg.out_spatial_res  # TODO: should extract this information from reference image
 
-    @property
-    def shall_store(self):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        No OTB related step requires its result to be stored on disk and to
-        break in_memory connection by default.
-
-        However, the artificial Step produced by :class:`Store` factory will
-        force the result of the `previous` application(s) to be stored on disk.
+        Set S2 related information, that'll be carried around.
         """
-        return False
+        super().update_image_metadata(meta, all_inputs)
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        imd['S2_TILE_CORRESPONDING_CODE'] = meta['tile_name']
+        imd['SPATIAL_RESOLUTION']         = str(self.__out_spatial_res)
 
-    def release_app(self):
+    def parameters(self, meta: Meta) -> OTBParameters:
         """
-        Makes sure that steps with applications are releasing the application
+        Returns the parameters to use with :external:std:doc:`super impose
+        <Applications/app_Superimpose>` to projected the Geoid onto the S2 geometry.
         """
-        pass
+        in_s2_dem = in_filename(meta)
+        return {
+                'ram'                     : ram(self.ram_per_process),
+                'inr'                     : in_s2_dem,  # Reference input is the DEM projected on S2
+                'inm'                     : self.__GeoidFile,
+                'interpolator'            : self.__interpolation_method,  # TODO: add parameter
+                'interpolator.bco.radius' : 2,  # 2 is the default value for bco
+        }
 
-    def clean_cache(self):
-        """
-        Takes care or removing intermediary files once we know they are no
-        longer required like the orthorectified subtiles once the
-        concatenation has been done.
-        """
-        if 'files_to_remove' in self.meta :
-            files = self.meta['files_to_remove']
-            # All possible geom files that may exist
-            geoms = [re.sub(re_tiff, '.geom', fn) for fn in files]
-            # All geaoms that do actually exist
-            geoms = [fn for fn in geoms if os.path.isfile(fn)]
-            files = files + geoms
-            if is_debugging_caches(self.meta):
-                logger.debug('NOT cleaning intermediary files: %s (cache debugging mode!)', files)
-            else:
-                logger.debug('Cleaning intermediary files: %s', files)
-                if not is_running_dry(self.meta):
-                    Utils.remove_files(files)
-            self.meta.pop('files_to_remove', None)
 
+class SumAllHeights(OTBStepFactory):
+    """
+    Factory that produces a :class:`Step` that adds DEM + Geoid that cover a
+    same footprint, as described in :ref:`Sum DEM + Geoid
+    <sum_dem_geoid_on_s2-proc>`.
 
-    def _write_image_metadata(self):
-        """
-        Update Image metadata (with GDAL API).
-        Fetch the new content in ``meta['image_metadata']``
-        """
-        img_meta = self.meta.get('image_metadata', {})
-        # fullpath = out_filename(self.meta)
-        fullpath = self.tmp_filename
-        if not img_meta:
-            logger.debug('No metadata to update in %s', fullpath)
-            return
-        if is_running_dry(self.meta):
-            logger.debug("Don't set metadata in %s (dry-run)", fullpath)
-            return
-        def do_write(fullpath, img_meta):
-            logger.debug('Set metadata in %s', fullpath)
-            dst = gdal.Open(fullpath, gdal.GA_Update)
-            assert dst
+    It requires the following information from the configuration object:
 
-            for (kw, val) in img_meta.items():
-                assert isinstance(val, str), f'GDAL metadata shall be strings. "{kw}" is a {val.__class__.__name__} (="{val}")'
-                logger.debug(' - %s -> %s', kw, val)
-                dst.SetMetadataItem(kw, val)
-            dst.FlushCache()  # We really need to be sure it has been flushed now, if not closed
-            del dst
-            logger.debug('Metadata Set! (%s)', fullpath)
-        if isinstance(fullpath, list):
-            # Case of applications that produce several files like ComputeLIA
-            for fp in fullpath:
-                # TODO: how to specialize DESCRIPTION for each output image
-                do_write(fp, img_meta)
-        else:
-            do_write(fullpath, img_meta)
+    - `ram_per_process`
+    - `tmp_dir`    -- useless in the in-memory nomical case
+    - `fname_fmt`  -- optional key: `height_on_s2`, useless in the in-memory nominal case
 
+    It requires the following information from the metadata dictionary:
 
-class ExecutableStep(AbstractStep):
-    """
-    Generic step for calling any external application.
+    - `nodata` -- optional
     """
-    def __init__(self, exename, *argv, **kwargs):
+    def __init__(self, cfg: Configuration) -> None:
         """
         Constructor.
         """
-        super().__init__(None, *argv, **kwargs)
-        self._exename = exename
-        # logger.debug('ExecutableStep %s constructed', self._exename)
-
-    @property
-    def tmp_filename(self):
-        """
-        Property that returns the name of the file produced by the current step while
-        the external application is running.
-        Eventually, it'll get renamed into :func:`AbstractStep.out_filename` if
-        the application succeeds.
-        """
-        return tmp_filename(self.meta)
-
-    def execute_and_write_output(self, parameters):  # pylint: disable=no-self-use
-        """
-        Actually execute the external program.
-        While the program runs, a temporary filename will be used as output.
-        On successful execution, the output will be renamed to match its
-        expected final name.
-        """
-        dryrun = is_running_dry(self.meta)
-        logger.debug("ExecutableStep: %s (%s)", self, self.meta)
-        execute([self._exename]+ parameters, dryrun)
-        if not dryrun:
-            self._write_image_metadata()
-            commit_execution(self.tmp_filename, self.out_filename)
-        if 'post' in self.meta and not dryrun:
-            for hook in self.meta['post']:
-                hook(self.meta)
-        self.clean_cache()
-        self.meta['pipe'] = [self.out_filename]
+        fname_fmt = 'DEM+GEOID_projected_on_{tile_name}.tiff'
+        fname_fmt = cfg.fname_fmt.get('height_on_s2', fname_fmt)
+        super().__init__(
+                cfg,
+                appname='BandMath', name='SumAllHeights', param_in='il', param_out='out',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=None,      # Use gen_tmp_dir,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description='DEM + GEOID height info projected on S2 tile',
+        )
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        """
+        Complete meta information with inputs, and
+        register temporary files from previous step for removal.
+        """
+        meta = super().complete_meta(meta, all_inputs)
+        meta['inputs'] = all_inputs
+        dem_on_s2  = fetch_input_data('in_s2_dem', all_inputs).out_filename
+        meta['files_to_remove'] = [dem_on_s2]  # DEM on S2
+        logger.debug('Register files to remove after height_on_S2 computation: %s', meta['files_to_remove'])
+        return meta
 
+    def _get_inputs(self, previous_steps: List[InputList]) -> InputList:
+        """
+        Extract the last inputs to use at the current level from all previous
+        products seens in the pipeline.
 
-class _StepWithOTBApplication(AbstractStep):
-    """
-    Internal intermediary type for `Steps` that have an application object.
-    Not meant to be used directly.
+        This method is overridden in order to fetch N-1 "in_s2_dem" input.
+        It has been specialized for S1Tiling exact pipelines.
+        """
+        assert len(previous_steps) > 1
 
-    Parent type for:
+        # "in_s2_geoid" is expected at level -1, likelly named '__last'
+        s2_geoid = fetch_input_data('__last', previous_steps[-1])
+        # "in_s2_dem"     is expected at level -2, likelly named 'in_s2_dem'
+        s2_dem   = fetch_input_data('in_s2_dem', previous_steps[-2])
 
-    - :class:`Step`  that will own the application
-    - and :class:`StoreStep` that will just reference the application from the previous step
-    """
-    def __init__(self, app, *argv, **kwargs):
-        """
-        Constructor.
-        """
-        # logger.debug("Create Step(%s, %s)", app, meta)
-        super().__init__(*argv, **kwargs)
-        self._app = app
-        self._out = None  # shall be overriden in child classes.
+        inputs = [{'in_s2_geoid': s2_geoid, 'in_s2_dem': s2_dem}]
+        _check_input_step_type(inputs)
+        logging.debug("%s inputs: %s", self.__class__.__name__, inputs)
+        return inputs
 
-    def __del__(self):
+    def _get_canonical_input(self, inputs: InputList) -> AbstractStep:
         """
-        Makes sure the otb app is released
+        Helper function to retrieve the canonical input associated to a list of inputs.
+
+        In current case, the canonical input comes from the "in_s2_geoid"
+        step instanciated in :func:`s1tiling.s1_process_lia` pipeline builder.
         """
-        if self._app:
-            self.release_app()
+        _check_input_step_type(inputs)
+        keys = set().union(*(input.keys() for input in inputs))
+        assert len(keys) == 2, f'Expecting 2 inputs. {len(inputs)} is/are found: {keys}'
+        assert 'in_s2_geoid' in keys
+        return [input['in_s2_geoid'] for input in inputs if 'in_s2_geoid' in input.keys()][0]
+
+    def parameters(self, meta: Meta) -> OTBParameters:
+        """
+        Returns the parameters to use with :external:doc:`BandMath OTB
+        application <Applications/app_BandMath>` for additionning DEM and Geoid
+        data projected on S2.
+        """
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        in_s2_dem   = fetch_input_data('in_s2_dem',   inputs).out_filename
+        in_s2_geoid = fetch_input_data('in_s2_geoid', inputs).out_filename
+        nodata = meta.get('nodata', -32768)
+        params : OTBParameters = {
+                'ram'         : ram(self.ram_per_process),
+                self.param_in : [in_s2_dem, in_s2_geoid],
+                'exp'         : f'im2b1 == {nodata} ? {nodata} : im1b1+im2b1'
+        }
+        return params
+
+
+class ComputeGroundAndSatPositionsOnDEM(OTBStepFactory):
+    """
+    Factory that prepares steps that run :external:doc:`Applications/app_SARDEMProjection`
+    as described in :ref:`Normals computation` documentation to obtain the XYZ
+    ECEF coordinates of the ground and of the satellite positions associated
+    to the pixel from input the `heigth` file.
+
+    :external:doc:`Applications/app_SARDEMProjection` application fill a
+    multi-bands image anchored on the footprint of the input DEM image.
+    In each pixel in the DEM/output image, we store the XYZ ECEF coordinate of
+    the ground point (associated to the pixel), and the XYZ coordinates of the
+    satellite position (associated to the pixel...)
+
+    Requires the following information from the configuration object:
+
+    - `ram_per_process`
+    - `dem_db_filepath`   -- to fill-up image metadata
+    - `dem_field_ids`     -- to fill-up image metadata
+    - `dem_main_field_id` -- to fill-up image metadata
+    - `tmp_dir`           -- useless in the in-memory nomical case
+    - `fname_fmt`         -- optional key: `ground_and_sat_s2`, useless in the in-memory nominal case
+
+    Requires the following information from the metadata dictionary
+
+    - `basename`
+    - `input filename`
+    - `output filename`
+    - `nodata` -- optional
+
+    It also requires :envvar:`$OTB_GEOID_FILE` to be set in order to ignore any
+    DEM information already registered in dask worker (through
+    :external:doc:`Applications/app_OrthoRectification` for instance) and only use
+    the Geoid.
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'XYZ_projected_on_{tile_name}_{orbit_direction}_{orbit}.tiff'
+        fname_fmt = cfg.fname_fmt.get('ground_and_sat_s2', fname_fmt)
+        super().__init__(
+                cfg,
+                appname='SARDEMProjection2', name='SARDEMProjection',
+                param_in=None, param_out='out',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=None,  # Use gen_tmp_dir
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description="XYZ ground and satellite positions on S2 tile",
+        )
+        self.__cfg = cfg  # Will be used to access cached DEM intersecting S2 tile
+
+    @staticmethod
+    def reduce_inputs(inputs: List[Meta]) -> List:
+        """
+        Filters which insar input will be kept.
+
+        Given several (usually 2 is the maximum) possible input S1 files
+        ("insar" input channels), select and return the one that maximize its
+        time coverage with the current S2 destination tile.
+
+        Actually, this function returns the first S1 image that time-covers
+        the whole S2 tile. The S1 images are searched in reverse order of
+        their footprint-coverage.
+        """
+        # Sort by coverages (already computed), then return the first that time-covers everything
+        # Or the first if none time-covers
+        sorted_inputs = sorted(inputs, key=lambda inp: inp['tile_coverage'], reverse=True)
+        best_covered_input = sorted_inputs[0]
+        logger.debug('Best coverage is %.2f%% at %s among:', best_covered_input['tile_coverage'], best_covered_input['acquisition_time'])
+        for inp in sorted_inputs:
+            logger.debug(' - %s: %.2f%%', inp['acquisition_time'], inp['tile_coverage'])
+        for inp in sorted_inputs:
+            product = out_filename(inp).replace("measurement", "annotation").replace(".tiff", ".xml")
+            az_start, az_stop, obt_start, obt_stop = Utils.get_s1image_orbit_time_range(product)
+            dt = az_stop - az_start
+            is_enough = (obt_start <= az_start - dt) and (az_stop + dt < obt_stop)
+            logger.debug(" - %s AZ: %s, OBT: %s: 2xAZ ∈ OBT: %s", os.path.dirname(inp['manifest']), [str(az_start), str(az_stop)], [str(obt_start), str(obt_stop)], is_enough)
+            if is_enough:
+                logger.debug(
+                        "Using %s which has orbit data that covers entirelly %s, and with a %.2f%% footprint coverage",
+                        out_filename(best_covered_input), best_covered_input['tile_name'], best_covered_input['tile_coverage']
+                )
+                return [inp]
+        logger.warning(
+                "None of the orbit state vector sequence from input S1 products seems wide enough to cover entirelly %s tile. Returning %s which has the best footprint coverage: %.2f%%",
+                best_covered_input['tile_name'], out_filename(best_covered_input), best_covered_input['tile_coverage']
+        )
+        return [best_covered_input]
+
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        """
+        Injects the :func:`reduce_inputs_insar` hook in step metadata, and
+        provide names clear from polar related information.
+        """
+        # Ignore polarization in filenames
+        if 'polarless_basename' in meta:
+            assert meta['polarless_basename'] == remove_polarization_marks(meta['basename'])
+        else:
+            meta['polarless_basename'] = remove_polarization_marks(meta['basename'])
 
-    def release_app(self):
-        # Only `Step` will delete, here we just reset the reference
-        self._app = None
+        meta['reduce_inputs_insar'] = ComputeGroundAndSatPositionsOnDEM.reduce_inputs
+        return meta
 
-    @property
-    def app(self):
+    def _update_filename_meta_post_hook(self, meta: Meta) -> None:
         """
-        OTB Application property.
+        Register ``accept_as_compatible_input`` hook for
+        :func:`s1tiling.libs.meta.accept_as_compatible_input`.
+        It will tell whether a given heights file on S2 tile input is
+        compatible with the current S2 tile.
         """
-        return self._app
-
-    @property
-    def is_first_step(self):
-        return self._app is None
+        meta['accept_as_compatible_input'] = lambda input_meta : does_s2_data_match_s2_tile(meta, input_meta)
 
-    @property
-    def param_out(self):
+    def _get_inputs(self, previous_steps: List[InputList]) -> InputList:
         """
-        Name of the "out" parameter used by the OTB Application.
-        Default is likely to be "out", while some applications use "io.out".
+        Extract the last inputs to use at the current level from all previous
+        products seens in the pipeline.
+
+        This method is overridden in order to fetch N-2 "insar" and "inheight" inputs.
+        It has been specialized for S1Tiling exact pipelines.
         """
-        return self._out
+        for i, st in enumerate(previous_steps):
+            logger.debug("INPUTS: %s previous step[%s] = %s", self.__class__.__name__, i, st)
 
+        inputs = [fetch_input_data_all_inputs({"insar", "inheight"}, previous_steps)]
+        _check_input_step_type(inputs)
+        logging.debug("%s inputs: %s", self.__class__.__name__, inputs)
+        return inputs
 
-class Step(_StepWithOTBApplication):
-    """
-    Interal specialized `Step` that holds a binding to an OTB Application.
+    def _get_canonical_input(self, inputs: InputList) -> AbstractStep:
+        assert inputs, "No inputs found in ComputeGroundAndSatPositionsOnDEM"
+        assert 'insar' in inputs[0], f"'insar' input is missing from ComputeGroundAndSatPositionsOnDEM inputs: {inputs[0].keys()}"
+        return inputs[0]['insar']
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        """
+        Computes dem information and adds them to the meta structure, to be used
+        later to fill-in the image metadata.
+
+        Also register temporary files from previous step for removal.
+        """
+        # logger.debug("ComputeGroundAndSatPositionsOnDEM inputs are: %s", all_inputs)
+        meta = super().complete_meta(meta, all_inputs)
+        meta['inputs'] = all_inputs
+        assert 'inputs' in meta, "Meta data shall have been filled with inputs"
+
+        # Cannot register height_on_s2 for ulterior removal as the file can be
+        # used with different orbits
+        # => TODO count how many XYZ files depend on the height_on_s2 file
+        # height_on_s2  = fetch_input_data('inheight', all_inputs)
+        # meta['files_to_remove'] = [height_on_s2.out_filename]
+        # logger.debug('Register files to remove after ground+satpos XYZ computation: %s', meta['files_to_remove'])
+
+        sar = fetch_input_data('insar', all_inputs).meta
+
+        # TODO: Check whether the DEM_LIST is already there and automatically propagated!
+        meta['dem_infos'] = self.__cfg.get_dems_covering_s2_tile(meta['tile_name'])
+        meta['dems'] = sorted(meta['dem_infos'].keys())
+
+        logger.debug("SARDEMProjection: DEM found for %s: %s", in_filename(sar), meta['dems'])
+        _, inbasename = os.path.split(in_filename(sar))
+        meta['inbasename'] = inbasename
+        return meta
 
-    The application binding is expected to be built by a dedicated :class:`StepFactory` and
-    passed to the constructor.
-    """
-    def __init__(self, app, *argv, **kwargs):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        constructor
+        Set SARDEMProjection related information that'll get carried around.
         """
-        # logger.debug("Create Step(%s, %s)", app, meta)
-        super().__init__(app, *argv, **kwargs)
-        self._out = kwargs.get('param_out', 'out')
+        super().update_image_metadata(meta, all_inputs)
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        imd['POLARIZATION']             = ""  # Clear polarization information (makes no sense here)
+        imd['DEM_LIST']                 = ', '.join(meta['dems'])
+        imd['band.DirectionToScanDEM*'] = ''
+        imd['band.Gain']                = ''
+
+    def parameters(self, meta: Meta) -> OTBParameters:
+        """
+        Returns the parameters to use with
+        :external:doc:`SARDEMProjection OTB application
+        <Applications/app_SARDEMProjection>` to project S1 geometry onto DEM tiles.
+        """
+        nodata = meta.get('nodata', -32768)
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        inheight = fetch_input_data('inheight', inputs).out_filename
+        insar    = fetch_input_data('insar'   , inputs).out_filename
+        # `elev.geoid='@'` tells SARDEMProjection2 that GEOID shall not be used
+        # from $OTB_GEOID_FILE, indeed geoid information is already in
+        # DEM+Geoid input.
+        return {
+                'ram'        : ram(self.ram_per_process),
+                'insar'      : insar,
+                'indem'      : inheight,
+                'elev.geoid' : '@',
+                'withcryz'   : False,
+                'withxyz'    : True,
+                'withsatpos' : True,
+                # 'withh'      : True,  # uncomment to analyse/debug height computed
+                'nodata'     : nodata
+        }
 
-    def release_app(self):
-        del self._app
-        super().release_app()  # resets self._app to None
+    def requirement_context(self) -> str:
+        """
+        Return the requirement context that permits to fix missing requirements.
+        SARDEMProjection2 comes from normlim_sigma0.
+        """
+        return "Please install https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0."
 
 
-def _check_input_step_type(inputs):
+class _ComputeNormals(OTBStepFactory):
     """
-    Internal helper function that checks :func:`StepFactory.create_step()`
-    ``inputs`` parameters is of the expected type, i.e.:
-    list of dictionaries {'key': :class:`AbstractStep`}
-    """
-    assert all(issubclass(type(inp), dict) for inp in inputs), f"Inputs not of expected type: {inputs}"
-    assert all(issubclass(type(step), AbstractStep) for inp in inputs for _, step in inp.items()), f"Inputs not of expected type: {inputs}"
+    Abstract factory that prepares steps that run
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    as described in :ref:`Normals computation <compute_normals-proc>` documentation.
 
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    computes surface normals.
 
-class StepFactory(ABC):
-    """
-    Abstract factory for :class:`Step`
+    Requires the following information from the configuration object:
 
-    Meant to be inherited for each possible OTB application or external
-    application used in a pipeline.
+    - `ram_per_process`
 
-    Sometimes we may also want to add some artificial steps that analyse
-    products, filenames..., or step that help filter products for following
-    pipelines.
+    Requires the following information from the metadata dictionary
 
-    See: `Existing processings`_
+    - input filename
+    - output filename
+    - `fname_fmt`  -- optional key: `normals`, useless in the in-memory nominal case
     """
-    def __init__(self, name, *unused_argv, **kwargs):  # pylint: disable=unused-argument
-        assert name
-        self._name               = name
-        self.__image_description = kwargs.get('image_description', None)
-        # logger.debug("new StepFactory(%s)", name)
+    def __init__(
+            self,
+            cfg               : Configuration,
+            gen_tmp_dir       : str,
+            output_fname_fmt  : str,
+            image_description : str,
+    ) -> None:
+        super().__init__(
+                cfg,
+                appname='ExtractNormalVector', name='ComputeNormals',
+                param_in='xyz', param_out='out',
+                gen_tmp_dir=gen_tmp_dir,
+                gen_output_dir=None,  # Use gen_tmp_dir
+                gen_output_filename=TemplateOutputFilenameGenerator(output_fname_fmt),
+                image_description=image_description,
+        )
 
-    @property
-    def name(self):
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
         """
-        Step Name property.
+        Injects ``polarless_basename`` -- Old LIA workflow case
         """
-        assert isinstance(self._name, str)
-        return self._name
+        # Ignore polarization in filenames
+        assert 'polarless_basename' in meta
+        assert meta['polarless_basename'] == remove_polarization_marks(meta['basename'])
+        return meta
 
-    @property
-    def image_description(self):
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
         """
-        Property image_description, used to fill ``TIFFTAG_IMAGEDESCRIPTION``
+        Override :func:`complete_meta()` to inject files to remove
         """
-        return self.__image_description
-
-    def check_requirements(self):
-        """
-        Abstract method used to test whether a :class:`StepFactory` has all
-        its external requirements fulfilled. For instance,
-        :class:`OTBStepFactory`'s will check their related OTB application can be executed.
+        meta = super().complete_meta(meta, all_inputs)
+        in_file = in_filename(meta)
+        meta['files_to_remove'] = [in_file]
+        logger.debug('Register files to remove after normals computation: %s', meta['files_to_remove'])
+        return meta
 
-        :return: ``None`` if  requirements are fulfilled.
-        :return: A message indicating what is missing otherwise, and some
-                 context how to fix it.
+    def parameters(self, meta: Meta) -> OTBParameters:
         """
-        return None
+        Returns the parameters to use with
+        :external:doc:`ExtractNormalVector OTB application
+        <Applications/app_ExtractNormalVector>` to generate surface normals
+        for each point of the origin S1 image.
+        """
+        nodata = meta.get('nodata', -32768)
+        xyz = in_filename(meta)
+        return {
+                'ram'             : ram(self.ram_per_process),
+                'xyz'             : xyz,
+                'nodata'          : float(nodata),
+        }
 
-    @abstractmethod
-    def build_step_output_filename(self, meta):
+    def requirement_context(self) -> str:
         """
-        Filename of the step output.
-
-        See also :func:`build_step_output_tmp_filename()` regarding the actual processing.
+        Return the requirement context that permits to fix missing requirements.
+        ComputeNormals comes from normlim_sigma0.
         """
-        pass
+        return "Please install https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0."
 
-    @abstractmethod
-    def build_step_output_tmp_filename(self, meta):
-        """
-        Returns a filename to a temporary file to use in output of the current application.
 
-        When an OTB (/External) application is harshly interrupted (crash or
-        user interruption), it leaves behind an incomplete (and thus invalid)
-        file.
-        In order to ignore those files when a pipeline is restarted, an
-        temporary filename is used by the application.
-        Once the application exits with success, the file will be renamed into
-        :func:`build_step_output_filename()`, and possibly moved into
-        :func:`_FileProducingStepFactory.output_directory()` if this is a final product.
-        """
-        pass
+class ComputeNormalsOnS2(_ComputeNormals):
+    """
+    Factory that prepares steps that run
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    on images in S2 geometry as described in :ref:`Normals
+    computation <compute_normals-proc>` documentation.
+
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    computes surface normals.
+
+    Requires the following information from the configuration object:
+
+    - `ram_per_process`
+
+    Requires the following information from the metadata dictionary
+
+    - input filename
+    - output filename
+    - `fname_fmt`  -- optional key: `normals_on_s2`, useless in the in-memory nominal case
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'Normals_on_{tile_name}'
+        fname_fmt = cfg.fname_fmt.get('normals_on_s2', fname_fmt)
+        super().__init__(
+                cfg,
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2'),
+                output_fname_fmt=fname_fmt,
+                image_description='Image normals on S2 grid',
+        )
+
+
+class _ComputeLIA(OTBStepFactory):
+    """
+    Abstract factory that prepares steps that run
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    as described in :ref:`LIA maps computation <compute_lia-proc>` documentation.
+
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    computes Local Incidende Angle Map.
+
+    Requires the following information from the configuration object:
+
+    - `ram_per_process`
+
+    Requires the following information from the metadata dictionary
+
+    - input filename
+    - output filename
+    """
+    def __init__(  # pylint: disable=too-many-arguments
+            self,
+            cfg               : Configuration,
+            fname_fmt_sin     : str,
+            fname_fmt_lia     : str,
+            gen_tmp_dir       : str,
+            gen_output_dir    : Optional[str],
+            image_description : str,
+    ) -> None:
+        fname_fmt          = [ TemplateOutputFilenameGenerator(fname_fmt_sin) ]
+        param_out          = ['out.sin']
+        extended_filenames = [ extended_filename_lia_sin(cfg) ]
+        pixel_types        = [ pixel_type(cfg, 'lia_sin') ]
+        if cfg.produce_lia_map:
+            # We always produce out.sin, and optionally we produce out.lia.
+            # Anyway, their production is always done in output_dir!
+            fname_fmt.append(TemplateOutputFilenameGenerator(fname_fmt_lia))
+            param_out.append('out.lia')
+            extended_filenames.append(extended_filename_lia_degree(cfg))
+            pixel_types.append(pixel_type(cfg, 'lia_deg', 'uint16'))
+        super().__init__(
+                cfg,
+                appname='SARComputeLocalIncidenceAngle', name='ComputeLIA',
+                param_in='in.normals',  # In-memory connected to in.normals
+                param_out=param_out,
+                gen_tmp_dir=gen_tmp_dir,
+                gen_output_dir=gen_output_dir,
+                gen_output_filename=OutputFilenameGeneratorList(fname_fmt),
+                image_description=image_description,
+                extended_filename=extended_filenames,
+                pixel_type=pixel_types,
+        )
 
-    def update_filename_meta(self, meta):  # to be overridden
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
         """
-        Duplicates, completes, and return, the `meta` dictionary with specific
-        information for the current factory regarding tasks analysis.
-
-        This method is used:
-
-        - while analysing the dependencies to build the task graph -- in this
-          use case the relevant information are the file names and paths.
-        - and indirectly before instanciating a new :class:`Step`
-
-        Other metadata not filled here:
-
-        - :func:`get_task_name` which is deduced from `out_filename`  by default
-        - :func:`out_extended_filename_complement`
-
-        It's possible to inject some other metadata (that could be used from
-        :func:`_get_canonical_input()` for instance) thanks to
-        :func:`_update_filename_meta_pre_hook()`.
+        Injects ``polarless_basename``.
         """
-        meta = meta.copy()
-        self._update_filename_meta_pre_hook(meta)
-        meta['in_filename']        = out_filename(meta)
-        meta['out_filename']       = self.build_step_output_filename(meta)
-        meta['out_tmp_filename']   = self.build_step_output_tmp_filename(meta)
-        meta['pipe']               = meta.get('pipe', []) + [self.__class__.__name__]
-        def check_product(meta):
-            filename        = out_filename(meta)
-            exist_file_name = os.path.isfile(filename)
-            logger.debug('Checking %s product: %s => %s',
-                    self.__class__.__name__,
-                    filename, '∃' if exist_file_name else '∅')
-            return exist_file_name
-        meta['does_product_exist'] = lambda : check_product(meta)
-        # meta['does_product_exist'] = lambda : os.path.isfile(out_filename(meta))
-        meta.pop('task_name',           None)
-        meta.pop('task_basename',       None)
-        meta.pop('update_out_filename', None)
-        meta.pop('is_compatible',       None)
-        # for k in list(meta.keys()):  # Remove all entries associated to reduce_* keys
-        #     if k.startswith('reduce_'):
-        #         del meta[k]
-        self._update_filename_meta_post_hook(meta)
+        assert 'polarless_basename' in meta
+        assert meta['polarless_basename'] == remove_polarization_marks(meta['basename'])
         return meta
 
-    def _update_filename_meta_pre_hook(self, meta):  # to be overridden  # pylint: disable=no-self-use
+    def _update_filename_meta_post_hook(self, meta: Meta) -> None:
         """
-        Hook meant to be overridden to complete product metadata before
-        they are used to produce filenames or tasknames.
-
-        Called from :func:`update_filename_meta()`
+        Override "does_product_exist" hook to take into account the multiple
+        output files produced by ComputeLIA
         """
-        return meta
+        meta['does_product_exist'] = lambda : all(os.path.isfile(of) for of in out_filename(meta))
 
-    def _update_filename_meta_post_hook(self, meta):  # to be overridden  # pylint: disable=no-self-use
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
         """
-        Hook meant to be overridden to fix product metadata by
-        overriding their default definition.
-
-        Called from :func:`update_filename_meta()`
+        Complete meta information with inputs
         """
+        meta = super().complete_meta(meta, all_inputs)
+        meta['inputs'] = all_inputs
         return meta
 
-    def complete_meta(self, meta, all_inputs):  # to be overridden  # pylint: disable=unused-argument
-        """
-        Duplicates, completes, and return, the `meta` dictionary with specific
-        information for the current factory regarding :class:`Step` instanciation.
-        """
-        meta.pop('out_extended_filename_complement', None)
-        return self.update_filename_meta(meta)
-
-    def update_image_metadata(self, meta, all_inputs):  # pylint: disable=unused-argument
-        """
-        Root implementation of :func:`update_image_metadata` that shall be
-        specialized in every file producing Step Factory.
+    def _get_inputs(self, previous_steps: List[InputList]) -> InputList:
         """
-        if 'image_metadata' not in meta:
-            meta['image_metadata'] = {}
-        imd = meta['image_metadata']
-        imd['TIFFTAG_DATETIME'] = str(datetime.datetime.now().strftime('%Y:%m:%d %H:%M:%S'))
-        if self.image_description:
-            imd['TIFFTAG_IMAGEDESCRIPTION'] = self.image_description.format(
-                    **meta,
-                    flying_unit_code_short=meta['flying_unit_code'][1:].upper())
+        Extract the last inputs to use at the current level from all previous
+        products seens in the pipeline.
 
-    def _get_inputs(self, previous_steps):  # pylint: disable=unused-argument,no-self-use
+        This method is overridden in order to fetch N-1 "xyz" input.
+        It has been specialized for S1Tiling exact pipelines.
         """
-        Extract the last inputs to use at the current level from all previous
-        products seen in the pipeline.
+        assert len(previous_steps) > 1
 
-        This method will need to be overridden in classes like
-        :class:`ComputeLIA` in order to fetch N-1 "xyz" input.
+        # "normals" is expected at level -1, likelly named '__last'
+        normals = fetch_input_data('__last', previous_steps[-1])
+        # "xyz"     is expected at level -2, likelly named 'xyz'
+        xyz = fetch_input_data('xyz', previous_steps[-2])
 
-        Postcondition:
-            :``_check_input_step_type(result)`` is True
-        """
-        # By default, simply return the last step information
-        assert len(previous_steps) > 0
-        inputs = previous_steps[-1]
+        inputs = [{'normals': normals, 'xyz': xyz}]
         _check_input_step_type(inputs)
         return inputs
 
-    def _get_canonical_input(self, inputs):
+    def parameters(self, meta: Meta) -> OTBParameters:
         """
-        Helper function to retrieve the canonical input associated to a list of inputs.
-        By default, if there is only one input, this will be the one returned.
-        Steps will multiple inputs will need to override this method.
+        Returns the parameters to use with
+        :external:doc:`SARComputeLocalIncidenceAngle OTB application
+        <Applications/app_SARComputeLocalIncidenceAngle>`.
+        """
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        xyz     = fetch_input_data('xyz', inputs).out_filename
+        normals = fetch_input_data('normals', inputs).out_filename
+        nodata  = meta.get('nodata', -32768)
+        return {
+                'ram'             : ram(self.ram_per_process),
+                'in.xyz'          : xyz,
+                'in.normals'      : normals,
+                'nodata'          : float(nodata),
+        }
 
-        Precondition:
-            :``_check_input_step_type(result)`` is True
+    def requirement_context(self) -> str:
         """
-        _check_input_step_type(inputs)
-        if len(inputs) == 1:
-            return list(inputs[0].values())[0]
-        else:
-            # If this error is raised, this means the current step has several
-            # inputs, we need to tell explicitely how the "main" input is found.
-            keys = set().union(*(input.keys() for input in inputs))
-            raise TypeError(f"No way to handle a multiple-inputs ({keys}) step from StepFactory: {self.__class__.__name__}")
-
-    def create_step(self, in_memory: bool, previous_steps):  # pylint: disable=unused-argument
+        Return the requirement context that permits to fix missing requirements.
+        ComputeLIA comes from normlim_sigma0.
         """
-        Instanciates the step related to the current :class:`StepFactory`,
-        that consumes results from the previous `input` steps.
-
-        1. This methods starts by updating metadata information through
-        :func:`complete_meta()` on the ``input`` metadatas.
+        return "Please install https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0."
 
-        2. in case the new step isn't related to an OTB application,
-        nothing specific is done, we'll just return an :class:`AbstractStep`
-
-        Note: While `previous_steps` is ignored in this specialization, it's
-        used in :func:`Store.create_step()` where it's eventually used to
-        release all OTB Application objects.
-        """
-        inputs = self._get_inputs(previous_steps)
-        inp    = self._get_canonical_input(inputs)
-        meta   = self.complete_meta(inp.meta, inputs)
-        self.update_image_metadata(meta, inputs) # Needs to be done after complete_meta!
 
-        # Return previous app?
-        return AbstractStep(**meta)
-
-
-class Pipeline:
+class ComputeLIAOnS2(_ComputeLIA):
     """
-    Pipeline of OTB applications.
+    Factory that prepares steps that run
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    on images in S2 geometry as described in :ref:`LIA maps computation <compute_lia-proc>` documentation.
 
-    It's instanciated as a list of :class:`AbstractStep` s.
-    :func:`Step.execute_and_write_output()` will be executed on the last step
-    of the pipeline.
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    computes Local Incidende Angle Map.
 
-    Internal class only meant to be used by :class:`PipelineDescriptionSequence`.
-    """
-    # Should we inherit from contextlib.ExitStack?
-    def __init__(self, do_measure, in_memory, do_watch_ram, name=None, dryrun=False, output=None):
-        self.__pipeline     = []
-        # self.__do_measure   = do_measure
-        self.__in_memory    = in_memory
-        self.__do_watch_ram = do_watch_ram
-        self.__dryrun       = dryrun
-        self.__name         = name
-        self.__output       = output
-        self.__inputs       = []
+    Requires the following information from the configuration object:
 
-    def __repr__(self):
-        return self.name
+    - `ram_per_process`
 
-    def set_inputs(self, inputs: list):
-        """
-        Set the input(s) of the instanciated pipeline.
-        The `inputs` is parameter expected to be a list of {'key': [metas...]} that'll
-        get tranformed into a dictionary of {'key': :class:`AbstractStep`}.
+    Requires the following information from the metadata dictionary
 
-        Some :class:`AbstractStep` will actually be :class:`MergeStep` instances.
-        """
-        logger.debug("Pipeline(%s).set_inputs(%s)", self.__name, inputs)
-        # all_keys = set().union(*(input.keys() for input in inputs))
-        all_keys = inputs.keys()
-        for key in all_keys:
-            # inputs_associated_to_key = [input[key] for input in inputs if key in input]
-            inputs_associated_to_key = inputs[key]
-            if len(inputs_associated_to_key) == 1:
-                self.__inputs.append({key: FirstStep(**inputs_associated_to_key[0])})
-            else:
-                self.__inputs.append({key: MergeStep(inputs_associated_to_key)})
-
-    @property
-    def _input_filenames(self):
-        """
-        Property _input_filenames
-        """
-        return [input[k].out_filename for input in self.__inputs for k in input]
-
-    @property
-    def appname(self):
-        """
-        Name of the pipeline application(s).
-        """
-        appname = (self.__name or '|'.join(crt.appname for crt in self.__pipeline))
-        return appname
+    - input filename
+    - output filename
+    - `fname_fmt`  -- optional key: `lia_product`
+    - `dname_fmt`  -- optional key: `lia_product`
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt0 = '{LIA_kind}_{flying_unit_code}_{tile_name}_{orbit_direction}_{orbit}.tif'
+        fname_fmt0 = cfg.fname_fmt.get('lia_product', fname_fmt0)
+        fname_fmt_lia = Utils.partial_format(fname_fmt0, LIA_kind="LIA")
+        fname_fmt_sin = Utils.partial_format(fname_fmt0, LIA_kind="sin_LIA")
+        dname_fmt = dname_fmt_lia_product(cfg)
+        super().__init__(
+                cfg,
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2'),
+                gen_output_dir=dname_fmt,
+                fname_fmt_lia=fname_fmt_lia,
+                fname_fmt_sin=fname_fmt_sin,
+                image_description='LIA on S2 grid',
+        )
 
-    @property
-    def name(self):
-        """
-        Name of the pipeline.
-        It's either user registered or automatically generated from the
-        registered :class:`StepFactory` s.
-        """
-        return f'{self.appname} -> {self.__output} from {self._input_filenames}'
 
-    @property
-    def output(self):
-        """
-        Expected pipeline final output file.
-        """
-        return self.__output
+class _FilterLIAStepFactory(StepFactory):
+    """
+    Helper root class for all LIA/sin filtering steps.
 
-    @property
-    def shall_watch_ram(self):
-        """
-        Tells whether objects in RAM shall be watched for memory leaks.
-        """
-        return self.__do_watch_ram
+    This class will be specialized on the fly by :func:`filter_LIA` which
+    will inject the static data ``_LIA_kind``.
 
-    def push(self, otbstep: StepFactory):
-        """
-        Registers a StepFactory into the pipeline.
-        """
-        assert isinstance(otbstep, StepFactory)
-        self.__pipeline.append(otbstep)
+    Related step will forward the selected input under a new task-name (that differs from the filename).
+    """
 
-    def check_requirements(self):
-        """
-        Check all the :class:`StepFactory`'s registered in the pipeline can be
-        exexuted.
+    # Useless definition used to trick pylint in believing self._LIA_kind is set.
+    # Indeed, it's expected to be set in child classes. But pylint has now way to know that.
+    _LIA_kind : Optional[str] = None
 
-        :return: ``None`` if requirements are fulfilled.
-        :return: A message indicating what is missing otherwise, and some
-                 context how to fix it.
+    def __init__(self, cfg: Configuration) -> None:
         """
-        sing_plur = {True: 'are', False: 'is'}
-        reqs = list(filter(None, (sf.check_requirements() for sf in self.__pipeline)))
-        missing_reqs = [rq for rq, _ in reqs]
-        contexts = set(ctx for _, ctx in reqs)
-        if reqs:
-            return f"{' and '.join(missing_reqs)} {sing_plur[len(missing_reqs) > 1]} required.", contexts
-        else:
-            return None
-
-    def do_execute(self):
+        Constructor.
+        Required to ignore the ``cfg`` parameter, and correctly forward the ``name`` parameter.
         """
-        Execute the pipeline.
+        super().__init__(self.__class__.__name__)
 
-        1. Makes sure the inputs exist -- unless in dry-run mode
-        2. Incrementaly create the steps of the pipeline.
-        3. Return the resulting output filename, or the caught errors.
-        """
-        assert self.__inputs
-        logger.info("INPUTS: %s", self.__inputs)
-        tested_files = list(Utils.flatten_stringlist(
-            [v.out_filename for inp in self.__inputs for _,v in inp.items()]))
-        logger.info("Testing whether input files exist: %s", tested_files)
-        missing_inputs = list(filterfalse(files_exist, tested_files))
-        if len(missing_inputs) > 0 and not self.__dryrun:
-            msg = f"Cannot execute {self} as the following input(s) {missing_inputs} do(es)n't exist"
-            logger.warning(msg)
-            return PipelineOutcome(RuntimeError(msg))
-        # logger.debug("LOG OTB: %s", os.environ.get('OTB_LOGGER_LEVEL'))
-        assert self.__pipeline  # shall not be empty!
-        steps = [self.__inputs]
-        for crt in self.__pipeline:
-            step = crt.create_step(self.__in_memory, steps)
-            if step:  # a StepFactory may return no step so it can be skipped
-                steps.append([{'__last': step}])
-
-        assert len(steps[-1]) == 1
-        res = steps[-1][0]['__last'].out_filename
-        assert res == self.output, \
-                f"Step output {self.output} doesn't match expected output {res}.\nThis is likely happenning because pipeline name generation isn't incremental."
-        steps = None
-        # logger.debug('Pipeline "%s" terminated -> %s', self, res)
-        return PipelineOutcome(res)
-
-
-# TODO: try to make it static...
-def execute4dask(pipeline, *args, **unused_kwargs):
-    """
-    Internal worker function used by Dask to execute a pipeline.
-
-    Returns the product filename(s) or the caught error in case of failure.
-    """
-    logger.debug('Parameters for %s: %s', pipeline, args)
-    watch_ram = pipeline.shall_watch_ram
-    if watch_ram:
-        objgraph.show_growth(limit=5)
-    try:
-        assert len(args) == 1
-        for arg in args[0]:
-            # logger.info('ARG: %s (%s)', arg, type(arg))
-            if isinstance(arg, PipelineOutcome) and not arg:
-                logger.warning('Cancel execution of %s because an error has occured upstream on a dependent input file: %s', pipeline, arg)
-                return copy.deepcopy(arg).add_related_filename(pipeline.output)
-        # Any exceptions leaking to Dask Scheduler would end the execution of the scheduler.
-        # That's why errors need to be caught and transformed here.
-        logger.info('Execute %s', pipeline)
-        res = pipeline.do_execute().add_related_filename(pipeline.output)
-        pipeline = None
-
-        if watch_ram:
-            objgraph.show_growth()
-
-            # all_objects = muppy.get_objects()
-            # sum1 = summary.summarize(all_objects)
-            # summary.print_(sum1)
-            w = get_worker()
-            if not hasattr(w, 'tracker'):
-                w.tr = tracker.SummaryTracker()
-            w.tr.print_diff()
-        return res
-    except Exception as ex:  # pylint: disable=broad-except  # Use in nominal code
-    # except RuntimeError as ex:  # pylint: disable=broad-except  # Use when debugging...
-        logger.exception('Execution of %s failed', pipeline)
-        logger.debug('(ERROR) %s has been executed with the following parameters: %s', pipeline, args)
-        return PipelineOutcome(ex).add_related_filename(pipeline.output).set_pipeline_name(pipeline.appname)
-
-
-class PipelineDescription:
-    """
-    Pipeline description:
-    - stores the various factory steps that describe a pipeline,
-    - can tell the expected product name given an input.
-    - tells whether its product is required
-    """
-    def __init__(self, factory_steps, dryrun, name=None, product_required=False,
-            is_name_incremental=False, inputs=None):
-        """
-        constructor
-        """
-        assert factory_steps  # shall not be None or empty
-        self.__factory_steps       = factory_steps
-        self.__is_name_incremental = is_name_incremental
-        self.__is_product_required = product_required
-        self.__dryrun              = dryrun
-        if name:
-            self.__name = name
-        else:
-            self.__name = '|'.join([step.name for step in self.__factory_steps])
-        assert inputs
-        self.__inputs              = inputs
-        # logger.debug("New pipeline: %s; required: %s, incremental: %s", '|'.join([step.name for step in self.__factory_steps]), self.__is_product_required, self.__is_name_incremental)
-
-    def expected(self, input_meta):
-        """
-        Returns the expected name of the product(s) of this pipeline
-        """
-        assert self.__factory_steps  # shall not be None or empty
-        try:
-            if self.__is_name_incremental:
-                res = input_meta
-                for step in self.__factory_steps:
-                    res = step.update_filename_meta(res)
-            else:
-                res = self.__factory_steps[-1].update_filename_meta(input_meta)
-            logger.debug("    expected: %s(%s) -> %s", self.__name, input_meta['out_filename'], out_filename(res))
-            return res
-        except CannotGenerateFilename as e:  # pylint: disable=broad-except
-            # logger.exception('expected(%s) rejected because', input_meta)
-            logger.debug('%s => rejecting expected(%s)', e, input_meta)
-            return None
-
-    @property
-    def inputs(self):
-        """
-        Property inputs
-        """
-        return self.__inputs
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        meta = super()._update_filename_meta_pre_hook(meta)
+        assert self._LIA_kind, "LIA kind should have been set in filter_LIA()"
+        meta['LIA_kind'] = self._LIA_kind
+        return meta
 
-    @property
-    def sources(self):
+    def _update_filename_meta_post_hook(self, meta: Meta) -> None:
         """
-        Property sources
+        Update task name to avoid collision with inputs as file aren't renamed by this filter.
         """
-        # logger.debug("SOURCES(%s) = %s", self.name, self.__inputs)
-        res = [(val if isinstance(val, str) else val.name) for (key,val) in self.__inputs.items()]
-        return res
+        meta['task_name']        = f'{out_filename(meta)}_FilterLIA'
 
-    @property
-    def name(self):
-        """
-        Descriptive name of the pipeline specification.
-        """
-        assert isinstance(self.__name, str)
-        return self.__name
+    def _get_input_image(self, meta: Meta) -> str:
+        # Flatten should be useless, but kept for better error messages
+        related_inputs = [f for f in Utils.flatten_stringlist(in_filename(meta))
+                if re.search(rf'\b{self._LIA_kind}_', f)]
+        assert len(related_inputs) == 1, (
+            f"Incorrect number ({len(related_inputs)}) of S1 LIA products of type '{self._LIA_kind}' in {in_filename(meta)} found: {related_inputs}"
+        )
+        return related_inputs[0]
 
-    @property
-    def product_is_required(self):
+    def build_step_output_filename(self, meta: Meta) -> str:
         """
-        Tells whether the product if this pipeline is required.
+        Forward the output filename.
         """
-        return self.__is_product_required
+        inp = self._get_input_image(meta)
+        logger.debug('%s KEEP %s from %s', self.__class__.__name__, inp, in_filename(meta))
+        return inp
 
-    def instanciate(self, file, do_measure, in_memory, do_watch_ram):
+    def build_step_output_tmp_filename(self, meta: Meta) -> str:
         """
-        Instanciates the pipeline specified.
-
-        Note: It systematically registers a :class:`Store` step at the end
-        if any :class:`StepFactory` is actually an :class:`OTBStepFactory`
-
-        Returns:
-            A :class:`Pipeline` instance
+        As there is no producer associated to :class:`_FilterLIAStepFactory`,
+        there is no temporary filename.
         """
-        pipeline = Pipeline(do_measure, in_memory, do_watch_ram, self.name, self.__dryrun, file)
-        need_OTB_store = False
-        for factory_step in self.__factory_steps + []:
-            pipeline.push(factory_step)
-            need_OTB_store = need_OTB_store or isinstance(factory_step, OTBStepFactory)  # TODO: use a dedicated function
-        if need_OTB_store:
-            pipeline.push(Store('noappname'))
-        return pipeline
-
-
-    def __repr__(self):
-        res = f'PipelineDescription: {self.name} ## Sources: {self.sources}'
-        return res
+        return self.build_step_output_filename(meta)
 
 
-def to_dask_key(pathname):
+def filter_LIA(LIA_kind: str) -> Type[_FilterLIAStepFactory]:
     """
-    Generate a simplified graph key name from a full pathname.
-    - Strip directory name
-    - Replace '-' with '_' as Dask has a special interpretation for '-' in key names.
+    Generates a new :class:`StepFactory` class that filters which LIA product
+    shall be processed: LIA maps or sin LIA maps.
     """
-    return pathname.replace('-', '_')
+    # We return a new class
+    return type(
+            f"Filter_{LIA_kind}",      # Class name
+            (_FilterLIAStepFactory,),  # Parent
+            { '_LIA_kind': LIA_kind}
+    )
 
 
-def register_task(tasks, key, value):
+class ApplyLIACalibration(OTBStepFactory):
     """
-    Register a task named `key` in the right format.
-    """
-    tasks[key] = value
-
+    Factory that concludes σ0 with NORMLIM calibration.
 
-def generate_first_steps_from_manifests(raster_list, tile_name, dryrun, debug_caches):
-    """
-    Flatten all rasters from the manifest as a list of :class:`FirstStep`
-    """
-    inputs = []
-    # Log commented and kept for filling in unit tests
-    # logger.debug('Generate first steps from: %s', raster_list)
-    # for raster, tile_origin in raster_list:
-    for raster_info in raster_list:
-        raster = raster_info['raster']  # Actually a S1DateAcquisition object...
+    It builds steps that multiply images calibrated with β0 LUT, and
+    orthorectified to S2 grid, with the sin(LIA) map for the same S2 tile (and
+    orbit number and direction).
 
-        manifest = raster.get_manifest()
-        for image in raster.get_images_list():
-            start = FirstStep(
-                    tile_name=tile_name,
-                    tile_origin=raster_info['tile_origin'],
-                    tile_coverage=raster_info['tile_coverage'],
-                    manifest=manifest,
-                    basename=image,
-                    dryrun=dryrun,
-                    debug_caches=debug_caches)
-            inputs.append(start.meta)
-    return inputs
+    Requires the following information from the configuration object:
 
+    - `ram_per_process`
 
-class TaskInputInfo:
-    """
-    Abstraction of the input(s) information associated to a particular task.
+    Requires the following information from the metadata dictionary
 
-    Used to merge, or to stack, information about inputs.
+    - input filename
+    - output filename
+    - flying_unit_code
+    - tile_name
+    - polarisation
+    - orbit_direction
+    - orbit
+    - acquisition_stamp
+    - `fname_fmt`  -- optional key: `s2_lia_corrected`
+    - `dname_fmt`  -- optional key: `tiled`
     """
-    def __init__(self, pipeline):
-        """
-        constructor
-        """
-        self.__pipeline     = pipeline
-        self._inputs        = {}  # map<source, meta / meta list>
-
-    def add_input(self, origin, input_meta, destination_meta):
-        """
-        Register a new input to the current task.
-
-        Parameters:
-            :origin:           Name of the source type the new input comes from
-            :input_meta:       Meta information associated to the new input (could be a list)
-            :destination_meta: Meta information associated to the current task
-
-        Several situations are possible:
-
-        - No input has been registered yet => simply register it
-        - If current task has a "reduce_inputs_{origin}" key in its meta
-          information, => use that function to filter which input is actually
-          kept.
-          This scenario is usefull in case several sets of inputs permit to
-          obtain a same product (e.g. when we don't actually need the data, but
-          only the geometry, etc).
-        - Otherwise, stack the new input with the previous ones.
-        """
-        if origin not in self._inputs:
-            logger.debug('    add_input[%s # %s]: first time <<-- %s', origin, out_filename(destination_meta), out_filename(input_meta))
-            self._inputs[origin] = [input_meta]
-            return True
-        logger.debug('add_input[%s # %s]: not empty <<-- %s', origin, out_filename(destination_meta), out_filename(input_meta))
-        logger.debug('check %s in %s', f'reduce_inputs_{origin}', destination_meta.keys())
-        if f'reduce_inputs_{origin}' in destination_meta.keys():
-            # logger.debug('add_input[%s]: self.__inputs[%s]= %s <--- %s', origin, origin, self._inputs[origin], destination_meta[f'reduce_inputs_{origin}'](self._inputs[origin] + [input_meta]))
-            self._inputs[origin] = destination_meta[f'reduce_inputs_{origin}'](
-                    self._inputs[origin] + [input_meta])
-            return False
-        else:
-            self._inputs[origin].append(input_meta)
-            return True
 
-    @property
-    def pipeline(self):
+    def __init__(self, cfg: Configuration) -> None:
         """
-        Property pipeline
+        Constructor.
         """
-        return self.__pipeline
+        fname_fmt = '{flying_unit_code}_{tile_name}_{polarisation}_{orbit_direction}_{orbit}_{acquisition_stamp}_NormLim.tif'
+        fname_fmt = cfg.fname_fmt.get('s2_lia_corrected', fname_fmt)
+        dname_fmt = dname_fmt_tiled(cfg)
+        super().__init__(
+                cfg,
+                appname='BandMath', name='ApplyLIACalibration', param_in='il', param_out='out',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=dname_fmt,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description='Sigma0 Normlim Calibrated Sentinel-{flying_unit_code_short} IW GRD',
+                extended_filename=extended_filename_tiled(cfg),
+                pixel_type=pixel_type(cfg, 'tiled'),
+        )
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        """
+        Complete meta information with inputs, and set compression method to
+        DEFLATE.
+        """
+        meta = super().complete_meta(meta, all_inputs)
+        meta['inputs']           = all_inputs
+        meta['calibration_type'] = 'Normlim'  # Update meta from now on
+
+        # As of v1.1, when S2 product is marked required iff calibration_is_done_in_S1,
+        # IOW, it's not required in normlim case, and we can safely remove the calibrated β0 file.
+        in_concat_S2 = fetch_input_data('concat_S2', all_inputs).out_filename
+        meta['files_to_remove'] = [in_concat_S2]
+        return meta
 
-    @property
-    def inputs(self):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        Inputs associated to the task.
-
-        It's organized as a dictionary that associates a source type to a meta or a list of meta
-        information.
+        Set σ° normlim calibration related information that'll get carried around.
         """
-        return self._inputs
+        super().update_image_metadata(meta, all_inputs)
+        inputs = meta['inputs']
+        in_sin_LIA   = fetch_input_data('sin_LIA',   inputs).out_filename
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        imd['CALIBRATION'] = meta['calibration_type']
+        imd['LIA_FILE']    = os.path.basename(in_sin_LIA)
 
-    @property
-    def input_task_names(self):
-        """
-        List of input tasks the current task depends on.
+    def _get_canonical_input(self, inputs: InputList) -> AbstractStep:
         """
-        tns = [get_task_name(meta) for meta in self.input_metas]
-        logger.debug('input_task_names(%s) --> %s', self.pipeline.name, tns)
-        return tns
+        Helper function to retrieve the canonical input associated to a list of inputs.
 
-    @property
-    def input_metas(self):
-        """
-        List of input meta informations the current task depends on.
+        In current case, the canonical input comes from the "concat_S2"
+        pipeline defined in :func:`s1tiling.s1_process` pipeline builder.
         """
-        metas = [meta for inputs in self.inputs.values() for meta in inputs]
-        return metas
+        _check_input_step_type(inputs)
+        keys = set().union(*(input.keys() for input in inputs))
+        assert len(inputs) == 2, f'Expecting 2 inputs. {len(inputs)} are found: {keys}'
+        assert 'concat_S2' in keys
+        return [input['concat_S2'] for input in inputs if 'concat_S2' in input.keys()][0]
+
+    def _update_filename_meta_post_hook(self, meta: Meta) -> None:
+        """
+        Register ``accept_as_compatible_input`` hook for
+        :func:`s1tiling.libs.meta.accept_as_compatible_input`.
+        It will tell whether a given sin_LIA input is compatible with the
+        current S2 tile.
+        """
+        meta['accept_as_compatible_input'] = lambda input_meta : does_sin_lia_match_s2_tile_for_orbit(meta, input_meta)
+        meta['basename']                   = self._get_nominal_output_basename(meta)
+        meta['calibration_type']           = 'Normlim'
+
+    def parameters(self, meta: Meta) -> OTBParameters:
+        """
+        Returns the parameters to use with :external:doc:`BandMath OTB application
+        <Applications/app_BandMath>` for applying sin(LIA) to β0 calibrated
+        image orthorectified to S2 tile.
+        """
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        in_concat_S2 = fetch_input_data('concat_S2', inputs).out_filename
+        in_sin_LIA   = fetch_input_data('sin_LIA',   inputs).out_filename
+        nodata = meta.get('nodata', -32768)
+        params : OTBParameters = {
+                'ram'         : ram(self.ram_per_process),
+                self.param_in : [in_concat_S2, in_sin_LIA],
+                'exp'         : f'im2b1 == {nodata} ? {nodata} : im1b1*im2b1'
+        }
+        return params
 
-    def __repr__(self):
-        res = 'TaskInputInfo:\n- inputs:\n'
-        for k, inps in self.inputs.items():
-            res += f'  - "{k}":\n'
-            for val in inps:
-                res += f'    - {val}\n'
-        res += f'- pipeline: {self.pipeline}\n'
-        return res
 
+# ======================================================================
+# Deprecated wrappers.
+# They were used in S1Tiling 1.0 when the worflow was done in S1 SAR geometry
+# until the production of the LIA map that was eventuall orthorectified and
+# concatenated.
 
-def _update_out_filename(updated_meta, with_meta):
+class AgglomerateDEMOnS1(AnyProducerStepFactory):
     """
-    Helper function to update the `out_filename` from metadata.
-    Meant to be used metadata associated to products made of several inputs
-    like Concatenate.
-    """
-    if 'update_out_filename' in updated_meta:
-        updated_meta['update_out_filename'](updated_meta, with_meta)
-
-
-def _register_new_input_and_update_out_filename(
-        tasks: list,  #: list[TaskInputInfo],  # Require Python 3.7+ ?
-        origin, input_meta, new_task_meta, outputs
-        ):
-    """
-    Helper function to register a new input to a :class:`TaskInputInfo` and
-    update the current task output filename if required.
-    """
-    task_name = get_task_name(new_task_meta)
-    if isinstance(task_name, list):
-        # TODO: correctly handle the case a task produce several filenames
-        task_name = task_name[0]
-    task_inputs = tasks[task_name]
-    if task_inputs.add_input(origin, input_meta, new_task_meta):
-        logger.debug('    The %s task depends on one more input, updating its metadata to reflect the situation.\nUpdating %s ...', task_name, new_task_meta)
-        _update_out_filename(new_task_meta, task_inputs)
-        logger.debug('    ...to (%s)', new_task_meta)
-        already_registered_next_input = [ni for ni in outputs if get_task_name(ni) == task_name]
-        assert len(already_registered_next_input) == 1, \
-                f'{len(already_registered_next_input)} != 1 => {already_registered_next_input}'
-        _update_out_filename(already_registered_next_input[0], task_inputs)
-        # Can't we simply override the already_registered_next_input with expected fields?
-        already_registered_next_input[0].update(new_task_meta)
-    else:
-        logger.debug('    The %s task depends on one more input, but only one will be kept.\n    %s has been updated.', task_name, new_task_meta)
-
+    Factory that produces a :class:`Step` that builds a VRT from a list of DEM files.
 
-class PipelineDescriptionSequence:
+    The choice has been made to name the VRT file after the basename of the
+    root S1 product and not the names of the DEM tiles.
     """
-    This class is the main entry point to describe pipelines.
 
-    Internally, it can be seen as a list of :class:`PipelineDescription` objects.
-    """
-    def __init__(self, cfg, dryrun, debug_caches):
+    def __init__(self, cfg: Configuration, *args, **kwargs) -> None:
         """
         constructor
         """
-        assert cfg
-        self.__cfg          = cfg
-        self.__pipelines    = []
-        self.__dryrun       = dryrun
-        self.__debug_caches = debug_caches
-
-    def register_pipeline(self, factory_steps, *args, **kwargs):
-        """
-        Register a pipeline description from:
-
-        Parameters:
-            :factory_steps:       List of non-instanciated :class:`StepFactory` classes
-            :name:                Optional name for the pipeline
-            :product_required:    Tells whether the pipeline product is expected as a
-                                  final product
-            :is_name_incremental: Tells whether `expected` filename needs evaluations of
-                                  each intermediary steps of whether it can be directly
-                                  deduced from the last step.
-        """
-        steps = [FS(self.__cfg) for FS in factory_steps]
-        assert 'dryrun' not in kwargs
-        if 'inputs' not in kwargs:
-            # Register the last pipeline as 'in' if nothing is specified
-            kwargs['inputs'] = {'in' : self.__pipelines[-1] if self.__pipelines else 'basename'}
-        pipeline = PipelineDescription(steps, self.__dryrun, *args, **kwargs)
-        logger.debug('--> Register pipeline %s as %s', pipeline.name, [fs.__name__ for fs in factory_steps])
-        self.__pipelines.append(pipeline)
-        return pipeline
-
-    def _build_dependencies(self, tile_name, raster_list):
-        """
-        Runs the inputs through all pipeline descriptions to build the full list
-        of intermediary and final products and what they require to be built.
-        """
-        first_inputs = generate_first_steps_from_manifests(
-                tile_name=tile_name,
-                raster_list=raster_list,
-                dryrun=self.__dryrun,
-                debug_caches=self.__debug_caches)
-
-        pipelines_outputs = {'basename': first_inputs}  # TODO: find the right name _0/__/_firststeps/...?
-        logger.debug('FIRST: %s', pipelines_outputs['basename'])
-
-        required = {}  # (first batch) Final products identified as _needed to be produced_
-        previous = {}  # Graph of deps: for a product tells how it's produced (pipeline + inputs): Map<TaskInputInfo>
-        task_names_to_output_files_table = {}
-        # +-> TODO: cache previous in order to remember which files already exists or not
-        #     the difficult part is to flag as "generation successful" or not
-        for pipeline in self.__pipelines:
-            logger.debug('#############################################################################')
-            logger.debug('#############################################################################')
-            logger.debug('Analysing |%s| dependencies', pipeline.name)
-            logger.debug('Sources --> %s', pipeline.sources)
-            outputs = []
-
-            dropped_inputs = {}
-            for origin, sources in pipeline.inputs.items():
-                source_name = sources if isinstance(sources, str) else sources.name
-                logger.debug('===========================================================================')
-                logger.debug('* Checking sources from "%s" origin: %s', origin, source_name)
-                # Locate all inputs for the current pipeline
-                # -> Select all inputs for pipeline sources from pipelines_outputs
-                inputs = [output for output in pipelines_outputs[source_name]]
-
-                logger.debug('  FROM all %s inputs as "%s": %s', len(inputs), origin, [out_filename(i) for i in inputs])
-                dropped = []
-                for input in inputs:  # inputs are meta
-                    logger.debug('  ----------------------------------------------------------------------')
-                    logger.debug('  - GIVEN "%s" "%s": %s', origin, out_filename(input), input)
-                    expected = pipeline.expected(input)
-                    if not expected:
-                        logger.debug("    No '%s' product can be generated from '%s' input '%s' ==> Ignore for now",
-                                pipeline.name, origin, out_filename(input))
-                        dropped.append(input)  # remember that source/input will be used differently
-                        continue
-                    expected_taskname = get_task_name(expected)
-                    logger.debug('    %s <-- from input: %s', expected_taskname, out_filename(input))
-                    logger.debug('    --> "%s": %s', out_filename(expected), expected)
-                    # TODO: Correctly handle the case where a task produce
-                    # several filenames. In that case we shall have only one
-                    # task, but possibly, several following tasks may depend on
-                    # the current task.
-                    # For the moment, just keep the first, and use product
-                    # selection pattern as in filter_LIA().
-                    if isinstance(expected_taskname, list):
-                        expected_taskname = expected_taskname[0] # TODO: see comment above
-
-                    # We cannot analyse early whether a task product is already
-                    # there as some product have names that depend on all
-                    # inputs (see Concatenate).
-                    # This is why the full dependencies tree is produced at
-                    # this time. Unrequired parts will be trimmed in the next
-                    # task producing step.
-                    if expected_taskname not in previous:
-                        outputs.append(expected)
-                        previous[expected_taskname] = TaskInputInfo(pipeline=pipeline)
-                        previous[expected_taskname].add_input(origin, input, expected)
-                        logger.debug('    This is a new product: %s, with a source from "%s"', expected_taskname, origin)
-                    elif get_task_name(input) not in previous[expected_taskname].input_task_names:
-                        _register_new_input_and_update_out_filename(
-                                tasks=previous,
-                                origin=origin,
-                                input_meta=input,
-                                new_task_meta=expected,
-                                outputs=outputs)
-                    if pipeline.product_is_required:
-                        # assert (expected_taskname not in required) or (required[expected_taskname] == expected)
-                        required[expected_taskname] = expected
-                    task_names_to_output_files_table[expected_taskname] = out_filename(expected)
-                # endfor input in inputs:  # inputs are meta
-                if dropped:
-                    dropped_inputs[origin] = dropped
-            # endfor origin, sources in pipeline.inputs.items():
-
-            # For all new outputs, check which dropped inputs would be compatible
-            logger.debug('* Checking dropped inputs: %s', dropped_inputs.keys())
-            for output in outputs:
-                for origin, inputs in dropped_inputs.items():
-                    for input in inputs:
-                        logger.debug("  - Is '%s' a '%s' input for '%s' ?", out_filename(input), origin, out_filename(output))
-                        if _is_compatible(output, input):
-                            logger.debug('    => YES')
-                            _register_new_input_and_update_out_filename(
-                                    tasks=previous,
-                                    origin=origin,
-                                    input_meta=input,
-                                    new_task_meta=output,
-                                    outputs=outputs)
-                        else:
-                            logger.debug('  => NO')
-
-            pipelines_outputs[pipeline.name] = outputs
-
-        logger.debug('#############################################################################')
-        logger.debug('#############################################################################')
-        required_task_names = set()
-        for name, meta in required.items():
-            logger.debug("check task_name: %s", name)
-            if product_exists(meta):
-                logger.debug("Ignoring %s as the product already exists", name)
-                previous[name] = False  # for the next log
-            else:
-                required_task_names.add(name)
-
-        logger.debug("Dependencies found:")
-        for task_name, prev in previous.items():
-            if prev:
-                logger.debug('- %s requires %s on %s', task_name, prev.pipeline.name, [out_filename(i) for i in prev.input_metas])
-            else:
-                logger.debug('- %s already exists, no need to produce it', task_name)
-        return required_task_names, previous, task_names_to_output_files_table
-
-    def _build_tasks_from_dependencies(self,
-            required, previous, task_names_to_output_files_table,
-            do_watch_ram):  # pylint: disable=no-self-use
-        """
-        Generates the actual list of tasks for :func:`dask.client.get()`.
-
-        `previous` is made of:
-        - "pipeline": reference to the :class:`PipelineDescription`
-        - "inputs": list of the inputs (metadata)
-        """
-        tasks = {}
-        logger.debug('#############################################################################')
-        logger.debug('#############################################################################')
-        logger.debug('Building all tasks')
-        while required:
-            new_required = set()
-            for task_name in required:
-                assert previous[task_name]
-                base_task_name = to_dask_key(task_name)
-                task_inputs    = previous[task_name].inputs
-                pipeline_descr = previous[task_name].pipeline
-                first = lambda files : files[0] if isinstance(files, list) else  files
-                input_task_keys = [to_dask_key(first(tn))
-                        for tn in previous[task_name].input_task_names]
-                assert list(input_task_keys)
-                logger.debug('* %s(%s) --> %s', task_name, list(input_task_keys), task_inputs)
-                output_filename = task_names_to_output_files_table[task_name]
-                pipeline_instance = pipeline_descr.instanciate(
-                        output_filename, True, True, do_watch_ram)
-                pipeline_instance.set_inputs(task_inputs)
-                logger.debug('  ~~> TASKS[%s] += %s(keys=%s)', base_task_name, pipeline_descr.name, list(input_task_keys))
-                register_task(
-                        tasks, base_task_name, (execute4dask, pipeline_instance, input_task_keys))
-
-                for t in previous[task_name].input_metas:  # TODO: check whether the inputs need to be produced as well
-                    tn = first(get_task_name(t))
-                    logger.debug('  Processing task %s: %s', tn, t)
-                    if not product_exists(t):
-                        logger.info('    => Need to register production of %s (for %s)', tn, pipeline_descr.name)
-                        new_required.add(tn)
-                    else:
-                        logger.info('    => Starting %s from existing %s', pipeline_descr.name, tn)
-                        register_task(tasks, to_dask_key(tn), FirstStep(**t))
-            required = new_required
-        return tasks
-
-    def _check_static_task_requirements(self, tasks):
-        """
-        Check all tasks have their requirement fulfilled for being generated.
-        Typically that the related applications are installed and can be
-        executed.
-
-        If any requirement is missing, the execution is stopped.
-        :todo: throw an exception instead of existing the process. See #96
-        """
-        logger.debug('#############################################################################')
-        logger.debug('#############################################################################')
-        logger.debug('Checking tasks static dependencies')
-        missing_apps = {}
-        contexts = set()
-        for key, task in tasks.items():
-            if isinstance(task, tuple):
-                assert isinstance(task[1], Pipeline)
-                req_ctx = task[1].check_requirements()
-                if req_ctx:
-                    req, ctx = req_ctx
-                    if req not in missing_apps:
-                        missing_apps[req] = []
-                    missing_apps[req].append(key)
-                    contexts.update(ctx)
-            else:
-                assert isinstance(task, FirstStep)
-        if missing_apps:
-            logger.error('Cannot execute S1Tiling because of the following reason(s):')
-            for req, task_keys in missing_apps.items():
-                logger.error("- %s for %s", req, task_keys)
-            for ctx in contexts:
-                logger.error(" -> %s", ctx)
-            sys.exit(exits.MISSING_APP)
-        else:
-            logger.debug('All required applications are correctly available')
-
+        fname_fmt = 'DEM_{polarless_rootname}.vrt'
+        fname_fmt = cfg.fname_fmt.get('dem_s1_agglomeration', fname_fmt)
+        super().__init__(  # type: ignore # mypy issue 4335
+            cfg,
+            gen_tmp_dir=os.path.join(cfg.tmpdir, 'S1'),
+            gen_output_dir=None,      # Use gen_tmp_dir,
+            gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+            name="AgglomerateDEMOnS1",
+            action=AgglomerateDEMOnS1.agglomerate,
+            *args, **kwargs)
+        self.__dem_db_filepath     = cfg.dem_db_filepath
+        self.__dem_dir             = cfg.dem
+        self.__dem_filename_format = cfg.dem_filename_format
+        self.__dem_field_ids       = cfg.dem_field_ids
+        self.__dem_main_field_id   = cfg.dem_main_field_id
 
-    def generate_tasks(self, tile_name, raster_list, do_watch_ram=False):
+    @staticmethod
+    def agglomerate(parameters: ExeParameters, dryrun: bool) -> None:
         """
-        Generate the minimal list of tasks that can be passed to Dask
-
-        Parameters:
-            :tile_name:   Name of the current S2 tile
-            :raster_list: List of rasters that intersect the tile.
-
-        TODO: Move into another dedicated class instead of PipelineDescriptionSequence
+        The function that calls :func:`gdal.BuildVRT()`.
         """
-        required, previous, task_names_to_output_files_table = self._build_dependencies(
-                tile_name=tile_name,
-                raster_list=raster_list)
-
-        # Generate the actual list of tasks
-        final_products = [to_dask_key(p) for p in required]
-        tasks = self._build_tasks_from_dependencies(
-                required=required,
-                previous=previous,
-                task_names_to_output_files_table=task_names_to_output_files_table,
-                do_watch_ram=do_watch_ram)
-        self._check_static_task_requirements(tasks)
-
-        for final_product in final_products:
-            assert final_product in tasks
-        return tasks, final_products
-
-
-# ======================================================================
-# Some specific steps
-class FirstStep(AbstractStep):
-    """
-    First Step:
-
-    - no application executed
-    """
-    def __init__(self, *argv, **kwargs):
-        super().__init__(*argv, **kwargs)
-        if 'out_filename' not in self._meta:
-            # If not set through the parameters, set it from the basename + out dir
-            self._meta['out_filename'] = self._meta['basename']
-        _, basename = os.path.split(self._meta['basename'])
-        self._meta['basename'] = basename
-        self._meta['pipe'] = [self._meta['out_filename']]
-
-    def __str__(self):
-        return f'FirstStep{self._meta}'
-
-    def __repr__(self):
-        return f'FirstStep{self._meta}'
+        logger.info("gdal.BuildVRT(%s, %s)", parameters[0], parameters[1:])
+        assert len(parameters) > 0
+        if not dryrun:
+            gdal.BuildVRT(parameters[0], parameters[1:])
 
-    @property
-    def input_metas(self):
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
         """
-        Specific to :class:`MergeStep` and :class:`FirstStep`: returns the
-        metas from the inputs as a list.
+        Injects the :func:`reduce_inputs_insar` hook in step metadata, and
+        provide names clear from polar related information.
         """
-        return [self._meta]
-
-
-class MergeStep(AbstractStep):
-    """
-    Kind of FirstStep that merges the result of one or several other steps
-    of same kind.
-
-    Used in input of :class:`Concatenate`
-
-    - no application executed
-    """
-    def __init__(self, input_steps_metas, *argv, **kwargs):
-        # meta = {**(input_steps_metas[0]._meta), **kwargs}  # kwargs override step0.meta
-        meta = {**(input_steps_metas[0]), **kwargs}  # kwargs override step0.meta
-        super().__init__(*argv, **meta)
-        self.__input_steps_metas = input_steps_metas
-        self._meta['out_filename'] = [out_filename(s) for s in input_steps_metas]
-
-    def __str__(self):
-        return f'MergeStep{self.__input_steps_metas}'
-
-    def __repr__(self):
-        return f'MergeStep{self.__input_steps_metas}'
+        # Ignore polarization in filenames
+        assert 'polarless_basename' not in meta
+        meta['polarless_basename'] = remove_polarization_marks(meta['basename'])
+        rootname = os.path.splitext(meta['polarless_basename'])[0]
+        meta['polarless_rootname'] = rootname
+        meta['reduce_inputs_insar'] = lambda inputs : [inputs[0]]  # TODO!!!
+        return meta
 
-    @property
-    def input_metas(self):
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
         """
-        Specific to :class:`MergeStep` and :class:`FirstStep`: returns the
-        metas from the inputs as a list.
+        Factory that takes care of extracting meta data from S1 input files.
         """
-        return self.__input_steps_metas
+        meta = super().complete_meta(meta, all_inputs)
+        # find DEMs that intersect the input image
+        meta['dem_infos'] = Utils.find_dem_intersecting_raster(
+            in_filename(meta), self.__dem_db_filepath, self.__dem_field_ids, self.__dem_main_field_id)
+        meta['dems'] = sorted(meta['dem_infos'].keys())
+        logger.debug("DEM found for %s: %s", in_filename(meta), meta['dems'])
+        dem_files = map(
+                lambda s: os.path.join(self.__dem_dir, self.__dem_filename_format.format_map(meta['dem_infos'][s])),
+                meta['dem_infos'])
+        missing_dems = list(filter(lambda f: not os.path.isfile(f), dem_files))
+        if len(missing_dems) > 0:
+            raise RuntimeError(
+                    f"Cannot create DEM vrt for {meta['polarless_rootname']}: the following DEM files are missing: {', '.join(missing_dems)}")
+        return meta
 
+    def parameters(self, meta: Meta) -> ExeParameters:
+        # While it won't make much a difference here, we are still using tmp_filename.
+        return [tmp_filename(meta)] \
+                + [os.path.join(self.__dem_dir,
+                                self.__dem_filename_format.format_map(meta['dem_infos'][s]))
+                   for s in meta['dem_infos']]
+
+
+class SARDEMProjection(OTBStepFactory):
+    """
+    Factory that prepares steps that run :external:doc:`Applications/app_SARDEMProjection`
+    as described in :ref:`Normals computation` documentation.
+
+    :external:doc:`Applications/app_SARDEMProjection` application puts a DEM file
+    into SAR geometry and estimates two additional coordinates.
+    For each point of the DEM input four components are calculated:
+    C (colunm into SAR image), L (line into SAR image), Z and Y. XYZ cartesian
+    components into projection are also computed for our needs.
+
+    Requires the following information from the configuration object:
+
+    - `ram_per_process`
+    - `dem_db_filepath`   -- to fill-up image metadata
+    - `dem_field_ids`     -- to fill-up image metadata
+    - `dem_main_field_id` -- to fill-up image metadata
+    - `tmp_dir`           -- useless in the in-memory nomical case
+    - `fname_fmt`         -- optional key: `s1_on_dem`, useless in the in-memory nominal case
+
+    Requires the following information from the metadata dictionary
+
+    - `basename`
+    - `input filename`
+    - `output filename`
+    - `nodata` -- optional
+
+    It also requires :envvar:`$OTB_GEOID_FILE` to be set in order to ignore any
+    DEM information already registered in dask worker (through
+    :external:doc:`Applications/app_OrthoRectification` for instance) and only use
+    the Geoid.
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'S1_on_DEM_{polarless_basename}'
+        fname_fmt = cfg.fname_fmt.get('s1_on_dem', fname_fmt)
+        super().__init__(
+                cfg,
+                appname='SARDEMProjection2', name='SARDEMProjection',
+                param_in=None, param_out='out',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S1'),
+                gen_output_dir=None,  # Use gen_tmp_dir
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description="SARDEM projection onto DEM list",
+        )
+        self.__dem_db_filepath     = cfg.dem_db_filepath
+        self.__dem_field_ids       = cfg.dem_field_ids
+        self.__dem_main_field_id   = cfg.dem_main_field_id
+
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        """
+        Injects the :func:`reduce_inputs_insar` hook in step metadata, and
+        provide names clear from polar related information.
+        """
+        # Ignore polarization in filenames
+        if 'polarless_basename' in meta:
+            assert meta['polarless_basename'] == remove_polarization_marks(meta['basename'])
+        else:
+            meta['polarless_basename'] = remove_polarization_marks(meta['basename'])
 
-class StoreStep(_StepWithOTBApplication):
-    """
-    Artificial Step that takes care of executing the last OTB application in the
-    pipeline.
-    """
-    def __init__(self, previous: Step):
-        assert not previous.is_first_step
-        super().__init__(previous._app, *[], **previous.meta)
-        self._out = previous.param_out
+        meta['reduce_inputs_insar'] = lambda inputs : [inputs[0]]  # TODO!!!
+        return meta
 
-    @property
-    def tmp_filename(self):
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
         """
-        Property that returns the name of the file produced by the current step while
-        the OTB application is running.
-        Eventually, it'll get renamed into `self.out_filename` if the application
-        succeeds.
-        """
-        return tmp_filename(self.meta)
-
-    @property
-    def shall_store(self):
-        return True
+        - Complete meta information with hook for updating image metadata
+          w/ directiontoscandemc, directiontoscandeml and gain.
+        - Computes dem information and add them to the meta structure, to be used
+          later to fill-in the image metadata.
+        """
+        meta = super().complete_meta(meta, all_inputs)
+        append_to(meta, 'post', self.add_image_metadata)
+        assert 'inputs' in meta, "Meta data shall have been filled with inputs"
+        # meta['inputs'] = all_inputs
+
+        # TODO: The following has been duplicated from AgglomerateDEM.
+        # See to factorize this code
+        # find DEMs that intersect the input image
+        meta['dem_infos'] = Utils.find_dem_intersecting_raster(
+            in_filename(meta), self.__dem_db_filepath, self.__dem_field_ids, self.__dem_main_field_id)
+        meta['dems'] = sorted(meta['dem_infos'].keys())
+
+        logger.debug("SARDEMProjection: DEM found for %s: %s", in_filename(meta), meta['dems'])
+        _, inbasename = os.path.split(in_filename(meta))
+        meta['inbasename'] = inbasename
+        return meta
 
-    def set_out_parameters(self):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        Takes care of setting all output parameters.
+        Set SARDEMProjection related information that'll get carried around.
         """
-        p_out = as_list(self.param_out)
-        files = as_list(self.tmp_filename)
-        assert self._app
-        for po, tmp in zip(p_out, files):
-            assert isinstance(po, str), f"String expected for param_out={po}"
-            assert isinstance(tmp, str), f"String expected for output tmp filename={tmp}"
-            self._app.SetParameterString(po, tmp + out_extended_filename_complement(self.meta))
+        super().update_image_metadata(meta, all_inputs)
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        imd['POLARIZATION'] = ""  # Clear polarization information (makes no sense here)
+        imd['DEM_LIST']     = ', '.join(meta['dems'])
 
-    def execute_and_write_output(self):
-        """
-        Specializes :func:`execute_and_write_output()` to actually execute the
-        OTB pipeline.
+    def add_image_metadata(self, meta: Meta, app) -> None:
         """
-        assert self._app
-        do_measure = True  # TODO
-        # logger.debug('meta pipe: %s', self.meta['pipe'])
-        pipeline_name = '%s > %s' % (' | '.join(str(e) for e in self.meta['pipe']), self.out_filename)
-        if files_exist(self.out_filename):
-            # This is a dirty failsafe, instead of analysing at the last
-            # moment, it's be better to have a clear idea of all dependencies
-            # and of what needs to be done.
-            logger.info('%s already exists. Aborting << %s >>', self.out_filename, pipeline_name)
-            return
-        with Utils.ExecutionTimer('-> pipe << ' + pipeline_name + ' >>', do_measure):
-            if not is_running_dry(self.meta):
-                # TODO: catch execute failure, and report it!
-                # logger.info("START %s", pipeline_name)
-                with Utils.RedirectStdToLogger(logging.getLogger('s1tiling.OTB')):
-                    # For OTB application execution, redirect stdout/stderr
-                    # messages to s1tiling.OTB
-                    self.set_out_parameters()
-                    self._app.ExecuteAndWriteOutput()
-                self._write_image_metadata()
-                commit_execution(self.tmp_filename, self.out_filename)
-        if 'post' in self.meta and not is_running_dry(self.meta):
-            for hook in self.meta['post']:
-                # Note: we can't extract and pass meta-data around from this hook
-                # Indeed the hook is executed at Store Factory level, while metadata
-                # are passed around between around Factories and Steps.
-                logger.debug("Execute post-hook for %s", self.out_filename)
-                hook(self.meta, self.app)
-        self.clean_cache()
-        self.meta['pipe'] = [self.out_filename]
+        Post-application hook used to complete GDAL metadata.
 
+        As :func:`update_image_metadata` is not designed to access OTB
+        application information (``directiontoscandeml``...), we need this
+        extra hook to fetch and propagate the PRJ information.
+        """
+        fullpath = out_filename(meta)
+        logger.debug('Set metadata in %s', fullpath)
+        dst = gdal.Open(fullpath, gdal.GA_Update)
+        assert dst
+
+        # Pointless here! :(
+        assert app
+        meta['directiontoscandeml'] = app.GetParameterInt('directiontoscandeml')
+        meta['directiontoscandemc'] = app.GetParameterInt('directiontoscandemc')
+        meta['gain']                = app.GetParameterFloat('gain')
+        dst.SetMetadataItem('PRJ.DIRECTIONTOSCANDEML', str(meta['directiontoscandeml']))
+        dst.SetMetadataItem('PRJ.DIRECTIONTOSCANDEMC', str(meta['directiontoscandemc']))
+        dst.SetMetadataItem('PRJ.GAIN',                str(meta['gain']))
+        dst.FlushCache()  # We really need to be sure it has been flushed now, if not closed
+        del dst
+
+    def parameters(self, meta: Meta) -> OTBParameters:
+        """
+        Returns the parameters to use with
+        :external:doc:`SARDEMProjection OTB application
+        <Applications/app_SARDEMProjection>` to project S1 geometry onto DEM tiles.
+        """
+        nodata = meta.get('nodata', -32768)
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        indem = fetch_input_data('indem', inputs).out_filename
+        return {
+                'ram'        : ram(self.ram_per_process),
+                'insar'      : in_filename(meta),
+                'indem'      : indem,
+                'withxyz'    : True,
+                # 'withh'      : True,  # uncomment to analyse/debug height computed
+                'nodata'     : nodata
+                }
 
-def commit_execution(tmp_fn, out_fn):
-    """
-    Concluding step that validates the successful execution of an application,
-    whether it's an OTB application or an external executable.
-
-    - Rename the tmp image into its final name
-    - Rename the associated geom file (if any as well)
-    """
-    assert type(tmp_fn) == type(out_fn)
-    if isinstance(out_fn, list):
-        for t, o in zip(tmp_fn, out_fn):
-            commit_execution(t, o)
-        return
-    logger.debug('Renaming: mv %s %s', tmp_fn, out_fn)
-    shutil.move(tmp_fn, out_fn)
-    tmp_geom = re.sub(re_tiff, '.geom', tmp_fn)
-    if os.path.isfile(tmp_geom):
-        out_geom = re.sub(re_tiff, '.geom', out_fn)
-        logger.debug('Renaming: mv %s %s', tmp_geom, out_geom)
-        shutil.move(tmp_geom, out_geom)
-    logger.debug('-> %s renamed as %s', tmp_fn, out_fn)
-    assert not os.path.isfile(tmp_fn)
-    assert os.path.isfile(out_fn)
-
-
-class _FileProducingStepFactory(StepFactory):
-    """
-    Abstract class that factorizes filename transformations and parameter
-    handling for Steps that produce files, either with OTB or through external
-    calls.
-
-    :func:`create_step` is kind of *abstract* at this point.
-    """
-    def __init__(self, cfg,
-            gen_tmp_dir, gen_output_dir, gen_output_filename,
-            *argv, **kwargs):
+    def requirement_context(self) -> str:
         """
-        Constructor
-
-        See :func:`output_directory`, :func:`tmp_directory`,
-        :func:`build_step_output_filename` and
-        :func:`build_step_output_tmp_filename` for the usage of ``gen_tmp_dir``,
-        ``gen_output_dir`` and ``gen_output_filename``.
+        Return the requirement context that permits to fix missing requirements.
+        SARDEMProjection2 comes from normlim_sigma0.
         """
-        super().__init__(*argv, **kwargs)
-        is_a_final_step = gen_output_dir and gen_output_dir != gen_tmp_dir
-        # logger.debug("%s -> final: %s <== gen_tmp=%s    gen_out=%s", self.name, is_a_final_step, gen_tmp_dir, gen_output_dir)
+        return "Please install https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0."
 
-        self.__gen_tmp_dir         = gen_tmp_dir
-        self.__gen_output_dir      = gen_output_dir if gen_output_dir else gen_tmp_dir
-        self.__gen_output_filename = gen_output_filename
-        self.__ram_per_process     = cfg.ram_per_process
-        self.__tmpdir              = cfg.tmpdir
-        self.__outdir              = cfg.output_preprocess if is_a_final_step else cfg.tmpdir
-        logger.debug("new _FileProducingStepFactory(%s) -> TMPDIR=%s  OUT=%s", self.name, self.__tmpdir, self.__outdir)
 
-    def parameters(self, meta):
-        """
-        Most steps that produce files will expect parameters.
+class SARCartesianMeanEstimation(OTBStepFactory):
+    """
+    Factory that prepares steps that run
+    :external:doc:`Applications/app_SARCartesianMeanEstimation` as described in
+    :ref:`Normals computation` documentation.
 
-        Warning: In :class:`ExecutableStepFactory`, parameters that designate
-        output filenames are expected to use :func:`tmp_filename` and not
-        :func:`out_filename`. Indeed products are meant to be first produced
-        with temporary names before being renamed with their final names, once
-        the operation producing them has succeeded.
 
-        Note: This method is kind-of abstract --
-        :class:`SelectBestCoverage <s1tiling.libs.otbwrappers.SelectBestCoverage>` is a
-        :class:`_FileProducingStepFactory` but, it doesn't actualy consume parameters.
-        """
-        raise TypeError(f"An {self.__class__.__name__} step don't produce anything!")
+    :external:doc:`Applications/app_SARCartesianMeanEstimation` estimates a simulated
+    cartesian mean image thanks to a DEM file.
 
-    def output_directory(self, meta):
-        """
-        Accessor to where output files will be stored in case their production
-        is required (i.e. not in-memory processing)
+    Requires the following information from the configuration object:
 
-        This property is built from ``gen_output_dir`` construction parameter.
-        Typical values for the parameter are:
+    - `ram_per_process`
 
-        - ``os.path.join(cfg.output_preprocess, '{tile_name}'),`` where ``tile_name``
-          is looked into ``meta`` parameter
-        - ``None``, in that case the result will be the same as :func:`tmp_directory`.
-          This case will make sense for steps that don't produce required products
-        """
-        return str(self.__gen_output_dir).format(**meta)
+    Requires the following information from the metadata dictionary
 
-    def _get_nominal_output_basename(self, meta):
-        """
-        Returns the pathless basename of the produced file (internal).
-        """
-        return self.__gen_output_filename.generate(meta['basename'], meta)
+    - input filename
+    - output filename
 
-    def build_step_output_filename(self, meta):
-        """
-        Returns the names of typical result files in case their production
-        is required (i.e. not in-memory processing).
+    Note: It cannot be chained in memory because of the ``directiontoscandem*`` parameters.
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'XYZ_{polarless_basename}'
+        fname_fmt = cfg.fname_fmt.get('xyz', fname_fmt)
+        super().__init__(
+                cfg,
+                appname='SARCartesianMeanEstimation2', name='SARCartesianMeanEstimation',
+                param_in=None, param_out='out',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S1'),
+                gen_output_dir=None,  # Use gen_tmp_dir
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description='Cartesian XYZ coordinates estimation',
+        )
 
-        This specialization uses ``gen_output_filename`` naming policy
-        parameter to build the output filename. See the `Available naming
-        policies`_.
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        """
+        Injects the :func:`reduce_inputs_insar` hook in step metadata, and
+        provide names clear from polar related information.
         """
-        filename = self._get_nominal_output_basename(meta)
-        in_dir = lambda fn : os.path.join(self.output_directory(meta), fn)
-        if isinstance(filename, str):
-            return in_dir(filename)
+        # Ignore polarization in filenames
+        if 'polarless_basename' in meta:
+            assert meta['polarless_basename'] == remove_polarization_marks(meta['basename'])
         else:
-            return [in_dir(fn) for fn in filename]
+            meta['polarless_basename'] = remove_polarization_marks(meta['basename'])
+        meta['reduce_inputs_insar'] = lambda inputs : [inputs[0]]  # TODO!!!
+        return meta
 
-    def tmp_directory(self, meta):
+    def _get_canonical_input(self, inputs: InputList) -> AbstractStep:
         """
-        Directory used to store temporary files before they are renamed into
-        their final version.
-
-        This property is built from ``gen_tmp_dir`` construction parameter.
-        Typical values for the parameter are:
+        Helper function to retrieve the canonical input associated to a list of inputs.
 
-        - ``os.path.join(cfg.tmpdir, 'S1')``
-        - ``os.path.join(cfg.tmpdir, 'S2', '{tile_name}')`` where ``tile_name``
-          is looked into ``meta`` parameter
+        In :class:`SARCartesianMeanEstimation` case, the canonical input comes
+        from the "indem" pipeline defined in :func:s1tiling.s1_process_lia`
+        pipeline builder.
         """
-        return self.__gen_tmp_dir.format(**meta)
+        _check_input_step_type(inputs)
+        keys = set().union(*(input.keys() for input in inputs))
+        assert len(inputs) == 3, f'Expecting 3 inputs. {len(inputs)} are found: {keys}'
+        assert 'indemproj' in keys
+        return [input['indemproj'] for input in inputs if 'indemproj' in input.keys()][0]
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        """
+        Complete meta information with hook for updating image metadata
+        w/ directiontoscandemc, directiontoscandeml and gain.
+        """
+        inputpath = out_filename(meta)  # needs to be done before super.complete_meta!!
+        meta = super().complete_meta(meta, all_inputs)
+        meta['inputs'] = all_inputs
+        if 'directiontoscandeml' not in meta or 'directiontoscandemc' not in meta:
+            self.fetch_direction(inputpath, meta)
+        indem     = fetch_input_data('indem',     all_inputs).out_filename
+        indemproj = fetch_input_data('indemproj', all_inputs).out_filename
+        meta['files_to_remove'] = [indem, indemproj]
+        logger.debug('Register files to remove after XYZ computation: %s', meta['files_to_remove'])
+        _, inbasename = os.path.split(in_filename(meta))
+        meta['inbasename'] = inbasename
+        return meta
 
-    def build_step_output_tmp_filename(self, meta):
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
         """
-        This specialization of :func:`StepFactory.build_step_output_tmp_filename`
-        will automatically insert ``.tmp`` before the filename extension.
+        Set SARCartesianMeanEstimation related information that'll get carried around.
         """
-        filename = self._get_nominal_output_basename(meta)
-        add_tmp = lambda fn : os.path.join(
-                self.tmp_directory(meta), re.sub(re_any_ext, r'.tmp\g<0>', fn))
-        if isinstance(filename, str):
-            return add_tmp(filename)
+        super().update_image_metadata(meta, all_inputs)
+        assert 'image_metadata' in meta
+        imd = meta['image_metadata']
+        # Clear PRJ.* information: makes no sense anymore
+        imd['PRJ.DIRECTIONTOSCANDEML'] = ""
+        imd['PRJ.DIRECTIONTOSCANDEMC'] = ""
+        imd['PRJ.GAIN']                = ""
+
+    def fetch_direction(self, inputpath, meta: Meta) -> None:
+        """
+        Extract back direction to scan DEM from SARDEMProjected image metadata.
+        """
+        logger.debug("Fetch PRJ.DIRECTIONTOSCANDEM* from '%s'", inputpath)
+        if not is_running_dry(meta):  # FIXME: this info is no longer in meta!
+            dst = gdal.Open(inputpath, gdal.GA_ReadOnly)
+            if not dst:
+                raise RuntimeError(f"Cannot open SARDEMProjected file '{inputpath}' to collect scan direction metadata.")
+            meta['directiontoscandeml'] = dst.GetMetadataItem('PRJ.DIRECTIONTOSCANDEML')
+            meta['directiontoscandemc'] = dst.GetMetadataItem('PRJ.DIRECTIONTOSCANDEMC')
+            if meta['directiontoscandeml'] is None or meta['directiontoscandemc'] is None:
+                raise RuntimeError(f"Cannot fetch direction to scan from SARDEMProjected file '{inputpath}'")
+            del dst
         else:
-            return [add_tmp(fn) for fn in filename]
+            meta['directiontoscandeml'] = 42
+            meta['directiontoscandemc'] = 42
 
-    @property
-    def ram_per_process(self):
+    def parameters(self, meta: Meta) -> OTBParameters:
         """
-        Property ram_per_process
+        Returns the parameters to use with
+        :external:doc:`SARCartesianMeanEstimation OTB application
+        <Applications/app_SARCartesianMeanEstimation>` to compute cartesian
+        coordinates of each point of the origin S1 image.
+        """
+        assert 'inputs' in meta, f'Looking for "inputs" in {meta.keys()}'
+        inputs = meta['inputs']
+        insar     = fetch_input_data('insar', inputs).out_filename
+        indem     = fetch_input_data('indem', inputs).out_filename
+        indemproj = fetch_input_data('indemproj', inputs).out_filename
+        return {
+                'ram'             : ram(self.ram_per_process),
+                'insar'           : insar,
+                'indem'           : indem,
+                'indemproj'       : indemproj,
+                'indirectiondemc' : int(meta['directiontoscandemc']),
+                'indirectiondeml' : int(meta['directiontoscandeml']),
+                'mlran'           : 1,
+                'mlazi'           : 1,
+        }
+
+    def requirement_context(self) -> str:
+        """
+        Return the requirement context that permits to fix missing requirements.
+        SARCartesianMeanEstimation2 comes from normlim_sigma0.
         """
-        return self.__ram_per_process
+        return "Please install https://gitlab.orfeo-toolbox.org/s1-tiling/normlim_sigma0."
 
 
-class OTBStepFactory(_FileProducingStepFactory):
+class ComputeNormalsOnS1(_ComputeNormals):
     """
-    Abstract StepFactory for all OTB Applications.
+    Factory that prepares steps that run
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    on images in S1 geometry as described in :ref:`Normals
+    computation <compute_normals-proc>` documentation.
 
-    All step factories that wrap OTB applications are meant to inherit from
-    :class:`OTBStepFactory`.
-    """
-    def __init__(self, cfg,
-            appname,
-            gen_tmp_dir, gen_output_dir, gen_output_filename,
-            *argv, **kwargs):
-        """
-        Constructor.
+    :external:doc:`ExtractNormalVector <Applications/app_ExtractNormalVector>`
+    computes surface normals.
 
-        See:
-            :func:`_FileProducingStepFactory.__init__`
+    Requires the following information from the configuration object:
 
-        Parameters:
-            :param_in:  Flag used by the default OTB application for the input file (default: "in")
-            :param_out: Flag used by the default OTB application for the ouput file (default: "out")
-        """
-        super().__init__(cfg, gen_tmp_dir, gen_output_dir, gen_output_filename, *argv, **kwargs)
-        # is_a_final_step = gen_output_dir and gen_output_dir != gen_tmp_dir
-        # logger.debug("%s -> final: %s <== gen_tmp=%s    gen_out=%s", self.name, is_a_final_step, gen_tmp_dir, gen_output_dir)
+    - `ram_per_process`
 
-        self._in                   = kwargs.get('param_in',  'in')
-        self._out                  = kwargs.get('param_out', 'out')
-        # param_in is only used in connected mode. As such a string is expected.
-        assert self.param_in  is None or isinstance(self.param_in, str), f"String expected for {appname} param_in={self.param_in}"
-        # param_out is always used.
-        assert isinstance(self.param_out, (str, list)), f"String or list expected for {appname} param_out={self.param_out}"
-        self._appname              = appname
-        logger.debug("new OTBStepFactory(%s) -> app=%s", self.name, appname)
+    Requires the following information from the metadata dictionary
 
-    @property
-    def appname(self):
-        """
-        OTB Application property.
-        """
-        return self._appname
-
-    @property
-    def param_in(self):
-        """
-        Name of the "in" parameter used by the OTB Application.
-        Default is likely to be "in", while some applications use "io.in", often "il" for list of
-        files...
-        """
-        return self._in
+    - input filename
+    - output filename
+    - `fname_fmt`  -- optional key: `normals_on_s1`, useless in the in-memory nominal case
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = 'Normals_{polarless_basename}'
+        fname_fmt = cfg.fname_fmt.get('normals_on_s1', fname_fmt)
+        super().__init__(
+                cfg,
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S1'),
+                output_fname_fmt=fname_fmt,
+                image_description='Image normals on Sentinel-{flying_unit_code_short} IW GRD',
+        )
 
-    @property
-    def param_out(self):
-        """
-        Name of the "out" parameter used by the OTB Application.
-        Default is likely to be "out", whie some applications use "io.out".
-        """
-        return self._out
 
-    def set_output_pixel_type(self, app, meta):
-        """
-        Permits to have steps force the output pixel data.
-        Does nothing by default.
-        Override this method to change the output pixel type.
-        """
-        pass
+class ComputeLIAOnS1(_ComputeLIA):
+    """
+    Factory that prepares steps that run
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    on images in S1 geometry as described in :ref:`LIA maps computation <compute_lia-proc>` documentation.
 
-    def create_step(self, in_memory: bool, previous_steps):
-        """
-        Instanciates the step related to the current :class:`StepFactory`,
-        that consumes results from the previous `input` step.
+    :external:doc:`SARComputeLocalIncidenceAngle <Applications/app_SARComputeLocalIncidenceAngle>`
+    computes Local Incidende Angle Map.
 
-        1. This methods starts by updating metadata information through
-        :func:`complete_meta()` on the `input` metadata.
+    Requires the following information from the configuration object:
 
-        2. Then, steps that wrap an OTB application will instanciate this
-        application object, and:
+    - `ram_per_process`
 
-           - either pipe the new application to the one from the `input` step
-             if it wasn't a first step
-           - or fill in the "in" parameter of the application with the
-             :func:`out_filename` of the `input` step.
+    Requires the following information from the metadata dictionary
 
-        2-bis. in case the new step isn't related to an OTB application,
-        nothing specific is done, we'll just return an :class:`AbstractStep`
+    - input filename
+    - output filename
+    - `fname_fmt`  -- optional key: `s1_lia`
+    - `fname_fmt`  -- optional key: `s1_sin_lia`
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt_lia = cfg.fname_fmt.get('s1_lia',     'LIA_{polarless_basename}')
+        fname_fmt_sin = cfg.fname_fmt.get('s1_sin_lia', 'sin_LIA_{polarless_basename}')
+        super().__init__(
+                cfg,
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S1'),
+                gen_output_dir=None,
+                fname_fmt_lia=fname_fmt_lia,
+                fname_fmt_sin=fname_fmt_sin,
+                image_description='LIA on Sentinel-{flying_unit_code_short} IW GRD',
+        )
 
-        Note: While `previous_steps` is ignored in this specialization, it's
-        used in :func:`Store.create_step()` where it's eventually used to
-        release all OTB Application objects.
 
-        Note: it's possible to override this method to return no step
-        (``None``). In that case, no OTB Application would be registered in
-        the actual :class:`Pipeline`.
-        """
-        inputs = self._get_inputs(previous_steps)
-        inp    = self._get_canonical_input(inputs)
-        meta   = self.complete_meta(inp.meta, inputs)
-        self.update_image_metadata(meta, inputs) # Needs to be done after complete_meta!
-        assert self.appname
-
-        # Otherwise: step with an OTB application...
-        if is_running_dry(meta):
-            logger.warning('DRY RUN mode: ignore step and OTB Application creation')
-            lg_from = inp.out_filename if inp.is_first_step else 'app'
-            logger.debug('Register app: %s (from %s) %s', self.appname, lg_from, ' '.join('-%s %s' % (k, as_app_shell_param(v)) for k, v in self.parameters(meta).items()))
-            meta['param_out'] = self.param_out
-            return Step('FAKEAPP', **meta)
-        with Utils.RedirectStdToLogger(logging.getLogger('s1tiling.OTB')):
-            # For OTB application execution, redirect stdout/stderr messages to s1tiling.OTB
-            app = otb.Registry.CreateApplication(self.appname)
-            if not app:
-                raise RuntimeError("Cannot create OTB application '" + self.appname + "'")
-            parameters = self.parameters(meta)
-            if inp.is_first_step:
-                if not files_exist(inp.out_filename):
-                    logger.critical("Cannot create OTB pipeline starting with %s as some input files don't exist (%s)", self.appname, inp.out_filename)
-                    raise RuntimeError(f"Cannot create OTB pipeline starting with {self.appname} as some input files don't exist ({inp.out_filename})")
-                # parameters[self.param_in] = inp.out_filename
-                lg_from = inp.out_filename
-            else:
-                assert isinstance(self.param_in, str), f"String expected for {self.param_in}"
-                assert isinstance(inp.param_out, str), f"String expected for {self.param_out}"
-                app.ConnectImage(self.param_in, inp.app, inp.param_out)
-                this_step_is_in_memory = in_memory and not inp.shall_store
-                # logger.debug("Chaining %s in memory: %s", self.appname, this_step_is_in_memory)
-                app.PropagateConnectMode(this_step_is_in_memory)
-                if this_step_is_in_memory:
-                    # When this is not a store step, we need to clear the input parameters
-                    # from its list, otherwise some OTB applications may comply
-                    del parameters[self.param_in]
-                lg_from = 'app'
-
-            self.set_output_pixel_type(app, meta)
-            logger.debug('Register app: %s (from %s) %s -%s %s',
-                    self.appname, lg_from,
-                    ' '.join('-%s %s' % (k, as_app_shell_param(v)) for k, v in parameters.items()),
-                    self.param_out, as_app_shell_param(meta.get('out_filename', '???')))
-            try:
-                app.SetParameters(parameters)
-            except Exception:
-                logger.exception("Cannot set parameters to %s (from %s) %s", self.appname, lg_from, ' '.join('-%s %s' % (k, as_app_shell_param(v)) for k, v in parameters.items()))
-                raise
-
-        meta['param_out'] = self.param_out
-        return Step(app, **meta)
-
-    def check_requirements(self):
-        """
-        This specialization of :func:`check_requirements` checks whether the
-        related OTB application can correctly be executed from S1Tiling.
-
-        :return: A pair of the message indicating what is required, and some
-                 context how to fix it -- by default: install OTB!
-        :return: ``None`` otherwise.
-        """
-        app = otb.Registry.CreateApplication(self.appname)
-        if not app:
-            return f"{self.appname}", self.requirement_context()
-        else:
-            app = None
-            return None
+class OrthoRectifyLIA(_OrthoRectifierFactory):
+    """
+    Factory that prepares steps that run
+    :external:doc:`Applications/app_OrthoRectification` on LIA maps.
 
-    def requirement_context(self):
-        """
-        Return the requirement context that permits to fix missing requirements.
-        By default, OTB applications requires... OTB!
-        """
-        return "Please install OTB."
+    Requires the following information from the configuration object:
 
+    - `ram_per_process`
+    - `out_spatial_res`
+    - `GeoidFile`
+    - `grid_spacing`
+    - `tmp_dem_dir`
 
-class ExecutableStepFactory(_FileProducingStepFactory):
-    """
-    Abstract StepFactory for executing any external program.
+    Requires the following information from the metadata dictionary
 
-    All step factories that wrap OTB applications are meant to inherit from
-    :class:`ExecutableStepFactory`.
+    - base name -- to generate typical output filename
+    - input filename
+    - output filename
+    - `manifest`
+    - `tile_name`
+    - `tile_origin`
     """
-    def __init__(self, cfg,
-            exename,
-            gen_tmp_dir, gen_output_dir, gen_output_filename,
-            *argv, **kwargs):
+    def __init__(self, cfg: Configuration) -> None:
         """
-        Constructor
-
-        See:
-            :func:`_FileProducingStepFactory.__init__`
+        Constructor.
+        Extract and cache configuration options.
         """
-        super().__init__(cfg, gen_tmp_dir, gen_output_dir, gen_output_filename, *argv, **kwargs)
-        self._exename              = exename
-        logger.debug("new ExecutableStepFactory(%s) -> exe=%s", self.name, exename)
+        fname_fmt = '{LIA_kind}_{flying_unit_code}_{tile_name}_{orbit_direction}_{orbit}_{acquisition_time}.tif'
+        fname_fmt = cfg.fname_fmt.get('lia_orthorectification', fname_fmt)
+        super().__init__(
+                cfg,
+                fname_fmt,
+                image_description='Orthorectified {LIA_kind} Sentinel-{flying_unit_code_short} IW GRD',
+        )
+        extra_ef = '&writegeom=false' if otb_version() < '8.0.0' else ''
+        self._extended_filenames = {
+                'LIA'     : extended_filename_lia_degree(cfg) + extra_ef,
+                'sin_LIA' : extended_filename_lia_sin(cfg) + extra_ef,
+        }
+
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        meta = super()._update_filename_meta_pre_hook(meta)
+        assert 'LIA_kind' in meta, "This StepFactory shall be registered after a call to filter_LIA()"
+        return meta
+
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        meta = super().complete_meta(meta, all_inputs)
+        assert 'out_extended_filename_complement' not in meta, f'{meta["out_extended_filename_complement"]=!r} nothing was expected'
+        kind = meta['LIA_kind']
+        meta['out_extended_filename_complement'] = self._extended_filenames[kind]
+        return meta
+
+    def _get_input_image(self, meta: Meta) -> str:
+        inp = in_filename(meta)
+        assert isinstance(inp, str), f"A single string inp was expected, got {inp}"
+        return inp   # meta['in_filename']
+
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
+        """
+        Set LIA kind related information that'll get carried around.
+        """
+        super().update_image_metadata(meta, all_inputs)
+        types = {
+                'sin_LIA': 'SIN(LIA)',
+                'LIA': '100 * degree(LIA)'
+        }
+        assert 'LIA_kind' in meta, "This StepFactory shall be registered after a call to filter_LIA()"
+        kind = meta['LIA_kind']
+        assert kind in types, f'The only LIA kind accepted are {types.keys()}'
+        imd = meta['image_metadata']
+        imd['DATA_TYPE'] = types[kind]
 
-    def create_step(self, in_memory: bool, previous_steps):
+    def set_output_pixel_type(self, app, meta: Meta) -> None:
         """
-        This Step creation method does more than just creating the step.
-        It also executes immediately the external process.
+        Force LIA output pixel type to ``INT16``.
         """
-        logger.debug("Directly execute %s step", self.name)
-        inputs = self._get_inputs(previous_steps)
-        inp    = self._get_canonical_input(inputs)
-        meta   = self.complete_meta(inp.meta, inputs)
-        self.update_image_metadata(meta, inputs) # Needs to be done after complete_meta!
-        res    = ExecutableStep(self._exename, **meta)
-        parameters = self.parameters(meta)
-        res.execute_and_write_output(parameters)
-        return res
+        if meta.get('LIA_kind', '') == 'LIA':
+            app.SetParameterOutputImagePixelType(self.param_out, otb.ImagePixelType_int16)
 
 
-class Store(StepFactory):
+class ConcatenateLIA(_ConcatenatorFactory):
     """
-    Factory for Artificial Step that forces the result of the previous app
-    sequence to be stored on disk by breaking in-memory connection.
+    Factory that prepares steps that run
+    :external:doc:`Applications/app_Synthetize` on LIA images.
 
-    While it could be used manually, it's meant to be automatically appended
-    at the end of a pipeline if any step is actually related to OTB.
-    """
-    def __init__(self, appname, *argv, **kwargs):  # pylint: disable=unused-argument
-        super().__init__('(StoreOnFile)', "(StoreOnFile)", *argv, **kwargs)
-        # logger.debug('Creating Store Factory: %s', appname)
-
-    def create_step(self, in_memory: bool, previous_steps):
-        """
-        Specializes :func:`StepFactory.create_step` to trigger
-        :func:`StoreStep.execute_and_write_output` on the last step that
-        relates to an OTB Application.
-        """
-        inputs = self._get_inputs(previous_steps)
-        inp    = self._get_canonical_input(inputs)
-        if inp.is_first_step:
-            # assert False  # Should no longer happen, yet it does w/ ConcatLIA...
-            # Special case of by-passed inputs
-            meta = inp.meta.copy()
-            return AbstractStep(**meta)
-
-        # logger.debug('Creating StoreStep from %s', inp)
-        res = StoreStep(inp)
-        try:
-            res.execute_and_write_output()
-        finally:
-            # logger.debug("Collecting memory!")
-            # Collect memory now!
-            res.release_app()
-            for inps in previous_steps:
-                for inp in inps:
-                    for _, step in inp.items():
-                        step.release_app()
-        return res
+    Requires the following information from the configuration object:
 
-    # abstract methods...
+    - `ram_per_process`
 
-    def build_step_output_filename(self, meta):
-        raise TypeError("No way to ask for the output filename of a Store Factory")
+    Requires the following information from the metadata dictionary
 
-    def build_step_output_tmp_filename(self, meta):
-        raise TypeError("No way to ask for the output temporary filename of a Store Factory")
+    - input filename
+    - output filename
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = '{LIA_kind}_{flying_unit_code}_{tile_name}_{orbit_direction}_{orbit}_{acquisition_day}.tif'
+        fname_fmt = cfg.fname_fmt.get('lia_concatenation', fname_fmt)
+        super().__init__(
+                cfg,
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=None,  # Use gen_tmp_dir
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+                image_description='Orthorectified {LIA_kind} Sentinel-{flying_unit_code_short} IW GRD',
+                extended_filename=None,  # will be set later...
+                pixel_type=None,         # will be set later...
+        )
+        self._extended_filenames = {
+                'LIA'     : extended_filename_lia_degree(cfg),
+                'sin_LIA' : extended_filename_lia_sin(cfg),
+        }
 
+    def _update_filename_meta_post_hook(self, meta: Meta) -> None:
+        """
+        Override "update_out_filename" hook to help select the input set with
+        the best coverage.
+        """
+        assert 'LIA_kind' in meta
+        meta['update_out_filename'] = self.update_out_filename  # <- needs to be done in post_hook!
+        # Remove acquisition_time that no longer makes sense
+        meta.pop('acquisition_time', None)
 
-# ======================================================================
-# Multi processing related (old) code
-def mp_worker_config(queue):
-    """
-    Worker configuration function called by Pool().
+    def update_image_metadata(self, meta: Meta, all_inputs: InputList) -> None:
+        """
+        Update concatenated LIA related information that'll get carried around.
+        """
+        super().update_image_metadata(meta, all_inputs)
+        imd = meta['image_metadata']
+        imd['DEM_LIST']  = ""  # Clear DEM_LIST information (a merge of 2 lists should be done actually)
 
-    It takes care of initializing the queue handler in the subprocess.
+    def complete_meta(self, meta: Meta, all_inputs: InputList) -> Meta:
+        meta = super().complete_meta(meta, all_inputs)
+        assert 'out_extended_filename_complement' not in meta, f'{meta["out_extended_filename_complement"]=!r} nothing was expected'
+        kind = meta['LIA_kind']
+        meta['out_extended_filename_complement'] = self._extended_filenames[kind]
+        return meta
 
-    Parameters:
-        :queue: multiprocessing.Queue used for passing logging messages from worker to main
-            process.
-    """
-    qh = logging.handlers.QueueHandler(queue)
-    global logger
-    logger = logging.getLogger()
-    logger.addHandler(qh)
+    def update_out_filename(self, meta: Meta, with_task_info: TaskInputInfo) -> None:
+        """
+        Unlike usual :class:`Concatenate`, the output filename will always ends
+        in "txxxxxx".
 
+        However we want to update the coverage of the current pair as a new
+        input file has been registered.
 
-# TODO: try to make it static...
-def execute4mp(pipeline):
-    """
-    Internal worker function used by multiprocess to execute a pipeline.
-    """
-    return pipeline.do_execute()
+        TODO: Find a better name for the hook as it handles two different
+        services.
+        """
+        inputs = with_task_info.inputs['in']
+        dates = {re.sub(r'txxxxxx|t\d+', '', inp['acquisition_time']) for inp in inputs}
+        assert len(dates) == 1, f"All concatenated files shall have the same date instead of {dates}"
+        date = min(dates)
+        logger.debug('[ConcatenateLIA] at %s:', date)
+        coverage = 0.
+        for inp in inputs:
+            if re.sub(r'txxxxxx|t\d+', '', inp['acquisition_time']) == date:
+                s1_cov = inp['tile_coverage']
+                coverage += s1_cov
+                logger.debug(' - %s => %s%% coverage', inp['basename'], s1_cov)
+        # Round coverage at 3 digits as tile footprint has a very limited precision
+        coverage = round(coverage, 3)
+        logger.debug('[ConcatenateLIA] => total coverage at %s: %s%%', date, coverage * 100)
+        meta['tile_coverage'] = coverage
+
+    def set_output_pixel_type(self, app, meta: Meta) -> None:
+        """
+        Force LIA output pixel type to ``INT16``.
+        """
+        if meta.get('LIA_kind', '') == 'LIA':
+            app.SetParameterOutputImagePixelType(self.param_out, otb.ImagePixelType_int16)
+
+
+class SelectBestCoverage(_FileProducingStepFactory):
+    """
+    StepFactory that helps select only one path after LIA concatenation:
+    the one that have the best coverage of the S2 tile target.
+
+    If several concatenated products have the same coverage, the oldest one
+    will be selected.
+
+    The coverage is extracted from ``tile_coverage`` step metadata.
+
+    The step produced does nothing: it only only rename the selected product
+    into the final expected name. Note: in LIA case two files will actually
+    renamed.
+
+    Requires the following information from the metadata dictionary
+
+    - `acquisition_day`
+    - `tile_coverage`
+    - `LIA_kind`
+    - `flying_unit_code`
+    - `tile_name`
+    - `orbit_direction`
+    - `orbit`
+    - `fname_fmt`  -- optional key: `lia_product`
+    - `dname_fmt`  -- optional key: `lia_product`
+    """
+    def __init__(self, cfg: Configuration) -> None:
+        fname_fmt = '{LIA_kind}_{flying_unit_code}_{tile_name}_{orbit_direction}_{orbit}.tif'
+        fname_fmt = cfg.fname_fmt.get('lia_product', fname_fmt)
+        dname_fmt = dname_fmt_lia_product(cfg)
+        super().__init__(
+                cfg,
+                name='SelectBestCoverage',
+                gen_tmp_dir=os.path.join(cfg.tmpdir, 'S2', '{tile_name}'),
+                gen_output_dir=dname_fmt,
+                gen_output_filename=TemplateOutputFilenameGenerator(fname_fmt),
+        )
+
+    def _update_filename_meta_pre_hook(self, meta: Meta) -> Meta:
+        """
+        Inject the :func:`reduce_LIAs` hook in step metadata.
+        """
+        def reduce_LIAs(inputs):
+            """
+            Select the concatenated pair of LIA files that have the best coverage of the considered
+            S2 tile.
+            """
+            # TODO: quid if different dates have best different coverage on a set of tiles?
+            # How to avoid computing LIA again and again on a same S1 zone?
+            # dates = set([re.sub(r'txxxxxx|t\d+', '', inp['acquisition_time']) for inp in inputs])
+            best_covered_input = max(inputs, key=lambda inp: inp['tile_coverage'])
+            logger.debug('Best coverage is %s at %s among:', best_covered_input['tile_coverage'], best_covered_input['acquisition_day'])
+            for inp in inputs:
+                logger.debug(' - %s: %s', inp['acquisition_day'], inp['tile_coverage'])
+            return [best_covered_input]
 
+        meta['reduce_inputs_in'] = reduce_LIAs
+        return meta
 
-class PoolOfOTBExecutions:
-    """
-    Internal multiprocess Pool of OTB pipelines.
-    """
-    def __init__(self,
-            title,
-            do_measure,
-            nb_procs, nb_threads,
-            log_queue, log_queue_listener,
-            debug_otb):
-        """
-        constructor
-        """
-        self.__pool = []
-        self.__title              = title
-        self.__do_measure         = do_measure
-        self.__nb_procs           = nb_procs
-        self.__nb_threads         = nb_threads
-        self.__log_queue          = log_queue
-        self.__log_queue_listener = log_queue_listener
-        self.__debug_otb          = debug_otb
-
-    def new_pipeline(self, **kwargs):
-        """
-        Register a new pipeline.
-        """
-        in_memory    = kwargs.get('in_memory', True)
-        do_watch_ram = kwargs.get('do_watch_ram', False)
-        pipeline = Pipeline(self.__do_measure, in_memory, do_watch_ram)
-        self.__pool.append(pipeline)
-        return pipeline
-
-    def process(self):
-        """
-        Executes all the pipelines in parallel.
-        """
-        nb_cmd = len(self.__pool)
-
-        os.environ["ITK_GLOBAL_DEFAULT_NUMBER_OF_THREADS"] = str(self.__nb_threads)
-        os.environ['OTB_LOGGER_LEVEL'] = 'DEBUG'
-        if self.__debug_otb:  # debug OTB applications with gdb => do not spawn process!
-            execute4mp(self.__pool[0])
-        else:
-            with multiprocessing.Pool(self.__nb_procs, mp_worker_config, [self.__log_queue]) as pool:
-                self.__log_queue_listener.start()
-                for count, result in enumerate(pool.imap_unordered(execute4mp, self.__pool), 1):
-                    logger.info("%s correctly finished", result)
-                    logger.info(' --> %s... %s%%', self.__title, count * 100. / nb_cmd)
-
-                pool.close()
-                pool.join()
-                self.__log_queue_listener.stop()
-
-
-class Processing:
-    """
-    Entry point for executing multiple instance of the same pipeline of
-    different inputs.
-
-    1. The object is initialized with a log queue and its listener
-    2. The pipeline is registered with a list of :class`StepFactory` s
-    3. The processing is done on a list of :class:`FirstStep` s
-    """
-    def __init__(self, cfg, debug_otb):
-        self.__log_queue          = cfg.log_queue
-        self.__log_queue_listener = cfg.log_queue_listener
-        self.__cfg                = cfg
-        self.__factory_steps      = []
-        self.__debug_otb          = debug_otb
-
-    def register_pipeline(self, factory_steps):
-        """
-        Register a list of :class:`StepFactory` s that describes a pipeline.
-        """
-        # Automatically append the final storing step
-        self.__factory_steps = factory_steps + [Store]
-
-    def process(self, startpoints):
-        """
-        Defines pipelines from the registered steps. Each pipeline is instanciated with a
-        startpoint. Then they registered into the PoolOfOTBExecutions.
-        The pool is finally executed.
-        """
-        assert self.__factory_steps
-        pool = PoolOfOTBExecutions("testpool", True,
-                self.__cfg.nb_procs, self.__cfg.OTBThreads,
-                self.__log_queue, self.__log_queue_listener, debug_otb=self.__debug_otb)
-        for startpoint in startpoints:
-            logger.info("register processing of %s", startpoint.basename)
-            pipeline = pool.new_pipeline(in_memory=True)
-            pipeline.set_inputs(startpoint)
-            for factory in self.__factory_steps:
-                pipeline.push(factory(self.__cfg))
+    def create_step(
+            self,
+            execution_parameters: Dict,
+            previous_steps: List[InputList]
+    ) -> AbstractStep:
+        logger.debug("Directly execute %s step", self.name)
+        inputs = self._get_inputs(previous_steps)
+        inp = self._get_canonical_input(inputs)
+        meta = self.complete_meta(inp.meta, inputs)
 
-        logger.debug('Launch pipelines')
-        pool.process()
+        # Let's reuse commit_execution as it does exactly what we need
+        if not is_running_dry(execution_parameters):
+            commit_execution(out_filename(inp.meta), out_filename(meta))
+
+        # Return a dummy Step
+        # logger.debug("%s step executed!", self.name)
+        res = AbstractStep('move', **meta)
+        return res
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/outcome.py` & `s1tiling-1.1.0rc1/s1tiling/libs/outcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # =========================================================================
 #   Program:   S1Processor
 #
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   Copyright 2017-2024 (c) CNES. All rights reserved.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -32,15 +32,15 @@
 from typing import Generic, List, Optional, TypeVar, Union
 
 Value   = TypeVar("Value")
 File    = TypeVar('File')
 Product = TypeVar('Product')
 
 
-class Outcome(Generic[Value]):
+class Outcome(Generic[Value, File]):
     """
     Kind of monad à la C++ ``std::expected<>``, ``boost::Outcome``.
 
     It stores tasks results which could be:
     - either the filename of task product,
     - or the error message that leads to the task failure.
     """
@@ -86,15 +86,15 @@
     def __repr__(self) -> str:
         if self.has_value():
             return f'Success: {self.__value_or_error}'
         else:
             return f'Error: {self.error()}'
 
 
-class PipelineOutcome(Outcome[Value], Generic[Value, File]):
+class PipelineOutcome(Outcome[Value, File], Generic[Value, File]):
     """
     Kind of monad à la C++ ``std::expected<>``, ``boost::Outcome`` that is specialized for
     generated products for better error messages.
 
     It stores tasks results which could be:
     - either the path to the downloaded product,
     - or the error message that leads to the task failure.
@@ -111,28 +111,28 @@
 
     def related_filenames(self) -> List[File]:
         """
         Returns the list of filenames related to the error or the result.
         """
         return self.__related_filenames
 
-    def add_related_filename(self, filename: File) -> "Outcome":
+    def add_related_filename(self, filename: File) -> "PipelineOutcome":
         """
         Register a filename(s) related to the result.
         """
         if isinstance(filename, list):
             for f in filename:
                 # Some OTB applications expect list passed with ``-il`` e.g.
                 self.__related_filenames.append(f)
         else:
             # While other OTB application expect only one file, passed with ``-in`` e.g.
             self.__related_filenames.append(filename)
         return self
 
-    def set_pipeline_name(self, pipeline_name: str) -> "Outcome":
+    def set_pipeline_name(self, pipeline_name: str) -> "PipelineOutcome":
         """
         Record the name of the pipeline in error
         """
         self.__pipeline_name = pipeline_name
         return self
 
     def __repr__(self) -> str:
@@ -144,19 +144,19 @@
                 msg += f' because {self.__pipeline_name} failed.'
             if len(self.__related_filenames) > 1:
                 errored_files = ', '.join(map(str, self.__related_filenames[:-1]))
                 # errored_files = str(self.__related_filenames)
                 msg += f' {errored_files} could not be produced: '
             else:
                 msg += ': '
-            msg +=  f'{self.error()}'
+            msg += f'{self.error()}'
             return msg
 
 
-class DownloadOutcome(Outcome[Value], Generic[Value, Product]):
+class DownloadOutcome(Outcome[Value, Product], Generic[Value, Product]):
     """
     Kind of monad à la C++ ``std::expected<>``, ``boost::Outcome`` that is specialized for
     downloaded products for better error messages.
 
     It stores tasks results which could be:
     - either the path to the downloaded product,
     - or the error message that leads to the task failure.
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/libs/vis.py` & `s1tiling-1.1.0rc1/s1tiling/libs/vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Licence: BSD-3 clause
 
 """
 Simple visualization of dask graph pipelines.
 """
 
 import os
+from typing import Dict, Optional
 import graphviz
 
 from dask.utils import key_split
 from dask.dot import _get_display_cls
 from dask.core import get_dependencies
 
 __author__ = "Jim Crist-Harif, and Silvio Rodrigues"
@@ -21,27 +22,27 @@
 __license__ = "BSD-3 clause"
 __version__ = "2"
 __status__ = "gist"
 __contact__ = "https://gist.github.com/jcrist/dc5b7cedfddff123f2177e5238e566e5"
 
 
 class SimpleComputationGraph:
-    def __init__(self):
+    def __init__(self) -> None:
         return
 
     @staticmethod
-    def _node_key(s):
+    def _node_key(s) -> str:
         if isinstance(s, tuple):
             return s[0]
         return str(s)
 
     def simple_graph(self,
-                     x,
+                     x: Dict,
                      filename='simple_computation_graph',
-                     format=None):
+                     format : Optional[str] = None):
 
         if hasattr(x, 'dask'):
             dsk = x.__dask_optimize__(x.dask, x.__dask_keys__())
         else:
             dsk = x
 
         deps = {k: get_dependencies(dsk, k) for k in dsk}
```

### Comparing `S1Tiling-1.0.0rc3/s1tiling/logging.conf.yaml` & `s1tiling-1.1.0rc1/s1tiling/logging.conf.yaml`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/resources/Geoid/egm96.grd` & `s1tiling-1.1.0rc1/s1tiling/resources/Geoid/egm96.grd`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.dbf` & `s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.dbf`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.shp` & `s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.shp`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/Features.shx` & `s1tiling-1.1.0rc1/s1tiling/resources/shapefile/Features.shx`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/resources/shapefile/srtm_tiles.gpkg` & `s1tiling-1.1.0rc1/s1tiling/resources/shapefile/srtm_tiles.gpkg`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/s1tiling/s1tiling-cluster.py` & `s1tiling-1.1.0rc1/deprecated/s1tiling-cluster.py`

 * *Files identical despite different names*

### Comparing `S1Tiling-1.0.0rc3/setup.py` & `s1tiling-1.1.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # =========================================================================
 #   Program:   S1Processor
 #
-#   Copyright 2017-2023 (c) CNES. All rights reserved.
+#   Copyright 2017-2024 (c) CNES. All rights reserved.
 #
 #   This file is part of S1Tiling project
 #       https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
@@ -26,40 +26,46 @@
 #          Luc HERMITTE (CS Group)
 #
 # =========================================================================
 
 import os
 import subprocess
 
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
+import re
 
 
 # Import the library to make sure there is no side effect
 import s1tiling
 
 def request_gdal_version() -> str:
     try:
         r = subprocess.run(['gdal-config', '--version'], stdout=subprocess.PIPE )
         version = r.stdout.decode('utf-8').strip('\n')
         print("GDAL %s detected on the system, using 'gdal==%s'" % (version, version))
         return version
     except Exception:  # pylint: disable=broad-except
         return '3.1.0'
 
+
+def normalize(name):
+    return re.sub(r"[-_.]+", "-", name).lower()
+
+
 BASEDIR = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
 
 metadata = {}
 with open(os.path.join(BASEDIR, "s1tiling", "__meta__.py"), "r") as f:
     exec(f.read(), metadata)
 
 with open(os.path.join(BASEDIR, "README.md"), "r") as f:
     readme = f.read()
 
 setup(
-    name                          = metadata["__title__"],
+    name                          = normalize(metadata["__title__"]),
     version                       = metadata["__version__"],
     description                   = metadata["__description__"],
     long_description              = readme,
     long_description_content_type = "text/markdown",
     author                        = metadata["__author__"],
     author_email                  = metadata["__author_email__"],
     url                           = metadata["__url__"],
@@ -68,59 +74,62 @@
 
     # Liste les packages à insérer dans la distribution
     # plutôt que de le faire à la main, on utilise la fonction
     # find_packages() de setuptools qui va chercher tous les packages
     # python recursivement dans le dossier courant.
     # C'est pour cette raison que l'on a tout mis dans un seul dossier:
     # on peut ainsi utiliser cette fonction facilement
-    packages=find_packages(exclude=("*.tests", "*.tests.*", "tests.*", "tests")),
+    packages=find_namespace_packages(exclude=("*.tests", "*.tests.*", "tests.*", "tests")),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True, # Take MANIFEST.in into account
 
     python_requires='>=3.8, <4',
     install_requires=[
         "click",
         "dask[distributed]>=2022.8.1",
         "eodag",
         "gdal=="+request_gdal_version(),
         "graphviz",
         "numpy",
         "objgraph", # leaks
-        "packaging", # version
+        # "packaging", # version
         "pympler", # leaks
-        "pyyaml",
+        "pyyaml>=5.1",
         # Any way to require OTB ?
         ],
     extras_require={
         "dev": [
             # "nose",
             # "tox",
             # "faker",
             # 'mock; python_version < "3.5" ',
             # "coverage",
             # "moto==1.3.6",
             # "twine",
             "wheel",
             "flake8",
+            "mypy",
             "pre-commit",
+            "pytest < 8.1",    # b/c pytest-bdd is old -> https://github.com/pytest-dev/pytest-bdd/issues/673
             "pytest-bdd < 6",  # Using "example table" feature, removed from v6
             #                    https://pytest-bdd.readthedocs.io/en/latest/#migration-from-5-x-x
             "pytest-check",
             "pytest-icdiff",
             "pytest-mock",
             "pylint",
             ],
         "docs": [
-            "jinja2 == 3.0.3",
+            "docutils<0.19.0", # reminder of sphinx_rtd_theme 1.3.0
+            "jinja2",
             "m2r2",
             "natsort",
-            "nbsphinx == 0.3.5",
-            "nbsphinx-link == 1.1.1",
-            "sphinx == 1.8.0",
-            "sphinx_rtd_theme",
+            "nbsphinx==0.9.3",
+            "nbsphinx-link==1.3.0",
+            "sphinx~=7.1",
+            "sphinx_rtd_theme~=1.3.0",
             ],
         },
 
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers.
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
@@ -132,14 +141,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: GIS",
         ],
 
     project_urls={
             "Bug Tracker": "https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling/-/issues",
             "Documentation": "https://s1-tiling.pages.orfeo-toolbox.org/s1tiling/latest",
             "Source Code": "https://gitlab.orfeo-toolbox.org/s1-tiling/s1tiling",
```

