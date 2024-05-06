# Comparing `tmp/sdss-kaiju-1.4.0b1.tar.gz` & `tmp/sdss_kaiju-1.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-kaiju-1.4.0b1.tar", last modified: Mon Feb 19 05:33:16 2024, max compression
+gzip compressed data, was "sdss_kaiju-1.4.0b2.tar", last modified: Mon May  6 05:26:35 2024, max compression
```

## Comparing `sdss-kaiju-1.4.0b1.tar` & `sdss_kaiju-1.4.0b2.tar`

### file list

```diff
@@ -1,62 +1,60 @@
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.206331 sdss-kaiju-1.4.0b1/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1504 2019-06-20 19:33:42.000000 sdss-kaiju-1.4.0b1/LICENSE.md
--rw-r--r--   0 gallegoj   (501) staff       (20)      108 2021-10-30 14:55:18.000000 sdss-kaiju-1.4.0b1/MANIFEST.in
--rw-r--r--   0 gallegoj   (501) staff       (20)     1020 2024-02-19 05:33:16.205021 sdss-kaiju-1.4.0b1/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)      101 2019-06-20 19:33:42.000000 sdss-kaiju-1.4.0b1/README.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)       90 2024-02-19 02:52:42.000000 sdss-kaiju-1.4.0b1/pyproject.toml
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.119687 sdss-kaiju-1.4.0b1/python/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.130800 sdss-kaiju-1.4.0b1/python/kaiju/
--rw-r--r--   0 gallegoj   (501) staff       (20)       52 2021-09-03 21:22:05.000000 sdss-kaiju-1.4.0b1/python/kaiju/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)       51 2024-02-19 03:48:27.000000 sdss-kaiju-1.4.0b1/python/kaiju/__version__.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.139512 sdss-kaiju-1.4.0b1/python/kaiju/etc/
--rw-r--r--   0 gallegoj   (501) staff       (20)     2691 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/fiducialCoords.csv
--rw-r--r--   0 gallegoj   (501) staff       (20)    19309 2021-10-30 14:55:18.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/fps_DesignReference.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)    49750 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/positionerTable.csv
--rw-r--r--   0 gallegoj   (501) staff       (20)     1691 2021-10-30 14:55:18.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/robotGrid.html
--rw-r--r--   0 gallegoj   (501) staff       (20)    10230 2021-10-30 14:55:18.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/robotGrid.js
--rw-r--r--   0 gallegoj   (501) staff       (20)    42610 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/python/kaiju/etc/wokCoords.csv
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.145703 sdss-kaiju-1.4.0b1/python/kaiju/include/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1992 2024-02-19 03:04:52.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/coordio.h
--rw-r--r--   0 gallegoj   (501) staff       (20)      201 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/fiducial.h
--rw-r--r--   0 gallegoj   (501) staff       (20)      229 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/gfa.h
--rw-r--r--   0 gallegoj   (501) staff       (20)     4292 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/robot.h
--rw-r--r--   0 gallegoj   (501) staff       (20)     4314 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/robotGrid.h
--rw-r--r--   0 gallegoj   (501) staff       (20)      636 2021-10-28 22:28:01.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/target.h
--rw-r--r--   0 gallegoj   (501) staff       (20)     1157 2021-10-28 22:28:01.000000 sdss-kaiju-1.4.0b1/python/kaiju/include/utils.h
--rw-r--r--   0 gallegoj   (501) staff       (20)    44501 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/python/kaiju/robotGrid.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     9547 2022-01-04 19:52:25.000000 sdss-kaiju-1.4.0b1/python/kaiju/utils.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.191300 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1020 2024-02-19 05:33:16.000000 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)     1269 2024-02-19 05:33:16.000000 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/SOURCES.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-02-19 05:33:16.000000 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/dependency_links.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)      246 2024-02-19 05:33:16.000000 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/requires.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        6 2024-02-19 05:33:16.000000 sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/top_level.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)      240 2024-02-19 03:06:56.000000 sdss-kaiju-1.4.0b1/requirements.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)       38 2024-02-19 05:33:16.206599 sdss-kaiju-1.4.0b1/setup.cfg
--rw-r--r--   0 gallegoj   (501) staff       (20)     4053 2022-01-26 22:03:16.000000 sdss-kaiju-1.4.0b1/setup.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.160936 sdss-kaiju-1.4.0b1/src/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1134 2021-05-25 19:54:33.000000 sdss-kaiju-1.4.0b1/src/Makefile
--rw-r--r--   0 gallegoj   (501) staff       (20)    11730 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/src/cKaiju.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)    12507 2024-02-19 03:04:52.000000 sdss-kaiju-1.4.0b1/src/conv.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)      214 2021-09-03 21:22:05.000000 sdss-kaiju-1.4.0b1/src/fiducial.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)      212 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/src/gfa.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)      726 2021-05-25 19:54:33.000000 sdss-kaiju-1.4.0b1/src/main.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)    15031 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/src/robot.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)    50832 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/src/robotGrid.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)      714 2021-09-03 21:22:05.000000 sdss-kaiju-1.4.0b1/src/target.cpp
--rw-r--r--   0 gallegoj   (501) staff       (20)    10357 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/src/utils.cpp
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-19 05:33:16.188795 sdss-kaiju-1.4.0b1/tests/
--rw-r--r--   0 gallegoj   (501) staff       (20)      759 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_collide.py
--rw-r--r--   0 gallegoj   (501) staff       (20)      614 2021-12-02 01:58:51.000000 sdss-kaiju-1.4.0b1/tests/test_explode.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     2251 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_fiducial.py
--rw-r--r--   0 gallegoj   (501) staff       (20)      640 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_gfaCollision.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1523 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_initGrid.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1155 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_memory.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1415 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_offlineRobots.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3475 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/tests/test_pathGen.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1578 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_robotGrid.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1081 2021-09-03 21:22:05.000000 sdss-kaiju-1.4.0b1/tests/test_rotGrid.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10242 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/tests/test_rotPath.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     6264 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_target.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1590 2022-10-20 16:03:32.000000 sdss-kaiju-1.4.0b1/tests/test_unevenCBs.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     1458 2021-11-24 16:32:42.000000 sdss-kaiju-1.4.0b1/tests/test_updatedGrids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.938987 sdss_kaiju-1.4.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 05:26:35.938987 sdss_kaiju-1.4.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.930987 sdss_kaiju-1.4.0b2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.930987 sdss_kaiju-1.4.0b2/python/kaiju/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.930987 sdss_kaiju-1.4.0b2/python/kaiju/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/fiducialCoords.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/fps_DesignReference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    49750 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/positionerTable.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/robotGrid.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/robotGrid.js
+-rw-r--r--   0 runner    (1001) docker     (127)    42610 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/etc/wokCoords.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.934987 sdss_kaiju-1.4.0b2/python/kaiju/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/fiducial.h
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/gfa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/robot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/robotGrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/target.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/include/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/robotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/python/kaiju/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.938987 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 05:26:35.000000 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-06 05:26:35.000000 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 05:26:35.000000 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 05:26:35.000000 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 05:26:35.000000 sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 05:26:35.938987 sdss_kaiju-1.4.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.934987 sdss_kaiju-1.4.0b2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/cKaiju.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/fiducial.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/gfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/robot.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/robotGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/target.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/src/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:26:35.938987 sdss_kaiju-1.4.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_collide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_explode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_fiducial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_gfaCollision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_initGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_offlineRobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_pathGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_robotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_rotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_rotPath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_unevenCBs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-06 05:26:07.000000 sdss_kaiju-1.4.0b2/tests/test_updatedGrids.py
```

### Comparing `sdss-kaiju-1.4.0b1/LICENSE.md` & `sdss_kaiju-1.4.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/PKG-INFO` & `sdss_kaiju-1.4.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-kaiju
-Version: 1.4.0b1
+Version: 1.4.0b2
 Summary: Collision Avoidance for SDSS-V Positioners
 Home-page: https://github.com/sdss/kaiju
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD3
 Keywords: astronomy software
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/fiducialCoords.csv` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/fiducialCoords.csv`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/fps_DesignReference.txt` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/fps_DesignReference.txt`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/positionerTable.csv` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/positionerTable.csv`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/robotGrid.html` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/robotGrid.html`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/robotGrid.js` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/robotGrid.js`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/etc/wokCoords.csv` & `sdss_kaiju-1.4.0b2/python/kaiju/etc/wokCoords.csv`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/include/robot.h` & `sdss_kaiju-1.4.0b2/python/kaiju/include/robot.h`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/include/robotGrid.h` & `sdss_kaiju-1.4.0b2/python/kaiju/include/robotGrid.h`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/include/target.h` & `sdss_kaiju-1.4.0b2/python/kaiju/include/target.h`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/include/utils.h` & `sdss_kaiju-1.4.0b2/python/kaiju/include/utils.h`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/robotGrid.py` & `sdss_kaiju-1.4.0b2/python/kaiju/robotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/kaiju/utils.py` & `sdss_kaiju-1.4.0b2/python/kaiju/utils.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/PKG-INFO` & `sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-kaiju
-Version: 1.4.0b1
+Version: 1.4.0b2
 Summary: Collision Avoidance for SDSS-V Positioners
 Home-page: https://github.com/sdss/kaiju
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD3
 Keywords: astronomy software
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sdss-kaiju-1.4.0b1/python/sdss_kaiju.egg-info/SOURCES.txt` & `sdss_kaiju-1.4.0b2/python/sdss_kaiju.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 python/kaiju/utils.py
 python/kaiju/etc/fiducialCoords.csv
 python/kaiju/etc/fps_DesignReference.txt
 python/kaiju/etc/positionerTable.csv
 python/kaiju/etc/robotGrid.html
 python/kaiju/etc/robotGrid.js
 python/kaiju/etc/wokCoords.csv
-python/kaiju/include/coordio.h
 python/kaiju/include/fiducial.h
 python/kaiju/include/gfa.h
 python/kaiju/include/robot.h
 python/kaiju/include/robotGrid.h
 python/kaiju/include/target.h
 python/kaiju/include/utils.h
 python/sdss_kaiju.egg-info/PKG-INFO
 python/sdss_kaiju.egg-info/SOURCES.txt
 python/sdss_kaiju.egg-info/dependency_links.txt
 python/sdss_kaiju.egg-info/requires.txt
 python/sdss_kaiju.egg-info/top_level.txt
 src/Makefile
 src/cKaiju.cpp
-src/conv.cpp
 src/fiducial.cpp
 src/gfa.cpp
 src/main.cpp
 src/robot.cpp
 src/robotGrid.cpp
 src/target.cpp
 src/utils.cpp
```

### Comparing `sdss-kaiju-1.4.0b1/setup.py` & `sdss_kaiju-1.4.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/Makefile` & `sdss_kaiju-1.4.0b2/src/Makefile`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/cKaiju.cpp` & `sdss_kaiju-1.4.0b2/src/cKaiju.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/main.cpp` & `sdss_kaiju-1.4.0b2/src/main.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/robot.cpp` & `sdss_kaiju-1.4.0b2/src/robot.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/robotGrid.cpp` & `sdss_kaiju-1.4.0b2/src/robotGrid.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/target.cpp` & `sdss_kaiju-1.4.0b2/src/target.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/src/utils.cpp` & `sdss_kaiju-1.4.0b2/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_collide.py` & `sdss_kaiju-1.4.0b2/tests/test_collide.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_explode.py` & `sdss_kaiju-1.4.0b2/tests/test_explode.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_fiducial.py` & `sdss_kaiju-1.4.0b2/tests/test_fiducial.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_gfaCollision.py` & `sdss_kaiju-1.4.0b2/tests/test_gfaCollision.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_initGrid.py` & `sdss_kaiju-1.4.0b2/tests/test_initGrid.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_memory.py` & `sdss_kaiju-1.4.0b2/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_offlineRobots.py` & `sdss_kaiju-1.4.0b2/tests/test_offlineRobots.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_pathGen.py` & `sdss_kaiju-1.4.0b2/tests/test_pathGen.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_robotGrid.py` & `sdss_kaiju-1.4.0b2/tests/test_robotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_rotGrid.py` & `sdss_kaiju-1.4.0b2/tests/test_rotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_rotPath.py` & `sdss_kaiju-1.4.0b2/tests/test_rotPath.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_target.py` & `sdss_kaiju-1.4.0b2/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_unevenCBs.py` & `sdss_kaiju-1.4.0b2/tests/test_unevenCBs.py`

 * *Files identical despite different names*

### Comparing `sdss-kaiju-1.4.0b1/tests/test_updatedGrids.py` & `sdss_kaiju-1.4.0b2/tests/test_updatedGrids.py`

 * *Files identical despite different names*

