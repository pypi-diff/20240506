# Comparing `tmp/python_seispy-1.3.6.tar.gz` & `tmp/python_seispy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_seispy-1.3.6.tar", last modified: Thu Apr 25 01:36:58 2024, max compression
+gzip compressed data, was "python_seispy-1.3.7.tar", last modified: Mon May  6 16:09:15 2024, max compression
```

## Comparing `python_seispy-1.3.6.tar` & `python_seispy-1.3.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-25 01:36:50.000000 python_seispy-1.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-25 01:36:58.453385 python_seispy-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-25 01:36:50.000000 python_seispy-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/python_seispy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.445385 python_seispy-1.3.6/seispy/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccp3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccppara.py
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccpprofile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.445385 python_seispy-1.3.6/seispy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/RFStation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/depmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/pertmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.449385 python_seispy-1.3.6/seispy/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)  2645806 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/EventCMT.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/ak135.vel
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/cmpVsVp.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/cyan.mat
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/iasp91.vel
--rwxr-xr-x   0 runner    (1001) docker     (127)      875 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/mtna.vel
--rwxr-xr-x   0 runner    (1001) docker     (127)     3696 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/prem.vel
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/saveicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    58484 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/seispy.png
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/decon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/distaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/eq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/get_cpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/hk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/hkpara.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/mccc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/modcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/para.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickdepth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/get_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/pickdepthui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickrf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/pickfigure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/pickui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/rpickfigure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickseis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickseis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickseis/sviewerui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/plotR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/plotRT.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/psrayp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/recalrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rf2depth_makedata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16742 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rfani.py
--rw-r--r--   0 runner    (1001) docker     (127)    43094 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rfcorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/seisfwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/setuplog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/slantstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:36:58.453385 python_seispy-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-25 01:36:50.000000 python_seispy-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case03.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case04.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.816999 python_seispy-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 16:09:07.000000 python_seispy-1.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-06 16:09:15.816999 python_seispy-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-06 16:09:07.000000 python_seispy-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.816999 python_seispy-1.3.7/python_seispy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 16:09:15.000000 python_seispy-1.3.7/python_seispy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.808999 python_seispy-1.3.7/seispy/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/ccp3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/ccppara.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/ccpprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.808999 python_seispy-1.3.7/seispy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/core/RFStation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/core/depmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/core/pertmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.812999 python_seispy-1.3.7/seispy/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2645806 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/EventCMT.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/ak135.vel
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/cmpVsVp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/cyan.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/iasp91.vel
+-rwxr-xr-x   0 runner    (1001) docker     (127)      875 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/mtna.vel
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3696 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/prem.vel
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/saveicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58484 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/data/seispy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/decon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/distaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25271 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/get_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/hk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/hkpara.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/mccc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/modcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/para.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.812999 python_seispy-1.3.7/seispy/pickdepth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickdepth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickdepth/get_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickdepth/pickdepthui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.816999 python_seispy-1.3.7/seispy/pickrf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickrf/pickfigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickrf/pickui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickrf/rpickfigure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.816999 python_seispy-1.3.7/seispy/pickseis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickseis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/pickseis/sviewerui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/plotR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/plotRT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/psrayp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/recalrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/rf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/rf2depth_makedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16742 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/rfani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43094 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/rfcorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/seisfwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/setuplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/slantstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-06 16:09:07.000000 python_seispy-1.3.7/seispy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:09:15.816999 python_seispy-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-06 16:09:07.000000 python_seispy-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:15.816999 python_seispy-1.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-06 16:09:07.000000 python_seispy-1.3.7/test/test_case01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-06 16:09:07.000000 python_seispy-1.3.7/test/test_case02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-06 16:09:07.000000 python_seispy-1.3.7/test/test_case03.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 16:09:07.000000 python_seispy-1.3.7/test/test_case04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-06 16:09:07.000000 python_seispy-1.3.7/test/test_case05.py
```

### Comparing `python_seispy-1.3.6/LICENSE.txt` & `python_seispy-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/PKG-INFO` & `python_seispy-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-seispy
-Version: 1.3.6
+Version: 1.3.7
 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.6 Author: Mijian Xu
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.7 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE.txt Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.9.1
 Requires-Dist: matplotlib>=3.5.0 Requires-Dist: pandas>=1.0.0 Requires-Dist:
 obspy>=1.2.1 Requires-Dist: pyside6>=6.2.0 Requires-Dist:
```

### Comparing `python_seispy-1.3.6/README.md` & `python_seispy-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/python_seispy.egg-info/PKG-INFO` & `python_seispy-1.3.7/python_seispy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-seispy
-Version: 1.3.6
+Version: 1.3.7
 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.6 Author: Mijian Xu
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.7 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE.txt Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.9.1
 Requires-Dist: matplotlib>=3.5.0 Requires-Dist: pandas>=1.0.0 Requires-Dist:
 obspy>=1.2.1 Requires-Dist: pyside6>=6.2.0 Requires-Dist:
```

### Comparing `python_seispy-1.3.6/python_seispy.egg-info/SOURCES.txt` & `python_seispy-1.3.7/python_seispy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/python_seispy.egg-info/entry_points.txt` & `python_seispy-1.3.7/python_seispy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/catalog.py` & `python_seispy-1.3.7/seispy/catalog.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/ccp3d.py` & `python_seispy-1.3.7/seispy/ccp3d.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/ccppara.py` & `python_seispy-1.3.7/seispy/ccppara.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/ccpprofile.py` & `python_seispy-1.3.7/seispy/ccpprofile.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/core/RFStation.py` & `python_seispy-1.3.7/seispy/core/RFStation.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/core/depmodel.py` & `python_seispy-1.3.7/seispy/core/depmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import glob
 from os.path import exists, join, dirname
 import numpy as np
 from matplotlib import pyplot as plt
 from scipy.interpolate import interp1d, interpn
-
 from seispy.utils import vs2vprho
+import warnings
+
+warnings.filterwarnings("ignore", "invalid value encountered in sqrt")
 
 
 def _search_vel_file(mode_name):
     """
     search vel file given by mode_name
         and try to open it with np.loadtxt:
```

### Comparing `python_seispy-1.3.6/seispy/core/pertmod.py` & `python_seispy-1.3.7/seispy/core/pertmod.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class Mod3DPerturbation:
     """ 
     Perturbation model for 3D velocity model.
     """   
     def __init__(self, modpath, YAxisRange, velmod='iasp91'):
         dep_mod = DepModel(YAxisRange, velmod=velmod)
         self.model = np.load(modpath)
-        new1dvp = interp1d(dep_mod.depthsraw, dep_mod.vpraw)(self.model['dep'])
-        new1dvs = interp1d(dep_mod.depthsraw, dep_mod.vsraw)(self.model['dep'])
+        new1dvp = interp1d(dep_mod.depths, dep_mod.vp)(self.model['dep'])
+        new1dvs = interp1d(dep_mod.depths, dep_mod.vs)(self.model['dep'])
         new1dvp, _, _ = np.meshgrid(new1dvp, self.model['lat'], self.model['lon'], indexing='ij')
         new1dvs, _, _ = np.meshgrid(new1dvs, self.model['lat'], self.model['lon'], indexing='ij')
         self.dvp = (self.model['vp'] - new1dvp) / new1dvp
         self.dvs = (self.model['vs'] - new1dvs) / new1dvs
         self.cvp = dep_mod.vp
         self.cvs = dep_mod.vs
```

### Comparing `python_seispy-1.3.6/seispy/data/EventCMT.dat` & `python_seispy-1.3.7/seispy/data/EventCMT.dat`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/cmpVsVp.txt` & `python_seispy-1.3.7/seispy/data/cmpVsVp.txt`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/cyan.mat` & `python_seispy-1.3.7/seispy/data/cyan.mat`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/iasp91.vel` & `python_seispy-1.3.7/seispy/data/iasp91.vel`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/mtna.vel` & `python_seispy-1.3.7/seispy/data/mtna.vel`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/prem.vel` & `python_seispy-1.3.7/seispy/data/prem.vel`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/saveicon.png` & `python_seispy-1.3.7/seispy/data/saveicon.png`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/data/seispy.png` & `python_seispy-1.3.7/seispy/data/seispy.png`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/decon.py` & `python_seispy-1.3.7/seispy/decon.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/distaz.py` & `python_seispy-1.3.7/seispy/distaz.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/eq.py` & `python_seispy-1.3.7/seispy/eq.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,25 +186,24 @@
         :param evdp: focal depth
         :type evdp: float
         :param dis: epicentral distance
         :type dis: float
         :param phase: phase name, defaults to 'P'
         :type phase: str, optional
         """
+        self.phase = phase
         arrivals = model.get_travel_times(evdp, dis, phase_list=[phase])
         if not arrivals:
-            raise ValueError('The phase of {} is not exists'.format(phase))
-        if len(arrivals) > 1:
-            raise ValueError('More than one phase were calculated with distance of {} and focal depth of {}'.format(dis, evdp))
-        else:
-            # self.arrival = arrivals[0]
-            self.arr_time = arrivals[0].time
-            self.rayp = arrivals[0].ray_param
-            self.inc = arrivals[0].incident_angle
-            self.phase = phase
+            raise ValueError('The phase of {} is not exists. Please check the setting of distance and phase'.format(phase))
+        # if len(arrivals) > 1:
+        #     raise ValueError('More than one phase were calculated with distance of {} and focal depth of {}'.format(dis, evdp))
+        # else:
+        self.arr_time = arrivals[0].time
+        self.rayp = arrivals[0].ray_param
+        self.inc = arrivals[0].incident_angle
 
     def search_inc(self, bazi):
         """Search incident angle for S wave
 
         :param bazi: back azimuth
         :type bazi: float
         :return: incident angle
```

### Comparing `python_seispy-1.3.6/seispy/geo.py` & `python_seispy-1.3.7/seispy/geo.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/get_cpt.py` & `python_seispy-1.3.7/seispy/get_cpt.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/harmonics.py` & `python_seispy-1.3.7/seispy/harmonics.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/hk.py` & `python_seispy-1.3.7/seispy/hk.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/hkpara.py` & `python_seispy-1.3.7/seispy/hkpara.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/io.py` & `python_seispy-1.3.7/seispy/io.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/mccc.py` & `python_seispy-1.3.7/seispy/mccc.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/modcreator.py` & `python_seispy-1.3.7/seispy/modcreator.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/para.py` & `python_seispy-1.3.7/seispy/para.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickdepth/get_depth.py` & `python_seispy-1.3.7/seispy/pickdepth/get_depth.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickdepth/pickdepthui.py` & `python_seispy-1.3.7/seispy/pickdepth/pickdepthui.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickrf/pickfigure.py` & `python_seispy-1.3.7/seispy/pickrf/pickfigure.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickrf/pickui.py` & `python_seispy-1.3.7/seispy/pickrf/pickui.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickrf/rpickfigure.py` & `python_seispy-1.3.7/seispy/pickrf/rpickfigure.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/pickseis/sviewerui.py` & `python_seispy-1.3.7/seispy/pickseis/sviewerui.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/plotR.py` & `python_seispy-1.3.7/seispy/plotR.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/plotRT.py` & `python_seispy-1.3.7/seispy/plotRT.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/psrayp.py` & `python_seispy-1.3.7/seispy/psrayp.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/recalrf.py` & `python_seispy-1.3.7/seispy/recalrf.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/rf.py` & `python_seispy-1.3.7/seispy/rf.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/rf2depth_makedata.py` & `python_seispy-1.3.7/seispy/rf2depth_makedata.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/rfani.py` & `python_seispy-1.3.7/seispy/rfani.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/rfcorrect.py` & `python_seispy-1.3.7/seispy/rfcorrect.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/scripts.py` & `python_seispy-1.3.7/seispy/scripts.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/seisfwd.py` & `python_seispy-1.3.7/seispy/seisfwd.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/setuplog.py` & `python_seispy-1.3.7/seispy/setuplog.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/signal.py` & `python_seispy-1.3.7/seispy/signal.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/slantstack.py` & `python_seispy-1.3.7/seispy/slantstack.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/seispy/utils.py` & `python_seispy-1.3.7/seispy/utils.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/setup.py` & `python_seispy-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 packages = find_packages()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "1.3.6"
+VERSION = "1.3.7"
 setup(name='python-seispy',
       version=VERSION,
       author='Mijian Xu',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author_email='gomijianxu@gmail.com',
       license='GPLv3',
```

### Comparing `python_seispy-1.3.6/test/test_case01.py` & `python_seispy-1.3.7/test/test_case01.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/test/test_case02.py` & `python_seispy-1.3.7/test/test_case02.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/test/test_case03.py` & `python_seispy-1.3.7/test/test_case03.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/test/test_case04.py` & `python_seispy-1.3.7/test/test_case04.py`

 * *Files identical despite different names*

### Comparing `python_seispy-1.3.6/test/test_case05.py` & `python_seispy-1.3.7/test/test_case05.py`

 * *Files identical despite different names*

