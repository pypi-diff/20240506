# Comparing `tmp/pyjhtdbv2-20240506.2.tar.gz` & `tmp/pyjhtdbv2-20240506.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjhtdbv2-20240506.2.tar", max compression
+gzip compressed data, was "pyjhtdbv2-20240506.3.tar", max compression
```

## Comparing `pyjhtdbv2-20240506.2.tar` & `pyjhtdbv2-20240506.3.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0    11323 2024-05-05 18:30:57.418257 pyjhtdbv2-20240506.2/LICENSE
--rw-r--r--   0        0        0     3013 2024-05-05 18:30:57.418344 pyjhtdbv2-20240506.2/README.md
--rw-r--r--   0        0        0     2214 2024-05-05 18:30:57.446934 pyjhtdbv2-20240506.2/pyJHTDB/MortonIndex.py
--rw-r--r--   0        0        0     3468 2024-05-05 18:33:04.019377 pyjhtdbv2-20240506.2/pyJHTDB/__init__.py
--rw-r--r--   0        0        0    30030 2024-05-05 18:30:57.447211 pyjhtdbv2-20240506.2/pyJHTDB/data/big_channel_Y_COOR.txt
--rw-r--r--   0        0        0    28495 2024-05-05 18:30:57.447367 pyjhtdbv2-20240506.2/pyJHTDB/data/channel5200_Y_COOR.txt
--rw-r--r--   0        0        0     6272 2024-05-05 18:30:57.447452 pyjhtdbv2-20240506.2/pyJHTDB/data/channel5200_ygrid.npy
--rw-r--r--   0        0        0    34912 2024-05-05 18:30:57.447656 pyjhtdbv2-20240506.2/pyJHTDB/data/channel_grid.h5
--rw-r--r--   0        0        0     8272 2024-05-05 18:30:57.447769 pyjhtdbv2-20240506.2/pyJHTDB/data/channel_xgrid.npy
--rw-r--r--   0        0        0     2128 2024-05-05 18:30:57.447837 pyjhtdbv2-20240506.2/pyJHTDB/data/channel_ygrid.npy
--rw-r--r--   0        0        0     6224 2024-05-05 18:30:57.447924 pyjhtdbv2-20240506.2/pyJHTDB/data/channel_zgrid.npy
--rw-r--r--   0        0        0      418 2024-05-05 18:30:57.447985 pyjhtdbv2-20240506.2/pyJHTDB/data/convert.py
--rw-r--r--   0        0        0     5264 2024-05-05 18:30:57.448055 pyjhtdbv2-20240506.2/pyJHTDB/data/convert2.py
--rw-r--r--   0        0        0     3885 2024-05-05 18:30:57.448117 pyjhtdbv2-20240506.2/pyJHTDB/data/transition_bl_Y_COORD.txt
--rw-r--r--   0        0        0     1024 2024-05-05 18:30:57.448170 pyjhtdbv2-20240506.2/pyJHTDB/data/transition_bl_ygrid.npy
--rw-r--r--   0        0        0     9278 2024-05-05 18:30:57.448292 pyjhtdbv2-20240506.2/pyJHTDB/dbinfo.py
--rw-r--r--   0        0        0    17025 2024-05-05 18:30:57.448438 pyjhtdbv2-20240506.2/pyJHTDB/generic_splines.py
--rw-r--r--   0        0        0    28111 2024-05-05 18:30:57.448596 pyjhtdbv2-20240506.2/pyJHTDB/interpolator.py
--rw-r--r--   0        0        0    21485 2024-05-06 13:36:59.553118 pyjhtdbv2-20240506.2/pyJHTDB/lib/C/local_tools.c
--rw-r--r--   0        0        0      263 2024-05-05 18:30:57.449710 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/.gitignore
--rw-r--r--   0        0        0  1425152 2024-05-05 18:30:57.458863 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelc
--rw-r--r--   0        0        0     6373 2024-05-05 18:30:57.459128 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelc.c
--rw-r--r--   0        0        0  1418832 2024-05-05 18:30:57.467874 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelf
--rw-r--r--   0        0        0    10529 2024-05-05 18:30:57.468245 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelf.f90
--rw-r--r--   0        0        0  1419896 2024-05-05 18:30:57.476559 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutc
--rw-r--r--   0        0        0     3077 2024-05-05 18:30:57.476917 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutc.c
--rw-r--r--   0        0        0  1410800 2024-05-05 18:30:57.488361 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutf
--rw-r--r--   0        0        0     3077 2024-05-05 18:30:57.488702 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutf.f90
--rw-r--r--   0        0        0  1434360 2024-05-05 18:30:57.498329 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdc
--rw-r--r--   0        0        0    17230 2024-05-05 18:30:57.498708 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdc.c
--rw-r--r--   0        0        0  1439312 2024-05-05 18:30:57.515329 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdf
--rw-r--r--   0        0        0    22789 2024-05-05 18:30:57.515727 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdf.f90
--rw-r--r--   0        0        0  1429848 2024-05-05 18:30:57.525002 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingc
--rw-r--r--   0        0        0    13295 2024-05-05 18:30:57.525406 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingc.c
--rw-r--r--   0        0        0  1431120 2024-05-05 18:30:57.533289 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingf
--rw-r--r--   0        0        0    18206 2024-05-05 18:30:57.533621 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingf.f90
--rw-r--r--   0        0        0  1429720 2024-05-05 18:30:57.543054 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbc
--rw-r--r--   0        0        0     9822 2024-05-05 18:30:57.543386 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbc.c
--rw-r--r--   0        0        0  1427024 2024-05-05 18:30:57.551491 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbf
--rw-r--r--   0        0        0    17789 2024-05-05 18:30:57.551773 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbf.f90
--rw-r--r--   0        0        0    11358 2024-05-05 18:30:57.551884 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/LICENSE-2.0.txt
--rw-r--r--   0        0        0     4397 2024-05-05 18:30:57.551952 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/Makefile
--rw-r--r--   0        0        0     3318 2024-05-05 18:30:57.552013 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/README.md
--rw-r--r--   0        0        0   608287 2024-05-05 18:30:57.554891 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/TurbulenceService.h
--rw-r--r--   0        0        0      694 2024-05-05 18:30:57.554997 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/TurbulenceServiceSoap.nsmap
--rw-r--r--   0        0        0  1404135 2024-05-05 18:30:57.573907 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapC.c
--rw-r--r--   0        0        0   286470 2024-05-05 18:30:57.578855 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapClient.c
--rw-r--r--   0        0        0   919477 2024-05-05 18:30:57.583988 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapH.h
--rw-r--r--   0        0        0   317462 2024-05-05 18:30:57.584573 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapStub.h
--rw-r--r--   0        0        0   635235 2024-05-05 18:30:57.585647 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/stdsoap2.c
--rw-r--r--   0        0        0   155733 2024-05-05 18:30:57.586131 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/stdsoap2.h
--rw-r--r--   0        0        0      986 2024-05-05 18:30:57.586206 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/testall
--rw-r--r--   0        0        0    93971 2024-05-05 18:30:57.586415 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/turblib.c
--rw-r--r--   0        0        0    30222 2024-05-05 18:30:57.586514 pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/turblib.h
--rw-r--r--   0        0        0    43272 2024-05-05 18:30:57.448807 pyjhtdbv2-20240506.2/pyJHTDB/libJHTDB.py
--rw-r--r--   0        0        0     1864 2024-05-05 18:30:57.448884 pyjhtdbv2-20240506.2/pyJHTDB/misc.py
--rw-r--r--   0        0        0    37105 2024-05-05 18:30:57.449220 pyjhtdbv2-20240506.2/pyJHTDB/test.py
--rw-r--r--   0        0        0    23795 2024-05-05 18:30:57.449354 pyjhtdbv2-20240506.2/pyJHTDB/test_data.py
--rw-r--r--   0        0        0      983 2024-05-06 13:47:28.841453 pyjhtdbv2-20240506.2/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 pyjhtdbv2-20240506.2/PKG-INFO
+-rw-r--r--   0        0        0    11323 2024-05-05 18:30:57.418257 pyjhtdbv2-20240506.3/LICENSE
+-rw-r--r--   0        0        0     3013 2024-05-05 18:30:57.418344 pyjhtdbv2-20240506.3/README.md
+-rw-r--r--   0        0        0      714 2024-05-06 14:18:44.191338 pyjhtdbv2-20240506.3/build.py
+-rw-r--r--   0        0        0      505 2024-05-06 14:29:11.284954 pyjhtdbv2-20240506.3/meson.build
+-rw-r--r--   0        0        0     2214 2024-05-05 18:30:57.446934 pyjhtdbv2-20240506.3/pyJHTDB/MortonIndex.py
+-rw-r--r--   0        0        0     3468 2024-05-05 18:33:04.019377 pyjhtdbv2-20240506.3/pyJHTDB/__init__.py
+-rw-r--r--   0        0        0    30030 2024-05-05 18:30:57.447211 pyjhtdbv2-20240506.3/pyJHTDB/data/big_channel_Y_COOR.txt
+-rw-r--r--   0        0        0    28495 2024-05-05 18:30:57.447367 pyjhtdbv2-20240506.3/pyJHTDB/data/channel5200_Y_COOR.txt
+-rw-r--r--   0        0        0     6272 2024-05-05 18:30:57.447452 pyjhtdbv2-20240506.3/pyJHTDB/data/channel5200_ygrid.npy
+-rw-r--r--   0        0        0    34912 2024-05-05 18:30:57.447656 pyjhtdbv2-20240506.3/pyJHTDB/data/channel_grid.h5
+-rw-r--r--   0        0        0     8272 2024-05-05 18:30:57.447769 pyjhtdbv2-20240506.3/pyJHTDB/data/channel_xgrid.npy
+-rw-r--r--   0        0        0     2128 2024-05-05 18:30:57.447837 pyjhtdbv2-20240506.3/pyJHTDB/data/channel_ygrid.npy
+-rw-r--r--   0        0        0     6224 2024-05-05 18:30:57.447924 pyjhtdbv2-20240506.3/pyJHTDB/data/channel_zgrid.npy
+-rw-r--r--   0        0        0      418 2024-05-05 18:30:57.447985 pyjhtdbv2-20240506.3/pyJHTDB/data/convert.py
+-rw-r--r--   0        0        0     5264 2024-05-05 18:30:57.448055 pyjhtdbv2-20240506.3/pyJHTDB/data/convert2.py
+-rw-r--r--   0        0        0     3885 2024-05-05 18:30:57.448117 pyjhtdbv2-20240506.3/pyJHTDB/data/transition_bl_Y_COORD.txt
+-rw-r--r--   0        0        0     1024 2024-05-05 18:30:57.448170 pyjhtdbv2-20240506.3/pyJHTDB/data/transition_bl_ygrid.npy
+-rw-r--r--   0        0        0     9278 2024-05-05 18:30:57.448292 pyjhtdbv2-20240506.3/pyJHTDB/dbinfo.py
+-rw-r--r--   0        0        0    17025 2024-05-05 18:30:57.448438 pyjhtdbv2-20240506.3/pyJHTDB/generic_splines.py
+-rw-r--r--   0        0        0    28111 2024-05-05 18:30:57.448596 pyjhtdbv2-20240506.3/pyJHTDB/interpolator.py
+-rw-r--r--   0        0        0    21485 2024-05-06 13:36:59.553118 pyjhtdbv2-20240506.3/pyJHTDB/lib/C/local_tools.c
+-rw-r--r--   0        0        0      263 2024-05-05 18:30:57.449710 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/.gitignore
+-rw-r--r--   0        0        0  1425152 2024-05-05 18:30:57.458863 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelc
+-rw-r--r--   0        0        0     6373 2024-05-05 18:30:57.459128 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelc.c
+-rw-r--r--   0        0        0  1418832 2024-05-05 18:30:57.467874 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelf
+-rw-r--r--   0        0        0    10529 2024-05-05 18:30:57.468245 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelf.f90
+-rw-r--r--   0        0        0  1419896 2024-05-05 18:30:57.476559 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutc
+-rw-r--r--   0        0        0     3077 2024-05-05 18:30:57.476917 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutc.c
+-rw-r--r--   0        0        0  1410800 2024-05-05 18:30:57.488361 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutf
+-rw-r--r--   0        0        0     3077 2024-05-05 18:30:57.488702 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutf.f90
+-rw-r--r--   0        0        0  1434360 2024-05-05 18:30:57.498329 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdc
+-rw-r--r--   0        0        0    17230 2024-05-05 18:30:57.498708 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdc.c
+-rw-r--r--   0        0        0  1439312 2024-05-05 18:30:57.515329 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdf
+-rw-r--r--   0        0        0    22789 2024-05-05 18:30:57.515727 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdf.f90
+-rw-r--r--   0        0        0  1429848 2024-05-05 18:30:57.525002 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingc
+-rw-r--r--   0        0        0    13295 2024-05-05 18:30:57.525406 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingc.c
+-rw-r--r--   0        0        0  1431120 2024-05-05 18:30:57.533289 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingf
+-rw-r--r--   0        0        0    18206 2024-05-05 18:30:57.533621 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingf.f90
+-rw-r--r--   0        0        0  1429720 2024-05-05 18:30:57.543054 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbc
+-rw-r--r--   0        0        0     9822 2024-05-05 18:30:57.543386 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbc.c
+-rw-r--r--   0        0        0  1427024 2024-05-05 18:30:57.551491 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbf
+-rw-r--r--   0        0        0    17789 2024-05-05 18:30:57.551773 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbf.f90
+-rw-r--r--   0        0        0    11358 2024-05-05 18:30:57.551884 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/LICENSE-2.0.txt
+-rw-r--r--   0        0        0     4397 2024-05-05 18:30:57.551952 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/Makefile
+-rw-r--r--   0        0        0     3318 2024-05-05 18:30:57.552013 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/README.md
+-rw-r--r--   0        0        0   608287 2024-05-05 18:30:57.554891 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/TurbulenceService.h
+-rw-r--r--   0        0        0      694 2024-05-05 18:30:57.554997 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/TurbulenceServiceSoap.nsmap
+-rw-r--r--   0        0        0  1404135 2024-05-05 18:30:57.573907 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapC.c
+-rw-r--r--   0        0        0   286470 2024-05-05 18:30:57.578855 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapClient.c
+-rw-r--r--   0        0        0   919477 2024-05-05 18:30:57.583988 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapH.h
+-rw-r--r--   0        0        0   317462 2024-05-05 18:30:57.584573 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapStub.h
+-rw-r--r--   0        0        0   635235 2024-05-05 18:30:57.585647 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/stdsoap2.c
+-rw-r--r--   0        0        0   155733 2024-05-05 18:30:57.586131 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/stdsoap2.h
+-rw-r--r--   0        0        0      986 2024-05-05 18:30:57.586206 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/testall
+-rw-r--r--   0        0        0    93971 2024-05-05 18:30:57.586415 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/turblib.c
+-rw-r--r--   0        0        0    30222 2024-05-05 18:30:57.586514 pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/turblib.h
+-rw-r--r--   0        0        0    43272 2024-05-05 18:30:57.448807 pyjhtdbv2-20240506.3/pyJHTDB/libJHTDB.py
+-rw-r--r--   0        0        0     1864 2024-05-05 18:30:57.448884 pyjhtdbv2-20240506.3/pyJHTDB/misc.py
+-rw-r--r--   0        0        0    37105 2024-05-05 18:30:57.449220 pyjhtdbv2-20240506.3/pyJHTDB/test.py
+-rw-r--r--   0        0        0    23795 2024-05-05 18:30:57.449354 pyjhtdbv2-20240506.3/pyJHTDB/test_data.py
+-rw-r--r--   0        0        0     1192 2024-05-06 14:29:42.066100 pyjhtdbv2-20240506.3/pyproject.toml
+-rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 pyjhtdbv2-20240506.3/PKG-INFO
```

### Comparing `pyjhtdbv2-20240506.2/LICENSE` & `pyjhtdbv2-20240506.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/README.md` & `pyjhtdbv2-20240506.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/MortonIndex.py` & `pyjhtdbv2-20240506.3/pyJHTDB/MortonIndex.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/__init__.py` & `pyjhtdbv2-20240506.3/pyJHTDB/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/big_channel_Y_COOR.txt` & `pyjhtdbv2-20240506.3/pyJHTDB/data/big_channel_Y_COOR.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel5200_Y_COOR.txt` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel5200_Y_COOR.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel5200_ygrid.npy` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel5200_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel_grid.h5` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel_grid.h5`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel_xgrid.npy` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel_xgrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel_ygrid.npy` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/channel_zgrid.npy` & `pyjhtdbv2-20240506.3/pyJHTDB/data/channel_zgrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/convert2.py` & `pyjhtdbv2-20240506.3/pyJHTDB/data/convert2.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/transition_bl_Y_COORD.txt` & `pyjhtdbv2-20240506.3/pyJHTDB/data/transition_bl_Y_COORD.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/data/transition_bl_ygrid.npy` & `pyjhtdbv2-20240506.3/pyJHTDB/data/transition_bl_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/dbinfo.py` & `pyjhtdbv2-20240506.3/pyJHTDB/dbinfo.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/generic_splines.py` & `pyjhtdbv2-20240506.3/pyJHTDB/generic_splines.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/interpolator.py` & `pyjhtdbv2-20240506.3/pyJHTDB/interpolator.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/C/local_tools.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/C/local_tools.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelc` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelc`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelc.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelc.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelf` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelf`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_channelf.f90` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_channelf.f90`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutc` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutc`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutc.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutc.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutf` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutf`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_getCutoutf.f90` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_getCutoutf.f90`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdc` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdc`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdc.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdc.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdf` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdf`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mhdf.f90` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mhdf.f90`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingc` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingc`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingc.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingc.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingf` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingf`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_mixingf.f90` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_mixingf.f90`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbc` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbc`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbc.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbc.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbf` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbf`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/DEMO_turbf.f90` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/DEMO_turbf.f90`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/LICENSE-2.0.txt` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/Makefile` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/Makefile`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/README.md` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/README.md`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/TurbulenceService.h` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/TurbulenceService.h`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/TurbulenceServiceSoap.nsmap` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/TurbulenceServiceSoap.nsmap`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapC.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapC.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapClient.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapClient.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapH.h` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapH.h`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/soapStub.h` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/soapStub.h`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/stdsoap2.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/stdsoap2.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/stdsoap2.h` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/stdsoap2.h`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/testall` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/testall`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/turblib.c` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/turblib.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/lib/turblib/turblib.h` & `pyjhtdbv2-20240506.3/pyJHTDB/lib/turblib/turblib.h`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/libJHTDB.py` & `pyjhtdbv2-20240506.3/pyJHTDB/libJHTDB.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/misc.py` & `pyjhtdbv2-20240506.3/pyJHTDB/misc.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/test.py` & `pyjhtdbv2-20240506.3/pyJHTDB/test.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyJHTDB/test_data.py` & `pyjhtdbv2-20240506.3/pyJHTDB/test_data.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20240506.2/pyproject.toml` & `pyjhtdbv2-20240506.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 [tool.poetry]
 name = "pyjhtdbv2"
-version = "20240506.2"
+version = "20240506.3"
 description = "Python wrapper for the Johns Hopkins turbulence database library"
 authors = ["Johns Hopkins Turbulence Database Group <turbulence@pha.jhu.edu>"]
 license = "Apache License 2.0"
 packages = [
     { include = "pyJHTDB", from = "." },
 ]
 readme = "README.md"
 include = [
     {path = "pyJHTDB/data/channel_xgrid.npy"},
     {path = "pyJHTDB/data/channel_ygrid.npy"},
     {path = "pyJHTDB/data/channel_zgrid.npy"},
     {path = "pyJHTDB/data/channel5200_ygrid.npy"},
     {path = "pyJHTDB/data/transition_bl_ygrid.npy"},
-    {path = "pyJHTDB/lib/**/*.so", format = "wheel"}
+    { path = "meson.build", format = "sdist" },
+    { path = "pendulum/lib/*.so", format = "wheel" },
+    { path = "pendulum/lib/*.pyd", format = "wheel" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 numpy = ">=1.15.0"
 scipy = ">=1.1.0"
 sympy = ">=1.2"
 h5py = ">=2.8.0"
 matplotlib = ">=3.0.0"
 wurlitzer = ">=2.0.2"
 
+[tool.poetry.group.build]
+optional = true
+
+[tool.poetry.group.build.dependencies]
+meson = "^0.63.2"
+ninja = "^1.10.2.3"
 
 [build-system]
-requires = ["poetry-core", "setuptools"]
+requires = ["poetry-core", "meson", "ninja"]
 build-backend = "poetry.core.masonry.api"
 
-# 2 pass build
-# [tool.poetry.build]
-# script = "build.py"
-# generate-setup-file = true
+[tool.poetry.build]
+generate-setup-file = false
+script = "build.py"
```

### Comparing `pyjhtdbv2-20240506.2/PKG-INFO` & `pyjhtdbv2-20240506.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyjhtdbv2
-Version: 20240506.2
+Version: 20240506.3
 Summary: Python wrapper for the Johns Hopkins turbulence database library
 License: Apache-2.0
 Author: Johns Hopkins Turbulence Database Group
 Author-email: turbulence@pha.jhu.edu
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5py (>=2.8.0)
```
